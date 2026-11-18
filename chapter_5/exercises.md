Page 265

## Problem Set 5.1

**Questions 1-12 are about the rules for determinants.**

1. If a $4$ by $4$ matrix has $\det A = \frac{1}{2}$, find $\det(2A)$ and
   $\det(-A)$ and $\det(A^2)$ and $\det(A^{-1})$.

2. If a $3$ by $3$ matrix has $\det A = -1$, find
   $\det\left(\dfrac{1}{2}A\right)$ and $\det(-A)$ and $\det(A^2)$ and
   $\det(A^{-1})$.

3. True or false, with a reason if true or a counterexample if false:

a. The determinant of $I + A$ is $1 + \det A$.

b. The determinant of $ABC$ is $|A||B||C|$.

c. The determinant of $4A$ is $4|A|$.

d. The determinant of $AB - BA$ is zero. Try an example with
$A =\left[\begin{array}{cc}0 & 0 \\0 & 1 \\\end{array}\right]$.

4. Which row exchanges show that these "reverse identity matrices" $J_3$ and
   $J_4$ have $|J_3| = -1$ but $|J_4| = +1$?

$$
\det\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] = -1
$$

but

$$
\det\left[\begin{array}{cccc}
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
\end{array}\right] = +1
$$

5. For $n = 5, 6, 7$, count the row exchanges to permute the reverse identity
   $J_n$ to the identity matrix $I_n$. Propose a rule for every size $n$ and
   predict whether $J{101}$ has determinant $+1$ or $-1$.

6. Show how Rule 6 (determinant $= 0$ if a row is all zero) comes from Rule 3.

7. Find the determinants of rotations and reflections:

$$ Q =
\left[\begin{array}{rr}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{array}\right]
$$

and

$$ Q =
\left[\begin{array}{rr}
1 - 2\cos^2\theta & -2\cos\theta\sin\theta \\
-2\cos\theta\sin\theta & 1 - 2\sin^2\theta \\
\end{array}\right]
$$

8. Prove that every orthogonal matrix $(Q^{\mathbf{T}}Q = I)$ ha determinant $1$
   or $-1$.

a. Use the product rule $|AB| = |A||B|$ and the transpose rule $|Q| =
|Q^\{\mathbf{T}}|$.

b. Use only the product rule. If $|\det Q| > 1$ then $\det Q^n = (\det A)^n$
blows up. How do you know this can't happen to $Q^n$?

9. Do these matrices have determinant $0, 1, 2$ or $3$?

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

10. If the entries in every row of $A$ add to zero, solve $Ax = \mathbf{0}$ to
    prove $\det A = 0$. If those entries add to one, show that
    $\det(A - I) = 0$. Does this mean $\det A = 1$?

11. Suppose that $CD = -DC$ and find the flaw in this reasoning: Taking
    determinants gives $|C||D| = -|D||C|$. Therefore $|C| = 0$ or $|D| = 0$. One
    or both of the matrices must be singular. (That is not true.)

12. The inverse of a $2$ by $2$ matrix seems to have determinant $= 1$:

$$ \det A^{-1} =
\det \frac{1}{ad - bc}
\left[\begin{array}{rr}
d & -b \\
-c & a \\
\end{array}\right] =
\frac{ad - bc}{ad - bc} = 1
$$

What is wrong with this calculation? What is the correct $\det A^{-1}$?

**Questions 13-27 use the rules to compute specific determinants.**

13. Reduce $A$ to $U$ and find $\det A =$ product of the pivots:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 2 & 3 \\
3 & 3 & 3 \\
\end{array}\right]
$$

14. By applying row operations to produce an upper triangular $U$, compute

$$
\det\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
2 & 6 & 6 & 1 \\
-1 & 0 & 0 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right]
$$

$$
\det\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
-1 & 2 & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

15. Use row operations to simplify and compute these determinants:

$$
\det\left[\begin{array}{ccc}
101 & 201 & 301 \\
102 & 202 & 302 \\
103 & 203 & 303 \\
\end{array}\right]
$$

and

$$
\det\left[\begin{array}{ccc}
1 & t & t^2 \\
t & 1 & t \\
t^2 & t & 1 \\
\end{array}\right]
$$

16. Find the determinants of a rank one matrix and a skew-symmetric matrix:

$$ A =
\begin{bmatrix}{}1\\2\\3\end{bmatrix}
\left[\begin{array}{rrr}
1 & -4 & 5 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{rrr}
0 & 1 & 3 \\
-1 & 0 & 4 \\
-3 & -4 & 0 \\
\end{array}\right]
$$

17. A skew-symmetric matrix has $A^{\mathbf{T}} = -A$. Insert $a, b, c$ for
    $1, 3, 4$ in Question 16 and show that $|A| = 0$. Write down a $4$ by $4$
    example with $|A| = 1$.

18. Use row operations to show that the $3$ by $3$ "Vandermonde determinant" is

$$
\det\left[\begin{array}{ccc}
1 & a & a^2 \\
1 & b & b^2 \\
1 & c & c^2 \\
\end{array}\right] = (b - a)(c - a)(c - b)
$$

