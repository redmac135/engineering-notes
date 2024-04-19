## Definition Linearly Independent
Linear independence is a property of [[Vector Space|vector spaces]].

$S$ [[Vector Space|vector space]] has items $\set{s_1,s_2,...,s_p}$ and is linearly independent if the equation $$x_1s_2+x_2s_2+...+x_ps_p=0$$ only has the zero trivial solution ($x_1=x_2=...=x_p=0$)

If a system is not linearly independent $\Rightarrow$ it is linearly dependent

*If the [[Zero Vector|zero vector]] is in the set, the set is automatically linearly dependent*

### Example 1 Set of Vectors
Consider the homogenous system
$$\begin{bmatrix}1 & 4 & 2 \\ 2 & 5 & 1 \\ 3 & 6 & 0\end{bmatrix}\begin{bmatrix}x_1 \\ x_2 \\ x_3\end{bmatrix}=\begin{bmatrix}0 \\ 0 \\ 0\end{bmatrix}$$

the system has only the zero solution $\Leftrightarrow$ the column vectors are linearly independent

**using [[Matrix Row Reduction]]**
$$\begin{bmatrix}1 & 4 & 2 & 0 \\ 2 & 5 & 1 & 0 \\ 3 & 6 & 0 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & 4 & 2 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 0 & 0\end{bmatrix}$$
$x_3$ is a free variable
- there are an infinite amount of solutions
- the columns are not linearly independent
- the columns of the matrix form a linearly dependent set

*Note: if a set $S$ contains more than one vector and one of the vectors is the zero vector $\vec{0}$, that set is linearly dependent.*

### Example 2 Polynomials
$P$ [[Vector Space|vector space]] of polynomials of degree $\le n$ 
$p_1(t)=1,\:p_2(t)=t,\:p_3(t)=7-5t$

as $p_3=7p_1-5p_2$, $P$ is linearly dependent. 

## Theorem Forced Linear Dependence
$S=\set{\vec{v_1},\vec{v_2},...,\vec{v_p}}$  vectors in $\mathbb{R}^n$
is $p>n$, the set is linearly dependent