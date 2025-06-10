---
title: Perkalian silang (cross Product)

---

# Perkalian Silang (cross Product)
## Definisi
**Cross product** 
adalah operasi perkalian dengan dua operand (objek yang dikalikan) berupa vektor. Tetapi hasil operasi ini tidak selalu adalah vektor.

$$\mathbf{u} = \begin{bmatrix} u_1 \\ u_2 \\ u_3 \end{bmatrix} dan \quad \mathbf{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}$$

Rumus hasil kali dari $\vec{u}$ dan $\vec{v}$, di notasikan seperti di bawah :  

$$\vec{u} \times \vec{v} = \begin{bmatrix}
u_2 v_3 - u_3 v_2 \\
-(u_1 v_3 - u_3 v_1) \\
u_1 v_2 - u_2 v_1
\end{bmatrix}$$

atau bisa dengan cara Menggunakan determinan untuk menemukan perkalian silang.

atau jika ingin mengetahui $\vec{v} \times \vec{u}$ maka rumus dibawah tinggal di balik.

Pertama, kita membentuk array $3 \times 3$ seperti yang ditunjukkan di bawah ini.

$$\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3 \\ \end{vmatrix}$$


$$\vec{u} \times \vec{v} = \begin{vmatrix}
u_2 & u_3 \\
v_2 & v_3 \end{vmatrix} 
\vec{i} - \begin{vmatrix}
u_1 & u_3 \\
v_1 & v_3 \end{vmatrix} 
\vec{j} + \begin{vmatrix}
u_1 & u_2 \\
v_1 & v_2 \end{vmatrix} \vec{k}$$

$$= (u_2 v_3 - u_3 v_2)\vec{i} - (u_1 v_3 - u_3 v_1)\vec{j} + (u_1 v_2 - u_2 v_1)\vec{k}$$

## SIFAT-SIFAT PERKALIAN SILANG


1. $\vec{u} \times \vec{v} = -(\vec{v} \times \vec{u})$  {Anticommutative Property}

2. a. $(\vec{u} + \vec{v}) \times \vec{w} = \vec{u} \times \vec{w} + \vec{v} \times \vec{w}$

   b. $\vec{u} \times (\vec{v} + \vec{w}) = \vec{u} \times \vec{v} + \vec{u} \times \vec{w}$ {Distributive Properties}
    
3. $c(\vec{u} \times \vec{v}) = (c \vec{u}) \times \vec{v} = \vec{u} \times (c \vec{v})$
    
4. a. $(\vec{u} \times \vec{v}) \cdot \vec{u} = 0$ {Orthogonality Properties}

   b. $(\vec{u} \times \vec{v}) \cdot \vec{v} = 0$ 
    
5. $\vec{u} \times \vec{0} = \vec{0}$
    
6. $\vec{0} \times \vec{v} = \vec{0}$
    
7. $\vec{u} \cdot (\vec{v} \times \vec{w}) = (\vec{u} \times \vec{v}) \cdot \vec{w}$ {Triple Scalar Product}


#### Perkalian silangnya (cross product) dari 2 vektor adalah :

$$\mathbf{u} \cdot \mathbf{v} = \mathbf{v} \cdot \mathbf{u}$$

#### TUGAS

##### Diketahui vektor $\vec{u} = 1, 1, 1$ dan $\vec{v} = 2, 1, 1$

##### 1. Mencari $\vec{u} \times \vec{v}$

$$\mathbf{u} = \begin{bmatrix} 1 \\ 1 \\ 1 \end{bmatrix} dan \quad \mathbf{v} = \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix}$$

$$\vec{u} \times \vec{v} = \begin{bmatrix}
u_2 v_3 - u_3 v_2 \\
-(u_1 v_3 - u_3 v_1) \\
u_1 v_2 - u_2 v_1
\end{bmatrix}$$

