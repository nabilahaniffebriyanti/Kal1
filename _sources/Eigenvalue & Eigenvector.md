---
title: Eigenvalue & Eigenvector

---

# EIGENVALUE & EIGENVECTOR
## DEFINISI 
**Eigenvalue** adalah vektor yang arahnya tidak berubah (atau terbalik ) oleh transformasi linear tertentu.

**Eigenvector** adalah Vektor yang mempertahankan arahnya setelah transformasi linear, hanya berubah dengan faktor skalar.

Misalkan : 
A adalah matriks persegi $(n×n)$. Jika ada sebuah vektor tak nol v dan sebuah skalar λ sehingga:

$$Av=λv$$

maka:

- $A$ = Matriks
- $v$ = eigenvektor
- $λ$ = eigenvalue (skalar)

Artinya,tranformasi matriks terhadap vektor hanya mengubah skala vektor tersebut dikali dengan,arahnya tetap.

### Cara mencari eigenvector & eigenvelues

Misal:

Matriks $A$ berukuran $n$ x $n$

$$A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$$

#### Langkah-langkah mencari eigenvector & eigenvelues : 
1. Tentukan persamaan karateristik
rumus : 

$$|A - \lambda I| = 0$$

$I$ = matriks identitas berukuran sama dengan 

$\lambda$ = eigenvalue

2. Hitung Determinan Matriks
Untuk matriks 2x2 : 

$$\begin{vmatrix} a-\lambda & b \\ c & d-\lambda \end{vmatrix} = 0$$

Hitung determinannya :

$$(a-\lambda)(d-\lambda) - (b \times c) = 0$$

Hasilnya adalah persamaan kuadrat (kalau 2×2) atau polinomial (kalau lebih besar).

3. Cari Nilai Eigenvalue $\lambda$

Selesaikan persamaan hasil langkah 2 untuk mendapatkan nilai-nilai $\lambda$.

4. Substitusi Setiap Nilai $\lambda$ ke Matriks $(A - \lambda I)$

Untuk masing-masing $\lambda$ cari :

$$(A - \lambda I) \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$

5. Cari Hubungan Antara Variabel (x dan y)

- Ambil salah satu baris dari matriks hasil substitusi.
- Buat persamaan linear antara variabel.
- Sederhanakan, sehingga salah satu variabel bisa diekspresikan terhadap yang lain.

6.  Tulis Eigenvector-nya
- Tulis eigenvector dalam bentuk:

$$\mathbf{v} = k \begin{pmatrix} x \\ y \end{pmatrix}$$

- $k$ adalah konstanta skalar bebas (karena solusi homogen, boleh dikalikan skalar).
Biasanya diambil nilai sederhana (misal salah satu komponen = 1 atau -1).

### Contoh 

$$Matriks A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$$

- Mencari Nilai Eigen : $Av=λv$

$$A = \begin{pmatrix} 2 & 1 \\ 1 & 2 \end{pmatrix}$$

- Nilai Eigen $\lambda_1 = 3$

- Vektor Eigen $\mathbf{v_1} = \begin{pmatrix} 1 \\ 1 \end{pmatrix}$

- Nilai Eigen $\lambda_2 = 1$

- Vektor Eigen $\mathbf{v_2} = \begin{pmatrix} -1 \\ 1 \end{pmatrix}$

```
# Codenya.
import numpy as np

# Matriks A
A = np.array([[2, 1],[1, 2]])

# Hitung eigenvalue dan eigenvector
eigenvalues, eigenvectors = np.linalg.eig(A)

# Urutkan indeks berdasarkan eigenvalue dari besar ke kecil
sorted_indices = np.argsort(eigenvalues)[::-1]

# Urutkan eigenvalue dan eigenvector sesuai indeks
eigenvalues_sorted = eigenvalues[sorted_indices]
eigenvectors_sorted = eigenvectors[:, sorted_indices]

# Cetak hasil
print("Eigenvalues (terurut):")
print(eigenvalues_sorted)
print(" ")
print("Eigenvectors (mengikuti eigenvalues):")
print(eigenvectors_sorted)
```
```
Eigenvalues (terurut):
[3. 1.]
 
Eigenvectors (mengikuti eigenvalues):
[[ 0.70710678 -0.70710678]
 [ 0.70710678  0.70710678]]
```

