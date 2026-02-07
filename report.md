# Laporan Hasil Research

<!-- Dokumen ini ditulis dalam format Markdown (.md) -->

## Background

Shelver OS merupakan sistem operasi yang dirancang secara khusus untuk mendukung kebutuhan lembaga GLAM (Gallery, Library, Archives, and Museums). Sistem ini dikembangkan dengan pendekatan fungsional dan berorientasi pada stabilitas, keberlanjutan, serta kemudahan untuk hardware dengan spesifikasi rendah dalam skala global.  

## Methods

### Pembentukan dan Pengelolaan Tim

Riset dimulai dengan pembentukan tim yang dimana awalnya ada pergantian ketua yang dilakukan secara musyawarah. Pembentukan tim dilakukan secara sukarela, tanpa ada paksaan untuk bergabung dengan tim riset shelver os. Untuk pengelolaan tim, dilakukan berdasarkan kemampuan individu, seperti kemampuan dalam melakukan instalasi kernel, desktop environment, dan browser. Testing terkait riset pun sudah dibagi kepada individu yang mampu melakukan testing.

### Proses Riset

Proses riset dilakukan secara bertahap, dimulai dari persiapan lingkungan pengujian, penentuan parameter pengukuran, hingga eksekusi pengujian. Setiap pengujian dilakukan dengan skenario yang sama untuk menjaga konsistensi data. Parameter yang diamati meliputi penggunaan sumber daya sistem, stabilitas selama penggunaan, serta respons sistem terhadap aktivitas tertentu.

Selama proses riset, seluruh aktivitas dicatat secara rinci, termasuk kondisi awal sistem, perubahan konfigurasi, dan hasil pengamatan. Dokumentasi dilakukan secara real-time untuk meminimalkan kehilangan data penting.

### kernel
#### 1. linux git

berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-git-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-git-using.png" width="800">


#### 2. linux lqx
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lqx-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lqx-using.png" width="800">


#### 3 linux lts61
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lts61-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lts61-using.png" width="800">


#### 4. linux lts66
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lts66-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lts66-using.png" width="800">


#### 5. linux mainline
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-mainline-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-mainline-using.png" width="800">


#### 6. linux rt
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-rt-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-rt-using.png" width="800">


#### 7. linux rt lts
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-rt-lts-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-rt-lts-using.png" width="800">


#### 8. linux tachyon
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-tachyon-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-tachyon-using.png" width="800">


#### 9. linux vfio
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-vfio-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-vfio-using.png" width="800">


#### 10. linux vfio lts
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-vfio-lts-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-vfio-lts-using.png" width="800">


#### 11. linux zen
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-zen-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-zen-using.png" width="800">

### desktop environment



### browser



### Penanganan Error

Dalam pelaksanaan riset, ditemukan beberapa error dan kendala teknis, seperti ketidakstabilan sistem, error aplikasi, maupun hasil pengukuran yang tidak konsisten. Setiap error tidak diabaikan, melainkan dicatat sebagai bagian dari data riset. Tim melakukan analisis penyebab error, kemudian menentukan apakah error tersebut berasal dari faktor sistem, konfigurasi, atau metode pengujian.

Pendekatan ini dilakukan agar hasil riset mencerminkan kondisi nyata di lapangan, bukan hanya kondisi ideal tanpa gangguan.

## Result

### Kernel

| Kernel       | Firefox   | CPU        | RAM       | Delay                                                                                                                                               | Hang                                                              |
| ------------ | --------- | ---------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| lqx          | 30 detik  | 36–89%     | 1,23G     | saat tab yutub dibuka terjadi delay yang cukup lama dan saat kursor digerakan jg terjadi delay                                                      | tidak ada                                                         |
| mainline     | 35 detik  | 36–86%     | 971M      | hanya saat diawal saja selebihnya sudah oke                                                                                                         | tidak ada                                                         |
| vfio         | 37 detik  | 66,2–87,3% | 1,4G      | saat buka firefox terjadi delay yang cukup lama, saat membuka tap yutub terjadi delay, dan juga saat membuka tap baru/gonta-ganti tab terjadi delay | tidak ada                                                         |
| tachyon      | 35 detik  | 36,8–90,1% | 1,4G      | saat buka firefooks terjadi delay yang cukup lama, dan saat searching ada sedikit delay                                                             | tidak ada                                                         |
| linux-git    | 13 detik  | 64–99,1%   | 1,06G     | Ada (saat load video pertama di youtube, setelah load masih ada delay yang terjadi)                                                                 | tidak ada                                                         |
| tkg          | 14 detik  | 46–96%     | 1,07G     | Ada (saat load page youtube video pertama kali ada sedikit lag sekitar 3 detik, setelah play tidak ada delay)                                       | tidak ada                                                         |
| linux-lts61  | 22 detik  | 24–94%     | 1,21G     | Ada (saat load video di youtube)                                                                                                                    | tidak ada                                                         |
| linux lts    | 10 detik  | 43,8%      | 1,216G    | Ada (browser 10–20 detik, buka page berat 4 detik)                                                                                                  | Ada (ketika membuka page berat hang sampai kursor tidak bergerak) |
| linux        | 12 detik  | 43,8%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| linux zen    | 12 detik  | 41,7%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| linux-rt-lts | 21 detik  | 50–94%     | 1,14G     | Ada (saat load video pertama di youtube, setelah load sudah tidak ada lag lagi)                                                                     | tidak ada                                                         |
| linux-rt     | 12 detik  | 43,8%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| lts66        | 24 detik  | 39,8–96%   | 1,11G     | saat buka youtube page delay selama 21 detik dan terjadi delay saat scroll di dalam youtube                                                         | tidak ada                                                         |
| vfio-lts    | 21 detik  | 40–90%     | 1,03G     | delay saat buka page youtube sekitar 8 detik, saat sudah di dalam video lancar                                                                      | tidak ada                                                         |
| **nitrous**  | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **lts515**   | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **lts510**   | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **xanmod** | **gagal** | **gagal** | **gagal** | **gagal** | **gagal** |
| **xanmod-rt** | **gagal** | **gagal** | **gagal** | **gagal** | **gagal** |

