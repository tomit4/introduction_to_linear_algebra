Page 134

## 3.1 Spaces of Vectors

---

Page 134

1. The standard $n$-dimensional space $\mathbf{R}^n$ contains all real column
   vectors with $n$ components.

2. If $v$ and $w$ are in a **vector space** $S$, every combination $cv + dw$
   must be in $S$.

3. The "vectors" in $S$ can be matrices or functions of $x$. The $1$-point space
   $\mathbf{Z}$ consists of $x = \mathbf{0}$.

4. A **subspace** of $\mathbf{R}^n$ is a vector space inside $\mathbf{R}^n$.
   _Example:_ The line $y = 3x$ inside $\mathbf{R}^2$.

5. The **column space** of $A$ contains all combinations of the columns of $A$:
   a subspace of $\mathbf{R}^m$.

6. The column space contains all the vectors $Ax$. So $Ax = b$ is solvable when
   $b$ is in $C(A)$.

---

Page 134

**DEFINITION**

The space $\mathbf{R}^n$ consists of all column vectors $b$ with $n$ components.

---

Page 135

$\mathbf{M}$ The vector space of _all real $2$ by $2$ matrices_.

$\mathbf{F}$ The vector space of _all real functions $f(x)$_

$\mathbf{Z}$ The vector space that consists only of a _zero vector_.

---

Page 136

**DEFINITION**

A _subspace_ of a vector space is a set of vectors (including $\mathbf{0}$) that
satisfies two requirements: If $v$ and $w$ are vectors in the subspace and $c$
is any scalar, then

i. $v + w$ is in the subspace

ii. $cv$ is in the subspace

---

Page 137

A subspace containing $v$ and $w$ must contain all linear combinations
$cv + dw$.

---

Page 138

**DEFINITION**

The _column space_ consists of _all linear combinations of the columns_. The
combinations are all possible vectors $Ax$. They fill the column space $C(A)$.

---

Page 138

The system $Ax = b$ is solvable if and only if $b$ is in the column space of
$A$.

---

Page 140

**Example 5**

Describe the column spaces (they are subspaces of $\mathbf{R}^2$) for

$$ I =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] \quad \text{ and } \quad
A =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right] \quad \text{ and } \quad
B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 4 \\
\end{array}\right]
$$

**Solution**

The column space of $I$ is the _whole space_ $\mathbf{R}^2$. Every vector is a
combination of the columns of $I$. In vector space language, $C(I)$ is
$\mathbf{R}^2$.

The column space of $A$ is only a line. The second column $(2, 4)$ is a multiple
of the first column $(1, 2)$. Those vectors are different, but our eye is on
vector _spaces_. The column space contains $(1, 2)$ and $(2, 4)$ and all other
vectors $(c, 2c)$ along that line. The equation $Ax = b$ is only solvable when
$b$ is on the line.

For the third matrix (with three columns) the column space $C(B)$ is all of
$\mathbf{R}^2$. Every $b$ is attainable. The vector $b = (5, 4)$ is column 2
plus column 3, so another possible $x$ is $(2, 0, 1)$. This matrix has the same
column space as $I$ - any $b$ is allowed. But now $x$ has extra components and
there are more solutions - more combinations that give $b$.

---

Page 140

**REVIEW OF THE KEY IDEAS**

1. $\mathbf{R}^n$ contains all column vectors with $n$ real components.

2. $\mathbf{M}$ (2 by 2 matrices) and $\mathbf{F}$ (functions) and $\mathbf{Z}$
   (zero vector alone) are vector spaces.

3. A subspace containing $v$ and $w$ must contain all their combinations
   $cv + dw$.

4. The combinations of the columns of $A$ form the _column space_ $C(A)$. Then
   the column space is "spanned" by the columns.

5. $Ax = b$ has a solution exactly when $b$ is the column space of $A$.

$$ C(A) = \textbf{all combinations of the columns } = \textbf{ all vectors } Ax $$

---

Page 146

## 3.2 The Nullspace of $A$: Solving $Ax = 0$ and $Rx = 0$

---

Page 146

