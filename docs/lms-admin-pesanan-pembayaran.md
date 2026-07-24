---
description: Mengelola pesanan, mengonfirmasi pembayaran, mengatur metode pembayaran (Tripay, QRIS, transfer manual), melakukan refund, dan membuat kupon diskon di LMS Indonesia.
---

# Pesanan, Pembayaran, dan Kupon

Setiap kali peserta membeli kursus, terbentuk sebuah **Order**. Grup **Transaksi** dipakai untuk memantau order, mengonfirmasi pembayaran, dan mengelola kupon diskon. Halaman ini juga membahas cara mengatur metode pembayaran lembaga Anda.

---

## Prasyarat

- Anda bisa login sebagai **Super Admin**, **Admin**, atau **Keuangan** — lihat [Ikhtisar dan Akses Panel Admin](lms-admin-pengenalan.md)
- Sudah ada kursus yang dipublikasikan — lihat [Mengelola Kursus dan Pelajaran](lms-admin-kursus.md)

---

## Alur Sebuah Order

```
Peserta beli → Order dibuat → Peserta bayar → Pembayaran dikonfirmasi → Peserta otomatis ter-enroll
```

Status yang akan Anda temui:

| Status Order | Arti |
|--------------|------|
| **Menunggu Pembayaran** | Order dibuat, peserta belum membayar |
| **Menunggu Konfirmasi** | Bukti bayar masuk, menunggu dicek admin |
| **Selesai** | Pembayaran sah, akses kursus diberikan |
| **Dibatalkan** | Order gagal / kedaluwarsa |
| **Dikembalikan** | Order sudah di-refund |

| Status Bayar | Arti |
|--------------|------|
| **Belum Bayar** · **Sudah Bayar** · **Gagal** · **Refunded** | — |

---

## Langkah-Langkah

### 1. Memantau Order

Klik **Transaksi → Order**. Tabel menampilkan nomor order, pembeli, total, status order, dan status bayar. Gunakan filter **Status Order** dan **Status Bayar** untuk menyaring — misalnya menampilkan hanya yang **Menunggu Konfirmasi**.

![Daftar order](https://GANTI-DENGAN-SCREENSHOT)

Klik sebuah order untuk melihat detail: rincian harga, item kursus, dan data transaksi pembayaran (termasuk **bukti transfer** bila ada).

### 2. Mengonfirmasi Pembayaran Transfer Manual

Untuk pembayaran lewat **transfer bank manual**, peserta mengunggah bukti transfer, lalu Anda memverifikasinya:

1. Buka order dengan status **Menunggu Konfirmasi**.
2. Periksa **Bukti Transfer** — cocokkan nominal dan tujuan dengan mutasi rekening Anda.
3. Klik tombol aksi **Konfirmasi Bayar**.

Setelah dikonfirmasi, order menjadi **Selesai**, status bayar **Sudah Bayar**, dan peserta otomatis mendapat akses kursus.

{% hint style="warning" %}
Pastikan dana **benar-benar sudah masuk** ke rekening sebelum menekan **Konfirmasi Bayar**. Konfirmasi memberi akses kursus secara permanen.
{% endhint %}

### 3. Menyinkronkan Pembayaran Tripay

Untuk order lewat gateway **Tripay** yang belum tercatat lunas, gunakan aksi **Sync Tripay**. Sistem akan mengecek status langsung ke Tripay dan memperbarui order (menjadi lunas, gagal, atau kedaluwarsa) sesuai hasilnya. Umumnya pembayaran Tripay terkonfirmasi otomatis; aksi ini hanya cadangan bila status belum ter-update.

### 4. Melakukan Refund

Aksi **Refund** mengubah order menjadi **Dikembalikan** dan otomatis **membatalkan komisi afiliasi** yang terkait order tersebut.

{% hint style="danger" %}
**Refund hanya bisa dilakukan Super Admin (dan Admin).** Peran **Keuangan tidak dapat** me-refund. Refund tidak otomatis mengirim uang kembali ke peserta — proses pengembalian dana dilakukan terpisah oleh Anda. Tindakan ini menandai order sebagai dikembalikan di sistem.
{% endhint %}

---

## Mengatur Metode Pembayaran

Buka **Pengaturan → Pengaturan Pembayaran**.

{% hint style="warning" %}
Kustomisasi metode pembayaran (Tripay, rekening transfer manual, dan QRIS statis milik sendiri) **hanya untuk paket Pro**. Tenant paket **Free** otomatis memakai **QRIS platform (Xendit)** — pembayaran diproses otomatis tanpa perlu setup. Untuk mengaktifkan metode sendiri, upgrade ke Pro; lihat [Pengaturan & Fitur Lanjutan](lms-admin-pengaturan.md).
{% endhint %}

Untuk tenant **Pro**, tersedia pengaturan:

| Bagian | Isi |
|--------|-----|
| **Payment Gateway (Tripay)** | Pilih metode aktif: QRIS, VA Maybank/BRI/BNI/BSI/Mandiri/BCA |
| **Rekening Bank Transfer Manual** | Daftar rekening (kode bank, nama bank, nomor rekening, atas nama) yang tampil saat peserta memilih transfer manual |
| **QRIS Manual** | QRIS statis merchant Anda; admin mengonfirmasi manual setelah peserta unggah bukti |
| **Penarikan Komisi Afiliasi** | Biaya transfer & minimum penarikan komisi (berlaku untuk semua paket) |

Klik **Simpan Pengaturan** setelah mengubah.

---

## Kupon Diskon

Menu **Transaksi → Kupon** dipakai membuat kode diskon.

### Membuat Kupon

Klik **Create**, lalu isi:

| Field | Keterangan |
|-------|-----------|
| **Kode Kupon** | Kode yang dimasukkan peserta saat checkout (mis. `RAMADHAN25`) |
| **Tipe** | Persentase atau nominal tetap |
| **Nilai Diskon** | Besar potongan sesuai tipe |
| **Minimum Order** | Batas belanja minimal agar kupon berlaku |
| **Batas Penggunaan** | Jumlah maksimal pemakaian kupon |
| **Berlaku Mulai / Sampai** | Rentang tanggal aktif |
| **Aktif** | Nyalakan/matikan kupon |

![Membuat kupon](https://GANTI-DENGAN-SCREENSHOT)

{% hint style="info" %}
Gunakan **Batas Penggunaan** dan **Berlaku Sampai** untuk kampanye terbatas agar diskon tidak dipakai melebihi rencana Anda.
{% endhint %}

---

## Checklist Transaksi

- [ ] Mengecek order **Menunggu Konfirmasi** secara rutin
- [ ] Selalu mencocokkan bukti transfer dengan mutasi bank sebelum konfirmasi
- [ ] Metode pembayaran sudah diatur (atau memakai QRIS platform untuk paket Free)
- [ ] Memahami bahwa refund hanya untuk Super Admin/Admin dan tidak mengirim dana otomatis
- [ ] Kupon dibuat dengan batas penggunaan dan masa berlaku yang jelas

---

## Butuh Bantuan?

📱 **WhatsApp:** [+62-812-1765-4564](https://wa.me/6281217654564)\
🌐 **Website:** [elshobah.com](https://elshobah.com)

---

*Kategori: LMS Indonesia — Admin Tenant · Diperbarui: 24 Juli 2026*
