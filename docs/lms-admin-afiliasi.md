---
description: Mengelola program afiliasi di LMS Indonesia — meninjau afiliasi, mengatur rate komisi per kategori, dan menyetujui permintaan penarikan komisi.
---

# Program Afiliasi

Program afiliasi memungkinkan mitra memasarkan kursus Anda dan mendapat komisi dari setiap penjualan lewat kode referral mereka. Grup **Manajemen** menyediakan tiga menu terkait: **Afiliasi**, **Rate Komisi**, dan **Penarikan**.

{% hint style="warning" %}
Afiliasi adalah **fitur opsional**. Tidak semua lembaga menggunakannya. Beberapa aksi lanjutan (mengelola/menyetel ulang program afiliasi) **hanya untuk Super Admin** — Admin biasa dapat meninjau dan menyetujui penarikan, tetapi tidak mengelola konfigurasi programnya.
{% endhint %}

---

## Prasyarat

- Anda bisa login sebagai **Super Admin** atau **Admin** — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Biaya & minimum penarikan komisi diatur di **Pengaturan Pembayaran** — lihat [Pesanan, Pembayaran, dan Kupon](lms-admin-pesanan-pembayaran.md)

---

## 1. Meninjau Afiliasi

Klik **Manajemen → Afiliasi**. Tabel menampilkan daftar mitra beserta kode referral dan status mereka.

![Daftar afiliasi](https://GANTI-DENGAN-SCREENSHOT)

Klik sebuah afiliasi untuk melihat detail lengkap:

| Bagian | Isi |
|--------|-----|
| **Profil Afiliasi** | Nama, email, kode referral, status, tanggal bergabung |
| **Keuangan** | Total Komisi, Total Dicairkan, Saldo |
| **Akuisisi (Funnel)** | Jumlah View, Klik, dan Konversi |
| **Rekening Bank** | Bank, nomor rekening, dan nama pemilik untuk pencairan |

Anda dapat mengubah **status** afiliasi (mis. menyetujui atau menonaktifkan) dari halaman ini.

---

## 2. Mengatur Rate Komisi

Klik **Manajemen → Rate Komisi** untuk menentukan besar komisi per **kategori** kursus.

| Field | Keterangan |
|-------|-----------|
| **Kategori** | Kategori kursus yang dikenai rate ini |
| **Rate Komisi (%)** | Persentase komisi dari nilai transaksi |
| **Maks Komisi per Transaksi** | Batas atas komisi (opsional) |
| **Aktif** | Nyalakan/matikan rate |

{% hint style="info" %}
Menetapkan rate per kategori memberi fleksibilitas — misalnya komisi lebih besar untuk kategori yang ingin Anda dorong penjualannya.
{% endhint %}

---

## 3. Menyetujui Penarikan Komisi

Saat afiliasi mengajukan pencairan, permintaan muncul di **Manajemen → Penarikan**.

![Daftar penarikan komisi](https://GANTI-DENGAN-SCREENSHOT)

Setiap permintaan menampilkan:

- **Penarikan (Bruto)** — jumlah yang diajukan
- **Biaya Transfer** — biaya yang dipotong (mis. BI Fast)
- **Ditransfer ke Afiliasi** — jumlah bersih = bruto − biaya
- **Rekening Tujuan** — bank, nomor rekening, nama pemilik
- **Catatan Admin** — catatan yang bisa Anda isi

**Alur menyetujui:**

1. Verifikasi saldo afiliasi mencukupi dan rekening tujuan benar.
2. Lakukan transfer manual ke rekening afiliasi sejumlah nominal bersih.
3. Perbarui status penarikan menjadi diproses/selesai, dan isi **Catatan Admin** bila perlu.

{% hint style="warning" %}
Biaya dan minimum penarikan mengikuti pengaturan di **Pengaturan Pembayaran → Penarikan Komisi Afiliasi**. Pastikan minimum penarikan lebih besar dari biaya transfer.
{% endhint %}

---

## Checklist Afiliasi

- [ ] Rate komisi per kategori sudah ditetapkan dan aktif
- [ ] Biaya & minimum penarikan sudah diatur di Pengaturan Pembayaran
- [ ] Memverifikasi rekening tujuan sebelum mentransfer
- [ ] Memperbarui status penarikan setelah dana dikirim

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
