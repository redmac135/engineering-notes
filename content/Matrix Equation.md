$A\in m\times n$ matrix
$\vec{x}\in n\times 1$ vector

**Matrix Equation**
$$A\vec{x}=\vec{b}\in m\times1$$
This equation represents a [[Linear Algebra#Def Linear System|linear system]] of $m$ equations and $n$ unknowns

## Existence of Solutions

The equation is consistent if and only if $\vec{b}$ is a [[Linear Combination]] of the columns of $A$ **OR** $\vec{b}\in\mathrm{span}(\set{\vec{a_1},\vec{a_2},...,\vec{a_n}})$

- [[Vector Span]]

## Theorem Augmented Matrix

$A$ consists of $n$ vectors each $\in m\times1$
$A=\begin{bmatrix}\vec{a_1} & \vec{a_2} & ... & \vec{a_n}\end{bmatrix}$

Then $A\vec{x}=\vec{b}$ is equivalent to $$\vec{a_1}x_1+\vec{a_2}x_2+...+\vec{a_n}x_n=\vec{b}$$ and to the system with [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]] $$\begin{bmatrix}\vec{a_1} & \vec{a_2} & ... & \vec{a_n} & \vec{b}\end{bmatrix}$$

## Theorem

For a matrix $A\in m\times n$ matrix, the following are equivalent:

1. For each $\vec{b}\in\mathbb{R}^m$, $A\vec{x}=\vec{b}$ has at least 1 solution
2. Each $\vec{b}\in\mathbb{R}^m$ is a [[Linear Combination]] of the columns of $A$
3. [[Vector Span]]: $\mathrm{span}(A)=\mathbb{R}^m$
4. $A$ has a [[Pivot Position]] in each row when brough to REF ([[Matrix Row Reduction]])

## Homogenous System

Is a matrix equation where $\vec{b}=\vec{0}$ the [[Zero Vector]]
$$A\vec{x}=\vec{0}$$

These always have the zero (trivial) solution (where $\vec{x}$ is a [[Zero Vector]])

If there are free variables, then there are more solutions in addition to the trivial solution. Otherwise, only the trivial solution exists.

_Note: if there is one nontrivial solution, then there must be a family of solutions (ref: [[Null Space of a Matrix]])_

## Related

- [[Cramer's Rule]]
