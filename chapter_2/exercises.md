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

_Solution:_

(Done by hand.)

_Note on drawing 3D vectors:_

When drawing 3D vectors, always draw as if the main axes (_i.e._ $x, y, z$) are
the back corner of a cube. From there, take your $x$ value and simply find it as
you would on a 2D Cartesian graph, then find $y$ on the $y$ axis. Now visualize
moving across the $y$ axes from your point on the $x$ axes the amount of $y$
units, this should feel (if the units are positive) like you are traversing the
bottom side of a cube.

From there, then go "up" in space $z$ units (along the $z$-axis), again
visualize as if you are now traversing up those units inside the cube. Plot that
point. Then, from the origin $(0, 0, 0)$, draw a line with an arrow pointing at
the point you just reached. This is the graphical representation of your vector
in 3-dimensional space.

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

_Solution:_

This is because when solved for $x, y, z$, the solution is the same:

$$
2x = 4 \Rightarrow x = 2 \\
3y = 9 \Rightarrow y = 3 \\
4z = 16 \Rightarrow z = 4 \\
$$

The three column vectors are changed, as they are scaled by $2, 3, 4$
respectively, but result in the same linear combination.

3. If equation 1 is added to equation 2, which of these are changed: the planes
   in the row picture, the vectors in the column picture, the coefficient
   matrix, the solution? The new equations in Problem 1 would be $x = 2$,
   $x + y = 5$, $z = 4$.

_Solution:_

The new matrix would be expressed as:

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}2\\5\\4\end{bmatrix}
$$

The planes changed since now the second row is $x + y = 5$, while the solution
for $y$ still crosses through $y = 3$ (since $x = 2$), it is now dependent on
$x$ and thus tilts along the $x$-axis. The vectors in the column picture do not
change since the solution itself is the same (as just explained). The
coefficient matrix has obviously changed by observation, there is now a $1$ in
the coefficient matrix for the $x$ column in the second row. As explained
earlier, the solution has not changed.

4. Find a point with $z = 2$ on the intersection line of the planes
   $x + y  + 3z = 6$ and $x - y + z = 4$. Find the point with $z = 0$. Find a
   third point halfway between.

_Solution:_

$$
\left[\begin{array}{cc}
1 & 1 & 3 \\
1 & -1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}6\\4\end{bmatrix}
$$

_Find a point with $z = 2$:_

Evaluating by rows, this is:

$$
x + y + 3z = 6 \\
x - y + z = 4 \\
$$

Now, if we say that $z = 2$:

$$
x + y + 3(2) = 6 \\
x - y + 2 = 4 \\
$$

$$
x + y + 6 = 6 \\
x - y + 2 = 4 \\
$$

$$
x + y = 0 \\
x - y = 2 \\
$$

Now, solving for $x$ and $y$:

$$
x = -y \\
x - y = 2 \\
$$

So:

$$
x = -y \\
(-y) - y = 2 \\
$$

$$
x = -y \\
-2y = 2 \\
$$

$$
x = -y \\
y = -1 \\
$$

$$
x = 1 \\
y = -1 \\
$$

So the point found when $z = 2$ is $(1, -1, 2)$.

_Now to solve when $z = 0$, a similar approach is applied:_

$$
x + y + 3z = 6 \\
x - y + z = 4 \\
$$

$$
x + y + 3(0) = 6 \\
x - y + (0) = 4 \\
$$

$$
x + y = 6 \\
x - y = 4 \\
$$

Now solve for $x$ and $y$:

$$
x = 6 - y \\
x - y = 4 \\
$$

So:

$$
x = 6 - y \\
(6 - y) - y = 4 \\
$$

$$
x = 6 - y \\
6 - 2y = 4 \\
$$

$$
x = 6 - y \\
-2y = -2 \\
$$

$$
x = 6 - y \\
y = 1 \\
$$

Then:

$$
x = 6 - (1) \\
y = 1 \\
$$

$$
x = 5 \\
y = 1 \\
$$