### CONTOH PADA MATRIKS 2X2 : 

Cari eigenvalue dan eigenvector dari :

$$A = \begin{pmatrix} 4 & 2 \\ 1 & 3 \end{pmatrix}$$

Langkah-Langkah penyelesaian : 
1. Tentukan Persamaan Karakteristik

$$|A - \lambda I| = 0$$ 

$$= \begin{vmatrix} 4-\lambda & 2 \\ 1 & 3-\lambda \end{vmatrix} = 0$$

2. Hitung Determinannya
Gunakan rumus determinan:

$$(4-\lambda)(3-\lambda) - (2 \times 1) = 0$$

$$= (12 - 4\lambda - 3\lambda + \lambda^2) - 2 = 0$$

$$= \lambda^2 - 7\lambda + 10 = 0$$

3. Cari Nilai Eigenvalue

Persamaan kuadrat :

$$\lambda^2 - 7\lambda + 10 = 0$$

Faktorkan :

$$(\lambda-5)(\lambda-2) = 0$$

Jadi:

- $\lambda_1 = 5$
- $\lambda_2 = 2$

4. Subtitusi ke $(A - \lambda I) v = 0$

untuk $\lambda_1 = 5$

$$A - 5I = \begin{pmatrix} 4-5 & 2 \\ 1 & 3-5 \end{pmatrix} = \begin{pmatrix} -1 & 2 \\ 1 & -2 \end{pmatrix}$$

untuk $\lambda_2 = 2$

$$A - 2I = \begin{pmatrix} 4-2 & 2 \\ 1 & 3-2 \end{pmatrix} = \begin{pmatrix} 2 & 2 \\ 1 & 1 \end{pmatrix}$$

5. Cari Hubungan Variabel

Dari baris pertama $\lambda_1 = 5$:

$$-1 \times x + 2y = 0$$ 

$$x = 2y$$

Dari baris pertama $\lambda_2 = 2$: 

$$2x + 2y = 0$$ 

$$x = -y$$

6. Tentukan Eigenvector

untuk $\lambda_1 = 5$
Ambil nilai sederhana, misal:

- $y = 1$
- $x = 2$

jadi : 

$$\mathbf{v_1} = \begin{pmatrix} 2 \\ 1 \end{pmatrix}$$

untuk $\lambda_2 = 2$
Ambil nilai sederhana, misal: 
- $y = 1$
- $x = -1$

jadi : 

$$\mathbf{v_2} = \begin{pmatrix} -1 \\ 1 \end{pmatrix}$$

Kesimpulan : 

Eigenvalue 

$$\lambda_1 = 5$$ 

$$\lambda_2 = 2$$

Eigenvector

$$\mathbf{v_1} = \begin{pmatrix} 2 \\ 1 \end{pmatrix}$$

$$\mathbf{v_2} = \begin{pmatrix} -1 \\ 1 \end{pmatrix}$$

```
import numpy as np
a = np.array([[4,2],[1,3]])
eigenvalues,eigenvectors = np.linalg.eig(a)
print(f"eigenvalues :{eigenvalues}")
print(f"eigenvector :\n{eigenvectors}")
```
```
eigenvalues :[5. 2.]
eigenvector :
[[ 0.89442719 -0.70710678]
 [ 0.4472136   0.70710678]]
```

### CONTOH MATRIKS 3X3

Diketahui matriks

$$A = \begin{pmatrix}
5 & 1 & 1 \\
1 & 5 & 1 \\
1 & 1 & 5 \\
\end{pmatrix}$$

#### Mencari Eigenvalue

Penyelesaian :

Gunakan persamaan :

