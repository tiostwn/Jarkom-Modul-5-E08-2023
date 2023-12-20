# Jarkom-Modul-5-E08-2023
Laporan Resmi Praktimum 3 JARKOM

**Anggota Kelompok `E08` `192.210`** 
| Nama | NRP |
| --- | --- |
| Hanafi Satriyo Utomo Setiawan | 5025211195 |
| Samuel Berkat Hulu | 5025201055 |


## Topologi
![Screenshot 2023-12-20 at 01 42 58](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/d04c3051-0b16-4927-81eb-b0d8f07db49e)

## Subnet 
![E08 - Subnet](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/a3e9c66a-692d-47a2-8781-7ffee6aaa6a9)

## Rute
<table><thead><tr><th>Nama Subnet</th><th>Rute</th><th>Jumlah IP</th><th>Netmask</th></tr></thead><tbody><tr><td>A1</td><td>router(Fern)-server(Revolte)</td><td>2</td><td>/30</td></tr><tr><td>A2</td><td>router(Fern)-server(Richter)</td><td>2</td><td>/30</td></tr><tr><td>A3</td><td>router(Himmel)-router(Fern)-pc(SchwerMountain)</td><td>66</td><td>/25</td></tr><tr><td>A4</td><td>router(Himmel)-pc(LaubHills)</td><td>256</td><td>/23</td></tr><tr><td>A5</td><td>router(Frieren)-router(Himmel)</td><td>2</td><td>/30</td></tr><tr><td>A6</td><td>router(Frieren)-server(Stark)</td><td>2</td><td>/30</td></tr><tr><td>A7</td><td>router(Aura)-router(Frieren)</td><td>2</td><td>/30</td></tr><tr><td>A8</td><td>router(Aura)-router(Heiter)</td><td>2</td><td>/30</td></tr><tr><td>A9</td><td>router(Heiter)-pc(TurkRegion)</td><td>1023</td><td>/21</td></tr><tr><td>A10</td><td>router(Heiter)-server(Sein)-pc(GrobeForest)</td><td>514</td><td>/22</td></tr><tr><td>Total</td><td></td><td>1871</td><td>/20</td></tr></tbody></table>

## VLSM Tree
![Jarkom Modul 4 - Frame 2](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/2fd8e948-9ca3-43fe-abf0-6263a37e7f38)

## Pembagian IP
<table><thead><tr><th>Subnet</th><th>Node</th><th>IP</th><th>Netmask</th><th>Length</th><th>NID</th><th>Broadcast</th></tr></thead><tbody><tr><td rowspan="2">A1</td><td>Fern</td><td>192.210.0.1</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.0</td><td rowspan="2">192.210.0.3</td></tr><tr><td>Revolte</td><td>192.210.0.2</td></tr><tr><td rowspan="2">A2</td><td>Fern</td><td>192.210.0.5</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.4</td><td rowspan="2">192.210.0.7</td></tr><tr><td>Richter</td><td>192.210.0.6</td></tr><tr><td rowspan="3">A3</td><td>Himmel</td><td>192.210.0.129</td><td rowspan="3">255.255.255.128</td><td rowspan="3">25</td><td rowspan="3">192.210.0.128</td><td rowspan="3">192.210.0.255</td></tr><tr><td>Fern</td><td>192.210.0.130</td></tr><tr><td>SchwerMountain</td><td>DHCP</td></tr><tr><td rowspan="2">A4</td><td>Himmel</td><td>192.210.2.1</td><td rowspan="2">255.255.254.0</td><td rowspan="2">23</td><td rowspan="2">192.210.2.0</td><td rowspan="2">192.210.3.255</td></tr><tr><td>LaubHills</td><td>DHCP</td></tr><tr><td rowspan="2">A5</td><td>Frieren</td><td>192.210.0.9</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.8</td><td rowspan="2">192.210.0.11</td></tr><tr><td>Himmel</td><td>192.210.0.10</td></tr><tr><td rowspan="2">A6</td><td>Frieren</td><td>192.210.0.13</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.12</td><td rowspan="2">192.210.0.15</td></tr><tr><td>Stark</td><td>192.210.0.14</td></tr><tr><td rowspan="2">A7</td><td>Aura</td><td>192.210.0.17</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.16</td><td rowspan="2">192.210.0.19</td></tr><tr><td>Frieren</td><td>192.210.0.18</td></tr><tr><td rowspan="2">A8</td><td>Aura</td><td>192.210.0.21</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.20</td><td rowspan="2">192.210.0.23</td></tr><tr><td>Heiter</td><td>192.210.0.22</td></tr><tr><td rowspan="2">A9</td><td>Heiter</td><td>192.210.8.1</td><td rowspan="2">255.255.248.0</td><td rowspan="2">21</td><td rowspan="2">192.210.8.0</td><td rowspan="2">192.210.15.255</td></tr><tr><td>TurkRegion</td><td>DHCP</td></tr><tr><td rowspan="3">A10</td><td>Heiter</td><td>192.210.4.1</td><td rowspan="3">255.255.252.0</td><td rowspan="3">22</td><td rowspan="3">192.210.4.0</td><td rowspan="3">192.210.7.255</td></tr><tr><td>Sein</td><td>192.210.4.2</td></tr><tr><td>GrobeForest</td><td>DHCP</td></tr></tbody></table>

