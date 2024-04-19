## Definition Project on Subspace
$\mathbb{R}^n,\:W$ [[Subspace of Rn]]
$\vec{y}\in{\mathbb{R}^n}$

**Def:** $\mathrm{proj}_W\:\vec{y}$ is the unique [[Vector]] in $W$ such that $\vec{y}-\mathrm{proj}_W\:\vec{y}\perp{W}$

Property: $\mathrm{proj}_W\:\vec{y}$ is the [[Vector]] in $W$ that is closest to $\vec{y}$.

If $y\in W\Rightarrow\mathrm{proj}_W\:\vec{y}=\vec{y}$

## Theorem
If $W$ is a [[Subspace]] of $\mathbb{R}^n$

$\vec{y}\in \mathbb{R}^n$ can be written as 

$$
\vec{y}=\mathrm{proj}_W\:\vec{y}+\vec{z}\tag{1}
$$

where $\mathrm{proj}_W\:\vec{y}\in W$ and $\vec{z}\perp{W}$

if $S=\set{\vec{u_1},\vec{u_2},...,\vec{u_p}}$ is a [[Orthogonal Basis]] of $W$. 

Then:

$$\mathrm{proj}_W\:\vec{y}=\frac{\vec{y}\cdot\vec{u_1}}{\vec{u_1}\cdot\vec{u_1}}\vec{u_1}+...+\frac{\vec{y}\cdot\vec{u_p}}{\vec{u_p}\cdot\vec{u_p}}\vec{u_p}$$

*Human: The projection of a vector onto a subspace is the sum of the projections of that vector onto each of the orthogonal bases for the subspace.*

if $S$ is an [[Orthonormal Basis]], then the equation simplifies to:
$$\mathrm{proj}_{W}\vec{y}=(\vec{y}\cdot\vec{u_1})\vec{u_1}+...+(\vec{y}\cdot\vec{u_p})\vec{u_p}$$

### Example
$\mathbb{R}^3, \vec{u_1}=\begin{bmatrix}2 \\ 5 \\ -1\end{bmatrix},\vec{u_2}=\begin{bmatrix}-2 \\ 1 \\ 1\end{bmatrix}$

$\vec{u_1}$ and $\vec{u_2}$ are [[Orthogonal Vectors|orthogonal]] as $\vec{u_1}\cdot\vec{u_2}=0$

$W=\mathrm{span}\set{\vec{u_1},\vec{u_2}}$ [[Subspace of Rn|subspace]] of $\mathbb{R}^3$ 

$B=\set{\vec{u_1},\vec{u_2}}$ is an [[Orthogonal Basis]] for $W$. 

Let $\vec{y}=\begin{bmatrix}1 \\ 2 \\ 3\end{bmatrix}$. Find $\mathrm{proj}_{W}\vec{y}$

$$\mathrm{proj}_{W}\vec{y}=\frac{\vec{y}\cdot\vec{u_1}}{\vec{u_1}\cdot\vec{u_1}}\vec{u_1}+\frac{\vec{y}\cdot\vec{u_2}}{\vec{u_2}\cdot\vec{u_2}}\vec{u_2}$$

$$\mathrm{proj}_{W}\vec{y}=\frac{2+10-3}{4+25+1}\cdot\begin{bmatrix}2 \\ 5 \\ -1\end{bmatrix}+\frac{-2+2+3}{4+1+1}\cdot\begin{bmatrix}-2 \\ 1 \\ 1\end{bmatrix}$$

$$\mathrm{proj}_{W}\vec{y}=\begin{bmatrix} \frac{-2}{5} \\ 2 \\ \frac{1}{5}\end{bmatrix}$$

Therefore:

$$\vec{z}=\vec{y}-\mathrm{proj}_{W}\vec{y}=\begin{bmatrix}1 \\ 2 \\ 3\end{bmatrix}-\begin{bmatrix} \frac{-2}{5} \\ 2 \\ \frac{1}{5}\end{bmatrix}=\begin{bmatrix} \frac{7}{5} \\ 0 \\ \frac{14}{5}\end{bmatrix}$$

$\vec{z}$ should then be [[Orthogonal Vectors]] to both $\mathrm{proj}_{W}\vec{y}$ and every element of $B$. 

### Example
$W$ [[Subspace of Rn]]


## Projection on Vector
Let $\vec{u}\in \mathbb{R}^n,\:\vec{y}\in \mathbb{R}^n$
We can write $\vec{y}=\vec{y_1}+\vec{y_2}$, where $\vec{y_1}=\alpha{\vec{u}}$ and $\vec{y_2}$ is [[Orthogonal Set|orthogonal]] to $\vec{u}$. 
*Initiatively, this just means breaking $\vec{y}$ into components*

$$\vec{y_2}=\vec{y}-\vec{y_1}\perp\vec{u}$$
$$0=(\vec{y}-\vec{y_1})\cdot\vec{u}=\vec{y}\cdot\vec{u}-\alpha\vec{u}\cdot\vec{u}$$
$$\alpha\vec{u}\cdot\vec{u}=\vec{y}\cdot\vec{u}$$
$$\alpha=\frac{\vec{y}\cdot\vec{u}}{\vec{u}\cdot\vec{u}}$$

We then call $\vec{y_1}$ the projection of $\vec{y}$ onto $\vec{u}$ or:
$$\vec{y_1}=\mathrm{proj}_{\vec{u}}\:\:\vec{y}=\frac{\vec{y}\cdot\vec{u}}{\vec{u}\cdot\vec{u}}\vec{u}\Rightarrow\vec{y}=\alpha\vec{u}$$

