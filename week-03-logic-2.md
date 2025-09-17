# Week 03 - Logic - Part 2


- Predicates and quantifiers
  - Motivation       
    **Case 1**     
    Suppose that we know that      
    <div style="padding-left:20px">
    "Every computer connected to ITK's network is functioning properly"
    </div>

    No rules of propositional logic allow us to conclude the truth of 
    the statement
    <div style="padding-left:20px">
    "LABTER-01-PC-015" is functioning properly,"
    </div>    

    where LABTER-01-PC-015 is one of the computer connected to the ITK's 
    network.


    **Case 2**    
    We also have the same situation like the following. Suppose we know
    that 
    <div style="padding-left:20px">
    "LABTER-02-PC-099" is under attack by an intruder,"
    </div>

    where LABTER-02-PC-099 is a computer on the ITK's network. We cannot 
    use the rules of propositional logic to conclude the statement
    <div style="padding-left:20px">
    "There is a computer on ITK's network that is under attack by an intruder."
    </div>
    
  - predicate is a property that the subject of the statement can have.   
    Example:    
    "$x$ is greater than 3"
  - propositional function $P$ at $x$.     
    Example:    
    "$x$ is greater than 3", can be represented by $P(x)$
    where $P$ denotes the predicate "is greater than 3".
  - quantification is a process to create a proposition from a propositional
    function.

  - Universal quantification of $P(x)$     
    **Definition 1**     
    The _universal quantification_ of $P(x)$ is the statement     
    "$P(x)$ for all values of $x$ in the domain."     
    The notation $\forall x P(x)$ denotes the universal quantification of 
    $P(x)$. 
    Here $\forall$ is called the **universal quantifier**. We read 
    $\forall x P(x)$ as "for all $x P(x)$" or "for every $x P(x)$." 
    An element for which $P(x)$ is false is called a **counterexample** 
    to $\forall x P(x)$

  - Existensial quanfication of $P(x)$      
    **Definition 2**     
    The _existensial quantification_ of $P(x)$ is the proposition    
    "There exists an element $x$ in the domain such that $P(x)$."     
    We use the notation $\exist x P(x)$ for the existensial quantification
    of $P(x)$. Here $\exist$ is called the _existensial quantifier_.

  - Connection between quantification and looping.     
    Suppose that there are $n$ objects in the domain for the variable $x$. 
    To determine whether $\forall x P(x)$ is true, we can loop through all
    $n$ values of $x$ to see whether $P(x)$ is always true. If we encounter
    a value $x$ for which $P(x)$ is false, then we have shown that 
    $\forall x P(x)$ if false. Otherwise, $\forall x P(x)$ is true. 
    To see whether $\exist x P(x)$ is true, we loop through the $n$ values
    of $x$ searching for a value for which $P(x)$ is true. If we find one, 
    then $\exist x P(x)$ is true. If we never find such an $x$, then
    we have determined that $\exist x P(x)$ is false. (Note that this
    searching procedure does not apply if there are infinitely many values in
    the domain. However, it is still a useful way of thinking about the
    true values of quantifiations.)

  - Logical equivalence involving quantifiers    
    **Definition 3**    
    Statements involving predicates and quantifiers are _logically equivalent_ 
    if and only if they have the same truth value no matter which predicates
    are substituted into these statements and which domain of discourse
    is used for the variables in these propositional functions.   
    We use the notation $S \equiv T$ to indicate that two statements
    $S$ and $T$ involving predicates and quantifiers are logically equivalent.

  - Negating quantified expressions    
    **De Morgan's Laws for Quantifiers**    
    <table>
    <thead>
    <tr>
    <td>Negation</td>
    <td>Equivalent statement</td>
    <td>When is negation true?</td>
    <td>When false?</td>
    </tr>

    <tr>
    <td>
    
    $\neg \exist x P(x)$</td>
    <td>

    $\forall x \neg P(x)$</td>
    <td>

    For every $x$, $P(x)$ is false.</td>
    <td>

    There is an $x$ for which $P(x)$ is true.</td>
    </tr>

    <tr>
    <td>

    $\neg \forall x P(x)$
    </td>
    <td>

    $\exist x \neg P(x)$
    </td>
    <td>

    There is an $x$ for which $P(x)$ is false.
    </td>
    <td>

    $P(x)$ is true for every $x$.
    </td>
    </tr>
    </thead>
    </table>

  - (optional) Translating from English into logical expression
  - (optional) Using quantifiers in system specifications
  - (optional) examples from Lewis Carroll
  - (optional) logic programming

