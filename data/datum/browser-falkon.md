# Browser Testing Report

## Informasi Umum
- **Nama Browser** :  falkon
- **Versi Browser** :  25.12.2
- **Kernel** :  linux vfio lts
- **Arsitektur** :  x64
- **Tanggal Pengujian** :  06/02/2026
- **Tester** :  mirza, hakim

---

## Lingkungan Pengujian

### Spesifikasi Perangkat
- **CPU** :  amd E2-1800
- **GPU** :  AMD Palm
- **RAM** :  2GB
- **Storage** : HDD, 300G)  

---

## 1. Performa

### 1.1 Penggunaan Resource (Idle)
> Kondisi: browser terbuka tanpa tab aktif

| Resource | Nilai |
|--------|------|
| CPU Usage | 4,5 % |
| RAM Usage | 516 M |

---

### 1.2 Performa Saat Digunakan
> Kondisi: beberapa tab terbuka (media sosial, streaming, dashboard)

| Aktivitas | Hasil |
|---------|------|
| Startup browser | cepat |
| Membuka tab baru | Cepat |
| Scrolling halaman berat | cepat |
| Video streaming (1080p) | drop frame |
| Web app (GDocs, Figma, dll) | Kurang responsif |

---

## 2. Stabilitas

### 2.1 Stabilitas Penggunaan
- Crash browser: Tidak 
- Tab crash: Tidak  
- Freeze / Hang: Tidak  

---

### 2.2 Error & Masalah
| Aktivitas | Masalah |
|----------|--------|
| play video 1080p    |  video buffering |

---

### 2.3 Konsistensi
- Digunakan selama: 1 jam
- Memory leak terdeteksi: Tidak  
- Perlu restart browser: Tidak  

**Kesimpulan Stabilitas:**  
( butuh optimasi )

---

## 3. User Experience (UX)

### 3.1 Antarmuka & Desain
- Tampilan UI: tidak modern
- Kerapian layout: seperti website jadul   
- Dark mode: Ada 

---

### 3.2 Kemudahan Penggunaan
- Navigasi menu: tidak terlalu Mudah
- Manajemen tab: Baik
- Pengaturan & kustomisasi: Lengkap

---

### 3.3 Responsivitas
- Respons klik & shortcut: Baik
- Transisi UI: Halus

---

### 3.5 Kelebihan & Kekurangan
**Kelebihan:**
-  sedikit lebih cepat dari firefox
-  kemudahan penggunaan

**Kekurangan:**
-  tampilan masih terlihat jadul
-  vidio yutub bofering

---

## 4. Kesimpulan Akhir

- browser dengan tampilan klasik dengan performa yang tidak jauh berbeda dengan firefox
- kurang ideal karena tampilan yang klasik dan performa yang masih berat

---

## 5. Lampiran
- Screenshot resource usage (`btop`, `htop`)

idle 

<img width="1896" height="999" alt="Image" src="https://github.com/user-attachments/assets/326c12f0-6678-4536-a3fa-f2bc5075407e" />

pemakaian

<img width="1890" height="1006" alt="Image" src="https://github.com/user-attachments/assets/3a304c06-775a-4ad2-ad13-3eab3ab5e2f6" />
