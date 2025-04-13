---
title: transformasi matriks

---

# TRANSFORMASI MATRIKS
## PENGERTIAN
Matriks Transformasi adalah matriks yang mengubah satu vektor menjadi vektor lain melalui proses perkalian matriks.

Matriks transformasi mengubah sistem kartesius dan memetakan koordinat vektor ke koordinat baru. Matriks transformasi T dengan orde ( mxn ) pada perkalian dengan vektor A dengan n komponen yang direpresentasikan sebagai matriks kolom mengubahnya menjadi matriks lain yang merepresentasikan vektor baru A'.

Untuk ruang vektor dua dimensi, matriks transformasi berorde 2 x 2, dan untuk ruang n dimensi, matriks transformasi berorde (n x n).

### A. Perkalian Matriks-Vektor
Perkalian Matriks-Vektor adalah operasi matematika di mana sebuah matriks dikalikan dengan sebuah vektor. Hasilnya adalah vektor baru.
Secara matematis, jika Anda memiliki matriks (A) berukuran ($m \times n$) (m baris dan n kolom) dan vektor (x) dengan panjang (n), perkalian matriks-vektor (Ax) menghasilkan vektor baru (b) dengan panjang (m). Setiap elemen dalam vektor hasil adalah kombinasi linear dari elemen-elemen di vektor awal, berdasarkan baris matriks.

#### Contoh 5.1.1 Perkalian vektor dengan matriks.

Misalkan  A adalah sebuah matriks, dan y,z serta $\vec{x}$, dan  $\vec{y}$ adalah vektor-vektor seperti yang diberikan di bawah ini.

Diketahui : $$A = \begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}, \quad 
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad 
\vec{y} = \begin{bmatrix} -1 \\ 1 \end{bmatrix}, \quad 
\vec{z} = \begin{bmatrix} 3 \\ -1 \end{bmatrix}$$

Grafik $\vec{x}$, $\vec{y}$, $\vec{z}$, serta $A\vec{x}$, $A\vec{y}$, dan $A\vec{z}$.

langkah-langkah: 
1. Menghitung $A\vec{x}$:

$$A\vec{x} = 
\begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix} 
\begin{bmatrix} 1 \\ 1 \end{bmatrix} = 
\begin{bmatrix} (1)(1) + (4)(1) \\ (2)(1) + (3)(1) \end{bmatrix} = 
\begin{bmatrix} 1 + 4 \\ 2 + 3 \end{bmatrix} = 
\begin{bmatrix} 5 \\ 5 \end{bmatrix}$$

2. Menghitung $A\vec{y}$ :

$$A\vec{y} = 
\begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix} 
\begin{bmatrix} -1 \\ 1 \end{bmatrix} = 
\begin{bmatrix} (1)(-1) + (4)(1) \\ (2)(-1) + (3)(1) \end{bmatrix} = 
\begin{bmatrix} -1 + 4 \\ -2 + 3 \end{bmatrix} = 
\begin{bmatrix} 3 \\ 1 \end{bmatrix}$$

3. Menghitung $A\vec{z}$:

$$A\vec{z} = 
\begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix} 
\begin{bmatrix} 3 \\ -1 \end{bmatrix} = 
\begin{bmatrix} (1)(3) + (4)(-1) \\ (2)(3) + (3)(-1) \end{bmatrix} = 
\begin{bmatrix} 3 - 4 \\ 6 - 3 \end{bmatrix} = 
\begin{bmatrix} -1 \\ 3 \end{bmatrix}$$

kesimpulan :

$$A\vec{x} = \begin{bmatrix} 5 \\ 5 \end{bmatrix}, \quad 
A\vec{y} = \begin{bmatrix} 3 \\ 1 \end{bmatrix}, \quad 
\text{dan} \quad A\vec{z} = \begin{bmatrix} -1 \\ 3 \end{bmatrix}.$$

