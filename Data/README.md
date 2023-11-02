## Kendala
Data tidak mencakup hari akhir pekan seperti sabtu dan minggu. Oleh karena itu pada pertemuan 8 kami memutuskan untuk **inputasi** data dengan interplolasi.
Namun ternyata ada website yang menyediakan data harga saham lengkap di [finance.yahoo.com](https://finance.yahoo.com/).
Sehingga daripada inputasi menggunakan program, lebih baik mengambil data sesungguhnya. Pada akhirnya kami memutuskan untuk menggunakan
data saham yang sama, dengan rentang periode dari tahun `2022` hingga `31-Oktober-2023`.  
  
### Folder Data Baru
Adapun data `csv` nya ada di folder [`Full Data`](https://github.com/Zen-Rofiqy/STA1341-MPDW/tree/main/Data/Full%20Data)
  
## Dataset MAANG Stock Prices  
_Notes :_ Data ini hanya digunakan sampai pertemuan 8.  
Link Dataset :  
https://www.kaggle.com/datasets/adityamhaske/maang-stock-prices-july-2018-to-july-2023?resource=download  
  
Dataset ini merupakan koleksi data harga saham historis dari beberapa raksasa teknologi paling berpengaruh di dunia: 
_Microsoft_, _Apple_, _Amazon_, _Nvidia_, _Google_, _Netflix_, dan _Meta_ (sebelumnya dikenal sebagai Facebook). 
Dataset ini menjadi sumber daya berharga bagi analis keuangan, ilmuwan data, dan penggemar pasar saham yang ingin 
menganalisis dan memahami tren harga perusahaan-perusahaan terkemuka di industri ini.  
  
* Jenis periode: Harian  
* Rentang periode `Juli 2018` sampai ` Juli 2023`  
* Variabel :
1. **Open:** yakni Harga saham pada awal periode perdagangan tertentu. 
Ini adalah harga saham pertama pada hari perdagangan tersebut.
2. **High:** Harga tertinggi yang saham capai selama periode perdagangan tersebut. 
Ini mencerminkan harga tertinggi yang pembeli bersedia bayar selama hari tersebut.
3. **Low:** Harga terendah yang saham capai selama periode perdagangan tersebut. 
Ini mencerminkan harga terendah yang penjual bersedia terima selama hari tersebut.
4. **Close:** Harga saham pada akhir periode perdagangan tertentu. 
Ini adalah harga saham terakhir pada hari perdagangan tersebut.
6. **Adj Close (Adjusted Close):** Harga penutup yang telah disesuaikan untuk memperhitungkan perubahan 
seperti pembagian saham atau dividen. Ini adalah harga penutup yang paling relevan untuk analisis jangka panjang, 
karena mencerminkan harga saham yang sebenarnya setelah penyesuaian.
7. **Volume:** Volume perdagangan saham selama periode tertentu. 
Ini mencerminkan jumlah saham yang diperdagangkan selama hari perdagangan tersebut.
