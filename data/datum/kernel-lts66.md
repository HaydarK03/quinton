# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | lts66 |
| Versi Kernel |  6.6.122|
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
| firefox | 24 detik| 
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
| CPU Usage (%) | 1.9% | 39.8-96%|
| Load Average |0.56 |  5.77|
| Frekuensi CPU |852 MHZ | 1268MHZ-1697MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,52G| 1.52G|
| RAM Terpakai (Avg) | 630M| 1,11G|
| Swap Usage | 0M| 0M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | saatbuka youtube page delay selama 21 detik dan terjadi delay saat scroll di dalam youtube |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **lts 66** dinyatakan:
- ⚠️  cukup jika hanya menggunakan slims, jika dengan youtube agak lag
- 

idle

<img width="1889" height="989" alt="Image" src="https://github.com/user-attachments/assets/63882187-7947-4be9-ae26-52b588dfb1c8" />

pemakaian

<img width="1895" height="982" alt="Image" src="https://github.com/user-attachments/assets/e83e9f30-301c-4d5c-908e-93c183168a33" />
