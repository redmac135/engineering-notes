A system of equations in matrix form with $n$ equations and $n$ unknown.

Matrix form: $$A\vec{x}=\vec{b}$$ where:

- $A\in n\times n$ matrix and is invertible ($\det{A}\ne0$)
  For any $\vec{b}$ in $\mathbb{R}^n$, the solution of the system is: $$x_i=\frac{\det{A_i(\vec{b})}}{\det{A}}$$ where $A_i(\vec{b})$ is the determinate of the matrix obtained by replacing the $i$th column of $A$ with $\vec{b}$.

## Example

$$A=\begin{bmatrix}3 & -2 \\ -5 & 4\end{bmatrix}, \vec{b}=\begin{bmatrix}6 \\ 8\end{bmatrix}$$
$$\det{A}=\begin{vmatrix}3 & -2\\-5 & 4\end{vmatrix}=12-10=2$$
$$\det{A_1(\vec{b})}=\begin{vmatrix}6 & -2 \\ 8 & 4\end{vmatrix}=40$$
$$\det{A_2(\vec{b})}=\begin{vmatrix}3 & 6 \\ -5 & 8\end{vmatrix}=54$$
Thus,
$$x_{1}=\frac{40}{2}=20$$
$$x_{2}=\frac{54}{2}=27$$
