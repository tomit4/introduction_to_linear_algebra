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
