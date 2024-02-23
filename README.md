# Python Project Pacman - Super Cashier

## **Latar Belakang Problems**
Andi adalah seorang pemilik supermarket besar di salah satu Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Andi akan membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, jumlah item yang dibeli, dan harga item yang dibeli dan fitur yang lain.

Sehingga customer yang tidak berada di kota tersebut bisa membeli barang dari supermarket tersebut. 
Setelah Andi melakukan riset, ternyata Andi memiliki masalah, yaitu Andi membutuhkan Programmer untuk membuatkan fitur-fitur agar bisa sistem kasir self-service di supermarket itu bisa berjalan dengan lancar.

## **Requirements & Objectives**
### Requirements
a) Customer memasukkan nama item, jumlah item, harga item

b) Kemudian customer dapat melakukan pengecekan barang belanja dengan menggunakan method check_order() 
  - Jika transaksi sudah benar, tampilkan "Transaksi Sudah Benar"
  - Jika terdapat kesalahan input, maka tampilkan "Terdapat Kesalahan Dalam Input Data"

c) Customer dapat memperbarui detail item (nama, jumlah, atau harga) jika terdapat kesalahan dalam input:
  - Perbarui nama item menggunakan `update_item_name()`
  - Perbarui jumlah item menggunakan `update_item_qty()`
  - Perbarui harga item menggunakan `update_item_price()`

d) Customer dapat membatalkan transaksi:
  - Hapus barang tertentu menggunakan method `delete_item(<nama_item>)`
  - Reset semua transaksi menggunakan methode `reset_transaction()`

e) Setelah melakukan pengecekan, customer dapat menghitung total pembelian menggunakan `total_harga_akhir()`. Sistem menerapkan aturan diskon sebagai berikut:
  - Diskon 5% untuk pembelian di atas Rp 200.000
  - Diskon 8% untuk pembelian di atas Rp 300.000
  - Diskon 10% untuk pembelian di atas Rp 500.000

### Objectives
Proyek ini bertujuan untuk mengembangkan sistem kasir supermarket dengan alur kerja sebagai berikut:

a) Customer memasukkan nama item, jumlah item, dan harga per item

b) Customer dapat memeriksa pesanan mereka untuk memastikan apakah inputan sudah benar atau belum
   - Tampilkan "Transaksi sudah benar" jika tidak ada kesalahan input.
   - Tampilkan "Terdapat Kesalahan Dalam Input Data" jika terdapat kesalahan input.
   - Tampilkan tabel yang berisi semua data pesanan.

c) Jika terdapat kesalahan input, customer dapat memperbarui data item:
  - Perbarui nama item
  - Perbarui jumlah item
  - Perbarui harga item
    
d) Customer dapat membatalkan pembelian barang:
  - Hapus 1 baris item
  - Reset semua transaksi.
    
e) Customer dapat menghitung total pembelian dan diskon sesuai dengan aturan yang ditetapkan

## **Flowchart**
![Flowchart - Supermarket Andi](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Flowchart%20-%20Supermarket%20Andi.jpeg)

### Penjelasan Alur Code

## **Functions**
* `add_item()` : digunakan untuk menambahkan item ke dalam item transaksi. Parameter `nama_item`, `jumlah_item`, `harga_item`
* `chek_order()` : digunakan untuk memeriksa apakah transaksi sudah benar atau terdapat kesalahan dalam melakukan input data
* `chek_items()` :  digunakan untuk menampilkan daftar item dalam transaksi menggunakan tabulate
* `update_item_name()` : digunakan untuk mengganti nama item pada daftar transaksi dari nama lama menjadi nama baru. Parameter `old_name` yaitu nama item lama yang ingin diganti , `new_name` adalah nama item baru
* `update_item_qty()` : digunakan untuk memperbarui jumlah item dalam transaksi. Parameter `name` adalah nama item yang jumlahnya ingin diganti, `new_qty` adalah jumlah item baru
* `update_item_price()` : digunakan untuk memperbarui harga per item dalam transaksi. Parameter `name` adalah nama item yang jumlahnya ingin diganti,`new_price` adalah harga item baru
* `delete_item()`: digunakan untuk menghapus 1 baris item yang ada di list_item. Parameter `nama_item` adalah nama item yang ingin dihapus
* `reset_transaction()` : digunakan untuk mereset transaksi dengan mengosongkan daftar item
* `total_price()`: digunakan untuk menghitung total harga pembelian dan diskon yang didapat

## **Test Case**
#### Testing 1 add item
![Test Case 1](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%201.JPG)

#### Testing 2 Delete items
![Test Case 2](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%202.JPG)

#### Testing 3 Reset Transaction
![Test Case 3](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%203.JPG)

#### Testing 4 Check Order
![Test Case 4](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%204.JPG)

#### Testing 5 Menghitung Total yang harus dibayar
![Test Case 5](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%205.JPG)

#### Testing 6 Update Item Name
![Test Case 6](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%206.JPG)

#### Testing 7 Update Item Jumlah
![Test Case 7](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%207.JPG)

#### # Testing 8 Update Item Harga
![Test Case 8](https://github.com/safaarub/Python-Project-Pacman---Super-Cashier-/blob/main/images/Test%20Case%208.JPG)

## **Saran Perbaikan**
