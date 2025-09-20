# 04_SDD_Software_Design_Document – FinNote
**Kelompok:**  
- Rifqy Niam Fadhil (1241)  
- Muhammad Ariyanto (1281)  

---

## 1. Pendahuluan
Dokumen ini menjelaskan desain perangkat lunak untuk aplikasi **FinNote**, mencakup arsitektur sistem, komponen utama, interaksi antar modul, serta desain database. Tujuannya adalah memastikan tim pengembang memiliki panduan teknis yang jelas dan konsisten.

---

## 2. Desain Arsitektur Sistem

### 2.1 Pola Arsitektur
- **Clean Architecture (3 Layered)**
  - **Presentation Layer (UI/UX):** Flutter + Riverpod
  - **Domain Layer:** Business logic, Entities, Use Cases
  - **Data Layer:** Repository, SQLite/Drift sebagai database lokal

### 2.2 Diagram Arsitektur (Konseptual)
[ UI (Flutter Widgets) ]
↓
[ Use Cases / Domain Logic ]
↓
[ Repository Interface ]
↓
[ Repository Implementation ]
↓
[ SQLite Database (Drift/Hive) ]

---

## 3. Komponen Perangkat Lunak

### 3.1 Presentation Layer
- **UI Components:** Dashboard, Transaksi List, Form Transaksi, Kategori
- **State Management:** Riverpod (provider + notifier)
- **Routing:** GoRouter untuk navigasi antar halaman

### 3.2 Domain Layer
- **Entities:**
  - Transaksi (id, jumlah, deskripsi, tanggal, kategoriId, tipe)
  - Kategori (id, nama, tipe: pemasukan/pengeluaran)
- **Use Cases:**
  - TambahTransaksi
  - HapusTransaksi
  - HitungSaldo
  - GenerateLaporanBulanan

### 3.3 Data Layer
- **Repositories:**
  - TransaksiRepository
  - KategoriRepository
- **Database:** SQLite (pakai Drift/Hive)
- **Logging:** Logger untuk debugging

---

## 4. Desain Database

### 4.1 Skema Tabel
**Tabel: Transaksi**
- id (INTEGER, PK, Auto Increment)
- jumlah (REAL, NOT NULL)
- deskripsi (TEXT, opsional)
- tanggal (DATETIME, NOT NULL)
- tipe (TEXT: ‘pemasukan’ | ‘pengeluaran’)
- kategoriId (INTEGER, FK → Kategori.id)

**Tabel: Kategori**
- id (INTEGER, PK, Auto Increment)
- nama (TEXT, unik)
- tipe (TEXT: ‘pemasukan’ | ‘pengeluaran’)

### 4.2 Hubungan
- One-to-Many: **Kategori → Transaksi**  
  (Satu kategori bisa digunakan oleh banyak transaksi)

---

## 5. Interaksi Antar Modul
1. Pengguna input transaksi melalui UI.  
2. UI memanggil **Use Case** di Domain Layer.  
3. Use Case memanggil **Repository Interface**.  
4. Repository Implementation mengakses database SQLite.  
5. Hasil dikembalikan ke UI untuk ditampilkan.  

---

## 6. Non-Fungsional
- **Responsif:** UI harus stabil pada berbagai ukuran layar.  
- **Keamanan:** Data hanya tersimpan lokal, tanpa akun.  
- **Pemeliharaan:** Kode mengikuti prinsip Clean Code (SOLID).  

---