$$\vec{u} \times \vec{v} = \begin{bmatrix}
1 \cdot 1 - 1 \cdot 1 \\
-(1 \cdot 1 - 1 \cdot 2) \\
1 \cdot 1 - 1 \cdot 2
\end{bmatrix} = \begin{bmatrix} 1 \\ 1 \\ -1 \end{bmatrix}$$

##### 2. Mencari $\vec{v} \times \vec{u}$

$$\vec{v} \times \vec{u} = det \begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
v_1 & v_2 & v_3 \\
u_1 & u_2 & u_3 \\ \end{vmatrix}$$


$$\vec{v} \times \vec{u} = \begin{vmatrix}
v_2 & v_3 \\
u_2 & u_3 \end{vmatrix} 
\vec{i} - \begin{vmatrix}
v_1 & v_3 \\
u_1 & u_3 \end{vmatrix} 
\vec{j} + \begin{vmatrix}
v_1 & v_2 \\
u_1 & u_2 \end{vmatrix} \vec{k}$$

$$= (v_2 u_3 - v_3 u_2)\vec{i} - (v_1 u_3 - v_3 u_1)\vec{j} + (v_1 u_2 - v_2 u_1)\vec{k}$$

$$= \begin{bmatrix}
1 \cdot 1 - 1 \cdot 1 \\
-(2 \cdot 1 - 1 \cdot 1) \\
2 \cdot 1 - 1 \cdot 1
\end{bmatrix} = \begin{bmatrix} 0 \\ -1 \\ 1 \end{bmatrix} = - \begin{bmatrix} 0 \\ 1 \\ 1 \end{bmatrix} $$

<iframe src="https://www.geogebra.org/material/iframe/id/kmr9nwad/width/800/height/600/border/888888/rc/false/ai/true/sdz/true/smb/false/stb/false" width="800" height="600" style="border:0px;"> </iframe>

## HASIL KALI SILANG DAN SUDUT

Misalkan $\vec{u}$ dan $\vec{v}$ adalah vektor tak nol di $\mathbb{R}^3$. Maka
$\|\vec{u} \times \vec{v}\| = \|\vec{u}\| \, \|\vec{v}\| \, \sin(\theta)$
di mana $\theta$, $0 \leq \theta \leq \pi$, adalah sudut antara $\vec{u}$ dan $\vec{v}$.

panjang vektor dapat dihitung menggunakan rumus di bawah : 

$$\text{Panjang vektor }= \|\vec{u} \times \vec{v}\| = \|\vec{u}\| \, \|\vec{v}\| \, \sin(\theta) $$

#### CONTOH 

Misalkan ada 2 vaktor di bawah : 

$${u} = (1, 2, 1), \quad {v} = (0, 0, 1)$$

Maka panjang vektor dari keduanya adalah : 

$$\|\vec{u} \times \vec{v}\| = \|\vec{u}\| \, \|\vec{v}\| \, \sin(\theta) $$

$$= \sqrt{u_1^2 + u_2^2 + u_3^2} . \sqrt{v_1^2 + v_2^2 + v_3^2} . \sin(\theta) $$

$$= \sqrt{1^2 + 2^2 + 1^2} . \sqrt{0^2 + 0^2 + 1^2} . \sin(\theta) $$

$$= \sqrt{6} . \sqrt{1} . \sin(\theta)$$

$$= \sqrt{6} . \sin(\theta)$$

Untuk mencari panjang vektor $|\vec{u} \times \vec{v}|$

$$|\vec{u} \times \vec{v}| = \sqrt{2^2 + (-1^2) + 0^2}$$

$$= \sqrt{4 + (-1) + 0}$$

$$= \sqrt{5}$$

kemudian untuk mencari $\sin(\theta)$

$$\sin \theta = \frac{\sqrt{5}}{\sqrt{6 \times 6}}$$

$$= \frac{\sqrt{5}}{6}$$

$$= \frac{\sqrt{5 \times 5}}{\sqrt{6 \times 6}}$$

