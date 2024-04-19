## Definition

$\lambda$ [[Eigenvectors and Eigenvalues|eigenvalue]] of $A$: $$A\vec{x}=\lambda\vec{x}\Leftrightarrow(A-\lambda I)\vec{x}=0$$
If the above equation has non-zero solutions, then $(A-\lambda I)$ is [[Matrix Inverse|singular]] (or not invertible). Therefore, its [[Determinant of a Matrix|determinant]] must be 0.

Therefore, in order for $\lambda$ to be a value eigenvalue: $$\det{(A-\lambda I)}=0$$
The above is the characteristic equation.

### Example Critical

Find the [[Eigenvectors and Eigenvalues|eigenvalues]] of $A=\begin{bmatrix}2 & 3 \\ 3 & -6\end{bmatrix}$

using the characteristic equation: $$\begin{vmatrix}2-\lambda & 3 \\ 3 & -6-\lambda\end{vmatrix}=0$$ $$(2-\lambda)(-6-\lambda)-(3)(3)=0$$ $$\lambda^2+4\lambda-21=0\Rightarrow(\lambda+7)(\lambda-3)$$ Therefore, $$\lambda=3, -7$$
$(\lambda+7)^1\cdot(\lambda-3)^1$
Both of these factors have a multiplicity of 1 (each factor is only power 1), meaning their respective eigenspaces can have a maximum dimension of 1.

_Notice how the order of the resulting polynomial is the same as the number of columns or rows of the matrix $A$, or, if $A\in n\times n$ then $\lambda$ can have at most $n$ solutions._

For
$\lambda=-7$
using the [[Eigenvectors and Eigenvalues|eigenvector equation]], $$(A+7I)\vec{x}=0$$ $$\begin{bmatrix}9 & 3 \\ 3 & 1\end{bmatrix}\begin{bmatrix}x_1 \\ x_2\end{bmatrix}=\begin{bmatrix}0 \\ 0\end{bmatrix}$$
once again, constructing an [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]] and solving for the possible values of $\vec{x}$:
$$\begin{bmatrix}9 & 3 & 0 \\ 3 & 1 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & \frac{1}{3} & 0 \\ 0 & 0 & 0\end{bmatrix}\Rightarrow\mathrm{let}\:x_2=s$$
$$\vec{x}=\begin{bmatrix} \frac{-1}{3} \\ 1\end{bmatrix}s$$
Therefore, $\set{\begin{bmatrix} \frac{-1}{3} \\ 1\end{bmatrix}}$ forms the basis for the eigenspace of $A$ with the [[Eigenvectors and Eigenvalues|eigenvector]] $\lambda$

## Invertible Matrix Theorem

$A\in n\times n$ an [[Matrix Inverse|invertible]] matrix, then, $A\vec{x}=0$ only has the zero solution.

And, $(A-0\cdot I)\vec{x}=0$ only has the trivial solution.

Then 0 is not an eigenvalue of $A$

likewise, it can be said that if $0$ is not an eigenvalue, then $A$ is invertible.
