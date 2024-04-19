## Definition

Define: $\vec{u},\vec{v}\in V=\mathbb{R}^n$ $n\times1$ matrices
$$\vec{u}=\begin{bmatrix}u_1 \\ u_2 \\ … \\ u_n\end{bmatrix},\vec{v}=\begin{bmatrix}v_1 \\ v_2 \\ … \\ v_n\end{bmatrix}$$
$\vec{u}^T$ is a $1\times n$ matrix where: $$\vec{u}^T=\begin{bmatrix}u_1 & u_2 & … & u_n\end{bmatrix}$$
Using [[Matrix Operations#Matrix Multiplication|matrix multiplication]]
$$\vec{u}^T\cdot \vec{v}=u_1v_1+u_2v_2+…+u_nv_n$$
We now define the **inner product** of $\vec{u}$ and $\vec{u}$ as:
$$\vec{u}\cdot\vec{v}=\vec{u}^T \vec{v}$$
This is also called:

- Scalar Product
- Dot Product

## Angle

The inner product can also be computed using $\cos$.
$\vec{v_1}\cdot\vec{v_2}=|\vec{v_1}||\vec{v_2}|\cos{\theta}$
where $\theta$ is the angle between the vectors.

## Properties

1. $\vec{u}\cdot\vec{v}=\vec{v}\cdot\vec{u}$
2. $\vec{u}\cdot(\vec{v}+\vec{w})=\vec{u}\cdot\vec{v}+\vec{u}\cdot\vec{w}$
3. $(c\vec{u})\cdot\vec{v}=\vec{u}\cdot(c\vec{v})=c(\vec{u}\cdot\vec{v})$
4. $\vec{u}\cdot\vec{u}\ge0$
5. $\vec{u}\cdot\vec{u}=0\Leftrightarrow\vec{u}=0$

If $V$ is an [[Vector Space]], an **inner product** is an operation that will satisfy properties 1 to 5.

## Length of a Vector

_"double absolute value" sign is used_
$$||\vec{u}||=\sqrt{\vec{u}\cdot\vec{u}}=\sqrt{u_1^2+u_2^2+…+u_n^2}$$
The distance between two vectors can be represented as:
$$d(\vec{u},\vec{v})=||\vec{u}-\vec{v}||$$
And:
$$d(\vec{u}, \vec{v})=0\Rightarrow\vec{u}-\vec{v}=0\Rightarrow\vec{u}=\vec{v}$$
_Human: If the distance between two vectors is zero, then they are the same vector_
