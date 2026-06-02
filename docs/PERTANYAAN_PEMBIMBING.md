# Pertanyaan untuk Pembimbing

## A. Tujuan dan Pengguna

1. Aplikasi ini akan dipakai oleh siapa saja? Petugas BPS saja, mitra statistik, admin, atau pihak lain?
2. Tujuan utama aplikasinya apa: pencarian data, validasi data, cross-check, pelaporan, atau semuanya?
3. Apakah aplikasi ini hanya untuk internal kantor atau nantinya bisa diakses dari luar jaringan kantor?
4. Apakah targetnya web app, aplikasi mobile, atau cukup dashboard web yang bisa dibuka dari HP?

## B. Kondisi Data Saat Ini

5. Data kependudukan saat ini bentuknya apa: Excel, CSV, spreadsheet, database, atau file lain?
6. Kalau belum ada database, apakah saya diminta membantu membuat struktur database dari raw data tersebut?
7. Data mentahnya berasal dari mana saja?
8. Apakah sudah ada template kolom baku yang harus diikuti?
9. Kolom apa saja yang wajib ada?
10. Apakah data menggunakan NIK, nomor KK, nama, alamat, kode wilayah, atau field lain?
11. Apakah boleh menggunakan data asli untuk testing, atau harus menggunakan data dummy/sintetis?

## C. Database dan Integrasi

12. Apakah kantor sudah punya database/server yang harus dipakai?
13. Kalau sudah ada, database-nya pakai apa: MySQL, PostgreSQL, SQL Server, SQLite, atau lainnya?
14. Apakah saya diberi akses langsung ke database, atau hanya boleh lewat file/API?
15. Apakah ada sistem kantor lain yang harus diintegrasikan?
16. Apakah data perlu di-update berkala? Harian, mingguan, bulanan, atau manual?

## D. Pencarian Data

17. Petugas perlu bisa mencari data berdasarkan apa saja: NIK, nama, alamat, kecamatan, desa, nomor KK, atau kombinasi?
18. Apakah hasil pencarian boleh menampilkan data lengkap atau hanya ringkasan?
19. Apakah perlu fitur filter, sorting, dan export Excel/PDF?
20. Apakah perlu fitur riwayat pencarian?

## E. Cross-check Data

21. Data penduduk akan di-cross-check dengan data apa?
22. Field apa yang harus dibandingkan?
23. Output cross-check yang diinginkan seperti apa: cocok/tidak cocok, skor kemiripan, daftar perbedaan, atau status verifikasi?
24. Kalau data tidak cocok, siapa yang boleh memperbaiki atau menandai hasil verifikasi?
25. Apakah perlu laporan hasil cross-check?

## F. WhatsApp Chatbot

26. WhatsApp chatbot untuk siapa? Semua petugas atau hanya admin tertentu?
27. Nomor WhatsApp petugas apakah akan didaftarkan/whitelist?
28. Bot boleh menjawab data apa saja?
29. Apakah bot cukup menjawab hasil ringkas atau harus bisa mengirim laporan?
30. Format perintah bot yang diinginkan seperti apa?
31. Apakah kantor sudah punya nomor WhatsApp Business/API, atau perlu pakai solusi alternatif untuk prototype?

## G. Keamanan dan Privasi

32. Karena data penduduk sensitif, aturan akses datanya seperti apa?
33. Apakah perlu role akses: admin, petugas, viewer?
34. Apakah semua aktivitas pencarian harus dicatat dalam audit log?
35. Apakah ada aturan khusus dari kantor/BPS tentang penyimpanan dan penggunaan data?
36. Apakah repository GitHub boleh berisi kode saja tanpa data asli?
37. Apakah data asli tidak boleh keluar dari komputer/server kantor?

## H. Output Magang

38. Output yang diharapkan dari saya sampai akhir magang apa?
39. Apakah cukup prototype, flowchart, database design, dokumentasi, atau aplikasi jadi?
40. Apakah ada deadline per tahap?
41. Apakah saya perlu membuat laporan teknis/presentasi/demo?
42. Apakah pembimbing ingin saya mulai dari flowchart dan ERD dulu sebelum coding?
