# AFPI-TEST

Project ini merupakan bagian dari proses pengolahan dan validasi data transaksi serta NPP (Nasabah Penerima Pinjaman) yang berasal dari sistem internal untuk keperluan analisis dan pelaporan.


## 🔄 Proses ETL

Project ini melakukan beberapa tahapan:

1. **Ekstraksi**: Mengambil data dari tabel `trx` dan `npp`.
2. **Transformasi & Validasi**:
   - TRX bulan H harus lebih besar dari bulan H-1.
   - NPP bulan H harus lebih besar atau sama dengan bulan H-1.
3. **Load**:
   - Data yang telah divalidasi disimpan ke tabel `trx_val` dan `npp_val`.
   - Kemudian data tersebut dimasukkan ke tabel `trx_done` dan `npp_done` dengan status `valid` atau `invalid`.

## 🛠 Tools yang Digunakan

- **SQL Server Management Studio (SSMS)**
- **SQL Server Integration Services (SSIS)**
- **Git & GitHub** untuk version control



