# laporan-1-dan-2-basis-data-

#### Septian Efan Fais Putra
#### XI RPL 2 
#### 22

### MODUL 1

#### 1.Instal xampp
![apk xampp](https://user-images.githubusercontent.com/114629208/192921901-69c7d5ba-9796-41fb-a792-11ac89e69adf.png)

#### 2.Nyalakan my sql di xampp
![Screenshot_1](https://user-images.githubusercontent.com/114629208/192921969-8dee229c-e25a-4160-990f-b08e8ef5f726.png)

#### 3.Buka cmd
![Screenshot_2](https://user-images.githubusercontent.com/114629208/192922027-ab641124-04dc-4c0b-a7d8-b86d9fd58561.png)

#### 4.masuk ke direktori mysql dan tuliskan sintaks berikut  
```
cd xampp/mysql/bin
```
#### 5. tuliskan sintaks 
```
\xampp\mysql\bin>mysql -u root
```
![Screenshot_3](https://user-images.githubusercontent.com/114629208/192922327-0f244d12-b179-4c87-87d8-f43684b547be.png)

#### Tanda Sudah Query
## Modul part 2

#### 1.Melihat show database dan tabel dengan kode berikut:
```
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| penjualan          |
| performance_schema |
| phpmyadmin         |
| sekolah            |
| test               |
+--------------------+
7 rows in set (0.001 sec)

MariaDB [(none)]> use sekolah
Database changed
MariaDB [sekolah]> show tables;
+-------------------+
| Tables_in_sekolah |
+-------------------+
| siswa             |
+-------------------+
1 row in set (0.001 sec)
```
### 2. Menggunakan use dalam cmd
```
MariaDB [(none)]> use sekolah
Database changed
```
#### 3. Menggunakan create dan menambahkan database dan tabel baru
```
create table siswa( nim int not null, nama char(20),wali int);
```
![Screenshot_5](https://user-images.githubusercontent.com/114629208/192924333-60d731e0-018e-47a3-8fbc-535d5f7a3891.png)

![Screenshot_6](https://user-images.githubusercontent.com/114629208/192924353-7a5d7e2e-0be0-4f11-aa27-5dcb2b495bbe.png)

```
create database sekolah;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| penjualan          |
| performance_schema |
| phpmyadmin         |
| sekolah            |
| test               |
+--------------------+
7 rows in set (0.001 sec)
```
#### 4. DESC Untuk melihat struktur (metadata) sebuah tabel.
```
desc siswa;
```
##### Dan hasil output
![Screenshot_7](https://user-images.githubusercontent.com/114629208/192925677-4db1fa02-335e-4c4c-a7a7-decb86342f94.png)

## Laporan Tugas
#### Membuat Database Dan Tabel
#### 1. Sebelum itu buatlah 
```
Create database Sekolah;
```
#### 2. Buat 2 buah tabel siswa dan dosen didalam database sekolah
```
Create table siswa(
nim int not null, 
nama char, 
wali int
);

create table wali (
Nip int not null, 
Nama char(20), 
Alamat char(50)
);
```
![Screenshot_8](https://user-images.githubusercontent.com/114629208/192931386-db9d24fe-4c26-468c-9cdf-d181b2f6bc2a.png)
