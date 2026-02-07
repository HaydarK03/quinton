# Desktop Environment Testing Report

## Informasi Umum
- **Desktop Environment** :  open-box
- **Versi** :  3.6.1
- **Kernel** :  linux-vfio-lts
- **Arsitektur** : x86_64
- **Tanggal Pengujian** :  02-06-20206
- **Tester** :  mirja

---

## Spesifikasi Perangkat
### Hardware
- **CPU** :  amd E2-1800
- **GPU** :  AMD Palm
- **RAM** :  2GB
- **Storage** : HDD, 300G)  

### Software
- **Display Server** : (X11)  
- **Window Manager / Compositor** : openbox
- **Driver Grafis** :  AMD palm

---

## 1. Performa

### 1.1 Penggunaan Resource (Idle)
> Kondisi: setelah login, tanpa aplikasi tambahan

| Resource | idle | pemakaian |
|--------|-------|
| CPU Usage |  1% |40-67%|
| RAM Usage |394M | 1,02G |

**Catatan:**  
(Diambil menggunakan `btop`, `htop`, atau tools sejenis)

---

### 1.2 Performa Saat Beban
> Kondisi: multitasking (browser, file manager, terminal, setting)

| Aktivitas | Respons |
|---------|--------|
| Buka aplikasi | cepat|
| Switching workspace |  tidak lag|

**Kesimpulan Performa:**  
(performa cepat untuk pindah pindah workspace)

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
| youtube halaman depan | delayed saat scroll |

---
### 2.3 Konsistensi Penggunaan
- Digunakan selama: (jam)
- Reboot diperlukan:Tidak  
- Memory leak terdeteksi: Tidak  

**Kesimpulan Stabilitas:**  
(DE stabil untuk penggunaan harian (namun tidak cocok untuk pemula karna tampilan hanya hitam)

---

## 3. User Experience (UX)

### 3.1 Tampilan & Desain
- Kesan visual: kosong hanya hitam
- Dukungan dark mode: Ya 

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: sulit 
- Pengaturan sistem: harus di install manual
- Cocok untuk pemula: tidak 

---

### 3.3 Responsivitas
- Mouse & Keyboard response: touchpad untuk klik tidak berfungsi
- Animasi UI: Halus

---

### 3.4 Kelebihan & Kekurangan
**Kelebihan:**
-  stabil ( di page youtube home delay tidak terlalu parah)

**Kekurangan:**
- tampilan tidak user friendly
- tidak support rounded
- 

---