19. Find the determinants of $U$ and $U^{-1}$ and $U^2$:

$$ U =
\left[\begin{array}{ccc}
1 & 4 & 6 \\
0 & 2 & 5 \\
0 & 0 & 3 \\
\end{array}\right]
$$

and

$$ U =
\left[\begin{array}{cc}
a & b \\
0 & d \\
\end{array}\right]
$$

20. Suppose you do two row operations at once, going from

$$
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] \quad \text{ to } \quad
\left[\begin{array}{rr}
a - Lc & b - Ld \\
c - la & d - lb \\
\end{array}\right]
$$

Find the second determinant. Does it equal $ad - bc$?

21. _Row exchange_: Add row $1$ of $A$ to row $2$, then subtract row $2$ from
    row $1$. Then add row $1$ to row $2$ and multiply row $1$ by $-1$ to reach
    $B$. Which rule show

$$
\det B =
\begin{vmatrix}
c & d \\
a & d \\
\end{vmatrix} \quad \text{equals} \quad
-\det A =
-\begin{vmatrix}
a & b \\
c & d \\
\end{vmatrix}\text{?}
$$

Those rules could replace Rule 2 in the definition of the determinant.

22. From $ad - bc$, find the determinants of $A$ and $A^{-1}$ and
    $A - \lambda I$:

$$ A =
\left[\begin{array}{cc}
2 & 1 \\
1 & 2 \\
\end{array}\right]
$$

and

$$ A^{-1} =
\frac{1}{3}
\left[\begin{array}{rr}
2 & -1 \\
-1 & 2 \\
\end{array}\right]
$$

and

$$ A - \lambda I =
\left[\begin{array}{cc}
2 - \lambda & 1 \\
1 & 2 - \lambda \\
\end{array}\right]
$$

Which two numbers $\lambda$ to $\det(A - \lambda I) = 0$? Write down the matrix
$A - \lambda I$ for each of those numbers $\lambda$ - it should not be
invertible.

23. From $A = \left[\begin{array}{cc}4 & 1 \\2 & 3 \\\end{array}\right]$ find
    $A^2$ and $A^{-1}$ and $A - \lambda I$ and their determinants. Which two
    numbers $\lambda$ lead to $\det(A - \lambda I) = 0$?

24. Elimination reduces $A$ to $U$. Then $A = LU$:

$$ A =
\left[\begin{array}{rrr}
3 & 3 & 4 \\
6 & 8 & 7 \\
-3 & 5 & -9 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
-1 & 4 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
3 & 3 & 4 \\
0 & 2 & -1 \\
0 & 0 & -1 \\
\end{array}\right] = LU
$$

Find the determinants of $L, U, A, U^{-1}, L^{-1}$, and $U^{-1}L^{-1}A$.

25. If the $i, j$ entry of $A$ is $i$ times $j$, show that $\det A = 0$.
    (Exception when $A = [1]$.)

26. If the $i, j$ entry of $A$ is $i + j$, show that $\det A = 0$. (Exception
    when $n = 1$ or $2$.)

27. Compute the determinants of these matrices by row operations:

$$ A =
\left[\begin{array}{ccc}
0 & a & 0 \\
0 & 0 & b \\
c & 0 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cccc}
0 & a & 0 & 0 \\
0 & 0 & b & 0 \\
0 & 0 & 0 & c \\
d & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
a & a & a \\
a & b & b \\
a & b & c \\
\end{array}\right]
$$

28. True or false (give a reason if true or a $2$ by $2$ example if false):

a. If $A$ is not invertible then $AB$ is not invertible.

b. The determinant of $A$ is always the product of its pivots.

c. The determinant of $A - B$ equals $\det A - \det B$.

d. $AB$ and $BA$ have the same determinant.

29. What is wrong with this proof that projection matrices have $\det P = 1$?

$$ P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} \quad \text{so} \quad |P| = |A|\frac{1}{|A^{\mathbf{T}}||A|}|A^{\mathbf{T}}| = 1 $$

30. (Calculus question) Show that the partial derivatives of $\ln(\det A)$ give
    $A^{-1}$!

$$ f(a, b, c, d) = \ln(ad - bc) \quad \text{leads to} \quad
\left[\begin{array}{cc}
\frac{\partial f}{\partial a} & \frac{\partial f}{\partial c} \\
\frac{\partial f}{\partial b} & \frac{\partial f}{\partial d} \\
\end{array}\right] = A^{-1}
$$

31. Omitted (no MATLAB).

32. Omitted (no MATLAB).

33. Omitted (no MATLAB).

34. If you know that $\det A = 6$, what is the determinant of $B$?

$$ \text{From }
\det A =
\begin{vmatrix}
\text{row } 1 \\
\text{row } 2 \\
\text{row } 3 \\
\end{vmatrix} = 6 \text{ find } \det B =
\begin{vmatrix}
\text{row } 3 + \text{row } 2 + \text{row } 1 \\
\text{row } 2 + \text{row } 1 \\
\text{row } 1 \\
\end{vmatrix}
$$
