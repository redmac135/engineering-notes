## Definition Subspaces

$V$ is a [[Vector Space|vector space]]
$H\subseteq V$ a subset of $V$ is called a subspace of $V$ if:

1. $0\in H$
2. $u,v\in{H}\Rightarrow u+v\in H$
3. $u\in H,c\in\mathbb{R}\Rightarrow cu\in H$
   These ensure that $H$ is a vector space.

### Example

$V=$ space of functions defined on $\mathbb{R}$
$H=$ set of polynomials with real coefficients

$H$ is a subspace of $V$

### Example

$V$ [[Vector Space|vector space]]
$v_1,v_2,...,v_p\in{V}$
$H=\mathrm{span}\set{v_1,v_2,...,v_p}$ is a subspace of $V$

### Example

$V=$ set of all functions defined on $\mathbb{R}$
$\sin{x},\cos{x}\in V$

$H=\set{a\sin{x}+b\cos{x};\:a,b\in\mathbb{R}}$ is a subspace of $V$

### Example

$V=\mathbb{R}^4$
$H=\set{\begin{bmatrix}a-3b \\ b-a \\ a \\ b\end{bmatrix},\mathrm{where\:}a,b\in\mathbb{R}}$

$\begin{bmatrix}1-3b \\ b-a \\ a \\ b\end{bmatrix}=\begin{bmatrix}a \\ -a \\ a \\ 0\end{bmatrix}+\begin{bmatrix}-3b \\ b \\ 0 \\ b\end{bmatrix}=a\begin{bmatrix}1 \\ -1 \\ 1 \\ 0\end{bmatrix}+b\begin{bmatrix}-3 \\ 1 \\ 0 \\ 1\end{bmatrix}$

therefore, $$H=\mathrm{span}\set{\begin{bmatrix}1 \\ -1 \\ 1 \\ 0\end{bmatrix},\begin{bmatrix}-3 \\ 1 \\ 0 \\ 1\end{bmatrix}}$$
Ref: [[Vector Span]]
