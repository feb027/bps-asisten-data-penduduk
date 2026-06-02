# Rancangan Awal Sistem

## Tujuan

Membuat aplikasi internal yang memudahkan petugas BPS Kabupaten Tasikmalaya mencari, merapikan, dan mencocokkan data kependudukan dari sumber data kantor.

## Masalah yang Ingin Diselesaikan

Saat ini data kemungkinan masih tersebar dalam file mentah seperti Excel/CSV/spreadsheet. Petugas perlu cara yang lebih cepat untuk mencari data, memverifikasi data, dan mencocokkan data dengan sumber pembanding tanpa membuka banyak file manual.

## Asumsi Awal

- Data awal belum tentu sudah ada di database.
- Data bisa berasal dari Excel, CSV, atau file kegiatan kantor.
- Sistem perlu tahap import dan cleaning sebelum data dapat dicari oleh aplikasi.
- Akses data harus dibatasi karena data kependudukan bersifat sensitif.
- WhatsApp chatbot sebaiknya menjadi fitur tambahan setelah database dan API siap.

## Alur Sistem

1. Admin/petugas mengunggah data mentah.
2. Sistem melakukan validasi struktur data.
3. Sistem melakukan normalisasi dan cleaning.
4. Data yang lolos validasi dimasukkan ke database.
5. Petugas login ke dashboard.
6. Petugas mencari data penduduk.
7. Sistem menampilkan hasil sesuai kewenangan akses.
8. Petugas dapat melakukan cross-check dengan data pembanding.
9. Sistem menyimpan log aktivitas.
10. WhatsApp chatbot dapat digunakan untuk query ringkas oleh petugas yang nomornya terdaftar.

## Modul Sistem

### A. Modul Import Data

Input:
- File Excel/CSV.
- Template kolom dari pembimbing/kantor.

Proses:
- Validasi kolom wajib.
- Cek format data.
- Cek duplikat.
- Cek data kosong.
- Normalisasi teks dan kode wilayah.

Output:
- Data valid masuk database.
- Data bermasalah masuk daftar perlu koreksi.

### B. Modul Database

Fungsi:
- Menyimpan data penduduk yang sudah rapi.
- Menyimpan data pembanding.
- Menyimpan data petugas dan role akses.
- Menyimpan audit log.

### C. Modul Dashboard

Fungsi:
- Login petugas.
- Pencarian data.
- Filter data.
- Detail data sesuai role.
- Cross-check data.
- Export laporan jika diizinkan.

### D. Modul Cross-check

Contoh hasil:
- `Cocok`: data utama dan data pembanding sama.
- `Tidak cocok`: ada perbedaan field.
- `Data kurang`: data pembanding tidak lengkap.
- `Perlu verifikasi`: sistem tidak bisa menyimpulkan otomatis.

### E. Modul WhatsApp Chatbot

Contoh format awal:

```text
CEK NIK 3206xxxxxxxxxxxx
CARI NAMA ASEP KEC SINGAPARNA
CEK WILAYAH DESA X
```

Prinsip keamanan:
- Nomor petugas harus whitelist.
- Bot tidak membalas data sensitif lengkap.
- Semua query dicatat.
- Bot hanya mengakses API, bukan langsung database.

## Prioritas Pengerjaan

1. Konfirmasi kebutuhan ke pembimbing.
2. Tentukan struktur data dan sumber data.
3. Buat flowchart final.
4. Buat desain database awal.
5. Buat prototype import Excel/CSV.
6. Buat dashboard pencarian sederhana.
7. Tambahkan cross-check.
8. Tambahkan WhatsApp chatbot.
