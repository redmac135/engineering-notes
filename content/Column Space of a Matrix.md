## Definition

$A=\begin{bmatrix}\vec{a_1} & \vec{a_2} & ... & \vec{a_m}\end{bmatrix},\: \vec{a_i}\in\mathbb{R}^n$

$\mathrm{Col}(A)=\mathrm{span}\set{\vec{a_1}, \vec{a_2}, ..., \vec{a_m}}$

## Rank of a Matrix

$\mathrm{rank}(A)=\dim\mathrm{Col}(A)$
def: [[Dimension of a Subspace]]

### Rank Theorem

$$\mathrm{rank}(A)+\dim{\mathrm{Nul}(A)}=\mathrm{number\:of\:columns\:in\:A}$$

## Example

Find a matrix $A$ such that $$\set{\begin{bmatrix}b-c \\ 2b+c+d \\ 5c-4d \\ d\end{bmatrix},\:b,c,d\in\mathbb{R}}$$
$$\begin{bmatrix}b-c \\ 2b+c+d \\ 5c-4d \\ d\end{bmatrix}=b\begin{bmatrix}1 \\ 2 \\ 0 \\ 0\end{bmatrix}+c\begin{bmatrix}-1 \\ 1 \\ 5 \\ 0\end{bmatrix}+d\begin{bmatrix}0 \\ 1 \\ -4 \\ 1\end{bmatrix}$$
As $RHS$ represents the solution set as a linear combination of 3 vectors, these vectors can simply be the columns of the desired matrix $A$.
$$A=\begin{bmatrix}1 & -1 & 0 \\ 2 & 1 & 1 \\ 0 & 5 & -4 \\ 0 & 0 & 1\end{bmatrix}$$

## Implications

_for [[Linear Algebra]]_

for a [[]]
