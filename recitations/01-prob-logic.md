# Recitations - Logic

Make sure you rewrite and understand the following problems and
their solutions during recitations!

## Problem 01

Which of these sentences are propositions? What are the truth values of those
that are propositions?

<ol type="a">

<li> Balikpapan is the capital of East Kalimantan.
<li> Samarinda is the capital of South Kalimantan.
<li>

$100 + 3 =103$

<li>

$2 + 5 = 100$

<li>

$y + 4 = -6$

<li>

Please remember the formula.

</ol>

### Solution

<ol>
<li> Proposition sentences, False
<li> Proposition sentences, False
<li> Proposition sentences, True 
<li> Proposition sentences, False
<li> Not proposition sentences, answer is neither true nor false
<li> Not proposition sentences, not a declarative sentence
</ol>

## Problem 02

Let $p$, $q$, and $r$ be the propositions

<div style="margin-left:30px">

$p$: You have the flu.  
$q$: You miss the final examination.  
$r$: You pass the course.

</div>

Express each of these propositions as an English sentence

<ol>
  <li>

$p \rightarrow q$

  <li>

$\neg q \leftrightarrow r$

  <li>

$q \rightarrow \neg r$

  <li>

$p \vee q \vee r$

  <li>

$(p \rightarrow \neg r) \vee (q \rightarrow \neg r)$

  <li>

$(p \wedge q) \vee (\neg q \wedge r)$

</ol>

**Solution**:

<ol>
<li>

$p \rightarrow q$ ( Implication; If p then q )
"If you have the flu, then you'll miss the final exam"

  <li>

$\neg q \leftrightarrow r$ ( Biconditional; p if and only if q )
"You will not miss the final exam if and only if you pass the course"

 <li>

$q \rightarrow \neg r$ ( Implication; If p then q )
"If you miss the final exam, then you will not pass the course"

  <li>

$p \vee q \vee r$ ( Disjunction; False when both are false )
"You have the flu or you miss the final exam or you pass the course"

 <li>

$(p \rightarrow \neg r) \vee (q \rightarrow \neg r)$
"If you have the flu then you do not pass the course or if you miss the final exam then you do not pass the course"

  <li>

$(p \wedge q) \vee (\neg q \wedge r)$ ( Conjunction $\wedge$; True when both are true )
"You have the flu and you miss the final exam or you don't miss the final exam and you pass the course"

</ol>

## Problem 03

Let $p$ be the proposition "I will do every exercise in this book"
and $q$ be the proposition "I will get an A in this course." Express each of
thse as a combination of $p$ and $q$.

<ol>
  <li> I will get an A in this course only if I do every exercise in this book.
  <li> I will get an A in this course and I will do very exercise in this book.
  <li> Either I will not get an A in this course or I will not do every exercise 
       in this book.
  <li> For me to get an A in this course it is necessary and sufficient that 
       I do every exercise in this book.
</ol>

**Solution**:

<ol>
  <li>

$q \rightarrow p$

  <li>

$q \wedge p$

  <li>

$q \vee p$

  <li>
  
$q \rightarrow p$

</ol>

## Problem 04

Determine whether each of these conditional statements is true or false.

<ol>
  <li> 
  
  If $1 + 1 = 3$, then unicorns exist.
  <li>

If $1 + 1 = 3$, then dogs can fly.

  <li>

If $1 + 1 = 2$, then dogs can fly.

  <li>

If $2 + 2 = 4$, then $1 + 2 = 3$.

</ol>

**Solution**:

<ol>
<li> True
<li> True
<li> False
<li> True
</ol>

## Problem 05

**Solution**:

For each of these sentences, determine whether an inclusive or, or an inclusive
or, is intended. Explain your answer.

<ol>
  <li> Coffee or tea comes with dinner.
  <li> A password must have at least three digits or be at least eight character
       long.
  <li> The prerequisite for the course is a course in number theory or a course
       in cryptography.
  <li> You can pay using Indonesian rupiahs or e-wallet.
</ol>

**Solution**:

<ol>
<li> Inclusive or, because dinner can come with either coffee, tea, or both 
<li> Inclusive or, because the password needs to meet one or both requirement for it to be valid
<li>  Inclusive or, because one could finish a course in both or just one of the course in number theory and cryptography as prequisite. 
<li> Exclusive or is intended because one can only choose a payment method for the transaction and not both.
</ol>

## Problem 06

Write each of these statements in the form "if $p$, then $q$" in English.

<ol>
  <li> I will remember to send you the address only if you send me an e-mail
       message.
  <li> To be a citizen of this country, it is sufficient that you were 
       born in Indonesia.
  <li> If you keep your textbook, it will be a useful reference in your future
       course
  <li> You will get a free ice cream cone, provided that you are among the 
       first 100 customers tomorrow.
