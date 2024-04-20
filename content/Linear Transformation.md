## Definition

$A\in m\times n$ matrix

$\vec{x}\in \mathbb{R}^n,\:n\times m$ matrix

$\vec{y}=A\cdot\vec{x}\in m\times 1$ matrix, this $\vec{y}\in\mathbb{R}^n$

Thus, $\vec{y}$ acts like a function, taking in any vector in $\mathbb{R}^n$ and outputting a vector in $\mathbb{R}^m$

It is called a **transformation** $T$

$T_A: \mathbb{R}^n\rightarrow\mathbb{R}^m$

Domain of $T_A$ is $\mathbb{R}^n$

Codomain of$T_A$ is $\mathbb{R}^m$

The range of a transformation:
$R(T)=$ {$\vec{y}\in\mathbb{R}^m$ for which there is an $\vec{x}\in\mathbb{R}^n$ such that $\vec{y}=T(x)$}

**What makes a transformation linear?**

1. $T(\vec{u}+\vec{v})=T(\vec{u})+T(\vec{v})$
2. $T(k\vec{u})=kT(\vec{u})$
   _These are the requirements for a linear transformation_

Note: all matrix transformations, that is, transformations resulting from multiplying a vector by a matrix, are linear.

### Example

$T:\:\mathbb{R}^2\rightarrow\mathbb{R}^2$
$$A=\begin{bmatrix}3 & 1 \\ 0 & 0\end{bmatrix},\:\vec{x}=\begin{bmatrix}x_1 \\ x_2\end{bmatrix}$$
$$T_A(\vec{x})=\begin{bmatrix}3 & 1 \\ 0 & 0\end{bmatrix}\cdot\begin{bmatrix}x_1 \\ x_2\end{bmatrix}=\begin{bmatrix}3x_1+x_2 \\ 0\end{bmatrix}$$
Q. is $\begin{bmatrix}4 \\ -1\end{bmatrix}$ is in the range of $T$?
No, because it has a non-zero second component which is not possible as can be seen above.

### Example

$$A=\begin{bmatrix}1 & 2 \\ 2 & 5 \\ -1 & 3\end{bmatrix}\Rightarrow T(\vec{x})=A\vec{x}$$
The dimension of the matrix is $3\times 2$, therefore:

- $\vec{x}\in\mathbb{R}^2$
- $A\vec{x}\in\mathbb{R}^3$
  $$T_A(\vec{x})=\begin{bmatrix}1 & 2 \\ 2 & 5 \\ -1 & 3\end{bmatrix}\begin{bmatrix}x_1 \\ x_2\end{bmatrix}=\begin{bmatrix}x_1+2x_2 \\ 2x_1+5x_2 \\ -x_1+3x_2\end{bmatrix}$$

**Question:** is $\begin{bmatrix}1 \\ 0 \\ -1\end{bmatrix}$ in the range of $T$?
Equivalent to asking, are there solutions to:
$$T_A(\vec{x})=\begin{bmatrix}1 \\ 0 \\ -1\end{bmatrix}\Rightarrow\begin{bmatrix}1 & 2 & 1 \\ 2 & 5 & 0 \\ -1 & 3 & -1\end{bmatrix}$$
Solving using [[Matrix Row Reduction]]
$$\rightarrow\begin{bmatrix}1 & 2 & 1 \\ 0 & 1 & -2 \\ 0 & 0 & 2\end{bmatrix}$$
which has no solutions, meaning the given vector is not in the range of $T$.

## 2D Transformation Types

### Shear Transformation

Can be created by "sheering" a given elementary basis.

Example: $$A=\begin{bmatrix}1  & 2\\ 0 & 1\end{bmatrix}$$
_shifts vertical vectors to the right by 2 units for every unit vertical_

### Scaling Transformation

$A=\begin{bmatrix}k & 0 \\ 0 & k\end{bmatrix}\Rightarrow A\vec{x}=\begin{bmatrix}kx_1 \\ kx_2\end{bmatrix}$

### Rotation Transformation

_Geometrically: rotates a vector about the origin, maintaining the length, counter-clockwise by an angle $\gamma$_

consider the plane $\mathbb{R}^2$. Form the standard basis by rotating the standard basis $\beta=\set{\vec{e_{1}},\vec{e_2}}$.
$$T(\vec{e_1})=\begin{bmatrix}\cos{\gamma} \\ \sin{\gamma}\end{bmatrix},\:T(\vec{e_2})=\begin{bmatrix}-\sin{\gamma} \\ \cos{\gamma}\end{bmatrix}$$
Thus,
$$A=\begin{bmatrix}\cos{\gamma} & -\sin{\gamma} \\ \sin{\gamma} & \cos{\gamma}\end{bmatrix}$$

## Matrix of a Linear Transformation

A matrix transformation is a linear transformation, but it can also be concluded that any linear transformation is a matrix transformation.

More formally,
Every linear transformation:
$T:\mathbb{R}^n\rightarrow\mathbb{R}^m$
is a matrix transformation using $A\in m\times n$ matrix.

Take the [[Basis of Subspaces#Definition Standard Basis|standard basis]] of $\mathbb{R}^n$.
$$\vec{e_1}=\begin{bmatrix}1 \\ 0 \\ 0 \\ ... \\ 0\end{bmatrix},\vec{e_2}=\begin{bmatrix}0 \\ 1 \\ 0 \\ ... \\ 0\end{bmatrix},...,\vec{e_n}=\begin{bmatrix}0 \\ 0 \\ 0 \\ ... \\ 1\end{bmatrix}$$
The $j$ column of $A$ will be $T(\vec{e_j})$ and constructs $A$ as:
$$A=\begin{bmatrix}T(\vec{e_1}) & T(\vec{e_2}) & ... & T(\vec{e_{n}})\end{bmatrix}$$
where $T(\vec{e_j})\in\mathbb{R}^m$

additionally,
$$\vec{x}=x_1\vec{e_1}+x_2\vec{e_2}+...+x_n\vec{e_n}$$
$$A\vec{x}=x_1T(\vec{e_1})+x_2T(\vec{e_2})+...+x_nT(\vec{e_n})$$

### Examples

$T:\mathbb{R}^2\rightarrow/\mathbb{R}^2$
$T(\vec{x})=3\vec{x}$

Find the matrix of $T$
$$T(\vec{e_1})=\begin{bmatrix}3 \\ 0\end{bmatrix},\:T(\vec{e_2})=\begin{bmatrix}0 \\ 3\end{bmatrix}$$
Thus the matrix of $T$ is:
$$A=\begin{bmatrix}3 & 0 \\ 0 & 3\end{bmatrix}$$

## Onto

If $T:\mathbb{R}^n\rightarrow\mathbb{R}^m$ is **onto** $\mathbb{R}^m$
Then for every vector $\vec{b}\in\mathbb{R}^m$, there is a vector $\vec{x}\in\mathbb{R}^n$ such that $T(\vec{x})=\vec{b}$. Or, the codomain of $T$ = the range of $T$.

## One-to-One

$T:\mathbb{R}^n\rightarrow\mathbb{R}^m$ is one-to-one if $$T(\vec{x_1})=T(\vec{x_2})\Rightarrow\vec{x_1}=\vec{x_2}$$
Example: projection transformations are not one-to-one.
