# Jarkom_Modul4_Lapres_D15
- Ammar Alifian Fahdan (05111840000007)
- Lii'zza Aisyah Putri Sulistio (05111840000073)
---
## VLSM (Variable Net Subnet Masking)
1. Bagi jaringan pada soal menjadi beberapa subnet. Berikut adalah subnet-subnet hasil pembagian kami:
![VLSM](https://user-images.githubusercontent.com/58472359/102002547-25fd1680-3d30-11eb-94b6-ab995aa42cfb.png)

2. Dari subnet-subnet tersebut, hitung berapa IP yang dibutuhkan untuk masing-masing jaringan.

| Subnet  | Jumlah IP | Submask |
| :-----: | :-------: | :-----: |
| A01  | 1001  | /22 |
| A02  | 2  | /30 |
| A03  | 2  | /30 |
| A04  | 101  | /25 |
| A05  | 2  | /30 |
| A06  | 502  | /23 |
| A07  | 13  | /28 |
| A08  | 701  | /22 |
| A09  | 2021  | /21 |
| A10  | 512  | /22 |
| A11  | 2  | /30 |
| A12  | 252  | /24 |
| A13  | 721  | /22 |
| **Total  | 5841  | /19** |

3. Untuk masing-masing subnet, hitung berapa length dari masing-masing subnet. Penghitungan panjang didapat dengan mengecek banyak IP. Sebagai contoh, untuk A01, IP yang dibutuhkan ada 1001. Maka lengthnya adalah 22, karena untuk length 23 IP tersedia hanya 510, sehingga tidak mencukupi. 

4. Berdasarkan length tersebut, buat diagramnya. Dan dari diagram tersebut, kita dapat memperoleh NIDnya.
![VLSM_Tree](https://user-images.githubusercontent.com/24503760/101633567-04fba380-3a5a-11eb-972e-0137d48331fc.png)

5. Berdasarkan length juga, tentukan netmasknya, contoh A01 length 22, netmasknya adalah `255.255.252.0`.

6. Tentukan broadcast IPnya. Broadcast IP diperoleh dengan cara NID + wildcard. Wildcard dapat ditentukan oleh lengthnya.

Setelah langkah diatas, diperoleh informasi seperti ini :

![image](https://user-images.githubusercontent.com/24503760/101633665-28265300-3a5a-11eb-9bf1-db78e8ed6e06.png)
