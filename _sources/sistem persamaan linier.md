---
title: sistem persamaan linier

---

# SISTEM PERSAMAAN LINEAR
## PENGERTIAN
Kumpulan persamaan linear yang terdiri dari beberapa variabel. Sistem persamaan linear merupakan salah satu materi dalam ilmu matematika.

Sistem persamaan linear bisa diartikan sebagai suatu persamaan aljabar. Dimana persamaan linear sendiri memiliki karakteristik pada setiap sukunya mengandung konstanta atau perkalian konstanta dengan variabel tunggal.
 
## SOLUSI SISTEM PERSAMAAN LINIER
### METODE ELIMINASI
Metode eliminasi adalah salah satu metode yang digunakan untuk menyelesaikan soal persamaan linear dua atau tiga variable. Dimana metode eliminasi secara garis besar akan menghapus atau menghilangkan satu variabel dalam persamaan tersebut.

#### ELIMINASI GAUSS
sistem persamaan linear yang di ubah menjadi bentuk matriks, matriks tersebut lalu diubah kebentuk Eselon Baris melalui Operasi Baris Elementer. Kemudian sistem diselesaikan dengan substitusi balik.

#### MEMBUAT PENJELASAN SOLUSI ATAU PENYELESAIAN PERSAMAAN 3 VARIABEL DENGAN MENGGUNAKAN ELIMINASI GAUUS SERTA MENAMPILKAN SOLUSINYA SECARA GRAFIS MENGGUNAKAN GEOGEBRA.  

Selesaikan sistem persamaan linier berikut :
 
 x+y+z= 6
2x+2y+3z= 14
3x+4y+2z= 13

Berikut adalah langkah-langkah menyelesaikan sistem persamaan linear diatas menggunakan metode eliminasi Gauss.

1. langkah pertama 

   Hasil Matriksnya : 

   1 1 1    |6
   2 2 3    |14
   3 4 2    |13

2. langkah kedua
- Jadikan elemen pivot pertama (baris 1, kolom 1) bernilai 1.
- Jika Sudah bernilai 1, jadi tidak perlu diubah.
- NOL-kan Elemen di bawah Elemen Pivot Pertama
- Pivot pertama sudah 1 di posisi (1,1). Maka Kita buat elemen di bawahnya menjadi nol:

  $𝑅_2→𝑅_2−2𝑅_1$
  
  Hasil Matriksnya : 
  1 1 1    | 6
  0 0 1    | 2
  3 4 2    | 13
  
  $𝑅_3→𝑅_3−3𝑅_1$
  
  Hasil Matriksnya : 
  1 1 1    | 6
  0 0 1    | 2
  0 1 -1   | -5
  
- Jadikan elemen pivot kedua (baris 2, kolom 2) bernilai 1:

  $𝑅_2→𝑅_2+𝑅_3$
  
  Hasil Matriksnya : 
  1 1 1    | 6
  0 1 0    | -3
  0 1 -1   | -5
  
- NOL-kan Elemen di bawah Elemen Pivot kedua
  
  $𝑅_3→𝑅_3-𝑅_2$
  
  Hasil Matriksnya : 
  1 1 1    | 6
  0 1 0    | -3
  0 0 -1   | -2
  
- Jadikan elemen pivot kedua (baris 3, kolom 3) bernilai 1:
  
  $𝑅_3→𝑅_3.(-3)$
  
  Hasil Matriksnya : 
  1 1 1    | 6
  0 1 0    | -3
  0 0 1    | 2
3. langkah ketiga
 Subtitusi Balik
 
- Dari baris terakhir
  z = 2
- Subtitusi z ke baris kedua
  y+z = -3
  y+2 = -3
  y   = -3-2
  y   = -5
- Subtitusi y dan z ke baris pertama
  x+y+z = 6
  x+(-5)+2 = 6
  x-5+2 = 6
  x-3 = 6
  x = 6+3
  x = 9
- Solusi akhir
  x = 9, y = -5, dan z = 2
 
hasil grafis dari persamaan diatas
![Screenshot 2025-03-03 172627](https://hackmd.io/_uploads/HyJzrZXo1l.png)
