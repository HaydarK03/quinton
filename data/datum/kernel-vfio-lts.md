# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | vfio-lts |
| Versi Kernel |  6.12.58|
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/06/2026|
| Tester | mirja |
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
| CPU Usage (%) | 2% | 40-90%|
| Load Average |0.5 |  3,75|
| Frekuensi CPU |850-1275 MHZ | 1025MHZ-1696MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,5G| 1.51G|
| RAM Terpakai (Avg) | 565M| 1,03G|
| Swap Usage | 0M| 15M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | delay saat buka page youtube sekitar 8detik saat sudah di dalam video lancar |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **vfio-lts** dinyatakan:
- ⚠️  cukup untuk menjalankan slims dan youtube
- dmesg tidak ada error


idle 

<img width="1903" height="1006" alt="Image" src="https://github.com/user-attachments/assets/dfabcf7e-0a52-4d1a-a965-6da900f39d08" />


pemakaian


<img width="1903" height="1002" alt="Image" src="https://github.com/user-attachments/assets/2985409f-1341-46c6-8d8c-c0eee7ca2dab" />
