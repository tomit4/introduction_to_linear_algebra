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
