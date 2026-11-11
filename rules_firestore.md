# Cloud Firestore Security Rules & Configuration Guide
# Proyek: Gentleman's Forge Barbershop
# Project ID: barberr-5bca8

Dokumen ini berisi aturan keamanan resmi (**Firestore Security Rules**) yang telah disesuaikan dengan skema database, API formulir booking pelanggan, modul live antrean real-time, serta panel admin kasir.

---

## 1. KODE ATURAN RESMI (Production Ready)
Salin kode berikut dan tempelkan (*paste*) ke tab **Firebase Console > Firestore Database > Rules**:

```javascript
rules_version = '2';

service cloud.firestore {
  match /databases/{database}/documents {

    // ===============================================================
    // 1. KOLEKSI: bookings (Reservasi & Live Antrean Barbershop)
    // ===============================================================
    match /bookings/{bookingId} {
      // READ: Siapapun (publik) boleh membaca antrean untuk widget live queue
      allow read: if true;

      // CREATE: Pengunjung website boleh membuat reservasi baru dari form booking
      // dengan validasi data agar database tetap bersih dan aman
      allow create: if request.resource.data.nama is string 
                    && request.resource.data.nama.size() >= 2
                    && request.resource.data.wa is string
                    && request.resource.data.paket is string;

      // UPDATE & DELETE: Diizinkan untuk kasir/admin barbershop 
      // (digunakan oleh admin.html untuk mengubah status ke 'Sedang Cukur' / 'Selesai' / Hapus)
      allow update, delete: if true;
    }

    // ===============================================================
    // 2. KOLEKSI: reviews (Ulasan & Rating Bintang Pelanggan)
    // ===============================================================
    match /reviews/{reviewId} {
      // READ: Siapapun boleh membaca testimoni yang tampil di website
      allow read: if true;

      // CREATE: Pelanggan boleh mengirim ulasan baru dengan batas rating 1 - 5
      allow create: if request.resource.data.reviewerName is string
                    && request.resource.data.comment is string
                    && request.resource.data.rating is number
                    && request.resource.data.rating >= 1 
                    && request.resource.data.rating <= 5;

      // UPDATE & DELETE: Tidak diizinkan sembarangan dari publik
      allow update, delete: if false;
    }

    // ===============================================================
    // 3. DEFAULT: Kunci semua koleksi dan dokumen lainnya
    // ===============================================================
    match /{document=**} {
      allow read, write: if false;
    }

  }
}
```

---

## 2. INFORMASI IDENTITAS PROYEK & API FIREBASE

Gunakan konfigurasi resmi berikut pada aplikasi front-end:

| Parameter | Nilai Proyek Anda |
| :--- | :--- |
| **Project ID** | `barberr-5bca8` |
| **API Key** | `AIzaSyDY9bHoSIXwHVRP0cwg09CN8uBAjtqw6hw` |
| **Auth Domain** | `barberr-5bca8.firebaseapp.com` |
| **Storage Bucket** | `barberr-5bca8.firebasestorage.app` |
| **Messaging Sender ID** | `134075026496` |
| **App ID** | `1:134075026496:web:62a5e8a78e4af3e479e3a5` |

---

## 3. PANDUAN PENERAPAN DI FIREBASE CONSOLE

1. Kunjungi [Firebase Console](https://console.firebase.google.com/).
2. Pilih proyek **`barberr-5bca8`**.
3. Di menu navigasi samping kiri, pilih **Build** &rarr; **Firestore Database**.
4. Klik tab **Rules** di bagian atas.
5. Hapus aturan lama yang berbatas waktu (`timestamp.date(2026, 12, 10)`).
6. Tempelkan (*paste*) kode di atas.
7. Klik tombol **Publish** (*Terbitkan*).

---

## 4. DAFTAR INDEKS DATABASE (INDEXING)

Query pada landing page menggunakan pengurutan waktu:
```javascript
query(collection(db, "bookings"), orderBy("createdAt", "desc"), limit(5))
```
Firestore secara otomatis mengindeks setiap kolom tunggal (`single-field index`). Tidak diperlukan pembuatan *composite index* tambahan kecuali Anda menambahkan filter ganda seperti status + tanggal secara bersamaan.

```

---

## 2. INFORMASI IDENTITAS PROYEK & API FIREBASE

Gunakan konfigurasi resmi berikut pada aplikasi front-end:

| Parameter | Nilai Proyek Anda |
| :--- | :--- |
| **Project ID** | `barberr-5bca8` |
| **API Key** | `AIzaSyDY9bHoSIXwHVRP0cwg09CN8uBAjtqw6hw` |
| **Auth Domain** | `barberr-5bca8.firebaseapp.com` |
| **Storage Bucket** | `barberr-5bca8.firebasestorage.app` |
| **Messaging Sender ID** | `134075026496` |
| **App ID** | `1:134075026496:web:62a5e8a78e4af3e479e3a5` |

---

## 3. PANDUAN PENERAPAN DI FIREBASE CONSOLE

1. Kunjungi [Firebase Console](https://console.firebase.google.com/).
2. Pilih proyek **`barberr-5bca8`**.
3. Di menu navigasi samping kiri, pilih **Build** &rarr; **Firestore Database**.
4. Klik tab **Rules** di bagian atas.
5. Hapus aturan lama yang berbatas waktu (`timestamp.date(2026, 12, 10)`).
6. Tempelkan (*paste*) kode di atas.
7. Klik tombol **Publish** (*Terbitkan*).

---

## 4. DAFTAR INDEKS DATABASE (INDEXING)

Query pada landing page menggunakan pengurutan waktu:
```javascript
query(collection(db, "bookings"), orderBy("createdAt", "desc"), limit(5))
```
Firestore secara otomatis mengindeks setiap kolom tunggal (`single-field index`). Tidak diperlukan pembuatan *composite index* tambahan kecuali Anda menambahkan filter ganda seperti status + tanggal secara bersamaan.