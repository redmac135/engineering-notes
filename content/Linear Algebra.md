## Systems of Linear Equations
#### Def: Linear Equation
$$a_1x_1+a_2x_2+a_3x_3+...+a_nx_n=b$$
unknown: $x_i$
coefficients: $a_i$

Ex: $5x_i-7x_2+x_3=11$
*note: highest power = 1*

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
*Note: these values can be matched visually*

Matrix of coefficients ($A_c$): $$A_{c}=\begin{bmatrix}1 & 1 & -2 \\ 2 & -3 & 2 \\ 1 & -1 & 1\end{bmatrix}$$
#### Augmented Matrix of Coefficients
Define the solution vector $\vec{b}$ as the vector of the right size of each linear equation in the linear system. This vector can be appended to the right of matrix $A_c$ to create the augmented matrix of coefficient $A_a$. $$A_a=\begin{bmatrix}1 & 1 & -2 & 2 \\ 2 & -3 & 2 & 4 \\ 1 & -1 & 1 & -1\end{bmatrix}$$
[[Matrix Row Reduction]] can now be performed on the augmented matrix. 

## [[Vector]]
*1.3 Vector Equations*

## [[Matrix Operations]]
*2.1 Matrix Operations*

## [[Matrix Inverse]]
*2.2 The Inverse of a Matrix*

## [[Elementary Matrices]]

## [[Linear Independence]]
*1.7 Linear Independence*

## [[Subspace of Rn]]
*2.8 Subspaces of Rn*

## [[Basis of Subspaces]]
*2.8 Subspaces of Rn*

## [[Dimension of a Subspace]]
*2.9 Dimension of a Subspace and Rank of a Matrix*

## [[Basis of Subspaces#The Basis Theorem|The Basis Theorem]]
*2.9 Dimension of a Subspace and Rank of a Matrix - continued*

## [[Determinant of a Matrix]]
*3.1 Determinants*

## [[Cramer's Rule]]
*3.3 Cramer's Rule*

## [[Subspace of Vector Space]] and [[Vector Space]]
*4.1 Vector Spaces and Subspaces*

## [[Null Space of a Matrix]] and [[Column Space of a Matrix]]
*4.2 Null Space, Column Spaces*

## [[Coordinate System]]
*4.4 Coordinate Systems*

## [[Dimension of a Vector Space]]
*4.5 Dimension of a Vector Space*

## [[Eigenvectors and Eigenvalues]]
*5.1 Eigenvectors, Eigenvalues*

## [[Matrix Characteristic Equation]]
*5.2 The Characteristic Equation*

## [[Diagonalization]]
*5.3 Diagonalization*

## [[Inner Product]]
*6.1 Inner Product Orthogonality*

## [[Orthogonal Set]]
*6.2 Orthogonal Sets*
- [[Orthogonal Basis]]

## [[Orthogonal Projection]]
*6.3 Orthogonal Projections*
- [[Orthonormal Set]]

## [[Gram-Schmidt Process (G.S)]]
*6.4 The Gram-Schmidt Process*

## [[Linear Transformation]]
*1.8 Introduction to Linear Transformation*
*1.9 The Matrix of a Linear Transformation*