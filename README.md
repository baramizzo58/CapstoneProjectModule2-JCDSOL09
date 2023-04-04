# CapstoneProjectModule2-JCDSOL09
Capstone Project Module 2 - Noor Kharismawan Akbar

# Background
**`Customer Personality Analysis`** adalah dataset pelanggan di suatu perusahaan yang terletak di USA pada tahun 2012-2014. Perusahaan ini menjual berbagai jenis produk seperti wine, buah, daging, ikan, manisan/permen, dan emas. Perusahaan ini juga membuka marketplace pada beberapa opsi seperti web, katalog, dan toko. Perusahaan ini juga telah berkali-kali melakukan campaign dan memberi diskon. Namun, tidak semua tawaran campaign diterima pelanggan & tidak semua diskon dapat menarik pembeli yang dapat menjadi customer loyal.

# Problem Statement
Perusahan ingin mengetahui customer mana yang memberikan profit yang banyak ke perusahaan. Kemudian juga ingin diketahui customer mana yang cenderung menerima tawaran campaign. Informasi ini akan digunakan perusahaan untuk membantu melakukan efisiensi dalam biaya, waktu, dan tenaga dalam promosi & campaign. Analisis ini dapat membantu bisnis untuk memodifikasi marketplace, produk, dan campaign berdasarkan target pelanggannya dari berbagai jenis segmen.

Pada analisis ini, akan dijawab pertanyaan yang secara garis besar sebagai berikut:<br>
* Bagaimana **kinerja penjualan produk** saat ini? 
Barang apa yang paling sering dibeli dan memberikan pemasukan yang banyak bagi perusahaan, serta melalui apa mereka membelinya?
* Bagaimana **kinerja marketing campaign** saat ini?
Bagaimana juga karakteristik customer yang menerima tawaran campaign, terutama dibandingkan customer yang menolak?
* Bagaimana juga **karakteristik customer** saat ini & customer terbaik (yang baru-baru membeli, paling sering, dan merupakan pembelanja berat)?

