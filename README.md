# 📒 FinNote – Aplikasi Pencatatan Keuangan Pribadi
**Kelompok:**  
- Rifqy Niam Fadhil (1241)  
- Muhammad Ariyanto (1281)  

---

## 📌 Deskripsi
**FinNote** adalah aplikasi pencatatan keuangan pribadi berbasis **Flutter** yang dikembangkan untuk memberikan solusi sederhana dan praktis dalam mengelola keuangan sehari-hari.  

Di tengah kesibukan mahasiswa, pekerja, maupun pelaku usaha kecil, sering kali pencatatan keuangan diabaikan atau dilakukan secara manual sehingga menyulitkan ketika ingin mengevaluasi kondisi finansial. FinNote hadir untuk menjawab kebutuhan tersebut dengan menghadirkan fitur pencatatan transaksi yang mudah, cepat, dan dapat diakses kapan saja.  

Aplikasi ini memungkinkan pengguna untuk:  
- **Mencatat pemasukan dan pengeluaran** hanya dengan beberapa klik.  
- **Mengelompokkan transaksi** berdasarkan kategori yang fleksibel seperti makanan, transportasi, atau tabungan.  
- **Menampilkan ringkasan saldo** secara otomatis sehingga pengguna selalu tahu kondisi keuangan terkini.  
- **Menyediakan laporan bulanan sederhana** yang membantu pengguna menganalisis pola pengeluaran dan kebiasaan finansial.  

FinNote dirancang dengan antarmuka yang minimalis dan intuitif agar mudah digunakan oleh semua kalangan, bahkan bagi yang baru pertama kali mencoba aplikasi keuangan. Dengan performa yang ringan dan responsif, aplikasi ini juga dapat berjalan lancar di perangkat dengan spesifikasi menengah tanpa mengorbankan pengalaman pengguna.  

Tidak hanya itu, FinNote juga dikembangkan dengan arsitektur **Clean Code** sehingga kode lebih terstruktur, mudah dikembangkan, dan bisa diperluas untuk fitur lanjutan di masa depan seperti sinkronisasi cloud, ekspor laporan ke PDF/Excel, maupun integrasi dengan sistem pembayaran digital.  

Dengan filosofi “simpel, cepat, dan berguna”, FinNote diharapkan dapat menjadi teman keuangan yang setia untuk membantu pengguna lebih bijak dalam mengelola setiap rupiah yang dimiliki.  

---

## 🎯 Tujuan Aplikasi
- Memberikan solusi pencatatan keuangan yang simpel, cepat, dan mudah dipahami.  
- Membantu pengguna mengatur pemasukan dan pengeluaran sehari-hari.  
- Menampilkan ringkasan saldo secara otomatis.  
- Menyediakan laporan bulanan sederhana.  
- Menghadirkan pengalaman pengguna yang modern dan intuitif.  

---

## 👥 Target Pengguna
- Mahasiswa yang ingin mencatat pengeluaran sehari-hari.  
- Pekerja atau karyawan yang ingin memantau finansial pribadi.  
- Pelaku UMKM atau usaha kecil yang butuh catatan transaksi sederhana.  
- Individu yang lebih suka aplikasi keuangan ringan dibanding aplikasi kompleks.  

---

## 📂 Struktur & Dokumen Proyek
Repositori ini juga mencakup dokumen–dokumen pendukung sebagai bagian dari tugas perancangan perangkat lunak:  

1. **01_PRD_Product_Requirement_Document.md** – Dokumen kebutuhan produk (Product Requirement Document).  
2. **02_SRS_Software_Requirement_Specification.md** – Dokumen spesifikasi kebutuhan perangkat lunak.  
3. **03_ERD_Entity_Relationship_Diagram.md** – Representasi basis data aplikasi dalam bentuk teks.  
4. **04_SDD_Software_Design_Document.md** – Dokumen desain arsitektur dan interaksi komponen sistem.  
5. **05_SPRINT_MVP_Timeline_Checklist.md** – Rencana kerja sprint pengembangan MVP.  

---

## 🛠️ Teknologi yang Digunakan
- **Flutter** → Framework pengembangan aplikasi.  
- **Dart** → Bahasa pemrograman utama.  
- **SQLite (Drift/Hive)** → Database lokal untuk menyimpan transaksi dan kategori.  
- **Riverpod/Provider** → State management.  
- **GoRouter** → Navigasi antar halaman.  

---

## 🚀 Fitur Utama (MVP)
- Tambah, edit, hapus transaksi.  
- Kelola kategori (pemasukan/pengeluaran).  
- Ringkasan saldo otomatis.  
- Laporan bulanan sederhana.  
- UI minimalis + dark mode.  

