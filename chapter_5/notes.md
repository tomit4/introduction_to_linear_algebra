Page 258

# 5.1 The Properties of Determinants

---

Page 258

1. The **determinant** of
   $A = \left[\begin{array}{cc}a & b \\c & d \\\end{array}\right]$. Singular
   matrix $A = \left[\begin{array}{cc}a & xa \\c & xc \\\end{array}\right]$ has
   $\det = \mathbf{0}$.

2. **Row exchange reverses signs**
   $PA = \left[\begin{array}{cc}0 & 1 \\1 & 0 \\\end{array}\right]\left[\begin{array}{cc}a & b \\c & d \\\end{array}\right] = \left[\begin{array}{cc}c & d \\a & b \\\end{array}\right]$
   has $\det PA = bc - ad = -\det A$.

3. The determinant of
   $\left[\begin{array}{cc}xa + yA & xb + yB \\c & d \\\end{array}\right]$ is
   $x(ad - bc)+ y(Ad - Bc)$. **Det is linear in row 1 by itself.**

4. **Elimination**
   $EA = \left[\begin{array}{cc}a & b \\0 & d - \dfrac{c}{a}b\end{array}\right]$
   $\det EA = a\left(d - \dfrac{c}{a}b\right) =$ **product of pivots**
   $= \det A$.

5. If $A$ is $n$ by $n$ then $1, 2, 3, 4$ remain true: $\det = \mathbf{0}$ when
   $A$ is singular, $\det$ reverses sign when rows are exchanged, $\det$ is
   linear in row $1$ by itself, $\det =$ product of the pivots. Always
   $\det BA = (\det B)(\det A)$ and $\det A^{\mathbf{T}} = \det A$. This is an
   amazing number.

---

Page 264

**REVIEW OF THE KEY IDEAS**

1. The determinant is defined by $\det I = 1$, sign reversal, and linearity in
   each row.

2. After elimination $\det A$ is $\pm$ (product of the pivots).

3. The determinant is zero exactly when $A$ is not invertible.

4. Two remarkable properties are $\det AB = (\det A)(\det B)$ and
   $\det A^{\mathbf{T}} = \det A$.

---

Page 269

## 5.2 Permutations and Cofactors

1. $2$ by $2$: $ad - bc$ has $2!$ terms with $\pm$ signs. $n$ by $n$: $\det A$
   adds $n!$ terms with $\pm$ signs.

2. For $n = 3$, $\det A$ adds $3! = 6$ terms. Two terms are
   $+a_{12}a_{23}a_{31}$ and $-a{13}a_{22}a_{31}$. Rows 1, 2, 3 and columns 1,
   2, 3 appear once in each term.

3. That minus sign came because the column order $3, 2, 1$ needs one exchange to
   recover $1, 2, 3$.

4. The six terms include
   $+a_{11}a_{22}a_{33} - a_{11}a_{23}a_{32} = a_{11}(a_{22}a_{33} - a_{23}a_{32}) = a_{11}(\text{cofactor } C_{11})$

5. Always $\det A = a_{11}C_{11} + a_{12}C_{12} + \cdots + a_{1n}C_{1n}$.
   Cofactors are determinants of size $n - 1$.

---

Page 270

$$ (\det P)(\det A) = (\det L)(\det U) \text{ gives } \det A = \pm(d_1d_2 \cdots d_n) $$

---

Page 270

**Pivots from determinants**

The $k$th pivot is

$$ d_k = \frac{d_1d_2 \cdots d_k}{d_1d_2 \cdots d_{k - 1}} = \frac{\det A_k}{\det A_{k - 1}} $$

---

Page 272

$\det A =$ sum of all $n!$ column permutations
$P = (\alpha, \beta, \dots, \omega)$

$$ = \sum(\det P)a_{1\alpha}a_{2\beta} \cdots a_{n\omega} = \textbf{BIG FORMULA} $$

---

Page 275

The determinant is the dot product of any row $i$ of $A$ with its cofactors
using other rows:

**COFACTOR FORMULA**

$$ \det A = a_{i1}C_{i1} + a_{i2}C_{i2} + \cdots + a_{in}C_{in} $$

Each cofactor $C_{ij}$ (order $n - 1$, without row $i$ and column $j$) includes
its correct sign:

**Cofactor**

$$ C_{ij} = (-1)^{i + j}\det M_{ij} $$

---

Page 276

**REVIEW OF THE KEY IDEAS**

1. With no row exchanges, $\det A = (\textit{product of pivots})$. In the upper
   left corner of $A$,
   $\det A_k = (\textit{product of the first } k \textit{pivots})$.

2. Every term in the big formula (8) uses each row and column once. Half of the
   $n!$ terms have plus signs (when $\det P = + 1$) and half have minus signs.

3. The cofactor $C_{ij}$ is $(-1)^{i + j}$ times the smaller determinant that
   omits row $i$ and column $j$ (because $a_{ij}$ uses that row and column).

4. The determinant is the dot product of any row of $A$ with its row of
   cofactors. When a row of $A$ has a lot of zeros, we only need a few
   cofactors.
