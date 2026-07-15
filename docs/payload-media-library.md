---
description: Cara mengunggah dan mengelola gambar di koleksi Media Payload — alt text, focal point, folder, dan ukuran gambar otomatis.
---

# Mengelola Media di Payload

Semua gambar yang dipakai di website — foto produk, gambar utama artikel, logo, foto tim — disimpan di koleksi **Media**. Panduan ini menjelaskan cara mengunggah dan mengelolanya dengan benar.

---

## Prasyarat

Sebelum mengunggah, pastikan:

- Anda sudah bisa login ke admin Payload — lihat [Login dan Mengenal Dashboard Payload](payload-login-dashboard.md)
- Gambar sudah dikompres — lihat [Tutorial Kompres Gambar](tutorial-kompres-gambar.md)

{% hint style="warning" %}
Kompres gambar **sebelum** diunggah. Payload memang membuat versi kecil secara otomatis, tapi file asli yang berat tetap memperlambat proses unggah dan memakan penyimpanan.
{% endhint %}

---

## Langkah-Langkah

### 1. Buka Koleksi Media

Klik menu **Media** di sidebar kiri. Anda akan melihat semua gambar yang pernah diunggah dalam tampilan grid.

### 2. Unggah Gambar Baru

Klik **Create New**, lalu pilih file dari komputer Anda — atau seret file langsung ke area unggah.

Satu file per dokumen Media.

---

### 3. Isi Alt Text

Setelah gambar terunggah, isi field **Alt**.

Alt text adalah deskripsi singkat isi gambar. Fungsinya dua: dibaca oleh pembaca layar untuk pengunjung tunanetra, dan dipakai Google untuk memahami isi gambar.

| Contoh | Nilai |
|--------|-------|
| ❌ Buruk | `IMG_20260715.jpg` — tidak menjelaskan apa pun |
| ❌ Buruk | `gambar produk` — terlalu umum |
| ✅ Baik | `Pupuk organik kemasan 5 kg tampak depan` |

{% hint style="info" %}
Field **Alt** secara teknis tidak wajib diisi, tapi tetap isi selalu. Gambar tanpa alt text merugikan SEO dan aksesibilitas website Anda.
{% endhint %}

### 4. Isi Caption (Opsional)

Field **Caption** adalah keterangan yang bisa tampil di bawah gambar pada blok tertentu. Isi hanya jika memang dibutuhkan — tidak semua tempat menampilkannya.

---

### 5. Atur Focal Point

Di bawah preview gambar, ada penanda **Focal Point** yang bisa digeser.

Focal point menentukan bagian gambar mana yang **tetap terlihat** saat gambar dipotong ke ukuran lain. Website menampilkan gambar dalam berbagai bentuk — persegi, memanjang, lebar — dan pemotongan tidak selalu di tengah.

Geser penanda ke bagian terpenting gambar. Untuk foto orang, arahkan ke wajah. Untuk foto produk, arahkan ke produknya.

### 6. Simpan

Klik **Save**. Gambar siap dipakai.

---

## Ukuran Gambar Otomatis

Setiap gambar yang diunggah otomatis dibuatkan beberapa versi oleh Payload. Anda tidak perlu membuatnya manual — website memilih ukuran yang paling pas sendiri.

| Nama | Ukuran | Dipakai untuk |
|------|--------|---------------|
| `thumbnail` | lebar 300px | Preview kecil di dalam admin |
| `square` | 500 × 500px | Tampilan kotak, misalnya kartu produk |
| `small` | lebar 600px | Layar ponsel |
| `medium` | lebar 900px | Layar tablet |
| `large` | lebar 1400px | Layar desktop |
| `xlarge` | lebar 1920px | Layar besar |
| `og` | 1200 × 630px | Gambar preview saat dibagikan ke WhatsApp dan media sosial |

{% hint style="success" %}
Karena versi terbesar yang dibuat adalah **1920px**, mengunggah gambar dengan lebar lebih dari itu tidak menambah kualitas — hanya menambah beban. Lebar 1920px sudah cukup untuk gambar apa pun.
{% endhint %}

---

## Merapikan dengan Folder

Koleksi Media mendukung **folder**. Klik **New Folder** untuk membuat pengelompokan, lalu pindahkan gambar ke dalamnya.

Ini sangat membantu setelah gambar Anda mencapai puluhan. Contoh pembagian yang praktis:

- `produk` — foto-foto produk
- `artikel` — gambar utama artikel
- `tim` — foto anggota tim
- `umum` — logo, ikon, gambar halaman

---

## Mengganti dan Menghapus Gambar

Untuk **mengganti file** pada dokumen Media yang sudah ada, buka dokumennya lalu klik ikon silang pada preview dan unggah file baru.

{% hint style="danger" %}
**Menghapus** dokumen Media hanya bisa dilakukan oleh **Admin** — lihat [Login dan Mengenal Dashboard Payload](payload-login-dashboard.md).

Sebelum menghapus, pastikan gambar itu tidak sedang dipakai di halaman, artikel, atau produk mana pun. Gambar yang dihapus padahal masih terpasang akan membuat gambar hilang di website.

Kalau ragu, biarkan saja. Gambar yang tidak dipakai tidak mengganggu tampilan website.
{% endhint %}

---

## Checklist Sebelum Unggah

- [ ] Gambar sudah dikompres
- [ ] Lebar gambar tidak lebih dari 1920px
- [ ] Nama file deskriptif, bukan `IMG_1234.jpg`
- [ ] **Alt** sudah diisi dan menjelaskan isi gambar
- [ ] **Focal point** sudah diarahkan ke bagian terpenting

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: ElsCMS with Payload · Diperbarui: 15 Juli 2026*
