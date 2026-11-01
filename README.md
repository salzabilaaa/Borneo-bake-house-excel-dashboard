# Borneo Bake House: Sistem Pencatatan Operasional & Dashboard (Excel)

Mini project Excel untuk mencatat dan merangkum operasional **cabang Sangatta** Borneo Bake House, unit usaha roti dan kue di bawah PT Borneo Mart. 
Hasil akhirnya berupa satu workbook berisi data master, pencatatan harian, laporan ringkas arus kas, dan **dashboard** yang menjawab enam pertanyaan bisnis.

Seluruh data dalam project ini dibuat untuk keperluan latihan dan portofolio. Periode data: **Juli 2026**.

---

## Latar belakang

Borneo Bake House dibentuk untuk memenuhi kebutuhan roti segar di jaringan swalayan Borneo Mart di Kalimantan Timur. 
Dapur produksi utama ada di Samarinda. Roti dikirim ke cabang Sangatta setiap **Senin dan Kamis**, 
lalu disalurkan ke lima outlet di sekitar Kutai Timur dengan jadwalnya masing-masing:

Outlet                                Hari kirim 
Sangatta Utara dan Sangatta Selatan   Senin, Kamis 
Bengalo                               Selasa, Jumat 
Muara Wahau                           Rabu 
Kaliorang                             Jumat 

Cake dan snack box diproduksi di dapur kecil cabang Sangatta, sedangkan wedding cake dibuat sesuai pesanan.
Cabang dijalankan 13 karyawan.

Dalam sehari ada banyak hal yang dicatat: kas kecil, stok, pengiriman, penjualan, dan absensi. 
Kalau catatannya terpisah dan tidak saling terhubung, stok yang menipis tidak terdeteksi, pengiriman tertunda tidak ditindaklanjuti, 
dan laporan ke pusat tidak cocok dengan catatan harian. Project ini dibuat dari sudut pandang **Admin General** untuk menyatukan semua catatan itu.

## Pertanyaan bisnis yang dijawab dashboard
1 Berapa penjualan bulan ini?
2 Uang keluar paling banyak untuk apa? 
3 Bagaiamana pengiriman ke outlet lancar atau ada yang tertunda?
4 Produk apa yang paling laku?
5 Apakah karyawan hadir dengan baik? 
6 Hari mana yang palaing ramai? 

## Ringkasan temuan Juli 2026

- **Penjualan** Rp15.745.000 dari 25 transaksi, dengan hari tertinggi 18 Juli (Rp1.650.000) dan terendah 10 Juli (Rp55.000).
- **Produk terlaris** berdasarkan nilai: Snack Box Reguler (Rp4.340.000), disusul Snack Box Premium dan Wedding Cake.
- **Pengeluaran kas** Rp4.765.000, dengan Transportasi sebagai porsi terbesar (Rp3.380.000, sekitar 71%).
- **Stok:** Roti Sobek Original berstatus Menipis (95 unit).
- **Pengiriman:** 22 dari 25 pengiriman (88%) berstatus Terkirim, sedangkan 2 Pending dan 1 Ditunda. Penundaan disebabkan jalan longsor, mobil box yang sedang servis, dan menunggu konfirmasi outlet.
- **Kehadiran** rata-rata 94,6%, dengan satu karyawan berstatus Perlu Perhatian.

## Asumsi dan keterbatasan

- Data penjualan tercatat sampai 24 Juli, sedangkan sheet lain mencakup sampai akhir bulan.
- Saldo Akhir Kas bukan laba, angkanya dari saldo awal ditambah penjualan dikurangi petty cash, dan biaya bahan baku serta gaji belum tercatat.
- Stok hanya mencakup 4 jenis roti,  Stok keluar dicatat saat barang dimuat (termasuk yang masih Pending/Ditunda), dan 10 unit rusak pada RT-003 masih ikut terhitung sebagai stok masuk.
- Penjualan belum punya status pembayaran dan nomor transaksi, dan dropdown validasi baru ada di status pengiriman.

## Rencana pengembangan
- Menambah kolom kategori penyebab keterlambatan pengiriman, lalu menampilkannya sebagai chart.
- Menambah metrik "stok cukup untuk berapa hari" berdasarkan rata-rata distribusi harian.
- Menambah data biaya bahan baku dan gaji agar laba bisa dihitung.
- Menambah nomor surat jalan di sheet pengiriman supaya dokumen fisik dan catatan di Excel bisa saling ditelusuri.
- Menambah validasi data (kode produk, jenis pelanggan, kategori kas) dan memakai rujukan Excel Table agar rumus otomatis mengikuti penambahan data.
- Memperluas dashboard ke beberapa bulan.

## Dokumen pendukung
- docs/SEJARAH_PERUSAHAAN_BORNEO_BAKE_HOUSE.docx: latar belakang dan alur operasional perusahaan.
- docs/SURAT_JALAN_BORNEO_BAKE_HOUSE.docx: contoh surat jalan pengiriman (17 Juli 2026, tujuan Bengalon).