## Soal

### Soal 1

Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi Aura menggunakan iptables, tetapi tidak ingin menggunakan MASQUERADE.

### Solusi

Pada node **Aura**, kita akan mengkonfigurasi iptables dengan perintah

```bash
iptables -t nat -A POSTROUTING -s 192.210.0.0/20 -o eth0 -j SNAT --to-source 192.168.122.1
```

- `-t nat` adalah opsi untuk menambahkan rule pada tabel nat
- `-A POSTROUTING` adalah opsi untuk menambahkan rule pada chain POSTROUTING
- `-s` adalah opsi untuk menentukan source IP
- `-o` adalah opsi untuk menentukan interface
- `-j SNAT` adalah opsi untuk melakukan SNAT
- `--to-source` adalah opsi untuk menentukan IP yang akan digunakan untuk SNAT

### Testing

Pada node **GrobeForest**, kita akan melakukan ping ke google.com dengan perintah

```bash
ping google.com
```

![image](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/19e04f7c-b816-4e9c-82f2-62d201b99b49)

### Soal 2

Kalian diminta untuk melakukan drop semua TCP dan UDP kecuali port 8080 pada TCP.

### Solusi

Untuk melakukan drop semua TCP dan UDP kecuali port 8080 pada TCP, kita akan mengkonfigurasi iptables pada node **SchewerMountain** dengan perintah

```bash

iptables -A INPUT -p tcp --dport 8080 -j ACCEPT
iptables -A INPUT -p tcp ! --dport 8080 -j DROP
iptables -A INPUT -p udp -j DROP
```

- `iptables -F` adalah opsi untuk menghapus semua rule yang ada

- `iptables -A INPUT -p tcp --dport 8080 -j ACCEPT` adalah opsi untuk menambahkan rule pada chain INPUT untuk menerima koneksi TCP pada port 8080

- `iptables -A INPUT -p tcp ! --dport 8080 -j DROP` adalah opsi untuk menambahkan rule pada chain INPUT untuk menolak koneksi TCP yang tidak menuju ke port 8080

### Testing

Disini akan dilakukan testing terhadap `client` yang akan menuju `Revolte` dengan bantuan netcat
![Screenshot 2023-12-20 at 02 17 13](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/56a2e9b3-1769-431f-b922-69e1a60b4ca0)
![Screenshot 2023-12-20 at 02 19 22](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/45e7ff90-9274-42a2-840a-af9200d7a3bc)
![Screenshot 2023-12-20 at 02 17 44](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/e1dde01d-c002-4a88-8b47-5c01586a6279)

### Soal 3

