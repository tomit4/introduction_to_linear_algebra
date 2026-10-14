## 1.1 Vectors and Linear Combinations

---

Page 12

**Linear combination**

$$ cv + dw = c\begin{bmatrix}{}1\\1\end{bmatrix} + d\begin{bmatrix}{}2\\2\end{bmatrix} = \begin{bmatrix}{}c + 2d\\c + 3d\end{bmatrix} $$

---

Page 13

1. $3v + 5w$ is a typical **linear combination** $cv + dw$ of vectors $v$ and
   $w$.

2. For $v = \begin{bmatrix}{}1\\1\end{bmatrix}$ and
   $w = \begin{bmatrix}{}2\\3\end{bmatrix}$ that combination is
   $3\begin{bmatrix}{}1\\1\end{bmatrix} + 5\begin{bmatrix}{}2\\3\end{bmatrix} = \begin{bmatrix}{}3 + 10\\3 + 15\end{bmatrix} = \begin{bmatrix}{}13\\18\end{bmatrix}$

3. The vector
   $\begin{bmatrix}{}2\\3\end{bmatrix} = \begin{bmatrix}{}2\\0\end{bmatrix} + \begin{bmatrix}{}0\\3\end{bmatrix}$
   goes across to $x = 2$ and up to $y = 3$ in the $xy$ plane.

4. The combinations $c\begin{bmatrix}{}1\\1\end{bmatrix}$ +
   $d\begin{bmatrix}{}2\\3\end{bmatrix}$ fill the whole $xy$ plane. They produce
   ever $\begin{bmatrix}{}x\\y\end{bmatrix}$.

5. The combinations $c\begin{bmatrix}{}1\\1\\1\end{bmatrix}$ +
   $d\begin{bmatrix}{}2\\3\\4\end{bmatrix}$ fill a **plane** in the $xyz$ space.
   Same plane for
   $\begin{bmatrix}{}1\\1\\1\end{bmatrix}, \begin{bmatrix}{}3\\4\\5\end{bmatrix}$.

6. But $\begin{bmatrix}{}c + 2d = 1\\c + 3d = 0\\c + 4d = 0\end{bmatrix}$ has no
   solution because its right side $\begin{bmatrix}{}1\\0\\0\end{bmatrix}$ is
   not on that plane.

---

Page 13

**Column vector $v$**

$$ v = \begin{bmatrix}{}v_1\\v_2\end{bmatrix} $$

$$ v_1 = \text{first component of } v\\ v_2 = \text{first component of } v $$

---

Page 13

**Vector Addition**

$$ v = \begin{bmatrix}{}v_1\\v_2\end{bmatrix} \text{ and } w = \begin{bmatrix}{}w_1\\w_2\end{bmatrix} \text{ add to } v + w = \begin{bmatrix}{}v_1 + w_1\\v_2 + w_2\end{bmatrix} $$

---

Page 13

**Scalar Multiplication**

$$ 2v = \begin{bmatrix}{}2v_1\\2v_2\end{bmatrix} = v + v - v = \begin{bmatrix}{}-v_1\\-v_2\end{bmatrix} $$

---

Page 14

The sum of $cv$ and $dw$ is a **linear combination $cv + dw$**.

---

Page 15

From now on $v = \begin{bmatrix}{}1\\1\\-1\end{bmatrix}$ is also written as
$v = (1, 1, -1)$.

---

Page 17

**1.1 A**

The linear combination of $v = (1, 1, 0)$ and $w = (0, 1, 1)$ fill a plane
$\mathbf{R}^3$. _Describe that plane_. Find a vector that is _not_ a combination
of $v$ and $w$ - not on the plane.

**Solution** The plane of $v$ and $w$ contains all combinations $cv + dw$. The
vectors in that plane allow any $c$ and $d$. The plane of Figure 1.3 fills in
between the two lines.

Combinations

$$ cv + dw = c\begin{bmatrix}{}1\\1\\0\end{bmatrix} + d\begin{bmatrix}{}0\\1\\1\end{bmatrix} = \begin{bmatrix}{}c\\c + d\\ d\end{bmatrix} $$

fill a plane.

Four vectors in that plane are $(0, 0, 0)$ and $(2, 3, 1)$ and $(5, 7, 2)$ and
$(\pi, 2\pi, \pi)$. The second component $c + d$ is always the sum of the first
and third components. Like most vectors $(1, 2, 3)$ _is **not** in the plane,
because_ $2 \neq 1 + 3$.

Another description of this plane through $(0, 0, 0)$ is to know that
$n = (1, -1, 1)$ is **perpendicular** to the plane. Section 1.2 will confirm
that $90\degree$ angle by testing dot products: $v \cdot n = 0$ and
$w \cdot n = 0$. Perpendicular vectors have zero dot products.

---

1.1 C Find two equations for $c$ and $d$ so that **the linear combination**
$cv + dw$ equals $b$:

$$ v = \begin{bmatrix}{}2\\-1\end{bmatrix} \quad w = \begin{bmatrix}{}-1\\2\end{bmatrix} \quad b = \begin{bmatrix}{}1\\0\end{bmatrix} $$

---

## 1.2 Lengths and Dot Products

---

Page 22

1. The "dot product" of $v = \begin{bmatrix}{}1\\2\end{bmatrix}$ and
   $w = \begin{bmatrix}{}4\\5\end{bmatrix}$ is
   $v \cdot w = (1)(4) + (2)(5) = 4 + 10 = 14$.

2. $v = \begin{bmatrix}{}1\\3\\2\end{bmatrix}$ and
   $w = \begin{bmatrix}{}4\\-4\\4\end{bmatrix}$ are perpendicular because
   $v \cdot w$ is zero:

