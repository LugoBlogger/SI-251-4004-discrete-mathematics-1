# Assignment 04

Silahkan memilih dua problem berikut untuk diselesaikan.

## Problem 1 (40 poin)

Beberapa bilangan bulat positif lebih besar dari dua dikatakan mereka
memiliki sifat _pairwise relatively prime_ jika setiap dua pasangan 
dari kumpulan bilangan tersebut memiliki sifat _relatively prime_.

Tentukan apakah bilangan-bilangan berikut _pairwise relatively prime_
<ol type="a">
<li>

$21, 34, 55$
<li>

$14, 17, 85$
<li>

$25, 41, 49, 64$
<li>

$17, 18, 19, 23$
</ol>

## Problem 2 (50 poin)

Menggunakan _fast modular exponentiation_ algoritma yang telah diajarkan
di perkuliahan, hitunglah _modular exponentiation_ berikut

<ol type="a">
<li> 

$7^{644} \,\,\mathbf{mod}\,\, 645$
<li>

$11^{644} \,\,\mathbf{mod}\,\, 645$
<li>

$3^{2003} \,\,\mathbf{mod}\,\, 99$
<li>

$123^{1001} \,\,\mathbf{mod}\,\, 101$
</ol>

## Problem 3 (30 poin)

Gunakan algoritma Euclidean untuk mencari

<ol type="a">
<li>

$\operatorname{gcd}(12, 8)$
<li>

$\operatorname{gcd}(111, 201)$
<li>

$\operatorname{gcd}(1001, 1331)$
<li>

$\operatorname{gcd}(12345, 54321)$
<li>

$\operatorname{gcd}(1000, 5040)$
<li>

$\operatorname{gcd}(9888, 6060)$
</ol>

## Problem 4 (40 poin)

Menggunakan algoritma Euklidean ekstensi, nyatakan
$\operatorname{gcd}$ dua bilangan berikut sebagai linear kombinasi 
dua bilangan itu
<ol type="a">
<li>

$10$ dan $11$
<li>

$21$ dan $44$
<li>

$36$ dan $48$
<li>

$34$ dan $55$
<li>

$117$ dan $213$
<li>

$0$ dan $223$
<li>

$123$ dan $2347$
<li>

$3454$ dan $4666$
<li>

$9999$ dan $11111$
</ol>

## Problem 5 (50 poin)

Misalkan Arisa dan Bobi memiliki _public keys_ dan _private keys_ sebagai 
berikut:
$$
\begin{cases}
  (n_\textrm{Arisa}, e_\textrm{Arisa}) = (2867, 7), \quad
    d_\textrm{Arisa} = 1183, \\
  (n_\textrm{Bobi}, e_\textrm{Bobi}) = (3127, 21), \quad 
    d_\textrm{Bobi} = 1149
\end{cases}
$$

Arisa ingin mengirim pesan berikut ke Bobi: "BELI SEKARANG".
Bobi dapat memverifikasi pesan tersebut datang dari Arisa dan hanya Bobi
yang mampu membaca pesan tersebut. Pesan seperti apakah yang harus dikirim
ke Bobi, dengan mengasumsikan bahwa Arisa menandatangani pesannya
dan lalu mengenkripsikannya menggunakan _public key_ milik Bobi?