So the point with $z = 0$ is $(5, 1, 0)$.

_Now to find a third point halfway between them:_

To find a point halfway between $(1, -1, 2)$ and $(5, 1, 0)$, we can simply add
each $x$, each $y$, and each $z$ respectively, then divide by $2$. This is akin
to adding a fractional scalar to the sum of the two points which we know both
lie on the same plane.

$$ \left(\frac{1 + 5}{2}, \frac{-1 + 1}{2}, \frac{2 + 0}{2}\right) $$

$$ \left(\frac{6}{2}, \frac{0}{2}, \frac{2}{2}\right) $$

$$ (3, 2, 1) $$

Ensure this is correct by plugging into both equations:

$$
x + y + 3z = 6 \\
x - y + z = 4
$$

$$
(3) + (0) + 3(1) = 6 \\
(3) - (0) + (1) = 4
$$

$$
6 = 6 \\
4 = 4
$$

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

_Solution:_

_If $x, y, z$ satisfy the first two equations then they also?:_

Satisfy the third equation.

_Find three solutions on $\mathbf{L}$:_

First solution:

$$
x + y + z = 2 \\
x + 2y + z = 3 \\
$$

Choose $x = 0$, then:

$$
0 + y + z = 2 \\
0 + 2y + z = 3 \\
$$

$$
y + z = 2 \\
2y + z = 3 \\
$$

Now solve for $y, z$:

$$
y = 2 - z \\
2(2 - z) + z = 3 \\
$$

$$
y = 2 - z \\
4 - 2z + z = 3 \\
$$

$$
y = 2 - z \\
4 - z = 3 \\
$$

$$
y = 2 - z \\
-z = 3 - 4 \\
$$

$$
y = 2 - z \\
-z = -1 \\
$$

$$
y = 2 - (1) \\
z = 1 \\
$$

$$
y = 1 \\
z = 1 \\
$$

So one solution is $(0, 1, 1)$.

Second solution:

$$
x + y + z = 2 \\
x + 2y + z = 3 \\
$$

Choose $x = 1$, then:

$$
(1) + y + z = 2 \\
(1) + 2y + z = 3 \\
$$

$$
y + z = 1 \\
2y + z = 2 \\
$$

$$
y = 1 - z \\
2(1 - z) + z = 2 \\
$$

$$
y = 1 - z \\
2 - 2z + z = 2 \\
$$

$$
y = 1 - z \\
2 - z = 2 \\
$$

$$
y = 1 - z \\
-z = 0 \\
$$

$$
y = 1 - (0) \\
z = 0 \\
$$

$$
y = 1 \\
z = 0 \\
$$

So another solution is $(1, 1, 0)$.

Third solution:

$$
x + y + z = 2 \\
x + 2y + z = 3 \\
$$

Choose $x = 2$, then:

$$
(2) + y + z = 2 \\
(2) + 2y + z = 3 \\
$$

$$
y + z = 0 \\
2y + z = 1 \\
$$

$$
y = -z \\
2(-z) + z = 1 \\
$$

$$
y = -z \\
-2z + z = 1 \\
$$

$$
y = -z \\
-z = 1 \\
$$

$$
y = -(-1) \\
z = -1 \\
$$

$$
y = 1 \\
z = -1 \\
$$

So a third solution is $(2, 1, -1)$.

6. Move the third plane in Problem 5 to a parallel plane $2x + 3y + 2z = 9$. Now
   the three equations have no solution - _why not_? The first two planes meet
   along the line $\mathbf{L}$, but the third plane doesn't ____ that line.

_Why not?:_

Because every point on $\mathbf{L}$ satisfies the first two equations, it
follows that every point on their their sum, _i.e._ $2x + 3y + 2z = 5$ is also
satisfied by $\mathbf{L}$, but when a parallel plane of the third equation is
drawn, $2x + 3y + 2z = 9$, the points along this new plane no longer satisfy the
same values of $x, y, z$ that define $\mathbf{L}$.

