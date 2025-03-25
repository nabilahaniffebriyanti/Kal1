---
title: aljabar matriks

---

# ALJABAR  MATRIKS

## Sifat-Sifat Operasi Matriks, Invers Aditif, dan Matriks Identitas

###  1. Sifat Operasi Matriks
#### A. Sifat Penjumlahan 
- Sifat komutatif adalah salah satu sifat dalam operasi matematika yang menyatakan bahwa urutan operand tidak memengaruhi hasil operasi. Dengan kata lain, jika ( a ) dan ( b ) adalah dua elemen, maka:
$( a + b = b + a )$
- Sifat asosiatif adalah salah satu sifat penting dalam operasi matematika yang menyatakan bahwa cara pengelompokan operand tidak memengaruhi hasil operasi.
$(𝐴+(𝐵+𝐶)=(𝐴+𝐵)+𝐶)$
#### B. Sifat Perkalian
- Sifat komutatif adalah salah satu sifat dalam operasi matematika yang menyatakan bahwa urutan operand tidak memengaruhi hasil operasi. Dengan kata lain, jika ( a ) dan ( b ) adalah dua elemen, maka:
perkalian matriks tidak selalu komutatif, sehingga $( A \cdot B \neq B \cdot A )$ dalam banyak kasus.
- Sifat asosiatif adalah salah satu sifat penting dalam operasi matematika yang menyatakan bahwa cara pengelompokan operand tidak memengaruhi hasil operasi.
Sifat asosiatif juga berlaku dalam perkalian matriks: $[ (A \cdot B) \cdot C = A \cdot (B \cdot C) ]$ Tetapi ingat, urutan pengelompokan tetap penting meskipun hasil akhirnya sama. Namun, perkalian matriks tidak bersifat komutatif.

- Sifat distributif kiri adalah salah satu sifat dalam aljabar yang menghubungkan dua operasi, seperti perkalian dan penjumlahan, sehingga memenuhi aturan tertentu. Dalam konteks matriks, sifat distributif kiri menyatakan bahwa:
$[ A \cdot (B + C) = A \cdot B + A \cdot C ]$

- Sifat distributif kanan adalah sifat yang berlaku dalam operasi aljabar, khususnya dalam konteks perkalian dan penjumlahan matriks. Sifat ini menyatakan bahwa:
$[ (A + B) \cdot C = A \cdot C + B \cdot C ]$

#### C. Sifat Perkalian Skalar
- Sifat distributif pada matriks adalah sifat yang menghubungkan operasi penjumlahan dan perkalian matriks, di mana terdapat dua jenis utama: distributif kiri dan distributif kanan.
$𝑎(𝐵+𝐶)=𝑎𝐵+𝑎𝐶$

- Sifat distributif skalar mengacu pada interaksi antara bilangan skalar (angka) dan operasi penjumlahan atau perkalian matriks. Dalam konteks ini, skalar didistribusikan ke setiap elemen matriks atau ke setiap operasi penjumlahan matriks.
$(𝑎+𝑏)𝐶=𝑎𝐶+𝑏𝐶$

- Sifat asosiatif dalam konteks skalar mengacu pada bagaimana pengelompokan operasi perkalian skalar tidak memengaruhi hasil akhir. Dengan kata lain, untuk bilangan skalar ( k ) dan ( c ), serta matriks ( A ), sifat asosiatif skalar dapat dituliskan sebagai:
$[ (k \cdot c) \cdot A = k \cdot (c \cdot A) ]$
- Sifat komutatif skalar menunjukkan bahwa urutan perkalian antara bilangan skalar tidak memengaruhi hasil akhir. Secara matematis, untuk bilangan skalar ( k ) dan ( c ), berlaku:
$[ k \cdot c = c \cdot k ]$

### 2. Invers Aditif Matriks
Invers aditif dari suatu matriks adalah matriks lain yang jika dijumlahkan dengan matriks awal menghasilkan matriks nol (matriks identitas aditif). Secara matematis, jika matriks awal adalah \( A \), maka invers aditif dari \( A \) adalah \( -A \), sehingga:

