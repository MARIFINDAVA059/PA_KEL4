# PA_KEL4


Program ini adalah simulasi dari sistem kasir dan manajemen kafe bernama "RumahKita CoffeeShop". Program ini memungkinkan pengguna untuk melakukan sejumlah tugas, seperti mendaftarkan pengguna baru, melakukan pemesanan kopi, mengelola stok barang, dan melihat catatan pesanan. Program ini terdiri dari beberapa fungsi dan antarmuka pengguna yang berbeda. Ini adalah panduan singkat tentang cara kerja program:

Menu Utama

Program dimulai dengan tampilan menu utama yang memungkinkan pengguna untuk masuk atau mendaftar.
Mendaftar Pengguna Baru (register_user)

Pengguna baru dapat mendaftar dengan menentukan username, password, peran (cashier, manager, atau customer), dan saldo awal E-money.
Informasi pengguna baru disimpan dalam file CSV 'users.csv'.
Antarmuka Pelanggan (customer_interface)

Pengguna dengan peran 'customer' dapat masuk menggunakan username dan password mereka.
Setelah masuk, pengguna memiliki beberapa opsi:
Melakukan pemesanan kopi.
Melihat menu kafe yang berisi daftar kopi, harga, dan stok.
Mengakhiri pesanan dan melakukan pembayaran menggunakan E-money.
Menyimpan invoice pembelian ke dalam file teks yang dapat diedit.
Pesanan pelanggan dan informasi pengguna disimpan dalam dictionary.
Antarmuka Kasir (cashier_interface)

Pengguna dengan peran 'cashier' dapat masuk menggunakan username dan password mereka.
Setelah masuk, kasir memiliki beberapa opsi:
Melihat pesanan yang ditempatkan oleh pelanggan.
Menandai pesanan sebagai sudah dibayar dan menghapusnya dari daftar pesanan.
Mengupdate stok barang.
Menambahkan kopi baru ke menu.
Antarmuka Manajer (manager_interface)

Pengguna dengan peran 'manager' dapat masuk menggunakan username dan password mereka.
Setelah masuk, manajer memiliki beberapa opsi:
Melihat catatan pesanan yang telah dibayar.
Melihat stok barang.
Mengupdate pesanan pelanggan.
Tugas-tugas Tambahan

Program memiliki fungsi untuk memuat dan menyimpan data pengguna, menu kopi, dan stok barang dari dan ke file CSV.
Fungsi-fungsi ini memungkinkan program untuk menjaga konsistensi data antar-sesi.
Fungsi dan Operasi Lainnya

Ada berbagai fungsi untuk menampilkan data dalam format yang rapi menggunakan library "PrettyTable".
Fungsi "generate_invoice" digunakan untuk menghasilkan invoice pembelian.
Terdapat juga validasi input untuk memastikan data yang dimasukkan sesuai dengan aturan yang ada.
Program ini memungkinkan pengguna untuk berinteraksi dengan sistem sebagai pelanggan, kasir, atau manajer dengan batasan peran yang sesuai. Seluruh data pengguna, pesanan pelanggan, menu kopi, dan stok barang disimpan dalam file CSV untuk menjaga integritas data antar-sesi.

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/26df85f9-7376-468e-a39a-cffe79b9187c)
Tampilan Menu awal

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/11d8b619-2eeb-47e9-8fd8-24282f7d3c00)
Ketika user memilih opsi 2 : register
akan diminta 4 input
username
password
role
jumlah e money
ketika berhasil akan tersimpan ke users.csv

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/dd9b4b6b-6e20-4492-8593-32239260dfa4)
ketika username sudah ada

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/c80acd24-a472-4d55-816b-4caeb52ecbd8)
ketika input tidak sesuai role

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/c18dddcb-70f9-4551-b1b1-a4ade185fbd7)
Ketika user memilih opsi 1 : login
akan muncul pilihan role untuk dijalankan

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/4d48da9a-0c81-40f1-850c-ce6ad05a2053)
ketika user memilih opsi 1 : customer
akan diminta login dan mengisi password
jika user menginput "X" maka akan langsung kembali ke menu pemilihan role

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/86cc5790-20a6-4c9f-b8fc-0b199cd86907)
Ketika user memilih opsi 1 : order coffee
akan muncul menu coffee beserta harga dan stok yang ada
user dapat menginput nama coffee yg ingin diorder ( huruf Kapital harus sesuai )

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/eb7389cd-b001-42b3-9131-204b09e2a935)
Setelah user menginput coffee, akan diminta jumlah coffee yang ingin dipesan kemudian akan kembali menampilkan menu kembali serta total bill sementara... 
jika customer ingin mengoder lagi maka perlu memasukkan nama dan jumlah coffee..
namun jika customer sudah selesai dalam mengorder, maka dapat menginput "X"

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/32cd0346-d1c7-4fea-9b3f-e67c7833b51a)
Ketika user menginput "X" maka akan keluar total bill dan juga total bill
user diminta menginput e money untuk membayar ( jumlah harus lebih dari total bill )

kemudian akan tampil invoice dengan detail waktu transaksi, nama, jumlah dan harga coffee,total bill, total uang yang dibayar, dan uang kembalian )
dan kembali ke menu tampilan awal customer

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/0b85ec0f-5ae0-45bd-863a-df71599bc10b)
Ketika user menginput 2 maka akan muncul menu dengan fitur (sorting) yaitu menu yang sudah diurutkan berdasarkan harga terendah dari atas ke bawah

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/60796b1b-3927-47ca-898f-d1d14eadc4e7)
Ketika user menginput 3 maka akan keluar dari bagian customer dan ke menu login.. user dapat menginput "X" jika ingin keluar dari menu login dan menuju pemilihan role

![image](https://github.com/MARIFINDAVA059/PA_KEL4/assets/147223413/fa97844a-aebe-41f2-9bc9-f1c51ac2646b)
Ketika user menginput 2 maka akan ke menu cashier dan diminta untuk login username dan password
Kemudian jika user menginput 1 untuk melihat order maka akan muncul tampilan orderan yang sudah ada