1. The **nullspace** $N(A)$ in $\R^n$ contains all solutions $x$ to
   $Ax = \mathbf{0}$. This includes $x = \mathbf{0}$.

2. Elimination (from $A$ to $U$ to $R$) does not change the nullspace:
   $N(A) = N(U) = N(R)$.

3. The **reduced row echelon form** $R = \text{rref}(A)$ has all pivots $= 1$,
   with zeros above and below.

4. If column $j$ of $R$ is free (no pivot), there is a "_special solution_" to
   $Ax = \mathbf{0}$ with $x_j = 1$.

5. Number of pivots = number of nonzero rows in $R = \textbf{rank} r$. There are
   $n - r$ free columns.

6. Every matrix with $m < n$ has nonzero solutions to $Ax = \mathbf{0}$ in its
   nullspace.

---

Page 146

The nullspace $N(A)$ consists of all solutions to $Ax = \mathbf{0}$. These
vectors $x$ are in $\R^n$.

---

Page 150

**DEFINITION OF RANK**

The rank of $A$ is the number of pivots. This number is $r$.

---

Page 152

**REVIEW OF THE KEY IDEAS**

1. The nullspace $N(A)$ is a subspace of $\R^n$. It contains all solutions to
   $Ax = \mathbf{0}$.

2. Elimination on $A$ produces a row reduced $R$ with pivot columns and free
   columns.

3. Every free column leads to a special solution. That free variable is $1$, the
   others are $0$.

4. The _rank_ $r$ of $A$ is the number of pivots. All pivots are $1$'s in
   $R = \text{rref}(A)$.

5. The complete solution to $Ax = \mathbf{0}$ is a combination of the $n -
   special solutions.

6. $A$ always has a free column if $n > m$, giving a _nonzesro solution_ to
   $Ax = \mathbf{0}$.

---

Page 161

## The Complete Solution to $Ax = b$

---

Page 161

1. **Complete Solution** to $Ax = b$:
   $x = (\text{one particular solution } x_p) + (\text{any } x_n \text{ in the nullspace})$.

2. Elimination on $\begin{bmatrix}{}A\\b\end{bmatrix}$ leads to
   $\begin{bmatrix}{}R\\d\end{bmatrix}$. Then $Ax = b$ is equivalent to
   $Rx = d$.

3. $Ax = b$ and $Rx = d$ are solvable only when all zero rows of $R$ have zeros
   in $d$.

4. When $Rx = d$ is solvable, one very particular solution $x_p$ has all free
   variables equal to zero.

5. $A$ has **full column rank** $r = n$ when its nullspace $N(A) =$ zero vector:
   _no free variables_.

6. $A$ has **full row rank** $r = m$ when its column space $C(A)$ is
   $\R^{m}: Ax = b$ is always solvable.

7. The four cases are $r = m = n$ ($A$ is invertible) and $r = m < n$ (every
   $Ax = b$ is solvable) and $r = n < m$ ($Ax = b$ has $1$ or $0$ solutions) and
   $r < m, r < n$ ($0$ or $\infty$ solutions).

---

Page 164

Every matrix $A$ with $\textbf{full column rank} (r = n)$ has all these
properties:

1. All columns of $A$ are pivot columns.

2. There are no free variables or special solutions.

3. The nullspace $N(A)$ contains only the zero vector $x = \mathbf{0}$.

4. If $Ax = b$ has a solution (it might not) then it has only _one solution_.

---

Page 165

Every matrix $A$ with $\textbf{full row rank} (r = m)$ has all these properties:

1. All rows have pivots, and $R$ **has no zero rows.**

2. $Ax = b$ has a **solution for every right side** $b$.

3. The column space is the whole space $\R^m$.

4. There are $n - r = n - m$ special solutions in the nullspace of $A$.

---

Page 166

**The four possibilities for linear equations depend on the rank $r$**

