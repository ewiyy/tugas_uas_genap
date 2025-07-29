# Aplikasi Inventori Toko Apotek

Aplikasi sederhana berbasis Python CLI untuk mengelola stok obat di toko apotek. Cocok untuk usaha kecil atau inventaris manual tanpa sistem database.

---

## Fitur

- Tambah data obat baru
- Tampilkan semua data obat
- Edit jumlah stok
- Hapus obat
- Laporan stok (diurutkan dari yang terbanyak)
- Simpan data ke file JSON

---

## Cara Menjalankan

1. **Install Python 3** jika belum tersedia.
2. Simpan file Python dengan nama `inventori_apotek.py`.
3. Jalankan aplikasi melalui terminal:
   ```bash
   python inventori_apotek.py
| File                    | Deskripsi                        |
| ----------------------- | -------------------------------- |
| `inventori_apotek.py`   | Kode utama aplikasi              |
| `inventori_apotek.json` | File data obat dalam format JSON |
| `README.md`             | Dokumentasi penggunaan aplikasi  |

## Panduan Penggunaan 
Saat dijalankan, aplikasi menampilkan menu berikut
1. Tambah Obat
2. Lihat Semua Obat
3. Edit Stok Obat
4. Hapus Obat
5. Laporan Stok
6. Simpan & Keluar

## Penjelasan vitur 
1. Tambah Obat
   Untuk menambahkan obat baru ke dalam sistem.
   Input yang diminta:
   Kode obat (unik)
   Nama obat
   Jumlah stok awal
   Jika kode sudah ada, akan muncul peringatan.
Contoh :
Kode obat: OBT001
Nama obat: Paracetamol
Jumlah stok: 100

2. Lihat Semua Obat
   Menampilkan seluruh data obat yang tersimpan dalam sistem.
   Format tampilan:
OBT001 - Paracetamol (Stok: 100)

3. Edit Stok Obat
   Untuk mengubah jumlah stok dari obat yang sudah ada.
   Masukkan kode obat, lalu stok baru.

Contoh:
  Masukkan kode obat yang ingin diedit: OBT001
  Stok baru: 50

4. Hapus Obat
Untuk menghapus data obat dari sistem.
Hanya memerlukan kode obat.

Contoh:
Masukkan kode obat yang ingin dihapus: OBT004
Obat berhasil dihapus.

5. Laporan Stok
   Menampilkan daftar semua obat yang diurutkan berdasarkan jumlah stok dari terbanyak ke tersedikit.
   Berguna untuk pemantauan stok secara cepat.

Contoh Output:
Laporan stok (diurutkan dari jumlah terbanyak):
Ponstan - Stok: 200
Bodrex Extra - Stok: 150
Paracetamol - Stok: 50

6. Simpan & Keluar
   Menyimpan semua perubahan ke file inventori_apotek.json.
   Program akan keluar setelah penyimpanan berhasil.
