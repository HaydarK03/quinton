# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | xanmod-lst | 
| Versi Kernel |  6.12.68 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/06/2026|
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
| firefox | 33 detik| 
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
| CPU Usage (%) | 1.9% | 51,3-86,5%|
| Load Average |0.31 |  4,30 |
| Frekuensi CPU |1700MHZ | 860MHZ-16970MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 480M | 1.12G|
| RAM Terpakai (Avg) | 1,52 G | 971 M|
| Swap Usage | 0 K | 108 M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | hanya delay pas masuk ke firefox sisanya sudah oke |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-xanmond-lts** dinyatakan:
- ⚠️ cukup layak walau pada awalnya sedikit lemot dan seturusnya sudah agak medingan
---

