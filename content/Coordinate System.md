## Definition
$V$ [[Vector Space|vector space]], $B$ [[Basis of Subspaces|basis]] for $V$ $$B=\set{\vec{b_1},\vec{b_2},\vec{b_3},...,\vec{b_n}}$$
Any $\vec{x}\in V$ can be written in a unique way as $$\vec{x}=c_1\vec{b_1}+c_2\vec{b_2}+...+c_n\vec{b_n}$$
$c_1,c_2,...,c_n$ make up the coordinate of $\vec{x}$ in the basis $B$

### Example
$V=\mathbb{R}^2,\:B=\set{\begin{bmatrix}1 \\ 2\end{bmatrix},\begin{bmatrix}3 \\ 0\end{bmatrix}}$
Find the coordinate of $\vec{v}=\begin{bmatrix}7 \\ -3\end{bmatrix}$ in the basis $B$
$$\begin{bmatrix}7 \\ -3\end{bmatrix}=a_1\begin{bmatrix}1 \\ 2\end{bmatrix}+a_2\begin{bmatrix}3 \\ 0\end{bmatrix}$$
$$\begin{cases}
a_1+3a_2=7 \\
2a_1=-3
\end{cases}$$
By observation or by a [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]],
$$a_{1}=\frac{-3}{2},\:a_{2}=\frac{17}{6}$$
Therefore, the coordinate of $\vec{v}$ in basis $B$ is $$\begin{bmatrix}\vec{x}\end{bmatrix}_{B}=\begin{bmatrix}\frac{-3}{2} \\ \frac{{17}}{{6}}\end{bmatrix}$$
## Finding a Basis
If $A\in m\times n$ matrix $$A\vec{x}=\vec{b}$$
$A=\begin{bmatrix}\vec{a_1} & \vec{a_2} & ... & \vec{a_n}\end{bmatrix}$ 
where $\vec{a_i}$ is the $i$th column of $A$
$$\vec{x}=\begin{bmatrix}x_1 \\ x_2 \\ ... \\ x_n\end{bmatrix}=x_1\vec{a_1}+x_2\vec{a_2}+...+x_n\vec{a_n}$$
Define $\set{\vec{a_1},\vec{a_2},...,\vec{a_n}}=B$ to be the [[Basis of Subspaces|basis]] of [[Vector Space|vector space]] $V$

Reaffirming:
- $\vec{x}$ the coordinate vector of $\vec{b}$ in basis $B$
- $A$ is a matrix where its columns are the vectors of basis $B$

We can then represent the vector $\vec{b}$ as $$\vec{b}=A\begin{bmatrix}\vec{b}\end{bmatrix}_B$$
Because the columns of $A$ (by definition of a [[Basis of Subspaces|basis]]) are [[Linear Independence|linearly independent]], the matrix $A$ is [[Matrix Inverse|invertible]].

multiplying by the inverse yields $$A^{-1}\cdot\vec{b}=\begin{bmatrix}\vec{b}\end{bmatrix}_B$$
Thus, we can find the coordinate of a vector $\vec{b}$ in the basis $B$ using the inverse of the matrix representing the basis $A^{-1}$

This matrix $A$ is commonly called $P_B$. 

### Example
*continuing example from [[#Example]]*
$$P_B=\begin{bmatrix}1 & 3 \\ 2 & 0\end{bmatrix}$$
computing the [[Matrix Inverse]] yields $$P_B^{-1}=\begin{bmatrix}0 & \frac{1}{2} \\ \frac{1}{3} & \frac{-1}{6}\end{bmatrix}$$ $$\vec{x}=\begin{bmatrix}7 \\ -3\end{bmatrix}\Rightarrow\begin{bmatrix}\vec{x}\end{bmatrix}_B=P_B^{-1}\cdot\vec{x}=\begin{bmatrix}0 & \frac{1}{2} \\ \frac{1}{3} & \frac{-1}{6}\end{bmatrix}\cdot\begin{bmatrix}7 \\ -3\end{bmatrix}$$
$$\begin{bmatrix}\vec{x}\end{bmatrix}_{B}=\begin{bmatrix}\frac{-3}{2} \\ \frac{{17}}{{6}}\end{bmatrix}$$
## Concluding Example
$\vec{v_1}=\begin{bmatrix}3 \\ 6 \\ 2\end{bmatrix},\:\vec{v_2}=\begin{bmatrix}-1 \\ 0 \\ 1\end{bmatrix}\in\mathbb{R}^3$
$H=\mathrm{span}\set{\vec{v_1},\vec{v_2}}$ is a [[Subspace|subspace]] of $\mathbb{R}^3$.
$B=\set{\vec{v_1},\vec{v_2}}$ is a [[Basis of Subspaces|basis]] of $H$.

Given $\vec{x}=\begin{bmatrix}3 \\ 12 \\ 7\end{bmatrix}$, determine if $\vec{x}\in H$ and if so, find its coordinates in $B$.

If $\vec{x}\in H$ then $\vec{x}$ is a [[Linear Combination|linear combination]] of the vectors in basis $B$. $$\vec{x}=c_1\vec{v_1}+c_2\vec{v_2}$$breaking into vector components$$\begin{cases}
3c_1-c_2=3 \\
6c_1=12 \\
2c_1+c_2=7
\end{cases}$$ an augmented matrix can be formed as follows: $$\begin{bmatrix}3 & -1 & 3 \\ 6 & 0 & 12 \\ 2 & 1 & 7\end{bmatrix}$$ performing [[Matrix Row Reduction]] yields $$\begin{bmatrix}1 & 0 & 2 \\ 0 & 1 & 3 \\ 0 & 0 & 0\end{bmatrix}$$ therefore the coordinate of the vector $\vec{x}$ in $B$ is: $$c_1=2,\:c_2=3\Rightarrow\begin{bmatrix}\vec{x}\end{bmatrix}_B=\begin{bmatrix}2 \\ 3\end{bmatrix}$$
