---
title: Singular Value Decomposition

---

# SINGULAR VALUE DECOMPOSITION

## APA ITU SVD?

**Singular Value Decomposition** adalah Teknik dalam aljabar linear yang digunakan untuk memecah atau menguraikan suatu matriks menjadi tiga matriks yang lebih sederhana. SVD juga sering digunakan untuk reduksi data atau dimensionalitas. 

**Singular Value Decomposition (SVD)** adalah metode pemfaktoran matriks di aljabar linear, di mana sebuah matriks A diuraikan menjadi hasil perkalian tiga matriks : 

$U \in \mathbb{R}^{m \times m}$ adalah matriks ortogonal, berisi vektor-vektor eigen dari $AA^T$.
  
$\Sigma \in \mathbb{R}^{m \times n}$ adalah matriks diagonal, dengan elemen-elemen diagonalnya disebut sebagai $\textbf{nilai singular}.$

$V \in \mathbb{R}^{n \times n}$ adalah matriks ortogonal, berisi vektor-vektor eigen dari $A^T A$.

## KEGUNAAN SVD

1. Pengurangan Dimensi dan Kompresi Data:
SVD memungkinkan untuk mengurangi dimensi data dengan memproyeksikan data ke ruang berdimensi lebih rendah, yang mengarah pada kompresi data. 
2. Analisis Data dan Ekstraksi Fitur:
SVD dapat digunakan untuk mengekstrak fitur penting dari data, seperti komponen utama dalam analisis komponen utama (PCA).
3. Analisis Komponen Utama (PCA):
SVD adalah dasar dari Principal Component Analysis (PCA), metode analisis statistik yang digunakan untuk mengidentifikasi komponen-komponen utama dalam data yang menjelaskan sebagian besar variasi dalam data tersebut. 

## BAGAIMANA FORMULA? 

Rumus **SVD** (Singular Value Decomposition) dalam aljabar linear adalah : 

$$A = UΣV^T$$

Di mana : 
$A \Rightarrow$ adalah matriks asli yang ingin diuraikan.
$U \Rightarrow$ adalah matriks singular kiri, dengan kolom-kolomnya membentuk basis ortonormal untuk ruang kolom $A$.
$Σ \Rightarrow$ adalah matriks diagonal dengan nilai singular (akar kuadrat dari nilai eigen dari $A^T A$ atau $AA^T$) di diagonal utamanya.
$V^T \Rightarrow$ adalah Transpose dari matriks singular kanan. Matriks $V$ memiliki kolom-kolom yang membentuk basis ortonormal untuk ruang nol $A$.

## LANGKAH-LANGKAH :  

1. Menghitung matriks transpose dari matriks $(A^T)=A$

2. Menghitung matriks transpose dari matriks $A(A^T)$

3. Menghitung nilai eigenvalue dari $A(A^T)$

4. Menghitung nilai eigenvektor untuk matriks $V$

5. Mencari matriks $V$

6. Mencari nilai $\Sigma$

7. Mencari $U$

## CONTOH 1

Matriks : $$A = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}$$

#### Mencari Transpose matriks A
Transpose = baris jadi kolom : 

$$A^T = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}$$

Karena $A$ simetris, Maka $A^T = A$.

####  Menghitung matriks Transpose dari matriks $A(A^T)$ : 

$$A^T = AA = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix} \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix} = \begin{bmatrix} 10 & 6 \\ 6 & 10 \end{bmatrix}$$

#### Menghitung nilai eigenvalue dari $A(A^T)$ : 

$$\det(A^T A - \lambda I) = 0$$

$$\det \begin{bmatrix}
10 - \lambda & 6 \\
6 & 10 - \lambda
\end{bmatrix} = 0$$

$$(10 - \lambda)^2 - 36 = 0$$

$$(10 - \lambda)^2 = 36$$

$$10 - \lambda = \pm 6$$

$$\lambda = 10 \mp 6$$

$$\Rightarrow \lambda_1 = 16, \quad \lambda_2 = 4$$

#### Singular Value

$$\sigma_1 = \sqrt{16} = 4, \quad \sigma_2 = \sqrt{4} = 2$$


#### Menghitung nilai eigenvektor untuk matriks $V$ : 

##### Untuk $\lambda_1 = 16$

