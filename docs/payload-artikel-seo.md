---
description: Cara membuat dan mengedit artikel di Payload — gambar utama, editor Lexical, kategori, penulis, dan optimasi SEO.
---

# Membuat Artikel dan Optimasi SEO di Payload

Artikel, berita, dan blog dikelola di koleksi **Posts**. Panduan ini membahas cara menulisnya sekaligus mengoptimalkannya agar mudah ditemukan di Google.

---

## Prasyarat

- Anda sudah bisa login ke admin Payload — lihat [Login dan Mengenal Dashboard Payload](payload-login-dashboard.md)
- Anda sudah paham alur draft dan publish — lihat [Draft, Preview, dan Publish di Payload](payload-draft-preview-publish.md)
- Gambar utama artikel sudah diunggah — lihat [Mengelola Media di Payload](payload-media-library.md)

---

## Langkah-Langkah

### 1. Buat Artikel Baru

Klik menu **Posts** di sidebar kiri, lalu klik **Create New**.

### 2. Isi Judul

Field **Title** wajib diisi. Ini judul yang tampil di website dan menjadi dasar slug.

{% hint style="success" %}
Judul yang baik itu spesifik dan mengandung kata yang benar-benar diketik orang saat mencari. Bandingkan "Tips Merawat Tanaman" dengan "7 Cara Merawat Tanaman Hias Agar Tidak Mudah Layu" — yang kedua jauh lebih mungkin diklik dari hasil pencarian.
{% endhint %}

### 3. Periksa Slug

Di sidebar kanan, field **Slug** terisi otomatis dari judul. Untuk mengubahnya, klik ikon gembok lalu ketik slug baru.

Slug yang baik itu pendek dan mengandung kata kunci. Untuk judul panjang di atas, slug `cara-merawat-tanaman-hias` lebih baik daripada slug penuh yang ikut memuat angka dan kata sambung.

{% hint style="danger" %}
Jangan ubah slug artikel yang sudah tayang dan sudah dibagikan — semua tautan lama akan mati. Kalau terpaksa, buat **Redirect** dari slug lama ke slug baru.
{% endhint %}

---

### 4. Pilih Gambar Utama

Di tab **Content**, field **Hero Image** adalah gambar utama artikel. Gambar ini tampil di bagian atas artikel dan di daftar artikel.

Klik untuk memilih gambar dari Media, atau unggah baru langsung dari sini.

---

### 5. Tulis Isi Artikel

Field **Content** wajib diisi. Editornya bernama **Lexical** dan bekerja seperti pengolah kata biasa.

Toolbar di atas menyediakan format standar:

| Fitur | Keterangan |
|-------|-----------|
| **Heading** | H1 sampai H4 untuk sub-judul |
| **Bold / Italic** | Penekanan teks |
| **List** | Daftar berpoin atau bernomor |
| **Link** | Tautan ke halaman lain atau URL luar |
| **Blockquote** | Kutipan |
| **Horizontal Rule** | Garis pemisah antar bagian |

Anda juga bisa menyisipkan **block** di tengah tulisan. Ketik `/` di baris kosong, atau klik tombol tambah di sisi kiri baris:

| Block | Fungsinya |
|-------|-----------|
| **Media Block** | Menyisipkan gambar di tengah artikel |
| **Banner** | Kotak sorot untuk info, peringatan, atau catatan penting |
| **Code** | Cuplikan kode program |

{% hint style="success" %}
**Soal heading:** judul artikel sudah menjadi H1 secara otomatis. Jadi di dalam tulisan, mulailah sub-judul dari **H2**, dan pakai **H3** untuk anak-bagiannya. Struktur yang runut membantu pembaca memindai tulisan sekaligus membantu Google memahami isinya.
{% endhint %}

---

### 6. Pilih Kategori

Di sidebar kanan, field **Categories** menentukan pengelompokan artikel. Satu artikel boleh punya **lebih dari satu** kategori.

Kategori harus sudah dibuat lebih dulu di menu **Categories**.

### 7. Isi Penulis

Di sidebar kanan, field **Authors** memilih penulis artikel dari daftar user. Bisa diisi lebih dari satu orang.

### 8. Pilih Artikel Terkait

Field **Related Posts** di sidebar kanan menentukan artikel yang disarankan di bagian bawah tulisan. Artikel yang sedang dibuka otomatis tidak muncul di pilihan.

{% hint style="success" %}
Mengisi Related Posts membuat pengunjung betah membaca lebih lama, dan tautan antar artikel juga memperkuat SEO internal website Anda.
{% endhint %}

---

### 9. Optimalkan Tab SEO

Klik tab **SEO**. Bagian ini menentukan tampilan artikel Anda di Google dan saat dibagikan ke WhatsApp.

| Field | Keterangan | Panjang ideal |
|-------|-----------|---------------|
| **Title** | Judul di hasil pencarian Google | 50–60 karakter |
| **Description** | Deskripsi di bawah judul | 150–160 karakter |
| **Image** | Gambar preview saat tautan dibagikan | 1200 × 630px |

Tombol **Auto-generate** pada Title akan mengisinya dari judul artikel dan menambahkan nama website di belakangnya. Hasilnya boleh Anda sunting.

Di bagian bawah ada **Preview** — simulasi tampilan di hasil pencarian. Pakai ini untuk memastikan tidak ada yang terpotong.

{% hint style="success" %}
**Title** adalah judul untuk mesin pencari, jadi tidak harus sama persis dengan judul artikel — tulis ulang agar lebih menggoda diklik, dengan kata kunci utama di bagian depan.

**Description** bukan tempat menumpuk kata kunci. Tulis satu-dua kalimat yang membuat orang penasaran, karena inilah yang mereka baca sebelum memutuskan klik.
{% endhint %}

---

### 10. Atur Tanggal dan Publikasikan

Field **Published At** di sidebar kanan menentukan tanggal dan jam terbit artikel.

Kalau dibiarkan kosong, Payload mengisinya otomatis dengan waktu saat Anda menekan **Publish**. Isi manual hanya jika Anda ingin menampilkan tanggal tertentu.

Cek dulu lewat **Live Preview**, lalu klik **Publish**. Selengkapnya di [Draft, Preview, dan Publish di Payload](payload-draft-preview-publish.md).

{% hint style="info" %}
Setelah dipublikasikan, artikel otomatis masuk ke indeks pencarian di dalam website. Tidak ada langkah tambahan yang perlu dilakukan.
{% endhint %}

---

## Checklist Sebelum Publish

- [ ] **Title** spesifik dan mengandung kata kunci
- [ ] **Slug** pendek dan deskriptif
- [ ] **Hero Image** sudah dipilih dan alt text-nya terisi
- [ ] **Content** lengkap, tanpa typo, sub-judul mulai dari H2
- [ ] Gambar di dalam artikel disisipkan lewat **Media Block**
- [ ] **Categories** sudah dipilih
- [ ] **Authors** sudah diisi
- [ ] **Related Posts** sudah dipilih
- [ ] **SEO Title** dan **Description** sudah dioptimasi dan tidak terpotong di Preview
- [ ] **SEO Image** sudah dipilih
- [ ] Sudah dicek di **Live Preview** ukuran Mobile

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS with Payload · Diperbarui: 15 Juli 2026*