$$ \begin{array}{l}
r = m \text{ and } r = n \quad \textit{Square and invertible} \quad Ax = b
\quad \text{has } 1 \text{ solution} \\ r = m \text{ and } r < n \quad
\textit{Short and wide} \quad Ax = b \quad \text{has } \infty \text{ solution} \\
r < m \text{ and } r = n \quad \textit{Tall and thin} \quad Ax = b \quad
\text{has } 0 \text{ or } 1 \text{ solution} \\
r < m \text{ and } r < n \quad \textit{Not full rank} \quad Ax = b \quad
\text{has } 0 \text{ or } \infty \text{ solution} \\
\end{array}
$$

---

Page 166

**Four types for $R$ and Their ranks**

$$
\left[\begin{array}{c}
I\\
\end{array}\right] \\
r = m = n
$$

$$
\left[\begin{array}{cc}
I & F \\
\end{array}\right] \\
r = m < n
$$

$$
\left[\begin{array}{c}
I \\
F \\
\end{array}\right] \\
r = n < m
$$

$$
\left[\begin{array}{cc}
I & F \\
0 & 0 \\
\end{array}\right] \\
r < m, r < n
$$

---

Page 166

**REVIEW OF THE KEY IDEAS**

1. The rank $r$ is the number of pivots. The matrix $R$ has $m - r$ zero rows.

2. $Ax = b$ is solvable if and only if the last $m - r$ equations reduce to
   $0 = 0$.

3. One particular solution $x_p$ has all free variables equal to zero.

4. The pivot variables are determined after the free variables are chosen.

5. Full column rank $r = n$ means no free variables: one solution or none.

6. Full row rank $r = m$ means one solution if $m = n$ or infinitely many if
   $m < n$.

---

Page 167

**The six steps to finding the complete solution (3.3A)**

1. Reduce $\left[\begin{array}{cc}A & b\\\end{array}\right]$ to
   $\left[\begin{array}{cc}U & c\\\end{array}\right]$, so that $Ax = b$ becomes
   a triangular system $Ux = c$.

2. Find the condition on $b_1, b_2, b_3$ for $Ax = b$ to have a solution.

3. Describe the column space of $A$. Which plane in $\R^3$?

4. Describe the nullspace of $A$. Which special solutions in $\R^4$?

5. Reduce $\left[\begin{array}{cc}U & c\\\end{array}\right]$ to
   $\left[\begin{array}{cc}R & d\\\end{array}\right]$: Special solutions from
   $R$, particular solution from $d$.

6. Find a particular solution to $Ax = (0, 6, -6)$ and then the complete
   solution.

---

Page 175

## 3.4 Independence, Basis and Dimension

---

Page 175

1. **Independent columns** of $A$: The only solution to $Ax = \mathbf{0}$ is
   $x = \mathbf{0}$. The nullspace is $\Z$.

2. Independent vectors: The only zero combination $c_1v_1 + \cdots + c_kv_k = 0$
   has all $c$'s $= 0$.

3. A matrix with $m < n$ has **dependent columns**: At least $n - m$ free
   variables/ special solutions.

4. The vectors $v_1, \dots, v_k$ **span the space** $S$ if $S =$ all
   combinations of the $v$'s.

5. The vectors $v_1, \dots, v_k$ are a **basis for** $S$ if they are independent
   and they span $S$.

6. The **dimension of a space** $S$ is the number of vectors in every basis for
   $S$.

7. If $A$ is 4 by 4 and invertible, its columns are a basis for $\R^4$. The
   dimension of $\R^4$ is 4.

---

Page 175

1. Independent vectors _(no extra vectors)_

2. Spanning a space _(enough vectors to produce the rest)_

3. Basis for a space _(not too many or two few)_

4. Dimension of a space _(the number of vectors in a basis)_

---

Page 175

**DEFINITION**

The columns of $A$ are _linearly independent_ when the only solution to
$Ax = \mathbf{0}$ is $x = \mathbf{0}$. _No other combination $Ax$ of the columns
gives the zero vector_.

---

Page 176

**DEFINITION**

The sequence of vectors $v_1, \dots, v_n$ is _linearly independent_ if the only
combination that gives the zero vector is $0v_1 + 0v_2 + \cdots + 0v_n$.

**Linear independence**

