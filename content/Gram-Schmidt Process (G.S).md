$V$ [[Subspace of Rn|subspace]] of $\mathbb{R}^n$, $\beta$ is a [[Basis of Subspaces|basis]] of $V$, the G.S. process will construct an [[Orthogonal Basis]] using the basis $\beta$.

## Example R4

$\vec{u_1}=\begin{bmatrix}1 \\ 1 \\ 1 \\ 1\end{bmatrix},\:\vec{u_2}=\begin{bmatrix}0 \\ 1 \\ 1 \\ 1\end{bmatrix},\:\vec{u_3}=\begin{bmatrix}0 \\ 0 \\ 1 \\ 1\end{bmatrix},\:\beta=\set{\vec{u_1},\vec{u_2},\vec{u_3}}$
$V=\mathrm{span}\set{\beta}$

$W_i=\mathrm{span}\set{\vec{u_1},...,\vec{u_i}}=\mathrm{span}\set{\vec{v_1},...,\vec{v_i}}$

**G.S. Process:**

1. $\vec{v_1}=\vec{u_1}$
2. $\vec{v_2}=\vec{u_2}-\mathrm{proj}_{W_1}\vec{u_2}$
   _Note: $\vec{v_2}\perp\vec{v_1}$_ by equation 1 defined in [[Orthogonal Projection]].
3. $\vec{v_3}=\vec{u_3}-\mathrm{proj}_{W_2}\vec{u_3}$

_Human: basically we sequentially subtract the components which are not orthogonal to the prior vectors to ensure every new vector is orthogonal_

$$\vec{v_1}=\vec{u_1}=\begin{bmatrix}1 \\ 1 \\ 1 \\ 1\end{bmatrix}$$
$$\vec{v_2}=\vec{u_{2}}-\mathrm{proj}_{W_1}\vec{u_2}=\begin{bmatrix}0 \\ 1 \\ 1 \\ 1\end{bmatrix}- \frac{3}{4}\begin{bmatrix}1 \\ 1 \\ 1 \\ 1\end{bmatrix}=\begin{bmatrix} \frac{-3}{4} \\ \frac{1}{4} \\ \frac{1}{4} \\ \frac{1}{4}\end{bmatrix}$$ As this is a basis, we can also set and multiply $\vec{v_2}$ by some constant $k$.
$$\vec{v_3}=\vec{u_3}-\mathrm{proj}_{W_2}\vec{u_3}=\begin{bmatrix}0 \\ 0 \\ 1 \\ 1\end{bmatrix}-\frac{\vec{u_3}\cdot\vec{v_1}}{\vec{v_1}\cdot\vec{v_1}}\vec{v_1}-\frac{\vec{u_3}\cdot\vec{v_2}}{\vec{v_2}\cdot\vec{v_2}}\vec{v_2}$$
$$\vec{v_3}=\begin{bmatrix}0 \\ 0 \\ 1 \\ 1\end{bmatrix}- \frac{2}{4}\begin{bmatrix}1 \\ 1 \\ 1 \\ 1\end{bmatrix}- \frac{2}{12}\begin{bmatrix}-3 \\ 1 \\ 1 \\ 1\end{bmatrix}=\begin{bmatrix}0 \\ \frac{-2}{3} \\ \frac{1}{3} \\ \frac{1}{3}\end{bmatrix}$$

The [[Orthogonal Basis]] is $\beta_o=\set{\vec{v_1},\vec{v_2},\vec{v_3}}$

## The General Case

$V$ [[Subspace of Rn|subspace]] of $\mathbb{R}^3$
$\set{\vec{x_1},\vec{x_2},...,\vec{x_p}}$ basis of $V$
To construct an [[Orthogonal Basis]]
$\vec{v_1}=\vec{x_1}$
$\vec{v_2}=\vec{x_2}-\frac{\vec{x_2}\cdot\vec{v_1}}{\vec{v_1}\cdot\vec{v_1}}\vec{v_1}$
$\vec{v_3}=\vec{x_3}-\frac{\vec{x_3}\cdot\vec{v_1}}{\vec{v_1}\cdot\vec{v_1}}\vec{v_1}-\frac{\vec{x_3}\cdot\vec{v_2}}{\vec{v_2}\cdot\vec{v_2}}\vec{v_2}$
...
$\vec{v_p}=\vec{x_p}-\frac{\vec{x_1}\cdot\vec{v_1}}{\vec{v_1}\cdot\vec{v_1}}\vec{v_1}...-\frac{\vec{x_p}\cdot\vec{v_{p-1}}}{\vec{v_{p-1}}\cdot\vec{v_{p-1}}}\vec{v_{p-1}}$

or $$\vec{v_p}=\vec{x_p}-\sum\limits_{i=0}^{p-1}\frac{\vec{x_p}\cdot\vec{v_i}}{\vec{v_i}\cdot\vec{v_i}}\vec{v_i}$$
