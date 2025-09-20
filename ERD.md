# Entity Relationship Diagram (ERD) - FinNote 

---

## Gambaran Umum
ERD ini menggambarkan struktur database relasional untuk aplikasi **FinNote**, yaitu aplikasi pencatatan keuangan pribadi.  
Fokus utama pada entitas: **Categories**, **Transactions**, dan **Budgets**, serta hubungan antar entitasnya.  
Pada MVP awal, aplikasi tidak memerlukan entitas **Users** karena data disimpan secara lokal.  

---

## Entitas dan Atribut

### Categories
- `id` (INTEGER, PK, AUTOINCREMENT) → Primary key kategori.  
- `name` (TEXT, NOT NULL) → Nama kategori transaksi (misal: Makanan, Transportasi).  
- `type` (TEXT, NOT NULL) → Jenis kategori (`income` atau `expense`).  
- `color` (TEXT, NULLABLE) → Warna kategori (misal hex code `#RRGGBB`).  

### Transactions
- `id` (INTEGER, PK, AUTOINCREMENT) → Primary key transaksi.  
- `title` (TEXT, NOT NULL) → Judul atau nama transaksi.  
- `amount` (REAL, NOT NULL) → Nominal transaksi.  
- `date` (INTEGER, NOT NULL) → Tanggal transaksi (Unix timestamp).  
- `note` (TEXT, NULLABLE) → Catatan tambahan.  
- `category_id` (INTEGER, FK → Categories.id, NULLABLE).  
- `created_at` (INTEGER, NOT NULL) → Waktu transaksi dicatat.  
- `updated_at` (INTEGER, NOT NULL) → Waktu transaksi terakhir diperbarui.  

### Budgets
- `id` (INTEGER, PK, AUTOINCREMENT) → Primary key anggaran.  
- `category_id` (INTEGER, FK → Categories.id, NOT NULL).  
- `amount_limit` (REAL, NOT NULL) → Batas maksimal anggaran kategori.  
- `start_date` (INTEGER, NOT NULL) → Tanggal mulai periode anggaran.  
- `end_date` (INTEGER, NOT NULL) → Tanggal akhir periode anggaran.  

---

## Hubungan Antar Entitas
1. **Categories (1) → (Many) Transactions**  
   - Satu kategori bisa dipakai untuk banyak transaksi.  
   - Jika kategori dihapus, `category_id` pada transaksi diset `NULL`.  

2. **Categories (1) → (Many) Budgets**  
   - Satu kategori dapat memiliki lebih dari satu anggaran (misalnya tiap bulan).  
   - Jika kategori dihapus, anggaran terkait juga ikut dihapus (**ON DELETE CASCADE**).  

---

## Diagram (Mermaid)

```mermaid
erDiagram
    Categories ||--o{ Transactions : has
    Categories ||--o{ Budgets : defines

    Categories {
        INTEGER id PK
        TEXT name
        TEXT type
        TEXT color
    }

    Transactions {
        INTEGER id PK
        TEXT title
        REAL amount
        INTEGER date
        TEXT note
        INTEGER category_id FK
        INTEGER created_at
        INTEGER updated_at
    }

    Budgets {
        INTEGER id PK
        INTEGER category_id FK
        REAL amount_limit
        INTEGER start_date
        INTEGER end_date
    }
