---
description: Panduan membuat dan mempublikasikan artikel di ElsCMS (Directus) — dari judul, konten, gambar utama, kategori, tag, hingga pengaturan SEO.
---

# Cara Membuat Artikel di ElsCMS

Panduan ini menjelaskan cara membuat artikel baru di **ElsCMS** — sistem manajemen konten berbasis Directus yang digunakan untuk mengelola artikel, berita, dan blog di website Anda.

---

## Prasyarat

Sebelum membuat artikel, pastikan:

- Anda sudah memiliki akses ke dashboard ElsCMS
- Anda sudah login sebagai user dengan role yang memiliki izin membuat post

---

## Langkah-Langkah

### 1. Buka Koleksi Posts

Di sidebar kiri dashboard ElsCMS, klik menu **Posts**.

Anda akan melihat daftar artikel yang sudah ada.

### 2. Buat Artikel Baru

Klik tombol **"+"** atau **"Create Item"** di pojok kanan atas untuk membuat artikel baru.

---

### 3. Isi Informasi Utama Artikel

Di bagian atas form, isi field-field berikut:

| Field | Keterangan | Wajib |
|-------|-----------|-------|
| **Status** | Pilih `draft` saat mengerjakan, `published` saat siap tayang, `archived` untuk arsip | Ya |
| **Slug** | URL artikel — gunakan huruf kecil, kata dipisah tanda hubung (`-`). Contoh: `tips-digital-marketing` | Disarankan |
| **Featured Image** | Gambar utama/thumbnail artikel | Disarankan |
| **Author** | Penulis artikel — pilih dari daftar user | Opsional |
| **Published At** | Tanggal dan waktu publikasi — isi jika ingin menjadwalkan | Opsional |

{% hint style="info" %}
**Slug** harus unik untuk setiap website. Hindari menggunakan karakter khusus, spasi, atau huruf kapital.
{% endhint %}

---

### 4. Isi Konten Artikel (Translations)

Klik tab **Translations** atau section **id-ID** (Bahasa Indonesia) untuk mengisi konten utama artikel.

| Field | Keterangan | Wajib |
|-------|-----------|-------|
| **Title** | Judul artikel yang tampil di website | Ya |
| **Excerpt** | Ringkasan singkat artikel — digunakan untuk preview di halaman daftar artikel dan meta SEO | Disarankan |
| **Content** | Isi lengkap artikel — menggunakan editor rich text (WYSIWYG) | Opsional |
| **SEO Title** | Judul khusus untuk mesin pencari — maksimal **60 karakter** | Opsional |
| **SEO Description** | Deskripsi meta untuk Google — maksimal **160 karakter** | Opsional |

{% hint style="success" %}
**Tips SEO:**
- **SEO Title** — tulis ulang judul agar lebih menarik di hasil pencarian Google. Pastikan mengandung kata kunci utama.
- **SEO Description** — ringkasan yang muncul di bawah judul di Google. Buat kalimat yang mendorong pengunjung untuk klik.
- **Excerpt** — jika SEO Description kosong, excerpt sering digunakan sebagai fallback meta description.
{% endhint %}

---

### 5. Gunakan Editor Konten

Editor konten ElsCMS mendukung formatting HTML lengkap:

| Fitur | Keterangan |
|-------|-----------|
| **Heading** | H1–H6 untuk struktur judul dan sub-judul |
| **Bold / Italic** | Penekanan teks |
| **Bullet / Numbered List** | Daftar tidak berurutan / berurutan |
| **Link** | Tautan ke halaman lain atau URL eksternal |
| **Image** | Sisipkan gambar dari file library |
| **Table** | Tabel data |
| **Blockquote** | Kutipan dengan tampilan khusus |
| **Code** | Cuplikan kode program |

{% hint style="warning" %}
Saat menyisipkan gambar di dalam konten, gunakan gambar dari **File Library** ElsCMS agar URL gambar stabil dan terkelola.
{% endhint %}

---

### 6. Tambahkan Kategori

Di section **Categories**, klik **"Add Existing"** untuk memilih kategori yang sesuai dari daftar yang tersedia.

- Satu artikel bisa memiliki **lebih dari satu kategori**
- Pastikan kategori sudah dibuat sebelumnya di koleksi **Categories**

---

### 7. Tambahkan Tags

Di section **Tags**, klik **"Add Existing"** untuk menambahkan tag yang relevan dengan isi artikel.

Tags membantu pengunjung menemukan konten terkait dan memperkuat struktur SEO internal website.

---

### 8. Atur Status dan Publikasikan

Di field **Status** (langkah 3), pilih:

| Status | Keterangan |
|--------|-----------|
| `draft` | Artikel masih dalam pengerjaan — belum tampil di website |
| `published` | Artikel aktif dan tampil di website |
| `archived` | Artikel disembunyikan tanpa dihapus |

Klik **Save** (ikon centang atau tombol simpan) untuk menyimpan perubahan.

{% hint style="info" %}
Untuk menjadwalkan publikasi di waktu tertentu, set **Status** ke `published` dan isi field **Published At** dengan tanggal dan jam yang diinginkan.
{% endhint %}

---

## Checklist Sebelum Publish

Pastikan semua poin ini sudah diisi sebelum mengubah status ke **published**:

- [ ] **Title** sudah diisi (di bagian Translations)
- [ ] **Slug** sudah diatur — singkat, deskriptif, mengandung keyword utama
- [ ] **Featured Image** sudah dipilih
- [ ] **Excerpt** sudah ditulis (ringkasan 1–2 kalimat)
- [ ] **Konten** lengkap dan tidak ada typo
- [ ] **Kategori** sudah dipilih
- [ ] **Tags** relevan sudah ditambahkan
- [ ] **SEO Title** dan **SEO Description** sudah dioptimasi
- [ ] **Status** diubah ke `published`

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS · Diperbarui: 17 Mei 2026*
