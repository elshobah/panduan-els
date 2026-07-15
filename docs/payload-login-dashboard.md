---
description: Cara login ke panel admin Payload dan mengenal bagian-bagian dashboard — sidebar, koleksi, dan pengaturan akun.
---

# Login dan Mengenal Dashboard Payload

Panduan ini menjelaskan cara masuk ke panel admin **Payload** dan mengenali bagian-bagian utamanya. Baca ini lebih dulu sebelum panduan lain, karena istilah di sini dipakai di seluruh dokumentasi ElsCMS with Payload.

---

## Prasyarat

Sebelum mulai, pastikan:

- Anda sudah menerima **alamat website** dan **akun admin** (email + password) dari tim Elshobah
- Anda menggunakan browser versi terbaru — Chrome, Edge, atau Firefox

---

## Langkah-Langkah

### 1. Buka Halaman Admin

Tambahkan `/admin` di belakang alamat website Anda, lalu buka di browser.

Contoh: jika website Anda `https://namawebsite.com`, maka halaman admin ada di `https://namawebsite.com/admin`

### 2. Masuk dengan Email dan Password

Isi **Email** dan **Password** yang diberikan tim Elshobah, lalu klik **Login**.

{% hint style="warning" %}
Jangan bagikan akun admin Anda ke orang lain. Jika ada anggota tim yang perlu akses, buatkan akun terpisah lewat menu **Users** — supaya jelas siapa mengubah apa.
{% endhint %}

### 3. Lupa Password?

Klik **Forgot password?** di halaman login. Payload akan mengirim tautan reset ke email Anda.

Jika email tidak masuk dalam beberapa menit, cek folder spam. Kalau tetap tidak ada, hubungi tim Elshobah.

---

### 4. Kenali Sidebar

Setelah login, Anda akan melihat daftar koleksi di sidebar kiri. Inilah tempat semua konten website dikelola:

| Menu | Isinya |
|------|--------|
| **Pages** | Halaman website — Beranda, Tentang Kami, Kontak, dan sebagainya |
| **Posts** | Artikel, berita, dan blog |
| **Media** | Semua gambar dan file yang diunggah |
| **Categories** | Kategori untuk artikel |
| **Projects** | Portofolio atau proyek yang ditampilkan di website |
| **Users** | Daftar akun yang bisa masuk ke admin — hanya tampil untuk Admin |

Di grup **Produk** terdapat dua menu terpisah:

| Menu | Isinya |
|------|--------|
| **Products** | Daftar produk |
| **Product Categories** | Kategori produk |

{% hint style="info" %}
Menu **Forms**, **Form Submissions**, **Redirects**, dan **Search** juga muncul di sidebar. Ketiganya dibahas di panduan tersendiri — **Search** terisi otomatis dan tidak perlu Anda sentuh.
{% endhint %}

---

### 5. Kenali Bagian Atas Sidebar

Di bagian bawah sidebar ada dua menu global yang tidak berbentuk daftar:

- **Header** — mengatur menu navigasi di bagian atas website
- **Footer** — mengatur tautan di bagian bawah website

Berbeda dengan koleksi, keduanya hanya berisi **satu dokumen** yang diedit langsung.

---

### 6. Buka Sebuah Koleksi

Klik salah satu menu, misalnya **Posts**. Anda akan melihat daftar dokumen dengan beberapa kontrol:

| Kontrol | Fungsi |
|---------|--------|
| **Create New** | Membuat dokumen baru |
| **Search** | Mencari dokumen berdasarkan judul |
| **Filters** | Menyaring daftar, misalnya hanya yang berstatus draft |
| **Columns** | Memilih kolom yang tampil di daftar |

Klik judul dokumen mana pun untuk membukanya.

---

### 7. Ubah Akun Anda Sendiri

Klik ikon akun di pojok kanan bawah sidebar, lalu pilih **Account** untuk mengubah nama atau password Anda. Halaman ini bisa diakses semua role, termasuk Editor.

Klik **Log out** untuk keluar.

---

## Hak Akses: Admin dan Editor

Setiap akun punya salah satu dari dua role:

| Role | Boleh melakukan |
|------|-----------------|
| **Editor** | Membuat dan mengedit semua konten — halaman, artikel, produk, proyek, media, kategori — serta mempublikasikan dan menariknya dari website |
| **Admin** | Semua yang bisa dilakukan Editor, **ditambah** menghapus konten dan mengelola akun user |

Perbedaan pentingnya ada di **menghapus**. Editor bisa mengubah apa saja, tapi tidak bisa menghapus dokumen apa pun — tombol hapusnya tidak akan berfungsi untuk mereka.

{% hint style="info" %}
Menu **Users** hanya muncul di sidebar untuk Admin. Kalau Anda tidak melihatnya, artinya akun Anda berrole Editor — dan itu memang semestinya.
{% endhint %}

{% hint style="success" %}
Batasan hapus ini adalah pengaman, bukan hambatan. Editor tetap bisa menarik konten dari website lewat **Unpublish** kapan pun — dan cara itu memang lebih baik daripada menghapus, karena isinya masih bisa dikembalikan sewaktu-waktu.
{% endhint %}

### Menambah User Baru (Admin saja)

Klik menu **Users**, lalu **Create New**. Isi **Name**, **Email**, dan **Password**, kemudian pilih **Roles**.

Role bawaan untuk user baru adalah **Editor**. Naikkan ke Admin hanya untuk orang yang memang perlu menghapus konten atau mengelola akun lain.

{% hint style="warning" %}
Field **Roles** hanya bisa diubah oleh Admin. Editor tidak dapat menaikkan role-nya sendiri dari halaman akunnya — ini disengaja.
{% endhint %}

---

## Checklist Setelah Login Pertama

- [ ] Berhasil masuk ke `/admin`
- [ ] Password bawaan sudah diganti lewat menu **Account**
- [ ] Sudah tahu role akun Anda — Admin atau Editor
- [ ] Sudah tahu letak **Pages**, **Posts**, **Media**, dan **Products**
- [ ] Sudah tahu letak **Header** dan **Footer**

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS with Payload · Diperbarui: 15 Juli 2026*