$$ (1)(4) + (3)(-4) + (2)(4) = 0 $$

3. The length squared of $v = \begin{bmatrix}{}1\\3\\2\end{bmatrix}$ is
   $v \cdot v = 1 + 9 + 4 = 14$. The **length is** $\|v\| = \sqrt{14}$.

4. Then
   $u = \dfrac{v}{\|v\|} = \dfrac{v}{\sqrt{14}} = \dfrac{1}{\sqrt{14}}\begin{bmatrix}{}1\\3\\2\end{bmatrix}$
   has length $\|u\| = 1$. Check
   $\dfrac{1}{14} + \dfrac{9}{14} + \dfrac{4}{14} = 1$.

5. The angle $\theta$ between $v$ and $w$ has
   $\cos\theta = \dfrac{v \cdot w}{\|v\| \|w\|}$.

6. The angle between $\begin{bmatrix}{}1\\0\end{bmatrix}$ and
   $\begin{bmatrix}{}1\\1\end{bmatrix}$ has
   $\cos\theta = \dfrac{1}{(1)(\sqrt{2})}$. That angle is $\theta = 45\degree$.

7. All angles have $|\cos\theta| \leq 1$. So all vectors have
   $\boxed{| v \cdot w| \leq \|v\| \|w\|}$.

---

Page 22

The **dot product** or **inner product** of $v = (v_1, v_2)$ and
$w = (w_1, w_2)$ is the number $v \cdot w$:

$$ v \cdot w = v_1w_1 + v_2w_2 $$

---

Page 23

**Definition**

The **length** $\|v\|$ of a vector $v$ is the square root of $v \cdot v$:

$$ \textbf{length} = \|v\| = \sqrt{v \cdot v} = \left(v_1^2 + v_2^2 + \cdots + v_n^2\right)^{\frac{1}{2}} $$

---

Page 24

**Definition**

A _unit vector $u$ is a vector whose length equals one._ Then $u \cdot u = 1$.

---

Page 24

**Unit Vector**

$u = \dfrac{v}{\|v\|}$ is a unit vector in the same direction as $v$.

---

Page 25

**Right Angles**

The dot product is $v \cdot w = 0$ when $v$ is perpendicular to $w$.

---

Page 26

Unit vectors $u$ and $U$ at angle $\theta$ have $u \cdot U = \cos\theta$.
Certainly $|u \cdot U| \leq 1$.

---

Page 27

**COSINE FORMULA**

If $v$ and $w$ are nonzero vectors then
$\dfrac{v \cdot w}{\|v\|\|w\|} = \cos\theta$.

---

Page 27

**SCHWARZ INEQUALITY**

$$ |v \cdot w| \leq \|v\|\|w\| $$

---

Page 27

**TRIANGLE INEQUALITY**

$$ \|v + w\| \leq \|v\| + \|w\| $$

---

Page 33

1. $A = \left[\begin{array}{cc} 1 & 2 \\ 3 & 4 \\ 5 & 6 \\ \end{array}\right]$
   is a $3$ by $2$ matrix: $m = 3$ rows and $n = 2$ columns.

2. $Ax = \left[\begin{array}{cc} 1 & 2 \\ 3 & 4 \\ 5 & 6 \\ \end{array}\right]\begin{bmatrix}{}x_1\\x_2\end{bmatrix}$
   is a **combination of the columns**
   $A_x = x_1\begin{bmatrix}{}1\\3\\5\end{bmatrix} + x_2\begin{bmatrix}{}2\\4\\6\end{bmatrix}$.

3. The $3$ components of $Ax$ are dot products of the $3$ rows of $A$ with the
   vector $x$:

$$ \text{Row at a time} \quad
\left[\begin{array}{cc}
1 & 2 \\
3 & 4 \\
5 & 6 \\
\end{array}\right]
\begin{bmatrix}{}7\\8\end{bmatrix}
= \begin{bmatrix}{}1 \cdot 7 + 2 \cdot 8\\3 \cdot 7 + 4 \cdot 8\\ 5 \cdot 7 + 6 \cdot 8\end{bmatrix} = \begin{bmatrix}{}23\\53\\83\end{bmatrix} $$

4 Equations in matrix form

$$ Ax = b: \left[\begin{array}{cc}
2 & 5 \\
3 & 7 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}b_2\\b_2\end{bmatrix}
$$

replaces

$$
2x_1 + 5x_2 = b_2 \\
3x_2 + 7x_2 = b_2
$$

5. The solution to $Ax = b$ can be written as $x = A^{-1}b$. But some matrices
   don't allow $A^{-1}$.

---

Page 33

**Matrix times vector Combination of columns**

$$
Ax = \left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}x_1\\x_2 - x_1\\ x_3 - x_2\end{bmatrix}
$$

---

Page 35

**Equations $Ax = b$**

$$ x_1 = b_1 \\ -x_1 + x_2 = b_2 \\

- x_2 + x_3 = b_3 $$

**Solution $x = A^{-1}b$**

$$
x_1 = b_1 \\
x_2 = b_1 + b_2 \\
x_3 = b_1 + b_2 + b_3
$$

---

Page 36

**Cyclic**

$$
C_x =
\left[\begin{array}{ccc}
1 & 0 & -1 \\
-1 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}x_1 - x_3\\x_2 - x_1\\ x_3 - x_2\end{bmatrix} =
b
$$

---

Page 37

**$Cx = b$**

$$ \begin{bmatrix}{}x_1 - x_3\\x_2 - x_1\\ x_3 - x_2\end{bmatrix} = \begin{bmatrix}{}1\\3\\5\end{bmatrix} $$

Left sides add to $0$

Right sides add to $9$.

_No solution_ $x_1, x_2, x_3$
