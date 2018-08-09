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

**Definition: (Left-injective)**<br>
A relation $\sim$ on $A\times B$ is left-injective if $a_1 \sim b$ and $a_2 \sim b$ then $a_1 = a_2$.

**Definition: (Right-injective)**<br>
A relation $\sim$ on $A\times B$ is right-injective if $a \sim b_1$ and $a \sim b_2$ then $b_1 = b_2$.

**Definition: (Left-surjective)**<br>
A relation $\sim$ on $A\times B$ is left-surjective if for all $b \in B$ there exists $a \in A$ such that $a \sim b$.

**Definition: (Right-surjective)**<br>
A relation $\sim$ on $A\times B$ is right-surjective if for all $a \in A$ there exists $b \in B$ such that $b \sim a$.

**Definition: (Function)**<br>
A function is a relation that is left-injective and left-surjective.


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