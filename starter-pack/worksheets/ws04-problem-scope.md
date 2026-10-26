# WS04: Problem Identification & Scope

**Mata Kuliah**: Konsep Sistem Informasi (KSI)

**Kerangka Kerja**: Project-Based Learning (PBL) Level 1

**Fase Learning Spine**: **Fase 2 — Frame (Problem Discovery & Scope) Minggu / Alokasi Waktu**: Minggu 2 / 14 Jam Belajar

**Sub-CPMK / SFIA**: S-01.1 (Introduce - Problem Framing) | SFIA BUSA L1 (_Business Analysis_), IRMG L1

#### Penanggung Jawab Fase: Phase Lead 2 (Frame — Mahasiswa B)

**Keterkaitan Deliverable**: Sumber Utama Penyusunan **Deliverable D1 (Problem Brief - TPL-01)**

## 1. Identifikasi Tim & Objek Proyek

| **Elemen Informasi**           | **Rincian Identitas Kelompok & Mitra** |
| ------------------------------ | -------------------------------------- |
| **Nama Kelompok / Kelas**      | Young Achievers / Kelas A              |
| **Phase Lead 2 (Frame - M2)**  | Muhammad Khoirul Anam-2600016037       |
| **\-Nama UMKM Mitra Lapangan** | Toko Kelontong Miayu Bu Yati           |
| **Pemilik / Kontak Mitra**     | Bapak                                  |

## 2. Matriks Problem Framing & Analisis Akar Masalah (Root Cause Analysis)

Gunakan temuan kuantitatif dari WS03 untuk memisahkan antara **Gejala Permukaan (_Symptoms_)** dan **Akar Masalah Utama (_Root Cause_)** operasional bisnis mitra:

| **No** | **Kategori Observasi**      | **Gejala Permukaan (_Symptoms_)**                     | **Akar Masalah Operasional (_Root Cause_)**                                           | **Bukti Kuantitatif (_Baseline Data_)**         |
| ------ | --------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------- |
| **1**  | **Proses Transaksi Kasir**  | Antrean mengular panjang saat jam sibuk.              | Pencatatan pesanan dan penghitungan total harga masih manual di buku nota.            | Rata-rata waktu transaksi = **90 detik/orang**. |
| **2**  | **Pengelolaan Stok Barang** | Sering kehabisan stok barang populer secara mendadak. | Pengurangan stok tidak dicatat saat transaksi (_As-Is_), rekap stok hanya bulanan.    | Selisih stok rata-rata **12% per bulan**.       |
| **3**  | **Rekapitulasi Keuangan**   | Pemilik usaha lelah merekap penjualan setiap malam.   | Nota kertas harus dihitung ulang dengan kalkulator dan ditulis ke spreadsheet manual. | Durasi rekap harian = **60–90 menit/malam**.    |

## 3. Perumusan Problem Statement Kontekstual

##### Berdasarkan analisis di atas, rumuskan **Problem Statement** utama dalam 1–2 paragraf terstruktur

_Petunjuk_: Hindari mendefinisikan masalah sebagai _"Mitra belum memiliki aplikasi Python/komputer"_. Definisikan dari hambatan bisnis nyata mitra!

#### Rumusan Problem Statement Kelompok

"Pencatatan transaksi dan inventaris yang masih dilakukan secara manual menggunakan buku kertas nota di \[Nama UMKM Mitra\] (kondisi As-Is) menyebabkan bottleneck operasional berupa waktu transaksi kasir yang lambat (90 detik/pelanggan), keterlambatan pemesanan ulang stok akibat selisih stok 12% per bulan, serta waktu rekapitulasi harian pemilik usaha yang memakan waktu hingga 1,5 jam setiap malam. Kondisi ini menghambat efisiensi operasional dan potensi pertumbuhan omzet mitra."

## 4. Menetapkan Batasan Sistem (System Boundary / Scope Alignment)

Untuk mencegah terjadinya pembengkakan fitur (_Scope Creep_) yang membahayakan penyelesaian proyek dalam 1 semester, tentukan secara tegas apa yang **Masuk Cakupan (_In-Scope_)** dan apa yang **Di Luar Cakupan (_Out-of-Scope_)**:

None