</ol>

**Solution**:

<ol>
<li> If I remember to send you the address, then you will send me an e-mail message.
<li> If you become a citizen of this country, then you were born in Indonesia
<li> If you keep your textbook, then it will be a useful reference in your future course
<li> If you are among the first 100 costumers tomorrow, then you will get a free ice cream cone.
</ol>

## Problem 07

Write each of these propositions in the form "$p$ if and only if $q$" in English.

<ol>
  <li> For you to get an A in this course, it is necessary and sufficient that 
       you learn how to solve discrete mathematics problems.
  <li> If you read the newspaper every day, you will be informed, and conversely.
  <li> It rains if it is weekend day, and it is a weekend day if it rains.
  <li> My airplane flight is late exactly when I have to catch a connecting flight.
</ol>

**Solution**:

<ol>
<li> You can get an A in this course if and only if you learn how to solve discrete mathematics problems.
<li> You read the newspaper everyday if and only if you are informed, and conversely
<li> It rains if and only if it's a weekend day.
<li> My airplane flight will be late if and only if I have to catch a connecting flight 
</ol>

## Problem 08

State the converse, contrapositive, and inverse of each of these conditional
statements

<ol>
  <li> If it snows tonight, then I will stay at home.
  <li> I go to the beach whenever it is a sunny summer day.
  <li> When I stay up late, it is necessary that I sleep until noon.
</ol>

**Solution**:

<ol>

Converse : q $\rightarrow$ p
Contrapositive : $\neg$q $\rightarrow$ $\neg$p
Inverse : $\neg$p $\rightarrow$ $\neg$q

<li>
 p : It snows tonight

q: I stay home
Converse : If I stay home then it will snow tonight

Contrapositive : I will not stay home if It doesn't snow tonight

Inverse : If it does not snow tonight then I will not stay home

<li> 
p : I go to the beach

q : It is a sunny day

Converse : If its a sunny day, then I will go to the beach
Contrapositive : If I do not go to the beach, then it is not a sunny day
Inverse : If it is not a sunny day, then I will not go to the beach

<li> 
p : I stay up late 
q : I sleep until noon

Converse : If I sleep until noon, then I stayed up late
Contrapositive : If I do not sleep until noon, then I did not stayed up late
Inverse : If I did not stayed up late, then I did not sleep until noon

</ol>

## Problem 09

How many rows appear in a truth table for each of these compound propositions?

<ol>
  <li>

$(q \rightarrow \neg p) \vee (\neg p \rightarrow \neg q)$

  <li>

$(p \vee \neg t) \wedge (p \vee \neg s)$

  <li>

$(p \rightarrow r) \vee (\neg s \rightarrow \neg t) \vee (\neg u \rightarrow v)$

  <li>

$(p \wedge r \wedge s) \vee (q \wedge t) \vee (r \wedge \neg t)$

</ol>

**Solution**:
2 <sup>n</sup>

<ol> 
<li>2<sup>2</sup> = 4 Rows.
<li> 2<sup>5</sup> = 32 Rows.
<li> 2<sup>7</sup> = 128 Rows.
<li> 2<sup>5</sup> = 32 Rows.
</ol>

## Problem 10

Construct a truth table for

<ol type="a">
  <li>

$((p \rightarrow q) \rightarrow r) \rightarrow s$.

  <li>

$(p \leftrightarrow q) \leftrightarrow (r \leftrightarrow s)$.

</ol>

**Solution**:

<ol type="a">
  <li>

$((p \rightarrow q) \rightarrow r) \rightarrow s$.
| ( ( p | $$\rightarrow$$ |q )| $$\rightarrow$$ | r)| $$\rightarrow$$ | s |
| --- | --- | ---| --- | --- | --- |---|
| T |T|T| T|T| T|T|
| T |T|T| T|T| F|F|
| T |T|T| F|F| T|T|
| T |T|T| F|F| T|F|
| T |F|F| T|T| T|T|
| T |F|F| T|T| F|F|
| T |F|F| T|F| T|T|
| T |F|F| T|F| F|F|
| F |T|T| T|T| T|T|
| F |T|T| T|T| F|F|
| F |T|T| F|F| T|T|
| F |T|T| F|F| T|F|
| F |T|F| T|T| T|T|
| F |T|F| T|T| F|F|
| F |T|F| F|F| T|T|
| F |T|F| F|F| T|F|

<li>

