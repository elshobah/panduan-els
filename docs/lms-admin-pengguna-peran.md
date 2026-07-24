---
description: Mengelola pengguna dan peran (role) di LMS Indonesia — memahami enam peran, siapa boleh apa, mengangkat instruktur, mendaftarkan peserta, dan membatasi akses.
---

# Mengelola Pengguna dan Peran

Setiap orang di lembaga Anda — admin, instruktur, staf keuangan, peserta, afiliasi — adalah satu **Pengguna** dengan satu atau beberapa **peran (role)**. Peran menentukan apa yang boleh dan tidak boleh dilakukan seseorang. Halaman ini menjelaskan cara mengelolanya lewat menu **Pengguna** di grup **Manajemen**.

---

## Prasyarat

- Anda sudah bisa login ke panel admin — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Untuk mengubah peran pengguna, akun Anda harus **Super Admin** atau **Admin**

---

## Enam Peran di LMS Indonesia

Setiap tenant memiliki enam peran bawaan. Peran ter-*scope* pada lembaga Anda — artinya seseorang yang menjadi admin di lembaga Anda tidak otomatis menjadi admin di lembaga lain.

| Peran | Untuk siapa | Akses panel `/admin` |
|-------|-------------|:--------------------:|
| **Super Admin** | Pemilik lembaga | ✅ Penuh |
| **Admin** | Pengelola harian | ✅ Terbatas |
| **Financial (Keuangan)** | Staf keuangan | ✅ Hanya transaksi |
| **Instructor (Instruktur)** | Pengajar | ❌ |
| **Student (Siswa)** | Peserta belajar | ❌ |
| **Affiliate (Afiliasi)** | Mitra pemasaran | ❌ |

{% hint style="info" %}
Instruktur, Siswa, dan Afiliasi **tidak masuk** ke panel `/admin`. Mereka menggunakan halaman depan website: instruktur mengelola materinya lewat dashboard pengajar, siswa belajar, afiliasi memantau komisinya.
{% endhint %}

---

## Siapa Boleh Apa

Perbedaan terpenting adalah antara **Super Admin** dan **Admin**. Keduanya bisa mengelola konten dan pengguna, tetapi beberapa aksi berisiko **hanya boleh dilakukan Super Admin**.

| Aksi | Super Admin | Admin | Keuangan |
|------|:-----------:|:-----:|:--------:|
| Lihat & buat kursus | ✅ | ✅ | ❌ |
| Publikasikan kursus | ✅ | ✅ | ❌ |
| **Hapus kursus** | ✅ | ❌ | ❌ |
| Kelola pelajaran | ✅ | ✅ | ❌ |
| Lihat & ubah status order | ✅ | ✅ | ✅ |
| **Refund order** | ✅ | ❌ | ❌ |
| Lihat & ubah pengguna | ✅ | ✅ | ❌ |
| **Ban pengguna** | ✅ | ❌ | ❌ |
| Kelola kupon | ✅ | ✅ | ❌ |
| Lihat afiliasi & setujui penarikan | ✅ | ✅ | ❌ |
| **Kelola program afiliasi (rate komisi)** | ✅ | ❌ | ❌ |
| Lihat laporan | ✅ | ✅ | ✅ |
| **API Key & Log Aktivitas** | ✅ | ❌ | ❌ |

{% hint style="warning" %}
Peran **Keuangan** sengaja dibuat sangat terbatas: staf keuangan hanya melihat grup **Transaksi** dan **Donasi** untuk mencocokkan pembayaran dengan mutasi bank dan mengonfirmasi transfer manual. Menu konten, pengguna, afiliasi, pengaturan, dan tombol refund **disembunyikan** dari mereka.
{% endhint %}

---

## Langkah-Langkah

### 1. Buka Daftar Pengguna

Klik **Manajemen → Pengguna** di sidebar. Anda akan melihat tabel berisi semua pengguna lembaga Anda beserta peran, jumlah kursus yang diikuti, dan tanggal bergabung.

![Daftar pengguna](https://GANTI-DENGAN-SCREENSHOT)

Gunakan filter **Role** di kanan atas untuk menyaring, misalnya hanya menampilkan instruktur.

### 2. Melihat Detail Pengguna

Klik ikon **lihat** (mata) pada baris pengguna untuk membuka profilnya: informasi kontak, alamat, bio, status verifikasi email, dan daftar kursus yang diikuti.

### 3. Mengubah Peran Pengguna

Klik **Edit** pada baris pengguna, lalu buka bagian **Role & Akses**. Centang peran yang ingin diberikan (bisa lebih dari satu), lalu klik **Save**.

![Bagian Role & Akses saat mengedit pengguna](https://GANTI-DENGAN-SCREENSHOT)

{% hint style="danger" %}
Berhati-hatilah memberikan peran **Super Admin** — peran ini bisa melakukan **semua** hal, termasuk menghapus kursus, me-refund pembayaran, dan mengelola API Key. Berikan hanya kepada orang yang benar-benar Anda percaya.
{% endhint %}

### 4. Mengangkat Seseorang Jadi Instruktur

Untuk cepat menjadikan pengguna sebagai pengajar, gunakan tombol aksi **Jadikan Instruktur** pada baris pengguna. Peran instruktur akan ditambahkan dan dicatat di Log Aktivitas.

Setelah itu, pengguna tersebut bisa dipilih sebagai **Instruktur / Pembicara** saat Anda membuat kursus.

### 5. Mendaftarkan Peserta ke Kursus (Enroll Manual)

Kadang Anda perlu memberi akses kursus tanpa lewat pembelian — misalnya untuk peserta undangan. Gunakan aksi **Enroll Kursus** pada baris pengguna, pilih kursus yang sudah dipublikasikan, lalu jalankan.

### 6. Mem-*ban* Pengguna

Aksi **Ban** akan mencabut sesi login (token) pengguna. Aksi ini **hanya tersedia untuk Super Admin** dan tidak bisa dikenakan ke sesama Super Admin.

---

## Catatan tentang Data Kontak & Alamat

Field seperti nomor HP, WhatsApp, Instagram, dan alamat pada profil pengguna umumnya **hanya-baca** dari sisi admin — data itu diisi sendiri oleh pengguna dari akunnya. Admin dapat melihat dan menghubungi (tersedia tombol pintas buka WhatsApp/Instagram), tetapi tidak mengubahnya sembarangan.

---

## Checklist Mengelola Pengguna

- [ ] Memahami perbedaan Super Admin vs Admin vs Keuangan
- [ ] Tahu bahwa Instruktur/Siswa/Afiliasi tidak masuk panel `/admin`
- [ ] Bisa menambah/mengubah peran lewat bagian **Role & Akses**
- [ ] Memberikan peran Super Admin hanya kepada orang tepercaya
- [ ] Tahu cara mengangkat instruktur dan meng-*enroll* peserta manual

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