---
## Product Requirements Document (PRD) - Smart Kasir
---
1. Pendahuluan
Smart Kasir adalah aplikasi kasir digital cerdas yang dirancang untuk membantu pemilik usaha kecil hingga menengah dalam mengelola transaksi penjualan, inventaris produk, dan laporan keuangan dengan lebih cepat, praktis, dan efisien. Aplikasi ini bertujuan untuk menyederhanakan operasional harian, mengurangi kesalahan manual, dan menyediakan wawasan bisnis yang actionable bagi UMKM.
2. Visi Produk
Menjadi aplikasi kasir pilihan utama bagi UMKM di Indonesia yang menawarkan solusi komprehensif, mudah digunakan, dan berbasis data untuk meningkatkan efisiensi operasional dan mendukung pertumbuhan bisnis.
3. Tujuan Bisnis
Meningkatkan efisiensi proses penjualan UMKM hingga 30%.
Mengurangi waktu yang dihabiskan untuk pencatatan manual dan rekap laporan.
Memberikan wawasan tentang kinerja produk dan tren penjualan kepada pemilik usaha.
Menyediakan platform yang stabil dan andal untuk pengelolaan bisnis sehari-hari.
4. Target Pengguna
Primer: Pemilik usaha kecil dan menengah (UMKM) seperti toko kelontong, kafe/restoran kecil, butik, kios, dan usaha retail sejenis.
Sekunder: Karyawan/Kasir di UMKM tersebut.
Kebutuhan Pengguna:
Proses transaksi yang cepat dan mudah.
Manajemen stok yang akurat.
Laporan penjualan yang informatif dan mudah diakses.
Biaya operasional yang rendah (simpel, ringan, tanpa perangkat mahal).
Akses data yang aman dan terjamin.
5. Fitur Produk (Detailed Requirements)
Berikut adalah daftar fitur utama Smart Kasir, dibagi berdasarkan kategori fungsionalitas:
5.1. Core Penjualan & Transaksi (POS)
5.1.1. Halaman Utama / POS:
Deskripsi: Antarmuka utama untuk melakukan transaksi penjualan.
Persyaratan:
Menampilkan daftar produk yang mudah dicari (berdasarkan nama/barcode).
Mekanisme untuk menambahkan produk ke keranjang belanja.
Menampilkan detail keranjang belanja (nama produk, kuantitas, harga, subtotal).
Opsi untuk menyesuaikan kuantitas produk atau menghapus item dari keranjang.
Menampilkan total pembayaran secara real-time.
5.1.2. Proses Pembayaran:
Deskripsi: Memungkinkan kasir untuk menyelesaikan pembayaran dan mencatat transaksi.
Persyaratan:
Pilihan metode pembayaran: Tunai dan Non-Tunai (Debit/Kredit/QRIS - sebagai penanda, tanpa integrasi gateway di MVP).
Untuk pembayaran tunai: input jumlah uang yang diterima dan otomatis menampilkan kembalian.
Opsi untuk menerapkan diskon (persen/nominal) ke seluruh transaksi atau per item.
Merekam nama kasir yang melakukan transaksi.
5.1.3. Riwayat Transaksi:
Deskripsi: Melihat daftar transaksi yang telah selesai.
Persyaratan:
Menampilkan daftar transaksi dengan informasi dasar (tanggal, waktu, total, kasir).
Filter berdasarkan tanggal.
Detail transaksi lengkap (produk, kuantitas, harga, diskon, metode pembayaran) saat dipilih.
5.2. Manajemen Produk & Inventaris
5.2.1. Daftar Produk:
Deskripsi: Mengelola daftar produk yang dijual.
Persyaratan:
Menampilkan daftar semua produk dengan nama, harga jual, stok, dan kategori.
Fungsi pencarian dan filter produk.
5.2.2. Tambah/Edit/Hapus Produk:
Deskripsi: Menambah, mengubah, atau menghapus informasi produk.
Persyaratan:
Formulir input untuk nama produk, harga beli (opsional, untuk perhitungan profit), harga jual, stok awal, kategori, kode produk/barcode.
Opsi untuk mengunggah gambar produk (opsional di MVP).
Validasi input data.
5.2.3. Manajemen Stok:
Deskripsi: Memastikan akurasi stok dan memberikan peringatan.
Persyaratan:
Stok otomatis berkurang setelah transaksi penjualan.
Opsi untuk penyesuaian stok manual (penambahan/pengurangan).
Pengaturan batas minimum stok untuk setiap produk.
Notifikasi/peringatan ketika stok produk mencapai batas minimum.
5.3. Laporan & Analisis
5.3.1. Laporan Penjualan:
Deskripsi: Menyediakan ringkasan dan analisis penjualan.
Persyaratan:
Filter laporan berdasarkan periode waktu (harian, mingguan, bulanan, kustom).
Menampilkan ringkasan: Total Omset, Jumlah Transaksi, Total Diskon, Penjualan Bersih.
Visualisasi data penjualan dalam bentuk grafik (misal: tren penjualan harian/bulanan).
Daftar produk terlaris berdasarkan kuantitas atau omset.
Informasi jam-jam transaksi ramai.
Opsi untuk mengekspor laporan ke format PDF dan Excel.
5.4. Cetak & Berbagi Struk
5.4.1. Struk Transaksi:
Deskripsi: Memberikan struk kepada pelanggan.
Persyaratan:
Fungsi untuk mencetak struk menggunakan printer thermal (Bluetooth).
Opsi untuk mengirim struk digital (teks sederhana atau PDF) melalui WhatsApp atau SMS ke nomor pelanggan.
Struk mencakup detail transaksi, nama toko, tanggal, dan total pembayaran.
5.5. Pengaturan & Lain-lain
5.5.1. Manajemen Pengguna:
Deskripsi: Mengelola akses pengguna (pemilik, kasir).
Persyaratan:
Sistem login dengan username dan password.
Dua peran: Pemilik (akses penuh) dan Kasir (hanya akses POS dan riwayat transaksi sendiri).
Pemilik dapat menambah, mengedit, atau menghapus akun kasir.
5.5.2. Pengaturan Toko:
Deskripsi: Mengatur informasi dasar toko.
Persyaratan:
Input nama toko, alamat, dan nomor telepon.
Pengaturan mata uang.
5.5.3. Backup & Sinkronisasi Data:
Deskripsi: Melindungi data dan memastikan konsistensi.
Persyaratan:
Opsi backup data ke perangkat lokal.
Opsi restore data dari backup lokal.
(Future/Enhancement): Sinkronisasi data ke cloud untuk multi-perangkat atau backup otomatis.
6. Persyaratan Teknis & Arsitektur
Platform: Android, iOS (Target utama: Android untuk UMKM).
Framework: Flutter.
State Management: Riverpod Generator.
Data Models: Freezed.
Navigasi: Go_router.
Error Handling/Functional Programming: fpdart (opsional, untuk kasus tertentu).
Logging: Logger.
Database Lokal: Drift (SQLite).
Arsitektur: Clean Code (Presentation, Domain, Data Layers).
Offline Support: Aplikasi harus berfungsi penuh secara offline, dengan sinkronisasi data saat koneksi tersedia (jika fitur cloud diimplementasikan).
7. Desain & Pengalaman Pengguna (UX/UI)
Simplicity: Antarmuka harus sangat intuitif, bersih, dan minimalis.
Efisiensi: Alur kerja transaksi harus cepat, meminimalkan jumlah ketukan atau navigasi.
Aksesibilitas: Ikon yang jelas, teks yang mudah dibaca, dan kontras warna yang baik.
Konsistensi: Desain komponen UI yang konsisten di seluruh aplikasi.
Feedback Visual: Memberikan umpan balik yang jelas untuk setiap tindakan pengguna (misal: notifikasi sukses/gagal).
8. MVP (Minimum Viable Product) Scope
Untuk iterasi awal, MVP akan fokus pada fitur-fitur inti berikut untuk memberikan nilai langsung kepada UMKM:
Core Penjualan & Transaksi: Halaman POS, Proses Pembayaran (Tunai/Non-Tunai sebagai penanda), Riwayat Transaksi (basic).
Manajemen Produk & Inventaris: Daftar Produk, Tambah/Edit/Hapus Produk, Manajemen Stok (pengurangan otomatis & penyesuaian manual), Peringatan Stok Menipis.
Laporan Dasar: Ringkasan Penjualan (Harian/Bulanan), Produk Terlaris.
Cetak Struk: Integrasi dengan printer thermal (Bluetooth).
Manajemen Pengguna: Login/Logout, Peran Pemilik/Kasir (basic).
Pengaturan Toko: Input nama toko.
Backup Data: Backup lokal.
Fitur lain seperti sinkronisasi cloud, kirim struk via WhatsApp/SMS, laporan analisis mendalam, atau fitur pintar lainnya akan dipertimbangkan untuk fase pengembangan selanjutnya.
9. Metrik Keberhasilan
Jumlah unduhan dan aktivasi aplikasi.
Frekuensi penggunaan harian/mingguan.
Rata-rata waktu penyelesaian transaksi.
Feedback positif dari pengguna UMKM.
Akurasi data stok.
10. Asumsi & Keterbatasan
Pengguna memiliki perangkat Android/iOS yang memadai.
Printer thermal yang didukung adalah yang terhubung via Bluetooth (untuk MVP).
Tidak ada integrasi langsung dengan sistem pembayaran pihak ketiga (bank, QRIS provider) di MVP, hanya pencatatan metode pembayaran.
Tidak ada fitur manajemen pelanggan atau utang/piutang di MVP.

---
## Entity-Relationship Diagram (ERD) & Skema Database - Smart Kasir
---
1. Pendahuluan

Skema database ini dirancang untuk mendukung fitur inti aplikasi Smart Kasir, dengan fokus pada pengelolaan produk, transaksi penjualan, dan pengguna. Struktur ini akan menjadi fondasi bagi implementasi database lokal menggunakan Drift.

2. Aturan Relasi (Cardinality)

One-to-Many (1:N): Satu entitas bisa berhubungan dengan banyak entitas lain.

Many-to-One (N:1): Banyak entitas bisa berhubungan dengan satu entitas lain.

One-to-One (1:1): Satu entitas berhubungan dengan tepat satu entitas lain.

3. Entitas (Tabel) Utama dan Atributnya
3.1. Users (Pengguna)

Tujuan: Menyimpan informasi pengguna aplikasi (Pemilik, Kasir).

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

username (TEXT, UNIQUE, NOT NULL)

password_hash (TEXT, NOT NULL) - Disimpan sebagai hash untuk keamanan.

role (TEXT, NOT NULL) - Enum: 'owner', 'cashier'

name (TEXT, NOT NULL)

created_at (INTEGER) - Timestamp

updated_at (INTEGER) - Timestamp

3.2. Products (Produk)

