## Theorem

An [[Orthogonal Set]] of vectors $S$ is [[Linear Independence|linearly independent]].

Def: An orthogonal [[Basis of Subspaces|basis]] is a basis that is an orthogonal set.
Or: all the vectors in the basis are mutually orthogonal.

Let $\beta=\set{\vec{v_1},\vec{v_2},...,\vec{v_p}}$ be an orthogonal basis.

and any vector $y\in W$ can be written
$$\vec{y}=c_1\vec{u_1}+c_2\vec{u_2}+...+c_p\vec{u_{p}}\tag{1}$$
Then: $$c_j=\frac{\vec{y}\cdot\vec{u_j}}{\vec{u_j}\cdot\vec{u_j}}$$
This equation can be used to find the [[Coordinate System|coordinate]] of a vector in an orthogonal basis.

### Proof

Take equation $(1)$ and take the dot product on both sides with $\vec{u_j}$

$$\vec{u_j}\cdot\vec{y}=\vec{u_j}\cdot(c_1\vec{u_1}+c_2\vec{u_2}+...+c_p\vec{u_{p}})$$

### Example

$$\vec{u_1}=\begin{bmatrix}3 \\ 1 \\ 1 \end{bmatrix},\:\vec{u_2}=\begin{bmatrix}-1 \\ 2 \\ 1\end{bmatrix},\:\vec{u_3}=\begin{bmatrix} \frac{-1}{2} \\ -2 \\ \frac{7}{2}\end{bmatrix}$$
The set $\set{\vec{u_1},\vec{u_2},\vec{u_3}}$ is an orthogonal set.

**Q:** write $\vec{y}=\begin{bmatrix}6 \\ 1 \\ -8\end{bmatrix}$ as a linear combination of the [[Vector|vectors]] in the set.
$$\vec{y}=c_1\vec{u_1}+c_2\vec{u_2}+c_3\vec{u_3}$$
implementing our theorem equation to solve for $c_i$
$$c_1=\frac{\vec{y}\cdot\vec{u_1}}{\vec{u_1}\cdot\vec{u_1}}=1,\:c_{2}=-2,\:c_{3}=-2$$
