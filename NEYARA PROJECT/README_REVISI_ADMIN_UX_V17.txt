README REVISI ADMIN UX V17

Perubahan utama:
1. Tampilan login admin tidak lagi menampilkan password default di kolom password dan tidak lagi menampilkan teks kredensial default di bawah tombol login.
2. File User Manual pada menu admin sudah diganti dengan file PDF terbaru yang dikirim pengguna.
3. Sortir Booking dengan pilihan "Terbaru dibuat" diperbaiki agar data booking baru dari admin atau pelanggan tampil di posisi paling atas, meskipun database demo memiliki data jadwal Juli 2026.
4. Data booking baru kini menyimpan metadata createdAtMs dan source untuk pemeringkatan data masuk yang lebih stabil.
5. Ringkasan transaksi dashboard dan kartu Booking Terbaru juga memakai logika urutan data terbaru yang sama.

Catatan:
- Password login sistem tetap berlaku di logika autentikasi. Perubahan hanya menghapus tampilan password/default credential dari UI login.
- Data demo Mei, Juni, dan Juli tetap dipertahankan untuk kebutuhan pengujian filter tanggal, status, pencarian, grafik, dan ekspor CSV.
