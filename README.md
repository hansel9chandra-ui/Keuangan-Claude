# Keuanganku

Aplikasi pencatat keuangan untuk mahasiswa. Berjalan sepenuhnya di browser (HTML + CSS + JavaScript murni), tanpa server, tanpa instalasi, dan tanpa dependensi. Data disimpan di `localStorage` perangkat Anda.

## Fitur

- 3 kategori bawaan: **Uang Makan**, **Uang Jajan**, **Uang Kuliah**
- Tambah, edit, dan hapus **kategori** (nama, warna, anggaran bulanan opsional)
- Tambah, edit, dan hapus **transaksi** (pemasukan atau pengeluaran, jumlah, tanggal, catatan)
- Ringkasan: saldo total, pemasukan dan pengeluaran per bulan
- Saldo per kategori dan bar progres anggaran (peringatan jika melebihi anggaran)
- Grafik pengeluaran per kategori
- Riwayat transaksi dengan pencarian, filter kategori, dan filter jenis
- Pilih bulan untuk melihat riwayat bulan lain
- Ekspor/impor cadangan JSON, ekspor CSV (bisa dibuka di Excel)
- Tampilan responsif (HP dan desktop) dan mode gelap otomatis

## Menjalankan

Buka `index.html` di browser. Selesai.

## Upload ke GitHub dan hosting gratis (GitHub Pages)

1. Buat repository baru di GitHub, misalnya `keuanganku`.
2. Upload semua file dari folder ini (atau lewat terminal):
   ```bash
   git init
   git add .
   git commit -m "Versi pertama Keuanganku"
   git branch -M main
   git remote add origin https://github.com/USERNAME/keuanganku.git
   git push -u origin main
   ```
3. Di GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
4. Setelah beberapa menit, aplikasi bisa diakses di `https://USERNAME.github.io/keuanganku/`.

## Catatan

- Data tersimpan per browser dan per perangkat. Gunakan **Data → Ekspor cadangan** secara berkala, dan **Impor cadangan** untuk memindahkan data ke perangkat lain.
- Menghapus kategori juga menghapus semua transaksi di dalamnya.

## Struktur

```
index.html   Kerangka halaman
style.css    Tampilan
app.js       Logika aplikasi
```
