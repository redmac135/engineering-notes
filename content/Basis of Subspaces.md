## Definition
$V$ is a [[Subspace of Rn|subspace]] of $\mathbb{R}^n$
Collection of vectors in $V$, $\set{\vec{v_1},\vec{v_2},...,\vec{v_r}}$ is called a basis of $V$ if
1. $\set{\vec{v_1},\vec{v_2},...,\vec{v_r}}$ is [[Linear Independence|linearly independent]]
2. $\mathrm{span}\set{\vec{v_1},\vec{v_2},...,\vec{v_r}}=V$

### Example
$V$ = space of polynomials of degree $\le2$
$$p_1=1-x,\:p_2=1+x,\:p_3=2+x^2$$
$B=\set{p_1,p_2,p_3}$ is a basis of $V$

**1. Does $B$ span $V$**
$$y(1-x)+w(1+x)+z(2+x^2)=a+bx+cx^2$$
$$(y+w+2z)+(-y+w)x+zx^2$$
this can then represent a linear system
$$\begin{cases}y+w+2z=a \\
-y+w=b \\
z=c\end{cases}$$
create a [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]] and [[Matrix Row Reduction|row reduce]] to REF form to test if only one unique solution exists for every $a,b,c$

**2. Is the Set $B$ [[Linear Independence|Linearly Independent]]**
As they form a basis of $V$ the set must be linearly independent. 

## Theorem
any vector $\vec{v_i}\in{V}$ can be written in a unique way as a [[Linear Combination|linear combination]] of elements of the basis 

### Proof by Contradiction
$\set{\vec{v_1},\vec{v_2},...,\vec{v_r}}$ basis of $V$
assume $\vec{v}\in V$ can be written in 2 ways
$\vec{v}=a_1\vec{v_1}+a_2\vec{v_2}+...+a_r\vec{v_r}$
$\vec{v}=b_1\vec{v_1}+b_2\vec{v_2}+...+b_r\vec{v_r}$

making a homogenous equation to prove [[Linear Independence]]$$$\vec{0}=(a_1-b_1)\vec{v_1}+(a_2-b_2)\vec{v_2}+...$$if $a_i\ne{b_i}$ then $\set{\vec{v_1},\vec{v_2},...,\vec{v_r}}$ is linearly dependent, which contradicts initial assumption that $S$ is a basis. 

## Definition Standard Basis
The standard basis of $\mathbb{R}^n$ is made up of the vectors $$\vec{e_1}=\begin{bmatrix}1 \\ 0 \\ 0 \\ ... \\ 0\end{bmatrix},\vec{e_2}=\begin{bmatrix}0 \\ 1 \\ 0 \\ ... \\ 0\end{bmatrix},\vec{e_3}=\begin{bmatrix}0 \\ 0 \\ 1 \\ ... \\ 0\end{bmatrix},\vec{e_n}=\begin{bmatrix}0 \\ 0 \\ 0 \\ ... \\ 1\end{bmatrix}$$
*Note: a standard basis only applies to [[Vector Space|vector spaces]] of $\mathbb{R}^n$*

$\set{\vec{e_1},\vec{e_2},...,\vec{e_n}}$ form a basis for $\mathbb{R}^n$ called the standard basis.

$\vec{x}\in\mathbb{R}^n,\vec{x}=\begin{bmatrix}x_1 \\ x_2 \\ ... \\ x_n\end{bmatrix}$
$$\vec{x}=x_1\vec{e_1}+x_2\vec{e_2}+...+x_n\vec{e_n}$$
then,
$(x_1,x_2,...,x_n)$ are the [[Coordinate System|coordinate]] of $\vec{x}$ in the given matrix using the standard basis.

## The Basis Theorem
$H$ is a subspace of $\mathbb{R}^n$
$p=\dim(H)$ 
([[Dimension of a Subspace|dimension]])

1. A [[Linear Independence|linearly independent]] set of $p$ vectors $H$ is a basis for $H$.
2. A set of $p$ vectors in $H$ that [[Vector Span|span]] $H$ is a basis for $H$.

$\beta=\set{\vec{b_{1}},\vec{b_{2}}, ...,\vec{b_p}}$ is a basis for $H$, 
$\Rightarrow$ Any $\vec{x}\in H$ can be written uniquely as $\vec{x}=c_1\vec{b_{1}}+ c_2\vec{b_2}+...+c_p\vec{b_p}$