hasil grafiknya :
![Screenshot 2025-04-10 145717](https://hackmd.io/_uploads/rJyXseSRyg.png)

#### Contoh 5.1.3 Menggabungkan penjumlahan dan perkalian matriks.

Misalkan A adalah sebuah matriks dan y,z serta  $\vec{x}$, dan $\vec{y}$ adalah vektor-vektor seperti yang diberikan di bawah ini.

$$A = \begin{bmatrix} 1 & 1 \\ 1 & 2 \end{bmatrix}, \quad 
\vec{x} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \quad 
\vec{y} = \begin{bmatrix} -1 \\ 1 \end{bmatrix}.$$

Grafik $\vec{x}$ + $\vec{y}$, $A\vec{x}$, $A\vec{y}$ dan $A(\vec{x}$ + $\vec{y})$.

langkah-langkah : 

1. Penjumlahan vektor:

$$\vec{x} + \vec{y} = 
\begin{bmatrix} 2 \\ 1 \end{bmatrix} + \begin{bmatrix} -1 \\ 1 \end{bmatrix} = 
\begin{bmatrix} 2 + (-1) \\ 1 + 1 \end{bmatrix} = 
\begin{bmatrix} 1 \\ 2 \end{bmatrix}$$

2. Perkalian matriks dengan vektor :

$$A\vec{x} = 
\begin{bmatrix} 1 & 1 \\ 1 & 2 \end{bmatrix} 
\begin{bmatrix} 2 \\ 1 \end{bmatrix} =
\begin{bmatrix}
(1)(2) + (1)(1) \\
(1)(2) + (2)(1)
\end{bmatrix} =
\begin{bmatrix} 2 + 1 \\ 2 + 2 \end{bmatrix} = 
\begin{bmatrix} 3 \\ 4 \end{bmatrix}$$

3. Perkalian matriks dengan vektor :

$$A\vec{y} = 
\begin{bmatrix} 1 & 1 \\ 1 & 2 \end{bmatrix} 
\begin{bmatrix} -1 \\ 1 \end{bmatrix} =
\begin{bmatrix}
(1)(-1) + (1)(1) \\
(1)(-1) + (2)(1)
\end{bmatrix} =
\begin{bmatrix} -1 + 1 \\ -1 + 2 \end{bmatrix} = 
\begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

4. Perkalian matriks dengan hasil penjumlahan vektor:

$$A(\vec{x} + \vec{y}) = 
A \begin{bmatrix} 1 \\ 2 \end{bmatrix} =
\begin{bmatrix} 1 & 1 \\ 1 & 2 \end{bmatrix} 
\begin{bmatrix} 1 \\ 2 \end{bmatrix} =
\begin{bmatrix}
(1)(1) + (1)(2) \\
(1)(1) + (2)(2)
\end{bmatrix} =
\begin{bmatrix} 1 + 2 \\ 1 + 4 \end{bmatrix} =
\begin{bmatrix} 3 \\ 5 \end{bmatrix}$$

kesimpulan :

$$\vec{x} + \vec{y} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}; \quad 
A\vec{x} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}; \quad 
A\vec{y} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}; \quad 
A(\vec{x} + \vec{y}) = \begin{bmatrix} 3 \\ 5 \end{bmatrix}.$$

Hasil grafiknya :
![Screenshot 2025-04-10 150123](https://hackmd.io/_uploads/SJdDTgSR1l.png)

#### Contoh 5.1.5 Menggambarkan efek dari perkalian matriks.

Misalkan $A$, $\vec{x}$, $\vec{y}$, dan $\vec{z}$ didefinisikan sebagai berikut:

$$A = \begin{bmatrix} 1 & -1 \\ 1 & -1 \end{bmatrix}, \quad 
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad 
\vec{y} = \begin{bmatrix} -1 \\ 1 \end{bmatrix}, \quad 
\vec{z} = \begin{bmatrix} 4 \\ 1 \end{bmatrix}$$

Gambarkan $\vec{x}$, $\vec{y}$, dan $\vec{z}$ serta $A\vec{x}$, $A\vec{y}$, dan $A\vec{z}$.

Kesimpulan :

$$A\vec{x} = 
\begin{bmatrix} 0 \\ 0 \end{bmatrix}, \quad 
A\vec{y} = 
\begin{bmatrix} -2 \\ -2 \end{bmatrix}, \quad 
A\vec{z} = 
\begin{bmatrix} 3 \\ 3 \end{bmatrix}$$

### B. Transformasi Bidang Cartesian
Perubahan posisi atau bentuk dari suatu objek di bidang datar (2 dimensi) menggunakan operasi matematika tertentu. Dalam sistem koordinat Cartesian (x, y), transformasi ini biasanya dilakukan dengan menggunakan matriks transformasi.

#### Contoh 5.1.7 Memvisualisasikan transformasi matriks menggunakan vektor.

Gambarkan vektor-vektor dari persegi satuan sebelum dan sesudah dikalikan dengan matriks , di mana:

$$A = \begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}$$

