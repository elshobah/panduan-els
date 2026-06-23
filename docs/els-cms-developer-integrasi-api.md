---
description: Panduan developer untuk mengintegrasikan data artikel ElsCMS (Directus) ke website frontend via REST API — autentikasi, struktur data, query, dan contoh kode.
---

# Integrasi API ElsCMS untuk Developer

Panduan ini ditujukan untuk **developer** yang ingin mengambil data artikel dari **ElsCMS** (`https://cms.elshobah.com`) dan menampilkannya di website frontend (Next.js, React, PHP, atau stack apa pun yang bisa melakukan HTTP request).

ElsCMS dibangun di atas **Directus** dan bersifat **multi-tenant** — satu instance CMS melayani banyak website sekaligus. Setiap data (artikel, kategori, tag, menu, pengaturan situs) dipisahkan per website lewat field `tenant_id`.

{% hint style="warning" %}
**Wajib filter `tenant_id`.** Semua query ke collection `posts`, `categories`, `tags`, `menus`, dan `site_settings` **harus** menyertakan filter `tenant_id` sesuai website Anda. Tanpa filter ini, response API bisa berisi data milik tenant/website lain.
{% endhint %}

---

## Prasyarat

- **Base URL:** `https://cms.elshobah.com`
- **Tenant ID** website Anda — minta ke tim Elshobah Developer jika belum punya
- **Access Token** (Static Token atau hasil login) untuk request yang membutuhkan autentikasi

---

## 1. Autentikasi

ElsCMS mendukung dua cara autentikasi REST API Directus:

### a. Static Access Token (disarankan untuk server-side / build-time fetch)

Sertakan token di header setiap request:

```
Authorization: Bearer <STATIC_ACCESS_TOKEN>
```

### b. Login Email/Password (untuk kebutuhan dinamis/server backend)

```bash
curl -X POST https://cms.elshobah.com/auth/login \
  -H "Content-Type: application/json" \
  -d '{"email": "developer@example.com", "password": "********"}'
```

Response berisi `access_token` dan `refresh_token` yang dipakai untuk request berikutnya.

{% hint style="danger" %}
**Jangan expose token di client-side (browser)** kecuali endpoint memang dikonfigurasi sebagai public-read. Simpan token di environment variable (`.env`) dan lakukan fetch dari server (SSR/API route), bukan langsung dari browser.
{% endhint %}

---

## 2. Struktur Data Artikel (Collection `posts`)

### Field utama — `posts`

| Field | Tipe | Keterangan |
|-------|------|-----------|
| `id` | uuid | Primary key |
| `tenant_id` | uuid (relasi → `tenants`) | **Wajib difilter** sesuai website Anda |
| `slug` | string | URL slug, unik per tenant |
| `status` | string | `draft`, `published`, `scheduled`, `archived` |
| `published_at` | timestamp | Tanggal publikasi (cek juga jika status `scheduled`) |
| `featured_image` | uuid (relasi → `directus_files`) | Gambar utama artikel |
| `author` | uuid (relasi → `directus_users`) | Penulis |
| `categories` | uuid (relasi → `categories`) | Satu kategori per artikel |
| `post_tags` | relasi m2m → `tags` (via `posts_tags`) | Tag artikel (bisa lebih dari satu) |
| `tags` | uuid (relasi → `tags`) | ⚠️ **Deprecated** — gunakan `post_tags` |
| `translations` | o2m → `posts_translations` | Konten artikel per bahasa |

### Field terjemahan — `posts_translations`

| Field | Tipe | Keterangan |
|-------|------|-----------|
| `languages_code` | string | Kode bahasa, contoh `id-ID`, `en-US` |
| `title` | string | Judul artikel |
| `excerpt` | text | Ringkasan untuk preview & fallback meta description |
| `content` | text (HTML) | Isi artikel lengkap (rich text HTML) |
| `seo_title` | string | Judul SEO (≤ 60 karakter) |
| `seo_description` | text | Meta description SEO (≤ 160 karakter) |

### Collection terkait

| Collection | Keterangan |
|-----------|-----------|
| `categories` / `categories_translations` | `slug`, `status`, `name` + terjemahan per `languages_code` |
| `tags` / `tags_translations` | `slug`, `status`, `name` + terjemahan (field lama `Nama` sudah deprecated) |
| `directus_files` | Metadata file/gambar — dipakai untuk resolve URL `featured_image` |

---

## 3. Mengambil Daftar Artikel

```
GET /items/posts
```

**Contoh query lengkap** (artikel published milik tenant Anda, lengkap dengan translasi, kategori, dan tag):

```
GET https://cms.elshobah.com/items/posts
  ?filter[tenant_id][_eq]=<TENANT_ID>
  &filter[status][_eq]=published
  &fields=id,slug,status,published_at,featured_image,categories.name,post_tags.tags_id.name,translations.languages_code,translations.title,translations.excerpt,translations.seo_title
  &sort=-published_at
  &limit=10
  &page=1
```

Versi `curl`:

```bash
curl "https://cms.elshobah.com/items/posts?filter[tenant_id][_eq]=<TENANT_ID>&filter[status][_eq]=published&fields=id,slug,published_at,featured_image,translations.title,translations.excerpt&sort=-published_at&limit=10" \
  -H "Authorization: Bearer <ACCESS_TOKEN>"
```

