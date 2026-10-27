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
