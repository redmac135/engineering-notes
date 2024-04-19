## Systems of Linear Equations

#### Def: Linear Equation

$$a_1x_1+a_2x_2+a_3x_3+...+a_nx_n=b$$
unknown: $x_i$
coefficients: $a_i$

Ex: $5x_i-7x_2+x_3=11$
_note: highest power = 1_

#### Def: Linear System

A set of more than 1 linear equation

Ex.
$$\begin{cases}x_1+x_2=2\\x_1-x_2=0\end{cases}$$
This system has 1 unique solution.

Ex.

$$
\begin{cases}
x_1+x_2=1 \\
x_1+x_2=3
\end{cases}
$$

This system has no solutions
Term: inconsistent - a system is inconsistent if there's no solutions. If there is 1 or more solutions, it is consistent.

$$
\begin{cases}
x_1+x_2=2 \\
2x_1+2x_2=4
\end{cases}
$$

This system has infinitely many solutions

### Matrix Notation of a System

$$
\begin{cases}
x_1+x_2-2x_3=2 \\
2x_1-3x_2+2x_3=4 \\
x_1-x_2+x_3=-1 \\
\end{cases}
$$

#### Matrix of Coefficients

Can be constructed using the coefficients in the linear system where rows are the equations.
_Note: these values can be matched visually_

Matrix of coefficients ($A_c$): $$A_{c}=\begin{bmatrix}1 & 1 & -2 \\ 2 & -3 & 2 \\ 1 & -1 & 1\end{bmatrix}$$

#### Augmented Matrix of Coefficients

Define the solution vector $\vec{b}$ as the vector of the right size of each linear equation in the linear system. This vector can be appended to the right of matrix $A_c$ to create the augmented matrix of coefficient $A_a$. $$A_a=\begin{bmatrix}1 & 1 & -2 & 2 \\ 2 & -3 & 2 & 4 \\ 1 & -1 & 1 & -1\end{bmatrix}$$
[[Matrix Row Reduction]] can now be performed on the augmented matrix.

## [[Vector]]

_1.3 Vector Equations_

## [[Matrix Operations]]

_2.1 Matrix Operations_

## [[Matrix Inverse]]

_2.2 The Inverse of a Matrix_

## [[Elementary Matrices]]

## [[Linear Independence]]

_1.7 Linear Independence_

## [[Subspace of Rn]]

_2.8 Subspaces of Rn_

## [[Basis of Subspaces]]

_2.8 Subspaces of Rn_

## [[Dimension of a Subspace]]

_2.9 Dimension of a Subspace and Rank of a Matrix_

## [[Basis of Subspaces#The Basis Theorem|The Basis Theorem]]

_2.9 Dimension of a Subspace and Rank of a Matrix - continued_

## [[Determinant of a Matrix]]

_3.1 Determinants_

## [[Cramer's Rule]]

_3.3 Cramer's Rule_

## [[Subspace of Vector Space]] and [[Vector Space]]

_4.1 Vector Spaces and Subspaces_

## [[Null Space of a Matrix]] and [[Column Space of a Matrix]]

_4.2 Null Space, Column Spaces_

## [[Coordinate System]]

_4.4 Coordinate Systems_

## [[Dimension of a Vector Space]]

_4.5 Dimension of a Vector Space_

## [[Eigenvectors and Eigenvalues]]

_5.1 Eigenvectors, Eigenvalues_

## [[Matrix Characteristic Equation]]

_5.2 The Characteristic Equation_

## [[Diagonalization]]

_5.3 Diagonalization_

## [[Inner Product]]

_6.1 Inner Product Orthogonality_

## [[Orthogonal Set]]

_6.2 Orthogonal Sets_

- [[Orthogonal Basis]]

## [[Orthogonal Projection]]

_6.3 Orthogonal Projections_

- [[Orthonormal Set]]

## [[Gram-Schmidt Process (G.S)]]

_6.4 The Gram-Schmidt Process_

## [[Linear Transformation]]

_1.8 Introduction to Linear Transformation_
_1.9 The Matrix of a Linear Transformation_
