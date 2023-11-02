# PA_KEL4


rogram ini adalah simulasi dari sistem kasir dan manajemen kafe bernama "RumahKita CoffeeShop". Program ini memungkinkan pengguna untuk melakukan sejumlah tugas, seperti mendaftarkan pengguna baru, melakukan pemesanan kopi, mengelola stok barang, dan melihat catatan pesanan. Program ini terdiri dari beberapa fungsi dan antarmuka pengguna yang berbeda. Ini adalah panduan singkat tentang cara kerja program:

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
