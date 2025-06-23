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

#### CONTOH 1
Langkah pertama : menentukan dua vektor 

$$\mathbf{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \mathbf{w} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$$

Langkah kedua : hitung dot product

$$\vec{v} . \vec{w} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
\cdot \begin{bmatrix} -1 \\ 2 \end{bmatrix}$$

$$= 2 \times -1 + 1 \times 2$$ 

$$= -2 + 2$$ 

$$= 0$$

jika hasil dari dua vektor tersebut 0 maka kedua vektor tersebut memiliki garis yang sejajar dan memiliki sudut 90°

<iframe src="https://www.geogebra.org/material/iframe/id/tnsb5s84/width/800/height/600/border/888888/rc/false/ai/true/sdz/true/smb/false/stb/false" width="800" height="600" style="border:0px;"> </iframe>

#### CONTOH 2

Langkah pertama : menentukan dua vektor 

$$\mathbf{v} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}, \mathbf{w} = \begin{bmatrix} -3 \\ -4 \end{bmatrix}$$

Langkah kedua : hitung dot product

$$\vec{v} . \vec{w} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}
\cdot \begin{bmatrix} -3 \\ 4 \end{bmatrix}$$

$$= 3 \times -3 + 4 \times -4$$ 

$$= -9 - 16$$ 

$$= -25$$

jika hasil dari dua vektor tersebut -(minus) maka kedua vektor tersebut memiliki garis yang berlawanan arah dan memiliki sudut 180°

<iframe src="https://www.geogebra.org/material/iframe/id/px9u4fkv/width/800/height/600border888888rc/false/ai/false/sdz/false/sfsb/true/stb/false"allowfullscreen>
</iframe>

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