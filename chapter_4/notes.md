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

Page 206

_The row space is perpendicular to the nullspace_. Every row of $A$ is
perpendicular to every solution of $Ax = \mathbf{0}$. That gives the $90\degree$
angle on the left side of the figure. This perpendicularity of subspaces is Part
2 of the Fundamental Theorem of Linear Algebra.

_The column space is perpendicular to the nullspace of $A^{\mathbf{T}}$_. When
$b$ is outside the column space - when we want to solve $Ax = b$ and can't do
it - then this nullspace of $A^{\mathbf{T}}$ comes into its own. It contains the
error $e = b - Ax$ in the "least-squares" solution. Least squares is the key
application of linear algebra in this chapter.

---

Page 206

**DEFINITION**

Two subspaces $V$ and $W$ of a vector space are _orthogonal_ if every vector $v$
in $V$ is perpendicular to every vector $w$ in $W$.

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

Page 208

**DEFINITION**

The _orthogonal complement of a subspace $V$ contains _every_ vector that is
perpendicular to $V$. This orthogonal subspace is denoted by $V^{\perp}$
(pronounced "$V$" perp).

By this definition, the nullspace is the orthogonal complement of the row space.
_Every_ $x$ that is perpendicular to the rows satisfies $Ax = \mathbf{0}$, and
lies in the nullspace.

The reverse is also true. _If $v$ is orthogonal to the nullspace, it must be in
the row space_. Otherwise we could add this $v$ as an extra row of the matrix,
without changing its nullspace. The row space would grow, which breaks the law
$r + (n - r) = n$. We conclude that the nullspace complement $N(A)^{\perp}$ is
exactly the row space $C(A^{\mathbf{T}})$.

In the same way, the left nullspace and column space are orthogonal in $\R^m$,
and they are orthogonal complements. Their dimensions $r$ and $m - r$ add to the
full dimension $m$.

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

---

Page 217

## 4.2 Projections

---

Page 217

1. The projection of a vector $b$ onto the line through $a$ is the closest point
   $p = a(a^{\mathbf{T}}b/a^{\mathbf{T}}a)$.

2. The error $e = b - p$ is perpendicular to $a$: Right triangle $bpe$ has
   $\|p\|^2 + \|e\|^2 = \|b\|^2$.

3. The **projection** of $b$ onto a subspace $S$ is the closest vector $p$ in
   $S$; $b - p$ is orthogonal to $S$.

4. $A^{\mathbf{T}}A$ is invertible (and symmetric) only if $A$ has independent
   columns: $N(A^{\mathbf{T}}A) = N(A)$.

5. Then the projection of $b$ onto the column space of $A$ is the vector
   $p = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}b$.

6. The **projection matrix** onto $C(A)$ is
   $\boxed{P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}}$. It has $p = Pb$ and
   $P^2 = P = P^{\mathbf{T}}$.

---

Page 219

The projection of $b$ onto the line through $a$ is the vector

$$ p = \hat{x}a = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}a $$

Special case 1: If $b = a$ then $\hat{x} = 1$. The projection of $a$ onto $a$ is
itself. $Pa = a$.

Special case 2: If $b$ is perpendicular to $a$ then $a^{\mathbf{T}}b = 0$. The
projection is $p = \mathbf{0}$.

---

Page 220

Projection matrix $P$

$$ p = a\hat{x} = a\frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} = Pb $$

when the matrix is

$$ P = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

---

Page 223

$A^{\mathbf{T}}A$ is invertible if and only if $A$ has linearly independent
columns.

---

Page 224

**REVIEW OF THE KEY IDEAS**

1. The projection of $b$ onto the line through $a$ is
   $p = a\hat{x} = a(a^{\mathbf{T}}b/a^{\mathbf{T}}a)$.

2. The rank one projection matrix $P = aa^{\mathbf{T}}/a^{\mathbf{T}}a$
   multiplies $b$ to produce $p$.

3. Projecting $b$ onto a subspace leaves $e = b - p$ perpendicular to the
   subspace.

4. When $A$ has full rank $n$, the equation
   $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$ leads to $\hat{x}$ and
   $p = A\hat{x}$.

5. The projection matrix $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ has
   $P^{\mathbf{T}} = P$ and $P^2 = P$ and $Pb = p$.
