# Chapter 2

---

## Problem Set 2.1

Page 52

**Problems 1-8 are about the row and column pictures of $Ax = b$.**

1. With $A = I$ (the identity matrix) draw the planes in the row picture. Three
   sides of a box meet at the solution $x = (x, y, z) = (2, 3, 4)$:

$$
1x + 0y + 0z = 2 \\
0x + 1y + 0z = 3 \\
0x + 0y + 1z = 4 \\
$$

or

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}2\\3\\4\end{bmatrix}
$$

Draw the vectors in the column picture. Two times column 1 plus three times
column 2 plus four times column 3 equals the right side $b$.

2. If the equations in Problem 1 are multiplied by $2, 3, 4$ they become
   $DX = B$:

$$
2x + 0y + 0z = 4 \\
0x + 3y + 0z = 0 \\
0x + 0y + 4z = 16 \\
$$

or

$$
DX =
\left[\begin{array}{ccc}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & 4 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}4\\9\\16\end{bmatrix} = B
$$

Why is the row picture the same? Is the solution $X$ the same as $x$? What is
changed in the column picture - the columns or the right combination to give
$B$?

3. If equation 1 is added to equation 2, which of these are changed: the planes
   in the row picture, the vectors in the column picture, the coefficient
   matrix, the solution? The new equations in Problem 1 would be $x = 2$,
   $x + y = 5$, $z = 4$.

4. Find a point with $z = 2$ on the intersection line of the planes
   $x + y  + 3z = 6$ and $x - y + z = 4$. Find the point with $z = 0$. Find a
   third point halfway between.

5. The first of these equations plus the second equals the third:

$$
x + y + z = 2 \\
x + 2y + z = 3 \\
2x + 3y + 2z = 5
$$

The first two planes meet along a line. The third plane contains that line,
because if $x, y, z$ satisfy the first two equations then they also ____. The
equations have infinitely many solutions (the whole line $\mathbf{L}$). Find
three solutions on $\mathbf{L}$.

6. Move the third plane in Problem 5 to a parallel plane $2x + 3y + 2z = 9$. Now
   the three equations have no solution - _why not_? The first two planes meet
   along the line $\mathbf{L}$, but the third plane doesn't ____ that line.

7. In Problem 5 the columns are $(1, 1, 2)$ and $(1, 2, 3)$ and $(1, 1, 2)$.
   This is a "singular case" because the third column is ____. Find two
   combinations of the columns that give $b = (2, 3, 5)$. This is only possible
   for $b = (4, 6, c)$ if $c =$ ____.

8. Normally 4 "planes" in 4-dimensional space meet at a ____. Normally 4 column
   vectors in 4-dimensional space can combine to produce $b$. What combination
   of $(1, 0, 0, 0), (1, 1, 0, 0), (1, 1, 1, 0), (1, 1, 1, 1)$ produces
   $b = (3, 3, 3, 2)$? What 4 equations for $x, y, z, t$ are you solving?

**Problems 9-14 are about multiplying matrices and vectors.**

9. Compute each $Ax$ by dot products of the rows with the column vector:

a.

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
-2 & 3 & 1 \\
-4 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}2\\2\\3\end{bmatrix}
$$

b.

$$
\left[\begin{array}{cccc}
2 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 \\
0 & 1 & 2 & 1 \\
0 & 0 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\2\end{bmatrix}
$$

10. Compute each $Ax$ in Problem 9 as a combination of the columns:

9(a) becomes

$$ Ax = 2\begin{bmatrix}{}1\\-2\\-4\end{bmatrix} + 2\begin{bmatrix}{}2\\3\\1\end{bmatrix} + 3\begin{bmatrix}{}4\\1\\2\end{bmatrix} = \begin{bmatrix}{}\\\end{bmatrix}$$

How many separate multiplications for $Ax$, when the matrix is "3 by 3"?

11. Find the two components of $Ax$ by rows or by columns:

$$
\left[\begin{array}{cc}
2 & 3 \\
5 & 1 \\
\end{array}\right]
\begin{bmatrix}{}4\\2\end{bmatrix}
$$

and

$$
\left[\begin{array}{cc}
3 & 6 \\
6 & 12 \\
\end{array}\right]
\begin{bmatrix}{}2\\-1\end{bmatrix}
$$

and

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
2 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\1\\1\end{bmatrix}
$$

12. Multiply $A$ times $x$ to find three components of $Ax$:

$$
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix}
$$

and

