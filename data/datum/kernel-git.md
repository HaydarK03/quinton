# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | linux-git|
| Versi Kernel |  6.19.8 |
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
| firefox | 13 detik| 
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
| CPU Usage (%) | 1 - 2.6
% | 64-99.1%|
| Load Average |0.04 | 2.35 - 5.28|
| Frekuensi CPU |849MHZ - 1325MHZ | 1175MHZ-1696MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,51 G| 1.51G|
| RAM Terpakai (Avg) | 576M| 1,06G|
| Swap Usage | 0K| 53.8M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (saat load video pertama di youtube, setelah load masih ada delay yang terjadi |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-git** dinyatakan:
- ⚠️ cukup untuk menjalankan slims dan menyetel musik 
---


## 7. kesimpulan
-tab youtube berjalan dengan sedikit delay baik vidio pertama atau setelahnya, tetapi masih layak untuk digunakan
- dmesg tidak ada error

idle

<img width="1895" height="999" alt="Image" src="https://github.com/user-attachments/assets/79f2260c-4c0d-42da-a8e8-e59f65a8c8aa" />

pemakaian

<img width="1903" height="994" alt="Image" src="https://github.com/user-attachments/assets/1e830898-96ec-4635-bde5-b3ae8779935d" />