Solusi

- Empat sudut dari persegi satuan dapat direpresentasikan oleh vektor-vektor:

$$\begin{bmatrix} 0 \\ 0 \end{bmatrix}, \quad
\begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad
\begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad
\begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

- Mengalikan masing-masing vektor dengan matriks  menghasilkan :

$$\begin{bmatrix} 0 \\ 0 \end{bmatrix}, \quad
\begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad
\begin{bmatrix} 5 \\ 5 \end{bmatrix}, \quad
\begin{bmatrix} 4 \\ 3 \end{bmatrix}$$

(untuk mempercepat perhitungan  maka kita bisa membuat matriks berukuran 2 × 4 yang kolom-kolomnya merupakan vektor-vektor tersebut. 

$$B = \begin{bmatrix} 0 & 1 & 1 & 0 \\ 0 & 0 & 1 & 1 \end{bmatrix}$$

Kemudian kalikan $A$ dengan $B$, dan hasil transformasi dapat dibaca langsung dari kolom-kolomnya:

$$AB = \begin{bmatrix} 0 & 1 & 5 & 4 \\ 0 & 2 & 5 & 3 \end{bmatrix}$$

Kita bisa mudah dengan melewatkan kolom pertama (karena itu adalah kolom nol, hasilnya akan tetap nol setelah dikalikan dengan $A$ ).

![Screenshot 2025-04-10 195055](https://hackmd.io/_uploads/HkmTAVHCkl.png)

Persegi satuan dan transformasinya digambarkan dalam Gambar diatas.
Di mana titik sudut yang berbentuk saling bersesuaian di kedua grafik. Perhatikan bagaimana persegi berubah menjadi semacam segi empat.(sebenarnya itu adalah jajaran genjang). Hal yang sangat menarik adalah bagaimana titik sudut segitiga dan persegi tampak berubah tempat—seolah-olah persegi, selain diregangkan hingga keluar bentuknya, juga terbalik.

#### Contoh 5.1.10 Memvisualisasikan transformasi matriks menggunakan suatu wilayah.

Gambarkan persegi satuan yang telah ditransformasikan setelah ditransformasikan oleh A,dimana : 
solusi Matriks transformasi:

$$A = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$$

Matriks ini adalah rotasi searah jarum jam sebesar 90 derajat terhadap vektor di bidang 2D.

Sebelum Transformasi:

Empat titik sudut persegi satuan adalah :

$$\begin{bmatrix} 0 \\ 0 \end{bmatrix}, 
\begin{bmatrix} 1 \\ 0 \end{bmatrix}, 
\begin{bmatrix} 1 \\ 1 \end{bmatrix}, 
\begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

Ini dikumpulkan dalam matriks :

$$B = \begin{bmatrix}
0 & 1 & 1 & 0 \\
0 & 0 & 1 & 1
\end{bmatrix}$$

Kalikan dengan :

$$AB = A \cdot B = 
\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}=
\begin{bmatrix}
0 & 1 & 1 & 0 \\
0 & 0 & 1 & 1
\end{bmatrix} =
\begin{bmatrix}
0 & 0 & -1 & -1 \\
0 & 1 & 1 & 0
\end{bmatrix}$$

Empat titik baru setelah transformasi adalah :

1. Titik [0,0] tetap [0,0]
2. Titik [1,0] menjadi [0,1]
3. Titik [1,1] menjadi [−1,1]
4. Titik [0,1] menjadi [−1,0]

satuan persegi kembali digambar bersama dengan transformasinya pernyataan oleh A.
![Screenshot 2025-04-10 220207](https://hackmd.io/_uploads/ByVaT8HCyg.png)

#### Contoh 5.1.12 Menentukan transformasi matriks.
Cari matriks  yang membalik bidang Cartesian terhadap sumbu-x dan kemudian meregangkan bidang secara horizontal dengan faktor dua.

Solusi : 
mempertimbangkan $\vec{e_1} = \begin{bmatrix} 1 & 0 \end{bmatrix}$. Ke mana sudut ini pergi setelah transformasi diberikan? Membalik bidang terhadap sumbu-x tidak mengubah $\vec{e_1}$ sama sekali, meregangkan bidang mengubah $\vec{e_1}$ menjadi $\begin{bmatrix} 2 & 0 \end{bmatrix}$ . Oleh karena itu, kolom pertama dari matriks $A$ adalah $\begin{bmatrix} 0 & -1 \end{bmatrix}$.

Sekarang pertimbangkan $\vec{e_2}$. Membalik bidang terhadap sumbu-x mengubah $\vec{e_2}$   menjadi vektor $\begin{bmatrix} 0 & -1 \end{bmatrix}$ ; kemudian meregangkan bidang secara horizontal tidak mempengaruhi vektor ini. Oleh karena itu, kolom kedua dari $A$ adalah $\begin{bmatrix} 0 & -1 \end{bmatrix}$.

Menggabungkan semuanya, kita dapatkan:

$$A = \begin{bmatrix} 2 & 0 \\ 0 & -1 \end{bmatrix}$$

![Screenshot 2025-04-13 135551](https://hackmd.io/_uploads/SyuBekt0kl.png)

Di mana suatu bentuk ditransformasikan di bawah matriks ini. Perhatikan bagaimana bentuk tersebut dibalik dan diregangkan secara horizontal dengan faktor dua. (Garis kisi diberikan sebagai bantuan visual.)

### C. 2D Matrix Transformations
Transformasi matriks 2D adalah cara menggunakan matriks untuk mengubah posisi, ukuran, atau orientasi titik-titik atau bentuk-bentuk dalam ruang dua dimensi.

1. Peregangan horizontal dengan faktor k.
$\begin{bmatrix} k & 0 \\ 0 & 1 \end{bmatrix}$
2. Peregangan vertikal dengan faktor k.
$\begin{bmatrix} 1 & 0 \\ 0 & k \end{bmatrix}$
3. Geser horizontal dengan faktor k.
$\begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}$
4. Geser vertikal dengan faktor k.
$\begin{bmatrix} 1 & 0 \\ k & 1 \end{bmatrix}$
5. Refleksi vertikal sepanjang sumbu y.
$\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}$
6. Refleksi horizontal sepanjang sumbu x.
$\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$
7. Refleksi diagonal melintasi garis y=x.
$\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$
8. Rotasi di sekitar titik asal dengan sudut θ.
$\begin{bmatrix} cos & -sin0 \\ sin0 & cos0 \end{bmatrix}$

### Tugas
#### Menghitung hasil perkalian matriks  dengan vektor $\vec{x}$, $\vec{y}$, $A\vec{x}$, dan $A\vec{y}$, lalu menggambar keempat vektor  pada bidang Cartesius.

Dengan Diketahui :

$$\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}  dan \quad \vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$$

