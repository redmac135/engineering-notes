## Elementary Row Operations

1. Replace one row with **sum** of **itself** and **another row**:
   ex. $R_1+R_{2}\to R_1$
2. Interchange 2 rows:
   ex. $R_{1}\to R_2,R_{2}\to R_1$
3. Multiply a row by a non-zero constant
   ex. $kR_{1}\to R_1,k\ne0$

Matrices obtained from these row operations are called **Row Equivalent**

Row equivalent augmented matrices contain the same solution set.

## Row Echelon Forms

A matrix is in **Row Echelon Form (REF)** if:

- all zero rows are at the bottom
- first non-zero element of a row is to the right of the first non-zero element of the row above it
- all entries below a first non-zero element of a row are zero
  ex. $$\begin{bmatrix}2 & 4 & -1 & 5 \\ 0 & 2 & 7 & -1 \\ 0 & 0 & 0 & 4\end{bmatrix},\mathrm{is\:in\:REF}$$
  A matrix that is **REF** is in **reduced row Echelon Form (RREF)** if:
- all leading non-zero elements is a 1
  _note: must also satisfy REF requirements_
  ex. $$\begin{bmatrix}1 & 0 & 0 & 2 & 0 & 7 \\ 0 & 1 & 0 & 3 & 0 & -4 \\ 0 & 0 & 1 & -1 & 0 & 0 \\ 0 & 0 & 0 & 0 & 1 & 9\end{bmatrix}$$

## Resources

[Row Reduction (gatech.edu)](https://textbooks.math.gatech.edu/ila/row-reduction.html)
