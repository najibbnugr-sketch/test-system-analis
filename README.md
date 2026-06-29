# Sistem Informasi Pengadaan & Pembayaran Barang (SIP Barang)

Prototipe web application Single Page Application (SPA) untuk pengelolaan pengadaan barang dari hulu (permintaan unit) hingga hilir (pembayaran kasir) dengan simulasi Role-Based Access Control (RBAC).

## Live Demo & Deployment
Aplikasi telah di-deploy dan dapat dicoba secara langsung di Vercel:
**[https://test-system-analis.vercel.app](https://test-system-analis.vercel.app)**

---

## Akun Demo & Matriks Peran (RBAC)
Aplikasi mendukung multi-role login untuk mensimulasikan alur bisnis riil. Gunakan akun berikut dengan sandi **`demo123`**:

 Nama Pengguna  Peran (Role)  Hak Akses Utama 
---------
 **ahmad**  Unit Pemohon (IT)  Mengajukan permintaan barang baru, melihat riwayat permintaan unit sendiri 
 **budi**  Petugas Procurement  Validasi kelayakan permintaan, membuat PKS & Purchase Order (PO) supplier 
 **citra**  Petugas Budgeting  Verifikasi ketersediaan pagu anggaran unit sebelum PO diterbitkan 
 **dina**  Petugas Keuangan  Mencatat tagihan invoice dari supplier berdasarkan PO & PKS 
 **eko**  Petugas Kasir  Melakukan pencairan dana pembayaran termin, melihat laporan anggaran 

---

##  Fitur Utama
1. **Google Workspace UI Style**: Desain antarmuka datar (flat), minimalis, bersih, dan fungsional dengan ikon SVG konsisten tanpa emoji.
2. **Dashboard Kontekstual & Chart**: Grafik real-time realisasi anggaran vs sisa pagu menggunakan *Chart.js*.
3. **Sistem Notifikasi**: Riwayat aktivitas log transaksi yang diperbarui secara dinamis pada *localStorage*.
4. **Dokumentasi Sistem Terintegrasi**: UML Class Diagram, Sequence Diagram, Use Case Diagram, ERD, dan Matriks RBAC interaktif langsung di dalam aplikasi (menggunakan *Mermaid.js*).

---

## Teknologi yang Digunakan
* HTML5 (Struktur & Tata Letak)
* Vanilla CSS3 (Desain Responsif & Tata Letak Google Style)
* Vanilla JavaScript (Logika State Management, localStorage DB, dan Navigasi RBAC)
* Chart.js (Visualisasi Laporan Grafik)
* Mermaid.js (Rendering UML & Flowchart secara dinamis)
