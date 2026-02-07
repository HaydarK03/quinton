# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | tkg | 
| Versi Kernel |  6.18.7 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/03/2026|
| Tester | Popon |
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
| firefox | 14 detik| 
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
| CPU Usage (%) | 1.3% | 46-96%|
| Load Average |0.08 | 1.5 - 2.35|
| Frekuensi CPU |867MHZ | 1032MHZ-1676MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,5 G| 1.5G|
| RAM Terpakai (Avg) | 365M| 1,07G|
| Swap Usage | 101M| 107M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (saat load page youtube video pertama kali ada sedikit lag sekitar 3 detik, setekah ke play tidak ada delay) |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux** dinyatakan:
- ⚠️ cukup untuk menjalankan slims
---


## 7. kesimpulan
- cpu dan ram terpakai lebih banyak dari pada kernel linux, namun saat sudah terender semua seperti youtube dan workflow kerja slims lebih nyaman di linux zen