_Doesn't?:_

contain

7. In Problem 5 the columns are $(1, 1, 2)$ and $(1, 2, 3)$ and $(1, 1, 2)$.
   This is a "singular case" because the third column is ____. Find two
   combinations of the columns that give $b = (2, 3, 5)$. This is only possible
   for $b = (4, 6, c)$ if $c =$ ____.

_The third column is?:_

The same as the first (or, more succinctly, a scalar multiple of the first).

_Find two combinations of the columns that give $b = (2, 3, 5)$:_

The column representation of the equations in problem 5 are:

$$ x\begin{bmatrix}{}1\\1\\2\end{bmatrix} + y\begin{bmatrix}{}1\\2\\3\end{bmatrix} + z\begin{bmatrix}{}1\\1\\2\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

We can use one of our solutions for $x, y, z$ from problem 5, let's use
$(0, 1, 1)$:

$$ 0\begin{bmatrix}{}1\\1\\2\end{bmatrix} + 1\begin{bmatrix}{}1\\2\\3\end{bmatrix} + 1\begin{bmatrix}{}1\\1\\2\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}0\\0\\0\end{bmatrix} + \begin{bmatrix}{}1\\2\\3\end{bmatrix} + \begin{bmatrix}{}1\\1\\2\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}1 + 1\\2 + 1\\3 + 2\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}2\\3\\5\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

Now let's use $(1, 1, 0)$:

$$ 1\begin{bmatrix}{}1\\1\\2\end{bmatrix} + 1\begin{bmatrix}{}1\\2\\3\end{bmatrix} + 0\begin{bmatrix}{}1\\1\\2\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}1\\1\\2\end{bmatrix} + \begin{bmatrix}{}1\\2\\3\end{bmatrix} + \begin{bmatrix}{}0\\0\\0\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}1 + 1\\1 + 2\\2 + 3\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

$$ \begin{bmatrix}{}2\\3\\5\end{bmatrix} = \begin{bmatrix}{}2\\3\\5\end{bmatrix} = b $$

_This is only possible for $b = (4, 6, c)$ if $c =$?:_

$$ c = 5 \cdot 2 = 10 $$

Since $2 \cdot 2 = 4$ and $3 \cdot 2 = 6$.

8. Normally 4 "planes" in 4-dimensional space meet at a ____. Normally 4 column
   vectors in 4-dimensional space can combine to produce $b$. What combination
   of $(1, 0, 0, 0), (1, 1, 0, 0), (1, 1, 1, 0), (1, 1, 1, 1)$ produces
   $b = (3, 3, 3, 2)$? What 4 equations for $x, y, z, t$ are you solving?

_Normally 4 "planes" in 4-dimensional space meet at a?:_

point

_What combination of $(1, 0, 0, 0), (1, 1, 0, 0), (1, 1, 1, 0), (1, 1, 1, 1)$
produces $b = (3, 3, 3, 2)$?:_

$$
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
1 & 1 & 0 & 0 \\
1 & 1 & 1 & 0 \\
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}3\\3\\3\\2\end{bmatrix} = b
$$

By row:

$$
x = 3 \\
x + y = 3 \\
x + y + z = 3 \\
x + y + z + t = 2 \\
$$

$$
x = 3 \\
(3) + y = 3 \\
(3) + y + z = 3 \\
(3) + y + z + t = 2 \\
$$

$$
x = 3 \\
y = 0 \\
(3) + (0) + z = 3 \\
(3) + (0) + z + t = 2 \\
$$

$$
x = 3 \\
y = 0 \\
z = 0 \\
(3) + (0) + (0) + t = 2 \\
$$

$$
x = 3 \\
y = 0 \\
z = 0 \\
t = -1 \\
$$

Thus the linear combination for $x, y, z, t$ that produces $b = (3, 3, 3, 2)$ is
(in column form):

