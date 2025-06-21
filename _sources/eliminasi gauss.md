---
title: eliminasi gauss

---

# ELIMINASI GAUSS
## PENGERTIAN
### METODE ELIMINASI
**Metode eliminasi** adalah salah satu metode yang digunakan untuk menyelesaikan soal persamaan linear dua atau tiga variable. Dimana metode eliminasi secara garis besar akan menghapus atau menghilangkan satu variabel dalam persamaan tersebut.

### ELIMINASI GAUSS
Sistem persamaan linear yang di ubah menjadi bentuk matriks, matriks tersebut lalu diubah kebentuk Eselon Baris melalui Operasi Baris Elementer. Kemudian sistem diselesaikan dengan substitusi balik.

#### TUGAS
MEMBUAT PENJELASAN SOLUSI ATAU PENYELESAIAN PERSAMAAN 3 VARIABEL DENGAN MENGGUNAKAN ELIMINASI GAUUS SERTA MENAMPILKAN SOLUSINYA SECARA GRAFIS MENGGUNAKAN GEOGEBRA !!

Selesaikan sistem persamaan linier berikut :
 
$$x + y + z = 6$$

$$2x + 2y + 3z = 14$$

$$3x + 4y + 2z = 13$$

Berikut adalah langkah-langkah menyelesaikan sistem persamaan linear diatas menggunakan metode eliminasi Gauss.

1. langkah pertama 

persamaan linier di ubah ke dalam bentuk Matriks Augmented

Hasil Matriksnya : 

$$\begin{bmatrix}
1 & 1 & 1 & | 6 \\
2 & 2 & 3 & | 14 \\
3 & 4 & 2 & | 13  \
\end{bmatrix}$$


2. langkah kedua
- Jadikan elemen pivot pertama (baris 1, kolom 1) bernilai 1.
- Jika Sudah bernilai 1, maka tidak perlu diubah.
- NOL-kan Elemen di bawah Elemen Pivot Pertama
- Pivot pertama sudah 1 di posisi (1,1). Maka Kita akan buat elemen di bawahnya menjadi nol:

$$𝑅_2→𝑅_2−2𝑅_1$$
  
  hasil matriksnya : 
  
$$\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 0 & 1 & | 2  \\
3 & 4 & 2 & | 13  \
\end{bmatrix}$$
 
  
$$𝑅_3→𝑅_3−3𝑅_1$$
  
  hasil matriksnya : 
  
$$\begin{bmatrix}
1 & 1 & 1 &  | 6 \\
0 & 0 & 1 &  | 2  \\
0 & 1 & -1 & | -5  \
\end{bmatrix}$$
  
  
- Jadikan elemen pivot kedua (baris 2, kolom 2) bernilai 1:

$$𝑅_2→𝑅_2+𝑅_3$$
  
  hasil matriksnya :
  
$$\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 1 & 0 & | -3 \\
0 & 1 & -1 & | -5 \
\end{bmatrix}$$
  
 - NOL-kan Elemen di bawah Elemen Pivot kedua :
$$𝑅_3→𝑅_3-𝑅_2$$
  hasil matriksnya : 

$$\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 1 & 0 & | -3 \\
0 & 0 & -1 & | -2 \
\end{bmatrix}$$
  
  
- Jadikan elemen pivot kedua (baris 3, kolom 3) bernilai 1:
  
$$𝑅_3→𝑅_3.(-1)$$
  hasil matriksnya : 

$$\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 1 & 0 & | -3 \\
0 & 0 & 1 & | 2   \ 
\end{bmatrix}$$
  
3. langkah ketiga
   Subtitusi Balik
   
$$\text{Dari baris terakhir } : $$

$$z = 2$$

$$\text{Substitusi z ke baris kedua} : $$

$$ y - 2 = -5 \quad \Rightarrow \quad y = -3 $$

$$ \text{Substitusi y dan z ke baris pertama}:$$

