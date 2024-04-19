**For 2x2**
$$A=\begin{bmatrix}a & b \\ c & d\end{bmatrix}$$
Determinant of A $$\det{A}=\begin{vmatrix}a & b \\ c & d\end{vmatrix}=ab-cd$$
**For 3x3**
![[_obsidian/drawings/Linear Algebra 2024-02-12 08.41.06.excalidraw]]
$$\begin{vmatrix}a & b & c \\ d & e & f \\ g & h & k\end{vmatrix}=aek+bfg+cdh-gec-hfa-kdb$$

**For $n\times n$**
$$A\in n\times n\:\mathrm{matrix}$$
$A_{ij}$ is a $(n-1\times n-1)$ matrix obtained from $A$ by removing row $i$ and column $d$
$$\det{A}=(-1)^{k+1}\cdot\det{A_{k1}}+(-1)^{k+2}\cdot\det{A_{k2}}+...+(-1)^{k+n})\cdot\det{A_{kn}}$$

_Note: The end result is the same, no matter what row (or column) you choose_

### Readable Version

1. Take any row to expand by.
2. For each cell from left to right on the chosen row
   1. remove the column and row that the cell belongs to
   2. compute the determinant of the resulting matrix
   3. multiply by the original cell value
   4. add if this is your 1st, 3rd, 5th... or subtract if its the 2nd, 4th, 6th..

### Example

$$A=\begin{vmatrix}1 & 2 & 0 \\ -2 & 4 & 5 \\ 2 & 2 & 1\end{vmatrix}$$
_Note: as any row can be chosen, it is most beneficial to choose a row with as many zeros as possible_

Using the first row ($k=1$):
$$\det{A}=1\cdot\begin{vmatrix}4 & 5 \\ 2 & 1\end{vmatrix}-2\cdot\begin{vmatrix}-2 & 5 \\ 2 & 1\end{vmatrix}+0\cdot\begin{vmatrix}-2 & 4 \\ 2 & 2\end{vmatrix}=18$$

Using the second row ($k=2$):
$$\det{A}=-(-2)\cdot\begin{vmatrix}2 & 0 \\ 2 & 1\end{vmatrix}+4\begin{vmatrix}1 & 0 \\ 2 & 1\end{vmatrix}-5\cdot\begin{vmatrix}1 & 2 \\ 2 & 2\end{vmatrix}=18$$
Note the leading negative sign as $k$ is odd

### Cofactor Expansion

$C_{ij}$ is known as the [[Matrix Cofactor|Cofactor]].
$$\det{A}=a_{k1}c_{k1}+a_{k2}c_{k2}+...+a_{kn}c_{kn}$$

### Special Cases

**A triangular matrix:**
$$\begin{bmatrix}2 & -1 & 3 & 5 \\ 0 & 4 & 1 & 7 \\ 0 & 0 & 3 & 9 \\ 0 & 0 & 0 & 1\end{bmatrix}$$
All elements below the main diagonal is $0$.

or $$\begin{bmatrix}3 & 0 & 0 & 0 \\ 2 & 1 & 0 & 0 \\ -1 & 2 & 4 & 0 \\ 3 & 2 & 7 & 2\end{bmatrix}$$ All elements above main diagonal is $0$.

The determinant of a triangle matrix is the product of the elements in the main diagonal.
$$2\cdot4\cdot3\cdot1,\:3\cdot1\cdot4\cdot2$$

## Properties

Def: $A\in n\times n$ matrix

**Row Operations**

- If $B$ is obtained from $A$ by adding a multiple of a row to another row, then $\det{A}=\det{B}$. Example: $$\det{A}=\begin{vmatrix}1 & 1 & 1 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{vmatrix}=\det{I_3}=1$$
- If $B$ is obtained from $A$ by switching 2 rows, then $\det{B}=-\det{A}$. Example: $$\det{A}=\begin{vmatrix}1 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & 1 & 0\end{vmatrix}=-\det{I_3}=-1$$
- If $B$ is obtained from $A$ by multiplying a row by a constant $k$, then $\det{B}=k\cdot\det{A}$. Example: $$\det{A}=\begin{vmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 3\end{vmatrix}=3\cdot\det{I_3}=3$$ _Note: due to the above rule, multiplying a matrix with $n$ rows with a scalar $k$ has the effect of multiplying its determinant by $k^n$_

**Transpose**
[[Matrix Transpose|transposing]] a matrix $A$ does not change its determinant.
$$\det{A}=a\Rightarrow\det{A^T}=a$$

**Multiplication**
[[Matrix Operations#Matrix Multiplication|Multiplication]] two matrices has the effect of multiplying its determinants.
$$\det{A}=a,\:\det{B}=b\Rightarrow\det{A\cdot B=ab}$$

**Inverse**
[[Matrix Inverse|inverting]] a matrix has the effect of taking the reciprocal of its determinant.
$$\det{A}=a\Rightarrow\det{A^{-1}}=\frac{1}{a}$$

_Note: there is no theorem for the determinant of the addition or subtraction of matrices_