$$ 3\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} + 0\begin{bmatrix}{}0\\1\\1\\1\end{bmatrix} + 0\begin{bmatrix}{}0\\0\\1\\1\end{bmatrix} + (-1)\begin{bmatrix}{}0\\0\\0\\1\end{bmatrix} = \begin{bmatrix}{}3\\3\\3\\2\end{bmatrix} $$

_What 4 equations for $x, y, z, t$ are you solving?_

$$
x = 3 \\
x + y = 3 \\
x + y + z = 3 \\
x + y + z + t = 2 \\
$$

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

_Solution:_

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
-2 & 3 & 1 \\
-4 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}2\\2\\3\end{bmatrix} =
\begin{bmatrix}{}(1)(2) + (2)(2) + (4)(3)\\(-2)(2) + (3)(2) + (1)(3)\\(-4)(2) + (1)(2) + (2)(3)\end{bmatrix}
$$

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
-2 & 3 & 1 \\
-4 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}2\\2\\3\end{bmatrix} =
\begin{bmatrix}{}2 + 4 + 12\\(-4) + 6 + 3\\(-8) + 2 + 6\end{bmatrix}
$$

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
-2 & 3 & 1 \\
-4 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}2\\2\\3\end{bmatrix} =
\begin{bmatrix}{}18\\5\\0\end{bmatrix}
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

_Solution:_

$$
\left[\begin{array}{cccc}
2 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 \\
0 & 1 & 2 & 1 \\
0 & 0 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\2\end{bmatrix} =
\begin{bmatrix}{}(2)(1) + (1)(1) + (0)(1) + (0)(2)\\(1)(1) + (2)(1) + (1)(1) + (0)(2)\\(0)(1) + (1)(1) + (2)(1) + (1)(2)\\(0)(1) + (0)(1) + (1)(1) + (2)(2)\end{bmatrix}
$$

$$
\left[\begin{array}{cccc}
2 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 \\
0 & 1 & 2 & 1 \\
0 & 0 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\2\end{bmatrix} =
\begin{bmatrix}{}2 + 1\\1 + 2 + 1\\1 + 2 + 2\\1 + 4\end{bmatrix}
$$

$$
\left[\begin{array}{cccc}
2 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 \\
0 & 1 & 2 & 1 \\
0 & 0 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\2\end{bmatrix} =
\begin{bmatrix}{}3\\4\\5\\5\end{bmatrix}
$$

10. Compute each $Ax$ in Problem 9 as a combination of the columns:

9(a) becomes

$$ Ax = 2\begin{bmatrix}{}1\\-2\\-4\end{bmatrix} + 2\begin{bmatrix}{}2\\3\\1\end{bmatrix} + 3\begin{bmatrix}{}4\\1\\2\end{bmatrix} = \begin{bmatrix}{}\\\end{bmatrix}$$

How many separate multiplications for $Ax$, when the matrix is "3 by 3"?

_Solution (1<sup>st</sup> part):_

$$ Ax = 2\begin{bmatrix}{}1\\-2\\-4\end{bmatrix} + 2\begin{bmatrix}{}2\\3\\1\end{bmatrix} + 3\begin{bmatrix}{}4\\1\\2\end{bmatrix} = \begin{bmatrix}{}\\\end{bmatrix}$$

$$ = \begin{bmatrix}{}2\\-4\\-8\end{bmatrix} + \begin{bmatrix}{}4\\6\\2\end{bmatrix} + \begin{bmatrix}{}12\\3\\6\end{bmatrix} $$

$$ \begin{bmatrix}{}2 + 4 + 12\\(-4) + 6 + 3\\(-8) + 2 + 6\end{bmatrix} $$

$$ \begin{bmatrix}{}18\\5\\0\end{bmatrix} $$

_How many separate multiplications for $Ax$, when the matrix is "3 by 3"?_

9 total multiplications.

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

_Solution (1st):_

$$
\left[\begin{array}{cc}
2 & 3 \\
5 & 1 \\
\end{array}\right]
\begin{bmatrix}{}4\\2\end{bmatrix}
$$

By column:

$$ = 4\begin{bmatrix}{}2\\5\end{bmatrix} + 2\begin{bmatrix}{}3\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}4(2)\\4(5)\end{bmatrix} + \begin{bmatrix}{}2(3)\\2(1)\end{bmatrix}$$

$$ = \begin{bmatrix}{}8\\20\end{bmatrix} + \begin{bmatrix}{}6\\2\end{bmatrix}$$

$$ = \begin{bmatrix}{}8 + 6\\20 + 2\end{bmatrix} $$

$$ = \begin{bmatrix}{}14\\22\end{bmatrix} $$

_Solution (2nd):_

$$
\left[\begin{array}{cc}
3 & 6 \\
6 & 12 \\
\end{array}\right]
\begin{bmatrix}{}2\\-1\end{bmatrix}
$$

By column:

$$ 2\begin{bmatrix}{}3\\6\end{bmatrix} + (-1)\begin{bmatrix}{}6\\12\end{bmatrix} $$

$$ \begin{bmatrix}{}2(3)\\2(6)\end{bmatrix} + \begin{bmatrix}{}(-1)6\\(-1)12\end{bmatrix} $$

$$ \begin{bmatrix}{}6\\12\end{bmatrix} + \begin{bmatrix}{}-6\\-12\end{bmatrix} $$

$$ \begin{bmatrix}{}6 + (-6)\\12 + (-12)\end{bmatrix} $$

$$ \begin{bmatrix}{}0\\0\end{bmatrix} $$

_Solution (3rd):_

$$
\left[\begin{array}{ccc}
1 & 2 & 4 \\
2 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\1\\1\end{bmatrix}
$$

By column:

$$ = 3\begin{bmatrix}{}1\\2\end{bmatrix} + 1\begin{bmatrix}{}2\\0\end{bmatrix} + 1\begin{bmatrix}{}4\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}3(1)\\3(2)\end{bmatrix} + \begin{bmatrix}{}1(2)\\1(0)\end{bmatrix} + \begin{bmatrix}{}1(4)\\1(1)\end{bmatrix} $$

$$ = \begin{bmatrix}{}3\\6\end{bmatrix} + \begin{bmatrix}{}2\\0\end{bmatrix} + \begin{bmatrix}{}4\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}3 + 2 + 4\\6 + 0 + 1\end{bmatrix} $$

$$ = \begin{bmatrix}{}9\\7\end{bmatrix} $$

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

_Solution (1st):_

$$
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix}
$$

