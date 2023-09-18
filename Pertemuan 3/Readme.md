## Tujuan
Tujuan Praktikum kali ini adalah membuat **Model Regresi terbaik dengan Peubah Lag**.  
  
## Link RPUBS
Agar _memudahkan_ untuk dibaca..  
Daripada liatin rmd nya, mending liat `rpubs` nya.. XD    
Yuk mampir ke :  
https://rpubs.com/ZenR_Prog/MPDW-Prak03  
  
## Tentang Data
Link Data :  
https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data?select=salesmonthly.csv   
Saya menggunakan data yang sama dengan pertemuan 2.  
Data ini merupakan data penjualan 8 obat di sebuah farmasi.  
Ada beberapa pilihan data. Data dengan periode per-jam, per-hari, per-minggu, dan per-bulan.  
Data yang saya gunakan adalah data dengan periode per-bulan.  
Berikut adalah kode obat yang tersedia dan deskripsinya:  
1. `M01AB` : Obat antiinflamasi dan antirheumatik non-steroid, derivatif asam asetat.
2. `M01AE` : Obat antiinflamasi dan antirheumatik non-steroid, derivatif asam propionat.
3. `N02BA` : Analgesik dan antipiretik, asam salisilat dan derivatifnya.
4. `N02BE` : Analgesik dan antipiretik, pirazolon dan anilida.
5. `N05B`  : Obat psikoleptik, ansiolitik.
6. `N05C`  : Obat psikoleptik, obat tidur dan penenang.
7. `R03`   : Obat untuk penyakit saluran napas obstruktif.
8. `R06`   : Antihistamin untuk penggunaan sistemik.  
Data yang akan saya gunakan adalah data dalam periode per bulan.  
Beberapa waktu yang lalu saya merasa sulit untuk tidur. Kebetulan ada obat `N05C` yang merupakan obat tidur dalam dataset saya. `N05C` merupakan obat penenang, sifat tenang ini yang mungkin membantu seseorang untuk tidur. Ternyata ada obat tipe penenang lainnya, yakni `N05B`.  
  
Kedua obat ini memiliki kesamaan yakni termasuk dalam klasifikasi **ATC N** (*Nervous System*), yang berarti keduanya berhubungan dengan **sistem saraf**. Kedua obat ini termasuk dalam kelompok ***"Psycholeptics drugs,"*** yang berarti keduanya dapat memengaruhi **sistem saraf** dan **suasana hati** pasien.  
  
Namun ada beberapa perbedaan, diantaranya: `N05B` lebih fokus pada **obat penenang** dan pengobatan **gangguan kecemasan**. Sementara `N05C` lebih fokus pada **obat tidur** dan pengobatan **gangguan tidur**. Contoh obat-obatan yang termasuk dalam kategori ini berbeda, dengan `N05B` memiliki contoh obat-obatan penenang seperti *benzodiazepin*, sementara `N05C` memiliki obat tidur seperti *zolpidem*.  
  
Kali ini saya akan melihat *"Apakah **penjualan** obat penenang `N05B`* *pada **periode*** ***waktu saat inidipengaruhi*** *oleh penjualan obat tidur `N05C`* *pada **periode waktu sebelumnya?**"* Atau *"Apakah **penjualan** obat tidur `N05C`**periodesebelumnya** memiliki **pengaruh signifikan** terhadap **penjualan** obat penenang `N05B`* *pada **periode*** ***waktu saat ini* ?***.*  

