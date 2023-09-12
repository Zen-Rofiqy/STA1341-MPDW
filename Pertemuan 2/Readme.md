## Tujuan
Tujuan praktikum kali ini adalah menangani autokorelasi.  

## Link RPUBS
Agar _memudahkan_ untuk dibaca..  
Daripada liatin rmd nya, mending liat `rpubs` nya.. XD    
Yuk mampir ke :  
https://rpubs.com/ZenR_Prog/MPDW-Prak02  
  
## Tentang Data
Link Data :  
https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data?select=salesmonthly.csv   
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
Obat `M01AB` dan `M01AE` merupakan obat yang sama, namun dengan bahan dasar yang berbeda.  
Saya penasaran _Apakah penjualan obat `M01AB` dipengaruhi oleh penjualan obat `M01AB` dan obat-obat lainnya?_  
Sehingga saya memilih Peubah `M01AB` sebagai peubah respon `Y`. Dan peubah lainnya sebagai peubah penjelas `X`.  
  


