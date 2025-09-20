# Dokumen PRD (Product Requirement Document) – FinNote
**Kelompok:**  
- Rifqy Niam Fadhil (1241)  
- Muhammad Ariyanto (1281)  

---

## 1. Pendahuluan (Introduction)  
**FinNote** adalah aplikasi pencatatan keuangan pribadi yang dirancang untuk membantu pengguna mengelola pemasukan dan pengeluaran sehari-hari secara sederhana, cepat, dan terorganisir.  

Dengan fokus pada kemudahan penggunaan dan kinerja yang ringan, FinNote memungkinkan pengguna mencatat transaksi, melihat ringkasan saldo, serta memantau laporan bulanan tanpa kerumitan.  

Aplikasi ini akan dikembangkan menggunakan **Flutter** dengan arsitektur **Clean Code** untuk memastikan skalabilitas, pemeliharaan yang mudah, dan pengalaman pengguna yang optimal.  

---

## 2. Tujuan Produk (Product Goals)  
- Memberikan solusi pencatatan keuangan yang simpel, cepat, dan mudah dipahami.  
- Membantu pengguna mengatur dan melacak pemasukan serta pengeluaran harian.  
- Menyediakan laporan keuangan bulanan yang sederhana.  
- Menawarkan pengalaman pengguna yang modern, intuitif, dan minimalis.  
- Memastikan kinerja aplikasi yang ringan, responsif, dan aman.  

---

## 3. Target Pengguna (Target Audience)  
- Mahasiswa yang ingin mencatat pengeluaran sehari-hari.  
- Pekerja atau karyawan yang ingin memantau kondisi finansial pribadi.  
- Pelaku UMKM atau usaha kecil yang membutuhkan catatan transaksi sederhana.  
- Individu yang lebih suka aplikasi keuangan ringan dibandingkan aplikasi kompleks.  

---

## 4. Lingkup Fitur (Feature Scope)  

### Manajemen Transaksi Dasar  
- Tambah Transaksi: Catat pemasukan/pengeluaran dengan jumlah, deskripsi, tanggal, dan kategori.  
- Lihat Daftar Transaksi: Menampilkan semua transaksi dengan filter tanggal/kategori.  
- Edit Transaksi: Mengubah detail transaksi yang sudah dicatat.  
- Hapus Transaksi: Menghapus transaksi tertentu.  

### Kategori Transaksi  
- Tambah kategori baru (contoh: Makanan, Transportasi, Tabungan).  
- Hapus kategori.  
- Tipe kategori (Pemasukan atau Pengeluaran).  

### Ringkasan & Laporan  
- Ringkasan saldo total (pemasukan – pengeluaran).  
- Laporan bulanan sederhana dengan grafik (opsional setelah MVP).  

### UI/UX Dasar  
- Halaman dashboard saldo + transaksi terbaru.  
- Halaman daftar transaksi lengkap.  
- Form tambah/edit transaksi.  
- Navigasi sederhana (tab atau drawer).  
- Tema Light/Dark Mode.  

---

## 5. Arsitektur Teknis (Technical Architecture)  

### Lapisan Presentasi (Presentation Layer)  
- Flutter (UI/UX).  
- State management: Provider atau Riverpod.  
- Navigasi: GoRouter.  

### Lapisan Domain (Domain Layer)  
- Business logic inti aplikasi.  
- Entity: Transaksi, Kategori.  
- Use cases: tambah transaksi, hitung saldo, buat laporan.  

### Lapisan Data (Data Layer)  
- Repositori & data source.  
- SQLite (pakai Drift/Hive) untuk database lokal.  
- Logger untuk debugging.  

---

## 6. User Interface (UI) dan User Experience (UX)  
- Desain minimalis, sederhana, dan mudah dipahami.  
- Navigasi jelas dengan fokus pada pencatatan transaksi.  
- Tampilan responsif untuk berbagai ukuran layar.  
- Mendukung tema Light dan Dark Mode.  
- Ringkasan saldo terlihat di halaman utama.  

---

## 7. Metrik Keberhasilan (Success Metrics)  
- Jumlah unduhan dan pengguna aktif harian/mingguan.  
- Retensi pengguna dalam 7, 30, dan 90 hari.  
- Frekuensi penggunaan fitur utama (pencatatan transaksi).  
- Rating aplikasi di Google Play Store.  
- Performa aplikasi (cepat, ringan, hemat memori).  

---

## 8. Batasan (Constraints)  
- Platform awal: Android (min. Android 8.0).  
- Bahasa: Bahasa Indonesia sebagai bahasa utama.  
- Penyimpanan data lokal, tanpa autentikasi akun (untuk MVP).  
- Monetisasi: Versi awal gratis dengan fitur inti.  

---

## 9. Rencana Rilis (Release Plan)  

**MVP (Alpha Release):**  
- Fitur inti (catat transaksi, kategori, ringkasan saldo, UI sederhana).  
- Pengujian internal.  

**Beta Release:**  
- Perbaikan bug berdasarkan feedback tester.  
- Penambahan laporan bulanan sederhana.  

**Public Release:**  
- Rilis di Google Play Store.  
- Promosi dan pengumpulan review pengguna.  

**Iterasi Selanjutnya:**  
- Sinkronisasi data cloud.  
- Export laporan ke PDF/Excel.  
- Fitur premium (multi-device, backup otomatis).  

---

## 10. Lampiran (Appendices)  
- ERD sederhana (Transaksi – Kategori).  
- Wireframe awal aplikasi (akan ditambahkan setelah PRD disetujui).  
- Skema tabel database SQLite (Transaksi, Kategori).  

---
