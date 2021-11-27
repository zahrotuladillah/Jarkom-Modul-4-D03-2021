# Jarkom-Modul-4-D03-2021

- Zahrotul Adillah (05111940000139)
- Muhammad Nur Abdurrauf (05111940000140)
- Aflah Hilmy (05111940000177)

## Daftar Isi
- [Topografi](#topografi)
- [VLSM](#vlsm)
- [CIDR](#cidr)

## Topografi
![image](https://user-images.githubusercontent.com/72771774/143580040-3ca46e05-45a4-4e47-9de1-1b4524b743b1.png)

## VLSM
### Subnetting
#### Penjelasan Jawaban
Menentukan subnet-subnet yang ada
![semua subnet](https://user-images.githubusercontent.com/29938033/143676256-1cb8f9ef-314c-405f-93f3-d533ad8cadcc.png)

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

Melakukan implementasi di CPT:

Interface di Foosha

![image](https://user-images.githubusercontent.com/74708771/143678029-7c175c82-045c-4974-9e88-e60f53e936cd.png)
![image](https://user-images.githubusercontent.com/74708771/143678020-f1425552-5a2b-40ff-9394-27b10be40c48.png)
![image](https://user-images.githubusercontent.com/74708771/143678043-426d8322-e347-4f73-8077-7ec90ea94fad.png)
![image](https://user-images.githubusercontent.com/74708771/143678051-26abc013-905c-4c29-9d62-6da658ef5f0b.png)
![image](https://user-images.githubusercontent.com/74708771/143678066-2ba55f24-0f45-40c7-8414-76eb98086026.png)

Interface di Water7

![image](https://user-images.githubusercontent.com/74708771/143678083-d23aaae0-e4a4-4b8c-a976-ae6605d4ed7e.png)
![image](https://user-images.githubusercontent.com/74708771/143678091-dd9a77e5-760f-4192-a85a-866ca52f0e5e.png)
![image](https://user-images.githubusercontent.com/74708771/143678103-eebc287d-5955-4444-9b13-026569e92b8d.png)

Interface di Pucci

![image](https://user-images.githubusercontent.com/74708771/143678134-1d949278-50ce-4a9b-8c5d-7e44de3a9787.png)
![image](https://user-images.githubusercontent.com/74708771/143678145-f2b1d164-f470-4a70-b7aa-1858997b25f3.png)
![image](https://user-images.githubusercontent.com/74708771/143678153-62aa57b9-0f34-4d9a-b50a-11200b049017.png)

Interface di Guanhao

![image](https://user-images.githubusercontent.com/74708771/143678173-f2723f3e-5ebd-4f6d-b92d-4b7193a694fb.png)
![image](https://user-images.githubusercontent.com/74708771/143678186-f9ef01c9-e504-4706-b653-ba7524e459ae.png)
![image](https://user-images.githubusercontent.com/74708771/143678196-e5e0aa43-a882-4904-9e52-cf6c284b5bf5.png)
![image](https://user-images.githubusercontent.com/74708771/143678203-ba7341ae-b42e-4d9a-bdc4-9794abf5818c.png)

Interface di Alabasta

![image](https://user-images.githubusercontent.com/74708771/143678222-2356ef67-5249-45de-89e5-41698c2541c1.png)
![image](https://user-images.githubusercontent.com/74708771/143678231-e227e52c-998c-44da-b194-2ae80583520f.png)

Interface di Oimo

![image](https://user-images.githubusercontent.com/74708771/143678253-a06d36e4-46e5-476c-808d-c4cacffab9f6.png)
![image](https://user-images.githubusercontent.com/74708771/143678264-0197e1c1-4fa8-4a39-99b7-f8a577033995.png)
![image](https://user-images.githubusercontent.com/74708771/143678269-03b4ea4e-24b5-45dc-95a7-34755b82dc9f.png)

Interface di Seastone

![image](https://user-images.githubusercontent.com/74708771/143678286-0bc18017-a6fe-48b0-b857-5ccd572b2166.png)
![image](https://user-images.githubusercontent.com/74708771/143678297-6154fde4-d9ba-496e-9acc-ab3957befa63.png)

Interface di Jipangu

![image](https://user-images.githubusercontent.com/74708771/143678435-21633a81-5ca6-4683-b4e3-4688d59ee832.png)

Interface di Courtyard

![image](https://user-images.githubusercontent.com/74708771/143678444-5c63a0d0-c8c3-4166-8158-1107fc0a1f57.png)

Interface di Calmbelt

![image](https://user-images.githubusercontent.com/74708771/143678449-a1b52ea0-351e-4c38-a1c2-9e2f56223f94.png)

Interface di Cipher

![image](https://user-images.githubusercontent.com/74708771/143678457-6cd6ffeb-6edb-435b-b687-4fd2fab4a66e.png)

Interface di Blueno

![image](https://user-images.githubusercontent.com/74708771/143678462-c4eb5e3e-b328-4fc6-8b4d-7f75085dae87.png)

Interface di Jabra

![image](https://user-images.githubusercontent.com/74708771/143678468-7fedf918-4693-47dc-909a-3c8ec68ccc59.png)

Interface di Maingate

![image](https://user-images.githubusercontent.com/74708771/143678478-b4c6eff0-990a-44f9-b4ac-fafabda5ad15.png)

Interface di Jorge

![image](https://user-images.githubusercontent.com/74708771/143678485-526a2e0c-1609-4d32-90b6-3cafab3e4983.png)

Interface di Enieslobby

![image](https://user-images.githubusercontent.com/74708771/143678494-171ead40-d7fd-4b08-99a4-7f0148db7d7d.png)

Interface di Elena

![image](https://user-images.githubusercontent.com/74708771/143678502-8f224b6c-dfef-40db-80ed-3c28ce927f3b.png)

Interface di Doriki

![image](https://user-images.githubusercontent.com/74708771/143678512-9722b5e3-1b92-450c-bac4-83b83bfee3e3.png)

Interface di Fukurou

![image](https://user-images.githubusercontent.com/74708771/143678519-19ff8622-693f-4f5b-9314-5e715f87c5cc.png)

### Routing
#### Penjelasan Jawaban
Melakukan konfigurasi routing static pada router seusai dengan konfigurasi dibawah ini

| ROUTER   |	SUBNET  | NETWORK       |	MASK          	| NEXT HOP     |
|----------|----------|---------------|-----------------|--------------|
| FOOSHA   |	A1	    | 192.193.0.128 |	255.255.255.128	| 192.193.0.6  |
|          |	A2	    | 192.193.4.0   |	255.255.252.0   |	192.193.0.6  |
|          |	A3	    | 192.193.0.0   |	255.255.255.252 |	192.193.0.6  |
|          |	A4	    | 192.193.24.0	| 255.255.248.0   |	192.193.0.6  |
|          |	A7	    | 192.193.12.0	| 255.255.252.0   |	192.193.0.10 |
|          |	A8	    | 192.193.1.0	  | 255.255.255.0   |	192.193.0.10 |
|          |	A10	    | 192.193.0.12	| 255.255.255.252	| 192.193.0.10 |
|          |	A11	    | 192.193.16.0	| 255.255.252.0	  | 192.193.0.10 |
|          |	A12	    | 192.193.2.0	  | 255.255.254.0	  | 192.193.0.10 |
|          |	A13	    | 192.193.0.16	| 255.255.255.240	| 192.193.0.10 |
|          |	FUKUROU	| 192.193.128.0	| 255.255.255.0   |	192.193.0.10 |
| WATER7   |	DEFAULT	| 0.0.0.0	      | 0.0.0.0	        | 192.193.0.5  |
|          |	A1	    | 192.193.0.128	| 255.255.255.128	| 192.193.0.2  |
|          |	A4	    | 192.193.24.0	| 255.255.248.0	  | 192.193.0.2  |
| PUCCI    |	DEFAULT | 0.0.0.0       |	0.0.0.0	        | 192.193.0.1  |
| GUANHAO  |	DEFAULT | 0.0.0.0       |	0.0.0.0	        | 192.193.0.9  |
|          |	A8	    | 192.193.1.0	  | 255.255.255.0 	| 192.193.0.14 |
|          |	A11	    | 192.193.16.0  |	255.255.252.0 	| 192.193.0.14 |
|          |	A13	    | 192.193.0.16  |	255.255.255.240	| 192.193.2.3  |
|          |	FUKUROU | 192.193.128.0 |	255.255.255.0	  | 192.193.0.14 |
| ALABASTA |	DEFAULT | 0.0.0.0       |	0.0.0.0	        | 192.193.2.1  |
| OIMO     |	DEFAULT | 0.0.0.0       |	0.0.0.0	        | 192.193.0.13 |
|          |	A11	    | 192.193.16.0	| 255.255.252.0	  | 192.193.1.3  |
| SEASTONE |	DEFAULT | 0.0.0.0       |	0.0.0.0	        | 192.193.1.1  |

## CIDR
### Subnetting
#### Penjelasan Jawaban
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

### Routing
#### Penjelasan Jawaban
Melakukan konfigurasi routing pada router seusai dengan konfigurasi dibawah ini

| ROUTER   |	SUBNET  | NETWORK       |	MASK          	| NEXT HOP      |
|----------|----------|---------------|-----------------|---------------|
| FOOSHA   |	E1	    | 192.193.0.128 |	255.255.192.0   | 192.193.192.2 |
|          |	F1	    | 192.193.0.0   |	255.255.224.0   |	192.193.32.2  |
|          |	FUKUROU	| 192.193.78.0	| 255.255.255.255 |	192.193.32.2  |
| WATER7   |	C1    	| 192.193.128.0 | 255.255.240.0   | 192.193.144.2 |
| GUANHAO  |	B1      | 192.193.0.0   |	255.255.248.0   | 192.193.8.2   |
|          |	A13	    | 192.193.26.0  | 255.255.255.240	| 192.193.24.2  |
|          |	FUKUROU | 192.193.78.0  |	255.255.255.255 | 192.193.8.2   |
| OIMO     |	A11     | 192.193.0.0   |	255.255.255.0   | 192.193.4.2   |


Melakukan implementasi Subnetting dan Routing di GNS3:

Topologi GNS3
![image](https://user-images.githubusercontent.com/74708771/143679943-1212e975-fb29-4d47-8ad2-b23a15157a36.png)

Konfigurasi di Foosha
```
auto eth0 #cloud
iface eth0 inet dhcp
up iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.193.0.0/16

auto eth1 #doriki
iface eth1 inet static
address 192.193.73.1
netmask 255.255.255.255

auto eth2 #A5
iface eth2 inet static
address 192.193.64.1
netmask 255.255.252.0

auto eth3 #A6
iface eth3 inet static
address 192.193.192.1
netmask 255.255.255.252
up route add -net 192.193.128.0 netmask 255.255.192.0 gw 192.193.192.2 #E1

auto eth4 #A9
iface eth4 inet static
address 192.193.32.1
netmask 255.255.255.252
up route add -net 192.193.0.0 netmask 255.255.224.0 gw 192.193.32.2 #F1
up route add -net 192.193.78.0 netmask 255.255.255.255 gw 192.193.32.2 #FUKUROU
```

Konfigurasi di Water7
```
auto eth0 #A6
iface eth0 inet static
address 192.193.192.2
netmask 255.255.255.252
gateway 192.193.192.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A2
iface eth1 inet static
address 192.193.160.1
netmask 255.255.252.0

auto eth2 #A3
iface eth2 inet static
address 192.193.144.1
netmask 255.255.255.252
up route add -net 192.193.128.0 netmask 255.255.240.0 gw 192.193.144.2 #C1
```

Konfigurasi di Pucci
```
auto eth0 #A3
iface eth0 inet static
address 192.193.144.2
netmask 255.255.255.252
gateway 192.193.144.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A1
iface eth1 inet static
address 192.193.136.1
netmask 255.255.255.128

auto eth2 #A4
iface eth2 inet static
address 192.193.128.1
netmask 255.255.248.0
```

Konfigurasi di Guanhao
```
auto eth0 #A9
iface eth0 inet static
address 192.193.32.2
netmask 255.255.255.252
gateway 192.193.32.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A7
iface eth1 inet static
address 192.193.16.1
netmask 255.255.252.0

auto eth2 #A10
iface eth2 inet static
address 192.193.8.1
netmask 255.255.255.252
up route add -net 192.193.0.0 netmask 255.255.248.0 gw 192.193.8.2 #B1
up route add -net 192.193.78.0 netmask 255.255.255.255 gw 192.193.8.2 #FUKUROU

auto eth3 #A12
iface eth3 inet static
address 192.193.24.1
netmask 255.255.254.0
up route add -net 192.193.26.0 netmask 255.255.255.240 gw 192.193.24.2 #A13
```

Konfigurasi di Alabasta
```
auto eth0 #A12
iface eth0 inet static
address 192.193.24.2
netmask 255.255.254.0
gateway 192.193.24.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A13
iface eth1 inet static
address 192.193.26.1
netmask 255.255.255.240
```

Konfigurasi di Oimo
```
auto eth0 #A10
iface eth0 inet static
address 192.193.8.2
netmask 255.255.255.252
gateway 192.193.8.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A8
iface eth1 inet static
address 192.193.4.1
netmask 255.255.255.0
up route add -net 192.193.0.0 netmask 255.255.252.0 gw 192.193.4.2 #A11

auto eth2 #fukurou
iface eth2 inet static
address 192.193.78.1
netmask 255.255.255.255
```

Konfigurasi di Seastone
```
auto eth0 #A8
iface eth0 inet static
address 192.193.4.2
netmask 255.255.255.0
gateway 192.193.4.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf

auto eth1 #A11
iface eth1 inet static
address 192.193.0.1
netmask 255.255.252.0
```

Konfigurasi di Jipangu
```
auto eth0
iface eth0 inet static
address 192.193.136.2
netmask 255.255.255.128
gateway 192.193.136.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Courtyard
```
auto eth0
iface eth0 inet static
address 192.193.128.3
netmask 255.255.248.0
gateway 192.193.128.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Calmbelt
```
auto eth0
iface eth0 inet static
address 192.193.128.2
netmask 255.255.248.0
gateway 192.193.128.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Cipher
```
auto eth0
iface eth0 inet static
address 192.193.160.2
netmask 255.255.252.0
gateway 192.193.160.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Blueno
```
auto eth0
iface eth0 inet static
address 192.193.64.2
netmask 255.255.252.0
gateway 192.193.64.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Jabra
```
auto eth0
iface eth0 inet static
address 192.193.16.2
netmask 255.255.252.0
gateway 192.193.16.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Maingate
```
auto eth0
iface eth0 inet static
address 192.193.24.3
netmask 255.255.254.0
gateway 192.193.24.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Jorge
```
auto eth0
iface eth0 inet static
address 192.193.26.2
netmask 255.255.255.240
gateway 192.193.26.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Enieslobby
```
auto eth0
iface eth0 inet static
address 192.193.4.3
netmask 255.255.255.0
gateway 192.193.4.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Elena
```
auto eth0
iface eth0 inet static
address 192.193.0.2
netmask 255.255.252.0
gateway 192.193.0.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Doriki
```
auto eth0
iface eth0 inet static
address 192.193.73.2
netmask 255.255.255.255
gateway 192.193.73.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

Konfigurasi di Fukurou
```
auto eth0
iface eth0 inet static
address 192.193.78.2
netmask 255.255.255.255
gateway 192.193.78.1
up echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### Testing
ping its.ac.id dari Blueno

![image](https://user-images.githubusercontent.com/74708771/143680321-b2224687-7370-4e00-b54d-01fd87ae0b39.png)

Ping its.ac.id dari Enieslobby

![image](https://user-images.githubusercontent.com/74708771/143680414-fba311e0-0d9a-48c0-bfef-4645a8aad2d9.png)

Ping Fukurou dari Jorge

![image](https://user-images.githubusercontent.com/74708771/143680554-2b9e247b-ea9c-4193-9215-b2db735ced97.png)

Ping Doriki dari Jabra

![image](https://user-images.githubusercontent.com/74708771/143680526-0a67ab3b-22be-4155-8225-c6e03657ad64.png)
