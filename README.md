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

Dari pohon itu, akan terbentuk pembagian ip seperti berikut:
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
    <td>255.255.255.254</td>
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

## Routing
### Penjelasan Jawaban

## Testing
### Penjelasan Jawaban

