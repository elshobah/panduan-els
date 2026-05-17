---
description: Cara mengelola kategori kursus di Tutor LMS untuk mengorganisasi konten pembelajaran secara terstruktur.
---

# Menu Kategori

Kategori adalah bagian penting dari hierarki manajemen konten di Tutor LMS, terutama untuk platform dengan banyak instruktur dan kursus. Kategori memudahkan pengorganisasian dan pemfilteran kursus.

**Akses via:** WordPress Admin → **Tutor LMS** → **Kategori**

{% hint style="info" %}
Buat kategori sebelum mulai membuat kursus — ini memudahkan pengelompokan sejak awal.
{% endhint %}

---

## Tampilan Menu

![Tampilan Menu Kategori Tutor LMS](https://is3.cloudhost.id/elsweb/2022/07/image-2.png)

---

## Menambah Kategori Baru

Di sisi kiri halaman, isi form berikut:

| Field | Keterangan |
|-------|-----------|
| **Nama** | Nama kategori yang jelas dan relevan (contoh: "Pemrograman Web", "Desain Grafis") |
| **Slug** | URL-friendly identifier — dibuat otomatis, dapat diubah manual |
| **Induk** | Pilih kategori induk untuk membuat sub-kategori (hierarki) |
| **Deskripsi** | Penjelasan singkat jenis kursus dalam kategori ini |
| **Thumbnail** | Gambar yang ditampilkan di halaman arsip dan daftar kursus |

Klik **Tambah Kategori Baru** untuk menyimpan.

---

## Membuat Hierarki Kategori

Anda dapat membuat struktur kategori bertingkat:

```
Teknologi (induk)
├── Pemrograman Web
│   ├── HTML & CSS
│   └── JavaScript
└── Mobile Development
    ├── Android
    └── iOS
```

Pilih kategori induk pada field **Induk** saat membuat sub-kategori.

---

## Mengedit Kategori

Di daftar kategori (sisi kanan), arahkan kursor ke nama kategori untuk memunculkan opsi:

| Opsi | Fungsi |
|------|--------|
| **Edit** | Buka halaman edit lengkap |
| **Edit Cepat** | Ubah nama dan slug langsung tanpa pindah halaman |
| **Hapus** | Hapus kategori (kursus di dalamnya tidak ikut terhapus) |
| **Lihat** | Buka halaman arsip kategori di frontend |

---

## Navigasi Terkait

- ← [Menu Announcement](tutor-lms-menu-announcement.md)
- [Menu Kursus](tutor-lms-menu-kursus.md) →

---

*Kategori: Tutor LMS · Diperbarui: 20 Juli 2022*