$$
\left[\begin{array}{ccc}
2 & 1 & 3 \\
1 & 2 & 3 \\
3 & 3 & 6 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\-1\end{bmatrix}
$$

and

$$
\left[\begin{array}{cc}
2 & 1 \\
1 & 2 \\
3 & 3 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\end{bmatrix}
$$

13.

a. A matrix with $m$ rows and $n$ columns multiplies a vector with ____
components to produce a vector with ____ components.

b. The planes from the $m$ equations $Ax = b$ are in ____-dimensional space. The
combination of the columns of $A$ is in ____-dimensional space.

14. Write $2x + 3y + z + 5t = 8$ as a matrix $A$ (how many rows?) multiplying
    the column vector $x = (x, y, z, t)$ to produce $b$. The solutions $x$ fill
    a plane or "hyperplane" in 4-dimensional space. _The plane is
    $3$-dimensional with no $4D$ volume_.

**Problems 15-22 ask for matrices that act in special ways on vectors.**

15.

a. What is the $2$ by $2$ identity matrix? $I$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ equals
$\begin{bmatrix}{}x\\y\end{bmatrix}$.

b. What is the $2$ by $2$ exchange matrix? $P$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ equals
$\begin{bmatrix}{}y\\x\end{bmatrix}$.

16.

a. What $2$ by $2$ matrix $R$ rotates every vector by $90\degree$? $R$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ is $\begin{bmatrix}{}y\\-x\end{bmatrix}$.

b. What $2$ by $2$ matrix $R^2$ rotates every vector by $180\degree$?

17. Find the matrix $P$ that multiplies $(x, y, z)$ to give $(y, z, x)$. Find
    the matrix $Q$ that multiplies $(y, z, x)$ to bring back $(x, y, z)$.

18. What $2$ by $2$ matrix $E$ subtracts the first component from the second
    component? What $3$ by $3$ matrix does the same?

$$ E\begin{bmatrix}{}3\\5\end{bmatrix} = \begin{bmatrix}{}3\\2\end{bmatrix} $$

and

$$ E\begin{bmatrix}{}3\\5\\7\end{bmatrix} = \begin{bmatrix}{}3\\5\\7\end{bmatrix} $$

19. What $3$ by $3$ matrix $E$ multiplies $(x, y, z)$ to give $(x, y, z + x)$?
    What matrix $E^{-1}$ multiplies $(x, y, z)$ to give $(x, y, z - x)$? If you
    multiply $(3, 4, 5)$ by $E$ and then multiply $E^{-1}$, the two results are
    ____ and ____.

20. What $2$ by $2$ matrix $P_1$ projects the vector $(x, y)$ onto the $x$ axis
    to produce $(x, 0)$? What matrix $P_2$ projects onto the $y$ axis to produce
    $(0, y)$? If you multiply $(5, 7)$ by $P_1$ and then multiply by $P_2$, you
    get ____ and ____.

21. What $2$ by $2$ matrix $R$ rotates every vector through $45\degree$? The
    vector $(1, 0)$ goes to
    $\left(\dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2}\right)$. The vector $(0, 1)$
    goes to $\left(-\dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2}\right)$. Those
    determine the matrix. Draw these particular vectors in the $xy$ plane and
    find $R$.

22. Write the dot product of $(1, 4, 5)$ and $(x, y, z)$ as a matrix
    multiplication $Ax$. The matrix $A$ has one row. The solutions to
    $Ax = \mathbf{0}$ lie on a ____ perpendicular to the vector ____. The
    columns of $A$ are only in ____-dimensional space.

23. Omitted (no MATLAB).

24. Omitted (no MATLAB).

25. Omitted (no MATLAB).

**Questions 26-28 review the row and column pictures in 2, 3, and 4
dimensions.**

26. Draw the row and column pictures for the equations $x - 2y = 0$,
    $x + y = 6$.

27. For two linear equations in three unknowns $x, y, z$, the row picture will
    show (2 or 3) (lines or planes) in (2 or 3)-dimensional space. The column
    picture is in (2 or 3)-dimensional space. The solutions normally lie on a
    ____.

28. For four linear equations in two unknowns $x$ and $y$, the row picture shows
    four ____. The column picture is in ____-dimensional space. The equations
    have no solution unless the vector on the right side is a combination of
    ____.

29. Start with the vector $u_0 = (1, 0)$. Multiply again and again by the same
    "Markov matrix" $A= [.8 .3; .2 .7]$. The next three vectors are
    $u_1, u_2, u_3$:

$$
u_1 =
\left[\begin{array}{cc}
.8 & .3 \\
.2 & .7 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\end{bmatrix} =
\begin{bmatrix}{}.8\\.2\end{bmatrix}
$$

$u_2 = Au_1 =$ ____

$u_3 = Au_2 =$ ____

What property do you notice for all four vectors $u_0, u_1, u_2, u_3$?
