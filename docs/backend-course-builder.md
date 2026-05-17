---
description: Panduan lengkap membuat kursus online menggunakan Tutor LMS di WordPress — dari judul, modul, lesson, quiz, hingga pengaturan lanjutan.
---

# Membuat Kursus dengan Tutor LMS

Tutor LMS adalah plugin WordPress yang digunakan untuk membangun dan menjual kursus online. Panduan ini menjelaskan seluruh proses pembuatan kursus dari backend WordPress.

{% embed url="https://www.youtube.com/watch?v=twmVHKiAqTk" %}

**Akses via:** WordPress Admin → **Tutor LMS** → **Kursus** → **Tambah Baru**

---

## 1. Judul & Deskripsi Kursus

### Judul Kursus

Buat judul yang informatif namun ringkas. Pastikan mencakup:

| Elemen | Contoh |
|--------|--------|
| **Subjek** | PHP, Desain UX, Penulisan Konten |
| **Tingkat kesulitan** | untuk Pemula / Mahir / Lanjutan |
| **Jenis kursus** | Panduan Lengkap / Seri Bagian 1 |

**Contoh judul yang baik:**
- ✅ "Belajar PHP untuk Pemula — Dari Nol hingga Membuat Website"
- ❌ "Kursus PHP"

### Deskripsi Kursus

Tulis deskripsi yang mencakup:

- Apa yang akan dipelajari (pelajaran & kuis)
- Hasil pembelajaran yang dapat dicapai siswa
- Ringkasan silabus kursus

---

## 2. Pengaturan Kursus

| Pengaturan | Fungsi |
|-----------|--------|
| **Siswa Maksimum** | Batasi jumlah pendaftar (berguna untuk kelas eksklusif) |
| **Periode Pendaftaran** | Durasi akses kursus dalam hari setelah enrollment |
| **Tingkat Kesulitan** | Indikator level untuk calon siswa |
| **Content Drip** | Atur jadwal rilis konten secara bertahap (add-on) |
| **Kategori** | Kelola di WP Admin → Tutor LMS Pro → Kategori |
| **Thumbnail** | Gambar sampul kursus |

{% hint style="info" %}
Aktifkan **Periode Pendaftaran** di: WP Admin → Tutor LMS → Pengaturan
{% endhint %}

---

## 3. Course Attachments (Lampiran)

Sediakan materi pendukung yang dapat diunduh siswa:

- File latihan (exercise files)
- Template atau contoh project
- Materi referensi tambahan (PDF, slide, dll.)

Siswa dapat mengunduh file ini langsung dari halaman kursus.

---

## 4. Course Prerequisites (Prasyarat)

Tetapkan kursus yang **wajib diselesaikan terlebih dahulu** sebelum mengakses kursus ini.

**Contoh alur:**

```
Basics of Programming  →  Advanced Programming  →  Expert Programming
     (prasyarat)              (prasyarat)
```

Fitur ini membantu Anda membangun jalur pembelajaran (learning path) yang terstruktur.

---

## 5. Course Builder

Ini adalah inti pembuatan kursus. Struktur konten mengikuti hierarki:

```
Kursus
└── Topik
    ├── Pelajaran (Lesson)
    └── Kuis (Quiz)
```

{% hint style="success" %}
**Rekomendasi struktur:** 2–5 pelajaran dan 1 kuis per topik untuk pengalaman belajar yang optimal.
{% endhint %}

### Menambah Topik Baru

1. Klik **"Tambah Topik Baru"**
2. Isi nama dan ringkasan topik
3. Tambahkan pelajaran dan kuis dari tombol di bawah topik

![Antarmuka penambahan topik baru di Course Builder](https://is3.cloudhost.id/elsweb/2022/07/image-5.png)

### Lesson (Pelajaran)

Setiap pelajaran terdiri dari:

| Komponen | Keterangan |
|----------|-----------|
| **Judul** | Nama pelajaran |
| **Deskripsi** | Penjelasan singkat isi pelajaran |
| **Gambar unggulan** | Thumbnail pelajaran (opsional) |
| **Video** | Sumber video eksternal atau internal + durasi |
| **Lampiran** | Materi tambahan untuk pelajaran ini |

![Struktur form lesson — judul, deskripsi, dan gambar unggulan](https://is3.cloudhost.id/elsweb/2022/07/image-6.png)

**Sumber video yang didukung:**
- Self-hosted (upload langsung)
- YouTube
- Vimeo
- Embed URL lainnya

![Opsi sumber video dan upload lampiran pada lesson](https://is3.cloudhost.id/elsweb/2022/07/image-7.png)

### Quiz (Kuis)

Kuis memiliki fitur yang sangat lengkap — lihat dokumentasi terpisah di **Quiz Builder** untuk panduan detail.

### Fitur Pro

| Fitur | Keterangan |
|-------|-----------|
| **Kuis Impor** | Import kuis dari file via addon Impor/Ekspor |
| **Tugas (Assignment)** | Berikan tugas tertulis kepada siswa |
| **Pelajaran Langsung** | Sesi live via integrasi Zoom |

{% hint style="warning" %}
Fitur Live Class membutuhkan akun Zoom yang aktif.
{% endhint %}

---

## 6. Additional Data (Informasi Pemasaran)

Informasi ini ditampilkan di halaman kursus untuk menarik calon siswa:

| Field | Keterangan | Format |
|-------|-----------|--------|
| **Course Duration** | Estimasi total waktu belajar | — |
| **Benefits** | Skill & pengetahuan yang akan dikuasai | Satu poin per baris |
| **Requirements** | Prasyarat atau persiapan yang dibutuhkan | Satu poin per baris |
| **Target Audience** | Siapa yang paling cocok mengikuti kursus ini | Satu poin per baris |
| **Materials Included** | Aset yang akan diterima siswa | Satu poin per baris |

---

## 7. Tutor Settings

| Pengaturan | Efek |
|-----------|------|
| **Jadikan Publik** | Semua orang bisa akses tanpa perlu mendaftar |
| **Nonaktifkan Tanya Jawab** | Menutup forum Q&A kursus |
| **Nonaktifkan Sertifikat** | Siswa tidak mendapat sertifikat selesai |

---

## 8. Video Pengantar Kursus

Tambahkan video intro yang muncul di halaman overview kursus — ini adalah "trailer" kursus Anda.

**Sumber video yang didukung:**
- Video self-hosted (`.mp4`)
- YouTube
- Vimeo
- Embed URL kustom

---

## Checklist Sebelum Publish Kursus

- [ ] Judul informatif dan mengandung keyword
- [ ] Deskripsi lengkap dan menarik
- [ ] Thumbnail kursus sudah diset
- [ ] Minimal 1 topik dengan 1 pelajaran sudah dibuat
- [ ] Benefits & Target Audience sudah diisi
- [ ] Harga sudah dikonfigurasi (jika kursus berbayar)
- [ ] Video pengantar sudah ditambahkan

---

*Kategori: Pengetahuan Dasar · Diperbarui: 1 Agustus 2022*
