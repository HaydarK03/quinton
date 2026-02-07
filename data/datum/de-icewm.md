# Desktop Environment Testing Report

## Informasi Umum
- **Desktop Environment** :  icewm
- **Versi** :  4.0.0
- **Kernel** :  linux-vfio-lts
- **Arsitektur** : x86_64
- **Tanggal Pengujian** :  02-06-2026
- **Tester** :  sultan

---

## Spesifikasi Perangkat
### Hardware
- **CPU** :  amd E2-1800
- **GPU** :  AMD Palm
- **RAM** :  2GB
- **Storage** : HDD, 300G)  

### Software
- **Display Server** : (X11)  
- **Window Manager / Compositor** : xfwm4  
- **Driver Grafis** :  AMD palm

---

## 1. Performa

### 1.1 Penggunaan Resource (Idle)
> Kondisi: setelah login, tanpa aplikasi tambahan

| Resource | idle | pemakaian |
|--------|-------|
| CPU Usage |  2.9% | 36-90% |
| RAM Usage | 418M | 1,14G |

**Catatan:**  
(Diambil menggunakan `htop`)

---

### 1.2 Performa Saat Beban
> Kondisi: multitasking (browser, file manager, terminal, setting)

| Aktivitas | Respons |
|---------|--------|
| Buka aplikasi | 5 detik |
| Switching workspace | lancar |

**Kesimpulan Performa:**  
(performa bagus )

---

## 2. Stabilitas

### 2.1 Stabilitas Sistem
- Crash Desktop Environment: Tidak  
- Freeze / Hang: tidak ada
- Logout mendadak: Tidak  

---

### 2.2 Error & Bug
| Aktivitas | Error / Bug |
|----------|------------|
| youtube halaman depan | delayed saat scroll sepersekian detik |

---
### 2.3 Konsistensi Penggunaan
- Digunakan selama: 26 min
- Reboot diperlukan:Tidak  
- Memory leak terdeteksi: Tidak  

**Kesimpulan Stabilitas:**  
(DE stabil untuk penggunaan harian (namun tidak untuk buka banyak page sekaligus)

---

## 3. User Experience (UX)

### 3.1 Tampilan & Desain
- Kesan visual: hanya ada taskbar dibawah (default)  
- Dukungan dark mode: Ya 

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: sedikit sulit 
- Pengaturan sistem: lengkap 
- Cocok untuk pemula: kurang, harus terbiasa 

---

### 3.3 Responsivitas
- Mouse & Keyboard response: Baik   
- Animasi UI: Halus   

---

### 3.4 Kelebihan & Kekurangan
**Kelebihan:**
-  tampilan mudah dimengerti karena mirip tampilan windows 

**Kekurangan:**
-  butuh update tampilan karna tampilan lumayan 
