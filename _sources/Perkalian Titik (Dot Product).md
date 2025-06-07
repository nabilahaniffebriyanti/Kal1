---
title: Perkalian Titik (Dot Product)

---

# Perkalian Titik (Dot Product)
## Definisi
**Dot product** (atau hasil skalar) adalah cara mengalikan dua vektor, dan hasilnya adalah sebuah angka (skalar). atau Perkalian titik itu cara buat ngukur seberapa searah dua vektor.

Untuk vektor-vektor dua dimensi v dan w, hasil kali titik (v · w) dapat didefinisikan sebagai bilangan skalar sebagai berikut:

Misal dua vektor:

$$\mathbf{v} = \begin{bmatrix} v_1 \\ v_2 \end{bmatrix}, \quad \mathbf{w} = \begin{bmatrix} w_1 \\ w_2 \end{bmatrix}$$

Perkalian titiknya (dot product) dari 2 vektor adalah:

$$\mathbf{v} \cdot \mathbf{w} = v_1 w_1 + v_2 w_2$$

#### CONTOH 
Langkah pertama : menentukan dua vektor 

$$\mathbf{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \mathbf{w} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$$

Langkah kedua : hitung dot product

$$\vec{v} . \vec{w} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
\cdot \begin{bmatrix} -1 \\ 2 \end{bmatrix}$$

$$= 2 \times -1 + 1 \times 2$$ 

$$= -2 + 2$$ 

$$= 0$$

jika hasil dari dua vektor tersebut 0 maka kedua vektor tersebut memiliki garis yang sejajar dan memiliki sudut 90°

![vektor u,v](https://hackmd.io/_uploads/SkdBwP7zge.png)

[https://www.geogebra.org/classic/tnsb5s84](https://)

#### CONTOH BASIS ADA 2 MACAM YAITU : 

##### 1. Basis 2D ada 2 yaitu : 

$$\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$

dot product yaitu : 

$$\begin{bmatrix} 1 \\ 0 \end{bmatrix}
\cdot \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

$$= 1 \cdot 0 + 0 \cdot 1$$ 

$$= 0$$

##### 2. Basis 3D ada 3 yaitu : 

$$\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}$$

dot product yaitu : 

$$b1 =\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, b2 =\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}, b3 =\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix} $$

$$b1 \cdot b2 =\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix},\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix} = (1 \cdot 0) + (0 \cdot 1)+(0 \cdot 0) =0$$

$$b1 \cdot b3 =\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix},\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix} = (1 \cdot 0) + (0 \cdot 0)+(0 \cdot 1) =0$$

$$b2 \cdot b3 =\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix},\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix} = (0 \cdot 0) + (1 \cdot 0)+(0 \cdot 1) =0$$

## Perkalian titik dan Panjang Vektor
**Panjang vektor** adalah seberapa "besar" vektor tersebut, yang diukur dari titik asal (0,0) ke titik ujung vektor. Istilah lainnya adalah **norma**.

panjang vektor atau jarak titik dapat dihitung menggunakan Teorema Pythagoras, dengan rumus : 

$$\text{Panjang vektor } \mathbf{x} = \sqrt{x^2 + y^2}.$$

Dimana x hasil dari vektor yang berada di sumbu x dan y juga sebaliknya hasil dari vektor yang berada di sumbu y.

$${u} = (2, 1), \quad {v} = (-1, 2)$$

$$|\vec{u}| = \sqrt{2^2 + 1^2}$$

$$= \sqrt{5}$$

$$|\vec{v}| = \sqrt{(-1)^2 + 2^2}$$

$$= \sqrt{5}$$

Artinya: kita kuadratkan setiap angka, lalu jumlahkan semuanya, dan ambil akar kuadrat dari hasil penjumlahan itu.