$(p \leftrightarrow q) \leftrightarrow (r \leftrightarrow s)$.
| ( p | $\leftrightarrow$ |q )| $\leftrightarrow$ | (r| $\leftrightarrow$ | s) |
| --- | --- | ---| --- | --- | --- |---|
| T |T|T| T|T| T|T|
| T |T|T| F|T| F|F|
| T |T|T| F|F| F|T|
| T |T|T| T|F| T|F|
| T |F|F| F|T| T|T|
| T |F|F| T|T| F|F|
| T |F|F| T|F| F|T|
| T |F|F| F|F| T|F|
| F |F|T| F|T| T|T|
| F |F|T| T|T| F|F|
| F |F|T| T|F| F|T|
| F |F|T| F|F| T|F|
| F |T|F| T|T| T|T|
| F |T|F| F|T| F|F|
| F |T|F| F|F| F|T|
| F |T|F| T|F| T|F|

</ol>

## Problem 11

An ancient Sicilian legend says that the barber in a remote town who can be
reached only by traveling a dangerous mountain road shaves those people,
and only those people, who do not shave themselves. Can there be such a barber?

**Solution**:

If there is a barber who shave himself, then the barber would not fulfill the rules of only shaving those who does not shave themselves. But if the barber does not shave himself, then the barber would need to shave himself to fulfil the rules of shaving people who does not shave themselves. No such barber exists.

## Problem 12

Translate the given statement into propositional logic using the propositions
provided

<ol type="a">

<li>

You cannot edit a protected Wikipedia entry unless you are an administrator.
Express your answer in terms of $e$: "You can edit a protected Wikipedia entry",
and $a$: "You are an administrator."

<li>

You are eligibile to be President of the Republic of Indonesia only if you
are at least 40 years old, were born in Indonesia, and be registered
as a tax payer and have paid taxes for at least the last five years. Express
your answer in terms of $e$: "You are at least 40 years old,"
$b$: "You were born in Indonesia," $p$: "You are a tax payer," and
$r$: "You have paid taxes for at least five years.".

</ol>

**Solution**:

<ol> 
<li>

$\neg$a $\rightarrow$ e
e $\rightarrow$ a

<li>

x $\rightarrow$ ( e $\wedge$ b $\wedge$ p $\wedge$ r )

</ol>

## Problem 13

When three professors are seated in a restaurant, the hostess asks them:
"Does everyone want coffee?" The first professor says "I do not know."
The second professor then says "I do not know." Finally, the third professor
says "No, not everyone wants coffee." The hostess comes back and gives
coffee to the professors who want it. How did she figures out who wanted coffee?

**Solution**:

The first professor wants coffee, because if he doesn’t want coffee then saying “no” would mean that the question is False, he is operating on the assumption that yes he himself does want coffee and isn’t sure if Professor 2 and Professor 3 also want coffee, which would be the requirement for the question to be True.

Professor 2 also wants coffee and for the same reason as Professor 1, he knows now that Professor 1 wants coffee, and he himself wants coffee, but isn’t sure about Professor 3, again, all three must want coffee for the original question to be True (note the use of "everyone" in the question).

Therefore Professor 3 is the only remaining variable that can negate the question. He then does negate the question with his statement, hence Professor 3 is the only one who does not want coffee.

## Problem 14

Suppose there are signs on the doors to two rooms. The sign on the first door
reads "In this room there is a lady, and in the other one there is a tiger";
and the sign on the second door reads "In one of these rooms, there is a lady,
and in one of them there is a tiger." Suppose that you know that one of
these signs is true and the other is false. behind which door is the lady?

**Solution**:

The lady is behind the second door. If the sign on the first door is true, then the sign on the second door is also true, while we know that one of the sign is false. If the sign on the first door is false, and second door true, the lady would either be in room 2, tiger in room 1, or both the tiger and lady in the same room together.

## Problem 15

Use truth tables to verify these equivalences.

<ol type="a">
  <li>

$p \wedge \mathbf{T} \equiv p$

  <li>

$p \vee \mathbf{F} \equiv p$

  <li>

$p \wedge \mathbf{F} \equiv \mathbf{F}$

  <li>

$p \vee \mathbf{T} \equiv \mathbf{T}$

  <li>

$p \vee p \equiv p$

  <li>

$p \wedge p \equiv p$

</ol>

**Solution**:

<ol>

<li>

| p   | $\wedge$ | T   | $\equiv$ | p   |
| --- | -------- | --- | -------- | --- |
| T   | T        | T   | T        | T   |
| F   | F        | T   | T        | F   |

Equivalent.

<li>

| p   | $\vee$ | F   | $\equiv$ | p   |
| --- | ------ | --- | -------- | --- |
| T   | T      | F   | T        | T   |
| F   | F      | F   | T        | F   |

Equivalent.

<li>

| p   | $\wedge$ | F   | $\equiv$ | F   |
| --- | -------- | --- | -------- | --- |
| T   | F        | F   | T        | F   |
| F   | F        | F   | F        | F   |

