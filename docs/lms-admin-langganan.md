---
description: Mengelola modul langganan (subscription) di LMS Indonesia — membuat paket langganan berdurasi dan memantau subscriber yang aktif.
---

# Langganan (Subscription)

Modul Langganan memungkinkan peserta membayar berkala untuk mengakses sekumpulan kursus selama periode tertentu — model "membership". Menu terkait: **Paket Langganan** (grup **Konten**) dan **Subscriber** (grup **Transaksi**).

{% hint style="warning" %}
Langganan adalah **fitur tambahan (add-on)** yang perlu **diaktifkan** untuk lembaga Anda. Jika menu **Paket Langganan** dan **Subscriber** belum muncul, aktifkan lewat halaman **Add-on Langganan** di panel, atau hubungi tim kami. Selengkapnya di [Pengaturan & Fitur Lanjutan](lms-admin-pengaturan.md).
{% endhint %}

---

## Prasyarat

- Modul Langganan sudah aktif untuk lembaga Anda
- Anda bisa login sebagai **Super Admin** atau **Admin** — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Sudah ada kursus yang akan dimasukkan ke paket — lihat [Mengelola Kursus dan Pelajaran](lms-admin-kursus.md)

---

## 1. Membuat Paket Langganan

Klik **Konten → Paket Langganan → Create**.

![Membuat paket langganan](https://GANTI-DENGAN-SCREENSHOT)

| Field | Keterangan |
|-------|-----------|
| **Nama Paket** | Nama membership (mis. "Member Premium") |
| **Slug** | Versi URL dari nama |
| **Deskripsi** | Penjelasan manfaat paket |
| **Harga** | Harga langganan |
| **Harga Diskon** | Harga coret, opsional |
| **Durasi** | Lama akses (mis. bulanan, tahunan) |
| **Status** | Draft / Aktif |
| **Urutan Tampil** | Posisi paket di daftar |
| **Kursus yang Termasuk** | Kursus-kursus yang bisa diakses subscriber |

{% hint style="info" %}
Pilih kursus yang termasuk dengan cermat — subscriber akan mengakses **semua** kursus dalam paket selama masa langganannya aktif.
{% endhint %}

Klik **Save**, lalu ubah status menjadi **Aktif** saat siap dijual.

---

## 2. Memantau Subscriber

Klik **Transaksi → Subscriber** untuk melihat daftar pelanggan aktif.

| Field | Keterangan |
|-------|-----------|
| **Pengguna** & **Email** | Identitas subscriber |
| **Paket** | Paket langganan yang diambil |
| **Status** | Aktif / berakhir / dibatalkan |
| **Mulai** & **Berakhir** | Periode langganan |

Anda dapat **membatalkan** langganan seorang subscriber dari halaman ini bila diperlukan.

{% hint style="warning" %}
Saat langganan **berakhir** atau **dibatalkan**, akses subscriber ke kursus-kursus dalam paket akan berhenti. Pastikan komunikasi perpanjangan berjalan agar peserta tidak kehilangan akses mendadak.
{% endhint %}

---

## Checklist Langganan

- [ ] Modul Langganan sudah aktif untuk lembaga Anda
- [ ] Paket punya harga, durasi, dan daftar kursus yang jelas
- [ ] Paket dipublikasikan (status Aktif) hanya setelah kursusnya siap
- [ ] Memantau subscriber yang akan berakhir untuk perpanjangan

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