## 1. Perbandingan Kecepatan Aplikasi (Firefox)

### Tercepat membuka Firefox

1. **linux lts** – 10 detik
2. **linux / linux zen / linux-rt** – 12 detik
3. **linux-git** – 13 detik
4. **tkg** – 14 detik

### Paling lambat

* **vfio** – 37 detik
* **mainline / tachyon** – 35 detik
* **lqx** – 30 detik

👉 **Catatan:** cepat buka Firefox **tidak selalu berarti respons sistem baik** (contoh: linux lts).

---

## 2. Perbandingan Performa CPU

### CPU Paling Stabil (range tidak ekstrem)

* **mainline** (36–86%)
* **lqx** (36–89%)
* **vfio-lts** (40–90%)
* **linux-rt-lts** (50–94%)

### CPU Paling Agresif / Spike Tinggi

* **linux-git** (hingga 99,1%)
* **tkg** (hingga 96%)
* **lts66** (hingga 96%)

👉 Kernel agresif terasa cepat, tapi **berpotensi bikin lag di hardware lemah**.

---

## 3. Perbandingan Penggunaan RAM

### Paling Hemat RAM

1. **mainline** – 971M
2. **vfio-lts** – 1,03G
3. **linux-git** – 1,06G
4. **tkg** – 1,07G

### Paling Boros RAM

* **vfio / tachyon** – 1,4G
* **lqx** – 1,23G

👉 Untuk RAM 2 GB, **mainline dan vfio-lts paling aman**.

---

## 4. Perbandingan Delay & Respons Sistem

### Delay Paling Ringan / Bisa Ditoleransi

* **mainline** → hanya di awal
* **tkg** → ±3 detik, setelah itu lancar
* **linux-rt-lts** → hanya saat load awal
* **vfio-lts** → ±8 detik, setelah itu lancar

### Delay Berat & Mengganggu

* **lqx** → delay panjang + kursor ikut delay
* **vfio** → delay di hampir semua aktivitas
* **lts66** → delay 21 detik + scroll lag
* **linux lts** → delay browser 10–20 detik

---

## 5. Perbandingan Stabilitas (Hang)

### Paling Stabil (tidak ada hang)

* lqx
* mainline
* vfio
* tachyon
* linux-git
* tkg
* linux-lts61
* linux-rt-lts
* lts66
* vfio-lts

### Ada Risiko Hang

* **linux lts**
* **linux**
* **linux zen**
* **linux-rt**

👉 Kernel non-LTS & non-RT **lebih sering tidak konsisten stabilitasnya**.

---

## 6. Kernel Gagal Total

Tidak lolos pengujian:

* **nitrous**
* **lts515**
* **lts510**
* **xanmod**
* **xanmod-rt**

❌ Tidak layak dipakai di sistem uji ini.

---

## 7. Kesimpulan Akhir (Berdasarkan Data)

### 🔥 Kernel Paling Seimbang (Rekomendasi)

1. **vfio-lts** → RAM hemat, delay ringan, stabil
2. **mainline** → RAM paling irit, delay minimal
3. **tkg** → cepat & responsif setelah load awal

### ⚠️ Cukup Tapi Kurang Nyaman

* lts66
* linux-lts61
* linux-rt-lts

### ❌ Tidak Direkomendasikan

* vfio (non-lts)
* lqx
* linux lts / linux / linux zen / linux-rt
* kernel yang statusnya **gagal**

## Conclusion

Berdasarkan seluruh rangkaian riset yang telah dilakukan, dapat disimpulkan bahwa pendekatan riset yang terstruktur dan transparan sangat berpengaruh terhadap kualitas hasil yang diperoleh. Pencatatan error sebagai bagian dari data terbukti memberikan nilai tambah dalam memahami kondisi nyata sistem.

Riset ini berhasil mencapai tujuan awal, yaitu menghasilkan data yang objektif dan dapat digunakan sebagai dasar evaluasi serta pengambilan keputusan. Ke depan, riset lanjutan dapat dilakukan dengan memperluas parameter pengujian atau menambahkan variasi skenario agar hasil yang diperoleh semakin komprehensif dan akurat.
