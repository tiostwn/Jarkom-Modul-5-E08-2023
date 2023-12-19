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
<table><thead><tr><th>Subnet</th><th>Node</th><th>IP</th><th>Netmask</th><th>Length</th><th>NID</th><th>Broadcast</th></tr></thead><tbody><tr><td rowspan="2">A1</td><td>Fern</td><td>192.210.0.1</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.0</td><td rowspan="2">192.210.0.3</td></tr><tr><td>Revolte</td><td>192.210.0.2</td></tr><tr><td rowspan="2">A2</td><td>Fern</td><td>192.210.0.5</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.4</td><td rowspan="2">192.210.0.7</td></tr><tr><td>Richter</td><td>192.210.0.6</td></tr><tr><td rowspan="3">A3</td><td>Himmel</td><td>192.210.0.129</td><td rowspan="3">255.255.255.128</td><td rowspan="3">25</td><td rowspan="3">192.210.0.128</td><td rowspan="3">192.210.0.255</td></tr><tr><td>Fern</td><td>192.210.0.130</td></tr><tr><td>SchwerMountain</td><td>DHCP</td></tr><tr><td rowspan="2">A4</td><td>Himmel</td><td>192.210.2.1</td><td rowspan="2">255.255.254.0</td><td rowspan="2">23</td><td rowspan="2">192.210.2.0</td><td rowspan="2">192.210.3.255</td></tr><tr><td>LaubHills</td><td>DHCP</td></tr><tr><td rowspan="2">A5</td><td>Frieren</td><td>192.210.0.9</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.8</td><td rowspan="2">192.210.0.11</td></tr><tr><td>Himmel</td><td>192.210.0.10</td></tr><tr><td rowspan="2">A6</td><td>Frieren</td><td>192.210.0.13</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.12</td><td rowspan="2">192.210.0.15</td></tr><tr><td>Stark</td><td>192.210.0.14</td></tr><tr><td rowspan="2">A7</td><td>Aura</td><td>192.210.0.17</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.16</td><td rowspan="2">192.210.0.19</td></tr><tr><td>Frieren</td><td>192.210.0.18</td></tr><tr><td rowspan="2">A8</td><td>Aura</td><td>192.210.0.21</td><td rowspan="2">255.255.255.252</td><td rowspan="2">30</td><td rowspan="2">192.210.0.20</td><td rowspan="2">192.210.0.23</td></tr><tr><td>Heiter</td><td>192.210.0.22</td></tr><tr><td rowspan="2">A9</td><td>Heiter</td><td>192.210.8.1</td><td rowspan="2">255.255.248.0</td><td rowspan="2">21</td><td rowspan="2">192.210.8.0</td><td rowspan="2">192.210.15.255</td></tr><tr><td>TurkRegion</td><td>DHCP</td></tr><tr><td rowspan="3">A10</td><td>Heiter</td><td>192.210.4.1</td><td rowspan="3">255.255.252.0</td><td rowspan="3">22</td><td rowspan="3">192.210.4.0</td><td rowspan="3">192.210.7.255</td></tr><tr><td>Sein</td><td>192.210.4.2</td></tr><tr><td>GrabForest</td><td>DHCP</td></tr></tbody></table>

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

Pada node **GrabForest**, kita akan melakukan ping ke google.com dengan perintah

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






