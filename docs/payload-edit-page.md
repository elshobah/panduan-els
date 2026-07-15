---
description: Cara membuat dan mengedit halaman website di Payload — mengatur Hero, menyusun Layout dengan block, dan mengisi SEO.
---

# Membuat dan Mengedit Halaman di Payload

Halaman website — Beranda, Tentang Kami, Layanan, Kontak — dikelola di koleksi **Pages**. Berbeda dengan artikel yang isinya satu tulisan panjang, halaman disusun dari **block** yang bisa ditumpuk dan diurutkan sesuai kebutuhan.

---

## Prasyarat

- Anda sudah bisa login ke admin Payload — lihat [Login dan Mengenal Dashboard Payload](payload-login-dashboard.md)
- Anda sudah paham alur draft dan publish — lihat [Draft, Preview, dan Publish di Payload](payload-draft-preview-publish.md)
- Gambar yang akan dipakai sudah diunggah — lihat [Mengelola Media di Payload](payload-media-library.md)

---

## Langkah-Langkah

### 1. Buka Koleksi Pages

Klik menu **Pages** di sidebar kiri, lalu klik **Create New** untuk halaman baru — atau klik judul halaman yang sudah ada untuk mengeditnya.

### 2. Isi Judul

Field **Title** di bagian atas wajib diisi. Judul ini dipakai sebagai nama halaman di dalam admin, dan biasanya juga tampil di website.

### 3. Periksa Slug

Di sidebar kanan ada field **Slug** — bagian alamat halaman setelah nama domain. Slug terisi otomatis dari judul.

Contoh: judul "Tentang Kami" menghasilkan slug `tentang-kami`, sehingga alamatnya `namawebsite.com/tentang-kami`

Untuk mengubahnya, klik ikon gembok di sebelah field lalu ketik slug baru.

{% hint style="danger" %}
Jangan mengubah slug halaman yang **sudah tayang dan sudah dibagikan**. Semua tautan lama ke halaman itu akan mati.

Kalau memang harus diubah, buat **Redirect** dari slug lama ke slug baru supaya pengunjung tidak tersesat.
{% endhint %}

---

### 4. Atur Hero

Klik tab **Hero**. Hero adalah bagian paling atas halaman — hal pertama yang dilihat pengunjung.

Pilih **Type** sesuai kebutuhan:

| Type | Kapan dipakai |
|------|---------------|
| **None** | Halaman tanpa hero, langsung masuk ke isi |
| **High Impact** | Gambar besar memenuhi layar — cocok untuk Beranda |
| **Medium Impact** | Gambar dengan porsi sedang |
| **Split Impact** | Teks di satu sisi, gambar di sisi lain |
| **Low Impact** | Hanya teks, tanpa gambar — cocok untuk halaman biasa |

Setelah memilih Type, isi bagian berikut:

- **Rich Text** — judul dan teks pembuka hero
- **Links** — tombol ajakan, maksimal **2 tombol**
- **Media** — gambar hero. **Wajib** untuk High Impact, Medium Impact, dan Split Impact

Khusus **Split Impact**, muncul dua field tambahan:

- **Teks Rating** — angka atau capaian singkat, misalnya `320+`
- **Sub-teks Rating** — keterangannya, misalnya `Klien Puas`

{% hint style="info" %}
Field yang tidak relevan otomatis disembunyikan. Kalau ada field yang Anda cari tapi tidak muncul, kemungkinan besar **Type** hero-nya belum sesuai.
{% endhint %}

---

### 5. Susun Layout dengan Block

Klik tab **Content**. Di sinilah isi halaman dirakit.

Klik **Add Block**, lalu pilih block yang dibutuhkan. Ulangi untuk menambah block berikutnya — halaman dibaca dari block paling atas ke paling bawah.

Block yang tersedia:

| Block | Fungsinya |
|-------|-----------|
| **Content** | Teks bebas, bisa dibagi menjadi beberapa kolom |
| **Media Block** | Menampilkan satu gambar |
| **Call to Action** | Kotak ajakan dengan tombol |
| **Archive** | Menampilkan daftar artikel otomatis |
| **Arsip Produk** | Menampilkan daftar produk |
| **Arsip Proyek** | Menampilkan daftar proyek atau portofolio |
| **Form Block** | Memasang formulir yang dibuat di menu Forms |
| **Service Cards** | Kartu-kartu layanan dengan ikon |
| **Feature Grid** | Kisi keunggulan dengan ikon |
| **Trust Bar** | Deretan logo klien |
| **About Intro** | Blok perkenalan dengan poin unggulan |
| **Tim** | Kisi foto dan jabatan anggota tim |
| **Testimoni** | Kutipan pelanggan, lengkap dengan rating |
| **FAQ** | Daftar tanya-jawab yang bisa dibuka-tutup |

{% hint style="info" %}
Daftar block bisa **berbeda di tiap website**, menyesuaikan kebutuhan masing-masing. Yang tampil di admin Anda adalah yang berlaku.
{% endhint %}

### 6. Atur Urutan dan Rapikan

Setiap block punya kontrol di sisi kanannya:

| Kontrol | Fungsi |
|---------|--------|
| Titik enam (⣿) | Seret untuk memindah urutan block |
| Panah ▸ | Buka atau tutup isi block |
| Menu ⋯ | Duplicate, Remove, atau Copy block |

Block baru muncul dalam keadaan tertutup supaya daftar tetap ringkas. Klik panahnya untuk mengisi.

{% hint style="success" %}
Butuh tiga kartu layanan yang mirip? Isi satu sampai selesai, lalu **Duplicate** dua kali dan ubah isinya. Jauh lebih cepat daripada membuat dari nol.
{% endhint %}

---

### 7. Isi Tab SEO

Klik tab **SEO**. Isi bagian ini menentukan tampilan halaman Anda di hasil pencarian Google dan saat dibagikan ke WhatsApp.

| Field | Keterangan |
|-------|-----------|
| **Title** | Judul di hasil pencarian Google |
| **Description** | Deskripsi singkat di bawah judul |
| **Image** | Gambar preview saat tautan dibagikan ke WhatsApp atau media sosial |

Tombol **Auto-generate** mengisi Title secara otomatis dari judul halaman. Hasilnya bisa Anda sunting.

Di bagian bawah ada **Preview** — simulasi tampilan di Google. Gunakan untuk memastikan judul dan deskripsi tidak terpotong.

{% hint style="success" %}
Panjang ideal: **Title** sekitar 50–60 karakter, **Description** sekitar 150–160 karakter. Payload menampilkan penghitung karakter dengan indikator warna — jaga tetap hijau.
{% endhint %}

---

### 8. Preview dan Publikasikan

Klik tab **Live Preview** untuk melihat hasil susunan block Anda, lalu cek tampilan **Mobile** dan **Desktop**.

Kalau sudah rapi, klik **Publish**. Selengkapnya di [Draft, Preview, dan Publish di Payload](payload-draft-preview-publish.md).

---

## Checklist Sebelum Publish

- [ ] **Title** sudah diisi
- [ ] **Slug** sudah sesuai dan tidak mengubah halaman lama tanpa redirect
- [ ] **Hero** sudah diatur, dan gambarnya terpasang jika Type-nya butuh gambar
- [ ] Urutan **block** sudah runut dari atas ke bawah
- [ ] Tidak ada block kosong yang terlanjur ditambahkan
- [ ] Tab **SEO** — Title, Description, dan Image sudah diisi
- [ ] Sudah dicek di **Live Preview** ukuran Mobile dan Desktop

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS with Payload · Diperbarui: 15 Juli 2026*
