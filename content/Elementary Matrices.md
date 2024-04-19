## Definition

An elementary matrix $E$ is a matrix obtained from performing **one** [[Matrix Row Reduction#Elementary Row Operations|elementary row operation]] on an [[Identity Matrix|identity matrix]].

### Example

$$E=\begin{bmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 4\end{bmatrix}$$ _multiplying row 3 by 4_
$$E=\begin{bmatrix}1 & 0 & -2 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$$_adding $-2R_3$ to $R_1$_

The [[Matrix Inverse|inverse]] of an elementary matrix is the opposite row operation.

## Applications

$E\cdot A$ = the result of performing the same [[Matrix Row Reduction#Elementary Row Operations|elementary row operation]] on $A$

To performing several row operations, resulting with a matrix $A_r$: $$A_r=E_r\cdot...\cdot E_3\cdot{E_2}\cdot{E_1}\cdot{A}$$ _note the reverse order_

**if multiplied on right**
then the operation is instead performed on the column.

e.g. $$E=\begin{bmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 3\end{bmatrix}$$
$E\cdot A$ multiplies row 3 by 3.
$A\cdot E$ multiplies column 3 by 3.

### Example

$$E=\begin{bmatrix}1 & 0 & -2 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$$
$$A=\begin{bmatrix}1 & 0 & -1 & 4 \\ 2 & -1 & 1 & 0 \\ 0 & 1 & 3 & 1\end{bmatrix}$$
$$E\cdot A=\begin{bmatrix}1 & -2 & -7 & 2 \\ 2 & -1 & 1 & 0 \\ 0 & 1 & 3 & 1\end{bmatrix}$$

## Properties

An elementary matrix is always [[Matrix Inverse|invertible]] as it is row equivalent to the [[Identity Matrix]].
