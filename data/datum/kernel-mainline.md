# Laporan Hasil Testing Kernel

## 1. Informasi Umum
| Item | Keterangan |
|------|-----------|
| Nama Kernel | mainline | 
| Versi Kernel |  6.19.0 |
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
| CPU Usage (%) | 1.9% | 36-86%|
| Load Average |0.00 |  2.54|
| Frekuensi CPU |849MHZ | 849MHZ-1670MHZ |

**Observasi:**
> Tuliskan hasil pengamatan performa CPU berdasarkan htop.

---

### 4.2 Memory Performance
| Parameter | idle | pemakaian |
|---------|-------| --- |
| Total RAM | 1,51G| 1.51G|
| RAM Terpakai (Avg) | 360M| 971 M|
| Swap Usage | 47M| 51M|

**Observasi:**
 RAM stabil tanpa kenaikan abnormal.


---

## 5. Hasil Pengujian Stabilitas Kernel

### 5.1 Respons Sistem
| Aspek | Hasil |
|------|-------|
| Delay Input | hanya saat diawal saja selebihnya sudah oke |
| Process Hang | tidak ada  |

---

---

## 6. Kesimpulan
Kernel **linux-mainline** dinyatakan:
- ⚠️ cukup layak walau pada awalnya sedikit lemot dan seturusnya sudah agak medingan
---


## 7. kesimpulan


idle

<img width="1899" height="1014" alt="Image" src="https://github.com/user-attachments/assets/fd8a7dcc-bb75-4c5a-9e51-33b2d156a198" />


pemakaian

<img width="1902" height="993" alt="Image" src="https://github.com/user-attachments/assets/1a44430a-23a3-4662-99af-dabdad536a13" />
