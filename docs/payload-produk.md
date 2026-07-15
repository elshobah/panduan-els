---
description: Cara membuat dan mengedit produk di Payload — foto utama, galeri, deskripsi, spesifikasi, harga, status stok, dan tombol WhatsApp.
---

# Membuat dan Mengedit Produk di Payload

Produk dikelola di koleksi **Products**, di dalam grup menu **Produk** pada sidebar. Panduan ini menjelaskan cara menambah produk baru sampai siap tayang.

---

## Prasyarat

- Anda sudah bisa login ke admin Payload — lihat [Login dan Mengenal Dashboard Payload](payload-login-dashboard.md)
- Anda sudah paham alur draft dan publish — lihat [Draft, Preview, dan Publish di Payload](payload-draft-preview-publish.md)
- Foto produk sudah diunggah — lihat [Mengelola Media di Payload](payload-media-library.md)
- Kategori produk sudah dibuat di menu **Product Categories**

---

## Langkah-Langkah

### 1. Buat Produk Baru

Di sidebar kiri, buka grup **Produk** lalu klik **Products**. Klik **Create New**.

### 2. Isi Nama Produk

Field **Title** wajib diisi. Ini nama produk yang tampil di website dan menjadi dasar slug.

Tulis nama yang sesuai cara orang mencarinya. "Pupuk Organik Granul 5 kg" lebih baik daripada "POG-5000" — kode internal tidak dicari siapa pun.

### 3. Periksa Slug

Di sidebar kanan, **Slug** terisi otomatis dari nama produk. Klik ikon gembok kalau ingin mengubahnya.

---

### 4. Isi Tab Konten

Klik tab **Konten**.

| Field | Keterangan | Wajib |
|-------|-----------|-------|
| **Featured Image** | Foto utama produk — tampil di daftar produk dan bagian atas halaman produk | Ya |
| **Galeri Foto** | Foto tambahan dari sudut lain | Opsional |
| **Deskripsi** | Penjelasan lengkap produk, memakai editor Lexical | Opsional |
| **Spesifikasi** | Detail teknis dalam bentuk pasangan label dan nilai | Opsional |

Untuk menambah foto galeri, klik **Add Galeri Foto** lalu pilih gambar. Ulangi sebanyak yang dibutuhkan, dan seret untuk mengatur urutan.

{% hint style="success" %}
**Featured Image** adalah satu-satunya foto yang tampil di daftar produk, jadi pilih yang paling jelas menunjukkan wujud produk. Sudut-sudut lain, detail kemasan, dan foto produk saat dipakai lebih cocok masuk **Galeri**.
{% endhint %}

Untuk **Spesifikasi**, klik **Add Spesifikasi** lalu isi dua field — keduanya wajib:

| Label | Value |
|-------|-------|
| `Berat` | `5 kg` |
| `Kemasan` | `Karung plastik` |
| `Isi` | `20 sachet` |

Hasilnya tampil sebagai tabel rapi di halaman produk.

{% hint style="info" %}
Di editor **Deskripsi**, sub-judul dimulai dari **H2** — H1 sudah dipakai oleh nama produk.
{% endhint %}

---

### 5. Isi Tab Harga & Stok

Klik tab **Harga & Stok**.

| Field | Keterangan |
|-------|-----------|
| **Harga (Rp)** | Isi angkanya saja, tanpa titik atau "Rp" — misalnya `150000` |
| **Catatan Harga** | Keterangan di sebelah harga, misalnya `per batang`, `nego`, `hubungi kami` |
| **Status Stok** | Pilih **Ready** atau **Pre-order** |
| **Template Pesan WhatsApp** | Pesan yang terisi otomatis saat pembeli menekan tombol WhatsApp |

{% hint style="info" %}
**Harga** boleh dikosongkan untuk produk yang harganya harus dinegosiasi. Isi **Catatan Harga** dengan `Hubungi kami` supaya pengunjung tetap tahu harus berbuat apa.
{% endhint %}

**Template Pesan WhatsApp** sudah punya isi bawaan yang umum. Ubah kalau produk ini butuh informasi khusus dari pembeli — misalnya jumlah pesanan atau lokasi pengiriman.

{% hint style="success" %}
Jaga **Status Stok** tetap akurat. Pembeli yang menghubungi lewat WhatsApp untuk produk bertanda Ready lalu diberi tahu barangnya kosong hampir pasti tidak kembali lagi.
{% endhint %}

---

### 6. Pilih Kategori dan Produk Terkait

Di sidebar kanan:

- **Category** — kategori produk. Berbeda dengan artikel, satu produk hanya punya **satu** kategori
- **Related Products** — produk lain yang disarankan di bagian bawah halaman. Produk yang sedang dibuka otomatis tidak muncul di pilihan

{% hint style="success" %}
Isi **Related Products** dengan produk yang benar-benar saling melengkapi, bukan asal produk sejenis. Pembeli pupuk kemungkinan butuh media tanam — itu yang membuat mereka menambah belanjaan.
{% endhint %}

---

### 7. Isi Tab SEO

Klik tab **SEO**.

| Field | Keterangan | Panjang ideal |
|-------|-----------|---------------|
| **Title** | Judul di hasil pencarian Google | 50–60 karakter |
| **Description** | Deskripsi di bawah judul | 150–160 karakter |
| **Image** | Gambar preview saat tautan dibagikan ke WhatsApp | 1200 × 630px |

Tombol **Auto-generate** mengisi Title dari nama produk. Sunting seperlunya.

{% hint style="success" %}
Untuk produk, masukkan hal yang dicari pembeli ke dalam **Description**: harga, ukuran, atau ketersediaan. "Pupuk organik granul 5 kg, siap kirim, mulai Rp150.000" lebih menarik diklik daripada kalimat promosi umum.
{% endhint %}

---

### 8. Preview dan Publikasikan

Field **Published At** di sidebar kanan terisi otomatis saat Anda menekan Publish, jadi biarkan kosong kecuali Anda ingin tanggal tertentu.

Cek lewat **Live Preview** — terutama ukuran **Mobile**, karena hampir semua pembeli membuka halaman produk dari ponsel. Lalu klik **Publish**.

---

## Checklist Sebelum Publish

- [ ] **Title** memakai nama yang dicari orang, bukan kode internal
- [ ] **Featured Image** sudah dipilih dan alt text-nya terisi
- [ ] **Galeri Foto** sudah diisi foto dari sudut lain
- [ ] **Deskripsi** lengkap, sub-judul mulai dari H2
- [ ] **Spesifikasi** sudah diisi
- [ ] **Harga** dan **Catatan Harga** sudah benar
- [ ] **Status Stok** sesuai kondisi sebenarnya
- [ ] **Template Pesan WhatsApp** sudah dicek
- [ ] **Category** sudah dipilih
- [ ] **Related Products** sudah dipilih
- [ ] Tab **SEO** — Title, Description, dan Image sudah diisi
- [ ] Sudah dicek di **Live Preview** ukuran Mobile

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS with Payload · Diperbarui: 15 Juli 2026*
