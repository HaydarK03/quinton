# Desktop Environment Testing Report

## Informasi Umum
- **Desktop Environment** :  lxde
- **Versi** :  1508
- **Kernel** :  linux-lvfio-lts
- **Arsitektur** : x86_64
- **Tanggal Pengujian** : 6 - 02 - 2026 
- **Tester** :  popon

---

## Spesifikasi Perangkat
### Hardware
- **CPU** :  AMD 1800
- **RAM** :  2 G
- **Storage** : (SSD / HDD, kapasitas)  

### Software
- **Display Server** : (X11 )  
- **Window Manager / Compositor** :  openbox - lxde
- **Driver Grafis** :  

---

## 1. Performa

### 1.1 Penggunaan Resource (Idle)
> Kondisi: setelah login, tanpa aplikasi tambahan

| Resource | idle | pemakaian |
|--------|-------|-------|
| CPU Usage | 2.3% | 30 - 60% | 
| RAM Usage | 482M | 1020M |

**Catatan:**  
(Diambil menggunakan `btop`, `htop`, atau tools sejenis)

---

### 1.2 Performa Saat Beban
> Kondisi: multitasking (browser, file manager, terminal, setting)

| Aktivitas | Respons |
|---------|--------|
| Buka aplikasi | Sedang |
| Switching workspace | Lancar |
| Animasi UI | Kurang halus |

**Kesimpulan Performa:**  
(saat sedang digunakan lancar tetapi saat membuka aplikasi terdapat jeda agar muncul)

---

## 2. Stabilitas

### 2.1 Stabilitas Sistem
- Crash Desktop Environment: Tidak  
- Freeze / Hang: Tidak  
- Logout mendadak: Tidak  

---

### 2.2 Error & Bug
| Aktivitas | Error / Bug |
|-------------|--------------|
| youtube | masih lag saat scroll di youtube | 


---

### 2.3 Konsistensi Penggunaan
- Digunakan selama: (30 M)
- Reboot diperlukan: Tidak  
- Memory leak terdeteksi: tidak

**Kesimpulan Stabilitas:**  
(DE masih butuh perbaikan untuk digunakan secara harian)

---

## 3. User Experience (UX)

### 3.1 Tampilan & Desain
- Kesan visual:Klasik  
- Konsistensi tema: Cukup 
- Dukungan dark mode: Ya   

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: Mudah 
- Pengaturan sistem: Lengkap  
- Cocok untuk pemula: Ya   

---

### 3.3 Responsivitas
- Mouse & Keyboard response: Baik 
- Animasi UI: Sedang 
---

### 3.4 Kelebihan & Kekurangan
**Kelebihan:**
-  cukup mirip dengan dekstop windows jadi tidak terlalu perlu adaptasi yang lama
-  memiliki respon yang cukup cepat

**Kekurangan:**
-  menu setting dipisah menjadi banyak bagian jadi harus lebih teliti dalam mencari


