# Week 09 - Number Theory - Part 1

## Motivation


## Divisibility and Modular Arithmetic

- Definition of divisibility

- Theorem 1 (some of the basic properties of divisibility of integers)
- Corollary 1

- The division algorithm (Theorem 2)

- Divisor, dividend, quotient and remainder

- Modular arithmetic
  - congruence, modulus (plural moduli)
  - Theorem 3 -> Example 5
  - Theorem 4
  - Theorem 5 -> Example 6
  - Corollary 2 -> Example 7

- Arithmetic modulo $m$

## Integer Representations and Algorithms

- Binary expansions
- Octal and hexadecimal expansions
- Base conversion

- Table 1 - Hexadecimal, octal, and binary representaiton of the integers 0 
  through 15.

- Conversion between binary, octal, and hexadecimal expansions

- Algorithms for integer operations
  - Addition algorithm
  - Multiplcation algorithm
  - Algorithm for `div` and `mod`
- Modular exponentiation -> Fast Modulear Exponentiation

## Primes and Greatest Common Divisors

- Definition of primes

- The Fundamental theorem of Arithmetic

- Trial division - Theorem 2

- Greatest Common Divisors and Least Common Multiples

**Definition 2**     
Let $a$ and $b$ be integers, not both zero. The largest integer $d$ such
that $d \mid a$ and $d | b$ is called the _greatest common divisor_ of $a$
and $b$. The greatest common divisor of $a$ and $b$ is denoted by 
$\gcd(a, b)$.


**Definition 3**    
The integers $a$ and $b$ are _relatively prime_ if their greatest common divisor is $1$.

**Definition 5**     
The _least common multiple_ of the positive integers $a$ and $b$ is the smallest
positive integer that is divisible by both $a$ and $b$. The least common
multiple of $a$ and $b$ is denoted by $\operatorname{lcm}(a, b)$


- (optional) gcds as Linear Combinations
  - Bézout's theorem
  - Bézout's identity
    1. First method to find it using two passes of Euclidean algorithm
    2. Second method to find it using extended Euclidean algorithm
