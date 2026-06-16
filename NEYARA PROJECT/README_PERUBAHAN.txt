PERUBAHAN PROYEK SPA KAMPOENG SUKOHARJO

1. Panel admin sudah disatukan ke halaman utama melalui index.html.
   Akses melalui tombol "☰ Admin" pada navbar atau melalui index.html#admin.

2. admin.html tidak lagi menjadi dashboard terpisah.
   File tersebut hanya mengarahkan kembali ke index.html#admin agar alur admin menyatu dengan halaman user.

3. Login admin:
   Username: admin
   Password: admin123

4. Fitur admin yang ditambahkan:
   - Dashboard ringkas: total booking, pendapatan lunas, pending payment, layanan aktif.
   - CRUD Booking: tambah, edit, hapus, ubah status, pencarian, filter status, dan tombol WhatsApp.
   - CRUD Layanan: tambah, edit, hapus, aktif/nonaktif layanan.
   - Perubahan layanan otomatis masuk ke halaman user: kartu layanan, tabel harga, dan pilihan booking.
   - Export data booking ke CSV.
   - Backup semua data ke JSON.
   - Hapus semua data booking.

5. Catatan teknis:
   - Proyek ini masih berbasis HTML, CSS, JavaScript statis.
   - Data disimpan di localStorage browser, bukan database server.
   - Untuk produksi nyata, autentikasi admin dan penyimpanan data sebaiknya dipindahkan ke backend/database.


PEMBENAHAN LANJUTAN:
1. Tipografi website diperbarui menggunakan kombinasi Playfair Display dan Poppins agar tampilan lebih menarik, modern, dan mudah dibaca oleh admin maupun user.
2. Halaman sukses booking diperbarui menjadi halaman konfirmasi khusus dengan animasi kembang api estetis tanpa library eksternal.
3. Setelah pembayaran selesai, user diarahkan ke success.html dan booking tetap masuk ke panel admin melalui localStorage.
4. Riwayat pemesanan user ditambahkan pada halaman utama setelah form booking, lengkap dengan detail jadwal, layanan, status, tombol WhatsApp, tombol notifikasi H-1, dan tombol tambah ke kalender.
5. Nomor WhatsApp Q&A setelah booking disesuaikan menjadi +62 812-5697-6887.
6. Reminder WhatsApp otomatis belum dapat berjalan pada website statis tanpa backend/WhatsApp Business API. Solusi yang diterapkan adalah tombol WhatsApp dengan pesan otomatis, notifikasi browser H-1, dan file kalender (.ics) dengan alarm H-1.


PATCH ADMIN FULLSCREEN:
- Panel admin diperbaiki menjadi full viewport, bukan drawer setengah halaman.
- Admin overlay memakai 100vw dan 100dvh agar tidak terpotong di desktop maupun mobile.
- Konten admin memakai flex:1 dan overflow-y:auto agar tabel/form panjang dapat discroll tanpa memotong layout.

Update katalog layanan spa realistis:
- Daftar layanan pada bagian Service diganti menjadi katalog spa yang lebih realistis untuk UMKM jasa spa.
- Katalog mencakup Body & Massage, Hair & Head Spa, Facial & Skin Care, Foot & Nail Care, Family & Special Care, Bride Package, dan Signature Package.
- Harga, durasi, kategori, label, dan deskripsi layanan sudah disesuaikan agar lebih natural untuk katalog spa nyata.
- Bagian katalog kategori di halaman utama sekarang mengikuti data layanan aktif.
- Admin dapat menentukan layanan mana yang tampil sebagai rekomendasi melalui kolom "Tampil di Rekomendasi".
- Versi katalog diperbarui agar browser yang masih menyimpan data lama di localStorage memuat katalog baru secara otomatis.


=== UPDATE TIPOGRAFI FINAL ===
- Font heading diperbarui ke Cormorant Garamond agar karakter spa tetap elegan.
- Font teks utama diperbarui ke Nunito Sans agar lebih bersih, modern, dan mudah dibaca.
- Ukuran font body, navigasi, tombol, form, tabel admin, kartu layanan, riwayat booking, halaman pembayaran, dan halaman sukses booking diperbesar secara proporsional.
- Sistem ukuran memakai clamp() agar tetap responsif di desktop, tablet, dan mobile.
- Ukuran teks kecil seperti label, badge, status, dan menu admin dinaikkan agar tidak terlihat terlalu kecil.


UPDATE FONT V2 - 30 Mei 2026
- Seluruh skala tipografi website dinaikkan secara global, bukan hanya pada satu halaman.
- Ukuran teks body, paragraf, katalog, form booking, tombol, label, tabel admin, riwayat pemesanan, pembayaran, dan halaman sukses diperbesar agar lebih mudah dibaca.
- Heading tetap memakai gaya elegan, tetapi ukuran dan hierarki visual diperjelas.
- Ukuran font dibuat responsif agar tetap aman di desktop, tablet, dan ponsel.
