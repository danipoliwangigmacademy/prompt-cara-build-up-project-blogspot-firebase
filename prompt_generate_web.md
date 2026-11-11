Bertindaklah sebagai Expert Blogger Template Developer & Frontend Engineer. Berdasarkan dokumen PRD dan struktur template Blogspot V4.9 yang saya gunakan, buatkan potongan kode terpisah (HTML + CSS inline/scoped + JavaScript Firebase) yang dipecah khusus untuk di-paste ke dalam gadget/widget Blogger berikut ini:

1. KODE UNTUK WIDGET "Menu Melayang" (Header Menu Section):
   - Buat kode HTML/JS untuk Navbar melayang (Fixed Top) dengan efek backdrop-blur.
   - Menu anchor link: #home, #about, #layanan, #galeri, #booking, #lokasi.
   - Logo menggunakan URL: https://1.bp.blogspot.com/--KdXEY6UfLw/XBsauiP1LaI/AAAAAAAAB4w/_D-q8kBZwpQ3VKrQtk-Alj4V8UqUlTxzwCLcBGAs/s480/logo.png (atau sesuaikan dari folder assets).

2. KODE UTAMA UNTUK WIDGET "Landing Page Di Sini" (Landing Page Home Section):
   - Buat kode One-Page lengkap menggunakan HTML5 murni & Bootstrap 5 CDN.
   - Sediakan seksi: Hero, Tentang Kami & Keunggulan, Katalog Layanan & Harga, Tim Master Barber, Lookbook Galeri, serta Sektor Form Booking & Live Queue (Database Firebase Firestore).
   - Pastikan menggunakan palet warna Dark Luxury (Charcoal #121212 & Gold #C59D5F).

3. KODE UNTUK WIDGET "Footer" (Footer Section):
   - Buat kode HTML untuk bagian footer bawah (informasi kontak, jam operasional, dan hak cipta).

4. SKRIP FIREBASE FIRESTORE (Disisipkan di bagian bawah Landing Page):
   - Berikan kode <script type="module"> lengkap untuk inisialisasi Firebase v10 dan fungsi addDoc (untuk form booking) serta onSnapshot (untuk menampilkan data antrean real-time).

Berikan kodenya secara terstruktur per bagian widget agar saya bisa langsung menyalinnya ke halaman Tata Letak Blogger.


Bertindaklah sebagai Senior Full-Stack Web Developer. Berdasarkan firebaseConfig yang sudah saya miliki (Project ID: barberr-5bca8), buatkan script JavaScript modular lengkap (menggunakan Firebase SDK v10 via CDN) untuk disisipkan ke dalam widget Landing Page Blogger.


//////////////////////
Script ini harus mencakup 2 fitur utama:
1. FORM BOOKING (Create to Firestore):
   - Menangkap event submit dari form ber-id "formBooking".
   - Mengambil data input: nama pelanggan (id="namaPelanggan"), nomor WhatsApp (id="noWa"), pilihan layanan (id="paketLayanan"), dan jam/tanggal booking (id="jamBooking").
   - Menyimpan data tersebut ke koleksi Firestore bernama "bookings" beserta timestamp server.
   - Menampilkan alert sukses dan mereset form setelah data berhasil dikirim.

2. LIVE ANTREAN REAL-TIME (Read from Firestore):
   - Mengambil data secara real-time menggunakan fungsi onSnapshot dari koleksi "bookings", diurutkan berdasarkan waktu terbaru (orderBy createdAt desc), dibatasi maksimal 5 data teratas.
   - Menampilkan hasilnya secara dinamis ke dalam elemen kontainer ber-id "daftarAntrean" di halaman web.

Berikan kodenya dalam bentuk tag <script type="module"> yang bersih, aman dari konflik parser XML Blogger, dan siap pakai.
/////////////////////