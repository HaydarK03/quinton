# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | linux-rat-lts|
| Versi Kernel |  6.6.87 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 03/02/2026|
| Tester | Mirza |
| Lingkungan | Bare Metal |
| Desktop | XFCE |

---

## 2. Spesifikasi Sistem Uji

### 2.1 Hardware
| Komponen | Detail |
|---------|--------|
| CPU | AMD E2 VISION|
| RAM | 2 GB|
| Storage | 50 GB |

### 2.2 Software
| sofware| Durasi|
|---------|--------|
| firefox | 21 detik| 
---

## 3. Metodologi Pengujian

### 3.1 Skenario Pengujian
- Idle system (tanpa beban)
- Pemakaian user (slims, youtube, htop)

### 3.2 Tools Pengujian
- `htop` → Monitoring performa sistem
- `dmesg` → Log kernel

---

## 4. Hasil Pengujian Performa (htop)

### 4.1 CPU Performance
| Parameter | Idle | Pemakaian |
|---------|------|-----|
| CPU Usage (%) | 1.9% | 50-94%|
| Load Average |0.22 | 4.4|
| Frekuensi CPU |850MHZ | 1300MHZ-1695MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,5 G| 1.5G|
| RAM Terpakai (Avg) | 435M| 1,14G|
| Swap Usage | 0M| 0M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (saat load video pertama di youtube, setelah load sudah tidak ada lag lagi |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-rt-lts** dinyatakan:
- ⚠️ cukup untuk menjalankan slims
---


## 7. kesimpulan
- tab youtube berjalan lancar lebih baik dari kernel linux dan linux-zen, sedikit lag di awal pemutaran video namun sudah tidak ada lag lagi setelah di putar
- eksperiens sama seperti menggunakan linux lts
- dmesg tidak ada error
