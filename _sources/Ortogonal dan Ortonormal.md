---
title: Ortogonal dan Ortonormal

---

# ORTOGONAL & ORTONORMAL
## DEFINISI
**Ortogonal** Adalah Dua vektor dikatakan ortogonal jika hasil dot product (perkalian titik) antara keduanya adalah nol.
Secara matematis, jika ada dua vektor $u$ dan $v$ maka:
$u$ . $v$ $= 0$

Artinya:

- Vektor $u$ & $v$ saling tegak lurus (membentuk sudut 90°).
- Tidak harus memiliki panjang (norma) tertentu.


**Ortonormal** Adalah Sekumpulan vektor dikatakan ortonormal jika mereka ortogonal satu sama lain dan masing-masing memiliki panjang (norma) 1.

Syarat Ortonormal :

Misal : 

$\vec{u}, \vec{v} \in \mathbb{R}^n$

1. Ortogonal antar vektor

$\mathbf{u} \cdot \mathbf{v} = 0 \ \text{jika} \ \mathbf{u} \neq \mathbf{v}$

Jika vektor berbeda, hasil dot product-nya harus nol (tegak lurus).

2. Norma 1 untuk setiap vektor

$||\mathbf{u}|| = 1 \ \text{dan} \ ||\mathbf{v}|| = 1$

Setiap vektor harus memiliki panjang (norma) = 1

---
### Contoh 

Misalkan kita punya matriks:

$A = \begin{pmatrix} 5 & 2 \\ 2 & 1 \end{pmatrix}$

Langkah 1: Cari Determinan $(A - \lambda I)$

$$\text{det}(A - \lambda I) = \begin{vmatrix} 5 - \lambda & 2 \\ 2 & 1 - \lambda \end{vmatrix}$$

Hitung determinannya:

$$= (5-\lambda)(1-\lambda) - (2 \times 2)$$

$$= (5-\lambda)(1-\lambda) - 4 $$

$$= (5-\lambda)(1-\lambda) - 4$$

$$= (5 \times 1) - 5\lambda - \lambda + \lambda^2 - 4 $$

$$= 5 - 5\lambda - \lambda + \lambda^2 - 4$$

$$= \lambda^2 - 6\lambda + 1 $$

Langkah 2: Gunakan Rumus Kuadrat

Pakai rumus:

$$\lambda = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

Dengan :
- $a = 1$
- $b = -6$
- $c = 1$

Maka:

$$\lambda = \frac{-(-6) \pm \sqrt{(-6)^2 - 4(1)(1)}}{2(1)}$$

$$= \frac{6 \pm \sqrt{36 - 4}}{2} $$

$$= \frac{6 \pm \sqrt{32}}{2}$$

$$= \frac{6 \pm 4\sqrt{2}}{2} $$

$$= 3 \pm 2\sqrt{2}$$

Hasil Akhir:

Jadi eigenvalue-nya:

$$\lambda_1 = 3 + 2\sqrt{2}, \ \lambda_2 = 3 - 2\sqrt{2}$$

#### Cari Eigenvector Untuk : $\lambda_1 = 3 + 2\sqrt{2}$

Hitung : 

$$A - \lambda_1 I = \begin{pmatrix} 5 - \lambda_1 & 2 \\ 2 & 1 - \lambda_1 \end{pmatrix}$$

Nilainya :

$$= \begin{pmatrix} 5 - (3 + 2\sqrt{2}) & 2 \\ 2 & 1 - (3 + 2\sqrt{2}) \end{pmatrix}$$

$$= \begin{pmatrix} 2 - 2\sqrt{2} & 2 \ 2 & -2 - 2\sqrt{2} \end{pmatrix} $$

Ambil salah satu persamaan (misal baris pertama):

$$(2 - 2\sqrt{2}) x + 2y = 0$$

$$\Rightarrow y = (\sqrt{2} - 1) x$$

Maka eigenvector-nya (belum dinormalisasi):

$$\vec{v_1} = \begin{pmatrix} 1 \\ \sqrt{2} - 1 \end{pmatrix}$$

Hitung Normanya :

$$\|\vec{v_1}\| = \sqrt{1^2 + (\sqrt{2} - 1)^2}$$

$$= \sqrt{1 + (3 - 2\sqrt{2})}$$

$$= \sqrt{4 - 2\sqrt{2}}$$

Nilainya kira-kira :

$$\approx 1.111$$

