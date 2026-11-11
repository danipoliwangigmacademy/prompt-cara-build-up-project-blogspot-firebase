Bertindaklah sebagai Senior UI/UX Designer dan Frontend Architect yang ahli dalam prototyping cepat menggunakan Stich. Buatkan wireframe dan tata letak struktur halaman (layout structure) yang lengkap, clean, dan profesional untuk proyek website One-Page "Gentleman's Forge Barbershop".

STANDAR DESAIN & SPESIFIKASI LAYAR:
- Target Viewport: Standar Laptop/Desktop (1920x1080px) dengan transisi responsif yang sempurna ke mobile.
- Tema & Mood: Dark Luxury & Modern Industrial (Gaya BootstrapMade Restaurantly / Append).
- Palet Warna: 
  * Background Utama: Deep Charcoal (#121212)
  * Surface/Card: Dark Slate (#1C1F26)
  * Aksen Utama (CTA & Badge): Warm Bronze / Gold (#C59D5F)
  * Teks Utama: Pure White (#FFFFFF) & Muted Gray (#A0AAB2)
- Tipografi: Heading menggunakan font serif elegan ('Playfair Display') dan Body menggunakan sans-serif bersih ('Plus Jakarta Sans' / 'Inter').

STRUKTUR SEKSI WIREFRAME YANG HARUS DIBUAT (URUTAN DARI ATAS KE BAWAH):

1. TOPBAR & STICKY GLASSMORPHISM NAVBAR:
   - Bar atas tipis menampilkan jam operasional ("Senin - Sabtu: 10:00 - 21:00") dan nomor telepon.
   - Navbar utama dengan efek backdrop-blur, logo di kiri, dan menu navigasi anchor: [Tentang Kami], [Layanan], [Team Barber], [Lookbook], [Reservasi], [Lokasi].
   - Tombol Call-to-Action (CTA) di sebelah kanan navbar: Berwarna Gold dengan teks "Reservasi Kursi".

2. HERO SECTION (BANNER UTAMA):
   - Background gelap penuh dengan overlay gambar suasana barbershop yang elegan.
   - Headline tebal maskulin: "Seni Cukur Presisi Untuk Karakter Pria Sejati".
   - Sub-headline singkat tentang layanan premium di Kota Batu.
   - Dua tombol CTA berdampingan: "Booking Jadwal Sekarang" (Primary Gold) dan "Lihat Katalog Layanan" (Outline White).

3. SECTION TENTANG KAMI & BENTO GRID FASILITAS:
   - Layout 2 kolom: Sisi kiri menampilkan foto studio berkualitas tinggi dengan border aksen gold, sisi kanan teks narasi tentang pengalaman kapster.
   - Di bawahnya, buat Bento Grid berisi 6 kartu fasilitas unggulan dengan ikon minimalis: Ruang Full AC, Sterilisasi Alat UV, Free Wi-Fi, Handuk Hangat Aromaterapi, Complimentary Drink, dan Area Parkir Luas.

4. SECTION KATALOG LAYANAN & HARGA (Gaya Menu Restoran Modern):
   - Judul seksi: "Layanan Terbaik & Harga Ramah".
   - Tampilan daftar harga 2 kolom dengan titik-titik penghubung (dots leader) antara Nama Layanan (misal: Gentleman Cut, Hot Towel Shave, Hair Coloring), Harga (IDR 20K - IDR 65K), dan deskripsi durasi pengerjaan.
   - Tombol "Pilih Layanan" di setiap item yang terhubung langsung ke form booking di bawah.

5. SECTION TIM MASTER BARBER:
   - Judul seksi: "Tenaga Ahli Berpengalaman".
   - Grid 4 kartu kapster (Adit, Bima, Doni, Rian) dengan foto berbentuk portrait rapi, nama tebal berwarna gold, spesialisasi keahlian, dan tombol tautan sosial media.

6. SECTION LOOKBOOK & GALERI GAYA RAMBUT (Blog-Style Preview):
   - Judul seksi: "Hasil Potongan Rambut Terbaik Kami".
   - Filter kategori galeri: [All], [Fade Style], [Classic], [Modern Texture].
   - Grid 8 kartu foto gaya rambut (Curly, High Fade, Messy, Mohawk, Mullet, Quiff, Two Block, Undercut) dengan efek zoom saat kursor mendekat (hover).

7. SECTION ONLINE RESERVATION & LIVE QUEUE (Integrasi Firebase):
   - Layout 2 kolom interaktif:
     * Kolom Kiri (Form Booking): Input Nama Lengkap, Nomor WhatsApp, Dropdown Pilihan Layanan, Dropdown Pilihan Barber, Pemilihan Tanggal & Jam, serta tombol "Kirim Reservasi".
     * Kolom Kanan (Live Antrean & Ulasan): Kartu tampilan data antrean real-time yang mensimulasikan data dari database Firebase Firestore (Nama Pelanggan, Paket, Status Antrean).

8. SECTION LOKASI, JAM OPERASIONAL & FOOTER:
   - Menampilkan kotak informasi alamat lengkap di Temas, Kota Batu, kotak Google Maps interaktif, dan tabel jam buka harian.
   - Footer bawah: Logo, tautan media sosial (Instagram, TikTok, WhatsApp), dan teks hak cipta (Copyright).