# Data
Untuk menyelesaikan permasalahan ini, Digunakan dataset `marketing_campaign.csv` yang berasal dari proyek **Dr. Omar Romero-Hernandez**. Dataset ini dapat diunduh [di laman ini](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
**Column Description**:
* People
    * ID: ID unik pelanggan
    * Year_Birth: Tahun lahir pelanggan
    * Education: Tingkat pendidikan pelanggan
    * Marital_Status: Status perkawinan pelanggan
    * Income: Pendapatan rumah tangga tahunan pelanggan
    * Kidhome: Jumlah anak dalam rumah tangga pelanggan
    * Teenhome: Jumlah remaja dalam rumah tangga pelanggan
    * Dt_Customer: Tanggal pendaftaran pelanggan dengan perusahaan
    * Recency: Jumlah hari sejak pembelian terakhir pelanggan
    * Complain: 1 jika pelanggan melakukan komplain dalam 2 tahun terakhir, 0 jika tidak
* Product
    * MntWines: Amount spent untuk wine dalam 2 tahun terakhir
    * MntFruits: Amount spent untuk buah-buahan dalam 2 tahun terakhir
    * MntMeatProducts: Amount spent untuk daging dalam 2 tahun terakhir
    * MntFishProducts: Amount spent untuk membeli ikan dalam 2 tahun terakhir
    * MntSweetProducts: Amount spent untuk permen dalam 2 tahun terakhir
    * MntGoldProds: Amount spent untuk emas dalam 2 tahun terakhir
* Promotion
    * NumDealsPurchases: Jumlah pembelian yang dilakukan dengan diskon
    * AcceptedCmp1: 1 jika pelanggan menerima penawaran di campaign pertama, 0 jika tidak
    * AcceptedCmp2: 1 jika pelanggan menerima penawaran di campaign ke-2, 0 jika tidak
    * AcceptedCmp3: 1 jika pelanggan menerima penawaran di campaign ke-3, 0 jika tidak
    * AcceptedCmp4: 1 jika pelanggan menerima penawaran di campaign ke-4, 0 jika tidak
    * AcceptedCmp5: 1 jika pelanggan menerima penawaran di campaign ke-5, 0 jika tidak
    * Response: 1 jika pelanggan menerima tawaran di campaign terakhir, 0 jika tidak
* Place
    * NumWebPurchases: Jumlah pembelian yang dilakukan melalui situs web perusahaan
    * NumCatalogPurchases: Jumlah pembelian yang dilakukan menggunakan katalog
    * NumStorePurchases: Jumlah pembelian yang dilakukan langsung di toko
    * NumWebVisitsMonth: Jumlah kunjungan ke website perusahaan dalam sebulan terakhir
    
# Analisis
Dapat dilihat di file ipynb & ppt.

# Kesimpulan
Dari analisis yang telah dilakukan, akhirnya didapatkan jawaban atas problem yang dinyatakan sebelumnya yang tertuang pada poin-poin berikut:
1. Kinerja penjualan:
    * Semakin **tinggi pendapatan** dan semakin **sedikit keturunan** yang dimiliki customer, mereka lebih cenderung membeli **banyak produk** dan lebih **sering berbelanja**.
    * **Wine** & **Meat** merupakan produk yang paling **sering dibeli** & memberikan **pemasukan paling banyak** pada perusahaan kita. Sementara itu
    * Customer cenderung lebih **sering berbelanja langsung di toko**, namun amount spent nya lebih besar ketika berbelanja menggunakan **katalog**.
    * Jika dilihat dari **frekuensi pembelian** & **jumlah spent** nya, customer dengan pendidikan **`PhD`** memiliki total terbanyak, namun proporsi orang yang berpendidikan tinggi dalam dataset ini masih yang terrendah.
    * **Jumlah pendaftar** (customer baru) semakin **lama** semakin **sedikit**.<br><br>

2. Kinerja Marketing Campaign:
    * Customer yang **menerima penawaran** campaign lebih banyak untuk produk **Wine** & **Meat**, kemudian untuk pembelian menggunakan **katalog**. Pembelian melalui situs web lebih menarik customer ketika ada **diskon**.
    * Customer kebanyakan **menerima tawaran** campaign yang **terakhir**.
    * Customer yang cenderung menerima penawaran campaign berasal dari segmen pendapatan yang **tinggi** ($51,939 - $105,900), **hidup sendiri** (Single, Widow, Divorced), **tidak punya anak**, dan education **`PhD`**.
    * Acceptance rate campaign menunjukkan tren yang **menurun sejak Oktober 2012** hingga masa akhir campaign.<br><br>

3. Karakteristik Customer:
    * Berdasarkan analisis **RFM**, saat ini hampir **sepertiga** dari total customer sudah **lama tidak melakukan pembelian** dan **bukan** customer yang **sering sekali berbelanja**. Segmen ini perlu diberi approach dengan cara tertentu agar lebih sering menggunakan produk kita.
    * Berdasarkan analisis **RFM** juga, Customer yang **belum lama melakukan pembelian** & **sering melakukan pembelian** kebanyakan berusia **35-65 tahun** yang hidup **bersama pasangan** yang memiliki **0-1 anak**. Kebanyakan juga merupakah seorang yang sedang menempuh pendidikan atau sudah lulus **sarjana** dengan income **$51,939 - $105,900**.

# Rekomendasi
1. Melakukan **marketing campaign** di lokasi strategis yang banyak dikunjungi oleh orang berpendidikan tinggi seperti di dekat tempat **penelitian** & **Instansi pendidikan**.
2. **Jangan terlalu memandang status pernikahan** dalam targetting customer, cukup ditinjau secara umum saja apakah customer tersebut hidup sendiri atau bersama.
3. Memberikan promo berupa **paket bundling** untuk produk **Wine** & **Meat** karena dua produk itu yang paling berpengaruh pada total spent. Kemudian bisa ditambahkan promo juga untuk pembelian pada **Katalog**.
4. Sebagian besar customer sudah jarang berbelanja di market kita, sehingga perlu adanya approach dan penawaran yang membuat customer segera membeli produk kita. Contohnya dengan **Limited Time Offers**.
5. Untuk pengambilan data selanjutnya, alangkah baiknya jika diberi **keterangan rinci** mengenai **campaign** yang dilakukan agar bisa dilakukan analisis lebih dalam menggunakan [**RICE Framework**](https://www.productplan.com/glossary/rice-scoring-model/).
