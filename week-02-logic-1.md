# Week 02 - Logic - Part 1

## Motivation

- Suppose you and I have the same amount of money. How much I give you so that 
  you have ten dollars more than I?

- A certain convention numbered on hundred politicians. Each politician 
  was either crooked or honest. We are given the following two facts:
  1. At least one of the politicians was honest.
  2. Given any two of the politicians, at least one of the two was crooked.    

  Can it be determined from these two facts how many of the politicians were 
  honest and how many were crooked?

- A bottle of wine cost ten dollars. The wine was worth nine dollars more than 
  the bottle. How much was the bottle worth?

## Learning concepts

- What is Logic?
- Statement 
  - definition of statement: something stated: such as a) a single declaration
    or remark (synonyms of assertion) b) a report of facts or opinions.    
  - definition of state: a mode or condition of being.
- Propositions
- Propositional variables
- Compound propositions
- Logical operators
  - Negation (unitary operator)
    - truth tables
  - Conjunction (AND)  (binary operator)
  - Disjunction (OR) (binary operator)
  - [optional] Exclusive or
- Conditional statements (see 2022-09-12-logic.xopp)
  - An example that reflects truth tables of conditional
    statements (obligation)
- Some variations of conditional statements $p \rightarrow q$
  - converse $q \rightarrow p$
  - contrapositive $\neg q \rightarrow \neg p$
  - inverse  $\neg p \rightarrow \neg q$
- Truth table of conditional statements, converse, contrapositive, 
  and inverse to see logically equivalent between them.
  
- Truth table of implication and bi-implication
- Truth table of compound propositions 
- Exercises (Rosen 1.1 Propositional logic Exercises)    
  
  14. Let $p$, $q$, and $r$ be the propositions     
      $p$: You have the flu.    
      $q$: You miss the final examination   
      $r$: You pass the course of Discrete Mathematics.   
      Express each of these propositions as an English sentence
      1. $(p \rightarrow \neg r) \vee (q \rightarrow \neg r)$ 
      2. $p \vee q \vee r$
      3. $(p \wedge q) \vee (\neg q \wedge r)$

  39. Construct a truth table for each of these compound propositions.
      1. $(p \rightarrow q) \vee (\neg p \rightarrow r)$ 
      2. $(p \leftrightarrow q) \vee (\neg q \leftrightarrow r)$
      3. $(\neg p \leftrightarrow \neg q) \leftrightarrow (q \leftrightarrow r)$

- Application of Propositional Logic
  - Translating English sentences
  - ~~Boolean search~~
    - ~~Google Search (AND, OR, NOT operator)~~
  - Logic puzzle
    - Determining two inhabitants

- Propositional equivalence

  - Tautology: a compound proposition that is always true, no matter what the
    truth values of the propositional variables that occur in it

  - The compound propositions $p$ and $q$ are called _logically equivalent_ 
    if $p \leftrightarrow q$ is a tautology. The notation $p \equiv q$ denotes 
    that $p$ and $q$ are logically equivalent.
  

## References
- (Smullyan, 1983) - The Lady or the tiger? and other logical puzzles.