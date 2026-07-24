---
description: Membuat dan mengelola kursus, webinar, dan event di LMS Indonesia — mengatur tipe, harga, infaq, jadwal, kurikulum, topik & pelajaran, hingga mempublikasikan.
---

# Mengelola Kursus dan Pelajaran

Kursus adalah inti dari lembaga belajar Anda. Menu **Kursus** (grup **Konten**) dipakai untuk membuat tiga jenis produk belajar: **Kursus Online**, **Webinar/Live**, dan **Kegiatan/Event**. Halaman ini membahas cara membuatnya dari awal sampai tayang.

---

## Prasyarat

- Anda bisa login sebagai **Super Admin**, **Admin**, atau **Instruktur**
- Minimal satu **Kategori** sudah dibuat — lihat [Kategori dan Paket Kursus](lms-admin-kategori-bundle.md)
- Minimal satu pengguna berperan **Instruktur** tersedia — lihat [Mengelola Pengguna dan Peran](lms-admin-pengguna-peran.md)
- Gambar thumbnail sudah dikompres — lihat [Tutorial Kompres Gambar](tutorial-kompres-gambar.md)

{% hint style="warning" %}
Hanya **Super Admin** yang dapat **menghapus** kursus. Admin dan Instruktur bisa membuat dan mengedit, tetapi tidak menghapus.
{% endhint %}

---

## Langkah-Langkah

### 1. Buka Menu Kursus & Klik Buat Baru

Klik **Konten → Kursus**, lalu klik **Create** / **Buat Kursus** di kanan atas.

![Daftar kursus](https://GANTI-DENGAN-SCREENSHOT)

### 2. Isi Informasi Utama

| Field | Keterangan |
|-------|-----------|
| **Tipe** | 📚 Kursus Online, 🎙️ Webinar/Live, atau 📅 Kegiatan/Event |
| **Status** | Draft, Dipublikasikan, atau Privat |
| **Judul** | Nama kursus. **Slug** terisi otomatis dari judul |
| **Instruktur / Pembicara** | Pengguna berperan instruktur |
| **Kategori** | Kategori kursus |
| **Level** | Umum, Pemula, Menengah, atau Lanjutan (untuk webinar/event field ini disembunyikan) |
| **Bahasa** | Indonesia, English, atau Arab |

{% hint style="info" %}
Simpan kursus sebagai **Draft** dulu selama masih menyusun materi. Ubah ke **Dipublikasikan** hanya bila sudah siap tayang. Status **Privat** membuat kursus tersembunyi dari katalog publik.
{% endhint %}

### 3. Jadwal & Link (Khusus Webinar/Event)

Jika Tipe adalah Webinar atau Event, akan muncul bagian **Jadwal & Link**:

- **Waktu Mulai** dan **Waktu Selesai** (zona waktu WIB / Asia-Jakarta)
- **Link Zoom / YouTube Live / Meet**
- **Kuota Peserta** (kosongkan bila tidak terbatas)
- **Link Grup WhatsApp** untuk peserta yang sudah mendaftar

### 4. Tulis Deskripsi

- **Deskripsi Singkat** — ringkasan 1–2 baris untuk kartu kursus
- **Deskripsi Lengkap** — penjelasan penuh dengan editor teks kaya (bold, daftar, dll.)

### 5. Atur Harga

Cara mengatur harga bergantung pada tipe kursus.

**Untuk Kursus Online biasa:**

- Aktifkan toggle **Gratis** bila kursus tanpa biaya, atau
- Isi **Harga**, dan opsional **Harga Diskon** (harga coret)

**Untuk Webinar/Event**, tersedia pilihan **Tipe Harga**:

| Tipe Harga | Cara kerja |
|-----------|-----------|
| 💳 **Harga Tetap** | Peserta membayar nominal pasti |
| 🤲 **Infaq (Pilih Nominal)** | Peserta bebas memilih nominal kontribusi dari **Preset Nominal Infaq** yang Anda sediakan, dengan batas **Minimal Infaq** |

{% hint style="info" %}
Untuk mode **Infaq**, isi beberapa preset nominal (contoh: 199.000, 99.000, 25.000) agar peserta tinggal memilih. Anda juga menetapkan nominal minimal yang boleh dipilih.
{% endhint %}

### 6. Unggah Media

- **Thumbnail (Potrait)** — gambar utama untuk kartu kursus. Diunggah langsung dan dikompres otomatis.
- **Gambar Landscape** — opsional, untuk tampilan lebar/hero. Jika kosong, sistem memakai thumbnail.
- **URL Preview Video** — opsional, tautan video cuplikan.

### 7. Lengkapi Kurikulum & SEO

- **Prasyarat** — daftar hal yang perlu diketahui peserta sebelum ikut
- **Yang Akan Dipelajari** — poin-poin hasil belajar
- **Meta Title** & **Meta Description** — untuk optimasi mesin pencari

Klik **Save** untuk menyimpan kursus.

---

## Menyusun Materi: Topik & Pelajaran

Setelah kursus tersimpan, buka kembali kursus tersebut (klik **Edit** atau **View**). Di dalamnya tersedia tab pengelola relasi untuk menyusun struktur materi:

| Tab | Fungsi |
|-----|--------|
| **Topics** | Bab/bagian besar untuk mengelompokkan pelajaran |
| **Lessons** | Materi pelajaran (video, teks, dll.) di dalam topik |
| **Enrollments** | Daftar peserta yang terdaftar di kursus ini |

Alur yang disarankan: buat beberapa **Topic** lebih dulu, lalu tambahkan **Lesson** ke masing-masing topik.

![Menyusun topik dan pelajaran di dalam kursus](https://GANTI-DENGAN-SCREENSHOT)

---

## Mempublikasikan Kursus

Ada dua cara menayangkan kursus:

1. **Saat edit** — ubah field **Status** menjadi **Dipublikasikan**, lalu simpan.
2. **Dari daftar** — pada tabel kursus, gunakan aksi **Publish** (tombol hijau). Untuk menurunkan kembali ke draft, gunakan **Unpublish**.

{% hint style="success" %}
Sebelum publish, pastikan kursus punya thumbnail, deskripsi, harga yang benar, dan minimal beberapa pelajaran. Kursus yang tayang tanpa materi akan mengecewakan peserta.
{% endhint %}

---

## Sertifikat Penyelesaian

Peserta yang menyelesaikan kursus dapat memperoleh **sertifikat** secara otomatis. Tampilan sertifikat (logo, nama & jabatan penanda tangan, gambar tanda tangan) diatur di [Pengaturan & Fitur Lanjutan](lms-admin-pengaturan.md).

---

## Checklist Sebelum Publish Kursus

- [ ] Tipe, judul, instruktur, dan kategori sudah diisi
- [ ] Harga sudah benar (atau ditandai Gratis / Infaq)
- [ ] Thumbnail sudah diunggah dan proporsional
- [ ] Deskripsi singkat dan lengkap sudah ditulis
- [ ] Minimal ada beberapa topik dan pelajaran
- [ ] Untuk webinar: jadwal, link, dan kuota sudah diisi
- [ ] Status diubah ke **Dipublikasikan**

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