By column:

$$ = x\begin{bmatrix}{}0\\0\\1\end{bmatrix} + y\begin{bmatrix}{}0\\1\\0\end{bmatrix} + z\begin{bmatrix}{}1\\0\\0\end{bmatrix} $$

$$ = \begin{bmatrix}{}0\\0\\x\end{bmatrix} + \begin{bmatrix}{}0\\y\\0\end{bmatrix} + \begin{bmatrix}{}z\\0\\0\end{bmatrix} $$

$$ = \begin{bmatrix}{}z\\y\\x\end{bmatrix} $$

_Solution (2nd):_

$$
\left[\begin{array}{ccc}
2 & 1 & 3 \\
1 & 2 & 3 \\
3 & 3 & 6 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\-1\end{bmatrix}
$$

By column:

$$ = 1\begin{bmatrix}{}2\\1\\3\end{bmatrix} + 1\begin{bmatrix}{}1\\2\\3\end{bmatrix} + (-1)\begin{bmatrix}{}3\\3\\6\end{bmatrix} $$

$$ = \begin{bmatrix}{}2\\1\\3\end{bmatrix} + \begin{bmatrix}{}1\\2\\3\end{bmatrix} + \begin{bmatrix}{}-3\\-3\\-6\end{bmatrix} $$

$$ = \begin{bmatrix}{}2 + 1 - 3\\1 + 2 - 3\\3 + 3 - 6\end{bmatrix} $$

$$ = \begin{bmatrix}{}0\\0\\0\end{bmatrix} $$

_Solution (3rd):_

$$
\left[\begin{array}{cc}
2 & 1 \\
1 & 2 \\
3 & 3 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\end{bmatrix}
$$

By column:

$$ = 1\begin{bmatrix}{}2\\1\\3\end{bmatrix} + 1\begin{bmatrix}{}1\\2\\3\end{bmatrix} $$

$$ = \begin{bmatrix}{}2\\1\\3\end{bmatrix} + \begin{bmatrix}{}1\\2\\3\end{bmatrix} $$

$$ = \begin{bmatrix}{}2 + 1\\1 + 2\\3 + 3\end{bmatrix} $$

$$ = \begin{bmatrix}{}3\\3\\6\end{bmatrix} $$

13.

a. A matrix with $m$ rows and $n$ columns multiplies a vector with ____
components to produce a vector with ____ components.

_Multiplies a vector with:_

$n$ components

_To produce a vector with:_

$m$ components

b. The planes from the $m$ equations $Ax = b$ are in ____-dimensional space. The
combination of the columns of $A$ is in ____-dimensional space.

_The planes from the $m$ equations $Ax = b$ are in (?)-dimensional space._

$n$

_The combination of the columns of $A$ is in (?)-dimensional space._

$m$

14. Write $2x + 3y + z + 5t = 8$ as a matrix $A$ (how many rows?) multiplying
    the column vector $x = (x, y, z, t)$ to produce $b$. The solutions $x$ fill
    a plane or "hyperplane" in 4-dimensional space. _The plane is
    $3$-dimensional with no $4D$ volume_.

_Write $2x + 3y + z + 5t = 8$ as a matrix $A$ multiplying the column vector
$x = (x, y, z, t)$ to produce $b$:_

$$ A =
\left[\begin{array}{c}
2 & 3 & 1 & 5 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}8\end{bmatrix} = b
$$

_How many rows?:_

1

**Problems 15-22 ask for matrices that act in special ways on vectors.**

15.

a. What is the $2$ by $2$ identity matrix? $I$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ equals
$\begin{bmatrix}{}x\\y\end{bmatrix}$.

_Solution:_

$$
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

b. What is the $2$ by $2$ exchange matrix? $P$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ equals
$\begin{bmatrix}{}y\\x\end{bmatrix}$.

_Solution:_

$$
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right]
$$

16.

a. What $2$ by $2$ matrix $R$ rotates every vector by $90\degree$? $R$ times
$\begin{bmatrix}{}x\\y\end{bmatrix}$ is $\begin{bmatrix}{}y\\-x\end{bmatrix}$.

_Solution:_

$$
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
$$

b. What $2$ by $2$ matrix $R^2$ rotates every vector by $180\degree$?

_Solution:_

$$
\left[\begin{array}{cc}
-1 & 0 \\
0 & -1 \\
\end{array}\right]
$$

17. Find the matrix $P$ that multiplies $(x, y, z)$ to give $(y, z, x)$. Find
    the matrix $Q$ that multiplies $(y, z, x)$ to bring back $(x, y, z)$.

_Solution:_

_Find the matrix $P$ that multiplies $(x, y, z)$ to give $(y, z, x)$:_

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}y\\z\\x\end{bmatrix}
$$

