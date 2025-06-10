---
title: transformasi linier

---

# TRANSFORMASI LINIER

## PENGERTIAN
### Apa Transformasi Linier??
Fungsi T yang memetakan ruang vektor V ke ruang vektor W.

V : domain T
W : codomain T 

Dengan memenuhi dua sifat yaitu : 
### 1. Penjumlahan Vektor :

$$T(u+v)=T(u)+T(v)$$

Fungsi tersebut harus bersifat aditif, yang artinya menjumlahkan dua vektor dan kemudian memetakannya dan akan menghasilkan hasil yang sama dengan menjumlahkan hasil pemetaan masing-masing vektor.

### 2. Perkalian Skalar :

$$T(c.v)=c.T (v)$$

Fungsi tersebut harus bersifat homogen, yang artinya mengalikan vektor dengan skalar yang akan menghasilkan hasil yang sama dengan mengalikan hasil fungsi tersebut dengan skalar yang sama.

## TUGAS

### 1. membuktikan bahwa $T =(v1,v2)=(v1+v2,v1)$ adalah tranformasi linier.

PEMBUKTIANNYA DENGAN 2 SYARAT : 
#### 1. Penjumlahan Vektor : 
Syaratnya: $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$

Kalau kita jumlahkan 2 vektor dulu baru ditransformasi, hasilnya harus sama dengan kalau masing-masing vektor ditransformasi dulu, lalu hasilnya dijumlahkan.

Misalkan : 

$u = (u1,u2)$

$v = (v1,v2)$

Langkah-langkah : 


$$=T (\mathbf{u}+\mathbf{v})$$

$$=T(u_1 + v_1, u_2 + v_2)$$

$$= ((u_1 + v_1) + (u_2 + v_2), u_1 + v_1)$$

$$= (u_1 + u_2 + v_1 + v_2, u_1 + v_1)$$

$$= (u_1 + u_2, u_1) + (v_1 + v_2, v_1)$$

$$= T(\mathbf{u}) + T(\mathbf{v})$$

#### 2. Perkalian skalar
Syaratnya : $T(c\mathbf{v})=cT (\mathbf{v})$

Misalkan: 
$\mathbf{v} = v1 , v2$
, dan c bilangan skalar (real number).

Langkah-langkah : 

$$T(c \mathbf{v}) = T(c v_1, c v_2)$$

$$= (c v_1 + c v_2, c v_1)$$

$$= c (v_1 + v_2, v_1)$$

$$= (c (v_1 + v_2), c v_1)$$

$$= (c v_1 + c v_2, c v_1)$$

$$= c (v_1 + v_2, v_1)$$

$$= c T(\mathbf{v})$$

### 2. Buat 2 contoh titik masing-masing

#### a. Reflection about the x-axis
- Matriks
$\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}$

- Titik A. ( 4, -1 )
$\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
\times
\begin{bmatrix}
4 \\
-1
\end{bmatrix}
=
\begin{bmatrix}
1 \times 4 + 0 \times -1 \\
0 \times 4 + (-1) \times -1
\end{bmatrix}
=
\begin{bmatrix}
4 \\
1
\end{bmatrix}$

Jadi hasilnya A'(4, 1)

- Titik B. ( -2, 5 )
$\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
\times
\begin{bmatrix}
-2 \\
5
\end{bmatrix}
=
\begin{bmatrix}
-2 \\
-5
\end{bmatrix}$

Jadi hasilnya B'(-2, -5)

#### b. Reflection about the y-axis
- Matriks
$\begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix}$

- Titik A. ( 4, 6 )
$\begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix}
\times
\begin{bmatrix}
4 \\
6
\end{bmatrix}
=
\begin{bmatrix}
-1 \times 4 + 0 \times 6 \\
0 \times 4 + (-1) \times 6
\end{bmatrix}
=
\begin{bmatrix}
-4 \\
6
\end{bmatrix}$

Jadi hasilnya A'(-4, 6)

- Titik B. ( -3, -7 )
$\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
\times
\begin{bmatrix}
-3 \\
-7
\end{bmatrix}
=
\begin{bmatrix}
3 \\
-7
\end{bmatrix}$

Jadi hasilnya B'(3, -7)

#### c. Reflection about the line y=x
- Matriks
$\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}$

- Titik A. ( 2, 5 )
$\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
\times
\begin{bmatrix}
2 \\
5
\end{bmatrix}
=
\begin{bmatrix}
0 \times 2 + 1 \times 5 \\
1 \times 2 + 0 \times 5
\end{bmatrix}
=
\begin{bmatrix}
5 \\
2
\end{bmatrix}$

Jadi hasilnya A'(5, 2)

- Titik B. ( -3, 7 )
$\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
\times
\begin{bmatrix}
-3 \\
7
\end{bmatrix}
=
\begin{bmatrix}
0 \times -3 + 1 \times 7 \\
1 \times -3 + 0 \times 7
\end{bmatrix}
=
\begin{bmatrix}
7 \\
-3
\end{bmatrix}$

Jadi hasilnya B'(7, -3)

#### d. Reflection about the line y = -x
- Matriks
$\begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix}$

- Titik A. ( 3, 7 )
$\begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix}
\times
\begin{bmatrix}
3 \\
7
\end{bmatrix}
=
\begin{bmatrix}
0 \times 3 + 1 \times 7 \\
1 \times 3 + 0 \times 7
\end{bmatrix}
=
\begin{bmatrix}
-7 \\
-3
\end{bmatrix}$

Jadi hasilnya A'(-7, -3)

- Titik B. ( -4, 2 )
$\begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix}
\times
\begin{bmatrix}
-4 \\
2
\end{bmatrix}
=
\begin{bmatrix}
0 \times -4 + 1 \times 2 \\
1 \times -4 + 0 \times 2
\end{bmatrix}
=
\begin{bmatrix}
-2 \\
4
\end{bmatrix}$

Jadi hasilnya B'(-2, 4)

#### e. Reflection about the origin
- Matriks
$\begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix}$

- Titik A. ( 5, -3 )
$\begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix}
\times
\begin{bmatrix}
5 \\
-3
\end{bmatrix}
=
\begin{bmatrix}
0 \times 5 + 1 \times -3 \\
1 \times 5 + 0 \times -3
\end{bmatrix}
=
\begin{bmatrix}
-5 \\
3
\end{bmatrix}$

Jadi hasilnya A'(-5, 3)

- Titik B. ( -2, 6 )
$\begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix}
\times
\begin{bmatrix}
-2 \\
6
\end{bmatrix}
=
\begin{bmatrix}
0 \times -2 + 1 \times 6 \\
1 \times -2 + 0 \times 6
\end{bmatrix}
=
\begin{bmatrix}
2 \\
-6
\end{bmatrix}$

Jadi hasilnya B'(2, -6)