Nama    : Johannes Hutagalung
Nim     : 41426034
Prodi   : DIV-Teknologi Rekayasa Perangkat Lunak

Laporan Praktikum PSW I - Minggu 5 Sesi 2

1. Cara Menjalankan Web
A. Buka folder proyek ini di VS Code.
B. Klik kanan file index.html, lalu pilih Open with Live Server.
C. Buka DevTools di browser (tekan tombol F12) untuk melihat tampilan dan mencoba ukuran layar.

2. Catatan Hasil Percobaan
 **Navigasi Fleksibel:**
  Saya memakai display: flex dan flex-wrap: wrap pada navigasi. Ketika ukuran layar disempitkan, tombol navigasi tidak terpotong melainkan otomatis pindah ke baris bawahnya. Saat dicoba ganti flex-direction: column, tampilan navigasi berubah menjadi tersusun ke bawah.
  **Card Fleksibel:** 
  Saya memberi aturan flex: 15rem dan min-width: 0 pada bagian card. Di layar lebar (1200px) card akan berjejer ke samping, sedangkan di layar HP yang sempit (360px) card otomatis tersusun ke bawah.
 **Konten Judul Panjang:**
    Saya mencoba memasukkan judul yang sangat panjang tanpa spasi. Dengan menambahkan overflow-wrap: anywhere pada CSS judul (card h2), tulisan panjang tersebut tidak melipat keluar kotak card, bahkan saat browser di-zoom sampai 200%.

3. Tabel Hasil Pengujian (Matriks Uji)
Kasus yang Diuji:
**Layar Lebar (1200px)**
Yang Saya Lakukan:
Mengubah lebar layar browser ke 1200px
Hasil yang Terjadi:
Keempat card berjejer rapi ke samping
Lolos (`bukti/responsive-1200px.png`) 

Kasus yang Diuji
**Layar HP Sempit (360px)**
Yang Saya Lakukan:
Mengubah lebar layar browser ke 360px
Hasil yang Terjadi:
Card berpindah baris dan tersusun ke bawah
Status:
Lolos (`bukti/responsive-360px.png`)

Kasus yang Diuji
**Judul Panjang & Zoom 200%**
Yang Saya Lakukan:
Memasukkan judul panjang tanpa spasi & zoom 200%
Hasil yang Terjadi:
Teks memotong rapi ke bawah, kotak tidak hancur 
Status:
Lolos (`bukti/zoom-200px.png`)

Kasus yang Diuji:
**Navigasi Pakai Tombol Tab**
Yang Saya Lakukan:
Menekan tombol `Tab` di keyboard berulang kali
Hasil yang Terjadi:
Urutan fokus berpindah dari satu menu ke menu lain
Lolos

**Catatan hasil validator before vs after**
1. Error yang ditunjukkan oleh validator disebabkan pada kode baris 21 saya terdapat tag penutup </article> sedangkan diatasnya tidak ada tanda pembuka tag <article>
2. Untuk fix errornya saya menghapus tag </article> penutup yang berada di kode baris 21 yang dimana ini adalah tag yang nyasar karena saya lupa menghapus karena menyalin dari week 2 

4. AI Use Statement (Penggunaan AI)
**Alat yang Digunakan:** Gemini AI
**Tujuan:** Membantu memahami perintah modul, membantu memperbaiki error CSS, dan memberikan panduan penulisan laporan.
**Bagian yang Dibantu:** Penjelasan cara kerja Flexbox, perbaikan struktur HTML, dan penyusunan tabel pengujian.
**Cara Memverifikasi:** Saya mengecek langsung hasilnya di browser Google Chrome, mencoba fitur DevTools (overlay flexbox & mode responsif), dan memastikan kodenya berjalan dengan benar.