$x_1v_1 + x_2v_2 + \cdots x_nv_n = \mathbf{0}$ only happens when all $x$'s are
zero.

---

Page 177

**Full column rank**

The columns of $A$ are independent exactly when the rank is $r = n$. There are
$n$ pivots and no free variables. Only $x = \mathbf{0}$ is in the nullspace.

---

Page 177

Any set of $n$ vectors in $\R^m$ must be linearly dependent if $n > m$.

---

Page 178

**DEFINITION**

A set of vectors _spans_ a space if their linear combinations fill the space.

---

Page 179

**DEFINITION**

The _row space_ of a matrix is the subspace $\R^n$ spanned by the rows.

_The row space of $A$ is $C(A^{\mathbf{T}})$. It is the column space of
$A^{\mathbf{T}}$_.

---

Page 179

**DEFINITION**

A _basis_ for a vector space is a sequence of vectors with two properties:

_The basis vectors are linearly independent and they span the space._

---

Page 180

The vectors $v_1, \dots, v_n$ are a _basis for $\R^n$_ exactly when they are
_the columns of an $n$ by $n$ invertible matrix_. Thus $\R^n$ has infinitely
many different bases.

---

Page 180

_The pivot columns of $A$ are a basis for its column space._ The pivot rows of
$A$ are a basis for its row space. So are the pivot rows of its echelon form
$R$.

---

Page 181

If $v_1, \dots, v_m$ and $w_1, \dots, w_n$ are both bases for the same vector
space, then $m = n$.

---

Page 182

**DEFINITION**

The _dimension of a space is the number of vectors in every basis_.

---

Page 184

**REVIEW OF THE KEY IDEAS**

1. The columns of $A$ are _independent_ if $x = \mathbf{0}$ is the only solution
   to $Ax = \mathbf{0}$.

2. The vectors $v_1, \dots, v_r$ _span_ a space if their combinations fill that
   space.

3. _A basis consists of linearly independent vectors that span the space._ Every
   vector in the space is a _unique_ combination of the basis vectors.

4. All bases for a space have the same number of vectors. This number of vectors
   in a basis is the _dimension_ of the space.

5. The pivot columns are one basis for the column space. The dimension is $r$.

---

Page 192

## 3.5 Dimensions of the Four Subspaces

---

Page 192

1. The column space $C(A)$ and the row space $C(A^{\mathbf{T}})$ both have
   _dimension_ $r$ (the rank of $A$).

2. The nullspace $N(A)$ has _dimension_ $n - r$. The left nullspace
   $N(A^{\mathbf{T}})$ has _dimension_ $m - r$.

3. Elimination produces bases for the row space and nullspace of $A$: They are
   the same as for $R$.

4. Elimination often changes the column space and left nullspace (but dimensions
   don't change).

5. **Rank one matrices**: $A = uv^{\mathbf{T}} = \text{ column times row }$:
   $C(A)$ has basis $u$, $C(A^{\mathbf{T}})$ has basis $v$.

---

Page 192

**Four Fundamental Subspaces**

1. The _row space_ is $C(A^{\mathbf{T}})$, a subspace of $\R^n$.

2. The _column space_ is $C(A)$, a subspace of $\R^m$.

3. The _nullspace_ is $N(A)$, a subspace of $\R^n$.

4. The _left nullspace_ is $N(A^{\mathbf{T}})$, a subspace of $\R^m$. This is
   our new space.

---

Page 194

In $\R^n$ the row space and nullspace have dimensions $r$ and $n - r$ (adding to
$n$).

In $\R^m$ the column space and left nullspace have dimensions $r$ and $m - r$
(total $m$).

---

Page 196

$$ (\text{dimension of column space}) + (\text{dimension of nullspace}) = \text{dimension of } \R^n $$

---

Page 196

**Fundamental Theorem of Linear Algebra, Part 1**

The column space and row space both have dimension $r$.

The nullspaces have dimensions $n - r$ and $m - r$.

---

Page 199

Every rank one matrix is one column times one row

$$ A = uv^{\mathbf{T}} $$