<ul>
 <li> Rules of Inference </li>   
 <ul>
  <li> An <i>argument</i> in propositional logic is a sequence of propositions. 
    </li>
  <li> 
  
  All but the final proposition in the argument are called _premises_ and 
    the final proposition is called the _conclusion_. </li>
  <li> 
  
  An argument is _valid_ whener all its premises are true, the
  conclusion must also be true. </li>

  <li> 
  
  modus ponens (mode that affirms) / law of detachment:   
    It allows us to **detach** the consequent $q$ from the conditional 
    $p \rightarrow q$, once we know $p$ is true, thereby assertin $q$
    as independently true.   
    $(p \wedge (p \rightarrow q)) \rightarrow q$

  </li>
  <li>
  
  modus tollens (mode that denies) / law of denying the consequent:    
    $(\neg q \wedge (p \rightarrow q)) \rightarrow \neg p$

  </li>
  <li> Example 6 of Section 1.6 </li>

  <li>Resolution is a rule of inference for an automatic reasoning task. </li>

  <li> Fallacy is a form of incorrect reasoning that lead to invalid arguments.   
    <ul>
      <li> fallacy of affirming the conclusion </li>
      <li> fallacy of denying the hypothesis </li>
    </ul>
  </li>

  <li> Rules of inferences for quantified statements 

  <table>
  <thead>
    <tr> <td>Rule of Inference</td> <td>Name</td> </tr>
  </thead>
  <tbody>
  <tr> 
  <td>

  $\displaystyle \begin{array}{c} \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle \begin{array}{l} \forall x P(x) \\ \hline P(c) \end{array}$ 
  </td>
  <td>Universal instantiation
  </tr>

  <tr>
  <td>

  $\displaystyle \begin{array}{c} \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle \begin{array}{l} P(c) \text{ for an arbitrary } c \\ \hline \forall x P(x) \end{array}$ 
  </td>
  <td>Universal generalization</td>
  </tr>

  <tr>
  <td>

  $\displaystyle \begin{array}{c} \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle \begin{array}{l} \exist x P(x) \\ \hline P(c) \text{ for some element } c\end{array}$ 
  </td>
  <td>Existensial instantiation</td>
  </tr>
  <tr>
  <td>

  $\displaystyle \begin{array}{c} \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle \begin{array}{l} P(c) \text{ for some element } c\\ \hline \exist x P(x) \end{array}$ 
  </td>
  <td>Existensial generalization</td>
  </tr>
  </tbody>
  </table>

  </li>

  <li> Combining rules of inference for porpositions and quantified statements </li>
  <ul>
  <li> Universal modus ponens 
  
  $\displaystyle \begin{array}{c} \\ \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle 
  \begin{array}{l} \forall x (P(x) \rightarrow Q(x)) \\ 
    P(a), \text{ where } a \text{ is a particular element in the domain} \\ \hline
    Q(a)
  \end{array}$ 
  </li>

  <li> Universal modus tollens

  $\displaystyle \begin{array}{c} \\ \\ \therefore \end{array} \mkern-4mu$
  $\displaystyle 
  \begin{array}{l} \forall x (P(x) \rightarrow Q(x)) \\ 
    \neg Q(a), \text{ where } a \text{ is a particular element in the domain} \\ \hline
    \neg P(a)
  \end{array}$ 
  </li>
  </ul>
  </ul>
</ul>

- Assignment submission: using A4 paper. You can write both sides.  
- Put your name and student ID in every sheet. Draw a box of 1cm of margin on it. 
- No need to write the questions.     
- Announcement of the first assignment.






