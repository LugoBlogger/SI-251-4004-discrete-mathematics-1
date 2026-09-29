# Week 10 - Number Theory - Part 2

## Primes and Greatest Common Divisors

**Definition 1**    
An integer $p$ greater than $1$ is called _prime_ if the only positive factors
of $p$ are $1$ and $p$. A positive integer that is greater than $1$ and is 
not prime is called _composite_.

**Theorem 1** The Fundamental theorem of arithmetic

**Example 2**

Trial division     
**Theorem 2**    

- **Example 3**
- **Example 4**

The Sieve of Eratosthenes.   
Make the last subtable in Table 1   
Python demo

State in the calss that there are infinitely many primes according to Theorem 3.

Discuss about Mersenne primes (its definition) and the quest for searching
the largest prime number in the world. See https://www.mersenne.org/

Discuss about Goldbach's conjecture   
- Goldbach's version    
  Every odd integer $n$, $n > 5$, is the sum of three primes.
- Euler's version    
  Every even integer $n$, $n > 2$, is the sum of two primes

- Greatest Common Divisors and Least Common Multiples

**Definition 2**     
Let $a$ and $b$ be integers, not both zero. The largest integer $d$ such
that $d \mid a$ and $d \mid b$ is called the _greatest common divisor_ of $a$
and $b$. The greatest common divisor of $a$ and $b$ is denoted by 
$\gcd(a, b)$.

**Example 10**

**Example 14**


**Definition 3**    
The integers $a$ and $b$ are _relatively prime_ if their greatest common divisor is $1$.

**Example 12**   
Show that the integers 17 and 22 are relatively prime.

**Definition 5**     
The _least common multiple_ of the positive integers $a$ and $b$ is the smallest
positive integer that is divisible by both $a$ and $b$. The least common
multiple of $a$ and $b$ is denoted by $\operatorname{lcm}(a, b)$

**Example 15**    
What is the least common multiple of $95\,256$ and $432$?

**Theorem 5**   
Let $a$ and $b$ be positive integers. Then
$$
  ab = \operatorname{gcd}(a, b) \cdot \operatorname{lcm}(a, b)
$$

- The Euclidean algorithms

  **procedure** $\gcd$($a, b$: positive integer)    
  $x := a$   
  $y := b$  
  **while** $y \neq 0$   
  $\quad r := x \bmod y$    
  $\quad x := y$    
  $\quad y := r$  
  **return** $x$ (where $\gcd(a, b)$ is $x$)


- gcds as Linear Combinations    
  - **Theorem 6** Bézout's theorem     
    If $a$ and $b$ are positive integers, then there exist integers
    $s$ and $t$ such that $\gcd(a, b) = sa + tb$
  - **Definition 6**  Bézout's identity

  - How to find Bézout's identity
    1. First method to find it using two passes of Euclidean algorithm  
       **Example 17**    
    2. Second method to find it using extended Euclidean algorithm (single pass).  
       We have to set $(s_0, t_0) = (1, 0)$ and $(s_1, t_1) = (0, 1)$
       and let
       $$
       \begin{cases}
         s_j = s_{j-2} - q_{j-1} s_{j-1}, \\
         t_j = t_{j-2} - q_{j-1} t_{j-1}
       \end{cases}
       $$
       for $j = 2, 3, \ldots, n$, where $q_j$ are the quotients
      in the divisions used when the Euclidean algorithm finds 
      $\gcd(a, b)$.   
      It can be proved with strong induction that  
      $\gcd(a, b) = s_n a + t_n b$   
      **Example 18**


## Solving Congruences

A congruence of the form
$$
  ax \equiv b \pmod{m}
$$
where $m$ is a positive integer, $a$ and $b$ are integers, and $x$ is 
a variable, called a **linear congurence**

**Theorem 1** (existence of an inverse of $a$ modulo m)    
If $a$ and $m$ are relatively prime integers and $m > 1$, then an inverse
of $a$ modulo $m$ exists.   
Furthermore, this inverse is unique modulo $m$. (That is, there is a unique 
positive integer $\overline{a}$ less than $m$ thaat is an inverse
of $a$ modulo $m$ and every other inverse of $a$ modulo $m$ is congruent
to $\overline{a}$ modulo $m$.)

**How to get an inverse of $a$ modulo $m$**   
1. First check that $a$ and $m$ are relatively prime.   
2. After that, using extended Euclidean algorithm, find
   $s$ and $t$ such that
   $$
      \gcd(a, m) = sa + tm
   $$

