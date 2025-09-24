# Week 11 - Cryptography - Part 1

## Introduction 

The subject of transforming information so that it cannot be easily recovered 
without special knowledge. 

- shift chipers
- private key chipers
- cryptanalysis of shift chipers
- public key cryptography (invented in the 1970s)
- RSA cryptosystem
  - encrypt message using modular exponentiation, where the modulus is the 
    product of two large primes. It requires that someone know the modulus
    and an exponent
  - decrypt message requires someone to know how to invent the encryption function,
    which can only be done in a practical amount of time when someone knows
    these two large prime factors

- cryptography protocols: exchanges of messages carried out by two or more
  parties to achieve a specific security goal.

- homomorphic cryptosystem (it has an important role in cloud computing).  
  Data can become vulnerable if they must be decrypted for use as input
  to programs. Homomorphic encryption eliminates this vulnerability by 
  allowing programs to be run on encrypted data. The output of these
  programs is then the encryption of the desired output


## Clasisical Cryptography

- Julius Caesar. He made messages secret by shifting each letter three letters
  forward in the alphabet

- Definition of encryption.   
  A process of making a message secret.   

  $\mathbb{Z}_{26} := \{0, 1, 2, \ldots, 25\}$

  Caesar's encryption method can be represented by the function $f$
  that assigns to the nonnegative integer $p$, $p \leq 25$, the integer
  $f(p)$ in the set $\{0, 1, 2, \ldots, 25\}$ with
  $$
    f(p) = (p + 3) \mod 26
  $$


**Example 1** (a simple encryption)

- Definition of decryption    
  The process of determining the original message from the encrypted message

- Generalized Caesar chiper    
  encryption:   
  $$
    f(p) = (p + k) \mod 26
  $$
  decryption:   
  $$
    f^{-1}(p) = (p - k) \mod 26
  $$
  The integer $k$ above is called a **key**.

  More generalized Caesar chiper
  $$
    f(p) = (ap + b) \mod 26
  $$
  where $a$ and $b$ are integers. These two integer are chosen such 
  that the function $f(p)$ are bijection.
  It can be proved that the function $f(p)$ above are bijection if and only
  if $\gcd(a, 26) = 1$.

  The function above has a name of _affine transformation_, and the resulting
  chiper is called an _affine chiper_.


- Cryptanalysis or breaking codes.    
  A process of recovering plaintext from chipertext without knowledge of both 
  the encryption method and the key.

**Example 5** (a simple cryptanalysis)

- Block ciphers.    
  The above encryption methods (Caesar's encryption) are proned to 
  attacks based on the analysis of letter frequency in the chipertext.

  By considering a block of letters, we can increase the difficulty of
  cryptanalysis.  
  Instead of replacing individual characters with individual characters, 
  we replace block of letters with other block of letters. 
  The result of block replacement is called **block chipers**.

- Cryptosystems    
  A _cryptosystem_ is a five-tuple $(\mathcal{P}, \mathcal{C}, \mathcal{K}, 
  \mathcal{E}, \mathcal{D})$, where
  - $\mathcal{P}$ is the set of plaintext strings,
  - $\mathcal{C}$ is the set of chipertext strings,
  - $\mathcal{K}$ is the _keyspace_ (the set of all possible keys) ,
  - $\mathcal{E}$ is the set of encryption functions, and
  - $\mathcal{D}$ is the set of decryption functions.   

  We denote by $E_k$ the encryption function in $\mathcal{E}$  corresponding
  to the key $k$ and $D_k$ the decryption function in $\mathcal{D}$ that 
  decrypts ciphertext that was encrypted using $E_k$, that is, 
  $D_k(E_k(p)) = p$, for all plaintext strings $p$.

**Example 7** (Classify shift ciphers with the definition of the cryptosystem)

## Public Key Cryptography

- Private key cryptosystems   
  Two parties who wish to communicate in secret must share a secret key.  
  Because anyone who knows this key can both encrypt and decrypt messages, 
  two people who want to communicate securely need to securely exchange
  this key.    
  Example: shift cipher, affine cipher, and AES
- Public key cryptosystems (in 1970s).   
  Knowing how to send an encrypted message does not help decrypt messages.
  In such a system, everyone can have a publicly known encryption key.
  Onlyu the decryption keys are kept secret, and only the intended recipient
  of a message can decrypt it, because, as far as it is currently known, 
  knowledge of the encryption key does not let someone recover the plaintext
  message without an extraordinary amount of work (such as billions of
  years of computer time).    
  Example: RSA

## The RSA Cryptosystem

- RSA System (Ronald Rivest, Adi Shamir, and Leonar Adleman).   
  An encryption key $(n, e)$, where $n = pq$, the modulus is the product
  of two large parimes $p$ and $q$, say with 300 digits each,   
  and an exponent $e$ that is relatively prime to $(p-1)(q-1)$.

  The product of these primes $n = pq$, with approximately 600 digits, 
  cannot, as far as is currently known, be factored in a reasonable length 
  of time.

  With the advent of quantum computing, the new public key cryptosystem
  need to be invented.

## RSA Encryption

1. Set a particular key $(n, e)$
2. Prepare the plaintext $M$, and translate it using shift cipher 
   with two digits output. Then we concatenate these two-digit numbers
   into strings of digits.
3. We divide the string into equally sized blocks of $2N$ digit and 
   we choose $N$ such that $2N \leq n$. (We can also padd
   the string such that we have for the padded string, $2N = n$)
4. After that, we have a sequence of integers $m_1, m_2, \ldots, m_k$
   for some integers $k$, where $k$ is the number of the blocks.
   The encryption proceeds by transforming each block $m_i$
   to a ciphertext $c_i$, with the function
   $$
    c = m^e \mod n
   $$

**Example 8** (a short example of RSA encryption)

## RSA Decryption
1. Collect the information of the decryption key $d$,
   an inverse of $e$ modulo $(p-1)(q-1)$.
   


**Example 9** (a short example of RSA decryption)