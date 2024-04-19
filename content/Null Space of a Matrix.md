## Definition
$A\in m\times n$ matrix
$\vec{x}\in\mathbb{R}^n$
The set of solutions of $A\vec{x}=0$ 

$\mathrm{Nul}{(A)}$ is a [[Subspace of Rn|subspace]] of $\mathbb{R}^n$

## Example
$$A=\begin{bmatrix}-3 & 6 & -1 & 1 & -7 \\ 1 & -2 & 2 & 3 & -1 \\ 2 & -4 & 5 & 8 & -4\end{bmatrix}$$
To find $\mathrm{Nul}(A)$, find the solution set to the augmented matrix of $A\vec{x}=\vec{0}$. This can be done using [[Matrix Row Reduction|row reduction]] to RREF form.
$$\begin{bmatrix}-3 & 6 & -1 & 1 & -7 & 0 \\ 1 & -2 & 2 & 3 & -1 & 0 \\ 2 & -4 & 5 & 8 & -4 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & -2 & 0 & -1 & 3 & 0 \\ 0 & 0 & 1 & 2 & -2 & 0 \\ 0 & 0 & 0 & 0 & 0 & 0\end{bmatrix}$$
3 free variables:
- $x_2=s$
- $x_4=t$
- $x_5=w$
This generates the following system of equations
$$
\begin{cases}
x_1=2s+t-3w \\
x_3=-2t+2w
\end{cases}
$$
forming the general solution $$\vec{x}=\begin{bmatrix}2s+t-3w \\ s \\ -2t+2w \\ t \\ w\end{bmatrix}=\begin{bmatrix}2 \\ 1 \\ 0 \\ 0 \\ 0\end{bmatrix}s+\begin{bmatrix}1 \\ 0 \\ -2 \\ 1 \\ 0\end{bmatrix}t+\begin{bmatrix}-3 \\ 0 \\ 2 \\ 0 \\ 1\end{bmatrix}w$$ it follows that the vector coefficients of the free variables form a spanning set of the null space. $$\mathrm{Nul}(A)=\mathrm{span}\set{\begin{bmatrix}2 \\ 1 \\ 0 \\ 0 \\ 0\end{bmatrix},\begin{bmatrix}1 \\ 0 \\ -2 \\ 1 \\ 0\end{bmatrix},\begin{bmatrix}-3 \\ 0 \\ 2 \\ 0 \\ 1\end{bmatrix}}$$
