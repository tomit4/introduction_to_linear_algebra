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