$$= \frac{\sqrt{30}}{6}$$

## IMPLEMENTASI LUAS JAJAR GENJANG

Secara geometri luas jajar genjang bisa di cari dengan menggunakan rumus (A = a x t) 
dimana : 
- a = panjang alas
- t = tinggi

Kalau jajar genjang itu dibentuk dari dua vektor $\vec{u}$ dan $\vec{v}$, yang ujungnya berawal dari titik yang sama, kita bisa cari luasnya pakai rumus:

$$A = |\vec{u}| \, |\vec{v}| \sin(\theta) $$

Keterangan : 

- $|\vec{u}|$ =  Panjang vektor $\vec{u}$
- $|\vec{v}|$ =  Panjang vektor $\vec{v}$
- $\theta$ = sudut di antara kedua vektor itu

$$A = \|\vec{u}\| \, \|\vec{v}\|  \sin(\theta) = \|\vec{u} \times \vec{v}\| $$

## VOLUME PARALELEPIPED

Dengan menghitung hasil kali silang $\vec{v}$ dan $\vec{w}$ , kita mendapatkan vektor yang besarnya sama dengan luas alas. Menghitung titik vektor dengan $\vec{u}$ menghitung volume paralelepiped. Oleh karena itu, **Volume paralelepiped yang di tentukan oleh vektor $\vec{u}, \vec{v}$ dan $\vec{w}$ adalah :**

$$V = |\vec{u} \cdot (\vec{w})|.$$

#### CONTOH 

**Menghitung Volume Paralelepiped**

1. Tentukan volume paralelepiped yang di tentukan oleh vektor $\vec{u} = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix} , \vec{v} = \begin{bmatrix} -1 \\ 1 \\ 0 \end{bmatrix}, \vec{w} = \begin{bmatrix} 0 \\ 1 \\ 1 \end{bmatrix}.$

Pertama, kita hitung 

$$\vec{v} \times \vec{w} = \begin{bmatrix} 1 \\ 1 \\ -1 \end{bmatrix}$$

Kemudian,

$$|\vec{u} \cdot (\vec{v} \times \vec{w})| = 
\begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \\ -1  \end{bmatrix} = 2$$

Oleh karena itu, volume paralelipiped adalah 2 satuan kubik.

2. Tentukan volume paralelepiped yang di tentukan oleh vektor $\vec{u} = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix} , \vec{v} = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}, \vec{w} = \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}.$

$$\vec{v} \times \vec{w} = \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix} \cdot \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}$$

$$= -i$$

$$= \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$$

$$= - \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$$

Menghitung Volumenya : 

$$V = |\vec{u} \cdot (\vec{v} \cdot \vec{w})|$$

$$= |( 1, 0, 0 ) \cdot ( -1, 0, 0 )|$$

$$= ( 1 \cdot -1 + 0\cdot 0 + 0 \cdot 0)$$

$$= | -1 |$$

$$= 1$$

## Soal

### 1. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u} =  \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$


Luas Jajaran Genjang

$$\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

penyelesaiannya $\vec{u}$ dan $\vec{v}$ sebagai vektor di bidang / sumbu x-y dari $\mathbb{R}^3$, dan tulis kembali sebagai : 

$$\vec{u} = \begin{bmatrix} 1 \\ 2 \\ 0 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 2 \\ 1 \\ 0 \end{bmatrix}$$

kemudian hitung hasilnya dapat di tunjukan di bawah : 

$$\vec{u} \times \vec{v} = \begin{bmatrix} 0 \\ 0 \\ -3 \end{bmatrix}$$

Ada Cara lain Untuk mengetahui Luas Jajar genjang yaitu : 

Diketahui:

$$\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

Maka luas jajaran genjang:

$$L = | u_1 v_2 - u_2 v_1 |$$

$$= | 1 \times 1 - 2 \times 2 |$$

$$= | 1 - 4 |$$

$$= | -3 |$$

