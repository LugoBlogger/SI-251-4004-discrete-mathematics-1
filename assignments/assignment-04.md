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
Di dalam kriptosistem RSA diatur cara untuk mengubah 
pesan normal (_plaintext_) ke pesan acak (_chiphertext_), disebut
_encryption_, dan juga proses sebaliknya disebut _decryption_.

_Encryption_ dalam kriptosistem RSA mengikuti tahapan berikut
1. Diberikan dua pasangan bilangan bulat positif $n$ dan $e$.
2. Pastikan bahwa kita diberikan faktor prima dari $n$ 
   sedemikian rupa sehingga $n = p q$.
3. Pastikan juga $\gcd(e, (p-1)(q-1)) = 1$
4. Ubah setiap huruf di pesan _plaintext_ ke digit desimal 
   mengikuti konversi berikut:
   ($(A, B, C, \ldots, Z) \rightarrow (00, 01, 02, \ldots, 25)$).  
   Sebagai contoh, jika kita mempunyai kata "STOP", maka akan diubah menjadi
   $18\,19\,14\,15$
5. Kelompokan digit-digit desimal yang diperoleh untuk setiap $2N$ digit, 
   dengan $2N$ merupakan bilangan bulat terbesar yang masih 
   memenuhi $2N \leq n$.   
   Sebagai contoh, hasil konversi dari kata "STOP" memiliki digit 
   $18 \, 19\,14\,15$, dan kita memiliki $n = 2537$.   
   Jika kita menggunakan $2N = 2$, maka digit terbesar yang bisa dibentuk
   adalah $25$ (angka $25$ ini berasal dari huruf terakhir $Z$ yang
   memiliki desimal $25$), tentunya $25 < n = 2537$.   
   Jika kita menggunakan $2N = 4$, maka digit terbesar yang bisa dibentuk
   adalah $2525$ (angak $2525$ ini berasal dari perulangan dua kali 
   huruf terakhir $Z$ yang memiliki desimal $25$), 
   tentunya $2525 < n = 2537$.   
   Jika kita memggunakan $2N = 6$, maka digit terbesar yang bisa dibentuk
   adalah $252525$, tentukan nilai ini jauh lebih besar dari $n = 2537$.   
   Sehingga kita memerlukan pengelompokan $2N = 4$ digit. Diperoleh
   "STOP" $= 1819\,1415$

6. Untuk setiap kelompok angka yang diperoleh dari tahap 5), lakukan perhitungan
   untuk _chipertext_, $c$ berikut
   $$
      c = m^e \bmod n
   $$
   dengan $m$ adalah setiap angka yang terbentuk dari pengelompokan 
   di tahap 5).
   Di tahap ini dapat digunakan algoritma _fast modular exponentiation_
   untuk mempercepat perhitungan.    
   Sebagai contoh, untuk setiap kelompok yang terbentuk dari "STOP" 
   menggunakan $n=2537$, kita dapatkan 
   $m_1 = 1819$ dan $m_11414$. Lalu jika $e = 13$ kita dapat 
   menghitung $c_1 = m_1^{13} \bmod 2537$ dan $c_2 = m_2^{13} \bmod 2537$



7. Satukan setiap _chipertext_ yang diperoleh dari masing-masing
   kelompok untuk mendapatkan pesan keseluruahn yang terenkripsi.   
   Sebagai contoh dari contoh di tahap 6), kita dapatkan
   $c = c_1 c_2$ (kita tinggal menggabungkan dua _chipertext_ yang
   dihasilkan).


Misalkan Arisa ingin mengirim pesan berikut ke Yasuke: "BELI SEKARANG"
dengan $n = 2357$ dan $e = 13$, seperti apakah hasil _ciphertext_ yang
harus dikirim ke Yasuke, jika $n = 2357$ dapat difaktorkan ke dalam
perkalian dua bilangan prima $p$ dan $q$ sebagai $2357 = 43 \cdot 59$?