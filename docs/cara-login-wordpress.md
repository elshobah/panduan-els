---
description: Panduan lengkap untuk masuk ke area administrasi WordPress, termasuk cara mengatasi masalah umum saat login.
---

# Cara Login Admin di WordPress

Setiap website yang dibangun Elshobah menggunakan URL login khusus. Panduan ini menjelaskan cara masuk ke dashboard WordPress dan mengatasi masalah login yang umum terjadi.

---

## Langkah Login

### 1. Buka Halaman Login

Akses halaman login WordPress melalui URL berikut di browser Anda:

```
https://domainanda.com/els
```

{% hint style="info" %}
Elshobah menggunakan path `/els` (bukan `/wp-admin`) sebagai langkah keamanan tambahan.
{% endhint %}

### 2. Masukkan Kredensial

Isi form login dengan:

| Field | Keterangan |
|-------|-----------|
| **Username** | Username yang dibuat saat instalasi WordPress |
| **Password** | Password yang dibuat saat instalasi WordPress |

### 3. Masuk ke Dashboard

Setelah login berhasil, Anda akan diarahkan ke **WordPress Dashboard** — pusat kendali website Anda.

---

## Mengatasi Masalah Login

### Lupa Password

1. Klik link **"Lost your password?"** di bawah form login
2. Masukkan username atau alamat email terdaftar
3. Cek inbox email — klik link reset password yang dikirim
4. Buat password baru

{% hint style="warning" %}
Jika email reset tidak masuk, cek folder **Spam/Junk** terlebih dahulu.
{% endhint %}

**Alternatif via phpMyAdmin:**

Jika reset via email tidak berhasil, password dapat diubah secara manual:

1. Buka **phpMyAdmin** melalui cPanel
2. Pilih database WordPress Anda
3. Buka tabel `wp_users`
4. Edit field `user_pass` pada baris user Anda
5. Simpan perubahan

### Lupa Username

Username dapat dilihat atau diubah melalui cara yang sama — edit field `user_login` di tabel `wp_users` via phpMyAdmin.

---

## Catatan Penting

{% hint style="danger" %}
Pastikan alamat email yang terdaftar di WordPress valid dan dapat diakses. Email ini digunakan untuk proses reset password.
{% endhint %}

- Jangan bagikan kredensial login kepada pihak yang tidak berwenang
- Gunakan password yang kuat (kombinasi huruf, angka, dan simbol)
- Logout setelah selesai, terutama jika menggunakan perangkat publik

---

*Kategori: Pengetahuan Dasar · Diperbarui: 1 Agustus 2022*