$[ A + (-A) = 0 ]$

Di mana \( 0 \) adalah matriks nol dengan dimensi yang sama seperti \( A \). Setiap elemen matriks \( -A \) adalah kebalikan (negatif) dari elemen matriks \( A \).

### 3. Matriks Identitas
Matriks identitas adalah matriks persegi (jumlah baris sama dengan jumlah kolom) di mana elemen-elemen pada diagonal utama memiliki nilai \( 1 \), sementara elemen-elemen lainnya adalah \( 0 \). Matriks ini disebut juga sebagai matriks satuan karena berfungsi seperti elemen identitas dalam operasi perkalian matriks, yaitu:

$[ A \cdot I = A ]$
$[ I \cdot A = A ]$

Di mana \( A \) adalah matriks sembarang dengan ukuran yang sesuai, dan \( I \) adalah matriks identitas.

Sebagai contoh, matriks identitas berukuran $( 2 \times 2 )$ adalah:

$$\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$


Sedangkan matriks identitas berukuran $( 3 \times 3 )$ adalah:

$$\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}$$

### 4. Menghitung Invers Matriks
Matriks persegi $A$ memiliki invers $A^{-1}$ jika memenuhi: $A.A^{-1} = A.^{-1} = I$ Artinya, perkalian antara matriks dan inversnya menghasilkan matriks identitas.

Syarat suatu matriks memiliki invers:

Matriks harus berbentuk persegi (jumlah baris sama dengan jumlah kolom).

Determinan matriks tidak boleh nol, yaitu:$[ det (A) \neq \cdot 0)$

### 5. Menghitung Invers dengan OBE
metode OBE (Operasi Baris Elementer) untuk menghitung invers suatu matriks dengan langkah-langkah berikut:

##### a. Menyusun Matriks Augmented

$$[A \ | \ I]$$

##### b. Melakukan Operasi Baris Elementer (OBE)
Lakukan operasi baris hingga sisi kiri menjadi matriks identitas:

$$[I \ | \ A^{-1}]$$

##### c. Mencari Invers matriks
Matriks di sisi kanan setelah eliminasi Gauss-Jordan adalah .Selain itu, gambar juga menampilkan contoh matriks :

$$A = \begin{bmatrix} 2 & 5 \\ 1 & 3 \end{bmatrix}$$

Invers matriks nya dapat dihitung dengan menggunakan rumus:

$$A^{-1} = \frac{1}{\det(A)} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

dan dengan determinan:

$$\det(A) = ad - bc$$

Jika , maka invers bisa dihitung.
### 6. TUGAS
 
1. Buat persamaan 3 variabel dan hitunglah invers x yang hasilnya 1,0,0
### Penyelesaian
#### 1. Bentuk persamaan 3 variabel
$$2X_1 + X_2 + 3X_3 = 5$$
$$X_1 - 2X_2 + X_3 = 2$$
$$3X_1 + X_2 - X_3 = 3$$


#### 2. Bentuk matriks dari persamaan 3 variabel
$$A =\begin{bmatrix}
2 & 1 & 3 &  = 5 \\
1 & -2 & 1 & = 2 \\
3 & 1 & -1 & = 3
\end{bmatrix}$$

#### 3. Bentuk matriks utama dari persamaan 3 variabel

$$A =\begin{bmatrix}
2 & 1 & 3 & \\
1 & -2 & 1 & \\
3 & 1 & -1 & 
\end{bmatrix}$$

#### 4. Bentuk matriks dengan matriks diagonalnya dari persamaan 3 variabel


$$A =\begin{bmatrix}
2 & 1 & 3 & | 1 & 0 & 0 \\
1 & -2 & 1 & | 0 & 1 & 0 \\
3 & 1 & -1 & |0 & 0 & 1
\end{bmatrix}$$

#### 5. Gunakan penyelesaian dengan metode Eliminasi Gauss
- Langkah 4.1 Jadikan baris 1, kolom 1 bernilai 1