Equivalent.

<li>

| p   | $\vee$ | T   | $\equiv$ | T   |
| --- | ------ | --- | -------- | --- |
| T   | T      | T   | T        | T   |
| F   | T      | T   | T        | T   |

Equivalent.

<li>

| p   | $\vee$ | p   | $\equiv$ | p   |
| --- | ------ | --- | -------- | --- |
| T   | T      | T   | T        | T   |
| F   | F      | F   | T        | F   |

Equivalent.

<li>

| p   | $\wedge$ | p   | $\equiv$ | p   |
| --- | -------- | --- | -------- | --- |
| T   | T        | T   | T        | T   |
| F   | F        | F   | T        | F   |

Equivalent.

</ol>

## Problem 16

**Solution**:

Using De Morgan's laws to find the negation of each of the following statements

<ol type="a">
  <li> Jan is rich and happy.
  <li> Carlos will bicycle or run tomorrow.
  <li> Mei walks or takes the bus to class.
  <li> Ibrahim is smart and hard working.
</ol>

**Solution**:

De'Morgan Law
$\neg$(p $\wedge$ q) $\equiv$ $\neg$p $\vee$ $\neg$q
$\neg$(p $\vee$ q) $\equiv$ $\neg$p $\wedge$ $\neg$q

<ol>
<li>p: Jan is rich, q: happy.

Jan is not rich and not happy $\equiv$ Jan is neither happy nor rich

<li>p: Carlos will bicycle tomorrow, q: Carlos will run tomorrow.

Carlos will not bicycle nor run tomorrow $\equiv$ Carlos will not bicycle and run tomorrow

<li>p: Mei walks to class, q: Mei takes the bus to class

Mei does not walk nor take the bus to class $\equiv$ Mei does not walk and take the bus to class

<li>p: Ibrahim is smart, q: Ibrahim is hardworking

Ibrahim is not smart and hardworking $\equiv$ Ibrahim is neither smart nor hardworking

</ol>

## Problem 17

Show that each of these conditional statements is a tautology by using truth
tables

<ol type="a">
  <li>

$[\neg p \wedge (p \vee q)] \rightarrow q$

  <li>

$[(p \rightarrow q) \wedge (q \rightarrow r)] \rightarrow (p \rightarrow r)$

  <li>

$[p \wedge (p \rightarrow q)] \rightarrow q$

  <li>

$[(p \vee q) \wedge (p \rightarrow r) \wedge (q \rightarrow r)] \rightarrow r$

</ol>

**Solution**:

<ol>

<li>

| [$\neg$ p   | $\vee$ | (p | $\vee$   |q)] |  $\rightarrow$ | q   |
| --- | ------ | --- | -------- | --- |---|---|
| F   | T      | T   | T        | T   | T| T|
| F   | T      | T   | T        | F   | F| F|
| T   | T      | F   | T        | T   | T| T|
| T   | T      | F   | F        | F   | F |F |



<li>

| [(p   | $\rightarrow$ | q)| $\wedge$ | (q | $\rightarrow$   | r)] |  $\rightarrow$ | (p   | $\rightarrow$ | r) |
| --- | ------ | ---|---|-- | -------- | --- |---|---|---|---|
| T   | T      | T   | T        | T   | T| T|
| T   | T      | T   | T        | F   | F| F|
| F   | T      | F   | T        | T   | T| T|
| F   | T      | F   | F        | F   | F |F |

</ol>

## Problem 18

Determine whether $(\neg q \wedge (p \rightarrow q)) \rightarrow \neg p$ is
a tautology.

**Solution**:

## Problem 19

Show that $(p \wedge q) \rightarrow r$
and $(p \rightarrow r) \wedge (q \rightarrow r)$ are not logically equivalent.

**Solution**:

## Problem 20

The **dual** of a compound proposition that contains only the logical operators
$\vee$, $\wedge$, and $\neg$, is the compound proposition obtained by replacing
each $\vee$ by $\wedge$, each $\wedge$ by $\vee$, each $\mathbf{T}$ by $\mathbf{F}$,
and each $\mathbf{F}$ by $\mathbf{T}$. The dual of a compound proposition $s$
is denoted by $s^*$.

Find the dual of each of these compound propositions.

<ol type="a">
  <li> 
  
  $p \vee \neg q$
  <li>

$(p \wedge \neg q) \vee (q \wedge \mathbf{F})$

  <li>

$p \wedge (q \vee (r \wedge \mathbf{T}))$

  <li>

$p \wedge \neg q \wedge \neg r$

  <li>

$(p \vee \mathbf{F}) \wedge (q \vee \mathbf{T})$

  <li>

$(p \wedge q \wedge r) \vee s$

</ol>

**Solution**:
