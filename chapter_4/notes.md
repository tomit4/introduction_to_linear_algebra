Page 205

## 4.1 Orthogonality of the Four Subspaces

---

Page 205

1. Orthogonal vectors have $v^{\mathbf{T}}w = 0$. Then
   $||v||^2 + ||w||^2 = ||v + w||^2 = ||v - w||^2$.

2. Subspaces $V$ and $W$ are orthogonal when $v^{\mathbf{T}}w = 0$ for every $v$
   in $V$ and every $w$ in $W$.

3. The row space of $A$ is orthogonal to the nullspace. The column space is
   orthogonal to $N(A^{\mathbf{T}})$.

4. One pair of dimensions adds to $r + (n - r) = n$. The other pair has
   $r + (m - r) = m$.

5. Row space and nullspace are orthogonal _complements_. Every $x$ in $\R^n$
   splits into $x_{\text{row}} + x_{\text{null}}$.

6. Suppose a space $S$ has dimension $d$. Then every basis for $S$ consists of
   $d$ vectors.

7. If $d$ vectors in $S$ are independent, they span $S$. If $d$ vectors span
   $S$, they are independent.

---

Page 207

Every vector $x$ in the nullspace is perpendicular to every row of $A$, because
$Ax = \mathbf{0}$. The nullspace $N(A)$ and the row space $C(A^{\mathbf{T}})$
are orthogonal subspaces of $\R^n$.

---

Page 207

Every vector $y$ in the nullspace of $A^{\mathbf{T}}$ is perpendicular to every
column of $A$. The left nullspace $N(A^{\mathbf{T}})$ and the column space
$C(A)$ are orthogonal in $\R^m$.

---

Page 209

**Fundamental Theorem of Linear Algebra, Part 2**

$N(A)$ is the orthogonal complement of the row space $C(A^{\mathbf{T}})$ (in
$\R^n$).

$N(A^{\mathbf{T}})$ is the orthogonal complement of the column space $C(A)$ (in
$\R^m$)

---

Page 211

Any $n$ independent vectors in $\R^n$ must span $\R^n$. So they are a basis.

Any $n$ vectors that span $\R^n$ must be independent. So they are a basis.

---

Page 211

If the $n$ columns of $A$ are independent, they span $\R^n$. So $Ax = b$ is
solvable.

If the $n$ columns span $\R^n$, they are independent. SO $Ax = b$ has only one
solution.

---

**REVIEW OF THE KEY IDEAS**

1. Subspaces $V$ and $W$ are orthogonal if every $v$ in $V$ is orthogonal to
   every $w$ in $W$.

2. $V$ and $W$ are "orthogonal complements" if $W$ contains **all** vectors
   perpendicular to $V$ (and vice versa). Inside $\R^n$, the dimensions of
   complements $V$ and $W$ add to $n$.

3. The nullspace $N(A)$ and the row space $C(A^{\mathbf{T}})$ are orthogonal
   complements, with dimensions $(n - r) + r = n$. Similarly $N(A^{\mathbf{T}})$
   and $C(A)$ are orthogonal complements with $(m - r) + r = m$.

4. Any $n$ independent vectors in $\R^n$ span $\R^n$. Any $n$ spanning vectors
   are independent.