Tujuan: Menyimpan detail setiap produk yang dijual.

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

name (TEXT, UNIQUE, NOT NULL)

barcode (TEXT, UNIQUE, NULL) - Opsional, bisa digunakan untuk pencarian cepat.

purchase_price (REAL, NULL) - Harga beli (opsional untuk perhitungan profit).

selling_price (REAL, NOT NULL)

stock (INTEGER, NOT NULL) - Jumlah stok yang tersedia.

min_stock_alert (INTEGER, DEFAULT 5) - Batas minimum stok untuk peringatan.

category_id (INTEGER, NULL) - FOREIGN KEY ke ProductCategories.

image_path (TEXT, NULL) - Path lokal untuk gambar produk (opsional di MVP).

is_active (BOOLEAN, NOT NULL, DEFAULT TRUE) - Untuk menandai produk aktif/tidak aktif tanpa menghapus.

created_at (INTEGER)

updated_at (INTEGER)

3.3. ProductCategories (Kategori Produk)

Tujuan: Mengelompokkan produk ke dalam kategori.

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

name (TEXT, UNIQUE, NOT NULL)

created_at (INTEGER)

updated_at (INTEGER)

3.4. Transactions (Transaksi)

Tujuan: Menyimpan detail setiap transaksi penjualan yang terjadi.

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

invoice_number (TEXT, UNIQUE, NOT NULL) - Nomor unik untuk setiap transaksi.

transaction_date (INTEGER, NOT NULL) - Timestamp transaksi.

total_amount (REAL, NOT NULL) - Total jumlah yang harus dibayar sebelum diskon.

discount_amount (REAL, DEFAULT 0.0) - Total diskon yang diberikan pada transaksi.

final_amount (REAL, NOT NULL) - Total akhir yang dibayar pelanggan.

payment_method (TEXT, NOT NULL) - Enum: 'cash', 'non_cash'.

cash_paid (REAL, NULL) - Jumlah uang tunai yang diberikan pelanggan (jika metode tunai).

cash_return (REAL, NULL) - Jumlah kembalian (jika metode tunai).

user_id (INTEGER, NOT NULL) - FOREIGN KEY ke Users (kasir yang melakukan transaksi).

created_at (INTEGER)

updated_at (INTEGER)

3.5. TransactionItems (Item Transaksi)

Tujuan: Menyimpan detail setiap produk yang ada dalam suatu transaksi.

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

transaction_id (INTEGER, NOT NULL) - FOREIGN KEY ke Transactions.

product_id (INTEGER, NOT NULL) - FOREIGN KEY ke Products.

quantity (INTEGER, NOT NULL)

price_per_unit (REAL, NOT NULL) - Harga jual produk saat transaksi terjadi (untuk history).

subtotal (REAL, NOT NULL) - quantity * price_per_unit

discount_per_item (REAL, DEFAULT 0.0) - Diskon yang diterapkan pada item spesifik.

final_item_price (REAL, NOT NULL) - Harga akhir item setelah diskon.

created_at (INTEGER)

updated_at (INTEGER)

3.6. StockAdjustments (Penyesuaian Stok)

Tujuan: Mencatat setiap perubahan stok manual (masuk/keluar bukan dari penjualan).

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

product_id (INTEGER, NOT NULL) - FOREIGN KEY ke Products.

adjustment_type (TEXT, NOT NULL) - Enum: 'add', 'remove'.

quantity_changed (INTEGER, NOT NULL) - Jumlah stok yang berubah.

reason (TEXT, NULL) - Alasan penyesuaian (misal: "barang masuk", "rusak", "inventaris").

adjustment_date (INTEGER, NOT NULL) - Timestamp penyesuaian.

user_id (INTEGER, NOT NULL) - FOREIGN KEY ke Users (yang melakukan penyesuaian).

created_at (INTEGER)

updated_at (INTEGER)

3.7. ShopSettings (Pengaturan Toko)

Tujuan: Menyimpan pengaturan umum aplikasi dan informasi toko.

Atribut:

id (PRIMARY KEY, INTEGER, AUTOINCREMENT)

shop_name (TEXT, NOT NULL)

shop_address (TEXT, NULL)

shop_phone (TEXT, NULL)

currency_symbol (TEXT, NOT NULL, DEFAULT 'Rp')

created_at (INTEGER)

updated_at (INTEGER)

Catatan: Ini akan menjadi tabel dengan 1 baris data saja.

