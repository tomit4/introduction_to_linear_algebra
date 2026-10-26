Page 142

## Problem Set 3.1

**The first problems 1-8 are about vector spaces in general. The vectors in
those spaces are not necessarily column vectors. In the definition of a _vector
space_, vector addition $x + y$ and scalar multiplication $cx$ must obey the
following eight rules:**

(1) $x + y = y + x$

(2) $x + (y + z) = (x + y) + z$

(3) There is a unique "zero vector" such that $x + \mathbf{0} = x$ for all $x$.

(4) For each $x$ there is a unique vector $-x$ such that $x + (-x) = \mathbf{0}$

(5) $1$ times $x$ equals $x$

(6) $(c_1c_2)x = c_1(c_2x)$

(7) $c(x + y) = cx + cy$

(8) $(c_1 + c_2)x = c_1x + c_2x$

1. Suppose $(x_1, x_2) + (y_1, y_2)$ is defined to be $(x_1 + y_2, x_2 + y_1)$.
   With the usual multiplication $cx = (cx_1, cx_2)$, which of the eight
   conditions are not satisfied?

2. Suppose the multiplication $cx$ is defined to produce $(cx_1, 0)$ instead of
   $(cx_1, cx_2)$. With the usual addition in $\mathbf{R}^2$, are the eight
   conditions satisfied?

3.

a. Which rules are broken if we keep only the positive numbers $x > 0$ in
$\mathbf{R}^1$? Every $c$ must be allowed. The half-line is not a subspace.

b. The positive numbers with $x + y$ and $cx$ redefined to equal the usual $xy$
and $x^c$ _do_ satisfy the eight rules. Test rule 7 when $c = 3, x = 2, y = 1$.
(Then $x + y = 2$ and $cx = 8$.) Which number acts as the "zero vector"?

4. The matrix $A = \left[\begin{array}{cc}2 & -2 \\2 & -2 \\\end{array}\right]$
   is a "vector" in the space $\mathbf{M}$ of all 2 by 2 matrices. Write down
   the zero vector in this space, the vector $\dfrac{1}{2}A$, and the vector
   $-A$. What matrices are in the smallest subspace containing $A$?

5.

a. Describe a subspace of $\mathbf{M}$ that contains
$A = \left[\begin{array}{cc}1 & 0\\0 & 0\\\end{array}\right]$ but not
$B = \left[\begin{array}{cc}0 & 0\\0 & -1\\\end{array}\right]$.

b. If a subspace of $\mathbf{M}$ does not contain $A$ and $B$, must it contain
$I$?

c. Describe a subspace of $\mathbf{M}$ that contains no nonzero diagonal
matrices.

6. The functions $f(x) = x^2$ and $g(x) = 5x$ are "vectors" in $\mathbf{F}$.
   This is the vector of all real functions. (The functions are defined for
   $-\infty < x < \infty$.) The combination $3f(x) - 4g(x)$ is the function
   $h(x) =$ _ __.

7. Which rule is broken if multiplying $f(x)$ by $c$ gives the function $f(cx)$?
   Keep the usual addition $f(x) + g(x)$.

8. If the sum of the "vectors" $f(x)$ and $g(x)$ is defined to be the function
   $f(g(x))$, then the "zero vector" is $g(x) = x$. Keep the usual scalar
   multiplication $cf(x)$ and find two rules that are broken.

**Questions 9-18 are about the "subspace requirements": $x + y$ and $cx$ (and
then all linear combinations $cx + dy$) stay in the subspace.**

9. One requirement can be met while the other fails. Show this by finding

a. A set of vectors in $\mathbf{R}^2$ for which $x + y$ stays in the set but
$\dfrac{1}{2}x$ may be outside.

b. A set of vectors $\mathbf{R}^2$ (other than two quarter-planes) for which
every $cx$ stays in the set but $x + y$ may be outside.

10. Which of the following subsets of $\mathbf{R}^3$ are actually subspaces?

a. The plane of vectors $(b_1, b_2, b_3)$ with $b_1 = b_2$.

b. The plane of vectors with $b_1 = 1$.

c. The vectors with $b_1b_2b_3 = 0$.

d. All linear combinations of $v = (1, 4, 0)$ and $w = (2, 2, 2)$.

e. All vectors that satisfy $b_1 + b_2 + b_3 = 0$.

f. All vectors with $b_1 \leq b_2 \leq b_3$.

11. Describe the smallest subspace of the matrix space $\mathbf{M}$ that
    contains

a.

$$
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

and

$$
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

b.

$$
\left[\begin{array}{cc}
1 & 1 \\
0 & 0 \\
\end{array}\right]
$$

c.

$$
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

and

$$
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

12. Let $P$ be the plane in $\mathbf{R}^3$ with equation $x + y - 2z = 4$. The
    origin $(0, 0, 0)$ is not in $P$! Find two vectors in $P$ and check that
    their sum is not in $P$.

