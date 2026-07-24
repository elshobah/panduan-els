---
description: Mengatur identitas lembaga, kontak, AI Coach, sertifikat, notifikasi, dompet tenant, upgrade Pro, API Key, dan log aktivitas di panel Admin Tenant LMS Indonesia.
---

# Pengaturan dan Fitur Lanjutan

Grup **Pengaturan** adalah tempat Anda menyesuaikan identitas dan perilaku lembaga: nama, logo, kontak, AI Coach, sertifikat, hingga fitur lanjutan seperti API Key dan Log Aktivitas. Halaman ini merangkum semuanya.

---

## Prasyarat

- Anda bisa login sebagai **Super Admin** atau **Admin** — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Beberapa menu (API Key, Log Aktivitas) **hanya untuk Super Admin**

---

## Pengaturan Umum

Klik **Pengaturan → Pengaturan Umum**. Halaman ini terdiri dari beberapa bagian. Setelah mengubah, klik **Simpan Pengaturan**.

### Identitas Aplikasi

| Field | Keterangan |
|-------|-----------|
| **Nama Aplikasi** | Nama LMS yang tampil ke peserta |
| **Deskripsi Singkat** | Tagline lembaga |
| **Logo** | Logo yang tampil di website |
| **Favicon** | Ikon kecil di tab browser (.ico atau .png 32×32) |

### Kontak & Dukungan

| Field | Keterangan |
|-------|-----------|
| **Email Admin (Notifikasi)** | Penerima notifikasi sistem: order baru, penarikan, konfirmasi transfer |
| **Email Admin Kedua** | Opsional, menerima salinan (CC) notifikasi |
| **Email Support** | Email bantuan yang ditampilkan ke pengguna |
| **Nomor WhatsApp Support** | Format internasional tanpa `+` (mis. `6281234567890`) |

### Konfigurasi LMS

- **Timezone** — WIB / WITA / WIT / UTC
- **Bahasa Default** — Indonesia, English, atau Arab
- **Mode Maintenance** — menonaktifkan akses publik sementara (admin tetap bisa masuk)

### AI Coach

Bagian ini mengonfigurasi asisten AI per-pelajaran. Ingat: AI Coach juga harus **diaktifkan per kategori** — lihat [Kategori dan Paket Kursus](lms-admin-kategori-bundle.md).

| Field | Keterangan |
|-------|-----------|
| **Provider** | OpenRouter, Anthropic, atau OpenAI Compatible |
| **Base URL** | Wajib untuk provider "OpenAI Compatible" |
| **Model** | ID model (mis. `anthropic/claude-3.5-haiku`) |
| **API Key** | Kunci API provider Anda |
| **Panjang Respons** | Singkat (hemat biaya) / Sedang / Panjang |
| **Batas Anggaran Bulanan (USD)** | Pagu biaya AI per bulan |

{% hint style="warning" %}
AI Coach menggunakan layanan AI berbayar. Setel **Batas Anggaran Bulanan** dan pilih **Panjang Respons: Singkat** untuk mengendalikan biaya. Simpan API Key Anda dengan hati-hati.
{% endhint %}

### Notifikasi Email Admin

Nyalakan/matikan jenis notifikasi yang dikirim ke Email Admin: order baru, bukti transfer, pembayaran dikonfirmasi, request penarikan, donasi, member baru, kursus selesai, dan diskusi baru. Semua aktif secara default.

### Sertifikat

Atur tampilan sertifikat penyelesaian kursus:

- **Logo Sertifikat**
- **Nama Penanda Tangan** & **Jabatan Penanda Tangan**
- **Gambar Tanda Tangan** (disarankan PNG transparan)

### API & Integrasi (CORS)

Daftarkan **origin front-end** yang boleh memanggil API publik LMS dari browser — hanya perlu jika website depan Anda berada di domain/subdomain lain. Masukkan origin lengkap dengan skema, tanpa trailing slash (mis. `https://belajar.domain-anda.com`).

---

## Pengaturan Pembayaran

Diatur di menu terpisah **Pengaturan → Pengaturan Pembayaran** dan dibahas lengkap di [Pesanan, Pembayaran, dan Kupon](lms-admin-pesanan-pembayaran.md).

---

## Dompet Tenant

Halaman **Dompet Tenant** menampilkan saldo dan riwayat dana lembaga Anda di platform. Dari sini Anda memantau pemasukan bersih dan (bila tersedia) mengajukan penarikan ke rekening lembaga.

---

## Upgrade Pro

Halaman **Upgrade Pro** dipakai meningkatkan paket lembaga dari **Free** ke **Pro**. Paket Pro membuka fitur seperti:

- **Metode pembayaran sendiri** — Tripay, transfer manual, dan QRIS statis milik lembaga
- **Custom domain** — memakai domain sendiri (mis. `belajar.lembaga-anda.com`) dengan verifikasi
- Branding dan kapasitas yang lebih luas

{% hint style="info" %}
Tenant **Free** tetap bisa berjualan — pembayaran otomatis diproses via **QRIS platform (Xendit)**. Upgrade ke Pro saat Anda ingin memakai gateway dan domain sendiri.
{% endhint %}

---

## API Key (Super Admin)

Menu **Pengaturan → API Key** dipakai membuat kunci akses untuk integrasi API publik lembaga Anda — misalnya menghubungkan website atau aplikasi lain ke data kursus Anda.

{% hint style="warning" %}
Menu ini **hanya untuk Super Admin**. Perlakukan API Key seperti password: jangan dibagikan sembarangan, dan **Cabut** segera bila diduga bocor.
{% endhint %}

---

## Log Aktivitas (Super Admin)

Menu **Pengaturan → Log Aktivitas** adalah catatan audit yang **hanya-baca**: siapa mengubah peran, mengonfirmasi pembayaran, dan tindakan penting lainnya. Gunakan untuk menelusuri "siapa melakukan apa dan kapan". Menu ini juga **hanya untuk Super Admin**.

---

## Checklist Pengaturan Awal

- [ ] Nama, logo, dan favicon lembaga sudah diisi
- [ ] Email Admin & WhatsApp Support sudah benar
- [ ] Timezone diset ke zona wilayah Anda
- [ ] Sertifikat (logo & penanda tangan) sudah disiapkan
- [ ] AI Coach dikonfigurasi hanya jika akan dipakai, dengan batas anggaran
- [ ] API Key dijaga kerahasiaannya (khusus Super Admin)

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