1. $A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}$

##### Diketahui : 
$A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}$, $\quad \vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad \vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$

langkah-langkah penyelesaian : 
##### 1. Menghitung vektor $A\vec{x}$ :

$A\vec{x} = 
\begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
\begin{bmatrix} 1 \\ 1 \end{bmatrix} =
\begin{bmatrix} 1(1) + (-1)(1) \\ 2(1) + 3(1) \end{bmatrix} =
\begin{bmatrix} 0 \\ 5 \end{bmatrix}$

##### 2. Menghitung vektor $A\vec{y}$ :

$A\vec{y} =
\begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
\begin{bmatrix} -1 \\ 2 \end{bmatrix} =
\begin{bmatrix} (1)(-1) + (-1)(2) \\ (2)(-1) + (3)(2) \end{bmatrix} =
\begin{bmatrix} -3 \\ 4 \end{bmatrix}$

##### Kesimpulan :

Vektor $\vec{x}$ berubah dari ( 1, 1 ) menjadi ( 0, 5 ) : digeser ke atas.

Vektor $\vec{y}$ berubah dari ( -1, 2 ) ke( -3, 4 ) : digeser ke kiri dan ke atas.

hasil grafik carterius vektor diatas : 

![image](https://hackmd.io/_uploads/Sys87GrCkg.png)


2. $A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}$

##### Diketahui :

$A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}$, $\quad \vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad \vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$

langkah-langkah penyelesaian : 

##### 1. Menghitung vektor $A\vec{x}$ :

$A\vec{x} =
\begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
\begin{bmatrix} 1 \\ 1 \end{bmatrix} =
\begin{bmatrix} 2(1) + 0(1) \\ -1(1) + 3(1) \end{bmatrix} =
\begin{bmatrix} 2 \\ 2 \end{bmatrix}$

##### 2. Menghitung vektor $A\vec{y}$ :