$\set{c_1,c_2,...,c_{p}}$ - the [[Coordinate System|coordinate]] of $\vec{x}$ in the basis $\beta$ 

$$[\vec{x}]_\beta=\begin{bmatrix}c_1 \\ c_2 \\ ... \\ c_p\end{bmatrix},\:c_i\in\mathbb{R}$$

### Example
$\vec{v_1}=\begin{bmatrix}3 \\ 5 \\ 2\end{bmatrix}, \vec{v_2}=\begin{bmatrix}-1 \\ 0 \\ 1\end{bmatrix}, \vec{x}=\begin{bmatrix}3 \\ 12 \\ 7\end{bmatrix}$
there are in $\mathbb{R}^3$

$H=\mathrm{span}\set{\vec{v_1},\vec{v_2}}$ is a subspace of $\mathbb{R}^3$
$\set{\vec{v_1},\vec{v_2}}$ are linearly independent. Thus, $\beta=\set{\vec{v_1},\vec{v_2}}$ is a basis for $H$. $$\dim{H}=2$$
1. does $\vec{x}\in H$ 
it does if the equation $$v_1\vec{v_1}+c_2\vec{v_2}=\vec{x}$$has solutions

*note: because $\set{\vec{v_1},\vec{v_2}}$ is a basis, this system cannot have infinitely many solutions*

$$c_1\begin{bmatrix}3 \\ 6 \\ 2\end{bmatrix}+c_2\begin{bmatrix}-1 \\ 0 \\ 1\end{bmatrix}=\begin{bmatrix}3 \\ 12 \\ 7\end{bmatrix}$$
Augmented matrix:
$$\begin{bmatrix}3 & -1 & 3 \\ 6 & 0 & 12 \\ 2 & 1 & 7\end{bmatrix}\rightarrow\begin{bmatrix}1 & 0 & 2 \\ 0  & 1 & 3 \\ 0 & 0 & 0\end{bmatrix}$$
through [[Matrix Row Reduction|row reduction]]

thus, this system does have solutions. So $\vec{x}\in H$.

From the [[Matrix Row Reduction|row reduced]] matrix, the unique solution for this system is $c_1=2,c_2=3$. The coordinate vector for $\vec{x}$ in basis $\beta$ is $$\begin{bmatrix}\vec{x}\end{bmatrix}_\beta=\begin{bmatrix}2 \\ 3\end{bmatrix}\in\mathbb{R}^2$$
In the basis $\beta$, $H$ can be visualized as $\mathbb{R}^2$
- 1 to 1 correspondence between $H$ and $\mathbb{R}^2$
- $\vec{x}\to\begin{bmatrix}\vec{x}\end{bmatrix}_{\beta}$ isomorphism
which basically means, every element in $H$ can be mapped to an element of $\mathbb{R}^2$ and the inverse is also true.

$\Rightarrow H$ is isomorphic to $\mathbb{R}^2$

---
$A$ is a $n\times n$ matrix. The following statements are equivalent:
1. $A$ is [[Matrix Inverse|invertible]]
2. The columns of $A$ form a basis of $\mathbb{R}^n$
3. $\mathrm{Col}(A)=\mathbb{R}^n$
4. $\mathrm{rank}(A)=n$
5. $\dim{\mathrm{Nul}(A)}=0$ which means the only solution is the trivial solutions.  
6. Null space of $A$ is made of only of $\set{\vec{0}}$

### Example
$$A=\begin{bmatrix}2 & 5 & -3 & -4 & 8 \\ 4 & 7 & -4 & -3 & 9 \\ 6 & 9 & -5 & 2 & 4 \\ 0 & -9 & 6 & 5 & -6\end{bmatrix}$$find rank($A$) 

Use [[Matrix Row Reduction|row reduction]] $$A\to\begin{bmatrix}2 & 5 & -3 & -4 & 8 \\ 0 & -3 & 2 & 5 & -7 \\ 0 & 0 & 0 & -2 & 3 \\ 0 & 0 & 0 & 0 & 1\end{bmatrix}$$ this matrix has 4 pivot points $\Rightarrow \mathrm{rank} A = 4$ 

The nullity of $A$ can be found by subtracting the number of columns with the rank
Nul $A$ = Columns of $A$ - Nul $A$ = 5 - 4 = 1
