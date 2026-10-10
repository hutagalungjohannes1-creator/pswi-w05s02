Nama    : Johannes Hutagalung
Nim     : 41426034
Prodi   : DIV-Teknologi Rekayasa Perangkat Lunak

Laporan Praktikum PSW I - Minggu 5 Sesi 3

1. Mengubah Container
a. Tindakan yang Dilakukan:
Mengubah nama class elemen kontainer pembungkus pada index.html dari cards menjadi catalog.
b. Menghapus properti Flexbox pada kontainer di file style.css dan menerapkan aturan CSS Grid
c. Menguji tampilan dua kolom pada browser melalui server lokal.
Mengaktifkan Grid Overlay melalui Browser DevTools (tab Elements) dan mengamati struktur DOM anak langsung.

2. Grid Adaptif
Tindakan yang Dilakukan:

a. Mengubah definisi kolom pada .catalog di style.css menggunakan pola repeat(auto-fit, minmax(min(100%, 15rem), 1fr)).
b. Menambahkan item <article> kelima pada struktur HTML.
c. Menguji responsivitas tata letak pada viewport 320px, 768px, dan 1200px menggunakan fitur Responsive Design Mode di DevTools.
Bukti / Catatan Pengujian:
Pada folder bukti ada beberapa screenshot

3. REVIEW LAYOUT
Tindakan:
a. Memeriksa urutan tulisan di HTML supaya tetap rapi dan sesuai urutan aslinya tanpa diubah-ubah paksa posisinya menggunakan kode
b. Mencoba tes halaman web dengan kondisi jumlah kartu yang berbeda-beda: pas dicoba tanpa kartu (0), saat ada 1 kartu, sampai dikembalikan lagi menjadi 5 kartu.
Mengatur jarak dalam kartu (padding) menggunakan kode: padding: var(--space-2, 1rem);.

Hasilnya:
Tampilan web tetap stabil, rapi, dan tidak berantakan meskipun jumlah kartunya dikurangi atau ditambah

Alasan Pakai Grid dan Flexbox:
CSS Grid dipakai untuk bagian luar (katalog) karena paling gampang buat bikin kotak-kotak yang otomatis sejajar rapi ke samping atau ke bawah sendiri menyesuaikan layar.
Flexbox dipakai untuk bagian dalam kartu karena sangat pas buat merapikan isi kartu secara vertikal (dari judul, deskripsi, sampai tombol link ke bawah) dengan jarak yang rapi

4. LATIHAN MANDIRI DAN MATRIKS UJI.
Pengujian Ukuran Layar Kecil (320px):
Saat halaman web diuji pada ukuran layar sangat kecil (seperti 320px), hasilnya tidak mengalami overflow atau geseran ke samping. Teks dan kartu menyesuaikan lebar layar dengan rapi.
Pengujian Jumlah Kartu (Satu dan Lima Kartu):
Ketika diuji dengan satu kartu maupun lima kartu sekaligus, tata letak tetap terbaca dengan sangat baik. Posisi kartu otomatis berpindah (auto-placement) mengikuti luas ruang yang tersedia di layar.
Pengujian Urutan Tab (Navigasi Keyboard):
Saat tombol Tab pada keyboard ditekan berulang kali, urutan fokus berpindah secara teratur sesuai dengan urutan elemen di dalam HTML (DOM), mulai dari menu navigasi atas hingga turun ke tombol-tombol yang ada di dalam kartu.

Hasil Laporan Eksperimen (Kasus Normal, Batas, dan Gagal):
Kasus Normal: Ketika menampilkan 5 kartu secara penuh di layar laptop, semua kartu berjejer ke samping dengan jarak spasi yang pas dan rapi (bukti screenshot tersimpan di folder bukti).
Kasus Batas: Saat ukuran layar diperkecil menyerupai HP, tampilan katalog otomatis berubah menjadi satu kolom ke bawah tanpa ada bagian yang terpotong (bukti screenshot di bukti/grid-adaptif-320px.png)
Kasus Gagal: Saat diuji dengan teks judul yang sangat panjang tanpa spasi, teks tersebut tetap aman dan otomatis turun ke bawah karena sudah dilindungi oleh kode overflow-wrap: anywhere pada CSS.

AI Use Statement
Alat yang Digunakan: Asisten AI (Gemini).
Tujuan Penggunaan: Digunakan untuk memahami konsep tata letak responsif (responsive layout), mendiagnosis kesalahan penulisan sintaks CSS (troubleshooting), serta membantu menyusun format laporan dokumentasi pada file README.md
Bagian Bantuan: AI membantu memberikan penjelasan mengenai struktur CSS Grid dan Flexbox, memperbaiki struktur blok kode .card yang sempat bersarang (nested), serta menyusun draf catatan pengamatan dan matriks uji dalam bentuk teks biasa.
Verifikasi: Seluruh saran kode, hasil penyesuaian CSS, dan skenario pengujian telah diuji langsung melalui peramban web (browser) lokal serta divalidasi kesesuaian tampilannya dengan ketentuan modul sebelum dimasukkan ke dalam laporan.