Kepala Suku North Area meminta kalian untuk membatasi DHCP dan DNS Server hanya dapat dilakukan ping oleh maksimal 3 device secara bersamaan, selebihnya akan di drop.

### Solusi

Untuk membatasi DHCP dan DNS Server hanya dapat dilakukan ping oleh maksimal 3 device secara bersamaan, kita akan mengkonfigurasi iptables pada node **Revolte** dan **Richter** dengan perintah

```bash
iptables -A INPUT -p icmp -m connlimit --connlimit-above 3 --connlimit-mask 0 -j DROP
```

- `iptables -A INPUT -p icmp -m connlimit --connlimit-above 3 --connlimit-mask 0 -j DROP` adalah opsi untuk menambahkan rule pada chain INPUT untuk menolak koneksi ICMP yang lebih dari 3
- `--connlimit-above 3` adalah opsi untuk menentukan batas koneksi
- `--connlimit-mask 0` adalah opsi untuk menentukan mask

### Testing

Untuk melakukan testing, kita akan menggunakan node **Revolte** dan **Richter**. Untuk membuat perbandingan antara koneksi yang belum di batasi dan koneksi yang sudah di batasi, kita akan menggunakan netcat pada node **Revolte** dan **Richter** dengan perintah

- Testing pada node **Richter** (belum dijalankan iptables / rule nya)

https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/64a1e490-cd31-404a-9b1a-b6cb75abe72d

- Testing pada node **Revolte**
  
https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/b31ef5b3-178f-4638-aa3a-6c6616978671

Pada `TurkRegion` tidak berhasil melakukan ping karena `Revolte` sudah mencapai 3 koneksi.

### Soal 4

Lakukan pembatasan sehingga koneksi SSH pada Web Server hanya dapat dilakukan oleh masyarakat yang berada pada GrobeForest.

### Solusi

Untuk melakukan pembatasan koneksi SSH pada Web Server hanya dapat dilakukan oleh masyarakat yang berada pada GrobeForest, kita akan mengkonfigurasi iptables pada node **Sein** dan **Stark** dengan perintah

```bash
# Soal No 4
iptables -A INPUT -p tcp --dport 22 -s 192.210.4.0/22 -j ACCEPT
iptables -A INPUT -p tcp --dport 22 -j DROP
```

- -s `192.210.4.0/22` adalah opsi untuk menentukan source IP yang diizinkan pada kali ini adalah subnet `192.210.4.0/22` yaitu di block A10 yang merupakan GrobeForest
- `iptables -A INPUT -p tcp --dport 22 -j DROP` adalah opsi untuk menambahkan rule pada chain INPUT untuk menolak koneksi TCP pada port 22 yang tidak berasal dari subnet A10

Jadi, aturan ini memungkinkan lalu lintas TCP yang menuju ke port 22 (SSH) dari alamat IP yang dimulai dengan 192.210.x.x untuk diterima. aturan ini menolak semua lalu lintas TCP yang menuju ke port 22 (SSH). Ini bertentangan dengan aturan sebelumnya yang mengizinkan lalu lintas SSH dari alamat IP tertentu. Oleh karena itu, aturan ini bersifat "penolakan umum" untuk lalu lintas SSH yang tidak sesuai dengan aturan pertama.

### Testing

#### Testing pada `TurkRegion`
![Screenshot 2023-12-20 at 17 38 04](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/2a895a5c-234e-4d81-a34a-0a940f9e287b)

#### Testing pada `GrobeForest` 
![Screenshot 2023-12-20 at 17 39 15](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/976e2e64-b18b-432e-ae27-fa10b860a793)

## Soal 5

Selain itu, akses menuju WebServer hanya diperbolehkan saat jam kerja yaitu Senin-Jumat pada pukul 08.00-16.00.

### Solusi 
Karena disini akan Webserver hanya dapat diakses pada jam kerja saja, dapat menggunakan bantuan ``time`` dan lebih spesifiknya membutuhkan command ``--weekdays`` untuk membaca hari masuk (Senin, Selasa, Rabu, Kamis, Jumat). Kita juga perlu untuk menggunakan ``timestart`` dan ``timeout`` untuk membatasi akses.

