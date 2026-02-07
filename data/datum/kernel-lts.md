# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | linux lts |
| Versi Kernel |  6.12.68 |
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/03/2026|
| Tester | mirja, gibran |
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
| Browser | 10 detik| 
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
| CPU Usage (%) | 4,6% | 43,8%|
| Load Average | 2,9%-5,4%| 64,6%-99,4% |
| Frekuensi CPU |1,250MHZ | 1698MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,5 G| 1,5G|
| RAM Terpakai (Avg) | 520M/1,51G| 1,216G|
| Swap Usage | | |

**Observasi:**
> Contoh: Penggunaan RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | Ada (browser 10-20 detik, buka page berat 4 detik|
| Process Hang | Ada (ketika membuka page berat hang sampai kursor tidak bergerak)  |

---

## 6. Analisis dan Evaluasi
- 

---

## 7. Kesimpulan
Kernel **kernel lts** dinyatakan:
- Tidak direkomendasikan untuk membuka page berat


## 9. kesimpulan
-gakuat page berat seperti canva
-crash setelah close page berat
- youtube dan slims masih berjalan
- youtube video glitch ketika fullscreen

idle

<img width="1907" height="1004" alt="Image" src="https://github.com/user-attachments/assets/60cfb3cb-1d30-44d5-969a-12954ee5c1a6" />

pemakaian

<img width="1892" height="1012" alt="Image" src="https://github.com/user-attachments/assets/1d9a9e5b-b750-4288-b656-f2f6c5be774e" />
