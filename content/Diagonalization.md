## Definition
$A\in n\times n$ matrix is **diagonizable** if it is [[Similar Matrix|similar]] to a [[Diagonal Matrix|diagonal matrix]]. There is a diagonal matrix $D$. There is an invertible matrix $P$ such that: $$A=PDP^{-1}$$
- The columns of $P$ are [[Linear Independence|linearly independent]] [[Eigenvectors and Eigenvalues|eigenvectors]] of $A$. 
	- These columns can be put in any order.
- The diagonal elements of $D$ are the [[Eigenvectors and Eigenvalues|eigenvalues]] of $A$. 

### Example
$$A=\begin{bmatrix}1 & 3 & 3 \\ -3 & -5 & -3 \\ 3 & 3 & 1\end{bmatrix}$$
Diagonalize $A$ if possible.

Starting with the [[Matrix Characteristic Equation]]: $$\det{(A-\lambda I)}=0$$
$$\begin{vmatrix}1-\lambda & 3 & 3 \\ -3 & -5-\lambda & -3 \\ 3 & 3 & 1-\lambda\end{vmatrix}=0$$
$$(1-\lambda)(-5-\lambda)-27-27+9(5+\lambda)+9(1-\lambda)+9(1-\lambda)=0$$
Simplifying: $(1-\lambda)(\lambda+2)^2=0$

*Note: $\lambda=-2$ has multicity of 2, meaning its eigenspace has a maximum dimension of 2*

Begin with $\lambda=1:$ 
1. construct the homogenous equation $(A-\lambda I)\vec{x}=\vec{0}$
2. construct the [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]]
3. [[Matrix Row Reduction|row reduce]] to RREF
$$\begin{bmatrix}0 & 3 & 3 & 0 \\ -3 & -6 & -3 & 0 \\ 3 & 3 & 0 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & 0 & -1 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 0 & 0\end{bmatrix}$$
Free variable: $x_3=s$
$$\begin{cases}
x_1=s \\
x_2=-s
\end{cases}$$
$$\vec{x}=\begin{bmatrix}x_1 \\ x_2 \\ x_3\end{bmatrix}=\begin{bmatrix}1 \\ -1 \\ 1\end{bmatrix}s$$
The [[Eigenvectors and Eigenvalues|eigenspace]] is now the [[Vector Span|span]] of these vectors $$\mathrm{span}\set{\begin{bmatrix}1 \\ -1 \\ 1\end{bmatrix}}$$

Next $\lambda=-2$
performing the same calculation yields the following eigenspace: $$\mathrm{span}\set{\begin{bmatrix}-1 \\ 1 \\ 0\end{bmatrix},\begin{bmatrix}-1 \\ 0 \\ 1\end{bmatrix}}$$
Therefore, the matrix $A$ has 3 [[Linear Independence|linearly independent]] [[Eigenvectors and Eigenvalues|eigenvectors]] $\Rightarrow$ $A$ is diagonalizable and
$$P=\begin{bmatrix}1 & -1 & -1 \\ -1 & 1 & 0 \\ 1 & 0 & 1\end{bmatrix}$$
Finding the [[Matrix Inverse]]:
$$P^{-1}=\begin{bmatrix}1 & 1 & 1 \\ 1 & 2 & 1 \\ -1 & -1 & 0\end{bmatrix}$$

### Example
$$A=\begin{bmatrix}4 & -3 \\ 2 & -1\end{bmatrix},\:\mathrm{calculate}\:A^8$$
1. Diagonalize $A$
	- find [[Eigenvectors and Eigenvalues]]
$$\begin{vmatrix}4-\lambda & -3 \\ 2 & -1-\lambda\end{vmatrix}=0\Rightarrow(4-\lambda)(-1-\lambda)+6=0$$
$$(\lambda-1)(\lambda-2)=0$$
Therefore, $\lambda=1,2$ both of multiplicity $1$. Then, applying the [[Matrix Characteristic Equation|characteristic equation]]. Setting $\lambda=1$
$$\begin{bmatrix}3 & -3 & 0 \\ 2 & -2 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & -1 & 0 \\ 0 & 0 & 0\end{bmatrix}\Rightarrow\vec{x}=\begin{bmatrix}1 \\ 1\end{bmatrix}s,\:x_2=s$$
$$\vec{v_1}=\begin{bmatrix}1 \\ 1\end{bmatrix}$$
And then $\lambda=2$
$$\begin{bmatrix}2 & -3 & 0 \\ 2 & -3 & 0\end{bmatrix}\Rightarrow\vec{x}=\begin{bmatrix} \frac{3}{2} \\ 1\end{bmatrix}s,\:x_2=s$$
For simplicity, we can choose $s=2$, *s can be any real number*
$$\vec{x_2}=\begin{bmatrix}3 \\ 2\end{bmatrix}$$

As there are $2$ [[Eigenvectors and Eigenvalues|eigenvectors]], $A$ is diagonalizable and: $$P=\begin{bmatrix}1 & 3 \\ 1 & 2\end{bmatrix}\Rightarrow P^{-1}=\begin{bmatrix}-2 & 3 \\ 1 & -1\end{bmatrix}$$
Diagonalizing $D=\begin{bmatrix}1 & 0 \\ 0 & 2\end{bmatrix};A=PDP^{-1}$

Now raising both sides to the power of $8$
$$A^8=(PDP^{-1})^8=PDP^{-1}PDP^{-1}PDP^{-1}...$$
Any instance of $P\cdot P^{-1}=I$, so the right side can be simplified to:
$$A^8=PD^8P^{-1}$$
Raising a [[Diagonal Matrix]] to a power is very easy, as in general:
$$\begin{bmatrix}a & 0 & 0 \\ 0 & b & 0 \\ 0 & 0 & c\end{bmatrix}^k=\begin{bmatrix}a^k & 0 & 0 \\ 0 & b^k & 0 \\ 0 & 0 & c^k\end{bmatrix}$$

Therefore:
$$A^8=\begin{bmatrix}1 & 3 \\ 1 & 2\end{bmatrix}\begin{bmatrix}1 & 0 \\ 0 & 256\end{bmatrix}\begin{bmatrix}-2 & 3 \\ 1 & -1\end{bmatrix}$$

## Theorem
A $n\times n$ matrix that has $n$ [[Linear Independence|linearly independent]] [[Eigenvectors and Eigenvalues|eigenvectors]] is diagonalizable.

Special case: $A$ is diagonalizable if it has $n$ distinct [[Eigenvectors and Eigenvalues|eigenvalues]].