```sh
iptables -A INPUT -m time --timestart 08:00 --timestop 16:00 --weekdays Mon,Tue,Wed,Thu,Fri -j ACCEPT
iptables -A INPUT -j REJECT
```

**Penjelasan**

- ``-A INPUT``: Menambahkan aturan ke chain INPUT (rantai yang digunakan untuk lalu lintas yang menuju ke sistem).
- ``-m time``: Menggunakan modul waktu untuk menentukan aturan berdasarkan waktu.
- ``--timestart 08:00``: Menentukan waktu mulai, dalam hal ini pukul 08:00.
- ``--timestop 16:00``: Menentukan waktu berakhir, dalam hal ini pukul 16:00.
- ``--weekdays Mon,Tue,Wed,Thu,Fri``: Menentukan hari-hari di mana aturan ini berlaku, dalam hal ini Senin sampai Jumat.
- ``-j ACCEPT``: Menentukan tindakan yang diambil jika paket memenuhi kriteria aturan, dalam hal ini menerima paket.
- ``-j REJECT``: Menentukan tindakan yang diambil jika paket tidak memenuhi kriteria aturan, dalam hal ini menolak (REJECT) paket.

Jadi, aturan ini memungkinkan lalu lintas masuk (INPUT) hanya pada rentang waktu antara pukul 08:00 hingga 16:00 pada hari Senin sampai Jumat. Aturan ini juga menolak semua lalu lintas yang tidak sesuai dengan aturan sebelumnya. Ini termasuk lalu lintas di luar rentang waktu atau pada hari yang tidak termasuk dalam Senin sampai Jumat.

### Testing
**Note**: Jika jam / hari berbeda dengan rentang waktu yang telah di ``set`` sebelumnya, maka gunakan ``date --set="2023-12-13 14:00:00"``

**Sukses**

![Screenshot 2023-12-20 at 17 55 12](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/e147f455-c6d6-41c4-ab01-7391d45272c4)

**Gagal**

![Screenshot 2023-12-20 at 17 54 31](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/5c3e9992-2ae2-4042-a608-70340eb1203b)

## Soal 6
Lalu, karena ternyata terdapat beberapa waktu di mana network administrator dari WebServer tidak bisa stand by, sehingga perlu ditambahkan rule bahwa akses pada hari Senin - Kamis pada jam 12.00 - 13.00 dilarang (istirahat maksi cuy) dan akses di hari Jumat pada jam 11.00 - 13.00 juga dilarang (maklum, Jumatan rek).

### Solusi
Untuk membatasi waktu koneksi, ``iptables`` pada Web Server (Sein dan Stark) perlu dilakukan pendefinisian pada hari yang dapat terkoneksi atau dapat di ``drop``. Karena disini kita akan melakukan ``blok`` pada jam istirahat *weekdays* pada hari ``Senin - Kamis`` pukul ``12.00 - 13.00`` dan ``11.00 - 13.00`` pada hari ``jum'at``. Dapat menggunakan command sebagai berikut

```sh 
# Menolak akses pada Senin-Kamis pada jam 12.00-13.00
iptables -A INPUT -m time --weekdays Mon,Tue,Wed,Thu --timestart 12:00 --timestop 13:00 -j REJECT

# Menolak akses pada Jumat pada jam 11.00-13.00
iptables -A INPUT -m time --weekdays Fri --timestart 11:00 --timestop 13:00 -j REJECT
```

