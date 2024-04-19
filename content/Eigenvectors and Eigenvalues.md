## Definition
An eigenvector of $A\in n\times n$ matrix is a vector $\vec{v}\in\mathbb{R}^n$ such that $A\vec{v}=\lambda\vec{v},\:\lambda\in\mathbb{R}^n$. Where $\lambda$ is the eigenvalues.

The eigenvectors corresponding to an eigenvalue $\lambda$ form a [[Subspace]] called the eigenspace for $\lambda$. 

In order for a value $\lambda$ to be called an eigenvalue, there must be some vector $\vec{v}$ that is not the [[Zero Vector]]. But as there is more than the trivial solution, there must be an infinite number of solutions as proven in [[Matrix Equation#Homogenous System|homogenous systems]].

In general,
$$A\vec{x}=\lambda\vec{x}$$
$$A\vec{x}-\lambda\vec{x}=0\Rightarrow(A-\lambda I)\vec{x}=0$$
Multiplying $\lambda$ by the [[Identity Matrix]] allows for subtracting with the matrix $A$. 

This equation is the precursor to the [[Matrix Characteristic Equation]]

### Example
$$A=\begin{bmatrix}1 & 6 \\ 5 & 2\end{bmatrix},\:\vec{x}=\begin{bmatrix}x_1 \\ x_2\end{bmatrix},\:A\vec{x}=7\vec{x}$$
Is 7 an eigenvalue of $A$? Or: is there a vector $\vec{x}$ such that the equation is satisfied?
$$\begin{bmatrix}1 & 6 \\ 5 & 2\end{bmatrix}\begin{bmatrix}x_1 \\ x_2\end{bmatrix}=\begin{bmatrix}7x_1 \\ 7x_2\end{bmatrix}$$
$$
\begin{cases}
x_1+6x_2=7x_1 \\
5x_1+2x_2=7x_2
\end{cases}\Rightarrow\begin{cases}
-6x_1+6x_2=0 \\
5x_1-5x_2=0
\end{cases}
$$
constructing an [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]]: $$\begin{bmatrix}-6 & 6 & 0 \\ 5 & -5 & 0\end{bmatrix}\rightarrow\begin{bmatrix}1 & -1 & 0 \\ 0 & 0 & 0\end{bmatrix}$$ let $x_2=s$, then: $x_1=s$ and: $$\vec{x}=\begin{bmatrix}s \\ s\end{bmatrix}=s\cdot\begin{bmatrix}1 \\ 1\end{bmatrix},\:s\in\mathbb{R}$$
Therefore, any scalar multiple of $\begin{bmatrix}1 \\ 1\end{bmatrix}$ is an eigenvector for the eigenvalue $\lambda=7$.

### Example
let:
$$A=\begin{bmatrix}3 & -2 \\ 1 & 0\end{bmatrix},\:\vec{v}=\begin{bmatrix}2 \\ 1\end{bmatrix}$$
$$A\cdot\vec{v}=\begin{bmatrix}4 \\ 2\end{bmatrix}=2\cdot\vec{v}$$
This result is specific to this vector.

Contrary, let: $$\vec{u}=\begin{bmatrix}-1 \\ 1\end{bmatrix}\Rightarrow A\cdot\vec{u}=\begin{bmatrix}-5 \\ -1\end{bmatrix}$$ which is not a multiple of $\vec{u}$

### Example Eigenspace
$$A=\begin{bmatrix}4 & -1 & 6 \\ 2 & 1 & 6 \\ 2 & -1 & 8\end{bmatrix}$$
given $\lambda=2$ is an eigenvalue of $A$, find a basis for the corresponding eigenspace.
$$(A-\lambda I)\vec{x}=0\Rightarrow(A-2I)\vec{x}=0$$
$$A-2I=A-\begin{bmatrix}2 & 0 & 0 \\ 0 & 2 & 0 \\ 0 & 0 & 2\end{bmatrix}=\begin{bmatrix}2 & -1 & 6 \\ 2 & -1 & 6 \\ 2 & -1 & 6\end{bmatrix}$$
*wow! All rows are the same, who could've predicted this !!*
$$\begin{bmatrix}2 & -1 & 6 \\ 2 & -1 & 6 \\ 2 & -1 & 6\end{bmatrix}\begin{bmatrix}x_1 \\ x_2 \\ x_3\end{bmatrix}=\begin{bmatrix}0 \\ 0 \\ 0\end{bmatrix}$$
using this equation, we can construct the [[Linear Algebra#Augmented Matrix of Coefficients|augmented matrix]] and [[Matrix Row Reduction|row reduce]].
$$\begin{bmatrix}2 & -1 & 6 & 0 \\ 2 & -1 & 6 & 0 \\ 2 & -1 & 6 & 0\end{bmatrix}\rightarrow\begin{bmatrix} 1 & \frac{-1}{2} & 3 & 0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0\end{bmatrix}$$
This matrix has 2 free variables and only 1 [[Pivot Position]]. Now, we let: $x_2=s,\:x_3=t$ and,
$$x_{1}=\frac{1}{2}s-3t\Rightarrow\begin{bmatrix}x_1 \\ x_2 \\ x_3\end{bmatrix}=\begin{bmatrix} \frac{1}{2} \\ 1 \\ 0\end{bmatrix}s+\begin{bmatrix}-3 \\ 0 \\ 1\end{bmatrix}t$$
Therefore, $$\set{\begin{bmatrix} \frac{1}{2} \\ 1 \\ 0\end{bmatrix},\begin{bmatrix}-3 \\ 0 \\ 1\end{bmatrix}}$$
form a basis for the eigenspace of $A$ for $\lambda=2$.

## Special Cases
**$\lambda$ = 0**
$(A-0I)\vec{x}=0\Rightarrow A\vec{x}=0$
0 is an eigenvalue of $A$ if $A\vec{x}=0$ has non-zero solutions. 

**Linear Independence**
Vectors $\vec{v_i}$ corresponding to eigenvalues $\lambda_i$. For any set of vectors, if their eigenvalues are different, they are [[Linear Independence|linearly independent]]. Mathematically: $$S=\set{\vec{v_1},\vec{v_2},...,\vec{v_{n}}},\mathrm{if}\:\lambda_1\ne\lambda_2\ne...\ne\lambda_n$$ then the set $S$ is linearly independent.

**Triangular Matrix**
$$A=\begin{bmatrix}2 & 1 & -3  \\ 0 & 3 & 4 \\ 0 & 0 & 5\end{bmatrix}$$
then the eigenvalues are the elements on the main diagonal: $\lambda=2,3,5$

**[[Similar Matrix]]**
If two matrices are similar, then they have the same [[#Characteristic Equation|characteristic equation]] $\Rightarrow$ they have the same eigenvalues. 