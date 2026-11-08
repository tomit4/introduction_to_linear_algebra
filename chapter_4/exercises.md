Page 213

## Problem Set 4.1

**Questions 1-12 grow out of Figures 4.2 and 4.3 with four subspaces.**

1. Construct any 2 by 3 matrix of rank one. Copy Figure 4.2 and put one vector
   in each subspace (and put two in the nullspace). Which vectors are
   orthogonal?

2. Redraw Figure 4.3 for a $3$ by $2$ matrix of rank $r = 2$. Which subspace is
   $\Z$ (zero vector only)? The nullspace part of any vector $x$ in $\R^2$ is
   $x_n =$ ____.

3. Construct a matrix with the required property or say why that is impossible:

a. Column space contains $\begin{bmatrix}{}1\\2\\-3\end{bmatrix}$ and
$\begin{bmatrix}{}2\\-3\\5\end{bmatrix}$, nullspace contains
$\begin{bmatrix}{}1\\1\\1\end{bmatrix}$

b. Row space contains $\begin{bmatrix}{}1\\2\\-3\end{bmatrix}$ and
$\begin{bmatrix}{}2\\-3\\5\end{bmatrix}$, nullspace contains
$\begin{bmatrix}{}1\\1\\1\end{bmatrix}$

c. $Ax = \begin{bmatrix}{}1\\1\\1\end{bmatrix}$ has a solution and
$A^{\mathbf{T}}\begin{bmatrix}{}1\\0\\0\end{bmatrix} = \begin{bmatrix}{}0\\0\\0\end{bmatrix}$

d. Every row is orthogonal to every column ($A$ is not the zero matrix)

e. Columns add up to a column of zeros, rows add to a row of $1$'s.

4. If $AB = 0$ then the columns of $B$ are in the ____ of $A$. The rows of $A$
   are in the ____ of $B$. With $AB = 0$, why can't $A$ and $B$ be $3$ by $3$
   matrices of rank $2$?

5.

a. If $Ax = b$ has a solution and $A^{\mathbf{T}}y = \mathbf{0}$, _is_
($y^{\mathbf{T}}x = 0$) _or_ ($y^{\mathbf{T}}b = 0$)?

b. If $A^{\mathbf{T}}y = (1, 1, 1)$ has a solution and $Ax = \mathbf{0}$, then
____.

6. This system of equations $Ax = b$ has _no solution_ (they lead to $0 = 1$):

$$
x + 2y + 2z = 5 \\
2x + 2y + 3z = 5 \\
3x + 4y + 5z = 9 \\
$$

Find numbers $y_1, y_2, y_3$ to multiply the equations so they add to $0 = 1$.
You have found a vector $y$ in which subspace? Its dot product $y^{\mathbf{T}}b$
is $1$, so no solution $x$.

7. Every system with no solution is like the one in Problem 6. There are numbers
   $y_1, \dots, y_m$ that multiply the $m$ equations so they add up to $0 = 1$.
   This is called **Fredholm's Alternative**:

**Exactly one of these problems has a solution**

$$ Ax = b \quad \textbf{OR} \quad A^{\mathbf{T}}y = \mathbf{0} \text{ with } y^{\mathbf{T}}b = 1 $$

If $b$ is not in the column space of $A$, it is not orthogonal to the nullspace
of $A^{\mathbf{T}}$. Multiply the equations $x_1 - x_2 = 1$ and $x_2 - x_3 = 1$
and $x_1 - x_3 = 1$ by the numbers $y_1, y_2, y_3$ chosen so that the equations
add up to $0 = 1$.

8. In Figure 4.3, how do we know that $Ax_r$ is equal to $Ax$? How do we know
   that this vector is in the column space? If
   $A = \left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$ and
   $x = \begin{bmatrix}{}1\\0\end{bmatrix}$ what is $x_r$?

9. If $A^{\mathbf{T}}Ax = \mathbf{0}$ then $Ax = \mathbf{0}$. Reason: $Ax$ is
   the nullspace of $A^{\mathbf{T}}$ and also in the ____ of $A$ and those
   spaces are ____. _Conclusion:_ $A^{\mathbf{T}}A$ _has the same nullspace as
   $A$. This key fact is repeated in the next section._

10. Suppose $A$ is a symmetric matrix ($A^{\mathbf{T}} = A$).

a. Why is its column space perpendicular to its nullspace?

b. If $Ax = \mathbf{0}$ and $Az = 5z$, which subspaces contain these
"eigenvectors" $x$ and $z$? **Symmetric matrices have perpendicular eigenvectors
$x^{\mathbf{T}}z = 0$.**

11. (Recommended) Draw Figure 4.2 to show each subspace correctly for

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
3 & 6 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right]
$$

12. Find the pieces $x_r$ and $x_n$ and draw Figure 4.3 properly if

