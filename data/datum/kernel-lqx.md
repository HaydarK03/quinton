# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | lqx | 
| Versi Kernel |  6.18.8 |
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
| firefox | 30 detik| 
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
| CPU Usage (%) | 1.9% | 36-89%|
| Load Average |0.01 |  2.14|
| Frekuensi CPU |1060MHZ | 1032MHZ-1676MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,52G| 1.52G|
| RAM Terpakai (Avg) | 661M| 1,23G|
| Swap Usage | 0M| 435M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | saat tab yutub dibuka terjadi delay yang cukup lama dan saat kursor digerakan jg terjadi delay |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-lqx** dinyatakan:
- ⚠️ tidak layak untuk menjalankan slims dan youtube, meski dijalankan salah satunya saja sudah ngelag saat menjalankannya

