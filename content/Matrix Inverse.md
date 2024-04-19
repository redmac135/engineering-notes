only a square matrix can have an inverse
$A\in n\times n$ matrix

## Definition Invertibility

$A$ is invertible if there is a matrix $A^{-1}$ such that $A\cdot A^{-1}=A^{-1}\cdot A=I$ the [[Identity Matrix|identity matrix]]

If $A$ is not invertible, it is called a **singular matrix**

The following statements are equivalent

1. $A$ is invertible
2. $A$ is row equivalent to $I$ [[Identity Matrix]]
3. $A$ is $n$ [[Pivot Position|pivot positions]]
4. The system $A\cdot\vec{x}=0$ has only the trivial (zero) solution.
5. The system $A\cdot\vec{x}=\vec{b}$ has at least one solution for every $\vec{b}$
6. [[Vector Span]] of the columns of $A$ span all of $\mathbb{R}^n$

## Finding the Inverse

using [[Matrix Row Reduction]]

$A\in n\times n$ matrix
$A^{-1}$ can be found by constructing a matrix
$$\begin{bmatrix}A & I\end{bmatrix}$$
and performing [[Matrix Row Reduction|row reduction]] until it is in RREF form. The result will be: $$\begin{bmatrix}I & A^{-1}\end{bmatrix}$$
If $I$ is not found on the left (there isn't a [[Pivot Position|pivot position]] in each row), then $A$ is not invertible

### For 2x2 Matrix

$A\in 2\times2\:\mathrm{Matrix}$
$A=\begin{bmatrix}1 & b \\ c & d\end{bmatrix}\:a,b,c,d\in\mathbb{R}$

$A$ is invertible if its determinant $ad-bc\ne0$

$\Rightarrow A^{-1}=\frac{1}{ad-bc}\begin{bmatrix}d & -b \\ -c & a\end{bmatrix}$ _Note: main diagonal values swapped and other values times -1_

## Properties

$(A^{-1})^{-1}=A$

$(A^T)^{-1}=(A^-1)^T$
[[Matrix Transpose]]

$(A\cdot B)^{-1}=B^{-1}\cdot A^{-1}$
_Note: A and B swapped_

## Theorem Matrix Equation

Consider the [[Matrix Equation]]
$$A\vec{x}=\vec{b}$$ multiply **in front** both sides with the inverse
$$A^{-1}\cdot A\cdot\vec{x}=A^{-1}\cdot\vec{b}$$
$$\vec{x}=A^{-1}\cdot\vec{b}$$
Therefore, if $A$ is invertible, then there exists a unique solution for every $\vec{b}\in\mathbb{R}^n$
