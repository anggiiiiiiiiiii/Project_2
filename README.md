# Project2
**Sekilas mengenai NYC TLC Record**
Apa itu NYC TLC? 
NYC TLC adalah singkatan dari (New York CIty Taxi Limousin Comission) yang merupakan sebuah badan pemerintah Kota New York yang memberi lisensi dan mengatur taksi medali dan industri kendaraan sewaan , termasuk perusahaan berbasis aplikasi seperti Uber dan Lyft. Lembaga ini telah merekam kegiatan para pengemudi taksi atau limusin selama tiga puluh hari. Dengan adanya rekaman data ini, kita bisa mengetahui lokasi dengan ID mana saja yang sering terjadi kemacetan dan bagaimana pola atau kebiasaan dari kebanyakan penumpang.
# Cleaning Data
Kebanyakan dari data kosong yang ada diisi dengan nilai mediannya, tidak menggunakan mean karena data yang ada belum tentu terdistribusi normal. Juga karena proporsi dari nilai kosong tersebut tergolong kecil yakni dibawah 30% dari total keseluruhan data. Kalaupun terdapat data yang bernilai kosong dan proporsinya di atas 30% maka akan saya bagi menjadi beberapa bagian, salah satunya untuk dianalisis (maka NaN nya akan dihapus), sementara yang lainnya dibiarkan memiliki nilai kosong (selagi nilai kosong itu tidak memengaruhi nilai data yang akan dianalisis). Namun untungnya pada data kali ini tak ada kasus seperti yang dijelaskan diatas, Jikalaupun ada nilai NaN yang lebih besar dari 30% maka nilai NaN-nya itu memiliki proporsi 100% alias seluruh kolomnya bernilai kosong (yang memungkinkan saya untuk langsung menghapus kolomnya sekaligus)
Data yang sudah saya cleaning adalah file csv dengan nama: **data_bersih.csv**
# Analisis
Analisis yang dilakukan cenderung pada pengelompokan data berdasarkan point Estimation yang kemudian dibuat grafiknya. Contohnya pada salah satu code yang saya buat yaitu pengelompokan rata-rata jumlah penumpang tiap harinya dalam tiga puluh hari dan setelahnya dibuat grafik lineplotnya.
# Stakeholder
**Stakeholder dari data ini diantaranya:**
- Riders(Pengemudi)
- Fleet Manager/ Owner NYC TLC (Pemilik)
- NYC Departement of Transportation (Departemen Transportasi NYC)
# Insight
**Informasi yang didapat:**
- Kemacetan terjadi pada lokasi ID 65, ID 33, dan ID 97 karena tiap kali taksi menjemput atau mengantarkan penumpang pada ketiga lokasi tersebut selalu terjadi perlambatan durasi mengantar untuk satu mil perjalanan.
- Tipe tarif JFK adalah tipe tarif dengan rata-rata total pembayaran paling tinggi
- Terdapat korelasi hubungan searah antara durasi, tip dan tarif. Namun tidak dengan pajak
- PickUp lokasi tertinggi ada pada lokasi ID 74, disusul ID 75 dan ID 166
**Insight:**
- Bagi Fleet/Manager Owner dari NYC TLC penggunaan Credit Card diantara penumpang adalah yang paling besar, begitu juga dengan total rata-rata tarifnya, juga selalu ada peningkatan customer di hari kamis dan jumat mungkin saja bisa dilakukan strategi penetapan harga di kedua hari tersebut bagi yang menggunakan Credit Card. Misalnya harga tarif dinaikan khusus kedua hari sibuk itu bagi pengguna kartu kredit. Karena semakin besar total tarif yang didapatkan tidak berpengaruh pada besar pajak yang harus dibayarkan, maka dari itu adanya kenaikan tarif tidak akan menjadi masalah. 
- Bagi Fleet/Manager Owner dari NYC TLC perlu penyesuaian strategi harga untuk tipe tarif group rate karena sangat rendah jika dibandingkan dengan tipe tarif lainnya. Penyesuaian harga yang dimaksud disini adalah di adakannya diskon bagi pengguna tipe tarif group rate.
- Bagi NYC Departement Transportation, terdapat beberapa lokasi kemacetan yang ditemukan dari data, ketiga paling tinggi diantaranya lokasi dengan ID 97, 66 dan 33 sepertinya masih diperlukan peningkatan infrastruktur atau rekayasa lalu lintas di ketiga lokasi tersebut.
- Untuk Riders/Commuter disarankan untuk menetap pada lokasi ID 74, 75 dan 166 karena total penumpang yang di jemput dari ketiga lokasi tersebut sangat tinggi.