3. Because 
   $$
   \begin{align*}
      sa + tm &= \gcd(a, m) = 1\\
      sa + tm &\equiv 1 \pmod{m} \\
      (sa + tm) - 1 &= km, \quad k \in \mathbb{Z} \\
      sa - 1 &= (k - t) m, \quad (k - t) \in \mathbb{Z} \\
      sa &\equiv 1 \pmod{m}
   \end{align*}
   $$
   We have $s$ is the inverse of $a$ modulo $m$.

### The Chinese Remainder Theorem

**Example 4**   
In the first century, the Chinese mathematician Sun-Tsu asked:
> There are certain things whose number is unknown. When divided by 3, 
> the remainder is 2; when divided by 5, the remainder is 3; and when divided
> by 7, the remainder is 2. What will be the number of things?    

This puzzle can be translated into the following questions: What are the 
solutions of the systems of congurences
$$
   x \equiv 2 \,(\operatorname{mod} 3), \\ 
   x \equiv 3 \,(\operatorname{mod} 5), \\
   x \equiv 2 \,(\operatorname{mod} 7)?
$$

<br>

**Theorem 2** (The Chinese Remainder Theorem)     
Example 5 (solution of Example 4)    
Example 6 (using different method to solve a similar problem like in Example 4; with back substitution) 



### Primitive Roots and Discrete Logarithms

**Definition 3**   
A **primitive root** modulo a prime $p$ is an integer $r$
in $\mathbb{Z}_p$ such that every nonzero element of $\mathbb{Z}_p$ is 
a power of $r$.

**Example 12**     
Determine whether 2 and 3 are primitive roots modulo 11.   
_Solution:_ When we compute the power of 2 in $\mathbb{Z}_{11}$, we obtain
$$
\begin{array}{cc}
   2^1 = 2, & 2^6 = 9,\\
   2^2 = 4, & 2^7 = 7,\\
   2^3 = 8, & 2^8 = 3,\\
   2^4 = 5, & 2^9 = 6,\\
   2^5 = 10, & 2^{10} = 1
\end{array}
$$
Because every nonzero element of $\mathbb{Z}_{11}$ is a power of 2, 2 is a
primitive root of $11$.

When we compute the power of 3 modulo 11, we obtain
$$
\begin{array}{ccccc}
   3^1=3, & 3^2=9, & 3^3 = 5, & 3^4 = 4, & 3^5 = 1
\end{array}
$$
This pattern repeats when we compute higher power of 3. Because not all 
nonzero elements of $\mathbb{Z}_{11}$ are powers of 3, we conclude that 3 is 
not a primitive root of 11

<br>

An important fact in number theory is that there is a primitive root 
modulo $p$ for every prime $p$.
See (Rosen, 2010) - Elementary Number Theory and Its Applications, 6th Ed, 
for the proof of this fact.

<br>

Suppose that $p$ is prime and $r$ is a primitive root modulo $p$.   
If $a$ is an integer between $1$ and $1 - p$, that is, a non-zero element of
$\mathbb{Z}_p$, we know that there is an unique exponent $e$ such that
$r^e = a$ in $\mathbb{Z}_p$, that is, $r^e \operatorname{mod} p = a$.

Now we can define the discrete logarithm based on the previous fact

**Definition 4**     
Suppose that $p$ is a prime, $r$ is a primitive root modulo $p$, and $a$
is an integer between $1$ and $p - 1$ inclusive ($1 \leq a \leq 1-p$).
If $r^e \operatorname{mod} p = a$ and $0 \leq e \leq p-1$, we say that 
$e$ is the _discrete logarithm_ of $a$ modulo $p$ to the base $r$ and we write
$\log_r a = e$ (where the prime $p$ is understood)

**Example 13**    
Find the discrete logarithms of 3 and 5 modulo 11 to the base 2.

<br>

The **discrete logarithm problem** takes as input a prime $p$, a primitive root 
$r$ modulo $p$, and a positive integer $a \in \mathbb{Z}_p$; its output
is the discrete logarithm of $a$ modulo $p$ to the base $r$.

[Interesting fact]    
Unsolved problem in computer science.    
Can the discrete logarithm be computed in polynomial time on a classical computer?

Existing classical algorithms
- Baby-step giant-step
- Function field sieve
- Index calculus algorith
- Number field sieve
- Pohlig-Hellman algorithm
- Pollard's rho algorithm for logarithms
- Pollard's kangaroo algorithm (aka Pollard's lambda algorithm)

There is an efficient quantum algorithm due to Peter Shor.

## Application of Congruences

- Hashing Functions

- Pseudorandom Numbers

- Check Digits