$$ x + y + z = 6 \quad \Rightarrow \quad x + (- 3) + 2 = 6 \quad \Rightarrow \quad x - 1 = 6 \quad \Rightarrow \quad x = 7 $$
$$ \text{Solusi akhir :}$$
$$ x = 7, \quad y = -3, \quad z = 2$$

### Penjelasan Solusi atau Penyelesaian

#### 1. Satu Solusi Unik 

Jika sistem persamaan memiliki satu solusi unik, maka sistem tersebut konsisten dan tidak bergantung. Setelah dilakukan eliminasi Gauss, matriks augmented akan memiliki bentuk segitiga atas, dan setiap variabel akan memiliki nilai tertentu setelah dilakukan substitusi balik.

Contoh sistem yang memiliki satu solusi unik:

$$x + y + z = 6$$

$$2x + 2y + 3z = 14$$

$$3x + 4y + 2z = 13$$

Setelah di lakukan penyelesaian menggunakan metode eliminasi Gauss, sistem ini menghasilkan solusi yang jelas, misalnya:

$$ x = 7, \quad y = -3, \quad z = 2$$

#### 2. Tidak Ada Solusi

Jika sistem persamaan linear tidak memiliki solusi, maka sistem tersebut inkonsisten. Hal ini terjadi ketika selama eliminasi Gauss kita memperoleh sebuah baris yang berbentuk seperti 0=1 (atau bentuk lain), yang menunjukkan bahwa tidak ada solusi yang memenuhi sistem persamaan tersebut.

Contoh sistem yang inkonsisten:

Sistem persamaan berikut:

$$x + y = 3$$

$$2x + 2y = 7$$

tidak memiliki solusi karena persamaan kedua sebenarnya adalah hasil dari persamaan pertama yang dikalikan 2, tetapi dengan konstanta yang berbeda (6 vs 7). Hal ini membuat sistem ini tidak konsisten dan tidak mungkin memiliki nilai  dan  yang memenuhi kedua persamaan secara bersamaan.
 
Jika kita melakukan eliminasi Gauss pada sistem ini, kita akan mendapatkan baris yang bertentangan, seperti:

$$0𝑥 + 0𝑦 = 1$$

Ini menunjukkan bahwa sistem tersebut tidak ada solusi.

#### 3. Tak Terhingga Banyak Solusi

Jika sistem persamaan memiliki lebih dari satu solusi, maka sistem tersebut konsisten dan bergantung. Ini terjadi ketika, setelah eliminasi Gauss, kita mendapatkan satu atau lebih baris yang semuanya nol (misalnya, 0=0 yang menunjukkan bahwa sistem tersebut memiliki tak terhingga banyak solusi.

Contoh sistem yang memiliki tak terhingga banyak solusi:

sistem persamaan berikut : 

$$𝑥 + 𝑦 = 2$$

$$2𝑥 + 2𝑦 = 4$$

memiliki tak hingga banyak solusi karena persamaan kedua sebenarnya adalah hasil dari persamaan pertama yang dikalikan 2. Ini berarti kedua persamaan sebenarnya sama dan merepresentasikan garis yang sama di bidang koordinat.

Setelah eliminasi Gauss, kita akan mendapatkan baris yang tidak memberikan informasi baru, seperti:

$$0𝑥 + 0𝑦 = 0$$
    
Ini menunjukkan bahwa sistem ini memiliki tak terhingga banyak solusi, dan solusinya dapat ditulis dalam bentuk parameter, seperti:

$$𝑥 = 2 − 𝑦$$
    
Dengan demikian, 𝑦 dapat berupa sembarang nilai, dan 𝑥 bergantung pada nilai 𝑦

Hasil grafis dari geogebra

<iframe src="https://www.geogebra.org/material/iframe/id/xjzddhvh/width/800/height/600/border/888888/rc/false/ai/true/sdz/true/smb/false/stb/false" width="800" height="600" style="border:0px;"> </iframe>