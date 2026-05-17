---
description: Platform digital all-in-one untuk bisnis Indonesia — e-commerce, kursus online, blog, dan manajemen konten dalam satu ekosistem.
cover: https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&w=1200&q=80
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Welcome to A Elshobah Co

Selamat datang di dokumentasi resmi **A Elshobah Co** — platform digital multi-tenant yang dirancang untuk membantu bisnis Indonesia tumbuh secara online. Dari toko produk digital, kursus online, hingga blog dan manajemen konten, semua tersedia dalam satu ekosistem yang terintegrasi.

---

## Apa itu Elshobah?

Elshobah adalah **platform SaaS multi-tenant** yang memberi Anda kendali penuh atas kehadiran digital bisnis Anda. Setiap tenant mendapatkan lingkungannya sendiri — konten, produk, pelanggan, dan pengaturan yang terisolasi dan aman.

![Platform overview — kelola semua aspek bisnis digital Anda dari satu dasbor](https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=1200&q=80)

---

## Fitur Utama

### 🛍️ E-Commerce

Kelola katalog produk, proses pesanan, dan terima pembayaran — semua terintegrasi dengan payment gateway lokal Indonesia.

![E-commerce dan manajemen pembayaran](https://images.unsplash.com/photo-1556742049-0cfed4f6a45d?auto=format&fit=crop&w=1200&q=80)

- **Katalog Produk** — kelola produk dengan kategori, tag, dan galeri gambar
- **Order Management** — pantau pesanan dari pending hingga selesai
- **Invoice Otomatis** — tagihan dibuat secara otomatis setiap transaksi
- **Payment Gateway** — integrasi dengan **Midtrans** dan **Xendit**
- **Webhook Handler** — log pembayaran real-time dari gateway

---

### 🎓 Learning Management System (LMS)

Buat dan jual kursus online dengan struktur modul yang fleksibel — dari satu video hingga kurikulum lengkap.

![Buat kursus online yang engaging](https://images.unsplash.com/photo-1434030216411-0b793f4b4173?auto=format&fit=crop&w=1200&q=80)

- **Courses** — buat kursus dengan deskripsi, harga, dan thumbnail
- **Modules & Lessons** — susun konten secara hierarkis: Kursus → Modul → Lesson
- **Enrollment** — akses kursus dibuat otomatis setelah pembayaran berhasil
- **Progress Tracking** — pantau progres peserta kursus

---

### ✍️ Blog & Content Management

Publikasikan artikel, berita, dan halaman statis dengan sistem CMS yang intuitif.

![Tulis dan publikasikan konten berkualitas](https://images.unsplash.com/photo-1499750310107-5fef28a66643?auto=format&fit=crop&w=1200&q=80)

- **Posts** — artikel blog dengan kategori, tag, dan dukungan multi-bahasa
- **Pages** — halaman statis seperti Home, About, Contact
- **Categories & Tags** — sistem taksonomi yang reusable lintas konten
- **Multi-language** — konten tersedia dalam berbagai bahasa

---

### ⚙️ Sistem & Infrastruktur

| Fitur | Deskripsi |
|-------|-----------|
| **Multi-Tenant** | Setiap bisnis terisolasi dengan data dan pengaturan sendiri |
| **Menu Management** | Navigasi dinamis dengan menu nested per tenant |
| **Site Settings** | Konfigurasi global per tenant (nama, logo, SEO) |
| **Role & Permissions** | Kontrol akses granular per pengguna |
| **Audit Trail** | Rekam semua aktivitas dan revisi konten |
| **Subscriptions** | Langganan berulang untuk model bisnis recurring |

---

## Mulai dari Mana?

{% hint style="info" %}
Jika Anda baru pertama kali menggunakan Elshobah, mulailah dengan memahami konsep **Tenant** — semua data Anda terikat pada tenant yang Anda miliki.
{% endhint %}

<table data-view="cards">
  <thead>
    <tr>
      <th></th>
      <th></th>
      <th data-hidden data-card-target data-type="content-ref"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>🚀 Quick Start</strong></td>
      <td>Setup tenant pertama Anda dalam 5 menit</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>🛍️ E-Commerce Guide</strong></td>
      <td>Tambah produk, kelola order, dan terima pembayaran</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>🎓 LMS Guide</strong></td>
      <td>Buat dan publikasikan kursus online pertama Anda</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>✍️ Content Guide</strong></td>
      <td>Tulis artikel blog dan kelola halaman konten</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>💳 Payment Setup</strong></td>
      <td>Konfigurasi Midtrans atau Xendit untuk menerima pembayaran</td>
      <td></td>
    </tr>
    <tr>
      <td><strong>🔌 API Reference</strong></td>
      <td>Integrasi Elshobah dengan aplikasi Anda via REST/GraphQL</td>
      <td></td>
    </tr>
  </tbody>
</table>

---

## Arsitektur Platform

```
Tenant (bisnis Anda)
├── 🛍️ E-Commerce
│   ├── Products (katalog)
│   ├── Orders & Order Items
│   ├── Invoices
│   └── Payments (via Midtrans / Xendit)
│
├── 🎓 LMS
│   ├── Courses
│   ├── Course Modules
│   ├── Course Lessons
│   └── Course Enrollments
│
├── ✍️ Content
│   ├── Posts (blog)
│   ├── Pages (statis)
│   ├── Categories & Tags
│   └── Multi-language Support
│
└── ⚙️ Sistem
    ├── Customers
    ├── Menus & Navigation
    ├── Site Settings
    └── Subscriptions
```

---

## Butuh Bantuan?

Jika Anda menemui kendala atau memiliki pertanyaan, tim kami siap membantu:

- 🌐 **Website:** [elshobah.com](https://elshobah.com)
- 📧 **Email:** support@elshobah.com
- 📖 **Dokumentasi:** [panduan.elshobah.com](https://panduan.elshobah.com)

---

*Dokumentasi ini diperbarui secara berkala. Terakhir diperbarui: Mei 2026.*
