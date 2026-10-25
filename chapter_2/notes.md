# Chapter 2

## 2.1 Vectors and Linear Equations

---

Page 42

1. The **column picture of** $A_x = b$: a combination of $n$ columns of $A$
   produces the vector $b$.

2. This is a vector equation $Ax = x_1a_1 + \cdots + x_na_n = b$: the columns of
   $A$ are $a_1, a_2, \dots, a_n$.

3. When $b = \mathbf{0}$, a combination $Ax$ of the columns is _zero_: one
   possibility is $x = (0, \dots, 0)$.

4. The **row picture of** $Ax = : m$ equations from $m$ rows gives $m$ planes
   meeting at $x$.

5. A dot product gives the equation of each plane:
   $(\textbf{row } 1) \cdot x = b_1, \dots, (\textbf{row } m) \cdot x = b_m$.

6. When $b = \mathbf{0}$, all the planes $\textbf{row } i \cdot x = 0$ go
   through the center point $x = (0, 0, \dots, 0)$.

---

Page 42

(1)

**Two equations Two unknowns**

$$
x - 2y = 1 \\
3x + 2y = 11
$$

---

Page 44

**Linear combination**

$$ 3\begin{bmatrix}{}1\\3\end{bmatrix} + \begin{bmatrix}{}-2\\2\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

---

Page 44

**Matrix equation $Ax = b$**

$$
\left[\begin{array}{cc}
1 & -2 \\
3 & 2 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}1\\11\end{bmatrix}
$$

---

Page 45

**Dot products with rows Combinations of columns**

$$
Ax = b \text{ is } \quad
\left[\begin{array}{cc}
1 & -2 \\
3 & 2 \\
\end{array}\right]
\begin{bmatrix}{}3\\1\end{bmatrix} =
\begin{bmatrix}{}1\\11\end{bmatrix}
$$

---

Page 48

$$
I =
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

always yields the multiplication $Ix = x$.

---

## 2.2 The Idea of Elimination

---

Page 57

1. For $m = n = 3$, there are three equations $Ax = b$ and three unknowns
   $x_1, x_2, x_3$.

2. The first two equations are $a_{11}x_1 + \cdots = b_1$ and
   $a_{21}x_1 + \cdots = b_2$.

3. Multiply the first equation by $\dfrac{a_{21}}{a_{11}}$ and subtract from the
   second: then $x_1$ **is eliminated**.

4. The corner entry $a_{11}$ is the first "pivot" and the ratio
   $\dfrac{a_{21}}{a_{11}}$ is the first "multiplier."

5. Eliminate $x_1$ from every remaining equation $i$ by subtracting
   $\dfrac{a_{i1}}{a_{11}}$ times the first equation.

6. Now the last $n - 1$ equations contain $n - 1$ unknowns $x_2, \dots, x_n$.
   _Repeat to eliminate $x_2$_.

7. Elimination breaks down if zero appears in the pivot. Exchanging two
   equations may save it.

---

Page 58

$$ \textit{Pivot } = \textit{ first nonzero in the row that does the elimination} $$

$$ \textit{Multiplier } = \textit{(entry to eliminate) divided by (pivot)} = \frac{3}{4} $$

---

Page 62

**REVIEW OF THE KEY IDEAS**

1. A linear system ($Ax = b$) becomes **upper triangular** ($Ux = c$) after
   elimination.

2. We subtract $\ell_{ij}$ times equation $j$ from equation $i$, to make the
   $(i, j)$ entry zero.

3. The **multiplier** is
   $\ell_{ij} = \dfrac{\text{entry to eliminate row } i}{\text{pivot in row }j}$.
   **Pivots** can not be zero!

4. When zero is in the pivot position, **exchange rows** if there is a nonzero
   below it.

5. The upper triangular $Ux = c$ is solved by **back substitution** (starting at
   the bottom).

6. When **breakdown** is permanent, $Ax = b$ has no solution or infinitely many.

---

## 2.3 Elimination Using Matrices

---

Page 69

1. The first step multiplies the equations $Ax = b$ by a matrix $E_{21}$ to
   produce $E_{21}Ax = E_{21}b$.

2. That matrix $E_{21}A$ has a zero in row 2, column 1 because $x_1$ is
   eliminated from equation 2.