_Find the matrix $Q$ that multiplies $(y, z, x)$ to bring back $(x, y, z)$:_

$$ Q =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}y\\z\\x\end{bmatrix} =
\begin{bmatrix}{}x\\y\\z\end{bmatrix}
$$

18. What $2$ by $2$ matrix $E$ subtracts the first component from the second
    component? What $3$ by $3$ matrix does the same?

$$ E\begin{bmatrix}{}3\\5\end{bmatrix} = \begin{bmatrix}{}3\\2\end{bmatrix} $$

and

$$ E\begin{bmatrix}{}3\\5\\7\end{bmatrix} = \begin{bmatrix}{}3\\2\\7\end{bmatrix} $$

_Solution:_

_What $2$ by $2$ matrix $E$ subtracts the first component from the second
component?:_

$$ E\begin{bmatrix}{}3\\5\end{bmatrix} = \begin{bmatrix}{}3\\2\end{bmatrix} $$

$$ E =
\left[\begin{array}{cc}
1 & 0 \\
-1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\5\end{bmatrix} =
\begin{bmatrix}{}3\\2\end{bmatrix}
$$

_What $3$ by $3$ matrix does the same?:_

$$ E\begin{bmatrix}{}3\\5\\7\end{bmatrix} = \begin{bmatrix}{}3\\2\\7\end{bmatrix} $$

$$ E =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\5\\7\end{bmatrix} =
\begin{bmatrix}{}3\\2\\7\end{bmatrix}
$$

19. What $3$ by $3$ matrix $E$ multiplies $(x, y, z)$ to give $(x, y, z + x)$?
    What matrix $E^{-1}$ multiplies $(x, y, z)$ to give $(x, y, z - x)$? If you
    multiply $(3, 4, 5)$ by $E$ and then multiply $E^{-1}$, the two results are
    ____ and ____.

_Solution:_

_What $3$ by $3$ matrix $E$ multiplies $(x, y, z)$ to give $(x, y, z + x)$?:_

$$ E =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
1 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}x\\y\\z + x\end{bmatrix}
$$

