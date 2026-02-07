# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | tachyon 
| Versi Kernel |  6.18.7|
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/05/2026|
| Tester | hakim |
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
| firefox | 35 detik| 
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
| CPU Usage (%) | 1,6% | 36,8-90,1%|
| Load Average |0.22 |  2.65|
| Frekuensi CPU |863 MHZ | 863MHZ-1696MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,51G| 1.51G|
| RAM Terpakai (Avg) | 323M| 1,4G|
| Swap Usage | 248M| 439M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | saat buka firefooks terjadi delay yang cukup lama, dan saat searching ada sedikit delay|
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-ltachyon** dinyatakan:
- ⚠️  layak untuk menjalankan slims dan youtube.