**Contoh response** (struktur nyata, disederhanakan):

```json
{
  "data": [
    {
      "id": "078272d8-e6be-4d32-a122-08aa392d8a17",
      "slug": "bahan-aktif-wajib-meracik-formula-skincare",
      "status": "published",
      "published_at": "2026-05-13T08:00:00.000Z",
      "featured_image": "01e96bd0-db47-46fd-9e12-bd426dcc8b59",
      "categories": { "name": "Skincare" },
      "post_tags": [],
      "translations": [
        {
          "languages_code": "id-ID",
          "title": "Mengenal Bahan Aktif Wajib sebelum Belajar Meracik Formula Skincare",
          "excerpt": "Sebelum mulai meracik formula skincare sendiri, kamu perlu mengenal bahan-bahan aktif utama yang sering digunakan...",
          "seo_title": "Bahan Aktif Wajib dalam Meracik Formula Skincare | Panduan Lengkap"
        }
      ]
    }
  ]
}
```

### Pagination

Gunakan `limit` dan `page` (atau `offset`) untuk memuat data secara bertahap:

```
&limit=10&page=2
```

---

## 4. Mengambil Detail Artikel by Slug

```
GET https://cms.elshobah.com/items/posts
  ?filter[tenant_id][_eq]=<TENANT_ID>
  &filter[slug][_eq]=bahan-aktif-wajib-meracik-formula-skincare
  &filter[status][_eq]=published
  &fields=*,translations.*,categories.name,post_tags.tags_id.name,featured_image
```

Karena `slug` unik per tenant (bukan global), filter `tenant_id` tetap wajib disertakan.

---

## 5. Menampilkan Gambar (Featured Image)

`featured_image` hanya berisi **ID file** (uuid). Untuk menampilkan gambar, gunakan endpoint assets Directus:

```
https://cms.elshobah.com/assets/<FILE_ID>
```

Directus juga mendukung transformasi gambar on-the-fly lewat query parameter:

```
https://cms.elshobah.com/assets/<FILE_ID>?width=800&format=webp&quality=80
```

{% hint style="info" %}
Parameter transformasi yang umum: `width`, `height`, `fit` (`cover`/`contain`/`inside`/`outside`), `format` (`webp`/`avif`/`jpg`/`png`), `quality` (1–100).
{% endhint %}

---

## 6. Multi-bahasa

Setiap artikel bisa punya beberapa baris di `posts_translations`, satu per `languages_code`. Untuk mengambil konten dalam bahasa tertentu saja, filter di level `deep`:

```
GET https://cms.elshobah.com/items/posts
  ?filter[tenant_id][_eq]=<TENANT_ID>
  &fields=id,slug,translations.title,translations.content
  &deep[translations][_filter][languages_code][_eq]=id-ID
```

---

## 7. Contoh Kode

### JavaScript (`fetch`)

```javascript
async function getLatestPosts(tenantId, lang = "id-ID") {
  const url = new URL("https://cms.elshobah.com/items/posts");
  url.searchParams.set("filter[tenant_id][_eq]", tenantId);
  url.searchParams.set("filter[status][_eq]", "published");
  url.searchParams.set(
    "fields",
    "id,slug,published_at,featured_image,categories.name,translations.title,translations.excerpt"
  );
  url.searchParams.set("sort", "-published_at");
  url.searchParams.set("limit", "10");
  url.searchParams.set("deep[translations][_filter][languages_code][_eq]", lang);

  const res = await fetch(url, {
    headers: { Authorization: `Bearer ${process.env.ELSCMS_TOKEN}` },
  });

  if (!res.ok) throw new Error(`ElsCMS API error: ${res.status}`);
  const { data } = await res.json();
  return data;
}
```

### cURL — artikel terbaru

```bash
curl "https://cms.elshobah.com/items/posts?filter[tenant_id][_eq]=<TENANT_ID>&filter[status][_eq]=published&sort=-published_at&limit=5" \
  -H "Authorization: Bearer <ACCESS_TOKEN>"
```

---

## Catatan Penting

- ⚠️ Field `tags` di collection `posts` **sudah deprecated** — gunakan relasi `post_tags` untuk multi-tag.
- ⚠️ Selalu filter `tenant_id` di setiap request — kelalaian di sini berisiko membocorkan data antar website.
- ⚠️ Artikel berstatus `scheduled` belum berarti tayang — cek juga `published_at` di sisi frontend/cache bila perlu menampilkan jadwal publikasi mendatang.
- Gunakan parameter `fields` untuk membatasi data yang diambil (hindari `fields=*` di production agar response lebih ringan).

---

## Checklist Integrasi

- [ ] Token akses (Static Token atau login) sudah didapat dan disimpan di environment variable
- [ ] `tenant_id` website sudah dikonfirmasi ke tim Elshobah Developer
- [ ] Query daftar artikel sudah difilter `tenant_id` + `status=published`
- [ ] URL gambar `featured_image` di-resolve lewat endpoint `/assets/:id`
- [ ] Penanganan multi-bahasa (jika website multilingual) sudah diuji
- [ ] Token tidak diekspos ke client-side bila bukan endpoint public-read

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS · Diperbarui: 23 Juni 2026*
