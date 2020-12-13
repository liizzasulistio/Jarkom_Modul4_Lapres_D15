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
| **Total**  | **5841**  | **/19** |

3. Untuk masing-masing subnet, hitung berapa length dari masing-masing subnet. Penghitungan panjang didapat dengan mengecek banyak IP. Sebagai contoh, untuk A01, IP yang dibutuhkan ada 1001. Maka lengthnya adalah 22, karena untuk length 23 IP tersedia hanya 510, sehingga tidak mencukupi. 

4. Berdasarkan length tersebut, buat diagramnya. Dan dari diagram tersebut, kita dapat memperoleh NIDnya.
![VLSM_Tree](https://user-images.githubusercontent.com/24503760/101633567-04fba380-3a5a-11eb-972e-0137d48331fc.png)

5. Berdasarkan length juga, tentukan netmasknya, contoh A01 length 22, netmasknya adalah `255.255.252.0`.

6. Tentukan broadcast IPnya. Broadcast IP diperoleh dengan cara NID + wildcard. Wildcard dapat ditentukan oleh lengthnya.

Setelah langkah diatas, diperoleh informasi seperti ini :
![Tabel1](https://user-images.githubusercontent.com/58472359/102003089-7a56c500-3d35-11eb-9689-bac04c7055d1.png)
![Tabel2](https://user-images.githubusercontent.com/58472359/102003091-7b87f200-3d35-11eb-9c80-15f0daadcd68.png)

---
## CIDR (Classless Inter Domain Routing)
1.	Menentukan subnet pada topologi dan pemberian labelling netmask terhadap masing-masing subnet.
![A](https://user-images.githubusercontent.com/58472359/102002093-c270ea00-3d2b-11eb-8740-4119fad54999.png)

2.	Menggabungkan subnet paling bawah di dalam topologi atau subnet yang paling jauh dari internet. Langkah 2 ini diulangi sampai terbentuk subnet besar.
    - Pembentukan subnet B
    ![B](https://user-images.githubusercontent.com/58472359/102002094-c43aad80-3d2b-11eb-9ef5-deabff834354.png)
    - Pembentukan subnet C
    ![C](https://user-images.githubusercontent.com/58472359/102002095-c6047100-3d2b-11eb-833f-98f048f3d2b7.png)
    - Pembentukan subnet D
    ![D](https://user-images.githubusercontent.com/58472359/102002096-c7359e00-3d2b-11eb-85fc-cc46e75e8b33.png)
    - Pembentukan subnet E
    ![E](https://user-images.githubusercontent.com/58472359/102002098-c866cb00-3d2b-11eb-8a7b-734af81eed73.png)
    - Pembentukan subnet F
    ![F](https://user-images.githubusercontent.com/58472359/102002099-c997f800-3d2b-11eb-94ba-d6771786491b.png)
3. Dari gambar di atas diperoleh subnet besar dengan submask /16, NID 192.168.0.0 dan netmask 255.255.0.0
![G](https://user-images.githubusercontent.com/58472359/102002100-cac92500-3d2b-11eb-86f5-d706e1bd6593.png)
4. Menghitung pembagian IP dengan pohon berdasarkan penggabungan subnet.
![Pohon_CIDR](https://user-images.githubusercontent.com/58472359/102002804-a755a880-3d32-11eb-8e39-b6d4a7dbc285.png)
5. Membuat tabel untuk pembagian IP yang telah diperoleh.
![Tabel1](https://user-images.githubusercontent.com/58472359/102002803-a6247b80-3d32-11eb-92eb-8aa021a6c6f1.png)
![Tabel2](https://user-images.githubusercontent.com/58472359/102002802-a58be500-3d32-11eb-817b-d71613177904.png)
6. Melakukan routing pada Cisco Packet Tracer, atau dapat dilihat pada [file berikut ini](https://github.com/liizzasulistio/Jarkom_Modul4_Lapres_D15/blob/main/praktikum_CIDR_revisi.pkt)
![CIDR_CPT](https://user-images.githubusercontent.com/58472359/102002101-cd2b7f00-3d2b-11eb-9c23-4a2269a0710a.png)
