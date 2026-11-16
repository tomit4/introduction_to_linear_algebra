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

---

Page 230

## 4.3 Least Squares Approximations

1. Solving $\boxed{A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b}$ gives the
   projection $p = A\hat{x}$ of $b$ onto the column space of $A$.

2. When $Ax = b$ has no solution, $\hat{x}$ is the "least-squares solution":
   $\|b - A\hat{x}\|^2 =$ minimum.

3. Setting partial derivatives of $E = \|Ax - b\|^2$ to zero
   $\left(\frac{\partial E}{\partial x_i} = 0\right)$ also produces
   $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

4. To fit points $(t_1, b_2), \dots, (t_m, b_m)$ by a straight line, $A$ has
   columns $(1, \dots, 1)$ and $(t_1, \dots, t_m)$.

5. In that case $A^{\mathbf{T}}A$ is the $2$ by $2$ matrix
   $\left[\begin{array}{cc}m & \sum{t_i} \\\sum{t_i} & \sum{t_i^2} \\\end{array}\right]$
   and $A^\mathbf{T}b$ is the vector
   $\begin{bmatrix}{}\sum{b_i}\\\sum{t_ib_i}\end{bmatrix}$.

---

Page 230

When $Ax = b$ has no solution, multiply by $A^{\mathbf{T}}$ and solve
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

---

Page 233

The partial derivatives of $\|Ax - b\|^2$ are zero when
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

---

Page 235

The line $C + Dt$ minimizes $e_1^2 + \cdots + e_m^2 = \|Ax - b\|^2$ when
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:

$$ A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b \quad
\left[\begin{array}{cc}
m & \sum{t_i} \\
\sum{t_i} & \sum{t_i^2} \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}\sum{b_i}\\\sum{t_ib_i}\end{bmatrix}
$$

---

Page 238

**REVIEW OF THE KEY IDEAS**

1. The least squares solution $\hat{x}$ minimizes
   $\|Ax - b\|^2 = x^{\mathbf{T}}A^{\mathbf{T}}Ax - 2x^{\mathbf{T}}A^{\mathbf{T}}b + b^{\mathbf{T}}b$.
   This is $E$, the sum of squares of the errors in the $m$ equations ($m > n$).

2. The best $\hat{x}$ comes from the normal equations
   $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$. $E$ is a minimum.

3. To fit $m$ points by a line $b = C + Dt$, the normal equations give $C$ and
   $D$.

4. The heights of the best line are $p = (p_1, \dots, p_m)$. The vertical
   distances to the data points are the errors $e = (e_1, \dots, e_m)$. A key
   equation is $A^{\mathbf{T}}e = \mathbf{0}$.

5. If we try to fit $m$ points by a combination of $n < m$ functions, the $m$
   equations $Ax = b$ are generally unsolvable. The $n$ equations
   $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$ give the least squares solution -
   the combination with the smallest $\text{MSE}$ (mean square error).

---

Page 244

## 4.4 Orthonormal Bases and Gram-Schmidt

---

Page 244

1. The columns $q_1, \dots, q_n$ are orthonormal if
   $q_i^{\mathbf{T}}q_j = \left\{\begin{array}{}0 \text{ for } i \neq j \\ 1 \text{ for } i = j \end{array}\right\}$.
   Then $\boxed{Q^{\mathbf{T}}Q = I}$.

2. If $Q$ is also square, then $QQ^{\mathbf{T}} = I$ and
   $\boxed{Q^{\mathbf{T}} = Q^{-1}}$. $Q$ is an "orthogonal matrix".

3. The least squares solution to $Qx = b$ is $\hat{x} = Q^{\mathbf{T}}b$.
   Projection of $b$: $p = QQ^{\mathbf{T}}b = Pb$.

4. The **Gram-Schmidt** process takes independent $a_i$ to orthonormal $q_i$.
   Start with $q_1 = \dfrac{a_1}{\|a_1\|}$.

5. $q_i$ is $\dfrac{(a_i - \text{projection } p_i)}{\|a_i - p_i\|}$; projection
   $p_i = (a_i^{\mathbf{T}}q_1)q_1 + \cdots + (a_i^{\mathbf{T}}q_{i - 1})q_{i - 1}$.

6. Each $a_i$ will be a combination of $q_1$ to $q_i$. Then $A = QR$; orthogonal
   $Q$ and triangular $R$.

---

Page 244

**DEFINITION**

The vectors $q_1, \dots, q_n$ are orthonormal if

$$
q_i^{\mathbf{T}}q_j =
\begin{cases}
0 & \text{when } i \neq j \quad (\text{orthogonal vectors}) \\
1 & \text{when } i = j \quad (\text{unit vectors: } \|q_i\| = 1)
\end{cases}
$$

A matrix with orthonormal columns is assigned the special letter $Q$.

---

Page 248

**First Gram-Schmidt step**

$$ B = b - \frac{A^{\mathbf{T}}b}{A^{\mathbf{T}}A}A $$

---

Page 248

**Next Gram-Schmidt step**

$$ C = c - \frac{A^{\mathbf{T}}c}{A^{\mathbf{T}}A}A = \frac{B^{\mathbf{T}}c}{B^{\mathbf{T}}B}B $$

---

Page 250

**(Gram-Schmidt)** From independent vectors $a_1, \dots, a_n$, Gram-Schmidt
constructs orthonormal vectors $q_1, \dots, q_n$. The matrices with these
columns satisfy $A = QR$. Then $R = Q^{\mathbf{T}}A$ is **upper triangular**
because later $q$'s are orthogonal to earlier $a$'s.

---

Page 251

**Least squares**

$$ R^{\mathbf{T}}R\hat{x} = R^{\mathbf{T}}Q^{\mathbf{T}}b $$

or

$$ R\hat{x} = Q^{\mathbf{T}}b $$

or

$$ \hat{x} = R^{-1}Q^{\mathbf{T}}b $$

---

Page 252

**REVIEW OF THE KEY IDEAS**

1. If the orthonormal vectors $q_1, \dots, q_n$ are the columns of $Q$, then
   $q_i^{\mathbf{T}}q_j = 0$ and $q_i^{\mathbf{T}}q_i = 1$ translate into the
   matrix multiplication $Q^{\mathbf{T}}Q = I$.

2. If $Q$ is square (an **orthogonal matrix**) then $Q^{\mathbf{T}} = Q^{-1}$:
   _transpose_ $=$ _inverse_.

3. The length of $Qx$ equals the length of $x$: $\|Qx\| = \|x\|$.

4. The projection onto the column space of $Q$ spanned by the $q$'s is
   $P = QQ^{\mathbf{T}}$.

5. If $Q$ is square then $P = QQ^{\mathbf{T}} = I$ and every
   $b = q_1(q_1^{\mathbf{T}}b) + \cdots + q_n(q_n^{\mathbf{T}}b)$.

6. Gram-Schmidt produces orthonormal vectors $q_1, q_2, q_3$ from independent
   $a, b, c$. In matrix form this is the factorization
   $A = QR = (\text{orthogonal } Q)(\text{triangular} R)$.