$$ A =
\left[\begin{array}{cc}
1 & -1 \\
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

and

$$ x =
\begin{bmatrix}{}2\\0\end{bmatrix}
$$

**Questions 13-23 are about orthogonal subspaces.**

13. Put bases for the subspaces $V$ and $W$ into the columns of matrices $V$ an
    $W$. Explain why the test for orthogonal subspaces an be written
    $V^{\mathbf{T}}W =$ zero matrix. This matches $v^{\mathbf{T}}w = 0$ for
    orthogonal vectors.

14. The floor $V$ and the wall $W$ are not orthogonal subspaces, because they
    share a nonzero vector (along the line where they meet). No planes $V$ and
    $W$ in $\R^3$ can be orthogonal! Find a vector in the column spaces of both
    matrices:

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
1 & 3 \\
1 & 2 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
5 & 4 \\
6 & 3 \\
5 & 1 \\
\end{array}\right]
$$

This will be a vector $Ax$ and also $B\hat{x}$. Think $3$ by $4$ with the matrix
$\left[\begin{array}{cc}A & B \\\end{array}\right]$.

15. Extend Problem 14 to a $p$-dimensional subspace $V$ and a $q$-dimensional
    subspace $W$ of $\R^n$. What inequality on $p + q$ guarantees that $V$
    intersects $W$ in a nonzero vector? These subspaces cannot be orthogonal.

16. Prove that every $y$ in $N(A^{\mathbf{T}})$ is perpendicular to every $Ax$
    in the column space, using the matrix shorthand of equation (2). Start from
    $A^{\mathbf{T}}y = \mathbf{0}$.

17. If $S$ is the subspace of $\R^3$ containing only the zero vector, what is
    $S^{\perp}$? If $S$ is spanned by $(1, 1, 1)$, what is $S^{\perp}$? IF $S$
    is spanned by $(1, 1, 1)$ and $(1, 1, -1)$, what is a basis for $S^{\perp}$?

18. Suppose $S$ only contains two vectors $(1, 5, 1)$ and $(2, 2, 2)$ (not a
    subspace). Then $S^{\perp}$ is the nullspace of a matrix $A =$ ____.
    $S^{\perp}$ is a subspace even if $S$ is not.

19. Suppose $L$ is a one-dimensional subspace (a line) in $\R^3$. Its orthogonal
    complement $L^{\perp}$ is the ____ perpendicular to $L$. Then
    $(L^{\perp})^{\perp}$ is a ____ perpendicular to $L^{\perp}$. In fact
    $(L^{\perp})^{\perp}$ is the same as ____.

20. Suppose $V$ is the whole space $\R^4$. Then $V^{\perp}$ contains only the
    vector ____. Then $(V^{\perp})^{\perp}$ is ____. So $(V^{\perp})^{\perp}$ is
    the same as ____.

21. Suppose $S$ is spanned by the vectors $(1, 2, 2, 3)$ and $(1, 3, 3, 2)$.
    Find two vectors that span $S^{\perp}$. This is the same as solving
    $Ax = \mathbf{0}$ for which $A$?

22. If $P$ is the plane of vectors in $\R^4$ satisfying
    $x_1 + x_2 + x_3 + x_4 = 0$, write a basis for $P^{\perp}$. Construct a
    matrix that has $P$ as its nullspace.

23. If a subspace $S$ is contained in a subspace $V$, prove that $S^{\perp}$
    contains $V^{\perp}$.

**Questions 24-30 are about perpendicular columns and rows.**

24. Suppose an $n$ by $n$ matrix is invertible: $AA^{-1} = I$. Then the first
    column of $A^{-1}$ is orthogonal to the space spanned by which rows of $A$?

25. Find $A^{\mathbf{T}}A$ if the columns of $A$ are unit vectors, all mutually
    perpendicular.

26. Construct a $3$ by $3$ matrix $A$ with no zero entries whose columns are
    mutually perpendicular. Compute $A^{\mathbf{T}}A$. Why is it a diagonal
    matrix?

27. The lines $3x + y = b_1$ and $6x + 2y = b_2$ are ____. They are the same
    line if ____. In that case $(b_1, b_2)$ is perpendicular to the vector ____.
    The nullspace of the matrix is the line $3x + y =$ ____. One particular
    vector in that nullspace is ____.

28. Why is each of these statements false?

a. $(1, 1, 1)$ is perpendicular to $(1, 1, -2)$ so the planes $x + y + z = 0$
and $x + y - 2z = 0$ are orthogonal subspaces.

b. The subspace spanned by $(1, 1, 0, 0, 0)$ and $(0, 0, 0, 1, 1)$ is the
orthogonal complement of the subspace spanned by $(1, -1, 0, 0, 0)$ and
$(2, -2, 3, 4, -4)$.

c. Two subspaces that meet only in the zero vector are orthogonal.

29. Find a matrix with $v = (1, 2, 3)$ in the row space and the column space.
    Find another matrix with $v$ in the nullspace and column space. Which pairs
    of subspaces can $v$ _not_ be in?
