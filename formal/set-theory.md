# Set theory
<img src="/public/img/venn.png"/>

A set is an unorder collection of elements.

# Powerset
The powerset of the set $A$ is a set containing all subsets of $A$.

## Example
If $S$ is the set ${x, y, z}$, then the subsets of $S$ are
$\{\}$ also denoted $\emptyset$, the empty set or the null set

- $\{x\}$
- $\{y\}$
- $\{z\}$
- $\{x, y\}$
- $\{x, z\}$
- $\{y, z\}$
- $\{x, y, z\}$

All the previous sets containing the set including itself.


**Definition: Cartesian product**<br>
The Cartesian product $A \times B$ of the sets $A$ and $B$ is the set
\[ \{ (a, b) : a \in A, b \in B \}. \]


In set theory, a Cartesian product is a mathematical product
that returns a set from multiple sets.

For sets $A$ and $B$, the Cartesian product $A \times B$ is the set of all ordered pairs $(a, b)$ where
a $C$ $A$ and b $C$ $B$.
Products can be specified using set-builder notation.

## Binary relation

**Definition: (Simple case)**<br>
A binary relation $R$ on $A$ is a set of ordered pairs of elements of $A$.

**Definition: (Relation. General case)**<br>
A binary relation $R$ on $A \times B$ is a set of ordered pairs of elements of $A$ and $B$

**Example:**<br>
Possible relations on the set $A = \{1, 2, 3\}$:
- $\{ (1,2), (2,3) \}$
- $\{ (1,2), (2,1) \}$
- $\{ (1,1), (2,2), (3,3) \}$ (Reflexive)
- $\{ (1,2), (2,3), (1,3) \}$ (Transitive)

**Definition: (Reflexivity)**<br>
A relation $\sim$ on $A$ is reflexive if $a\sim a$ for all $a \in A$.

**Definition: (Transitivity)**<br>
A relation $\sim$ on $A$ is transitive if $a\sim b$ and $b\sim c$ then $a\sim c$ for all $a,b,c \in A$.

**Exercise: (Number of relations)**<br>
The number of relations defined on $A \times B$ is the same as the number of
elements in the powerset $\mathcal{P}(A\times B)$. This number is
$|\mathcal{P}(A\times B)| = 2^{|A||B|}$.

**Exercise: (Number of functions)**<br>
The number of functions $f: X\to Y$ is $|Y|^{|X|}$



**Definition: (Multitransitivity)**<br>
A relation $\sim$ on $A$ is mulitrasitive if $a_1\sim a_2, a_2\sim a_3, \ldots, a_{n-1}\sim a_n$ then $a_1\sim a_n$ for all $a_1, a_2, \ldots, a_n \in A$, for any $n \in \mathbb{N}$.

**Theorem:**<br>
von Neumann was awesome

*Proof:*<br>
He could count anything but food.


**Theorem:**<br>
Transitivity implies multitransitivity.

*Proof (without induction):*<br>
Let $\sim$ be a transitive relation on $A\times B$. Assume that \[ a_1 \sim a_2
\sim a_3 \sim \ldots \sim a_{n-1} \sim a_n \], we must show that $a_1 \sim a_n$.
By transitivity we have that $a_1 \sim a_3$. Thus we now have \[ a_1 \sim a_3
\sim a_4 \sim \ldots \sim a_{n-1} \sim a_n \]. Similarly, we have $a_1 \sim a_4$
and we can repeat the process for $a_1 \sim a_5$ etc. We can repeat the process
until $a_1 \sim a_n$. Thus we are done.

*Proof (using induction):*<br>
Let $a_1\sim a_2, a_2\sim a_3$ where $a_1 = a; a_2 = b; a_3 = c$.
From the transitivity property it follows that $a_1\sim a_3$

Then, assume $a_n\sim a_{n+1}$ and $a_{n+1}\sim a_{n+2}$. Imply that $a_n\sim a_{n+2}$.



**Theorem (Relation between power sets and relations)**<br>
Every relation on $A\times B$ is an element in the powerset $\mathcal{P}(A\times
B)$, and vice versa. I.e. there is a bijection between the set of relations on
$A\times B$ and the powerset $\mathcal{P}(A\times B)$.

*Proof.*<br>

**Definition: (Function)**<br>
<img src="/public/img/function.png"/>
A relation $\sim$ on $A$ is a function

A function is a relation that associates each element
$x$ of a set $X$ the domain of the function to
a single element $y$ of another set $Y$.

**Definition: (Opposite relation)**<br>
Let $R$ be a relation on $A\times B$. The opposite relation of $R$ is the
relation $R_\text{op}$ is a relation on $B\times A$ given by $R_\text{op} =
\{(b, a) : (a, b) \in R \}$. The opposite relation is also known as converse
relation, transitive relation and inverse relation.

**Definition: (Injective relation)**<br>
A relation $\sim$ on $A\times B$ is injective if $a_1 \sim b$ and $a_2 \sim b$ then $a_1 = a_2$.

**Definition: (Surjective relation)**<br>
A relation $\sim$ on $A\times B$ is surjective if for all $b \in B$ there exists $a \in A$ such that $a \sim b$.

**Definition: (Function)**<br>
A function $f:X\to Y$ is a relation $f$ on $X\times Y$ such that for all $x \in
X$ there exists exactly one $y$ such that $(x, y) \in f$.

**Definition: (Bijective function)**<br>
A function is said to be bijective if it is injective and surjective.

## Inverse function

**Definition: (Left inverse function)**<br>
A function $f:X\to Y$ is said to have a *left inverse* function $g: Y \to X$ if
$g(f(x)) = x$ for all $x \in X$. A left inverse to $f$ is said to be a
*retraction* of $f$.

**Definition: (Right inverse function)**<br>
A function $f:X\to Y$ is said to have a *right inverse* function $g: Y \to X$ if
$f(g(y)) = y$ for all $y \in Y$. A right inverse to $f$ is said to be a
*section* of $f$.

**Definition: (Inverse function)**<br>
A function $f:X\to Y$ is said to have an inverse function $g: Y \to X$ if $g$ is
a left- and right inverse to $f$. The inverse function to $f$ is denoted $f^{-1}$.


# Functions
<img src="/public/img/function.png"/>
A function




## Range

## Codomain

## Injective
The function $f$ is injective (or one-to-one, or is an injection)
if f(a) ≠ f(b) for any two different elements $a$ and $b$ of $X$.

## Surjective
The function $f$ is surjective if the range equals
the codomain, that is, the number of elements of $x$ is equal to the number of elements of $y$

## Bijektiva
A function $f$ is bijective (or is a bijection or a one-to-one corresponance)
if it is both injective and surjective.

$f$ is bijective if, for any $y$



# Inverse functions
Code example