- ``-m time``: Menggunakan modul waktu untuk menentukan aturan berdasarkan waktu.
- ``--timestart 12:00``: Menentukan waktu mulai, dalam hal ini pukul 12:00.
- ``--timestop 13:00``: Menentukan waktu berakhir, dalam hal ini pukul 13:00.
- ``--weekdays Mon,Tue,Wed,Thu``: Menentukan hari-hari di mana aturan ini berlaku, dalam hal ini Senin sampai Kamis.
- ``--timestart 11:00``: Menentukan waktu mulai, dalam hal ini pukul 11:00.
- ``--timestop 13:00``: Menentukan waktu berakhir, dalam hal ini pukul 13:00.
- ``--weekdays Fri``: Menentukan hari di mana aturan ini berlaku, dalam hal ini Jumat.
- ``-j REJECT``: Menentukan tindakan yang diambil jika paket memenuhi kriteria aturan, dalam hal ini menolak (REJECT) paket.

Jadi, aturan ini menolak lalu lintas INPUT pada hari Senin sampai Kamis antara pukul 12:00 dan 13:00. Aturan ini juga menolak lalu lintas INPUT pada hari Jumat antara pukul 11:00 dan 13:00.

### Testing
Pada testing kali ini kami akan mencoba untuk melakukan pada waktu yang telah ditentukan (Gagal) dan waktu yang ``available`` untuk mengakses ``Web Server``

**Sukses**

![Screenshot 2023-12-20 at 18 09 45](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/92527b84-aae9-44bb-898c-738ad427ff43)

**Gagal**

![Screenshot 2023-12-20 at 18 09 24](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/b59589f8-1fff-4c2a-a4f1-57bb4e468cb2)

## Soal 8
> Karena berbeda koalisi politik, maka subnet dengan masyarakat yang berada pada Revolte dilarang keras mengakses WebServer hingga masa pencoblosan pemilu kepala suku 2024 berakhir. Masa pemilu (hingga pemungutan dan penghitungan suara selesai) kepala suku bersamaan dengan masa pemilu Presiden dan Wakil Presiden Indonesia 2024

### Solusi 
Untuk mengerjakan nomor ini diperlukan bantuan ``--datestart`` dan ``--datestop`` untuk melakukan pembatasan akses pada hari-hari tertentu. Disini diperlukan ``subnet`` dari ``Revolte`` karena pembatasn yang diinginkan adalah terhadap subnet. Disini ``subnet`` kami adalah terdapat pada ``A10`` dimana memiliki ip ``192.210.0.0/30`` dan menentukan protokol yang digunakan sebagai berikut 

```sh
iptables -A INPUT -p tcp --dport 80 -s 192.210.0.0/30 -m time --datestart 2023-12-10 --datestop 2024-02-15 -j DROP
```

**Penjelasan**
- ``-A INPUT``: Menambahkan aturan ke chain INPUT (rantai yang digunakan untuk lalu lintas yang menuju ke sistem).
- ``-p tcp``: Menentukan protokol yang digunakan, dalam hal ini TCP.
- ``--dport 80``: Menentukan port tujuan, dalam hal ini port 80 (umumnya digunakan untuk layanan HTTP).
- ``-s 192.210.0.0/30``: Menentukan alamat sumber yang diizinkan.
- ``-m time --datestart 2023-12-10 --datestop 2024-02-15``: Menggunakan modul waktu untuk menentukan aturan berdasarkan tanggal. Aturan ini akan berlaku mulai dari tanggal 10 Desember 2023 hingga 15 Februari 2024.
- ``-j DROP``: Menentukan tindakan yang diambil jika paket memenuhi kriteria aturan, dalam hal ini menolak (DROP) paket.

### Testing
testing dengan menggunakan ``client``

![Screenshot 2023-12-20 at 18 22 01](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/5a6fe384-abd0-48ce-984e-578daace18c3)

testing dengan menggunakan ``revolte`` dimana sudah diakukan pemblokan

![Screenshot 2023-12-20 at 18 22 04](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/e749a5a4-8f19-456d-841e-b9816dcc75c7)

testing dengan menggunkan ``revote`` tetapi di waktu yang diizinkan

![Screenshot 2023-12-20 at 18 23 12](https://github.com/tiostwn/Jarkom-Modul-5-E08-2023/assets/53292102/83d200de-50c0-4eca-a215-ac3071cac3f5)

 