3. $E_{21}$ is the **identity matrix** (diagonal of $1$'s) minus the multiplier
   $\dfrac{a_{21}}{a_{11}}$ in row 2, column 1.

4. Matrix-matrix multiplication is $n$ matrix-vector multiplications:
   $EA = \left[Ea_1 \dots Ea_n\right]$.

5. We must also multiply $Eb$! So $E$ is multiplying the **augmented matrix**
   $[Ab] = [a_1 \dots a_nb]$.

6. Elimination multiplies $Ax = b$ by $E_{21}, E_{32}, \dots, E_{n1}$, then
   $E_{32}, E_{42}, \dots, E_{n2}$, and onward.

7. The **row exchange matrix** is not $E_{ij}$ but $P_{ij}$. To find $P_{ij}$,
   exchange rows $i$ and $j$ of $I$.

---

Page 71

The **identity matrix** has $1$'s on the diagonal and otherwise $0$'s. Then
$Ib = b$ for all $b$. The **elementary matrix or elimination matrix** $E_{ij}$
has the extra nonzero entry - $\ell$ in the $i, j$ position. Then $E_{ij}$
subtracts a multiple $\ell$ of row $j$ from row $i$.

---

Page 72

**Associative law is true**

$$ A(BC) = (AB)C $$

**Commutative law is false**

Often

$$ AB \neq BA $$

---

Page 73

**Matrix multiplication**

$$ AB =
A\left[\begin{array}{ccc}
b_1 & b_2 & b_3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
Ab_1 & Ab_2 & Ab_3 \\
\end{array}\right]
$$

---

Page 74

**Row Exchange Matrix**

$P_{ij}$ is the identity matrix with rows $i$ and $j$ reversed. When this
"**permutation matrix**" $P_{ij}$ multiplies a matrix, it exchanges rows $i$ and
$j$.

---

Page 75

**REVIEW OF THE KEY IDEAS**

1. $Ax = x_1$ times column $1 + \cdots + x_n$ times column $n$. And
   $(Ax)_i = \sum_{j = 1}^{n}{a_{ij}x_j}$.

2. Identity matrix $= I$, elimination matrix $= E_{ij}$ using $\ell_{ij}$,
   exchange matrix $= P_{ij}$.

3. Multiplying $Ax = b$ by $E_{21}$ subtracts a multiple $\ell_{21}$ of equation
   1 from equation 2. The number $-\ell_{21}$ is the $(2, 1)$ entry of the
   elimination matrix $E_{21}$.

4. For the augmented matrix
   $\left[\begin{array}{cc} A & b\\ \end{array}\right]$, that elimination step
   gives $\left[\begin{array}{cc} E_{21}A & E_{21}b\\ \end{array}\right]$.

5. When $A$ multiplies any matrix $B$, it multiplies each column of $B$
   separately.

---

Page 81

## 2.4 Rules for Matrix Operations

---

Page 81

1. Matrices $A$ with $n$ columns multiply matrices $B$ with $n$ rows:
   $\boxed{A_{m \times n}B_{n \times p} = C_{m \times p}}$.

2. Each entry in $AB = C$ is a dot product:
   $C_{ij} = (\text{row } i \text{ of } A) \cdot (\text{column } j \text{ of } B)$.

3. This rule is chosen so that **$AB$ times $C$ equals $A$ times $BC$**. And
   $(AB)x = A(Bx)$.

4. More ways to compute $AB$: ($A$ times columns of $B$)(rows of $A$ times
   $B$)(_columns times rows_).

5. It is not usually true that $AB = BA$. In most cases _$A$ doesn't commute
   with $B$._

6. Matrices can be multiplied by _blocks:_
   $A = \left[\begin{array}{cc} A_1 & A_2 \\\end{array}\right]$ times
   $B = \begin{bmatrix}{}B_1\\B_2\end{bmatrix}$ is $A_1B_1 + A_2B_2$.

---

Page 81

**Fundamental Law of Matrix Multiplication**

$AB$ times $C$ equals $A$ times $BC$.

---

Page 85

**Block multiplication**

If blocks of $A$ can multiply blocks of $B$, then block multiplication of $AB$
is allowed. Cuts between columns of $A$ match cuts between rows of $B$.

$$
\left[\begin{array}{cc}
A_{11} & A_{12}\\
A_{21} & A_{22}\\
\end{array}\right]
\begin{bmatrix}{}B_{11}\\B_{12}\end{bmatrix} =
\begin{bmatrix}{}A_{11}B_{11} + A_{12}B_{21}\\A_{21}B{11} + A_{22}B_{21}\end{bmatrix}
$$

---

Page 87

**REVIEW OF THE KEY IDEAS**

1. The $(i, j)$ entry of $AB$ is
   $(\text{row } i \text{ of } A) \cdot (\text{column } j \text{ of } B)$.

2. An $m$ by $n$ matrix times an $n$ by $p$ matrix uses $mnp$ separate
   multiplications.

3. $A$ times $BC$ equals $AB$ times $C$ (surprisingly important).

4. $AB$ is also the sum of these $n$ matrices:
   $(\text{column } j \text{ of } A) \text{ times } (\text{row } j \text{ of } B)$.

5. Block multiplication is allowed when the block shapes match correctly.

6. Block elimination produces the _Schur complement_ $D - CA^{-1}B$.

---

Page 94

## 2.5 Inverse Matrices

---

Page 94

1. If the square matrix $A$ has an inverse, then both $A^{-1}A = I$ and
   $AA^{-1} = I$.

2. The _algorithm_ to test invertibility is elimination: $A$ must have $n$
   (nonzero) pivots.

3. The _algebra_ test for invertibility is the determinant of $A$: $\det A$ must
   not be zero.

4. The _equation_ that tests for invertibility is $Ax = \mathbf{0}$:
   $x = \mathbf{0}$ **must be the only solution.**

5. If $A$ and $B$ (same size) are invertible then so is $AB$:
   $\boxed{(AB)^{-1} = B^{-1}A^{-1}}$.

6. $AA^{-1} = I$ is $n$ equations for $n$ columns of $A^{-1}$. Gauss-Jordan
   eliminates $\left[\begin{array}{cc} A & I \\\end{array}\right]$ to
   $\left[\begin{array}{cc} I & A^{-1} \\\end{array}\right]$.

7. The last page of the book gives 14 equivalent conditions for a square $A$ to
   be invertible.

---

Page 94

**Definition**

The matrix $A$ is **invertible** if there exists a matrix $A^{-1}$ that
"inverts" $A$:

**Two-sided inverse:**

$$ A^{-1}A = I \text{ and } AA^{-1} = I $$

---

Page 95

If $A$ and $B$ are invertible then so is $AB$. The inverse of a product $AB$ is

$$ (AB)^{-1} = B^{-1}A^{-1} $$

---

Page 101

**REVIEW OF THE KEY IDEAS**

1. The inverse matrix gives $AA^{-1} = I$ and $A^{-1}A = I$.

2. $A$ is invertible if and only if it has $n$ pivots (row exchanges allowed).

3. _Important_. If $Ax = \mathbf{0}$ for a nonzero vector $x$, then $A$ has no
   inverse.

4. The inverse of $AB$ is the reverse product $B^{-1}A^{-1}$. And
   $(ABC)^{-1} = C^{-1}B^{-1}A^{-1}$.

5. The Gauss-Jordan method solves $AA^{-1} = I$ to find the $n$ columns of
   $A^{-1}$. The augmented matrix
   $\left[\begin{array}{cc}A & I \\\end{array}\right]$ is row-reduced to
   $\left[\begin{array}{cc}I & A^{-1}\\\end{array}\right]$.

6. Diagonally dominant matrices are invertible. Each $|a_{ii}|$ dominates its
   row.

---

## 2.6 Elimination = Factorization: $A = LU$

---

Page 108

1. Each elimination step $E_{ij}$ is inverted by $L_{ij}$. Off the main diagonal
   change $-\ell_{ij}$ to $+\ell_{ij}$.

2. The whole forward elimination process (with no row exchanges) is inverted by
   $L$:

$$ L = (L_{21}L_{31} \dots L_{n1})(L_{32} \dots L_{n2})(L_{43} \dots L_{n3})\dots(L_{n}L_{n - 1}) $$

3. The product matrix $L$ is still lower triangular. **Every mutiplier
   $\ell_{ij}$ is in row $i$, column $j$**.

4. The original $A$ is recovered from $U$ by $A = LU =$ (lower triangular)(upper
   triangular).

5. Elimination on $Ax = b$ reaches $Ux = c$. Then back-substitution solves
   $Ux = c$.

6. Solving a triangular system takes $\dfrac{n^2}{2}$ multiply-subtracts.
   Elimination to find $U$ takes $\dfrac{n^3}{3}$.

---

Page 109

$$ A = LU $$

**This is elimination without row exchanges.** The upper triangular $U$ has the
pivots on its diagonal. The lower triangular $L$ has all $1$'s on its diagonal.
**The multipliers $\ell_{ij}$ are below the diagonal of $L$.**

---

Page 113

**REVIEW OF THE KEY IDEAS**

1. Gaussian elimination (with no row exchanges) factors $A$ into $L$ times $U$.

2. The lower triangular $L$ contains the numbers $\ell_{ij}$ that multiply pivot
   rows, going from $A$ to $U$. The product $LU$ adds those rows back to recover
   $A$.

3. On the right side we solve $Lc = b$ (forward) and $Ux = c$ (backward).

4. _Factor:_ There are $\dfrac{1}{3}(n^3 - n)$ multiplications and subtractions
   on the left side.

5. _Solve:_ There are $n^2$ multiplications and subtractions on the right side.

6. For a band matrix, change $\dfrac{1}{3}n^3$ to $nw^2$ and change $n^2$ to
   $2wn$.

---

Page 120

## 2.7 Transposes and Permutations

---

Page 120

1. The transposes of $Ax$ and $AB$ and $A^{-1}$ are
   $x^{\mathbf{T}}A^{\mathbf{T}}$ and $B^{\mathbf{T}}A^{\mathbf{T}}$ and
   $(A^{\mathbf{T}})^{-1}$.

2. The dot product (inner product) is $x \cdot y = x^{\mathbf{T}}y$. This is
   $(1 \times n)(n \times 1) = (1 \times 1)$. The outer product is
   $xy^{\mathbf{T}} =$ column times row
   $= (n \times 1)(1 \times n) = n \times n$ matrix.

3. The idea behind $A^{\mathbf{T}}$ is that $Ax \cdot y$ equals
   $x \cdot A^{\mathbf{T}}y$ because
   $(Ax)^{\mathbf{T}}y = x^{\mathbf{T}}A^{\mathbf{T}}y = x^{\mathbf{T}}(A^{\mathbf{T}}y)$.

4. A **symmetric matrix** has $S^{\mathbf{T}} = S$ (and the product
   $A^{\mathbf{T}}A$ is always symmetric).

5. An **orthogonal matrix** has $Q^{\mathbf{T}} = Q^{-1}$. The columns of $Q$
   are orthogonal unit vectors.

6. A **permutation matrix** $P$ has the same rows as $I$ (in any order). There
   are $n!$ different orders.

7. Then $Px$ puts the components $x_1, x_2, \dots, x_n$ in that new order. And
   $P^{\mathbf{T}}$ equals $P^{-1}$.

---

Page 122

**Definition**

A **symmetric matrix has $S^{\mathbf{T}} = S$**. This means that
$s_{ji} = s_{ij}$.

---

Page 124

**Definition**

A **permutation matrix $P$ has the rows of the identity $I$ in any order.**

---

Page 126

**REVIEW OF THE KEY IDEAS**

1. The transpose puts the rows of $A$ into the columns of $A^{\mathbf{T}}$. Then
   $(A^{\mathbf{T}})_{ij} = A_{ji}$.

2. The transpose of $AB$ is $B^{\mathbf{T}}A^{\mathbf{T}}$. The transpose of
   $A^{-1}$ is the inverse of $A^{\mathbf{T}}$.

3. The dot product is $x \cdot y = x^{\mathbf{T}}y$. Then $(Ax)^{\mathbf{T}}y$
   equals the dot product $x^{\mathbf{T}}(A^{\mathbf{T}}y)$.

4. When $S$ is symmetric ($S^{\mathbf{T}} = S$), its $LDU$ factorization is
   symmetric: $S = LDL^{\mathbf{T}}$.

5. A permutation matrix $P$ has a $1$ in each row and column, and
   $P^{\mathbf{T}} = P^{-1}$.

6. There are $n!$ permutation matrices of size $n$. _Half even, half odd._

7. If $A$ is invertible then a permutation $P$ will reorder its rows for
   $PA = LU$.
