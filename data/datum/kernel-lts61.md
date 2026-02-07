# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | linux-lts61 |
| Versi Kernel |  6.1.161 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 03/02/2026|
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
| firefox | 22 detik| 
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
| CPU Usage (%) | 2.2 - 3.8% | 24-94%|
| Load Average |0.15 | 3.1|
| Frekuensi CPU |850MHZ | 850MHZ-1687MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,52 G| 1.52 G|
| RAM Terpakai (Avg) | 600M| 1,21G|
| Swap Usage | 0M| 0M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (saat load video di youtube |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-lts** dinyatakan:
- ⚠️ cukup untuk menjalankan slims dan menyetel musik 
---


## 7. kesimpulan
-tab youtube berjalan lancar walau terdapat delay saat scroll
- dmesg tidak ada error

idle

<img width="1911" height="998" alt="Image" src="https://github.com/user-attachments/assets/ca3c1fe7-557f-439e-9013-4ff1251a3e63" />

pemakaian

<img width="1889" height="1010" alt="Image" src="https://github.com/user-attachments/assets/f7fd33ad-0c6f-4dd2-8cb5-bb840f1dcd18" />