$$(A^T A - \lambda I) = 0$$

$$\begin{bmatrix}
10 - 16 & 6 \\
6 & 10 - 16
\end{bmatrix} = 0$$

$$\begin{bmatrix} -6 & 6 \\ 6 & -6 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}$$

$$\Rightarrow v_1 = v_2$$

dengan persamaan pertama : 

$$ -6x + 6y =  0$$

$$ 6y = 6x$$

$$y = x$$

maka : 

$$ v_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$$

kemudian dinormalisasikan : 

$$v_1 = \frac{1}{\sqrt{2}}, \quad v_2 =\frac{1}{\sqrt{2}}$$

##### Untuk $\lambda_2 = 4$

$$(A^T A - \lambda I) = 0$$

$$\begin{bmatrix}
10 - 16 & 6 \\
6 & 10 - 16
\end{bmatrix} = 0$$

$$\begin{bmatrix} 6 & 6 \\ 6 & 6 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \end{bmatrix}$$

$$\Rightarrow v_1 = - v_2 $$

dengan persamaan kedua : 

$$ 6x + 6y =  0$$

$$x = -y$$

maka : 

$$ v_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}$$

kemudian dinormalisasikan : 

$$v_1 = \frac{1}{\sqrt{2}}, \quad v_2 =-\frac{1}{\sqrt{2}}$$

#### Mencari Matriks $V$ : 

$$V = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$$

#### Mencari $U$ : 

$$u_1 = \frac{1}{\lambda_1}\times Av_1 $$

$$ = \frac{1}{16}\times \begin{bmatrix}
\frac{16}{\sqrt{2}} \\ \frac{16}{\sqrt{2}} \end{bmatrix}$$

$$ = \begin{bmatrix} \frac{1}{\sqrt{2}} \\ \frac{1}{\sqrt{2}} \end{bmatrix}$$

$$u_2 = \frac{1}{\lambda_2}\times Av_2 $$

$$ = \frac{1}{4}\times \begin{bmatrix}
\frac{4}{\sqrt{2}} \\ -\frac{4}{\sqrt{2}} \end{bmatrix}$$

$$ = \begin{bmatrix} \frac{1}{\sqrt{2}} \\ -\frac{1}{\sqrt{2}} \end{bmatrix}$$

Normalisasikan : 

$$U = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$$

kemudian cari nilai $\Sigma$

$$\Sigma =$$

$$\Sigma = \begin{bmatrix}
{\sqrt{16}} & 0 \\
0 & {\sqrt{4}}
\end{bmatrix}$$

$$\Sigma = \begin{bmatrix} 4 & 0 \\ 0 & 2 \end{bmatrix}$$

#### Hasil Akhir SVD

$$A = U \Sigma V^T$$

dengan :

$$U = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix},
\quad
\Sigma = \begin{bmatrix}
4 & 0 \\
0 & 2
\end{bmatrix},
\quad
V = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$$

### PEMBUKTIAN $A$ 

$$A = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}$$

$$ U = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$$

$$\Sigma = \begin{bmatrix}
4 & 0 \\
0 & 2
\end{bmatrix}
\quad$$

$$ V = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$$

#### Karena $V$ ortogonal

jadi : $$V^T = V$$

#### Menghitung $UΣ^T$

$$\Sigma V^T = \Sigma V = 
\begin{bmatrix}
4 & 0 \\
0 & 2 
\end{bmatrix}
\begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$$

Hasilnya :

$$= \frac{1}{\sqrt{2}}
\begin{bmatrix}
4 \cdot 1 + 0 \cdot 1 & 4 \cdot 1 + 0 \cdot (-1) \\
0 \cdot 1 + 2 \cdot 1 & 0 \cdot 1 + 2 \cdot (-1)
\end{bmatrix}
= \frac{1}{\sqrt{2}}
\begin{bmatrix}
4 & 4 \\
2 & -2
\end{bmatrix}$$

#### Menghitung $U \Sigma V^T$

$$U \Sigma V^T 
= \frac{1}{\sqrt{2}}
\begin{bmatrix}
1 & 1 \\
1 & -1
\end{bmatrix}
\frac{1}{\sqrt{2}}
\begin{bmatrix}
4 & 4 \\
2 & -2
\end{bmatrix}$$

Karena : 

