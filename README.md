# Jarkom-Modul-4-D03-2021

- Zahrotul Adillah (05111940000139)
- Muhammad Nur Abdurrauf (05111940000140)
- Aflah Hilmy (05111940000177)

## Daftar Isi
- [Topografi](#topografi)
- [Subnetting](#subnetting)
- [Routing](#routing)
- [Testing](#testing)

## Topografi
![image](https://user-images.githubusercontent.com/72771774/143580040-3ca46e05-45a4-4e47-9de1-1b4524b743b1.png)

## Subnetting
### Penjelasan Jawaban
Menentukan subnet-subnet yang ada
![semua subnet](https://user-images.githubusercontent.com/29938033/143676256-1cb8f9ef-314c-405f-93f3-d533ad8cadcc.png)

#### VLSM
Menentukan jumlah ip yang diperlukan di setiap subnet dan netmasknya
|Subnet|Host|Mask|
|------|----|----|
|A1	   |101	|/25 |
|A2	   |701 |/22 |
|A3	   |2   |/30 |
|A4	   |2021|/21 |
|A5	   |1001|/22 |
|A6	   |2	  |/30 |
|A7	   |521	|/22 |
|A8	   |252 |/24 |
|A9	   |2	  |/30 |
|A10	 |2	  |/30 |
|A11	 |721 |/22 | 
|A12	 |502	|/23 |
|A13	 |13  |/28 |
|Total |5841|/19 |

Total ip yang dibutuhkan adalah 5841, sehingga subnet dengan netmask /19 dibagi menggunakan tree berikut:
![Tree VLSM](https://user-images.githubusercontent.com/29938033/143676767-088fbef8-d34f-4623-b655-bdd437fe97fb.png)

Dari tree itu, akan terbentuk pembagian ip seperti berikut:
<table>
<tbody>
  <tr>
    <td rowspan="3">A1</td>
    <td>Network ID</td>
    <td>192.193.0.128</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.128</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.255</td>
  </tr>
  <tr>
    <td rowspan="3">A2</td>
    <td>Network ID</td>
    <td>192.193.4.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.7.255</td>
  </tr>
  <tr>
    <td rowspan="3">A3</td>
    <td>Network ID</td>
    <td>192.193.0.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.3</td>
  </tr>
  <tr>
    <td rowspan="3">A4 </td>
    <td>Network ID</td>
    <td>192.193.24.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.248.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.31.255</td>
  </tr>
  <tr>
    <td rowspan="3">A5</td>
    <td>Network ID</td>
    <td>192.193.8.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.11.255</td>
  </tr>
  <tr>
    <td rowspan="3">A6</td>
    <td>Network ID</td>
    <td>192.193.0.4</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.7</td>
  </tr>
  <tr>
    <td rowspan="3">A7</td>
    <td>Network ID</td>
    <td>192.193.12.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.15.255</td>
  </tr>
  <tr>
    <td rowspan="3">A8</td>
    <td>Network ID</td>
    <td>192.193.1.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.1.255</td>
  </tr>
  <tr>
    <td rowspan="3">A9</td>
    <td>Network ID</td>
    <td>192.193.0.8</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.11</td>
  </tr>
  <tr>
    <td rowspan="3">A10</td>
    <td>Network ID</td>
    <td>192.193.0.12</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.15</td>
  </tr>
  <tr>
    <td rowspan="3">A11</td>
    <td>Network ID</td>
    <td>192.193.16.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.19.255</td>
  </tr>
  <tr>
    <td rowspan="3">A12</td>
    <td>Network ID</td>
    <td>192.193.2.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.254.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.3.255</td>
  </tr>
  <tr>
    <td rowspan="3">A13</td>
    <td>Network ID</td>
    <td>192.193.0.16</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.240</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.0.31</td>
  </tr>
</tbody>
</table>

#### CIDR
Cari 2 subnet yang paling jauh dari cloud, kemudian digabungkan
![Penggabungan 1](https://user-images.githubusercontent.com/29938033/143676862-ce2075b9-dc59-4dcf-9283-b2acb0c75ef3.png)

Kemudian cari kembali subnet yang paling jauh dari cloud dan digabungkan.
![Penggabungan 2](https://user-images.githubusercontent.com/29938033/143676898-849ab872-187b-4a3a-8d19-6ccf7780e1ac.png)

Ulangi terus langkah itu hingga semua subnet tergabung menjadi satu subnet besar.
![Penggabungan 3](https://user-images.githubusercontent.com/29938033/143676998-c9e53b31-5203-4a47-a8f1-15aed102f3fd.jpg)
![Penggabungan 4](https://user-images.githubusercontent.com/29938033/143677053-5fa6c983-5c8c-4ca6-8417-264bffd3e58a.jpg)
![Penggabungan 5](https://user-images.githubusercontent.com/29938033/143677059-9df67c5b-2954-4320-ad5f-46549a2f2789.jpg)
![Penggabungan 6](https://user-images.githubusercontent.com/29938033/143677058-8a086ec7-47b7-4255-90d7-cc34e4353c6f.jpg)
![Penggabungan 7](https://user-images.githubusercontent.com/29938033/143677056-2ad6677a-99a6-4578-8ef9-5edf155f7fa1.jpg)
![Penggabungan 8](https://user-images.githubusercontent.com/29938033/143677054-34d7d231-4525-4d05-9a42-c93cd4bac521.jpg)

Setiap digabungkan, netmask subnet yang baru lebih besar 1 daripada netmask paling besar dari subnet yang digabungkan. Dari penggabungan diatas, maka akan didapatkan tabel seperti berikut:
|Subnet 1	|Subnet 2	|Subnet Gabungan	|Mask|
|---------|---------|-----------------|----|
|A8	      |A11   	  |B1	              |/21 |	
|A1	      |A4	      |C1	              |/20 |
|C1	      |A3	      |D1	              |/19 |
|B1	      |A10	    |D2	              |/20 |
|A12	    |A13	    |D3	              |/22 |
|D1	      |A2	      |E1	              |/18 |
|A7	      |D3	      |E2	              |/21 |
|D2	      |E2      	|F1	              |/19 |
|E1	      |A6	      |G1	              |/17 |
|F1	      |A9	      |G2	              |/18 |
|G2	      |A5	      |H1	              |/17 |
|H1	      |G1	      |I1	              |/16 |

Dari penggabungan subnet tersebut, alamat ip dapat dibagi menggunakan tree berikut:
![Tree CIDR](https://user-images.githubusercontent.com/29938033/143677272-e12ce25b-7786-4ea4-9caf-8ff4ff7e6193.png)

Dari tree itu, akan terbentuk pembagian ip seperti berikut:
<table>
<tbody>
  <tr>
    <td rowspan="3">A1</td>
    <td>Network ID</td>
    <td>192.193.136.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.128</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.136.127</td>
  </tr>
  <tr>
    <td rowspan="3">A2</td>
    <td>Network ID</td>
    <td>192.193.160.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.163.255</td>
  </tr>
  <tr>
    <td rowspan="3">A3</td>
    <td>Network ID</td>
    <td>192.193.144.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.144.3</td>
  </tr>
  <tr>
    <td rowspan="3">A4 </td>
    <td>Network ID</td>
    <td>192.193.128.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.248.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.135.255</td>
  </tr>
  <tr>
    <td rowspan="3">A5</td>
    <td>Network ID</td>
    <td>192.193.64.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.67.255</td>
  </tr>
  <tr>
    <td rowspan="3">A6</td>
    <td>Network ID</td>
    <td>192.193.192.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.192.3</td>
  </tr>
  <tr>
    <td rowspan="3">A7</td>
    <td>Network ID</td>
    <td>192.193.16.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.19.255</td>
  </tr>
  <tr>
    <td rowspan="3">A8</td>
    <td>Network ID</td>
    <td>192.193.4.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.4.255</td>
  </tr>
  <tr>
    <td rowspan="3">A9</td>
    <td>Network ID</td>
    <td>192.193.32.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.32.3</td>
  </tr>
  <tr>
    <td rowspan="3">A10</td>
    <td>Network ID</td>
    <td>192.193.8.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.252</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.8.3</td>
  </tr>
  <tr>
    <td rowspan="3">A11</td>
    <td>Network ID</td>
    <td>192.193.0.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.252.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.3.255</td>
  </tr>
  <tr>
    <td rowspan="3">A12</td>
    <td>Network ID</td>
    <td>192.193.24.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.254.0</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.25.255</td>
  </tr>
  <tr>
    <td rowspan="3">A13</td>
    <td>Network ID</td>
    <td>192.193.26.0</td>
  </tr>
  <tr>
    <td>Netmask</td>
    <td>255.255.255.240</td>
  </tr>
  <tr>
    <td>Broadcast Address</td>
    <td>192.193.26.15</td>
  </tr>
</tbody>
</table>

## Routing
### Penjelasan Jawaban

## Testing
### Penjelasan Jawaban