4. Entity-Relationship Diagram (ERD) Visualisasi
code
Mermaid
download
content_copy
expand_less
erDiagram
    Users ||--o{ Transactions : "places"
    Users ||--o{ StockAdjustments : "performs"
    ProductCategories ||--o{ Products : "categorizes"
    Products ||--o{ TransactionItems : "included_in"
    Products ||--o{ StockAdjustments : "adjusts"
    Transactions ||--o{ TransactionItems : "contains"

    Users {
        INTEGER id PK
        TEXT username UK
        TEXT password_hash
        TEXT role
        TEXT name
        INTEGER created_at
        INTEGER updated_at
    }

    ProductCategories {
        INTEGER id PK
        TEXT name UK
        INTEGER created_at
        INTEGER updated_at
    }

    Products {
        INTEGER id PK
        TEXT name UK
        TEXT barcode UK "NULL"
        REAL purchase_price "NULL"
        REAL selling_price
        INTEGER stock
        INTEGER min_stock_alert
        INTEGER category_id FK
        TEXT image_path "NULL"
        BOOLEAN is_active
        INTEGER created_at
        INTEGER updated_at
    }

    Transactions {
        INTEGER id PK
        TEXT invoice_number UK
        INTEGER transaction_date
        REAL total_amount
        REAL discount_amount
        REAL final_amount
        TEXT payment_method
        REAL cash_paid "NULL"
        REAL cash_return "NULL"
        INTEGER user_id FK
        INTEGER created_at
        INTEGER updated_at
    }

    TransactionItems {
        INTEGER id PK
        INTEGER transaction_id FK
        INTEGER product_id FK
        INTEGER quantity
        REAL price_per_unit
        REAL subtotal
        REAL discount_per_item
        REAL final_item_price
        INTEGER created_at
        INTEGER updated_at
    }

    StockAdjustments {
        INTEGER id PK
        INTEGER product_id FK
        TEXT adjustment_type
        INTEGER quantity_changed
        TEXT reason "NULL"
        INTEGER adjustment_date
        INTEGER user_id FK
        INTEGER created_at
        INTEGER updated_at
    }

    ShopSettings {
        INTEGER id PK
        TEXT shop_name
        TEXT shop_address "NULL"
        TEXT shop_phone "NULL"
        TEXT currency_symbol
        INTEGER created_at
        INTEGER updated_at
    }

(Gambar di atas adalah representasi textual dari ERD. Saya tidak dapat menghasilkan gambar visual langsung di sini, namun jika Anda ingin saya meminta model gambar untuk menggambarkannya, silakan beritahu saya.)

5. Penjelasan Relasi:

Users - Transactions (1:N): Satu user (kasir) dapat melakukan banyak transaksi. Setiap transaksi dilakukan oleh satu user.

Users - StockAdjustments (1:N): Satu user dapat melakukan banyak penyesuaian stok. Setiap penyesuaian stok dilakukan oleh satu user.

ProductCategories - Products (1:N): Satu kategori dapat memiliki banyak produk. Setiap produk hanya bisa memiliki satu kategori.

Products - TransactionItems (1:N): Satu produk dapat muncul di banyak item transaksi. Setiap item transaksi merujuk ke satu produk.

Products - StockAdjustments (1:N): Satu produk dapat memiliki banyak catatan penyesuaian stok. Setiap penyesuaian stok merujuk ke satu produk.

Transactions - TransactionItems (1:N): Satu transaksi dapat memiliki banyak item transaksi. Setiap item transaksi merujuk ke satu transaksi.

6. Pertimbangan Implementasi dengan Drift:

Setiap entitas di atas akan direpresentasikan sebagai Table dalam Drift.

Kolom created_at dan updated_at akan menggunakan DateTime atau int (untuk timestamp UNIX) di Dart, dan INTEGER di SQLite. Drift mendukung konversi ini.

Kolom BOOLEAN akan disimpan sebagai INTEGER (0 atau 1) di SQLite.

FOREIGN KEY akan didefinisikan secara eksplisit di setiap tabel yang merujuk.

UNIQUE constraint akan diterapkan pada kolom yang tidak boleh memiliki duplikat (misal: username, nama produk, nomor invoice).

---
## Software Requirements Specification (SRS) - Smart Kasir
---
1. Pendahuluan
Dokumen ini merinci persyaratan perangkat lunak untuk aplikasi Smart Kasir, sebuah aplikasi kasir digital yang dirancang untuk UMKM. SRS ini akan menjadi dasar bagi tim pengembangan dan pengujian untuk membangun dan memverifikasi fungsionalitas aplikasi.
1.1. Tujuan
Menyediakan deskripsi lengkap tentang fungsionalitas dan kinerja yang diharapkan dari Smart Kasir.
Sebagai acuan resmi untuk desain, pengembangan, dan pengujian aplikasi.
Memastikan pemahaman yang sama antara semua pemangku kepentingan mengenai ruang lingkup proyek.
1.2. Lingkup Produk
Smart Kasir adalah aplikasi mobile (Android/iOS) yang berfokus pada efisiensi transaksi penjualan, manajemen inventaris dasar, dan pelaporan penjualan. Aplikasi ini dirancang untuk operasional offline-first dengan potensi sinkronisasi data di masa depan.
1.3. Definisi, Akronim, dan Singkatan
UMKM: Usaha Mikro, Kecil, dan Menengah
POS: Point of Sale
PRD: Product Requirements Document
SRS: Software Requirements Specification
UI: User Interface
UX: User Experience
MVP: Minimum Viable Product
Flutter: Framework pengembangan UI lintas platform
Drift: Toolkit persistensi data untuk Dart & Flutter
Riverpod: State management solution untuk Flutter
Freezed: Code generator untuk data class
Go_router: Paket navigasi untuk Flutter
1.4. Referensi
Product Requirements Document (PRD) - Smart Kasir v1.0
Entity-Relationship Diagram (ERD) & Skema Database - Smart Kasir v1.0
2. Deskripsi Umum
2.1. Perspektif Produk
Smart Kasir adalah aplikasi mandiri yang akan berjalan di perangkat mobile. Ini adalah sistem tertutup di fase MVP, yang berarti tidak ada integrasi langsung dengan sistem eksternal (misal: payment gateway, sistem akuntansi pihak ketiga) selain interaksi dengan printer thermal via Bluetooth dan kemampuan berbagi via aplikasi pesan/email.
2.2. Fungsi Produk
Aplikasi akan menyediakan fungsi-fungsi utama sebagai berikut:
Manajemen Pengguna (Login, Logout, Peran)
Manajemen Produk (Tambah, Edit, Hapus, Kategorisasi)
Manajemen Stok (Pengurangan otomatis, Penyesuaian manual, Peringatan stok)
Proses Penjualan (Keranjang belanja, Pembayaran tunai/non-tunai, Perhitungan otomatis)
Pencetakan dan Berbagi Struk
Laporan Penjualan Dasar
Pengaturan Toko
Backup Data Lokal
2.3. Karakteristik Pengguna
Pemilik Usaha: Memiliki akses penuh ke semua fitur. Perlu melihat laporan penjualan, mengelola produk dan staf. Mungkin tidak terlalu teknis, sehingga UI/UX harus intuitif.
Kasir: Akses terbatas hanya untuk transaksi penjualan dan riwayat transaksi mereka. Perlu alur kerja yang sangat cepat dan efisien.
2.4. Batasan Umum
Sistem Operasi: Android (min. Android 7.0), iOS (min. iOS 12.0).
Konektivitas: Offline-first. Koneksi internet hanya diperlukan untuk fitur berbagi struk via email/WhatsApp atau backup cloud (jika diimplementasikan di masa depan).
Perangkat Keras: Membutuhkan printer thermal yang kompatibel dengan Bluetooth untuk pencetakan struk.
Keamanan: Data sensitif (password) akan di-hash. Data transaksi disimpan secara lokal di perangkat.
Skalabilitas: Dirancang untuk UMKM, bukan untuk rantai ritel besar dengan banyak cabang.
Integrasi: Tidak ada integrasi dengan sistem pembayaran eksternal atau sistem akuntansi pihak ketiga di MVP.
3. Persyaratan Fungsional (Functional Requirements)
3.1. FR1: Manajemen Autentikasi & Pengguna
FR1.1 Login Pengguna:
Deskripsi: Sistem harus memungkinkan pengguna (pemilik atau kasir) untuk masuk ke aplikasi menggunakan username dan password yang terdaftar.
Input: Username (TEXT), Password (TEXT).
Output: Sukses login (redirect ke Dashboard), Pesan error (username/password salah).
Prioritas: Tinggi.
FR1.2 Logout Pengguna:
Deskripsi: Sistem harus memungkinkan pengguna untuk keluar dari sesi aplikasi mereka.
Output: Redirect ke halaman Login.
Prioritas: Tinggi.
FR1.3 Manajemen Peran Pengguna:
Deskripsi: Sistem harus memberlakukan peran pengguna untuk membatasi akses ke fitur tertentu.
Peran: 'owner' (akses penuh), 'cashier' (akses terbatas ke POS, Riwayat Transaksi sendiri, tanpa manajemen produk/laporan lengkap).
Prioritas: Tinggi.
FR1.4 Tambah/Edit/Hapus Akun Kasir (Pemilik):
Deskripsi: Pemilik harus dapat menambah, mengedit detail (nama, password), dan menghapus akun kasir.
Input (Tambah): Username, Password, Nama, Peran (default: 'cashier').
Output: Konfirmasi penambahan/edit/hapus, Pesan error (username sudah ada).
Prioritas: Sedang.
3.2. FR2: Manajemen Produk
FR2.1 Tampilan Daftar Produk:
Deskripsi: Sistem harus menampilkan daftar semua produk yang tersedia.
Output: Daftar produk dengan nama, harga jual, stok.
Prioritas: Tinggi.
FR2.2 Pencarian & Filter Produk:
Deskripsi: Sistem harus memungkinkan pencarian produk berdasarkan nama, kode produk, atau kategori.
Input: Keyword pencarian, Filter kategori.
Prioritas: Tinggi.
FR2.3 Tambah Produk:
Deskripsi: Sistem harus memungkinkan pemilik untuk menambahkan produk baru.
Input: Nama Produk (UNIQUE, NOT NULL), Barcode (UNIQUE, NULL), Harga Beli (NULL), Harga Jual (NOT NULL), Stok Awal (NOT NULL), Kategori (NULL), Stok Minimum Peringatan (DEFAULT 5).
Output: Konfirmasi penambahan, Pesan error (nama/barcode duplikat).
Prioritas: Tinggi.
FR2.4 Edit Produk:
Deskripsi: Sistem harus memungkinkan pemilik untuk mengedit detail produk yang sudah ada.
Input: Semua atribut produk kecuali ID.
Output: Konfirmasi perubahan, Pesan error (nama/barcode duplikat).
Prioritas: Tinggi.
FR2.5 Hapus Produk:
Deskripsi: Sistem harus memungkinkan pemilik untuk menghapus produk (secara soft delete, yaitu mengubah is_active menjadi FALSE)
Output: Konfirmasi penghapusan, Produk tidak muncul di daftar aktif.
Prioritas: Sedang.
FR2.6 Manajemen Kategori Produk:
Deskripsi: Sistem harus memungkinkan pemilik untuk menambah, mengedit, dan menghapus kategori produk.
Input: Nama Kategori (UNIQUE, NOT NULL).
Prioritas: Sedang.
3.3. FR3: Manajemen Stok
FR3.1 Pengurangan Stok Otomatis:
Deskripsi: Stok produk harus otomatis berkurang sesuai kuantitas yang terjual setelah transaksi berhasil.
Pemicu: Transaksi selesai.
Prioritas: Tinggi.
FR3.2 Penyesuaian Stok Manual:
Deskripsi: Pemilik harus dapat menambah atau mengurangi stok produk secara manual.
Input: Produk, Jumlah Perubahan Stok, Jenis (Tambah/Kurang), Alasan.
Prioritas: Sedang.
FR3.3 Peringatan Stok Menipis:
Deskripsi: Sistem harus memberikan notifikasi visual (di UI, misal icon) ketika stok produk mencapai atau di bawah batas minimum yang ditentukan.
Prioritas: Tinggi.
3.4. FR4: Proses Penjualan (POS)
FR4.1 Tambah Produk ke Keranjang:
Deskripsi: Pengguna (kasir) dapat menambahkan produk ke keranjang belanja.
Input: Pilih produk dari daftar atau scan barcode (jika diimplementasikan).
Output: Produk muncul di keranjang.
Prioritas: Tinggi.
FR4.2 Edit & Hapus Item Keranjang:
Deskripsi: Pengguna dapat menyesuaikan kuantitas produk di keranjang atau menghapus item.
Prioritas: Tinggi.
FR4.3 Perhitungan Transaksi Otomatis:
Deskripsi: Sistem harus secara otomatis menghitung subtotal, total diskon, dan total akhir.
Prioritas: Tinggi.
FR4.4 Pembayaran Transaksi:
Deskripsi: Sistem harus memproses pembayaran transaksi.
Input: Metode pembayaran (Tunai/Non-Tunai), Jumlah uang tunai (jika Tunai).
Output: Perhitungan kembalian (jika Tunai), Penyimpanan transaksi.
Prioritas: Tinggi.
FR4.5 Terapkan Diskon Transaksi:
Deskripsi: Pengguna dapat menerapkan diskon ke seluruh transaksi (persen atau nominal).
Prioritas: Tinggi.
3.5. FR5: Laporan & Analisis Dasar
FR5.1 Laporan Penjualan (Ringkasan):
Deskripsi: Sistem harus menampilkan ringkasan penjualan (omset, transaksi, diskon, penjualan bersih) untuk periode tertentu.
Input: Filter tanggal (harian, mingguan, bulanan, kustom).
Prioritas: Tinggi.
FR5.2 Laporan Produk Terlaris:
Deskripsi: Sistem harus menampilkan daftar produk terlaris berdasarkan kuantitas atau omset.
Prioritas: Sedang.
FR5.3 Ekspor Laporan:
Deskripsi: Sistem harus memungkinkan ekspor laporan penjualan ke format PDF dan Excel.
Prioritas: Sedang.
3.6. FR6: Cetak & Berbagi Struk
FR6.1 Cetak Struk via Printer Thermal:
Deskripsi: Sistem harus dapat mencetak struk transaksi ke printer thermal via Bluetooth.
Output: Struk fisik tercetak.
Prioritas: Tinggi.
FR6.2 Bagikan Struk Digital:
Deskripsi: Sistem harus memungkinkan berbagi struk transaksi (format teks sederhana atau PDF) via WhatsApp atau SMS.
Prioritas: Sedang.
3.7. FR7: Pengaturan Toko
FR7.1 Edit Informasi Toko:
Deskripsi: Pemilik dapat mengedit informasi dasar toko (nama, alamat, telepon).
Prioritas: Sedang.
FR7.2 Pengaturan Mata Uang:
Deskripsi: Pemilik dapat mengatur simbol mata uang default.
Prioritas: Sedang.
3.8. FR8: Manajemen Data
FR8.1 Backup Data Lokal:
Deskripsi: Sistem harus memungkinkan pemilik untuk membuat cadangan database lokal.
Prioritas: Tinggi.
FR8.2 Restore Data Lokal:
Deskripsi: Sistem harus memungkinkan pemilik untuk mengembalikan database dari file cadangan lokal.
Prioritas: Tinggi.
4. Persyaratan Non-Fungsional (Non-Functional Requirements)
4.1. Performa
NFR1.1 Waktu Respons: Setiap aksi pengguna (misal: tambah produk ke keranjang, selesaikan transaksi) harus memiliki waktu respons kurang dari 1 detik.
NFR1.2 Kecepatan Pencarian: Pencarian produk harus menampilkan hasil dalam waktu kurang dari 500ms untuk database hingga 1000 produk.
4.2. Keamanan
NFR2.1 Autentikasi: Password pengguna harus disimpan dalam bentuk hash.
NFR2.2 Otorisasi: Akses fitur harus dikontrol berdasarkan peran pengguna.
NFR2.3 Keamanan Data Lokal: Data database lokal harus terlindungi dari akses tidak sah oleh aplikasi lain.
4.3. Usability (Kemudahan Penggunaan)
NFR3.1 Antarmuka Intuitif: UI harus mudah dipahami dan digunakan oleh kasir dengan pelatihan minimal.
NFR3.2 Minimal Ketukan: Alur transaksi harus dirancang untuk meminimalkan jumlah ketukan/interaksi yang diperlukan.
NFR3.3 Konsistensi UI: Elemen UI dan alur navigasi harus konsisten di seluruh aplikasi.
4.4. Reliabilitas
NFR4.1 Stabilitas: Aplikasi harus stabil dan tidak mengalami crash secara tidak terduga dalam penggunaan normal.
NFR4.2 Penanganan Error: Aplikasi harus menangani error secara gracefully dan memberikan pesan yang informatif kepada pengguna.
NFR4.3 Konsistensi Data: Data transaksi dan stok harus selalu konsisten dan akurat.
4.5. Portabilitas
NFR5.1 Lintas Platform: Aplikasi harus dapat berjalan dengan baik di perangkat Android dan iOS.
4.6. Maintainability (Kemudahan Pemeliharaan)
NFR6.1 Kode Bersih: Kode sumber harus mengikuti prinsip Clean Code dan pola desain yang telah ditetapkan.
NFR6.2 Dokumentasi: Kode yang kompleks harus didokumentasikan dengan baik.
4.7. Skalabilitas (Internal)
NFR7.1 Ukuran Database: Aplikasi harus dapat menangani hingga 10.000 produk dan 100.000 transaksi tanpa penurunan performa signifikan.
5. Lingkungan Implementasi
5.1. Lingkungan Pengembangan
IDE: Visual Studio Code / Android Studio
SDK: Flutter SDK [Versi Spesifik]
Bahasa: Dart
Manajemen Paket: pub.dev
5.2. Komponen Teknis Utama
UI Framework: Flutter
State Management: Riverpod Generator
Data Models: Freezed
Navigasi: Go_router
Local Database: Drift (SQLite)
Error Handling: fpdart (opsional)
Logging: logger
6. Desain Antarmuka Pengguna (UI Wireframe/Mockup - Jika Tersedia)
(Bagian ini akan diisi dengan wireframe, mockup, atau screenshot desain jika sudah dibuat. Untuk saat ini, kita bisa mendeskripsikan secara tekstual.)
Halaman Login: Input Username, Password, Tombol Login.
Dashboard Kasir: Daftar Produk (grid/list), Search bar, Keranjang Belanja (di sisi kanan/drawer), Total, Tombol Pembayaran.
Halaman Manajemen Produk: Daftar Produk, Tombol Tambah Produk, Tombol Edit/Hapus (per item).
Form Tambah/Edit Produk: Field input untuk detail produk.
Halaman Laporan: Filter tanggal, Ringkasan angka, Grafik sederhana, Tombol Ekspor.

---
## Software Design Document (SDD) - Smart Kasir
---

1. Pendahuluan
Dokumen ini menjelaskan desain arsitektur dan komponen perangkat lunak untuk aplikasi Smart Kasir. Desain ini disusun berdasarkan persyaratan fungsional dan non-fungsional yang telah didefinisikan dalam dokumen PRD dan SRS. Tujuan utama dokumen ini adalah untuk menyediakan panduan yang jelas bagi tim pengembangan, memastikan konsistensi dalam implementasi, dan memfasilitasi pemeliharaan serta pengembangan di masa mendatang.
1.1. Tujuan
Menyediakan gambaran arsitektur sistem secara keseluruhan.
Merinci desain komponen-komponen utama aplikasi.
Menjelaskan bagaimana persyaratan dari SRS akan dipenuhi melalui desain.
Menjadi referensi utama bagi pengembang selama tahap implementasi.
1.2. Lingkup
Dokumen ini mencakup desain arsitektur, struktur modul, desain data (bagaimana entitas diwakili dalam kode), dan desain antarmuka utama. Desain ini berfokus pada fase MVP dari Smart Kasir.
1.3. Definisi, Akronim, dan Singkatan
SDD: Software Design Document
PRD: Product Requirements Document
SRS: Software Requirements Specification
ERD: Entity-Relationship Diagram
Clean Architecture: Pola desain yang memisahkan kode menjadi lapisan-lapisan.
Bloc: Business Logic Component (sering digunakan di Flutter)
Provider: State management solution (Riverpod adalah salah satu implementasinya)
DTO: Data Transfer Object
DAO: Data Access Object
Usecase: Business logic (interactor)
1.4. Referensi
Product Requirements Document (PRD) - Smart Kasir v1.0
Software Requirements Specification (SRS) - Smart Kasir v1.0
Entity-Relationship Diagram (ERD) & Skema Database - Smart Kasir v1.0
2. Desain Arsitektur Sistem
Aplikasi Smart Kasir akan mengadopsi prinsip Clean Architecture yang disesuaikan untuk aplikasi Flutter, memanfaatkan Riverpod sebagai state management utama. Pendekatan ini mempromosikan pemisahan concern (separation of concerns), testability, dan fleksibilitas.
2.1. Lapisan Arsitektur
Aplikasi akan dibagi menjadi empat lapisan utama:
Presentation Layer (UI & State Management):
Tujuan: Menampilkan antarmuka pengguna dan mengelola interaksi pengguna.
Komponen: Widgets (UI), Pages/Screens, Providers (dari Riverpod) yang mengelola UI state dan berinteraksi dengan Domain Layer (melalui Usecases).
Dependencies: Tergantung pada Domain Layer.
Teknologi: Flutter Widgets, Riverpod.
Domain Layer (Business Logic Core):
Tujuan: Berisi aturan bisnis inti dan entitas aplikasi. Ini adalah lapisan yang paling independen.
Komponen:
Entities: Kelas-kelas data murni yang merepresentasikan konsep bisnis (misal: Product, Transaction, User). Dibuat immutable menggunakan Freezed.
Repositories (Abstract): Kontrak/interface yang mendefinisikan operasi data yang dapat dilakukan oleh Domain Layer.
Use Cases (Interactors): Logika bisnis spesifik yang mengorkestrasi operasi dari satu atau lebih Repository untuk menyelesaikan tugas bisnis.
Dependencies: Tidak tergantung pada lapisan lain.
Teknologi: Freezed, Dart.
Data Layer (Implementasi Data):
Tujuan: Bertanggung jawab untuk mengambil, menyimpan, dan mengelola data dari berbagai sumber (lokal database, API, dll.).
Komponen:
Data Sources: Implementasi konkret untuk mengambil/menyimpan data (misal: DriftDatasource, RemoteApiDatasource - jika ada).
Models (DTOs): Kelas-kelas data yang merepresentasikan struktur data dari sumber data (misal: tabel database Drift). Dibuat immutable menggunakan Freezed.
Repositories (Concrete Implementations): Implementasi konkret dari interface Repository yang didefinisikan di Domain Layer. Mereka berinteraksi dengan Data Sources dan melakukan pemetaan antara Models dan Entities.
Dependencies: Tergantung pada Domain Layer (karena mengimplementasikan interface Repository-nya).
Teknologi: Drift, Freezed, Dart.
Common/Core Layer:
Tujuan: Menyediakan utilitas, konstanta, penanganan error, dan ekstensi yang digunakan di seluruh lapisan.
Komponen: Logger, Either (dari fpdart untuk error handling), AppConstants, Result (custom type untuk operasi data).
Dependencies: Tidak tergantung pada lapisan bisnis, tetapi lapisan lain bisa bergantung padanya.
Teknologi: fpdart, logger, Dart.
2.2. Diagram Arsitektur (Konseptual)
code
Code
+---------------------+      +---------------------+      +---------------------+
|                     |      |                     |      |                     |
|  PRESENTATION LAYER |      |    DOMAIN LAYER     |      |     DATA LAYER      |
|  (Flutter Widgets)  |      |  (Business Logic)   |      | (Data Persistence)  |
|                     |      |                     |      |                     |
|  - Pages/Screens    | <==> |  - Use Cases        | <==> |  - Repository Impl. |
|  - Riverpod Providers|      |  - Entities (Freezed)|      |  - Data Sources     |
|  - UI State         |      |  - Repository Abs.  |      |  - Models (Freezed) |
+---------------------+      +---------------------+      +---------------------+
           ^                                 ^
           |                                 |
           |           COMMON / CORE LAYER           |
           | (Utils, Error Handling, Constants)      |
           +-----------------------------------------+
3. Desain Komponen Tingkat Tinggi
3.1. Struktur Proyek (lib folder)
code
Code
lib/
├── core/
│   ├── constants/       (AppConstants.dart)
│   ├── errors/          (Failure.dart, error_handler.dart)
│   ├── usecases/        (base_usecase.dart)
│   └── utils/           (logger_util.dart, extension_methods.dart)
├── features/
│   ├── auth/              (Login, Register, User Management)
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   ├── models/
│   │   │   └── repositories/
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   ├── repositories/
│   │   │   └── usecases/
│   │   └── presentation/
│   │       ├── providers/
│   │       ├── pages/
│   │       └── widgets/
│   ├── product/           (Product Management, Categories, Stock)
│   │   ├── data/ ...
│   │   ├── domain/ ...
│   │   └── presentation/ ...
│   ├── pos/               (Point of Sale, Transaction Processing)
│   │   ├── data/ ...
│   │   ├── domain/ ...
│   │   └── presentation/ ...
│   ├── reports/           (Sales Reports, Analytics)
│   │   ├── data/ ...
│   │   ├── domain/ ...
│   │   └── presentation/ ...
│   └── settings/          (Shop Settings, Backup/Restore)
│       ├── data/ ...
│       ├── domain/ ...
│       └── presentation/ ...
├── router/                (go_router_config.dart)
├── shared/                (Reusable widgets, components across features)
│   ├── widgets/
│   ├── styles/
│   └── themes/
└── main.dart
3.2. Go_router Configuration
go_router_config.dart: Akan berisi semua definisi route aplikasi, termasuk nested routes dan redirect berdasarkan status autentikasi.
Named Routes: Semua route akan menggunakan named routes untuk kemudahan navigasi dan pemeliharaan.
/login
/dashboard
/products
/products/add
/products/:id/edit
/transactions
/reports
/settings
3.3. Database Design (Drift)
Database akan diimplementasikan menggunakan Drift (SQLite).
Setiap entitas dari ERD (Users, Products, Transactions, TransactionItems, etc.) akan memiliki representasi sebagai Table dalam file .drift atau file Dart yang diperluas dari Table.
Database Class: Sebuah AppDatabase class akan meng-extend _$AppDatabase dan mengelola semua koneksi dan DAO.
DAO (Data Access Objects): Untuk setiap tabel atau grup tabel terkait, akan ada DAO (misal: UsersDao, ProductsDao). DAO ini akan menyediakan metode CRUD (Create, Read, Update, Delete) dan query kustom lainnya untuk mengakses data.
Contoh: ProductsDao akan memiliki getProducts(), insertProduct(), updateProduct(), deleteProduct().
3.4. State Management (Riverpod)
_Providers.g.dart: Riverpod Generator akan digunakan untuk menghasilkan provider secara otomatis.
Per-Feature Providers: Setiap fitur akan memiliki set provider-nya sendiri untuk mengelola state UI dan data.
Notifier Providers (AsyncNotifier/Notifier): Digunakan untuk state yang kompleks dan berubah. Misalnya, ProductListNotifier untuk mengelola daftar produk yang ditampilkan, CartNotifier untuk mengelola item di keranjang.
Future Providers / Stream Providers: Digunakan untuk mengambil data asinkron satu kali atau stream data dari repository.
Provider: Untuk dependensi (misal: productRepositoryProvider).
Dependency Injection: Riverpod akan digunakan sebagai alat Dependency Injection untuk menyediakan instance Repository dan Use Case ke Presentation Layer.
4. Desain Modul & Komponen Tingkat Rendah
4.1. Modul Autentikasi (auth feature)
Entities: User (dari Freezed).
Use Cases:
LoginUserUseCase(username, password): Mengotentikasi user.
CreateUserUseCase(user): Menambah user baru (kasir).
UpdateUserUseCase(user): Memperbarui detail user.
DeleteUserUseCase(userId): Menghapus user.
GetCurrentUserUseCase(): Mengambil user yang sedang login.
Repositories (Abstract): AuthRepository.
Data Sources: LocalAuthDataSource (menyimpan user di Drift).
Models: UserDbModel (dari Freezed, representasi tabel Drift Users).
Providers: authNotifierProvider (mengelola state login), userListProvider.
4.2. Modul Produk (product feature)
Entities: Product, ProductCategory.
Use Cases:
GetProductsUseCase(): Mengambil daftar produk.
GetProductByIdUseCase(id): Mengambil detail produk.
AddProductUseCase(product): Menambah produk.
UpdateProductUseCase(product): Mengupdate produk.
DeleteProductUseCase(id): Menghapus produk.
UpdateStockUseCase(productId, quantity, type): Menyesuaikan stok.
GetProductCategoriesUseCase(): Mengambil kategori produk.
AddProductCategoryUseCase(category): Menambah kategori.
Repositories (Abstract): ProductRepository.
Data Sources: DriftProductDataSource.
Models: ProductDbModel, ProductCategoryDbModel.
Providers: productListNotifier, productDetailProvider, categoryListProvider.
4.3. Modul POS (pos feature)
Entities: Transaction, TransactionItem, Cart.
Use Cases:
ProcessSaleUseCase(cart, paymentDetails): Memproses transaksi penjualan.
GetTransactionsUseCase(dateFilter): Mengambil daftar transaksi.
GetTransactionDetailUseCase(id): Mengambil detail transaksi.
Repositories (Abstract): TransactionRepository.
Data Sources: DriftTransactionDataSource.
Models: TransactionDbModel, TransactionItemDbModel.
Providers: cartNotifier (mengelola keranjang belanja), transactionListProvider.
4.4. Modul Laporan (reports feature)
Entities: SalesSummary, BestSellingProduct.
Use Cases:
GetSalesReportUseCase(startDate, endDate): Mengambil laporan ringkasan penjualan.
GetBestSellingProductsUseCase(startDate, endDate): Mengambil produk terlaris.
Repositories (Abstract): ReportRepository (mungkin menggunakan TransactionRepository dan ProductRepository secara internal).
Data Sources: Tidak ada Data Source terpisah, data diambil dari DAO yang ada.
Models: Output bisa langsung berupa Entities atau DTO khusus laporan.
Providers: salesReportProvider, bestSellingProductsProvider.
4.5. Modul Pengaturan (settings feature)
Entities: ShopSetting.
Use Cases:
GetShopSettingsUseCase(): Mengambil pengaturan toko.
UpdateShopSettingsUseCase(settings): Mengupdate pengaturan toko.
BackupDatabaseUseCase(): Melakukan backup database.
RestoreDatabaseUseCase(filePath): Melakukan restore database.
Repositories (Abstract): SettingsRepository.
Data Sources: DriftSettingsDataSource.
Models: ShopSettingDbModel.
Providers: shopSettingsNotifier.
5. Desain Antarmuka Pengguna (UI)
Komponen Umum: Akan menggunakan widget Flutter standar dan custom widget di shared/widgets.
Theming: Akan ada file theme.dart di shared/themes untuk mendefinisikan warna, tipografi, dan bentuk.
Halaman Login: Desain minimalis, input field, tombol login.
Halaman Dashboard/POS:
Bagian utama untuk menampilkan produk (menggunakan GridView atau ListView).
Search bar di bagian atas.
Bagian keranjang belanja (di samping atau sebagai bottom sheet/drawer) dengan item, kuantitas, subtotal, total.
Tombol "Bayar" yang jelas.
Halaman Manajemen Produk: Daftar produk (ListView.builder) dengan opsi edit/hapus (Slidable widget atau icon).
Form Input: Akan menggunakan TextFormField dengan validasi yang jelas.
6. Desain Penanganan Error
fpdart's Either Type: Digunakan di Domain dan Data Layer untuk merepresentasikan hasil operasi yang bisa sukses (Right) atau gagal (Left).
Failure Class: Sebuah hierarchy Failure class (misal: ServerFailure, CacheFailure, InputValidationFailure) akan didefinisikan di core/errors untuk standar error handling.
Presentation Layer: Akan menangani Failure yang diterima dari Usecases dan menampilkan pesan error yang sesuai kepada pengguna (misal: SnackBar, AlertDialog).
7. Desain Keamanan
Password Hashing: password_hash akan disimpan menggunakan algoritma hashing yang kuat (misal: Argon2, bcrypt) melalui sebuah paket Dart yang sesuai.
Akses Lokal: Database SQLite akan dilindungi oleh sistem file OS.
8. Backup & Restore Data
Backup: Akan menyalin file database SQLite (app_database.sqlite) ke lokasi yang ditentukan oleh pengguna (misal: direktori unduhan) atau direktori internal aplikasi.
Restore: Akan menimpa file database saat ini dengan file backup yang dipilih. Peringatan akan diberikan kepada pengguna.

---
Checklist Timeline Pekerjaan Sprint - Smart Kasir MVP
---
Durasi Sprint: 2 Minggu per Sprint (Total 4 Sprints = 8 Minggu)
Target MVP: Aplikasi kasir fungsional dengan manajemen produk dasar, transaksi penjualan, laporan sederhana, autentikasi user, dan backup lokal.
Sprint 1: Fondasi & Autentikasi (Minggu 1-2)
Tujuan Sprint: Menyiapkan arsitektur dasar, database lokal, dan modul autentikasi fungsional.
Backend/Data Layer:

Inisialisasi proyek Flutter.

Konfigurasi Drift:

Buat AppDatabase class.

Definisikan Users table (users.drift).

Definisikan ShopSettings table (shop_settings.drift).

Buat UsersDao untuk operasi CRUD user.

Buat ShopSettingsDao.

Konfigurasi Riverpod Generator.

Konfigurasi Go_router (base routes: /login, /dashboard).

Konfigurasi Freezed untuk User entity dan UserDbModel.

Implementasi core/errors (Failure classes).

Implementasi core/usecases/base_usecase.dart.

Implementasi AuthRepository (abstract & concrete).

Implementasi LocalAuthDataSource.

Implementasi LoginUserUseCase.

Implementasi CreateUserUseCase (untuk pemilik awal/pendaftaran pertama).

Implementasi UpdateShopSettingsUseCase (untuk setup awal nama toko).

Paket keamanan password (misal argon2_flutter atau bcrypt).
Frontend/Presentation Layer:

Desain UI Halaman Login.

Implementasi UI Halaman Login.

Integrasi LoginUserUseCase dengan UI Login menggunakan Riverpod.

Desain UI Halaman Pengaturan Toko awal (untuk input nama toko).

Implementasi UI Halaman Pengaturan Toko.

Integrasi UpdateShopSettingsUseCase dengan UI.

Implementasi navigasi dasar dengan Go_router (dari Login ke Pengaturan Toko/Dashboard).

Implementasi placeholder Dashboard kosong (setelah login).
Testing:

Unit test untuk LoginUserUseCase.

Unit test untuk AuthRepository (implementasi).

Unit test untuk UsersDao.

Widget test untuk Halaman Login.
Sprint 2: Manajemen Produk & Stok Dasar (Minggu 3-4)
Tujuan Sprint: Mengimplementasikan fitur manajemen produk dan stok dasar.
Backend/Data Layer:

Definisikan ProductCategories table (product_categories.drift).

Definisikan Products table (products.drift).

Buat ProductCategoriesDao dan ProductsDao.

Konfigurasi Freezed untuk Product dan ProductCategory entities/models.

Implementasi ProductRepository (abstract & concrete).

Implementasi LocalProductDataSource.

Implementasi AddProductUseCase.

Implementasi GetProductsUseCase.

Implementasi UpdateProductUseCase.

Implementasi DeleteProductUseCase (soft delete).

Implementasi UpdateStockUseCase (manual adjustment).

Implementasi GetProductCategoriesUseCase.

Implementasi AddProductCategoryUseCase.
Frontend/Presentation Layer:

Desain UI Halaman Daftar Produk (dengan search bar dan filter kategori).

Implementasi UI Halaman Daftar Produk.

Integrasi GetProductsUseCase dengan UI.

Desain UI Halaman Tambah/Edit Produk.

Implementasi UI Halaman Tambah/Edit Produk.

Integrasi AddProductUseCase dan UpdateProductUseCase dengan UI.

Implementasi UI Peringatan Stok Menipis (misal: ikon di daftar produk).

Navigasi Go_router untuk fitur produk.
Testing:

Unit test untuk ProductRepository.

Unit test untuk ProductsDao dan ProductCategoriesDao.

Unit test untuk AddProductUseCase, GetProductsUseCase, UpdateStockUseCase.

Widget test untuk Halaman Daftar Produk.
Sprint 3: Proses Penjualan (POS) & Riwayat Transaksi (Minggu 5-6)
Tujuan Sprint: Membangun inti sistem POS dan kemampuan mencatat transaksi.
Backend/Data Layer:

Definisikan Transactions table (transactions.drift).

Definisikan TransactionItems table (transaction_items.drift).

Buat TransactionsDao dan TransactionItemsDao.

Konfigurasi Freezed untuk Transaction, TransactionItem entities/models.

Implementasi TransactionRepository (abstract & concrete).

Implementasi LocalTransactionDataSource.

Implementasi ProcessSaleUseCase (mengelola keranjang, menyimpan transaksi, mengurangi stok).

Implementasi GetTransactionsUseCase (filter tanggal sederhana).

Implementasi GetTransactionDetailUseCase.
Frontend/Presentation Layer:

Desain UI Halaman POS:

Bagian daftar produk untuk dipilih.

Bagian keranjang belanja (menampilkan item, kuantitas, subtotal).

Perhitungan total, diskon, kembalian.

Input metode pembayaran (tunai/non-tunai).

Tombol "Bayar".

Implementasi UI Halaman POS.

Integrasi ProcessSaleUseCase dengan UI.

Implementasi CartNotifier dengan Riverpod untuk mengelola keranjang belanja.

Desain UI Halaman Riwayat Transaksi.

Implementasi UI Halaman Riwayat Transaksi.

Integrasi GetTransactionsUseCase dan GetTransactionDetailUseCase dengan UI.

Navigasi Go_router untuk fitur POS dan transaksi.
Testing:

Unit test untuk TransactionRepository.

Unit test untuk TransactionsDao dan TransactionItemsDao.

Unit test untuk ProcessSaleUseCase.

Widget test untuk Halaman POS.
Sprint 4: Laporan Dasar, Struk, Backup & Finalisasi MVP (Minggu 7-8)
Tujuan Sprint: Menyelesaikan fitur-fitur penting untuk MVP, termasuk laporan, cetak struk, backup, dan persiapan rilis.
Backend/Data Layer:

Implementasi ReportRepository (menggunakan DAO dari Transactions dan Products).

Implementasi GetSalesReportUseCase (ringkasan omset harian/bulanan).

Implementasi GetBestSellingProductsUseCase.

Implementasi BackupDatabaseUseCase.

Implementasi RestoreDatabaseUseCase.
Frontend/Presentation Layer:

Desain UI Halaman Laporan Penjualan (ringkasan angka, daftar produk terlaris).

Implementasi UI Halaman Laporan Penjualan.

Integrasi GetSalesReportUseCase dan GetBestSellingProductsUseCase.

Integrasi fitur cetak struk via Bluetooth (menggunakan paket Flutter yang relevan).

Integrasi fitur berbagi struk via aplikasi lain (WhatsApp/SMS - menggunakan share_plus atau custom intent).

Desain UI Halaman Backup/Restore.

Implementasi UI Halaman Backup/Restore.

Integrasi BackupDatabaseUseCase dan RestoreDatabaseUseCase.

Finalisasi navigasi Go_router.
Testing & Deployment:

Unit test untuk ReportRepository.

Unit test untuk BackupDatabaseUseCase dan RestoreDatabaseUseCase.

Integrasi test end-to-end untuk alur utama (login -> transaksi -> laporan).

Review Kode Lengkap & Refactoring: Pastikan mengikuti Clean Architecture dan praktik terbaik.

Pengujian UI/UX: Pastikan aplikasi responsif, intuitif, dan bebas bug.

Pengujian Performa: Cek waktu respons dan penggunaan sumber daya.

Pengujian Kompatibilitas: Coba di berbagai perangkat Android/iOS (jika ada).

Persiapan Rilis: Icon aplikasi, splash screen, informasi toko default.

Build Rilis: Android APK/AppBundle, iOS TestFlight build.
Catatan Penting:
Fleksibilitas: Timeline ini adalah estimasi. Selalu siap untuk menyesuaikan lingkup atau durasi sprint berdasarkan temuan selama pengembangan.
Buffer: Pertimbangkan untuk menyertakan sedikit waktu "buffer" di setiap sprint untuk hal-hal tak terduga (bug, perubahan kecil, dll.).
Komunikasi: Komunikasi rutin dalam tim sangat penting untuk melacak kemajuan dan mengatasi hambatan.
Fitur "Smart": Fitur analisis yang lebih mendalam (jam ramai, grafik lebih kompleks) bisa menjadi target di iterasi selanjutnya setelah MVP stabil.

✍️ **Dibuat oleh:**  
Kelompok FinNote – Rifqy Niam Fadhil (1241) & Muhammad Ariyanto (1281)  