$$\frac{1}{\sqrt{2}} \times \frac{1}{\sqrt{2}} = \frac{1}{2}= \frac{1}{2}
\begin{bmatrix}
1 \cdot 4 + 1 \cdot 2 & 1 \cdot 4 + 1 \cdot (-2) \\ 1 \cdot 4 + (-1) \cdot 2 & 1 \cdot 4 + (-1) \cdot (-2) \end{bmatrix}
= \frac{1}{2} \begin{bmatrix}
6 & 2 \\
2 & 6 \end{bmatrix}
=\begin{bmatrix}
3 & 1 \\
1 & 3 \end{bmatrix} = A$$

#### Kesimpulan
Terbukti bahwa hasil akhir dari rumus SVD sama dengan matriks awal.

## CONTOH 2

### Perhitungan SVD 

Matriks 3×2 :

$$A = \begin{bmatrix}
1 & 2 \\
0 & 3 \\
4 & 5 \end{bmatrix}$$

Langkah 1: Hitung $A^T A$

Karena matriks berukuran 3×2, maka $A^T A$ berukuran akan berubah jadi ukuran 2×2.

$$A^T = \begin{bmatrix}
1 & 0 & 4 \\
2 & 3 & 5
\end{bmatrix}$$

Hitung :

$$A^T A = \begin{bmatrix}
1 & 0 & 4 \\
2 & 3 & 5
\end{bmatrix}
\times
\begin{bmatrix}
1 & 2 \\
0 & 3 \\
4 & 5
\end{bmatrix}$$

kemudian Kalikan :

- untuk ( 1 , 1 ) :

$$1\times1 + 0\times0 + 4\times4 = 1 + 0 + 16 = 17$$

- untuk ( 1 , 2 ) :

$$1\times2 + 0\times3 + 4\times5 = 2 + 0 + 20 = 22$$

- untuk ( 2 , 1 ) :

$$2\times1 + 3\times0 + 5\times4 = 2 + 0 + 20 = 22$$

- untuk ( 2 , 2 ) :

$$2\times2 + 3\times3 + 5\times5 = 4 + 9 + 25 = 38$$

Jadi hasilnya :

$$A^T A = \begin{bmatrix}
17 & 22 \\
22 & 38 \end{bmatrix}$$

Langkah 2: Hitung eigenvalue dari $A^T A$

$$\left| A^T A - \lambda I \right| = 0$$

$$\begin{vmatrix}
17-\lambda & 22 \\
22 & 38-\lambda
\end{vmatrix}$$

$$= (17-\lambda)(38-\lambda) - (22)^2 = 0$$

Hitung :

$$(17-\lambda)(38-\lambda) = 646 - 55\lambda + \lambda^2 (22)^2 = 484 $$

Sehingga :

$$646 - 55\lambda + \lambda^2 - 484 = 0$$

$$\lambda^2 - 55\lambda + 162 = 0$$

Langkah 3: Cari akar-akar persamaan kuadrat

Pakai rumus kuadrat:

$$\lambda = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

Dengan :

a = 1

b = -55

c = 162


Hitung :

$$\Delta = (-55)^2 - 4 \times 1 \times 162 = 3025 - 648 = 2377$$

$$\sqrt{2377} \approx 48.76$$

Lalu :

$$\lambda_{1,2} = \frac{55 \pm 48.76}{2}$$

$$\lambda_1 = \frac{55 + 48.76}{2} = \frac{103.76}{2} \approx 51.88$$

$$\lambda_2 = \frac{55 - 48.76}{2} = \frac{6.24}{2} \approx 3.12$$

Langkah 4: Ambil singular value

$$\sigma_i = \sqrt{\lambda_i}$$

$$\sigma_1 = \sqrt{51.88} \approx 7.2$$

$$\sigma_2 = \sqrt{3.12} \approx 1.77$$

Hasil Akhir:

Singular value dari matriks $A$

$$\Sigma = \begin{bmatrix}
7.2 & 0 \\
0 & 1.77 \\
0 & 0 \end{bmatrix}$$

Kesimpulan :

Jadi SVD dari

$$A = \begin{bmatrix}
1 & 2 \\
0 & 3 \\
4 & 5
\end{bmatrix}$$

$$\sigma_1 \approx 7.2, \quad \sigma_2 \approx 1.77$$