13. Let $\mathbf{P}_0$ be the plane through $(0, 0, 0)$ parallel to the previous
    plane $P$. What is the equation for $\mathbf{P}_0$? Find two vectors in
    $\mathbf{P}_0$ and check that their sum is in $\mathbf{P}_0$.

14. The subspaces of $\mathbf{R}^3$ are planes, lines, $\mathbf{R}^3$ itself, or
    $\mathbf{Z}$ containing only $(0, 0, 0)$.

a. Describe the three types of subspaces of $\mathbf{R}^2$.

b. Describe all subspaces of $\mathbf{D}$, the space of 2 by 2 diagonal
matrices.

15.

a. The intersection of two planes through $(0, 0, 0)$ is probably a ____ in
$\mathbf{R}^3$ but it could be a ____. It can't be $\mathbf{Z}$!

b. The intersection of a plane through $(0, 0, 0)$ with a line through
$(0, 0, 0)$ is probably a ____ but it could be a ____.

c. If $\mathbf{S}$ and $\mathbf{T}$ are subspaces of $\mathbf{R}^5$, prove that
their intersection $\mathbf{S} \cap \mathbf{T}$ is a subspace of $\mathbf{R}^5$.
Here $\mathbf{S} \cap \mathbf{T}$ consists of the vectors that lie in both
subspaces. _Check that $x + y$ and $cx$ are in $\mathbf{S} \cap \mathbf{T}$ if
$x$ and $y$ are in both spaces._

16. Suppose $\mathbf{P}$ is a plane through $(0, 0, 0)$ and $\mathbf{L}$ is a
    line through $(0, 0, 0)$. The smallest vector space containing both
    $\mathbf{P}$ and $\mathbf{L}$ is either ____ or ____.

17.

a. Show that the set of _invertible_ matrices in $\mathbf{M}$ is not a subspace.

b. Show that the set of _singular_ matrices in $\mathbf{M}$ is not a subspace.

18. True or false (check addition in each case by an example):

a. The symmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} = A$) form a
subspace.

b. The skew-symmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} = -A$) form
a subspace.

c. The unsymmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} \neq A$) form
a subspace.

**Questions 19-27 are about column spaces $C(A)$ and the equation $Ax = b$.**

19. Describe the column spaces (lines or planes) of these particular matrices:

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 2 \\
0 & 0 \\
\end{array}\right]
$$

and

$$ C =
\left[\begin{array}{cc}
1 & 0 \\
2 & 0 \\
0 & 0 \\
\end{array}\right]
$$

20. For which right sides (find a condition on $b_1, b_2, b_3$) are these
    systems solvable?

a.

$$
\left[\begin{array}{rrr}
1 & 4 & 2 \\
2 & 8 & 4 \\
-1 & -4 & -2 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

b.

$$
\left[\begin{array}{rr}
1 & 4 \\
2 & 9 \\
-1 & -4 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

21. Adding row 1 of $A$ to row 2 produces $B$. Adding column 1 to column 2
    produces $C$. A combination of the columns of ($B$ or $C$?) is also a
    combination of the columns of $A$. Which two matrices have the same column
    ____?

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
1 & 2 \\
3 & 6 \\
\end{array}\right]
$$

and

$$ C =
\left[\begin{array}{cc}
1 & 3 \\
2 & 6 \\
\end{array}\right]
$$

22. For which vectors $(b_1, b_2, b_3)$ do these systems have a solution?

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

and

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

and

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

23. (Recommended) If we add an extra column $b$ to a matrix $A$, then the column
    space gets larger unless ____. Give an example where the column space gets
    larger and an example where it doesn't. Why is $Ax = b$ solvable exactly
    when the column space _doesn't_ get larger - it is the same for $A$ and
    $\left[\begin{array}{cc}A & b\\\end{array}\right]$?

24. The column of $AB$ are combinations of the columns of $A$. This means: _The
    column space of $AB$ is contained in_ (possible equal to) _the column space
    of_ $A$. Give an example where the column spaces of $A$ and $AB$ are not
    equal.

25. Suppose $Ax = b$ and $Ay = b^*$ are both solvable. Then $Az = b + b^*$ is
    solvable. What is $z$? This translates into: If $b$ and $b^*$ are in the
    column space $C(A)$, _then_ $b + b^*$ is in $C(A)$.

26. If $A$ is any 5 by 5 invertible matrix, then its column space is ____. Why?

27. True or false (with a counterexample if false):

a. The vectors $b$ that are not in the column space $C(A)$ form a subspace.

b. If $C(A)$ contains only the zero vector, then $A$ is the zero matrix.

c. The column space of $2A$ equals the column space of $A$.

d. The column space of $A -I$ equals the column space of $A$ (test this).

28. Construct a 3 by 3 matrix whose column space contains $(1, 1< 0)$ and
    $(1, 0, 1)$ but not $(1, 1, 1)$. Construct a 3 by 3 matrix whose column
    space is only a line.

29. If the 9 by 12 system $Ax = b$ is solvable for every $b$, then $C(A) =$
    ____.
