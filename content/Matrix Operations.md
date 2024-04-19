prerequisites: [[Matrix Shorthand]]

## Addition

_Only matrices of the same dimension can be added._
$A,B\in m\times n\:\mathrm{matrix}$
$A=\begin{bmatrix}a_{ij}\end{bmatrix},B=\begin{bmatrix}b_{ij}\end{bmatrix}$
$\Rightarrow A+B=[a_{ij}+b{ij}]$

## Multiplication by Scalar

$A,B\in m\times n\:\mathrm{matrix}, k\in\mathbb{R}$
$A=\begin{bmatrix}a_{ij}\end{bmatrix}$
$\Rightarrow k\cdot{A}=\begin{bmatrix}ka_{ij}\end{bmatrix}$

## Matrix Multiplication

$A\in m\times n\:\mathrm{matrix}, B\in n\times p\:\mathrm{matrix}$
$A=\begin{bmatrix}\vec{a_{i}}\end{bmatrix},\vec{a_i}\in\mathbb{R}^m$
$B=\begin{bmatrix}\vec{b_{j}}^T\end{bmatrix},\vec{b_j}^T\in\mathbb{R}^p$ [[Matrix Transpose]]

$\Rightarrow A\cdot{B}=\begin{bmatrix}\vec{a_i}\cdot\vec{b_j}\end{bmatrix}\in m\times p$ matrix
_dot product_

or$\Rightarrow (A\cdot B)_{ij}=a_{i1}\cdot b_{1j}+a_{i2}\cdot b_{2j} +...+ a_{in}\cdot b_{nj}$

### Powers

if $A$ is a square matrix
$A^k=A\cdot A\cdot A\cdot ...\in n\times n$ matrix
High powers can be calculated using [[Diagonalization]]

## Properties

_Assuming all valid operations_

1. $A\cdot(B+C)=A\cdot B+A\cdot C$
2. $A\cdot B\ne B\cdot A, A\ne B$
3. $A\cdot I=I\cdot A=A$ [[Identity Matrix]]
4. $(kA)\cdot B=A\cdot(kB)$

## Transpose

![[Matrix Transpose]]
