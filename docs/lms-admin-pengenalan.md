---
description: Mengenal panel Admin Tenant LMS Indonesia — cara login, memahami dashboard, dan peta menu untuk mengelola lembaga belajar online Anda sendiri.
---

# Ikhtisar dan Akses Panel Admin

LMS Indonesia adalah platform belajar online *multi-tenant*: satu sistem melayani banyak penyelenggara, dan setiap penyelenggara (disebut **tenant**) memiliki panel admin sendiri untuk mengelola kursus, peserta, transaksi, hingga sertifikat. Panduan ini adalah titik awal bagi **Admin Tenant** — orang yang mengoperasikan panel `/admin` lembaga Anda.

{% hint style="info" %}
Panduan ini adalah gerbang menuju seri lengkap Admin Tenant. Setiap topik dibahas mendalam di halamannya masing-masing, dan ditautkan di bagian bawah.
{% endhint %}

---

## Apa Itu Tenant?

Tenant adalah "lembaga" atau "penyelenggara" Anda di dalam LMS Indonesia — lengkap dengan nama, logo, warna, kursus, dan pesertanya sendiri. Semua data Anda **terpisah total** dari tenant lain: kursus, pengguna, dan pesanan tenant lain tidak akan pernah tampil di panel Anda, dan sebaliknya.

Panel admin diakses lewat satu alamat login:

```
https://lms.elshobah.com/admin/login
```

Setelah berhasil masuk, sistem otomatis mengarahkan Anda ke panel lembaga (tenant) Anda. Anda tidak perlu mengingat slug lembaga — cukup buka halaman login di atas.

---

## Cara Login

### 1. Buka Halaman Login

Buka [https://lms.elshobah.com/admin/login](https://lms.elshobah.com/admin/login) di browser.

![Halaman login panel Admin Tenant](https://GANTI-DENGAN-SCREENSHOT)

{% hint style="info" %}
Ganti setiap gambar `GANTI-DENGAN-SCREENSHOT` pada panduan ini dengan tangkapan layar asli dari panel lembaga Anda, lalu unggah ke penyimpanan gambar Anda dan tempel URL-nya.
{% endhint %}

### 2. Masuk dengan Email & Password

Masukkan **email** dan **password** akun Anda, lalu klik **Sign in**. Jika Anda pemilik lembaga, gunakan akun yang dibuat saat mendaftar penyelenggara.

{% hint style="warning" %}
Hanya pengguna dengan peran **Super Admin**, **Admin**, atau **Financial (Keuangan)** yang bisa masuk ke panel `/admin`. Peran Instruktur, Siswa, dan Afiliasi belajar dan bertransaksi lewat halaman depan website, bukan lewat panel admin ini. Selengkapnya di [Mengelola Pengguna dan Peran](lms-admin-pengguna-peran.md).
{% endhint %}

---

## Mengenal Dashboard

Setelah login, Anda akan tiba di halaman **Dashboard**. Di sini tersedia ringkasan cepat kondisi lembaga Anda:

| Bagian | Isi |
|--------|-----|
| **Statistik Pendapatan** | Ringkasan pemasukan dan transaksi terbaru |
| **Tindakan Tertunda** | Daftar hal yang butuh perhatian Anda — misalnya pembayaran manual yang menunggu konfirmasi atau permintaan penarikan komisi |
| **Ikon lonceng 🔔** | Notifikasi di dalam aplikasi (order baru, bukti transfer diunggah, dll.) |

![Dashboard panel Admin Tenant](https://GANTI-DENGAN-SCREENSHOT)

{% hint style="success" %}
Biasakan mengecek panel **Tindakan Tertunda** setiap kali login. Dari situ Anda bisa langsung menuju pekerjaan yang paling mendesak tanpa harus menelusuri menu satu per satu.
{% endhint %}

---

## Peta Menu

Menu di sidebar kiri dikelompokkan menjadi beberapa grup. Berikut peta lengkapnya beserta halaman panduan terkait:

| Grup | Menu | Panduan |
|------|------|---------|
| **Konten** | Kursus, Kategori, Paket Kursus, Paket Langganan | [Kursus](lms-admin-kursus.md), [Kategori & Bundle](lms-admin-kategori-bundle.md) |
| **Manajemen** | Pengguna, Afiliasi, Rate Komisi, Penarikan | [Pengguna & Peran](lms-admin-pengguna-peran.md), [Afiliasi](lms-admin-afiliasi.md) |
| **Transaksi** | Order, Kupon, Subscriber | [Pesanan & Pembayaran](lms-admin-pesanan-pembayaran.md), [Langganan](lms-admin-langganan.md) |
| **Donasi** | Kampanye Donasi, Kategori Donasi, Transaksi Donasi, Laporan Dana | [Donasi](lms-admin-donasi.md) |
| **Komunitas** | Diskusi | [Komunitas & Diskusi](lms-admin-komunitas.md) |
| **Pengaturan** | Pengaturan Umum, Pengaturan Pembayaran, API Key, Log Aktivitas | [Pengaturan & Fitur Lanjutan](lms-admin-pengaturan.md) |

{% hint style="info" %}
Beberapa menu **hanya muncul jika fiturnya aktif** untuk lembaga Anda. Grup **Donasi** dan menu **Paket Langganan / Subscriber** adalah fitur tambahan (add-on) yang perlu diaktifkan terlebih dahulu. Menu tertentu seperti **API Key** dan **Log Aktivitas** hanya terlihat oleh Super Admin.
{% endhint %}

---

## Alur Kerja yang Disarankan untuk Admin Baru

Jika lembaga Anda baru saja dibuat, urutan langkah ini paling efisien:

1. **Atur identitas lembaga** — nama, logo, kontak, dan zona waktu di [Pengaturan Umum](lms-admin-pengaturan.md).
2. **Buat kategori** kursus terlebih dahulu — lihat [Kategori & Paket Kursus](lms-admin-kategori-bundle.md).
3. **Tambahkan instruktur** dan atur peran pengguna — lihat [Mengelola Pengguna dan Peran](lms-admin-pengguna-peran.md).
4. **Buat kursus pertama** dan publikasikan — lihat [Mengelola Kursus dan Pelajaran](lms-admin-kursus.md).
5. **Atur metode pembayaran** agar peserta bisa membeli — lihat [Pesanan, Pembayaran, dan Kupon](lms-admin-pesanan-pembayaran.md).

---

## Checklist Login Pertama

- [ ] Berhasil masuk ke panel `/admin` lembaga Anda
- [ ] Mengenali widget **Statistik Pendapatan** dan **Tindakan Tertunda** di dashboard
- [ ] Mengetahui letak enam grup menu di sidebar
- [ ] Memahami peran akun Anda (Super Admin / Admin / Keuangan)

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