_What matrix $E^{-1}$ multiplies $(x, y, z)$ to give $(x, y, z - x)$?:_

$$ E^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}x\\y\\z - x\end{bmatrix}
$$

_If you multiply $(3, 4, 5)$ by $E$ and then multiply $E^{-1}$, the two results
are (?) and (?):_

$$ E =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
1 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\4\\5\end{bmatrix} =
\begin{bmatrix}{}3\\4\\8\end{bmatrix}
$$

$$ E^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\4\\8\end{bmatrix} =
\begin{bmatrix}{}3\\4\\5\end{bmatrix}
$$

20. What $2$ by $2$ matrix $P_1$ projects the vector $(x, y)$ onto the $x$ axis
    to produce $(x, 0)$? What matrix $P_2$ projects onto the $y$ axis to produce
    $(0, y)$? If you multiply $(5, 7)$ by $P_1$ and then multiply by $P_2$, you
    get ____ and ____.

_Solution:_

_What $2$ by $2$ matrix $P_1$ projects the vector $(x, y)$ onto the $x$ axis to
produce $(x, 0)$?:_

$$ P_1 =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}x\\0\end{bmatrix}
$$

_What matrix $P_2$ projects onto the $y$ axis to produce $(0, y)$?:_

$$ P_2 =
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}0\\y\end{bmatrix}
$$

_If you multiply $(5, 7)$ by $P_1$ and then multiply by $P_2$, you get (?) and
(?):_

$$ P_1 =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}5\\7\end{bmatrix} =
\begin{bmatrix}{}5\\0\end{bmatrix}
$$

$$ P_2 =
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}5\\0\end{bmatrix} =
\begin{bmatrix}{}0\\0\end{bmatrix}
$$

21. What $2$ by $2$ matrix $R$ rotates every vector through $45\degree$? The
    vector $(1, 0)$ goes to
    $\left(\dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2}\right)$. The vector $(0, 1)$
    goes to $\left(-\dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2}\right)$. Those
    determine the matrix. Draw these particular vectors in the $xy$ plane and
    find $R$.

_Solution:_

$$ R =
\left[\begin{array}{cc}
\dfrac{\sqrt{2}}{2} & -\dfrac{\sqrt{2}}{2} \\
\dfrac{\sqrt{2}}{2} & \dfrac{\sqrt{2}}{2} \\
\end{array}\right]
\begin{bmatrix}{}1\\0\end{bmatrix} =
\begin{bmatrix}{}\dfrac{\sqrt{2}}{2}\\\dfrac{\sqrt{2}}{2}\end{bmatrix}
$$

