# Desktop Environment Testing Report

## Informasi Umum
- **Desktop Environment** :  fluxbox
- **Versi** :  1.3.7
- **Kernel** :  linux-lts
- **Arsitektur** : x86_64
- **Tanggal Pengujian** :  06-02-2006
- **Tester** :  gibran

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
|--------|-------|-------|
| CPU Usage |  2,6% |3.6-49,7%|
| RAM Usage |309M | 887M |

**Catatan:**  
(Diambil menggunakan `btop`, `htop`, atau tools sejenis)

---

### 1.2 Performa Saat Beban
> Kondisi: multitasking (browser, file manager, terminal, setting)

| Aktivitas | Respons |
|---------|--------|
| Buka aplikasi | lancar |
| Switching workspace |  lancar |

**Kesimpulan Performa:**  
(performa lancar)

---

## 2. Stabilitas

### 2.1 Stabilitas Sistem
- Crash Desktop Environment: Tidak  
- Freeze / Hang: tidak ada
- Logout mendadak: Tidak  

---

### 2.2 Error & Bug
tidak ada

---
### 2.3 Konsistensi Penggunaan
- Digunakan selama: (jam)
- Reboot diperlukan:Tidak  
- Memory leak terdeteksi: Tidak  

**Kesimpulan Stabilitas:**  
(DE stabil untuk penggunaan harian (namun tidak untuk buka banyak page sekaligus)

---

## 3. User Experience (UX)

### 3.1 Tampilan & Desain
- Kesan visual: kaku 
- Dukungan dark mode: tidak

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: sulit
- Pengaturan sistem: tidak 
- Cocok untuk pemula: tidak

---

### 3.3 Responsivitas
- Mouse & Keyboard response: Baik   
- Animasi UI: Halus   

---

### 3.4 Kelebihan & Kekurangan
**Kelebihan:**
- ringan

**Kekurangan:**
-  sulit untuk membuka menu
- tidak ada dock

---
