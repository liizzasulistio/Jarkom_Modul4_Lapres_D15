# Jarkom_Modul4_Lapres_D15

## VLSM
1. Bagi jaringan pada soal menjadi beberapa subnet. Berikut adalah subnet-subnet hasil pembagian kami :
![https://user-images.githubusercontent.com/24503760/101630157-0f676e80-3a55-11eb-891f-b82d75387552.png](https://user-images.githubusercontent.com/24503760/101630157-0f676e80-3a55-11eb-891f-b82d75387552.png)

2. Dari subnet-subnet tersebut, hitung berapa IP yang dibutuhkan untuk masing-masing jaringan.

![image](https://user-images.githubusercontent.com/24503760/101630405-68370700-3a55-11eb-81bb-0bfad6b0b586.png)

3. Untuk masing-masing subnet, hitung berapa length dari masing-masing subnet. Penghitungan panjang didapat dengan mengecek banyak IP. Sebagai contoh, untuk A01, IP yang dibutuhkan ada 1001. Maka lengthnya adalah 22, karena untuk length 23 IP tersedia hanya 510, sehingga tidak mencukupi. 

4. Berdasarkan length tersebut, buat diagramnya. Dan dari diagram tersebut, kita dapat memperoleh NIDnya.
![VLSM_Tree](https://user-images.githubusercontent.com/24503760/101633567-04fba380-3a5a-11eb-972e-0137d48331fc.png)

5. Berdasarkan length juga, tentukan netmasknya, contoh A01 length 22, netmasknya adalah `255.255.252.0`.

6. Tentukan broadcast IPnya. Broadcast IP diperoleh dengan cara NID + wildcard. Wildcard dapat ditentukan oleh lengthnya.

Setelah langkah diatas, diperoleh informasi seperti ini :

![image](https://user-images.githubusercontent.com/24503760/101633665-28265300-3a5a-11eb-9bf1-db78e8ed6e06.png)