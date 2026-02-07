# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | vfio |
| Versi Kernel |  6.18.7|
| Arsitektur | x86_64 |
| Tanggal Pengujian | 02/05/2026|ac
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
| firefox | 37 detik| 
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
| CPU Usage (%) | 26,9% | 66,2-87,3%|
| Load Average |0.83 |  3,75|
| Frekuensi CPU |869 MHZ | 869MHZ-1696MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,4G| 1.51G|
| RAM Terpakai (Avg) | 354M| 1,4G|
| Swap Usage | 49,9M| 51,8M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | saat buka firefox terjadi delay yang cukup lama, saat membuka tap yutub terjadi delay, dan juga saat membuka tap baru/gonta-ganti tab terjadi delay
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **vfio** dinyatakan:
- ⚠️  tidak layak untuk menjalankan slims dan youtube,  karena lemot/ delaysaat di jalankan


idle

<img width="1907" height="1010" alt="Image" src="https://github.com/user-attachments/assets/78d279b0-671d-4a90-bfb3-881f3421d18b" />


pemakaian

<img width="1901" height="998" alt="Image" src="https://github.com/user-attachments/assets/45ec4a38-2943-404c-9ab0-52d774c2978d" />