$A\vec{y} =
\begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
\begin{bmatrix} -1 \\ 2 \end{bmatrix} =
\begin{bmatrix} 2(-1) + 0(2) \\ -1(-1) + 3(2) \end{bmatrix} =
\begin{bmatrix} -2 \\ 1 + 6 \end{bmatrix} =
\begin{bmatrix} -2 \\ 7 \end{bmatrix}$

##### Kesimpulan :

##### - Matriks ini memiliki efek skala dan rotasi sebagian :

- Baris pertama $\begin{bmatrix} 2 & 0 \\ \end{bmatrix}$ : mengalikan komponen x, memengaruhi arah horizontal.

- Baris kedua $\begin{bmatrix} -1 & 3 \\ \end{bmatrix}$: mencampur antara x dan y.

##### - Hasil transformasi dari $\vec{x}$ , dan $\vec{y}$ memperpanjang vektor dan mengubah arah secara tidak simetris.

hasil grafik carterius vektor diatas : 
![Screenshot 2025-04-10 164726](https://hackmd.io/_uploads/rkMy4fBAye.png)

5. mencari matriks transformasi $A$ yang mengubah unit square menjadi bentuk yang ditampilkan pada masing-masing gambar (soal 5 dan 6). 
![Screenshot 2025-04-10 164907](https://hackmd.io/_uploads/rkhQNzH0yl.png)

Matriks transformasi $A$ bekerja dengan cara mengubah:

- $\vec{i} = \begin{bmatrix} 1 & 0 \end{bmatrix}$
- $\vec{j} = \begin{bmatrix} 0 & 1 \end{bmatrix}$

Transformasi matriks  akan mengubah vektor  dan  menjadi vektor baru yang menjadi kolom-kolom dari matriks .

- Titik  $\vec{i}$ = (1, 0) dipetakan ke (1, 2) → kolom pertama matriks (bentuk persegi).

- Titik $\vec{j}$ = (0, 1)  dipetakan ke (2, 3) → kolom kedua matriks (bentuk segitiga).

- Titik ( 1, 1 ) menjadi ( 1+2, 2+3 )=(3,5)(bentuk lingkaran).

Sebuah matriks A berfungsi seperti : 
$A$ . $\vec{i}$ = kolom pertama, $A$ . $\vec{j}$ = kolom kedua
karena  $A\vec{i}$ = (1, 2) dan $A\vec{j}$ = (2, 3)
Maka:

$$A = \begin{bmatrix} 1 & 2 \\ 2 & 3 \end{bmatrix}$$

hasil : 
vektor $\vec{x} = \begin{bmatrix} 1 & 1\end{bmatrix}$, yaitu titik ( 1,1 ): 

$$A = \begin{bmatrix} 1 & 2 \\ 2 & 3 \end{bmatrix} \begin{bmatrix} 1\\1 \end{bmatrix} = \begin{bmatrix} 1 + 2 \\ 2 + 3 \end{bmatrix} = \begin{bmatrix} 3\\5 \end{bmatrix}$$

kesimpulan : 
jadi : $$A = \begin{bmatrix} 1 & 2 \\ 2 & 3 \end{bmatrix}$$

![Screenshot 2025-04-10 165940](https://hackmd.io/_uploads/S1uiLfrRkl.png)

- $\vec{i} = \begin{bmatrix} 1 & 0 \end{bmatrix}$ → ujung kanan bawah
- $\vec{j} = \begin{bmatrix} 0 & 1 \end{bmatrix}$ → ujung kiri atas

Transformasi matriks  akan mengubah vektor  dan  menjadi vektor baru yang menjadi kolom-kolom dari matriks .

- Titik  $\vec{i}$ = (1, 0) dipetakan ke (1, 1) → (tanda kotak).
- Titik $\vec{j}$ = (0, 1)  dipetakan ke (-1, 1) → (tanda segitiga).
- Gabungan dari kedua dapat dipetakan ke (1+ (-1), 1+1)=(0,2)(lingkaran)

Maka:

$$A = \begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix}$$

hasil : 
vektor $\vec{x} = \begin{bmatrix} 1 & 1\end{bmatrix}$, yaitu titik ( 1,1 ): 

$$A = \begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} 1\\1 \end{bmatrix} = \begin{bmatrix} 1 + (-1) \\ 1 + 1 \end{bmatrix} = \begin{bmatrix} 0\\2 \end{bmatrix}$$

kesimpulan : 
jadi : 
$$A = \begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix}$$