Normalisasi :

$$\vec{u_1} = \frac{1}{1.111} \begin{pmatrix} 1 \\ \sqrt{2} - 1 \end{pmatrix}$$

Hasil kira-kira :

$$\vec{u_1} \approx \begin{pmatrix} 0.900 \\ 0.434 \end{pmatrix}$$

Hasil Akhir :

Jadi, eigenvector untuk $\lambda_1 = 3 + 2 \sqrt2$  adalah:

$$\vec{u_1} \approx \begin{pmatrix} 0.900 \\ 0.434 \end{pmatrix}$$

#### Cari Eigenvector untuk $\lambda_2 = 3 - 2 \sqrt2$

Hitung :

$$A - \lambda_2 I = \begin{pmatrix} 5 - \lambda_2 & 2 \\ 2 & 1 - \lambda_2 \end{pmatrix}$$

Nilainya :

$$= \begin{pmatrix} 5 - (3 - 2\sqrt{2}) & 2 \\ 2 & 1 - (3 - 2\sqrt{2}) \end{pmatrix}$$

$$= \begin{pmatrix} 2 + 2\sqrt{2} & 2 \ 2 & -2 + 2\sqrt{2} \end{pmatrix}$$

Ambil salah satu persamaan (misal baris pertama):

$$(2 + 2\sqrt{2})x + 2y = 0$$

$$\Rightarrow y = -(1 + \sqrt{2}) x$$

Maka eigenvector-nya (belum dinormalisasi) :

$$\vec{v_2} = \begin{pmatrix} 1 \\ -(1+\sqrt{2}) \end{pmatrix}$$

Hitung Normanya :

$$\|\vec{v_2}\| = \sqrt{1^2 + (-(1+\sqrt{2}))^2}$$

$$= \sqrt{1 + (1+2+2\sqrt{2})}$$

$$= \sqrt{4 + 2\sqrt{2}}$$

Nilainya kira-kira :

$$\approx 2.613$$

Normalisasi :

$$\vec{u_2} = \frac{1}{2.613} \begin{pmatrix} 1 \\ -(1+\sqrt{2}) \end{pmatrix}$$

Hasil kira-kira :

$$\vec{u_2} \approx \begin{pmatrix} 0.383 \\ -0.924 \end{pmatrix}$$

Hasil Akhir :

Jadi, eigenvector untuk $\lambda_2 = 3 - 2 \sqrt2$  adalah :

$$\vec{u_2} \approx \begin{pmatrix} 0.383 \\ -0.924 \end{pmatrix}$$

#### Hasil Akhir Ortonormal dari Eigenvektor

Dua vektor ortonormal hasil normalisasi eigenvektor:

$$\vec{u}_1 = \begin{pmatrix} 0.900 \\ 0.434 \end{pmatrix}, \ 
\vec{u}_2 = \begin{pmatrix} 0.383 \\ -0.924 \end{pmatrix}$$

Verifikasi :

1. $\vec{u}_1 ,\vec{u}_2 =0$ (ortogonal)


2. $\|\vec{u_1}\| = 1$ $\|\vec{u_2}\| = 1$ (norma 1)


3. Jadi keduanya adalah ortonormal


4. Dan merupakan eigenvektor dari matriks A

```
import numpy as np

# Matriks simetris baru
B = np.array([[5, 2],
              [2, 1]])

# Cari eigenvalue dan eigenvektor
eigenvalues, eigenvectors = np.linalg.eig(B)

# Tampilkan hasil
print("Eigenvalue:")
print(eigenvalues)

print("\nEigenvektor (sebelum dinormalisasi):")
print(eigenvectors)

# Normalisasi eigenvektor untuk jadi ortonormal
normalized_vectors = []
for v in eigenvectors.T:  # per kolom
    norm = np.linalg.norm(v)
    normalized_vectors.append(v / norm)

# Konversi ke array NumPy
normalized_vectors = np.array(normalized_vectors)

print("\nEigenvektor yang sudah dinormalisasi (ortonormal):")
print(normalized_vectors)
```

```
Eigenvalue:
[5.82842712 0.17157288]

Eigenvektor (sebelum dinormalisasi):
[[ 0.92387953 -0.38268343]
 [ 0.38268343  0.92387953]]

Eigenvektor yang sudah dinormalisasi (ortonormal):
[[ 0.92387953  0.38268343]
 [-0.38268343  0.92387953]]
```