$$R_1 = R_1 / 2 $$
$$A =\begin{bmatrix}
1 & 0.5 & 1.5 & | 0.5 & 0 & 0 \\
1 & -2 & 1 & | 0 & 1 & 0\\
3 & 1 & -1 & | 0 & 0 & 1
\end{bmatrix}$$

- Langkah 4.2 Ubah baris 2 kolom 1 dan baris 3 kolom 1 menjadi 0

$$R_2 = R_2 - R_1$$
$$R_3 = R_3 - 3R_1$$
$$A =\begin{bmatrix}
1 & 0.5 & 1.5 & | 0.5 & 0 & 0 \\
0 & -2.5 & -0.5 & | -0.5 & 1 & 0\\
0 & -0.5 & -5.5 & | -1.5 & 0 & 1
\end{bmatrix}$$

- Langkah 4.3 Jadikan baris 2 kolom 2 bernilai 1

$$R_2 = R_2 / - 2.5$$
$$A =\begin{bmatrix}
1 & 0.5 & 1.5 & | 0.5 & 0 & 0 \\
0 & 1 & 0.2 & | 0.2 & -0.4 & 0\\
0 & -0.5 & -5.5 & | -1.5 & 0 & 1
\end{bmatrix}$$

- Langkah 4.4 Ubah baris 1 kolom 2 menjadi 0

$$R_1 = R_1 / - 0.5 R_2$$
$$A =\begin{bmatrix}
1 & 0 & 1.4 & | 0.4 & 0.2 & 0 \\
0 & 1 & 0.2 & | 0.2 & -0.4 & 0\\
0 & -0.5 & -5.5 & | -1.5 & 0 & 1
\end{bmatrix}$$

- Langkah 4.5 Ubah baris 3 kolom 3 menjadi 1

$$R_3 = R_3 / - 5.5$$
$$A =\begin{bmatrix}
1 & 0 & 1.4 & | 0.4 & 0.2 & 0 \\
0 & 1 & 0.2 & | 0.2 & -0.4 & 0\\
0 & -0.0909 & 1 & | 0.2727 & 0 & -0.1818
\end{bmatrix}$$

- Langkah 4.6 Ubah baris 1 kolom 3 menjadi 0

$$R_1 = R_1 / - 1.4 R_3$$
$$A =\begin{bmatrix}
1 & -0.127 & 0 & | 0.018 & 0.2 & 0.255 \\
0 & 1 & 0.2 & | 0.2 & -0.4 & 0\\
0 & 0.091 & 1 & | 0.273 & 0 & -0.182
\end{bmatrix}$$

- Langkah 4.7 Ubah baris 2 kolom 3 menjadi 0

$$R_2 = R_2 / - 0.2 R_3$$
$$A =\begin{bmatrix}
1 & -0.127 & 0 & | 0.018 & 0.2 & 0.255 \\
0 & 0.982 & 0 & | 0.145 & -0.4 & 0.036 \\
0 & 0.091 & 1 & | 0.273 & 0 & -0.182
\end{bmatrix}$$

#### 6. Setelah itu gunakan rumus invers$(Ax= B)$

$Ax = B$
$A^{-1}Ax = A^{-1}B$
$Ix = A^{-1}B$
$x= A^{-1}B$

hasil perhitungan dari persamaan  variabel

$$A^{-1} =
\begin{bmatrix}
0.037 & 0.148 & 0.259 \\
0.148 & -0.407 & 0.037 \\
0.259 & 0.037 & -0.185
\end{bmatrix}$$

$$\begin{bmatrix}
x\\
y \\
z\end{bmatrix}= \begin{bmatrix}
0.037 & 0.148 & 0.259 \\
0.148 & -0.407 & 0.037 \\
0.259 & 0.037 & -0.185
\end{bmatrix}= \begin{bmatrix}
5\\
2 \\
3\end{bmatrix}=\begin{bmatrix}
1\\
0 \\
0\end{bmatrix}$$