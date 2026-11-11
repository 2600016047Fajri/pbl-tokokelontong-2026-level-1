# WORKBOOK: LEMBAR KERJA MAHASISWA WS05

## Formulasi Kebutuhan Fungsional: User Story & Acceptance Criteria

Mata Kuliah: **Konsep Sistem Informasi (KSI)**

Kerangka Kerja: **Project-Based Learning (PBL) Level 1**

Fase Learning Spine: **Fase 3 — Define (Minggu 3)**

Sub-CPMK / SFIA: **S-01.1 (Intermediate - Problem Framing) & S-03.1 (Intermediate - Pemetaan SI)** | **SFIA BUSA L1, REQM L2**

Keterkaitan Deliverable: **Bahan Utama Deliverable D2 (System & Solution Design - TPL-02)**

### 1. Identifikasi Kelompok & Rotasi Kepemimpinan

##### Nama Kelompok: Young Achievers

- **Objek UMKM Mitra**: Toko Kelontong
- **Phase Lead 3 (Define)**: Muh Ali NP
- **Anggota Tim**: 1. Fajri Alfiturrahman
- 2\. Muhammad Khoirul Anam
- 3\. Habib Reifan Alfarisi
- 4\. Muhammad Faqih Hammam

### 2. Landasan Konseptual: Analisis Sistem "What" vs "How"

Dalam tahap _Systems Analysis_, fokus utama tim adalah menentukan **APA (_What_)** yang dibutuhkan pengguna bisnis untuk memecahkan masalahnya, **BUKAN BAGAIMANA (_How_)** sistem dibangun secara teknis (Marakas & O'Brien, 2013).

- **User Story** merepresentasikan kebutuhan fungsional dari sudut pandang pengguna bisnis dengan pola:

\$\$\\text{"Sebagai \[Peran Pengguna\], Saya ingin \[Kemampuan/Fitur\], Sehingga \[Manfaat Bisnis Nyata\]"}\$\$

- **Acceptance Criteria (Given-When-Then)** mendefinisikan batas kondisi kapan sebuah fitur dinyatakan selesai dan memenuhi syarat penerimaan pengguna (Rainer et al., 2021).

### 3. Workspace A: Formulasi User Story Fungsional

Petakan minimal **3 User Story Utama** yang langsung menjawab akar masalah pada D1 / WS04:

#### User Story 1 (Prioritas Utama / Core Feature)

- **Sebagai (_As a_)**:

pemilik toko kelontong

- **Saya ingin (_I want to_)**:

Saya ingin memiliki catatan pemasukan dan pengeluaran agar dapat memantau kondisi keuangan toko

- **Sehingga (_So that_)**:

Sehingga catatan pemasukan dan pengeluaran terstruktur dan mudah di pantau

#### User Story 2 (Fitur Manajemen Stok / Data)

- **Sebagai (_As a_)**:

Pemilik toko kelontong

- **Saya ingin (_I want to_)**:

Saya ingin mengetahui stok barang yang tersedia

- **Sehingga (_So that_)**:

Sehingga memudahkan saya memantau stok barang dan mengetahui barang yang perlu di tambah.

#### User Story 3 (Fitur Pelaporan / Informasi)

- **Sebagai (_As a_)**:

Pemilik toko kelontong

- **Saya ingin (_I want to_)**:

Saya ingin memiliki laporan transaksi penjualan yang tercatat dan akurat

- **Sehingga (_So that_)**:

Sehingga saya mengetahui Riwayat transaksi penjualan dan jumlah pemasukan atau pengeluaran toko.

### 4. Workspace B: Acceptance Criteria Berbasis Skenario (Given-When-Then)

Susun kriteria penerimaan terstruktur untuk **User Story 1** (mencakup Skenario Sukses dan Skenario Penanganan Eror):

#### Skenario 1A: Transaksi Penjualan Berhasil (Happy Path)

- **Diberikan (_Given_)**:

Total belanjaan pembeli _RP 10.000_

- **Ketika (_When_)**:

Bapak mencatat pemasukan ke dalam buku _RP 10.000_

- **Maka (_Then_)**:

Pencatatan benar dan tidak mengalami kerugian

#### Skenario 1B: Penanganan Pembayaran Kurang / Eror (Exception Path)

- **Diberikan (_Given_)**:

Total belanjaan pembeli RP 25.000

- **Ketika (_When_)**:

Bapak mencatat total belanjaan _RP 20.000_

- **Maka (_Then_)**:

Pencatatan salah dan mengalami kerugian

### 5. Workspace C: Catatan Validasi Kebutuhan dengan Mitra (Field Confirmation)

##### Tanggal Validasi

- **Narahubung Mitra**: (Pemilik / Staf Kasir)

##### Hasil Konfirmasi User Story

\[ \] Seluruh User Story disetujui mitra

\[ \] Terdapat penyesuaian/revisi kebutuhan (Tuliskan revisi jika ada):

### 6. Verifikasi Integritas AI (TPL-07) & Pengesahan

##### Penggunaan AI Co-pilot

Apakah tim menggunakan AI untuk membantu merumuskan skenario _Given-When-Then_? \[ \] Ya \[ \] Tidak

_(Jika Ya, wajib melampirkan formulir_ **_TPL-07: AI Usage Disclosure & Verification Note_**_)_.

##### Tanda Tangan Tim & Pengesahan Dosen

- **Phase Lead 3**: (Tanggal: )
- **Dosen Coach**: (Tanggal: ) \[ \] Approved