$$ R =
\left[\begin{array}{cc}
\dfrac{\sqrt{2}}{2} & -\dfrac{\sqrt{2}}{2} \\
\dfrac{\sqrt{2}}{2} & \dfrac{\sqrt{2}}{2} \\
\end{array}\right]
\begin{bmatrix}{}0\\1\end{bmatrix} =
\begin{bmatrix}{}\dfrac{-\sqrt{2}}{2}\\\dfrac{\sqrt{2}}{2}\end{bmatrix}
$$

_Drawing omitted (see Unit circle)._

22. Write the dot product of $(1, 4, 5)$ and $(x, y, z)$ as a matrix
    multiplication $Ax$. The matrix $A$ has one row. The solutions to
    $Ax = \mathbf{0}$ lie on a ____ perpendicular to the vector ____. The
    columns of $A$ are only in ____-dimensional space.

_Write the dot product of $(1, 4, 5)$ and $(x, y, z)$ as a matrix multiplication
$Ax$. The matrix $A$ has one row._

$$  Ax =
\left[\begin{array}{ccc}
1 & 4 & 5 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
1(x) + 4(y) + 5(z) = x + 4y + 5z
$$

_The solutions to $Ax = \mathbf{0}$ lie on a (?) perpendicular to the vector
(?):_

plane in 3 dimensions; $(1, 4, 5)$

_The columns of $A$ are only in (?)-dimensional space:_

one

23. Omitted (no MATLAB).

24. Omitted (no MATLAB).

25. Omitted (no MATLAB).

**Questions 26-28 review the row and column pictures in 2, 3, and 4
dimensions.**

26. Draw the row and column pictures for the equations $x - 2y = 0$,
    $x + y = 6$.

Done by hand.

27. For two linear equations in three unknowns $x, y, z$, the row picture will
    show (2 or 3) (lines or planes) in (2 or 3)-dimensional space. The column
    picture is in (2 or 3)-dimensional space. The solutions normally lie on a
    ____.

_For two linear equations in three unknowns $x, y, z$, the row picture will show
(2 or 3) (lines or planes) in (2 or 3)-dimensional space?:_

2 planes in 3 dimensional space

- 2 because there are 2 linear equations
- 3 dimensional space because 3 variables
- planes because we're in 3 dimensional space

_The column picture is in (2 or 3)-dimensional space. The solutions normally lie
on a (?):_

3 dimensional space (3 variables); line

- line because 3 variables - 2 equations = 1 dimension of freedom $\Rightarrow$
  line.

28. For four linear equations in two unknowns $x$ and $y$, the row picture shows
    four ____. The column picture is in ____-dimensional space. The equations
    have no solution unless the vector on the right side is a combination of
    ____.

_For four linear equations in two unknowns $x$ and $y$, the row picture shows
four (?):_

lines

_The column picture is in (?)-dimensional space:_

2

_The equations have no solution unless the vector on the right side is a
combination of (?):_

the two columns

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

_Solution:_

$$ u_2 =
\left[\begin{array}{cc}
.8 & .3 \\
.2 & .7 \\
\end{array}\right]
\begin{bmatrix}{}.8\\.2\end{bmatrix} =
\begin{bmatrix}{}.7\\.3\end{bmatrix}
$$

$$ u_3 =
\left[\begin{array}{cc}
.8 & .3 \\
.2 & .7 \\
\end{array}\right]
\begin{bmatrix}{}.7\\.3\end{bmatrix} =
\begin{bmatrix}{}.65\\.35\end{bmatrix}
$$

_What property do you notice for all four vectors $u_0, u_1, u_2, u_3$?:_

The components are positive and always add to 1 (this represents a probability,
they add up to 1 because these represent percentages, _i.e._ $.65 = 65\%$).

See [**Stochastic matrix**](https://en.wikipedia.org/wiki/Stochastic_matrix).
