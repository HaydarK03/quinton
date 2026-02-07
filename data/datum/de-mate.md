# Desktop Environment Testing Report

## Informasi Umum
- **Desktop Environment** :  mate
- **Versi** :  1.28.2
- **Kernel** :  linux-vfio-lts
- **Arsitektur** : x86_64
- **Tanggal Pengujian** :  02-06-20206
- **Tester** :  hakim

---

## Spesifikasi Perangkat
### Hardware
- **CPU** :  amd E2-1800
- **GPU** :  AMD Palm
- **RAM** :  2GB
- **Storage** : HDD, 300G)  

### Software
- **Display Server** : (X11)  
- **Window Manager / Compositor** : marco
- **Driver Grafis** :  AMD palm

---

## 1. Performa

### 1.1 Penggunaan Resource (Idle)
> Kondisi: setelah login, tanpa aplikasi tambahan

| Resource | idle | pemakaian |
|--------|-------|
| CPU Usage |  1,9% |82,2-98%|
| RAM Usage |558M | 1,11G |

**Catatan:**  
(Diambil menggunakan `btop`, `htop`, atau tools sejenis)

---

### 1.2 Performa Saat Beban
> Kondisi: multitasking (browser, file manager, terminal, setting)

| Aktivitas | Respons |
|---------|--------|
| Buka aplikasi |Sedang |
| Switching workspace |  Sedikit lag |

**Kesimpulan Performa:**  
(performa sedang karena ada sedikit lag di awal pembukaan web/page baru namun setelah berjalan sudah lancar)

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
- Digunakan selama: (38 menit)
- Reboot diperlukan:Tidak  
- Memory leak terdeteksi: Tidak  

**Kesimpulan Stabilitas:**  
(DE stabil untuk penggunaan harian (namun tidak untuk buka banyak page sekaligus)

---

## 3. User Experience (UX)

### 3.1 Tampilan & Desain
- Kesan visual: kuno (default)  
- Dukungan dark mode: Ya 

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: Mudah 
- Pengaturan sistem: Lengkap 
- Cocok untuk pemula: Ya 

---

### 3.3 Responsivitas
- Mouse & Keyboard response: Baik   
- Animasi UI: Halus   

---

### 3.4 Kelebihan & Kekurangan
**Kelebihan:**
-  tampilan mudah di mengerti untuk pemula karena mirip dengan di windows

**Kekurangan:**
-  butuh update tampilan karna tampilan lumayan tua, delay saat scrol yutub
- delay saat gonta-ganti tab dan agak sedikit ngelag
---