$$\det(A - \lambda I) = 0$$

a) Bentuk $A - \lambda I$

$$A - \lambda I = \begin{pmatrix}
5-\lambda & 1 & 1 \\
1 & 5-\lambda & 1 \\
1 & 1 & 5-\lambda \\
\end{pmatrix}$$

b) Hitung Determinan : 

Gunakan rumus determinan matriks 3×3:

$$\det(A-\lambda I) = (5-\lambda)\left[(5-\lambda)^2 - 1\right] - 1\left[1(5-\lambda) - 1\right] + 1\left[1 - 1(5-\lambda)\right]$$

c) Hitung minor-minor-nya : 

$$= (5-\lambda)^2 - 1$$

$$= (5-\lambda - 1)(5-\lambda + 1)$$

$$= (4-\lambda)(6-\lambda)$$

- Minor untuk elemen ( 1, 2 )


$$1(5-\lambda) - 1 $$

$$= (5-\lambda) - 1 $$

$$= (4-\lambda)$$

- Minor untuk elemen ( 1, 3 )

$$1 - 1(5-\lambda) $$

$$= (1-(5-\lambda)) $$

$$= (\lambda-4)$$

d) Masukkan ke rumus determinan :

$$= (5-\lambda)(4-\lambda)(6-\lambda) - 1(4-\lambda) + 1(\lambda-4)$$

Sederhanakan :

$$(4-\lambda) - (4-\lambda) = 0$$

Jadi determinannya :

$$\det(A-\lambda I) = (5-\lambda)(4-\lambda)(6-\lambda)$$

e) Hasil Eigenvalue :

$$\lambda = 4,\, 5,\, 6$$

#### Mencari Eigenvector

Untuk masing-masing eigenvalue :

Untuk $\lambda = 6$

$$A-6I = \begin{pmatrix}
-1 & 1 & 1 \\
1 & -1 & 1 \\
1 & 1 & -1 \\
\end{pmatrix}$$

hasil persamaannya :

$$-1x + y + z = 0$$

$$x - 1y + z = 0 $$

$$x + y - 1z = 0$$

Solusinya :

Misal $x = 1$

- Dari persamaan pertama : 

$$-1x + y + z = 0 \rightarrow y + z = 1$$

- Dari persamaan kedua : 

$$1-y + y + z = 0 \rightarrow z = y - 1$$

Substitusikan :

$$y + (y-1) = 1 \rightarrow 2y = 2 \rightarrow y=1$$

$$z = 1-1=0$$

Jadi :

$$v_1 = \begin{pmatrix} 1 \\ 1 \\ 0 \end{pmatrix}$$

Untuk $\lambda = 5$

$$A-5I = \begin{pmatrix}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{pmatrix}$$

hasil persamaannya :

$$y + z = 0 $$

$$x + z = 0 $$

$$x + y = 0$$

Solusinya :

$$y = -z, x = -z, x=-y$$

$$ x= y =z$$

Misal $x=1, y =1, z=1$

$$v_2 = \begin{pmatrix} 1 \\ 1 \\ 1 \end{pmatrix}$$

Untuk $\lambda = 4$

$$A-4I = \begin{pmatrix}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{pmatrix}$$

hasil persamaanya :

$$x + y + z = 0$$

Berarti, 2 bebas, 1 persamaan

Misal:

$$x = 1, y = -1, z=0$$

atau

$$x = 1, y = 0, z=-1$$

jadi :

$$v_3 = \begin{pmatrix} 1 \\ -1 \\ 0 \end{pmatrix}$$

Hasil Akhir :

Eigenvalue :

$$\lambda = 4,\, 5,\, 6$$

Eigenvector :

$$v_1 = \begin{pmatrix} 1 \\ 1 \\ 0 \end{pmatrix}$$

$$v_2 = \begin{pmatrix} 1 \\ 1 \\ 1 \end{pmatrix}$$

$$v_3 = \begin{pmatrix} 1 \\ -1 \\ 0 \end{pmatrix}$$