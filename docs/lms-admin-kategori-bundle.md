---
description: Mengatur kategori kursus (termasuk mengaktifkan AI Coach) dan membuat Paket Kursus (bundle) dengan harga hemat di LMS Indonesia.
---

# Kategori dan Paket Kursus

Dua menu di grup **Konten** ini membantu Anda merapikan dan mengemas kursus: **Kategori** untuk mengelompokkan kursus, dan **Paket Kursus** (bundle) untuk menjual beberapa kursus sekaligus dengan satu harga.

---

## Prasyarat

- Anda bisa login sebagai **Super Admin** atau **Admin** — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Untuk membuat bundle, sudah ada beberapa kursus — lihat [Mengelola Kursus dan Pelajaran](lms-admin-kursus.md)

---

## Bagian 1 — Kategori

Kategori adalah pengelompokan kursus (misalnya "Tahsin", "Bahasa Arab", "Parenting"). Setiap kursus wajib punya satu kategori, jadi sebaiknya buat kategori **sebelum** membuat kursus.

### 1. Buka Menu Kategori

Klik **Konten → Kategori**, lalu klik **Tambah Kategori**.

![Daftar kategori](https://GANTI-DENGAN-SCREENSHOT)

### 2. Isi Data Kategori

| Field | Keterangan |
|-------|-----------|
| **Nama Kategori** | Nama yang tampil ke peserta |
| **Slug** | Versi URL dari nama (biasanya terisi otomatis) |
| **Ikon (emoji atau kode)** | Ikon kecil pendamping kategori, opsional |
| **Urutan Tampil** | Angka untuk mengatur posisi kategori di daftar |
| **Deskripsi** | Penjelasan singkat kategori, opsional |
| **Aktifkan AI Coach** | Menyalakan asisten AI untuk kursus di kategori ini |

### 3. Tentang "Aktifkan AI Coach"

Toggle **Aktifkan AI Coach** menyalakan fitur asisten AI per-pelajaran untuk semua kursus dalam kategori tersebut. 

{% hint style="info" %}
AI Coach perlu dikonfigurasi lebih dulu (provider, model, dan anggaran) di **Pengaturan Umum** sebelum benar-benar berfungsi. Selengkapnya di [Pengaturan & Fitur Lanjutan](lms-admin-pengaturan.md). Jika belum dikonfigurasi, biarkan toggle ini mati.
{% endhint %}

Klik **Save** untuk menyimpan.

---

## Bagian 2 — Paket Kursus (Bundle)

Paket Kursus menggabungkan beberapa kursus menjadi satu produk dengan harga khusus — biasanya lebih hemat daripada membeli satu per satu.

### 1. Buka Menu Paket Kursus

Klik **Konten → Paket Kursus**, lalu klik **Create**.

![Daftar paket kursus](https://GANTI-DENGAN-SCREENSHOT)

### 2. Isi Informasi Paket

| Field | Keterangan |
|-------|-----------|
| **Status** | Draft atau Dipublikasikan |
| **Judul Paket** | Nama bundle |
| **Slug** | Versi URL dari judul |
| **Deskripsi Singkat** & **Deskripsi Lengkap** | Penjelasan isi paket |
| **Harga Paket** | Harga jual bundle |
| **Harga Diskon** | Harga coret, opsional |
| **Thumbnail** | Gambar utama paket |
| **Meta Title** & **Meta Description** | Untuk SEO |

### 3. Pilih Kursus yang Termasuk

Di dalam form paket, tambahkan kursus-kursus yang menjadi isi bundle. Jumlah kursus yang tergabung akan tampil di daftar paket.

{% hint style="success" %}
Beri harga paket yang jelas lebih murah daripada total harga satuan kursusnya. Selisih inilah yang membuat peserta memilih membeli paket.
{% endhint %}

Klik **Save**, lalu ubah status menjadi **Dipublikasikan** saat siap dijual.

---

## Checklist

- [ ] Kategori inti sudah dibuat sebelum membuat kursus
- [ ] Urutan tampil kategori sudah diatur agar rapi
- [ ] Toggle AI Coach hanya dinyalakan jika AI Coach sudah dikonfigurasi
- [ ] Paket berisi minimal dua kursus dengan harga hemat
- [ ] Paket dipublikasikan hanya setelah kursus di dalamnya siap

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