$$= 3$$

<iframe src="https://www.geogebra.org/material/iframe/id/rgrwwaga/width/800/height/600/border/888888/rc/false/ai/true/sdz/true/smb/false/stb/false" width="800" height="600" style="border:0px;"> </iframe>

### 2. Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u} =  \begin{bmatrix} 2 \\ 0 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}$


Luas Jajaran Genjang

Diketahui vektor :

$$\vec{u} = \begin{bmatrix} 2 \\ 0 \end{bmatrix}, \quad \vec{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}$$

Maka luas jajaran genjang:

$$L = | u_1 v_2 - u_2 v_1 |$$

$$= | 2 \times 3 - 0 \times 0 |$$

$$= | 6 |$$

$$= 6$$

### 3. Tentukan luas segitiga dengan titik-titik sudut (0, 0, 0), (1, 3, -1), dan (2, 1, 1). 

Luas Segitiga di Ruang 3D

Diketahui 3 titik :

$$A(0,0,0), \ B(1,3,-1), \ C(2,1,1)$$

Dan Dibentuk vektor :

$$\vec{u} = (1,3,-1), \quad \vec{v} = (2,1,1)$$

Menghitung hasil perkalian silang :

$$\vec{u} \times \vec{v}
= \begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
1 & 3 & -1 \\
2 & 1 & 1
\end{vmatrix}$$

$$= (3 \times 1 - (-1 \times 1))\vec{i} - (1 \times 1 - (-1 \times 2))\vec{j} + (1 \times 1 - 3 \times 2)\vec{k}$$

$$= (4)\vec{i} - (3)\vec{j} + (-5)\vec{k}$$

$$= (4, -3, -5)$$

Lalu panjang vektor hasil cross product :

$$|\vec{u} \times \vec{v}|$$

$$= \sqrt{4^2 + (-3)^2 + (-5)^2}$$

$$= \sqrt{16 + 9 + 25}$$

$$= \sqrt{50}$$

$$= 5 \sqrt{2}$$

Luas segitiga :

$$4L = \frac{1}{2} \times |\vec{u} \times \vec{v}|$$

$$= \frac{1}{2} \times 5 \sqrt{2}$$

$$= \frac{5 \sqrt{2}}{2}$$

### 4. Tentukan luas segitiga dengan titik-titik sudut (5, 2, -1), (3, 6, 2), dan (1, 0, 4).

Luas Segitiga di Ruang 3D

Diketahui titik :

$$D(5,2,-1), \ E(3,6,2), \ F(1,0,4)$$

Kemudian Dibentuk jadi vektor : 

$$\vec{u} = E - D = (3-5, 6-2, 2-(-1)) = (-2, 4, 3)$$

$$\vec{v} = F - D = (1-5, 0-2, 4-(-1)) = (-4, -2, 5)$$

$$\vec{u} = (-2,4,3), \quad \vec{v} = (-4,-2,5)$$

Menghitung hasil perkalian silang:

$$\vec{u} \times \vec{v}
= \begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5
\end{vmatrix}$$

$$ = (4 \times 5 - 3 \times (-2))\vec{i} - (-2 \times 5 - 3 \times (-4))\vec{j} + (-2 \times -2 - 4 \times (-4))\vec{k}$$

$$= (26)\vec{i} - (2)\vec{j} + (20)\vec{k}$$

$$= (26, -2, 20)$$


Menghitung Panjang vektor hasil cross product :

$$|\vec{u} \times \vec{v}|$$

$$= \sqrt{26^2 + (-2)^2 + 20^2}$$

$$= \sqrt{676 + 4 + 400}$$

$$= \sqrt{1080}$$

$$= 6 \sqrt{30}$$

Luas segitiga :

$$L = \frac{1}{2} \times |\vec{u} \times \vec{v}|$$

$$= \frac{1}{2} \times 6 \sqrt{30}$$

$$= 3 \sqrt{30}$$
