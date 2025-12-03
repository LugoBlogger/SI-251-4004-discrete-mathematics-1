# Week 10 - Number Theory - Part 2

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


## Application of Congruences