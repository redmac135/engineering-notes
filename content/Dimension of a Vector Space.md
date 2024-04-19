## Definition
$B$ is any [[Basis of Subspaces|basis]] for a [[Vector Space|vector space]] $V$. The number of elements in $B$ is the dimension of the vector space $V$ ($\dim{V}$).

*Note: no matter what basis you take of a vector space, the basis will have the same number of elements.*

### Example 
[[Basis of Subspaces#Definition Standard Basis|standard basis]] of $\mathbb{R}^3$ is: $$\set{\begin{bmatrix}1 \\ 0 \\ 0\end{bmatrix},\begin{bmatrix}0 \\ 1 \\ 0\end{bmatrix},\begin{bmatrix}0 \\ 0 \\ 1\end{bmatrix}}\Rightarrow\dim{\mathbb{R}^3}=3$$
## Theorem
If $B=\set{\vec{v_{1}},\vec{v_{2}},...,\vec{v_r}}$ is a basis of $V$, and we add a new vector to $B$, $\vec{v'}\in V$, then $B'=\set{\vec{v_{1}},\vec{v_{2}},...,\vec{v_r},\vec{v'}}$ will be [[Linear Independence|linearly dependent]].

### Example
$P_n$ space of polynomials of degree $\le n$
$P_n$ is a [[Vector Space|vector space]]

$\dim{P_n}=n+1$

**proof by example:**
Any element in $P_n$ can be represented as: $$c_1+c_2x+c_3x^2+...+c_{n+1}x^n$$
