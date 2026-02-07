# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | linux |
| Versi Kernel |  6.18.7 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/03/2026|
| Tester | Gibran, hakim |
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
| Browser | 12 detik| 
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
| CPU Usage (%) | 5,4% | 43,8%|
| Load Average | 2,9%-5,4%| 17,8%-43,8% |
| Frekuensi CPU |1,250MHZ | 1698MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,5 G| 1,5G|
| RAM Terpakai (Avg) | 538M/1,51G| 1,18G|
| Swap Usage | | |

**Observasi:**
> Contoh: Penggunaan RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (4 detik) |
| Process Hang | Ada / Tidak |

---

## 6. Analisis dan Evaluasi
- Kernel menunjukkan performa **stabil / cukup / kurang**
- Tidak ditemukan / ditemukan **kernel panic**
- Efisiensi resource **lebih baik / setara / lebih buruk** dibanding kernel default

---

## 7. Kesimpulan
Kernel **[nama kernel]** dinyatakan:
- ✅ Stabil untuk penggunaan harian
- ⚠️ Perlu optimasi pada _(bagian tertentu)_
- ❌ Tidak direkomendasikan untuk _(kondisi tertentu)_

---

## 8. Lampiran
- Screenshot btop (Idle, Load, Stress)
- Output `dmesg`
- File konfigurasi kernel (`.config`)

## 9. kesimpulan
-kalo untuk bukap tap slims tidak ada masalah (delay)
-untuk membuka tap youtube ada delay.