```
┌───────────────────────────────────────────┐
│
│
│
│
│
│
│
SYSTEM BOUNDARY (BATASAN SISTEM)
[ IN-SCOPE: Fitur yang Akan Dibangun ]
```

4. Pencatatan transaksi kasir berbasis konsol (CLI).
5. Pengurangan stok otomatis setiap transaksi berhasil.
6. Pencetakan ringkasan rekapitulasi harian untuk pemilik.

```
│
│
│
│
│
│
│
│─────────────────────────────────────────── │
│ │
│ [ OUT-OF-SCOPE: Di Luar Cakupan Proyek ] │
│ 1. Integrasi gateway pembayaran e-wallet / QRIS otomatis. │
│ 2. Fitur penggajian karyawan / manajemen HRD. │
│ 3. Pemesanan stok otomatis ke supplier luar. │
└────────────────────────────────────────────┘
```

**Tabel Penegasan Cakupan Proyek (_Scope Alignment Table_)**

| **No** | **Modul / Fitur Sistem**          | **Status Cakupan (_In-Scope /_**<br><br>**_Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan (O'Brien)**                                    |
| ------ | --------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------------------------ |
| **1**  | Input Transaksi & Kalkulasi Total | **IN-SCOPE**                                                | Kelayakan Operasional: Sangat dibutuhkan kasir untuk mempercepat transaksi.    |
| **2**  | Update Stok Otomatis              | **IN-SCOPE**                                                | Kelayakan Teknis: Dapat diimplementasikan dengan logika struktur data Python.  |
| **3**  | Laporan Rekap Harian (Laba/Rugi)  | **IN-SCOPE**                                                | Kelayakan Ekonomi: Memberikan nilai _Value of Information_ bagi pemilik usaha. |

| **No** | **Modul / Fitur Sistem**            | **Status Cakupan (_In-Scope /_**<br><br>**_Out-of-Scope_)** | **Alasan Pertimbangan Kelayakan (O'Brien)**                           |
| ------ | ----------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------- |
| **4**  | Pembayaran Online / Payment Gateway | **OUT-OF-SCOPE**                                            | Keterbatasan waktu 1 semester & kompleksitas API luar di PBL Level 1. |
| **5**  | Multi-Branch / Banyak Cabang        | **OUT-OF-SCOPE**                                            | Mitra saat ini hanya memiliki 1 lokasi usaha operasional.             |

## 5. Target Metrik Keberhasilan Solusi (To-Be Targets)

##### Tentukan target kuantitatif perbaikan yang ingin dicapai melalui solusi sistem informasi To-Be

| **Indikator Kinerja**               | **Kondisi As-Is (Baseline)** | **Target To-Be (Expected)** | **Estimasi Persentase Peningkatan**      |
| ----------------------------------- | ---------------------------- | --------------------------- | ---------------------------------------- |
| **Waktu Pelayanan Transaksi Kasir** | 90 detik / pelanggan         | **< 30 detik / pelanggan**  | Peningkatan efisiensi<br><br>**66.7%**   |
| **Durasi Rekapitulasi Harian**      | 60–90 menit / malam          | **< 10 menit / malam**      | Penghematan waktu<br><br>**83.3%**       |
| **Akurasi Pencatatan Stok**         | Selisih 12% / bulan          | **Akurasi > 98%**           | Penurunan tingkat kesalahan selisih stok |

## 6. Refleksi & Lembar Pengesahan Phase Lead

### A. Pertanyaan Refleksi Tim

1. _Bagaimana tim memastikan bahwa batasan proyek yang ditetapkan realistis untuk diselesaikan dalam 16 minggu?_

##### **Jawab**: \[ Jelaskan analisis kelayakan teknis dan kemampuan tim \]

2. _Apakah pemilik usaha mitra telah menyetujui batasan sistem yang diusulkan oleh kelompok?_
   - **Jawab**: \[ Jelaskan hasil konfirmasi awal ke mitra \]

### B. Tanda Tangan Pengesahan Phase Lead 2

None

```
Disusun oleh Phase Lead 2 (Frame): [ Nama Mahasiswa B — NIM ] Tanggal Penyusunan: [ Tanggal ]
Tanda Tangan Phase Lead 2:
Diverifikasi oleh Dosen Pengampu / Coach:
Tanggal: [ Tanggal ] | Status Checkpoint: [ APPROVED / REVISION NEEDED ] Catatan Dosen:
```