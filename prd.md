Product Requirements Document (PRD) & AI Master Prompt

Proyek: One-Page Website Barbershop & Grooming Studio (Integrasi Firebase Firestore)

Platform: Blogger (Blogspot) dengan Base Template Blogspot_V4.9.xml

Tech Stack: HTML5 Murni, CSS3/Bootstrap 5.3 CDN, AOS Animation, JavaScript ES6, dan Firebase Cloud Firestore (Modular v10+).

Bagian 1: Ringkasan Produk & Latar Belakang

Dokumen ini mendefinisikan perencanaan lengkap untuk pembuatan website One-Page Landing Page usaha tukang cukur modern bernama "Gentleman's Forge Barbershop" (berlokasi di Kota Batu). Website ini dirancang menggunakan arsitektur Blogger (Blogspot_V4.9.xml) agar memiliki performa SEO, AEO, dan GEO yang optimal, namun dengan tampilan dinamis layaknya aplikasi web modern berstandar BootstrapMade.

Target Pengguna (User Persona)

Pelanggan Lokal & Wisatawan (Pria / Anak-anak): Ingin melihat katalog gaya rambut, memeriksa daftar harga transparan, dan memesan jadwal cukur tanpa harus mengantre lama.

Pemilik Barbershop: Membutuhkan sistem pencatatan reservasi otomatis (Booking Management) yang masuk secara real-time ke database cloud tanpa perlu menyewa server VPS berbayar.

Bagian 2: Spesifikasi Fitur Utama (One-Page Layout)

Sticky Glassmorphism Navbar (HTML9):

Navigasi tetap di atas layar dengan efek transparan buram saat di-scroll (backdrop-blur-md).

Tombol menu responsif untuk perangkat mobile dan tautan lompat (anchor links) ke tiap seksi halaman.

Hero Section (HTML3):

Visual latar belakang maskulin beresolusi tinggi dengan tipografi elegan (Playfair Display & Poppins).

Menampilkan badge informasi jam operasional otomatis dan tombol CTA ganda ("Booking Kursi" & "Lihat Lookbook").

About & Perks Section (HTML3):

Layout modern yang memadukan cerita studio dengan 6 keunggulan utama (Ruang AC, Sterilisasi Alat UV, Wi-Fi Cepat, Handuk Hangat, Minuman Gratis, dan Parkir Luas).

Pricing & Services Menu (HTML3):

Daftar layanan 2 kolom bergaya menu restoran mewah (misalnya Gentleman Cut, Hot Towel Shave, Hair Coloring) lengkap dengan durasi estimasi dan harga.

Master Barbers Section (HTML3):

Kartu profil tim kapster profesional dengan badge spesialisasi (seperti Fade Specialist atau Scissor Master).

Lookbook & Grooming Tips (HTML3):

Galeri portofolio 8 gaya rambut populer (Curly, High Fade, Mullet, Undercut, dll.) dengan penjelasan kecocokan bentuk wajah.

Online Reservation & Live Queue (HTML3 - Integrasi Firebase):

Formulir Booking: Mengumpulkan Nama, No. WhatsApp, Pilihan Layanan, Barber, dan Jam, lalu menyimpannya langsung ke koleksi Firestore bookings.

Live Antrean Real-time: Menampilkan daftar pesanan yang masuk secara langsung (onSnapshot) dari database cloud.

Footer & Location (HTML1 & HTML8):

Informasi alamat di Temas, Kota Batu, peta interaktif Google Maps, serta tombol melayang WhatsApp (HTML8).

Bagian 3: Skema Database Firebase Firestore

Proyek ini menggunakan Cloud Firestore dengan dua koleksi utama:

Collection bookings:

nama (String)

wa (String)

paket (String)

jadwal (String)

createdAt (Timestamp)

Collection reviews:

reviewerName (String)

rating (Number)

comment (String)

createdAt (Timestamp)

Bagian 4: Master AI Prompt untuk Eksekusi Koding

Gunakan teks prompt di bawah ini pada AI Code Editor (seperti Antigravity atau VS Code AI) saat Anda masuk ke tahap pembuatan kode untuk diisikan ke widget HTML3 Blogger:

Bertindaklah sebagai Senior Front-End Developer dan Blogger Theme Expert. Buatkan kode HTML5 lengkap menggunakan kerangka Bootstrap 5.3.3 CDN, Bootstrap Icons, dan AOS Animation untuk diisikan ke dalam widget HTML3 (Landing Page Di Sini) pada file Blogspot_V4.9.xml.

ATURAN UTAMA:
1. JANGAN gunakan Bootstrap 3, jQuery, OwlCarousel, atau WOW.js. Gunakan murni Bootstrap 5.3.3, AOS, dan Vanilla JavaScript.
2. Terapkan palet warna Dark Luxury: Background utama #0F1115, Kartu Surface #181B22, Aksen Gold/Bronze #CDA45E, dan Teks #D1D5DB.
3. Desain harus sepenuhnya responsif di layar laptop (1920x1080p) dan mobile.

STRUKTUR HTML YANG HARUS DIBUAT DALAM SATU BLOK KODE:
1. #hero: Banner utama dengan judul "Gentleman's Forge Barbershop - Kota Batu", informasi jam buka, dan tombol reservasi.
2. #about: Seksi cerita studio dan 6 fasilitas unggulan dalam grid modern.
3. #services: Daftar menu layanan cukur dan harga (Gentleman Cut, Shave, Coloring) dengan tata letak dua kolom elegan.
4. #team: Grid 4 kartu kapster profesional.
5. #lookbook: Galeri portofolio gaya rambut (Curly, Fade, Mullet, Undercut, dll.).
6. #reservation: Formulir pemesanan online interaktif yang terhubung ke Firebase Firestore, lengkap dengan elemen <div id="daftarAntrean"> untuk menampilkan data antrean secara real-time.
7. Script Modular Firebase v10+ (menggunakan gstatic.com) yang menangani event submit form booking ke collection 'bookings' di Firestore dan pembacaan data real-time menggunakan onSnapshot.
