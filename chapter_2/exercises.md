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

---

## Problem Set 2.2

Page 64

**Problems 1-10 are about elimination on 2 by 2 systems.**

1. What multiple $\ell_{21}$ of equation 1 should be subtracted from equation 2?

$$
2x + 3y = 1 \\
10x + 9y = 11
$$

After elimination, write down the upper triangular system and circle the two
pivots. The numbers 1 and 11 don't affect the pivots - use them now in back
substitution.

_Solution:_

_What multiple $\ell_{21}$ of equation 1 should be subtracted from equation 2?:_

$$ \ell_{21} = \frac{10}{2} = 5 $$

_Elimination:_

$$ \begin{array}{rrr} 10x + 9y = 11 \\

- 5(2x + 3y = 1) \end{array} $$

$$ \begin{array}{rrr} 10x + 9y = 11 \\

- 10x - 15y = -5 \end{array} $$

$$ -6y = 6 $$

_Pivots:_

$$
\begin{array}{rrr}
\boxed{2}x + 3y = 1 \\
\boxed{-6}y = 6 \\
\end{array}
$$

_Solve for $y$:_

$$ y = -1 $$

_Back substitution:_

$$ 2x + 3(-1) = 1 $$

$$ 2x - 3 = 1 $$

$$ 2x = 4 $$

$$ x = 2 $$

Solution is $\boxed{(2, -1)}$.

2. Solve the triangular system of Problem 1 by back substitution, $y$ before
   $x$. Verify that $x$ times $(2, 10)$ plus $y$ times $(3, 9$)$ equals
   $(1, 11)$. If the right side changes to $(4, 44)$, what is the new solution?

_Verify:_

$$ x\begin{bmatrix}{}2\\10\end{bmatrix} + y\begin{bmatrix}{}3\\9\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

$$ 2\begin{bmatrix}{}2\\10\end{bmatrix} + (-1)\begin{bmatrix}{}3\\9\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

$$ \begin{bmatrix}{}4\\20\end{bmatrix} + \begin{bmatrix}{}-3\\-9\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

$$ \begin{bmatrix}{}4 + (-3)\\20 + (-9)\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

$$ \begin{bmatrix}{}1\\11\end{bmatrix} = \begin{bmatrix}{}1\\11\end{bmatrix} $$

_Change to $(4, 44)$, new solution?:_

$$
\begin{array}{rrr}
2x + 3y = 4 \\
10x + 9y = 44
\end{array}
$$

Elimination:

$$ 10x + 9y = 44 \\

- 5(2x + 3y = 4) $$

$$ 10x + 9y = 44 \\

- 10x - 15y = -20 $$

$$ -6y = 24 $$

$$
\begin{array}{rrr}
2x + 3y = 1 \\
-6y = 24
\end{array}
$$

$$ -6y = 24 $$

$$ y = -4 $$

_Back-substitution:_

$$ 2x + 3(-4) = 4 $$

$$ 2x - 12 = 4 $$

$$ 2x = 16 $$

$$ x = 8 $$

New solution is $(8, -4)$.

3. What multiple of equation 1 should be _subtracted_ from equation 2?

$$
2x - 4y = 6 \\
-x + 5y = 0
$$

After this elimination step, solve the triangular system. If the right side
changes to $(-6, 0)$, what is the new solution?

_Solution:_

_What multiple of equation 1 should be _subtracted_ from equation 2?_

$$ -x + 5y = 0 \\

- \left(-\frac{1}{2}\right)(2x - 4y = 6) $$

So the multiple is $-\dfrac{1}{2}$.

_Elimination:_

$$ -x + 5y = 0 \\

- \left(-\frac{1}{2}\right)(2x - 4y = 6) $$

$$ -x + 5y = 0 \\

- (-x + 2y = -3) $$

Remaining upper triangular system:

$$
\begin{array}{rrr}
2x - 4y = 6 \\
3y = 3
\end{array}
$$

Solving the triangular system:

$$ 3y = 3 $$

$$ y = 1 $$

Back-substitution:

$$ 2x - 4y = 6 $$

$$ 2x - 4(1) = 6 $$

$$ 2x - 4 = 6 $$

$$ 2x = 10 $$

$$ x = 5 $$

So, solution is $(5, 1)$.

_If the right side changes to $(-6, 0)$, what is the new solution?:_

If the right side changes to $(-6, 0)$, then so does the solution: $(-5, -1)$.

4. What multiple $\ell$ of equation 1 should be subtracted from equation 2 to
   remove $c$?

$$
ax + by = f \\
cx + dy = g
$$

The first pivot is $a$ (assumed nonzero). Elimination produces what formula for
the second pivot? What is $y$? The second pivot is missing when $ad = bc$:
singular.

_Solution:_

_What multiple $\ell$ of equation 1 should be subtracted from equation 2 to
remove $c$?:_

$$ \frac{c}{a} $$

_Elimination produces what formula for the second pivot?:_

$$ \left(d - \frac{c}{a}b\right)y = g - \frac{c}{a}f $$

_What is $y$?:_

$$ y = \frac{g - \dfrac{c}{a}f}{d - \dfrac{c}{a}b}$$

$$ y = \frac{g - \dfrac{cf}{a}}{d - \dfrac{cb}{a}}$$

$$ y = \frac{\dfrac{ga - cf}{a}}{\dfrac{da - cb}{a}}$$

$$ y = \frac{ga - cf}{da - cb} $$

5. Choose a right side which gives no solution and another right side which
   gives infinitely many solutions. What are two of those solutions?

$$
\textbf{Singular system} \\
3x + 2y = 10 \\
6x + 4y =
$$

_Solution:_

_Choose a right side which gives no solution:_

$$ (6x + 4y =) \\

- 2(3x + 2y = 10) $$

$$ 6x + 4y = \\

- 6x - 4y = -20 $$

$$ 6x + 4y = \\

0y = -20 $$

So choosing any right side except for $20$ cause this combination to yield no
solutions.

_And another right side which gives infinitely many solutions:_

From the above, we can ascertain that choosing $6x + 4y = 20$ will yield:

$$ 0y = 0 $$

And this yields infinitely many solutions for $y$.

_What are two of those solutions?:_

$$
3x + 2y = 10 \\
6x + 4y = 20 \\
$$

$$
3(2) + 2(2) = 10 \\
6(2) + 4(2) = 20 \\
$$

So $(2, 2)$ is one solution.

$$
3(-2) + 2(8) = 10 \\
6(-2) + 4(8) = 20 \\
$$

So $(-2, 8)$ is another solution.

6. Choose a coefficient $b$ that makes this system singular. Then choose a right
   side $g$ that makes it solvable. Find two solutions in that singular case.

$$
2x + by = 16 \\
4x + 8y = g
$$

_Choose a coefficient $b$ that makes this system singular:_

To make it singular, choose $b$ such that there are no or infinitely many
solutions.

Choose $b = 4$,then:

$$ 4x + 8y = g \\

- 2(2x + 4y = 16) \\ $$

$$ 4x + 8y = g \\

- 4x - 8y = -32 $$

$$
\begin{array}{rrr}
2x + by = 16 \\
0y = g - 32 \\
\end{array}
$$

Thus when $b = 4$, this system is singular (the value of $g$ determines if there
are no solutions, _i.e._ $g \neq 32$, or infinitely many solutions, _i.e._
$g = 32$).

_Then choose a right side $g$ that makes it solvable:_

Choose $g = 32$, then:

$$ (4x + 8y = 32) - 2(2x + 4y = 16) \Rightarrow (4x + 8y = 32) - (4x + 8y = 32) \Rightarrow 0y = 0 $$

_Find two solutions in that singular case:_

_first:_

Choose $b = 4, g = 32, y = 1$:

$$ 2x + 4 = 16 \Rightarrow 2x = 12 \Rightarrow x = 6 $$

$$ 4(6) + 8(1) = 32 \Rightarrow 24 + 8 = 32 \Rightarrow 32 = 32 $$

One solution $(6, 1)$.

_second:_

Choose $b = 4, g = 32, y = 2$:

$$ 2x + 8 = 16 \Rightarrow 2x = 8 \Rightarrow x = 4 $$

$$ 4(4) + 16 = 32 \Rightarrow 16 + 16 = 32 \Rightarrow 32 = 32 $$

Second solution $(4, 2)$.

7. For which numbers $a$ does elimination break down (1) permanently (2)
   temporarily?

$$
ax + 3y = -3 \\
4x + 6y = 6
$$

Solve for $x$ and $y$ after fixing the temporary breakdown by a row exchange.

_For which numbers $a$ does elimination break down permanently?:_

$$
ax + 3y = -3 \\
4x + 6y = 6
$$

If $a = 2$, then:

$$ 4x + 6y = 6 \\

- 2(2x + 3y = -3) \\ \Rightarrow 4x + 6y = 6 \\
- (4x + 6y = -6) \Rightarrow 0y = 12 $$

And this has no solution.

_For which numbers $a$ does elimination break down temporarily?:_

Setting $a = 0$, but then a row exchange as follows allows us to solve:

$$
4x + 6y = 6 \\
3y = -3 \\
$$

_Solve for $x$ and $y$ after fixing the temporary breakdown by a row exchange:_

$$
4x + 6y = 6 \\
3y = -3 \\
$$

$$ 3y = -3 \Rightarrow y = -1 $$

$$ 4x + 6(-1) = 6 \Rightarrow 4x - 6 = 6 \Rightarrow 4x = 12 \Rightarrow x = 3 $$

Solution is $(3, -1)$.

8. For which three numbers $k$ does elimination break down? Which is fixed by a
   row exchange? In each case, is the number of solutions $0$ or $1$ or
   $\infty$?

$$
kx + 3y = 6 \\
3x + ky = -6
$$

_For which three numbers $k$ does elimination break down?:_

When $k = 0, 3, -3$.

When $k = 0$, this is temporary, and fixed by a row exchange.

When $k = 3$, we get $0y = -12$, elimination fails and has no solution.

When $k = -3$, we get $0 = 0$ (you must _add_ the two equations for this result,
otherwise you get a redundant equation when subtracted). In this case, there are
infinitely many solutions.

_Which is fixed by a row exchange?:_

When $k = 0$, then just exchange rows:

$$
3x = -6 \\
3y = 6 \\
$$

_In each case, is the number of solutions $0$ or $1$ or $\infty$:_

When $k = 0$, the solution is:

$$ (-2, 2) $$

One solution.

When $k = 3$, there is no solution since $0y = -12$ indicates that elimination
failed.

When $k = -3$, there are $\infty$ solutions, as established earlier.

9. What test on $b_1$ and $b_2$ decides whether these two equations allow a
   solution? How many solutions will they have? Draw the column picture for
   $b = (1, 2)$ and $(1, 0)$.

$$
3x - 2y = b_1 \\
6x - 4y = b_2
$$

_What test on $b_1$ and $b_2$ decides whether these two equations allow a
solution?:_

Solving for this yields:

$$ 6x - 4y = b_2 \\

- 2(3x - 2y = b_1) $$

$$ \Rightarrow 6x - 4y = b_2 \\

- 6x + 4y = -2b_1 $$

$$ \Rightarrow
0 = b_2 - 2b_1
$$

If $0 = 0$, there are infinitely many solutions, so if $b_2 - 2b_1 \neq 0$,
there is no solution, this is the test:

$$ b_2 - 2b_1 \stackrel{?}{=} 0 $$

Or equivalently:

$$ b_2 \stackrel{?}{=} 2b_1 $$

_How many solutions will they have?:_

Infinite.

_Draw the column picture for $b = (1, 2)$:_

$$ x\begin{bmatrix}{}3\\6\end{bmatrix} + y\begin{bmatrix}{}-2\\-4\end{bmatrix} = \begin{bmatrix}{}1\\2\end{bmatrix} $$

_and $(1, 0)$:_

$$ x\begin{bmatrix}{}3\\6\end{bmatrix} + y\begin{bmatrix}{}-2\\-4\end{bmatrix} = \begin{bmatrix}{}1\\0\end{bmatrix} $$

10. In the $xy$ plane, draw the lines $x + y = 5$ and $x + 2y = 6$ and the
    equation $y =$ ____ that comes from elimination. The line $5x - 4y = c$ will
    go through the solution of these equations if $c =$ ____.

$$ x + 2y = 6 \\

- (x + y = 5) $$

$$ \boxed{y = 1} $$

$$ x + 2 = 6 \Rightarrow x = 4 $$

$$ 5(4) - 4(1) = c $$

$$ 20 - 4 = c $$

$$ \boxed{16 = c} $$

**Problems 11-20 study elimination on 3 by 3 systems (and possible failure).**

11. (Recommended) A system of linear equations can't have exactly two solutions.
    _Why_?

_Why?:_

Because a system of linear equations can only have no solutions (_i.e._
$0z \neq 0$), one solution, or infinitely many solutions (_i.e._ $0 = 0$).

a. If $(x, y, z)$ and $(X, Y, Z)$ are two solutions, what is another solution?

Another solution is some scalar multiple of these two solution's sum:

$$ \dfrac{1}{2}(x + X, y + Y, z + Z) $$

b. If $25$ planes meet at two points, where else do they meet?

They meet at all points throughout the line drawn by those two points, since
there being two points indicates there being two solutions, indicating there are
infinitely many more.

12. Reduce this system to upper triangular form by two row operations:

$$
2x + 3y + z = 8 \\
4x + 7y + 5z = 20 \\
-2y + 2z = 0
$$

Circle the pivots. Solve by back substitution for $z, y, x$.

_Solution:_

_Reduce this system to upper triangular form by two row operations:_

$$
2x + 3y + z = 8 \\
4x + 7y + 5z = 20 \\
-2y + 2z = 0
$$

$$ (4x + 7y + 5z = 20) - 2(2x + 3y + z = 8) = y + 3z = 4 $$

$$
y + 3z = 4 \\
-2y + 2z = 0
$$

$$ (-2y + 2z = 0) + 2(y + 3z = 4) = 8z = 8 $$

$$
\begin{array}{rrr}
2x + 3y + z = 8 \\
y + 3z = 4 \\
8z = 8 \\
\end{array}
$$

_Circle the pivots. Solve by back substitution for $z, y, x$:_

$$
\begin{array}{rrr}
\boxed{2}x + 3y + z = 8 \\
\boxed{1}y + 3z = 4 \\
\boxed{8}z = 8 \\
\end{array}
$$

$$ z = 1 $$

$$ y + 3(1) = 4 $$

$$ y + 3 = 4 $$

$$ y = 4 - 3 $$

$$ y = 1 $$

$$ 2x + 3(1) + 1 = 8 $$

$$ 2x + 3 + 1 = 8 $$

$$ 2x + 4 = 8 $$

$$ 2x = 8 - 4 $$

$$ 2x = 4 $$

$$ x = 2 $$

Solution: $(2, 1, 1)$.

13. Apply elimination (circle the pivots) and back substitution to solve

$$
2x - 3y = 3 \\
4x - 5y + z = 7 \\
2x - y - 3z = 5
$$

List the three row operations: Subtract ____ times row ____ from row ____.

_Solution:_

_Apply elimination:_

$$
2x - 3y = 3 \\
4x - 5y + z = 7 \\
2x - y - 3z = 5
$$

$$ (4x - 5y + z = 7) - 2(2x - 3y = 3) = (y + z = 1) $$

$$
2x - 3y = 3 \\
y + z = 1 \\
2x - y - 3z = 5
$$

$$ (2x - y - 3z = 5) - (2x - 3y = 3) = (2y - 3z = 2)  $$

$$
2x - 3y = 3 \\
y + z = 1 \\
2y - 3z = 2
$$

$$ (2y - 3z = 2) - 2(y + z = 1) = (-5z = 0) $$

$$
2x - 3y = 3 \\
y + z = 1 \\
-5z = 0 \\
$$

_circle the pivots:_

$$
\boxed{2}x - 3y = 3 \\
\boxed{1}y + z = 1 \\
\boxed{-5}z = 0 \\
$$

_back substitution to solve:_

$$ -5z = 0 $$

$$ z = 0 $$

$$ y + (0) = 1 $$

$$ y = 1 $$

$$ 2x - 3(1) = 3 $$

$$ 2x - 3 = 3 $$

$$ 2x = 6 $$

$$ x = 3 $$

Solution: $(3, 1, 0)$.

_List the three row operations:_

_Subtract (?) times row (?) from row (?):_

Subtract 2 times row 1 from row 2.

Subtract 1 times row 1 from row 3.

Subtract 2 times row 2 from row 3.

14. Which number $d$ forces a row exchange, and what is the triangular system
    (not singular) for that $d$? Which $d$ makes this system singular (no third
    pivot)?

$$
2x + 5y + z = 0 \\
4x + dy + z = 2 \\
y - z = 3
$$

_Solution:_

_Which number $d$ forces a row exchange?:_

$$ (4x + (10)y + z = 2) - 2(2x + 5y + z = 0) = (z = -2) $$

$$ d = 10 $$

forces a row change of rows 2 and 3.

_and what is the triangular system (not singular) for that $d$?:_

$$
\begin{array}{rrr}
2x  + 5y + z = 0 \\
y - z = 3 \\
z = -2 \\
\end{array}
$$

_Which $d$ makes this system singular (no third pivot)?:_

$$ (4x + (11)y + z = 2) - 2(2x + 5y + z = 0) = (y + z = -2) $$

$$ d = 11 $$

15. Which number $b$ leads later to a row exchange? Which $b$ leads to a missing
    pivot? In that singular case find a nonzero solution $x, y, z$.

$$
x + by = 0 \\
x - 2y - z = 0 \\
y + z = 0
$$

_Solution:_

_Which number $b$ leads later to a row exchange?:_

$$ (x - 2y - z = 0) - (x + (-2)y = 0) = (-z = 0)  $$

$$ b = -2 $$

_Which $b$ leads to a missing pivot?:_

$$ (x - 2y - z = 0) - (x + (-1)y = 0) = (-y - z = 0)  $$

$$ b = -1 $$

Because then eliminating the next line $y + z = 0$ is not possible, and row
exchange cannot fix it.

_In that singular case find a nonzero solution $x, y, z$:_

$$ b = -1 $$

$$
x + (-1)y = 0 \\
x - 2y - z = 0 \\
y + z = 0 \\
$$

$$
x - y = 0 \\
x - 2y - z = 0 \\
y + z = 0 \\
$$

$$ (x - 2y - z) - (x - y = 0) = (-y - z = 0) $$

$$
x - y = 0 \\
-y - z = 0 \\
y + z = 0 \\
$$

$$ (y + z = 0) + (-y - z = 0) = (0 = 0) $$

Infinite solutions, choose $y = 1$:

$$
x - (1) = 0 \\
x - 2(1) - z = 0 \\
(1) + z = 0 \\
$$

$$
x = 1 \\
x - 2 - z = 0 \\
z = -1 \\
$$

$$
x = 1 \\
(1) - 2 - (-1) = 0 \\
z = -1 \\
$$

$$
x = 1 \\
0 = 0 \\
z = -1 \\
$$

Solution: $(1, 1, -1)$.

16.

a. Construct a 3 by 3 system that needs two row exchanges to reach a triangular
form and a solution.

$$
0x + 2y + 0z = 4 \\
x + 2y + 2z = 5 \\
0x + 3y + 4z = 6 \\
$$

_Solution:_

$$
2y = 4 \\
x + 2y + 2z = 5 \\
3y + 4z = 6 \\
$$

First row exchange:

$$
x + 2y + 2z = 5 \\
2y = 4 \\
3y + 4z = 6 \\
$$

Second row exchange:

$$
\begin{array}{rrr}
x + 2y + 2z = 5 \\
3y + 4z = 6 \\
2y = 4 \\
\end{array}
$$

Solve:

$$
x + 2(2) + 2z = 5 \\
3(2) + 4z = 6 \\
y = 2 \\
$$

$$
x + 4 + 2z = 5 \\
6 + 4z = 6 \\
y = 2 \\
$$

$$
x + 4 + 2z = 5 \\
4z = 0 \\
y = 2 \\
$$

$$
x + 4 + 2(0) = 5 \\
z = 0 \\
y = 2 \\
$$

$$
x + 4 = 5 \\
z = 0 \\
y = 2 \\
$$

$$
x = 1 \\
z = 0 \\
y = 2 \\
$$

Solution: $\boxed{(1, 2, 0)}$

b. Construct a 3 by 3 system that needs a row exchange to keep going, but breaks
down later.

$$
0x + 3y + 4z = 4 \\
x + 2y + 2z = 5 \\
0x + 3y + 4z = 6 \\
$$

_Solution:_

$$
3y + 4z = 4 \\
x + 2y + 2z = 5 \\
3y + 4z = 6 \\
$$

One row exchange:

$$
3y + 4z = 4 \\
3y + 4z = 6 \\
x + 2y + 2z = 5 \\
$$

Now, keep going:

$$ (3y + 4z = 6) - (3y + 4z = 4) \Rightarrow 0 = 2 $$

Breakdown, no solution.

17. If rows 1 and 2 are the same, how far can you get with elimination (allowing
    row exchange)? If columns 1 and 2 are the same, which pivot is missing?

$$
\textbf{Equal rows} \\
2x - y + z = 0 \\
2x - y + z = 0 \\
4x + y + z = 2
$$

$$
\textbf{Equal columns} \\
2x + 2y + z = 0 \\
4x + 4y + z = 0 \\
6x + 6y + z = 2
$$

_Solution:_

_Equal rows, how far can you get with elimination?:_

$$
\textbf{Equal rows} \\
2x - y + z = 0 \\
2x - y + z = 0 \\
4x + y + z = 2
$$

To avoid immediately running into infinitely many solutions, let's substitute
first:

$$
2x - y + z = 0 \\
4x + y + z = 2 \\
2x - y + z = 0 \\
$$

$$ (4x + y + z = 2) - 2(2x - y + z = 0) \Rightarrow (3y - z = 2) $$

$$
\begin{array}{rrr}
2x - y + z = 0 \\
3y - z = 2 \\
2x - y + z = 0 \\
\end{array}
$$

Then subtract row 1 from row 3:

$$ (2x - y + z = 0) - (2x - y + z = 0) \Rightarrow 0 = 0 $$

No further pivots. This particular breakdown where $0 = 0$ implies infinitely
many solutions.

_Equal columns, which pivot is missing?:_

$$
\textbf{Equal columns} \\
2x + 2y + z = 0 \\
4x + 4y + z = 0 \\
6x + 6y + z = 2
$$

We do start off with a pivot:

$$
\textbf{Equal columns} \\
\boxed{2}x + 2y + z = 0 \\
4x + 4y + z = 0 \\
6x + 6y + z = 2
$$

But as soon as elimination starts, we get $0 = 0$, this implies that the second
column has no pivot whenever column 1 = column 2.

18. Construct a 3 by 3 example that has 9 different coefficients on the left
    side, but rows 2 and 3 become zero in elimination. How many solutions to
    your system with $b = (1, 10, 100)$ and how many with $b = (0, 0, 0)$?

_Solution:_

_Construct a 3 by 3 example that has 9 different coefficients on the left side,
but rows 2 and 3 become zero in elimination:_

In order to deduce such an example, work backwards. Consider two rows that must
eliminate and result in $0 = 0$, but start initially with different
coefficients.

$$
5y + 10z = 0 \\
20y + 40z = 0 \\
$$

Then, consider the first row as needing to be subtracted from a second,
currently unknown, row such that it results in the above (both rows must have
the $x$ variable and different corresponding coefficients):

$$ (\text{?}x + \text{?}y + \text{?}z = 0) - (\text{?}x + \text{?}y + \text{?}z = 0) \Rightarrow (5y + 10z = 0) $$

Where none of the $\text{?}$ equal any other $\text{?}$.

Try:

$$ (2x + 35y + 60z = 0) - 2(x + 15y + 25z = 0) \Rightarrow (5y + 10z = 0) $$

This leaves us with our solution:

$$
x + 15y + 25z = 0 \\
2x + 35y + 60z = 0 \\
0x + 20y + 40z = 0 \\
$$

As you can see, all 9 coefficients are unique (1, 15, 25, 2, 35, 60, 0, 20, 40).
Let's double check to be sure they become zero in elimination.

$$ (2x + 35y + 60z = 0) - 2(x + 15y + 25z = 0) \Rightarrow (5y + 10z = 0) $$

$$
\begin{array}{rrr}
x + 15y + 25z = 0 \\
5y + 10z = 0 \\
20y + 40z = 0 \\
\end{array}
$$

$$ (20y + 40z = 0) - 4(5y + 10z = 0) \Rightarrow (0 = 0) $$

Thus our choice of coefficients satisfies the problem statement's requirements.

_How many solutions to your system with $b = (1, 10, 100)$ and how many with
$b = (0, 0, 0)$?:_

When $b = (0, 0, 0)$, the amount of solutions is infinite as demonstrated above.

When $b = (1, 10, 100)$:

$$
x + 15y + 25z = 1 \\
2x + 35y + 60z = 10 \\
0x + 20y + 40z = 100 \\
$$

$$ (2x + 35y + 60z = 10) - 2(x + 15y + 25z = 1) \Rightarrow (5y + 10z = 8) $$

$$
x + 15y + 25z = 1 \\
5y + 10z = 8 \\
20y + 40z = 100 \\
$$

$$ (20y + 40z = 100) - 4(5y + 10z = 8) \Rightarrow (0 = 68) $$

Thus when $b = (1, 10, 100)$, there are no solutions.

19. Which number $q$ makes this system singular and which right side $t$ gives
    it infinitely many solutions? Find the solution that has $z = 1$.

$$
x + 4y - 2z = 1 \\
x + 7y - 6z = 6 \\
3y + qz = t
$$

_Solution:_

_Which number $q$ makes this system singular and which right side $t$ gives it
infinitely many solutions?:_

$$ (x + 7y - 6z = 6) - (x + 4y - 2z = 1) \Rightarrow (3y - 4z = 5) $$

$$
x + 4y - 2z = 1 \\
3y - 4z = 5 \\
3y + qz = t
$$

To get infinitely many solutions, the final conclusion of elimination must
result in $0 = 0$, thus the following must be true:

$$ (3y + qz = t) - (3y - 4z = 5) \Rightarrow (0 = 0) $$

Thus, let $q = -4, t = 5$, and:

$$ (3y - 4z = 5) - (3y - 4z = 5) \Rightarrow (0 = 0) $$

So our solution to this problem is $q = -4, t = 5$.

_Find the solution that has $z = 1$:_

$$
x + 4y - 2z = 1 \\
x + 7y - 6z = 6 \\
3y + qz = t
$$

From the previous part, let $q = -4, t = 5$, and from this part $z = 1$, then:

$$
x + 4y - 2(1) = 1 \\
x + 7y - 6(1) = 6 \\
3y - 4(1) = 5
$$

$$
x + 4y - 2 = 1 \\
x + 7y - 6 = 6 \\
3y - 4 = 5
$$

$$
x + 4y = 3 \\
x + 7y = 12 \\
3y = 9
$$

$$
x + 4(3) = 3 \\
x + 7(3) = 12 \\
y = 3
$$

$$
x + 12 = 3 \\
x + 21 = 12 \\
y = 3
$$

$$
x = -9 \\
x = -9 \\
y = 3
$$

So the solution when $z = 1$ is: $\boxed{(-9, 3, 1)}$.

20. Three planes can fail to have an intersection point, even if no planes are
    parallel. The system is singular if row $3$ of $A$ is a ____ of the first
    two rows. Find a third equation that can't be solved together with
    $x + y + z = 0$ and $x - 2y - z = 1$.

_The system is singular if row $3$ of $A$ is a (?) of the first two rows:_

linear combination

Essentially the third row must have the same equation on the left as the
difference of the first two rows (after an optional multiple is applied to get
rid of the initial $x$ column), but the right side of the third row equation
must not be equal to the right side of the difference equation. This is
demonstrated in the next part of this problem.

_Find a third equation that can't be solved together with $x + y + z = 0$ and
$x - 2y - z = 1$:_

$$
x + y + z = 0 \\
x - 2y - z = 1 \\
\text{(?)}
$$

$$ (x - 2y - z = 1) - (x + y + z = 0) \Rightarrow (-3y - 2z = 1) $$

$$
x + y + z = 0 \\
-3y - 2z = 1\\
\text{(?)}
$$

Now, our third row must be chosen such that:

$$ \text{(?)} - (-3y - 2z = 1) \Rightarrow (0 \neq 0) $$

Thus:

$$ (-3y - 2z = 2) - (-3y - 2z = 1) \Rightarrow (0 \neq 0) $$

So our third equation is:

$$ \boxed{-3y - 2z = 2} $$

As it results in no solution.

21. Find the pivots and the solution for both systems ($Ax = b$ and $Kx = b$):

$$
2x + y = 0 \\
x + 2y + z = 0 \\
y + 2z + t = 0 \\
z + 2t = 5
$$

$$
2x - y = 0 \\
-x - 2y - z = 0 \\
-y - 2z - t = 0 \\
-z - 2t = 5
$$

_Solution:_

_First system:_

$$
2x + y = 0 \\
x + 2y + z = 0 \\
y + 2z + t = 0 \\
z + 2t = 5
$$

To find the pivots, first find the upper triangular form:

$$
2x + y = 0 \\
x + 2y + z = 0 \\
y + 2z + t = 0 \\
z + 2t = 5
$$

$$ (x + 2y + z = 0) - \left(\frac{1}{2}\right)(2x + y = 0) \Rightarrow \left(\frac{3}{2}y + z = 0\right) $$

$$
2x + y = 0 \\
\frac{3}{2}y + z = 0\\
y + 2z + t = 0 \\
z + 2t = 5
$$

$$ (y + 2z + t = 0) - \left(\frac{2}{3}\right)\left(\frac{3}{2}y + z = 0\right) \Rightarrow \left(\frac{4}{3}z + t = 0\right) $$

$$
2x + y = 0 \\
\frac{3}{2}y + z = 0\\
\frac{4}{3}z + t = 0 \\
z + 2t = 5
$$

$$ (z + 2t = 5) - \left(\frac{3}{4}\right)\left(\frac{4}{3}z + t = 0\right) \Rightarrow \left(\frac{5}{4}t = 5\right) $$

Thus our pivots are:

$$
\begin{array}{rrr}
\boxed{2}x + y = 0 \\
\boxed{\dfrac{3}{2}}y + z = 0\\
\boxed{\dfrac{4}{3}}z + t = 0 \\
\boxed{\dfrac{5}{4}}t = 5 \\
\end{array}
$$

Now, to solve (by back substitution):

$$ \frac{5}{4}t = 5  $$

$$ t = 5\left(\frac{4}{5}\right)  $$

$$ t = 4 $$

$$ \frac{4}{3}z + (4) = 0 $$

$$ \frac{4}{3}z = -4 $$

$$ z = -4\left(\frac{3}{4}\right) $$

$$ z = -3 $$

$$ \frac{3}{2}y + (-3) = 0 $$

$$ \frac{3}{2}y = 3 $$

$$ y = 3\left(\frac{2}{3}\right) $$

$$ y = 2 $$

$$ 2x + (2) = 0 $$

$$ 2x = -2 $$

$$ x = -1 $$

Thus our solution is $\boxed{(-1, 2, -3, 4)}$.

_Second system:_

$$
2x - y = 0 \\
-x - 2y - z = 0 \\
-y - 2z - t = 0 \\
-z - 2t = 5
$$

Finding pivots:

$$ (-x - 2y - z = 0) - \left(-\frac{1}{2}\right)(2x - y = 0) \Rightarrow \left(-\frac{5}{2}y - z = 0\right) $$

$$
2x - y = 0 \\
-\dfrac{5}{2}y - z = 0\\
-y - 2z - t = 0 \\
-z - 2t = 5
$$

$$ (-y - 2z - t = 0) - \left(\frac{2}{5}\right)\left(-\frac{5}{2}y - z = 0\right) \Rightarrow \left(-\frac{8}{5}z - t = 0\right) $$

$$
2x - y = 0 \\
-\dfrac{5}{2}y - z = 0 \\
-\dfrac{8}{5}z - t = 0 \\
-z - 2t = 5
$$

$$ (-z - 2t = 5) - \left(\frac{5}{8}\right)\left(-\frac{8}{5}z - t = 0\right) \Rightarrow \left(-\frac{11}{8}t = 5\right) $$

So, our pivots are:

$$
\boxed{2}x - y = 0 \\
\boxed{-\dfrac{5}{2}}y - z = 0 \\
\boxed{-\dfrac{8}{5}}z - t = 0 \\
\boxed{-\dfrac{11}{8}}t = 5 \\
$$

Now to find the solution (by back substitution):

$$ -\frac{11}{8}t = 5 $$

$$ t = 5\left(-\frac{8}{11}\right) $$

$$ t = -\frac{40}{11} $$

$$ -\frac{8}{5}z - \left(-\frac{40}{11}\right) = 0 $$

$$ -\frac{8}{5}z = -\frac{40}{11} $$

$$ z = -\frac{40}{11}\left(-\frac{5}{8}\right) $$

$$ z = \frac{25}{11} $$

$$ -\frac{5}{2}y - \left(\frac{25}{11}\right) = 0 $$

$$ -\frac{5}{2}y = \frac{25}{11} $$

$$ y = \frac{25}{11}\left(-\frac{2}{5}\right) $$

$$ y = -\frac{10}{11} $$

$$ 2x - \left(-\frac{10}{11}\right) = 0 $$

$$ 2x = -\frac{10}{11} $$

$$ x = -\frac{10}{11}\left(\frac{1}{2}\right) $$

$$ x = -\frac{5}{11} $$

Thus our solution is:

$$ \boxed{\left(-\frac{5}{11}, -\frac{10}{11}, \frac{25}{11}, -\frac{40}{11}\right)} $$

_Note:_ This solution is to an incorrectly copied problem. Moving on anyways.

22. If you extend Problem 21 following the $1, 2, 1$ pattern or the $-1, 2, -1$
    pattern, what is the fifth pivot? What is the $n$th pivot? $K$ is my
    favorite matrix.

The correct answer to part (b) of 21 was $(1, 2, 3, 4)$ instead of
$(-1, 2, -3, 4)$. The key was recognizing that whenever you increased the amount
of pivots from $n$ to $n + 1$, that the pivot took on the form of
$\dfrac{n + 1}{n}$, thus the fifth pivot would follow $\dfrac{6}{5}$ for both
matrices multiplied by $1$ or $-1$ depending on the pattern of simply adding all
coefficients or subtracting all but the first (the $x$ coefficient).

23. If elimination leads to $x + y = 1$ and $2y = 3$, find three possible
    original problems.

_Solution:_

Strang is asking us to find a 2 x 2 system which ends in the upper triangular
form of:

$$
\begin{array}{rr}
x + y = 1 \\
2y = 3
\end{array}
$$

Thus each solution is asking us to find:

$$ (\text{?}) - (x + y = 1) \Rightarrow (2y = 3) $$

_1<sup>st</sup>:_

$$ (x + 3y = 4) - (x + y = 1) \Rightarrow (2y = 3) $$

$$
x + y = 1 \\
x + 3y = 4
$$

_2<sup>nd</sup>:_

$$ (2x + 4y = 5) - 2(x + y = 1) \Rightarrow (2y = 3) $$

$$
x + y = 1 \\
2x + 4y = 5
$$

_3<sup>rd</sup>:_

$$ (3x + 5y = 6) - 3(x + y = 1) \Rightarrow (2y = 3) $$

$$
x + y = 1 \\
3x + 5y = 6
$$

24. For which two numbers $a$ will elimination fail on
    $A = \left[\begin{array}{cc}
a & 2 \\
a & a \\
\end{array}\right]$?

_Solution:_

The problem statement is asking us which $a$ will elimination fail on the
following system:

$$
ax + 2y = b_1 \\
ax + ay = b_2
$$

So, finding upper triangular form involves the following evaluation:

$$ (ax + ay = b_2) - (ax + 2y = b_1) \Rightarrow ay - 2y = b_2 - b_1 \Rightarrow y(a - 2) = b_2 - b_1 $$

Upper triangular form:

$$
\begin{array}{rr}
ax + 2y = b_1 \\
y(a - 2) = b_2 - b_1
\end{array}
$$

If $a = 2$, then:

$$
(2)x + 2y = b_1 \\
(2)x + (2)y = b_2
$$

$$
2x + 2y = b_1 \\
2x + 2y = b_2
$$

$$ (2x + 2y = b_2) - (2x + 2y = b_1) \Rightarrow (0 = b_2 - b_1) $$

Thus if $b_2 - b_1 = 0$, then there are infinite solutions, and if
$b_2 - b_1 \neq 0$, there are no solutions. This is where elimination breaks
down.

Now consider $a = 0$:

$$
(0)x + 2y = b_1 \\
(0)x + (0)y = b_2
$$

$$
0 = b_2
2y = b_1 \\
$$

$$
0 = b_2
y = \dfrac{b_1}{2} \\
$$

Thus, since $x$ is now a free variable, there are infinitely many solutions when
$b_2 = 0$, and no solutions when $b_2 \neq 0$.

25. For which three numbers $a$ will elimination fail to give three pivots?

$$ A =
\left[\begin{array}{ccc}
a & 2 & 3 \\
a & a & 4 \\
a & a & a \\
\end{array}\right] \text{ is singular for three values of } a
$$

_Solution:_

This is similar to problem 24.

$$
ax + 2y + 3z = b_1 \\
ax + ay + 4z = b_2 \\
ax + ay + az = b_3 \\
$$

Upper triangular form:

$$ (ax + ay + 4z = b_2) - (ax + 2y + 3z = b_1) \Rightarrow ((ay - 2y) + (4z - 3z) = (b_2 - b_1)) \Rightarrow ((a - 2)y + z = b_2 - b_1) $$

$$
ax + 2y + 3z = b_1 \\
(a - 2)y + z = b_2 - b_1 \\
ax + ay + az = b_3 \\
$$

$$ (ax + ay + az = b_3) - (ax + 2y + 3z = b_1) \Rightarrow ((a - 2)y + (a - 3)z = b_3 - b_1) $$

$$
ax + 2y + 3z = b_1 \\
(a - 2)y + z = b_2 - b_1 \\
(a - 2)y + (a - 3)z = b_3 - b_1 \\
$$

$$ ((a - 2)y + (a - 3)z = b_3 - b_1) - ((a - 2)y + z = b_2 - b_1) \Rightarrow ((a - 3 - 1)z = (b_3 - b_1) - (b_2 - b_1)) $$

$$ \Rightarrow (a - 4)z = b_3 - b_1 - b_2 + b_1 $$

$$ \Rightarrow (a - 4)z = b_3 - b_2 $$

Final upper triangular form:

$$
\begin{array}{rrr}
ax + 2y + 3z = b_1 \\
(a - 2)y + z = b_2 - b_1 \\
(a - 4)z = b_3 - b_2 \\
\end{array}
$$

So, now to find $a$'s where elimination fails, simply set the pivots to $0$.
Notice the pivots:

$$
\begin{array}{rrr}
\boxed{a}x + 2y + 3z = b_1 \\
\boxed{(a - 2)}y + z = b_2 - b_1 \\
\boxed{(a - 4)}z = b_3 - b_2 \\
\end{array}
$$

So the values for $a$ where elimination fails are at $a = 0, 2, 4$.

26. Look for a matrix that has row sums $4$ and $8$, and column sums $2$ and
    $s$:

$$ \text{Matrix } =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

$$
a + b = 4 \\
c + d = 8 \\
a + c = 2 \\
b + d = s \\
$$

The four equations are solvable only if $s =$ ____. Then find two different
matrices that have the correct row and column sums. _Extra Credit:_ Write down
the $4$ by $4$ system $Ax = b$ with $x = (a, b, c, d)$ and make $A$ triangular
by elimination.

_The four equations are solvable only if $s =$ (?):_

This is a 4 x 4 system:

$$
1a + 1b + 0c + 0d = 4 \\
0a + 0b + 1c + 1d = 8 \\
1a + 0b + 1c + 0d = 2 \\
0a + 1b + 0c + 1d = s
$$

Exchange rows:

$$
1a + 1b + 0c + 0d = 4 \\
1a + 0b + 1c + 0d = 2 \\
0a + 0b + 1c + 1d = 8 \\
0a + 1b + 0c + 1d = s
$$

Now, evaluate to find upper triangular form:

$$ (1a + 0b + 1c + 0d = 2) - (1a + 1b + 0c + 0d = 4) \Rightarrow (-1b + 0c + 0d = -2) $$

$$
1a + 1b + 0c + 0d = 4 \\
-1b + 0c + 0d = -2 \\
0b + 1c + 1d = 8 \\
1b + 0c + 1d = s
$$

$$ (0b + 1c + 1d = 8) - (-1b + 0c + 0d = -2) \Rightarrow (1b + 1c + 1d = 10) $$

$$
1a + 1b + 0c + 0d = 4 \\
-1b + 0c + 0d = -2 \\
1b + 1c + 1d = 10 \\
1b + 0c + 1d = s
$$

$$ (1b + 0c + 1d = s) - (1b + 1c + 1d = 10) \Rightarrow (-1c + 0d = s - 10) $$

$$
1a + 1b + 0c + 0d = 4 \\
-1b + 0c + 0d = -2 \\
1b + 1c + 1d = 10 \\
-1c + 0d = s - 10
$$

Thus:

$$ -1c = s - 10 \Rightarrow c = 10 - s $$

Now, by substitution:

$$ c + d = 8 \Rightarrow (10 - s) + d = 8 \Rightarrow d = 8 - 10 + s \Rightarrow d = -2 + s $$

$$ a + c = 2 \Rightarrow a + (10 - s) = 2 \Rightarrow a = 2 - 10 + s \Rightarrow a = -8 + s $$

Then:

$$ b + d = s \Rightarrow b + (-2 + s) = s \Rightarrow b = s + 2 - s \Rightarrow b = 2 $$

$$ a + b = 4 \Rightarrow (-8 + s) + 2 = 4 \Rightarrow -6 + s = 4 \Rightarrow \boxed{s = 10} $$

_Then find two different matrices that have the correct row and column sums:_

We now know from the previous evaluation that:

$$
a + b = 4 \\
c + d = 8 \\
a + c = 2 \\
b + d = 10 \\
$$

We are tasked now with finding two different matrices of the form:

$$
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

So, choose $d = 2$, then $b = 8$, $a = -4$, $c = 6$.

$$
\left[\begin{array}{cc}
-4 & 8 \\
6 & 2 \\
\end{array}\right]
$$

Then, choose $d = 3$, then $b = 7$, $a = -3$, $c = 5$.

$$
\left[\begin{array}{cc}
-3 & 7 \\
5 & 3 \\
\end{array}\right]
$$

27. Elimination in the usual order gives what matrix $U$ and what solution to
    this "lower triangular" system? We are really solving by _forward
    substitution_:

$$
3x = 3 \\
6x + 2y = 8 \\
9x - 2y + z = 9
$$

_Solution:_

This is essentially working with the lower triangular form, which is the
opposite of the upper triangular form. Just take the first line and work
_forward_ from there.

$$ 3x = 3 \Rightarrow x = 1 $$

$$ 6x + 2y = 8 \Rightarrow 6(1) + 2y = 8 \Rightarrow 6 + 2y = 8 \Rightarrow 2y = 2 \Rightarrow y = 1 $$

$$ 9x - 2y + z = 9 \Rightarrow 9(1) - 2(1) + z = 9 \Rightarrow 9 - 2 + z = 9 \Rightarrow 7 + z = 9 \Rightarrow z = 2 $$

So the solution is $(1, 1, 2)$.

The problem statement asks us now to show a matrix $U$ from this, which is just
the coefficient matrix of the lower triangular form given:

$$
\left[\begin{array}{ccc}
3 & 0 & 0 \\
6 & 2 & 0 \\
9 & -2 & 1 \\
\end{array}\right]
$$

28. (Omitted, no MATLAB).

---

Page 77

## Problem Set 2.3

**Problems 1-15 are about elimination matrices.**

1. Write down the 3 by 3 matrices that produce these elimination steps:

a. $E_{21}$ subtracts $5$ times row 1 from row 2.

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

b. $E_{32}$ subtracts $-7$ times row 2 from row 3.

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
$$

c. $P$ exchanges rows 1 and 2, then rows 2 and 3.

First, exchange rows 1 and 2:

$$ P =
\left[\begin{array}{rrr}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Then exchange rows 2 and 3:

$$ P =
\left[\begin{array}{rrr}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

2. In Problem 1, applying $E_{21}$ and then $E_{32}$ to $b = (1, 0, 0)$ gives
   $E_{32}E_{21}b =$ ____. Applying $E_{32}$ before $E_{21}$ gives
   $E_{21}E_{32}b =$ ____. When $E_{32}$ comes first, row ____ feels no effect
   from row ____.

_Applying $E_{21}$ and then $E_{32}$ to $b = (1, 0, 0)$ gives $E_{32}E_{21}b =$
(?):_

$$ b = \begin{bmatrix}{}1\\0\\0\end{bmatrix} $$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21}b =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix}
$$

For simplicity's sake, let's first multiply $E_{32}E_{21}$ before applying them
to $b$.

$$ E_{32}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
-35 & 7 & 1 \\
\end{array}\right]
$$

Now, to solve:

$$ E_{32}E_{21}b =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
-35 & 7 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\begin{bmatrix}{}1\\-5\\-35\end{bmatrix}
$$

_Applying $E_{32}$ before $E_{21}$ gives $E_{21}E_{32}b =$ (?):_

$$ E_{21}E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
$$

$$ E_{21}E_{32}b =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-5 & 1 & 0 \\
0 & 7 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\begin{bmatrix}{}1\\-5\\0\end{bmatrix}
$$

_When $E_{32}$ comes first, row (?) feels no effect from row (?):_.

3;1

The reason for this is because $E_{32}$ affects row 3 based off of row 2, then
$E_{21}$ affects row 2 from row 1, since row 2 has yet to be affected by row 1,
it follows that row 3 is influenced by row 2 before row 2 is influenced by row
1, and thus row 3 is never affected by row 1.

3. Which three matrices $E_{21}, E_{31}, E_{32}$ put $A$ into triangular form
   $U$?

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
4 & 6 & 1 \\
-2 & 2 & 0 \\
\end{array}\right]
$$

and

$$ E_{32}E_{31}E_{21}A = U $$

Multiply those $E$'s to get one matrix $M$ that does elimination: $MA = U$.

_Solution:_

Let's evaluate what $E_{21}$ should do since it comes first.

$E_{21}$ should subtract 4 times row 1 from row 2, thus:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Applying this to $A$ yields:

$$ E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
4 & 6 & 1 \\
-2 & 2 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
-2 & 2 & 0 \\
\end{array}\right]
$$

$E_{31}$ should subtract $-2$ times _current_ row 1 from row 3.

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right]
$$

Apply $E_{31}$ to $E_{21}A$:

$$ E_{31}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
-2 & 2 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 4 & 0 \\
\end{array}\right]
$$

$E_{32}$ should subtract $2$ times _current_ row 2 from row 3.

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

Apply $E_{32}$ to $E_{31}E_{21}A$:

$$ E_{32}E_{31}E_{21}A  =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 4 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 0 & -2 \\
\end{array}\right] = U
$$

Now to find $M$:

$$ E_{32}E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & -2 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{31}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
10 & -2 & 1 \\
\end{array}\right] = M
$$

4. Include $b = (1, 0, 0)$ as a fourth column in Problem 3 to produce
   $\left[\begin{array}{c}A & b \\\end{array}\right]$. Carry out elimination
   steps on this augmented matrix to solve $Ax = b$.

_Solution:_

Adding $b$ as a column to $A$ yields:

$$ \left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
4 & 6 & 1 & 0 \\
-2 & 2 & 0 & 0 \\
\end{array}\right]
$$

$E_{21}$ should subtract 4 times row 1 from row 2, thus:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Applying this to $\left[\begin{array}{cc}A & b\end{array}\right]$ yields:

$$ E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
4 & 6 & 1 & 0 \\
-2 & 2 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
0 & 2 & 1 & -4 \\
-2 & 2 & 0 & 0 \\
\end{array}\right]
$$

$E_{31}$ should subtract $-2$ times _current_ row 1 from row 3.

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right]
$$

Apply $E_{31}$ to $E_{21}\left[\begin{array}{cc}A & b\end{array}\right]$:

$$ E_{31}E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
0 & 2 & 1 & -4 \\
-2 & 2 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
0 & 2 & 1 & -4 \\
0 & 4 & 0 & 2 \\
\end{array}\right]
$$

$E_{32}$ should subtract $2$ times _current_ row 2 from row 3.

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

Apply $E_{32}$ to $E_{31}E_{21}\left[\begin{array}{cc}A & b\end{array}\right]$:

$$ E_{32}E_{31}E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
0 & 2 & 1 & -4 \\
0 & 4 & 0 & 2 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 1 & 0 & 1 \\
0 & 2 & 1 & -4 \\
0 & 0 & -2 & 10 \\
\end{array}\right]
$$

Back substitution gives $z = -5, y = \dfrac{1}{2}, x = \dfrac{1}{2}$. The
solution is $\boxed{\left(\dfrac{1}{2}, \dfrac{1}{2}, -5\right)}$

5. Suppose $a_{33} = 7$ and the third pivot is $5$. If you change $a_{33}$ to
   $11$, the third pivot is ____. If you change $a_{33}$ to ____, there is no
   third pivot.

_Solution:_

Changing $a_{33}$ from $7$ to $11$ will change the third pivot from
$5 + (11 - 7) = 5 + 4 = 9$.

If you change $a_{33}$ to $2$, there is no third pivot. The reason for this is
if $a_{33}$ and the third pivot is $5$, then it means that somewhere along the
process of elimination, $2$ was subtracted from $7$ to get $5$.

6. If every column of $A$ is a multiple of $(1, 1, 1)$, then $Ax$ is always a
   multiple of $(1, 1, 1)$. Do a 3 by 3 example. How many pivots are produced by
   elimination?

_Solution:_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 2 & 3 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$$ Ax =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 2 & 3 \\
1 & 2 & 3 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}x_1 + 2x_2 + 3x_3\\x_1 + 2x_2 + 3x_3\\x_1 + 2x_2 + 3x_3\end{bmatrix}
$$

Elimination:

$E_{21}$ subtracts 1 times row 1 from row 2.

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Apply $E_{21}$ to $A$:

$$ E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 2 & 3 \\
1 & 2 & 3 \\
1 & 2 & 3 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & 0 & 0 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$E_{31}$ subtracts 1 times row 1 from row 3.

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

Apply $E_{31}$ to $E_{21}A$:

$$ E_{31}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & 0 & 0 \\
1 & 2 & 3 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

_How many pivots are produced by elimination?:_

Exactly 1:

$$
\left[\begin{array}{rrr}
\boxed{1} & 2 & 3 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

7. Suppose $E$ subtracts $7$ times row 1 from row 3.

a. To _invert_ that step should ____ $7$ times row ____ to row ____.

_Solution:_

add; 1; 3

b. What "inverse matrix" $E^{-1}$ takes that reverse step (so $E^{-1}E = I$)?

$$ E^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
7 & 0 & 1 \\
\end{array}\right]
$$

c. If the reverse step is applied first (and then $E$) show that $EE^{-1} = I$.

$$ E =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-7 & 0 & 1 \\
\end{array}\right]
$$

$$ EE^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-7 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
7 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

8. The _determinant_ of
   $\left[\begin{array}{cc} a & b \\ c & d \\ \end{array}\right]$ is $\det M =
   ad - bc$. Subtract $\ell$ times row 1 from row 2 to produce a new $M^*$. Show
   that $\det M^* = \det M$ for every $\ell$. When $\ell = \dfrac{c}{a}$, _the
   product pivots equals the determinant:_ $(a)(d - \ell b)$ equals $ad - bc$.

_Solution:_

_Subtract $\ell$ times row 1 from row 2 to produce a new $M^*$:_

$$ M =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

$$ M^* =
\left[\begin{array}{cc}
a & b \\
c - \ell a & d - \ell b \\
\end{array}\right]
$$

_Show that $\det M^* = \det M$ for every $\ell$:_

If we compute the $\det M^*$:

$$ \det M^* = a(d - \ell b) - b(c - \ell a) $$

$$ = ad - \ell ba - bc + \ell ba $$

$$ = ad \cancel{- \ell ba} - bc \cancel{+ \ell ba} $$

$$ = ad - bc  = \det M $$

9.

a. $E_{21}$ subtracts row 1 from row 2 and then $P_{23}$ exchanges rows 2 and 3.
What matrix $M = P_{23}E_{21}$ does both steps at once?

_Solution:_

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_{23} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ P_{23}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
-1 & 1 & 0 \\
\end{array}\right] = M
$$

b. $P_{23}$ exchanges rows 2 and 3 and then $E_{31}$ subtracts row 1 from row 3.
What matrix $M = E_{31}P_{23}$ does both steps at once? Explain why the $M$'s
are the same but the $E$'s are different.

_Solution:_

$$ P_{23} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}P_{23} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
-1 & 1 & 0 \\
\end{array}\right] = M
$$

_Explanation:_

The reason is that we're doing the same operation, just in reverse. In part (b)
we first exchange rows 2 and 3, then subtract row 1 from row 2 (note that row 2
is the original row 3). Now, here in part (b), we instead first subtract row
from row 1 from row 3, then exchange row 2 and row 3 (and here, row 2 is the
original row 3 after row 1 was subtracted from the original row 3).

10.

a. What 3 by 3 matrix $E_{13}$ will add row 3 to row 1?

_Solution:_

$$ E_{13} =
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

b. What matrix adds row 1 to row 3 and _at the same time_ row 3 to row 1?

_Solution:_

$$
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 1 \\
\end{array}\right]
$$

c. What matrix adds row 1 to row 3 and _then_ adds row 3 to row 1?

_Solution:_

$$
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
1 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 1 \\
\end{array}\right]
$$

11. Create a matrix that has $a_{11} = a_{22} = a_{33} = 1$ but elimination
    produces two negatives pivots without row exchanges. (The first pivot is
    $1$.)

_Solution:_

Let

$$ A =
\left[\begin{array}{rrr}
1 & 2 & 2 \\
1 & 1 & 2 \\
1 & 2 & 1 \\
\end{array}\right]
$$

We are trying to get to:

$$
\left[\begin{array}{rrr}
1 & ? & ? \\
? & -? & ? \\
? & ? & -? \\
\end{array}\right]
$$

Solving $A$ by row, the first thing to do is to subtract row 1 from row 2, so:

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Then, subtract row 1 from row 3:

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

That is all that will be necessary, so find $E_{31}E_{21}$a

$$ E_{31}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

And now $E_{31}E_{21}A$:

$$ E_{31}E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 2 & 2 \\
1 & 1 & 2 \\
1 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 2 & 2 \\
0 & -1 & 0 \\
0 & 0 & -1 \\
\end{array}\right]
$$

This is our solution.

_Note:_ This one took me a while, just think about $A$ as being the identity
matrix but then change all the $0$'s to some other positive number to start,
then think on the row operations. I learned during this that the Elimination
matrices _cannot_ change the $1$'s from the original Identity matrix from which
they are based. This is because that would be scaling the original matrix's
constants, which is not what elimination is trying to do (on its face).

12. Multiply these matrices:

$$
\left[\begin{array}{ccc}
0 & 0 & 1\\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 3 & 1 \\
1 & 4 & 0 \\
\end{array}\right]
$$

_Solution:_

_First set of matrices:_

$$
\left[\begin{array}{ccc}
0 & 0 & 1\\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

Divide the problem up, first start with the first two matrices on the left:

$$
\left[\begin{array}{ccc}
0 & 0 & 1\\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 \\
\end{array}\right] =
\left[\begin{array}{ccc}
7 & 8 & 9 \\
4 & 5 & 6 \\
1 & 2 & 3 \\
\end{array}\right]
$$

Now, multiply this product matrix by the third matrix:

$$
\left[\begin{array}{ccc}
7 & 8 & 9 \\
4 & 5 & 6 \\
1 & 2 & 3 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
9 & 8 & 7 \\
6 & 5 & 4 \\
3 & 2 & 1 \\
\end{array}\right]
$$

Notice what has happened here, twice over we have multiplied by a "reverse
Identity matrix", also known as a permutation matrix. We have essentially
reversed the rows in the first multiplication, then reversed the columns in the
second (this is dependent on the order of matrices in the multiplication).

_Second set of matrices:_

$$
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 2 & 3 \\
1 & 3 & 1 \\
1 & 4 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & 1 & -2 \\
0 & 2 & -3 \\
\end{array}\right]
$$

_Note:_ This is two Elimination matrices (two subtractions, _i.e._ two row
operations), but the final form isn't upper triangular, so the elimination step
isn't finished.

13. Explain these facts. If the third column of $B$ is all zero, the third
    column of $EB$ is all zero (for any $E$). If the third _row_ of $B$ is all
    zero, the third row of $EB$ might _not_ be zero.

_Solution:_

_If the third column of $B$ is all zero, the third column of $EB$ is all zero
(for any $E$):_

Consider $B$:

$$ B =
\left[\begin{array}{ccc}
a & b & 0 \\
c & d & 0 \\
e & f & 0 \\
\end{array}\right]
$$

Now consider our elimination steps. In order to eliminate the first row's $a$,
$c - xa = 0$ must occur with $x$ being any positive scalar integer, leaving
$d - bx$. For simplicity's sake, let $x = 1$, then:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

and:

$$ E_{21}B =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & b & 0 \\
c & d & 0 \\
e & f & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
a - c & b & 0 \\
c - a & d - b & 0 \\
e & f & 0 \\
\end{array}\right]
$$

As long as $c - a = 0$, then we can continue multiplying this result by further
elimination matrices, but the ultimate idea is that the third row times the
third column (which again, consists of all $0$s), will always result in a
solution matrix where the third column is also all $0$s.

_If the third _row_ of $B$ is all zero, the third row of $EB$ might _not_ be
zero:_

Consider $B$:

$$ B =
\left[\begin{array}{ccc}
a & b & c \\
d & e & f \\
0 & 0 & 0 \\
\end{array}\right]
$$

Similar to the previous, we start the process of elimination:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}B =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & b & c \\
d & e & f \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
a - d & b & c \\
d - a & e - b & f - c \\
0 & 0 & 0 \\
\end{array}\right]
$$

Continuing in this way, it might appear that the third row will always be $0$,
but consider that sometimes the operations involved in elimination sometimes
involve adding two rows instead of subtraction.

For example, if we add row 2 to row 3 at this point during the elimination, we
get:

$$
E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
$$

And the elimination process continues as follows:

$$ E_{32}E_{21}B =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a - d & b & c \\
d - a & e - b & f - c \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
a - d & b & c \\
d - a & e - b & f - c \\
d - a & e - b & f - c \\
\end{array}\right]
$$

And it is certainly not always true that $d - a = 0, e - b = 0, f - c = 0$.

14. This 4 by 4 matrix will need elimination matrices $E_{21}$ and $E_{32}$ and
    $E_{43}$. What are those matrices?

$$ A =
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
-1 & 2 & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

_Solution:_

$E_{21}$ indicates that we must subtract row 1 from row 2 in some form (by some
scalar value) in order to get $a_{11} = 0$.

Evaluating for this, we get:

$$ -1 + x \cdot 2 = 0 $$

$$ 2x = 1 $$

$$ x = \frac{1}{2} $$

This is the scalar value, so $E_{21}$ is:

$$ E_{21} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
\frac{1}{2} & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Finding $E_{21}A$ is:

$$ E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
\frac{1}{2} & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
-1 & 2 & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

Moving on, we are tasked with then finding $E_{32}$, where row 2 is subtracted
from row 3. Again, row 2 might be multiplied by some scalar value so that the
product matrix has an entry of $a_{32} = 0$.

Evaluating the scalar value:

$$ -1 - y \cdot \frac{3}{2} = 0 $$

$$ -y \cdot \frac{3}{2} = 1 $$

$$ -y = \frac{2}{3} $$

We leave $-y$ as negative because $(E_{21}A)_{32} = -1$.

So, $E_{32}$ is:

$$ E_{32} =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & \frac{2}{3} & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Now to find $E_{32}E_{21}A$:

$$ E_{32}E_{21}A =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & \frac{2}{3} & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & 0 & \frac{4}{3} & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

Now to find $E_{43}$. Again, $E_{43}$ should subtract row 3 from row 4, where
row 3 is multiplied by some scalar value. Evaluating:

$$ -1 - z \cdot \frac{4}{3} = 0 $$

$$ -z \cdot \frac{4}{3} = 1 $$

$$ -z = \frac{3}{4} $$

Again, we leave $-z$ as negative, as $(E_{32}E_{21}A)_{43} = -1$.

Thus $E_{43}$ is:

$$ E_{43} =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & \frac{3}{4} & 1 \\
\end{array}\right]
$$

Now to find $E_{43}E_{32}E_{21}A$:

$$ E_{43}E_{32}E_{21}A  =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & \frac{3}{4} & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & 0 & \frac{4}{3} & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & 0 & \frac{4}{3} & -1 \\
0 & 0 & 0 & \frac{5}{4} \\
\end{array}\right]
$$

And we have reached upper triangular form.

So our elimination matrices are:

$$ E_{21} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
\frac{1}{2} & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & \frac{2}{3} & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{43} =
\left[\begin{array}{rrrr}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & \frac{3}{4} & 1 \\
\end{array}\right]
$$

15. Write down the 3 by 3 matrix that has $a_{ij} = 2i - 3j$. This matrix has
    $a_{32} = 0$, but elimination still needs $E_{32}$ to produce a zero in the
    $3, 2$ position. Which previous step destroys the original zero and what is
    $E_{32}$?

_Solution:_

_Write down the 3 by 3 matrix that has $a_{ij} = 2i - 3j$:_

$$ a_{11} = 2(1) - 3(1) = 2 - 3 = -1 $$

$$ a_{12} = 2(1) - 3(2) = 2 - 6 = -4 $$

$$ a_{13} = 2(1) - 3(3) = 2 - 9 = -7 $$

$$ a_{21} = 2(2) - 3(1) = 4 - 3 = 1 $$

$$ a_{22} = 2(2) - 3(2) = 4 - 6 = -2 $$

$$ a_{23} = 2(2) - 3(3) = 4 - 9 = -5 $$

$$ a_{31} = 2(3) - 3(1) = 6 - 3 = 3 $$

$$ a_{32} = 2(3) - 3(2) = 6 - 6 = 0 $$

$$ a_{33} = 2(3) - 3(3) = 6 - 9 = -3 $$

$$ A =
\left[\begin{array}{ccc}
-1 & -4 & -7 \\
1 & -2 & -5 \\
3 & 0 & -3 \\
\end{array}\right]
$$

_Which previous step destroys the original zero?:_

Let's just go through elimination on $A$ and see.

$$ A =
\left[\begin{array}{ccc}
-1 & -4 & -7 \\
1 & -2 & -5 \\
3 & 0 & -3 \\
\end{array}\right]
$$

For $E_{21}$, simply add row 1 to row 2:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Now, find $E_{21}A$:

$$ E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
1 & -2 & -5 \\
3 & 0 & -3 \\
\end{array}\right] =
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
0 & -6 & -12 \\
3 & 0 & -3 \\
\end{array}\right]
$$

Now for $E_{31}$, add 3 times row 1 to row 3:

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
$$

Now find $E_{31}E_{21}A$:

$$ E_{31}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
0 & -6 & -12 \\
3 & 0 & -3 \\
\end{array}\right] =
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
0 & -6 & -12 \\
0 & -12 & -24 \\
\end{array}\right]
$$

So, the step of elimination that "destroys" the original zero is $E_{31}$.

_What is $E_{32}$?:_

$E_{32}$ should subtract 2 times row 2 from row 3:

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

Double checking by calculating $E_{32}E_{31}E_{21}A$:

$$ E_{32}E_{31}E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
0 & -6 & -12 \\
0 & -12 & -24 \\
\end{array}\right] =
\left[\begin{array}{rrr}
-1 & -4 & -7 \\
0 & -6 & -12 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Notice that since the last row is all $0$'s, this tells us that matrix $A$ is
singular.

**Problems 16-23 are about creating and multiplying matrices.**

16. Write these ancient problems in a 2 by 2 matrix form $Ax = b$ and solve
    them:

a. $X$ is twice as old as $Y$ and their ages add to $33$.

$$ X = 2Y \text{ and } X + Y = 33 $$

$$
X - 2Y = 0 \\
X + Y = 33 \\
$$

$$ Ax =
\left[\begin{array}{rrr}
1 & -2 \\
1 & 1 \end{array}\right]
\begin{bmatrix}{}X\\Y\end{bmatrix} =
\begin{bmatrix}{}0\\33\end{bmatrix} = b
$$

Now to solve, eliminate and then back substitute. First, let's express $Ax = b$
as a single matrix:

$$ [Ax|b] =
\left[\begin{array}{cc|c}
1 & -2 & 0 \\
1 & 1 & 33 \\
\end{array}\right]
$$

So, $E_{21}$ should subtract 1 times row 1 from row 2:

$$ E_{21} =
\left[\begin{array}{rr}
1 & 0 \\
-1 & 1\\
\end{array}\right]
$$

Now to evaluate $E_{21}[Ax|b]$:

$$ E_{21}[Ax|b] =
\left[\begin{array}{rr}
1 & 0 \\
-1 & 1\\
\end{array}\right]
\left[\begin{array}{cc|c}
1 & -2 & 0 \\
1 & 1 & 33 \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & -2 & 0 \\
0 & 3 & 33 \\
\end{array}\right]
$$

So, $3Y = 33 \Rightarrow \boxed{Y = 11}$, then
$X - 2(11) = 0 \Rightarrow \boxed{X = 22}$.

b. $(x, y) = (2, 5)$ and $(3, 7)$ lie on the line $y = mx + c$. Find $m$ and
$c$.

$$
5 = 2m + c \\
7 = 3m + c \\
$$

Equivalently:

$$
2m + c = 5 \\
3m + c = 7 \\
$$

Written as a form of $[Ax | b]$:

$$ [Ax | b] =
\left[\begin{array}{cc|c}
2 & 1 & 5 \\
3 & 1 & 7 \\
\end{array}\right]
$$

$E_{21}$ subtracts 3/2 times row 1 from row 2:

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-\frac{3}{2} & 1 \\
\end{array}\right]
$$

Find $E_{21}[Ax|b]$:

$$ E_{21}[Ax|b] =
\left[\begin{array}{cc}
1 & 0 \\
-\frac{3}{2} & 1 \\
\end{array}\right]
\left[\begin{array}{cc|c}
2 & 1 & 5 \\
3 & 1 & 7 \\
\end{array}\right] =
\left[\begin{array}{cc|c}
2 & 1 & 5 \\
0 & -\frac{1}{2} & -\frac{1}{2} \\
\end{array}\right]
$$

So $-\dfrac{1}{2}c = -\dfrac{1}{2} \Rightarrow c = 1$, and also
$2m + 1(1) = 5 \Rightarrow m = 2$.

17. The parabola $y = a + bx + cx^2$ goes through the points $(x, y) = (1, 4)$
    and $(2, 8)$ and $(3, 14)$. Find and solve a matrix equation for the
    unknowns $(a, b, c)$.

_Solution:_

$$ y = a + bx + cx^2 $$

$$ (x, y) = (1, 4), (x, y)  = (2, 8), (x, y) = (3, 14) $$

$$
4 = a + b(1) + c(1)^2 \\
8 = a + b(2) + c(2)^2 \\
14 = a + b(3) + c(3)^2 \\
$$

Equivalently:

$$
a + b + c = 4 \\
a + 2b + 4c = 8 \\
a + 3b + 9c = 14 \\
$$

Treat this as an $[Ax | b]$ matrix:

$$ [Ax | b] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
1 & 2 & 4 & 8 \\
1 & 3 & 9 & 14
\end{array}\right]
$$

Now, eliminate and back substitute:

$$ [Ax | b] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
1 & 2 & 4 & 8 \\
1 & 3 & 9 & 14
\end{array}\right]
$$

$E_{21}$ should subtract 1 times row 1 from row 2:

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Now evaluate $E_{21}[Ax|b]$:

$$ E_{21}[Ax|b] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
1 & 2 & 4 & 8 \\
1 & 3 & 9 & 14
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & 1 & 3 & 4 \\
1 & 3 & 9 & 14 \\
\end{array}\right]
$$

Now, $E_{31}$ should subtract 1 times row 1 from row 3:

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

Find $E_{31}E_{21}[Ax|b]$:

$$ E_{31}E_{21}[Ax|b] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & 1 & 3 & 4 \\
1 & 3 & 9 & 14 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & 1 & 3 & 4 \\
0 & 2 & 8 & 10 \\
\end{array}\right]
$$

Now, $E_{32}$ should subtract 2 times row 2 from row 3.

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

Find $E_{32}E_{31}E_{21}[Ax|b]$:

$$ E_{32}E_{31}E_{21}[Ax|b] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & 1 & 3 & 4 \\
0 & 2 & 8 & 10 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & 1 & 3 & 4 \\
0 & 0 & 2 & 2 \\
\end{array}\right]
$$

Now back substitute:

$$ 2c = 2 \Rightarrow c = 1 $$

$$ y + 3(1) = 4 \Rightarrow y = 1 $$

$$ a + 1 + 1 = 4 \Rightarrow a = 2 $$

Thus $\boxed{(a, b, c) = (2, 1, 1)}$.

_Note:_

In the solutions section, Strang mentions that:

$$
\left[\begin{array}{ccc}
1 & 1 & 1\\
1 & 2 & 3 \\
1 & 3 & 9 \\
\end{array}\right]
$$

Is what is known as a
[**Vandermonde matrix**](https://en.wikipedia.org/wiki/Vandermonde_matrix).

18. Multiply these matrices in the orders $EF$ and $FE$.

$$ E =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right]
$$

$$ F =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right]
$$

Also compute $E^2 = EE$ and $F^3 = FFF$. You can guess $F^{100}$.

_Solution:_

$EF$:

$$ EF =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
b & c & 1 \\
\end{array}\right]
$$

$FE$:

$$ FE =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
ca + b & c & 1 \\
\end{array}\right]
$$

$E^2$:

$$ E^2 =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2a & 1 & 0 \\
2b & 0 & 1 \\
\end{array}\right]
$$

$F^3$:

$$ F^2 =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2c & 1 \\
\end{array}\right]
$$

$$ F^3 = F^2F =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2c & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 3c & 1 \\
\end{array}\right]
$$

$F^{100}$:

Guess for $F^{100}$, extrapolating from finding $F^3$ is:

$$ F^{100} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 100c & 1 \\
\end{array}\right]
$$

19. Multiply these row exchange matrices in the orders $PQ$ and $QP$ and $P^2$:

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

and

$$ Q =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

Find another non-diagonal matrix whose square is $M^2 = I$.

_Solution:_

$PQ$:

$$ PQ =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$QP$:

$$ QP =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$P^2$:

$$ P^2 =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

_Find another non-diagonal matrix whose square is $M^2 = I$:_

Try $Q^2$:

$$ Q^2 =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

So $Q = M$, and $Q^2 = M^2 = I$.

20.

a. Suppose all columns of $B$ are the same. Then all columns of $EB$ are the
same, because each one is $E$ times ____.

that column of $B$.

b. Suppose all rows of $B$ are
$\left[\begin{array}{ccc}1 & 2 & 4\\\end{array}\right]$. Show by example that
all rows of $EB$ are _not_
$\left[\begin{array}{ccc}1 & 2 & 4\\\end{array}\right]$. It is true that those
rows are ____.

_Show by example that all rows of $EB$ are _not_
$\left[\begin{array}{ccc}1 & 2 & 4\\\end{array}\right]$:_

Suppose $B$ is a 3x3 matrix, then:

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 4 \\
1 & 2 & 4 \\
1 & 2 & 4 \\
\end{array}\right]
$$

Now, let us begin elimination.

$E_{21}$ subtracts 1 times row 1 from row 2:

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Find $E_{21}B$:

$$ E_{21}B =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 4 \\
1 & 2 & 4 \\
1 & 2 & 4 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 2 & 4 \\
0 & 0 & 0 \\
1 & 2 & 4 \\
\end{array}\right]
$$

Right away, because all rows have the same coefficients (namely,
$\left[\begin{array}{ccc}
1 & 2 & 4 \\
\end{array}\right]$), upon trying even the first form of elimination, we are
left with a row that is all $0$'s. This implies that all rows of $EB$ are
multiples of $\left[\begin{array}{ccc}
1 & 2 & 4\\
\end{array}\right]$.

_It is true that those rows are (?):_

multiples of $\left[\begin{array}{ccc}
1 & 2 & 4 \\
\end{array}\right]$.

21. If $E$ adds row 1 to row 2 and $F$ adds row 2 to row 1, does $EF$ equal
    $FE$?

$$ E =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
$$

$$ F =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
$$

$$ EF =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$$ FE =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 1 \\
1 & 1 \\
\end{array}\right]
$$

So no, because:

$$ FE =
\left[\begin{array}{cc}
2 & 1 \\
1 & 1 \\
\end{array}\right] \neq
\left[\begin{array}{cc}
1 & 1 \\
1 & 2 \\
\end{array}\right] = EF
$$

22. The entries of $A$ and $x$ are $a_{ij}$ and $x_j$. So the first component of
    $Ax$ is $\sum{a_1jx_j} = a_{11}x_1 + \cdots + a_{1n}x_n$. If $E_{21}$
    subtracts row 1 from row 2, write a formula for

a. the third component of $Ax$

$$ (Ax)_{33} = \sum{a_{3j}x_j}$$

b. the $(2, 1)$ entry of $E_{21}A$

$$ a_{21} - a_{11} $$

c. the $(2, 1)$ entry of $E_{21}(E_{21}A)$

$$ a_{21} - 2a_{11} $$

d. the first component of $E_{21}Ax$

$$ (E_{21}Ax)_{11} = (EAx)_1 = (Ax)_1 = \sum{a_{1j}x_j} $$

23. The elimination matrix
    $E = \left[\begin{array}{cc} 1 & 0 \\ -2 & 1 \\ \end{array}\right]$
    subtracts $2$ times row 1 of $A$ from row 2 of $A$. The result is $EA$. What
    is the effect of $E(EA)$? In the opposite order $AE$, we are subtracting $2$
    times ____ of $A$ from ____. (Do examples.)

_What is the effect of $E(EA)$?:_

$E(EA)$ first simply does $EA$, where it subtracts 2 times row 1 from row 2.
Let's denote this:

$$ EA = r_2 - 2r_1 $$

Then $E(EA)$ subtracts 2 times row 1 from row EA:

$$ E(EA) = (r_2 - 2r_1) - 2r_1 \Rightarrow r_2 - 4r_1 $$

In effect, $E(EA)$ subtracts 4 times row 1 from row 2.

_In the opposite order $AE$, we are subtracting $2$ times (?) of $A$ from (?):_

column 2; column 1

_Do examples:_

Omitted.

**Problems 24-27 include the column $b$ in the augmented matrix
$\left[\begin{array}{cc} A & b \\ \end{array}\right]$.**

24. Apply elimination to the 2 by 3 augmented matrix
    $\left[\begin{array}{cc} A & b \\ \end{array}\right]$. What is the
    triangular system $Ux = c$? What is the solution $x$?

$$ Ax =
\left[\begin{array}{cc}
2 & 3 \\
4 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}1\\17\end{bmatrix}
$$

_Solution:_

$$ \left[\begin{array}{cc}
A & b\\
\end{array}\right] =
\left[\begin{array}{cc|c}
2 & 3 & 1\\
4 & 1 & 17 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
$$

$$ E_{21}\left[\begin{array}{cc}
A & b\\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc|c}
2 & 3 & 1\\
4 & 1 & 17 \\
\end{array}\right] =
\left[\begin{array}{cc|c}
2 & 3 & 1 \\
0 & -5 & 15 \\
\end{array}\right]
$$

Back substitution yields:

$$ -5x_2 = 15 \Rightarrow x_2 = -3 $$

$$ 2x_1 + 3(-3) = 1 \Rightarrow 2x_1 - 9 = 1 \Rightarrow x_1 = 5 $$

Thus:

$$ x = \begin{bmatrix}{}5\\-3\end{bmatrix} $$

25. Apply elimination to the 3 by 4 augmented matrix
    $\left[\begin{array}{cc} A & b \\ \end{array}\right]$. How do you know this
    system has no solution? Change the last number 6 so there _is_ a solution.

$$ Ax =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 3 & 4 \\
3 & 5 & 7 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}1\\2\\6\end{bmatrix}
$$

_Solution:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
2 & 3 & 4 & 2 \\
3 & 5 & 7 & 6 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
2 & 3 & 4 & 2 \\
3 & 5 & 7 & 6 \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
0 & -1 & -2 & 0 \\
3 & 5 & 7 & 6 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21}\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
0 & -1 & -2 & 0 \\
3 & 5 & 7 & 6 \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
0 & -1 & -2 & 0 \\
0 & -1 & -2 & 3 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{31}E_{21}\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
0 & -1 & -2 & 0 \\
0 & -1 & -2 & 3 \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 1 \\
0 & -1 & -2 & 0 \\
0 & 0 & 0 & 3 \\
\end{array}\right]
$$

And here we have $0z = 3$, for which there is no solution.

We can get a solution by changing the $6$ to a $3$:

$$ Ax =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 3 & 4 \\
3 & 5 & 7 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}1\\2\\3\end{bmatrix}
$$

This is because at elimination
$E_{32}E_{31}E_{21}\left[\begin{array}{cc}A & b \\\end{array}\right]$,
$-3 + 0 + 3 = 0$ will ultimately result in a $0z = 0$ back substitution, and
that will mean there are infinitely many solutions.

26. The equations $Ax = b$ and $Ax^* = b^*$ have the same matrix $A$. What
    double augmented matrix should you use in elimination to solve both
    equations at once? Solve both of these equations by working on a 2 by 4
    matrix:

$$
\left[\begin{array}{cc}
1 & 4 \\
2 & 7 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}1\\0\end{bmatrix}
$$

and

$$
\left[\begin{array}{cc}
1 & 4 \\
2 & 7 \\
\end{array}\right]
\begin{bmatrix}{}u\\v\end{bmatrix} =
\begin{bmatrix}{}0\\1\end{bmatrix}
$$

_Solution:_

Let's express $Ax = b$ as $\left[\begin{array}{cc}A & b\\\end{array}\right]$.

$$ \left[\begin{array}{cc}A & b\\\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 4 & 1 \\
2 & 7 & 0 \\
\end{array}\right]
$$

Similarly for $Ax^* = b^*$, expressed as
$\left[\begin{array}{cc}A^* & b^*\\\end{array}\right]$:

$$ \left[\begin{array}{cc}A^* & b^*\\\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 4 & 0 \\
2 & 7 & 1 \\
\end{array}\right]
$$

If we add $b + b^*$, we can find
$\left[\begin{array}{ccc}A & b & b^*\\\end{array}\right]$:

$$ \left[\begin{array}{ccc}A & b & b^*\\\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 4 & 1 & 0 \\
2 & 7 & 0 & 1 \\
\end{array}\right]
$$

Now, by elimination:

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
$$

$$ E_{21}\left[\begin{array}{ccc}A & b & b^*\\\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc|cc}
1 & 4 & 1 & 0 \\
2 & 7 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 4 & 1 & 0 \\
0 & -1 & -2 & 1 \\
\end{array}\right]
$$

This gives us both $b$ and $b^*$.

So, for $b$:

$$
-y = -2 \Rightarrow y = 2 \\
x + 4(2) = 1 \Rightarrow x = -7 \\
$$

Thus $x = \begin{bmatrix}{}-7\\2\end{bmatrix}$.

And, for $b^*$:

$$
-y^* = 1 \Rightarrow y = -1 \\
x^* + 4(-1) = 0 \Rightarrow x = 4 \\
$$

Thus $x^* = \begin{bmatrix}{}4\\-1\end{bmatrix}$.

27. Choose the numbers $a, b, c, d$ in this augmented matrix so that there is
    (a) no solution (b) infinitely many solutions.

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 2 & 3 & a \\
0 & 4 & 5 & b \\
0 & 0 & d & c \\
\end{array}\right]
$$

Which of the numbers $a, b, c$, or $d$ have no effect on the solvability?

Omitted.

28. If $AB = I$ and $BC = I$ use the associative law to prove $A = C$.

**Proof:**

Suppose $A, B, C$ are any matrices. Let $I$ denote the identity matrix.

Furthermore, suppose $AB = I$ and $BC = I$.

It is to be shown that $A = C$.

By the definition of the identity matrix, any matrix multiplied by $I$ will
return that same matrix back as the solution.

Then, it follows that:

$$ A = A(I) $$

By the supposition, since $BC = I$, it follows that:

$$ A(I) = A(BC) $$

By the associative law of matrices, it is known that:

$$ A(BC) = (AB)C $$

Then, by the supposition, since $AB = I$, it follows that:

$$ (AB)C = (I)C = C $$

In totality, this takes the form of:

$$ A = A(I) = A(BC) = (AB)C = I(C) = C $$

It can be derived from the law of equality that $A = C$, and this is what was to
be shown.

Q.E.D.

---

Page 88

## Problem Set 2.4

**Problems 1-16 are about the laws of matrix multiplication.**

1. $A$ is $3$ by $5$, $B$ is $5$ by $3$, $C$ is $5$ by $1$, and $D$ is $3$ by
   $1$. _All entries are $1$_. Which of these matrix operations are allowed, and
   what are the results?

$$ BA \quad AB \quad ABD \quad DC \quad A(B + C) $$

2. What rows or columns or matrices do you multiply to find

a. the second column of $AB$?

b. the first row of $AB$?

c. the entry in row 3, column 5 of $AB$?

d. the entry in row 1, column 1 of $CDE$?

3. Add $AB$ to $AC$ and compare with $A(B + C)$:

$$ A =
\left[\begin{array}{cc}
1 & 5 \\
2 & 3 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
0 & 2 \\
0 & 1 \\
\end{array}\right]
$$

and

$$ C =
\left[\begin{array}{cc}
3 & 1 \\
0 & 0 \\
\end{array}\right]
$$

4. In Problem 3, multiply $A$ times $BC$. Then multiply $AB$ times $C$.

5. Compute $A^2$ and $A^3$. Make a prediction for $A^5$ and $A^n$.

$$ A =
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{cc}
2 & 2 \\
0 & 0 \\
\end{array}\right]
$$

6. Show that $(A + B)^2$ is different from $A^2 + 2AB + B^2$, when

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right]
$$

Write down the correct rule for $(A + B)(A + B) = A^2 +$ ____ + $B^2$.

7. True or false. Give a specific example when false:

a. If columns 1 and 3 of $B$ are the same, so are columns 1 and 3 of $AB$.

b. If rows 1 and 3 of $B$ are the same, so are rows 1 and 3 of $AB$.

c. If rows 1 and 3 of $A$ are the same, so are rows 1 and 3 of $ABC$.

d. $(AB)^2 = A^2B^2$.

8. How is each row of $DA$ and $EA$ related to the rows of $A$, when

$$ D =
\left[\begin{array}{cc}
3 & 0 \\
0 & 5 \\
\end{array}\right]
$$

and

$$ E =
\left[\begin{array}{cc}
0 & 1 \\
0 & 1 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

How is each column of $AD$ and $AE$ related to the columns of $A$?

9. Row 1 of $A$ is added to row 2. This gives $EA$ below. Then column 1 of $EA$
   is added to column 2 to produce $(EA)F$:

$$ EA =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a & b \\
a + c & b + d \\
\end{array}\right]
$$

and

$$ (EA)F =
(EA)\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
a & a + b \\
a + c & a + c + b + d \\
\end{array}\right]
$$

a. Do those steps in the opposite order. First add column 1 of $A$ to column 2
by $AF$, then add row 1 of $AF$ to row 2 by $E(AF)$.

b. Compare with $(EA)F$. What law is obeyed by matrix multiplication?

10. Row 1 of $A$ is again added to row 2 to produce $EA$. Then $F$ adds row 2 of
    $EA$ to row 1. The result is $F(EA)$:

$$ F(EA) =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
a + c & b + d \\
\end{array}\right] =
\left[\begin{array}{cc}
2a + c & 2b + d \\
a + c & b + d \\
\end{array}\right]
$$

a. Do those steps in the opposite order: first add row 2 to row 1 by $FA$, then
add row 1 of $FA$ to row 2.

b. What law is or is not obeyed by matrix multiplication?

11. This fact still amazes me. IF you do a row operation on $A$ and then a
    column operation, the result is the same as if you did the column operation
    first. (Try it.) Why is this true?

12. (3 by 3 matrices) Choose the only $B$ so that for every matrix $A$

a. $BA = 4A$

b. $BA = 4B$

c. $BA$ has rows 1 and 3 of $A$ reversed and row 2 unchanged

d. All rows of $BA$ are the same as row 1 of $A$.

13. Suppose $AB = BA$ and $AC = CA$ for these two particular matrices $B$ and
    $C$:

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] \quad \text{ commutes with } \quad
B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] \quad \text{ and } \quad
C =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

Prove that $a = d$ and $b = c = 0$. Then $A$ is a multiple of $I$. The only
matrices that commute with $B$ and $C$ and all other 2 by 2 matrices are $A =$
multiple of $I$.

14. Which of the following matrices are guaranteed to equal $(A - B)^2$:
    $A^2 - B^2$, $(B - A)^2$, $A^2 - 2AB + B^2$, $A(A - B) - B(A - B)$,
    $A^2 - AB - BA + B^2$?

15. True or false:

a. If $A^2$ is defined then $A$ is necessarily square.

b. If $AB$ and $BA$ are defined then $A$ and $B$ are square.

c. If $AB$ and $BA$ are defined then $AB$ and $BA$ are square.

d. If $AB = B$ then $A = I$.

16. IF $A$ is $m$ by $n$, how many separate multiplications are involved when

a. $A$ multiplies a vector $x$ with $n$ components?

b. $A$ multiplies an $n$ by $p$ matrix $B$?

c. $A$ multiplies itself to produce $A^2$? Here $m = n$.

17. For $A = \left[\begin{array}{cc}2 & -1 \\3 & -2\\\end{array}\right]$ and
    $B = \left[\begin{array}{cc}1 & 0 & 4 \\1 & 0 & 6\\\end{array}\right]$,
    compute these answers _and nothing more_:

a. column 2 of $AB$

b. row 2 of $AB$

c. row 2 of $AA = A^2$

d. row 2 of $AAA = A^3$

**Problems 18-20 use $a_{ij}$ for the entry in row $i$, column $j$ of $A$.**

18. Write down the 3 by 3 matrix $A$ whose entries are

a. $a_{ij} = \text{ minimum of } i \text{ and } j$

b. $a_{ij} = (-1)^{i + j}$

c. $a_{ij} = \dfrac{i}{j}$

19. What words would you use to describe each of these classes of matrices? Give
    a 3 by 3 example in each class. Which matrix belongs to all four classes?

a. $a_{ij} = 0 \text{ if } i \neq j$

b. $a_{ij} = 0 \text{ if } i < j$

c. $a_{ij} = a_{ji}$

d. $a_{ij} = a_{1j}$

20. The entries of $A$ are $a_{ij}$. Assuming that zeros don't appear, what is

a. the first pivot?

b. the multiplier $\ell_{31}$ of row 1 to be subtracted from row 3?

c. the new entry that replaces $a_{32}$ after that subtraction?

d. the second pivot?

**Problems 21-24 involve powers of $A$.**

21. Compute $A^2, A^2, A^4$ and also $Av, A^2v, A^3v, A^4v$ for

$$ A =
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right] \quad \text{ and } \quad
v = \begin{bmatrix}{}x\\y\\z\\t\end{bmatrix}
$$

22. By trial and error find real nonzero 2 by 2 matrices such that

$$ A^2 = -I \quad BC = 0 \quad DE = -ED(\text{not allowing } DE = 0) $$

23.

a. Find a nonzero matrix $A$ for which $A^2 = 0$.

b. Find a matrix that has $A^2 \neq 0$ but $A^3 = 0$.

24. By experiment with $n = 2$ and $n = 3$ predict $A^n$ for these matrices:

$$ A_1 =
\left[\begin{array}{cc}
2 & 1 \\
0 & 1 \\
\end{array}\right] \quad \text{ and } \quad
A_2 =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] \quad \text{ and } \quad
A_3 =
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right]
$$

**Problems 25-31 use column-row multiplication and block multiplication.**

25. Multiply $A$ times $I$ using columns of $A$ (3 by 3) times rows of $I$.

26. Multiply $AB$ using columns times rows:

$$ AB =
\left[\begin{array}{cc}
1 & 0 \\
2 & 4 \\
2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
3 & 3 & 0 \\
1 & 2 & 1 \\
\end{array}\right] =
\begin{bmatrix}{}1\\1\\2\end{bmatrix}
\left[\begin{array}{ccc}
3 & 3 & 0 \\
\end{array}\right] + \text{(?)} = \text{(?)}
$$

27. Show that the product of upper triangular matrices is always upper
    triangular:

$$ AB =
\left[\begin{array}{ccc}
x & x & x \\
0 & x & x \\
0 & 0 & x \\
\end{array}\right]
\left[\begin{array}{ccc}
x & x & x \\
0 & x & x \\
0 & 0 & x \\
\end{array}\right] =
\left[\begin{array}{ccc}
\\
0 & \\
0 & 0 & \\
\end{array}\right]
$$

_Proof using dot products (Row times columns)_ (Row 2 of $A$) $\cdot$ (column 1
of $B$) $= 0$. Which other dot products give zeros?

_Proof using full matrices (Column times row)_ Draw $x$'s and $0$'s in (column 2
of $A$) times (row 2 of $B$). Also show (column 3 of $A$) times (row 3 of $B$).

28. Draw the cuts in $A$ (2 by 3) and $B$ (3 by 4) and $AB$ to show how each of
    the four multiplication rules is really a block multiplication:

(1) Matrix $A$ times columns of $B$. **Columns of $AB$**

(2) Rows of $A$ times the matrix $B$. **Rows of $AB$**

(3) Rows of $A$ times columns of $B$. **Inner products** (numbers in $AB$)

(4) Columns of $A$ times rows of $B$. **Outer products** (matrices add to $AB$)

29. Which matrices $E_{21}$ and $E_{31}$ produce zeros in the $(2, 1)$ and
    $(3, 1)$ positions of $E_{21}A$ and $E_{31}A$?

$$ A =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
-2 & 0 & 1 \\
8 & 5 & 3 \\
\end{array}\right]
$$

Find the single matrix $E = E_{31}E_{21}$ that produces both zeros at once.
Multiply $EA$.

30. Block multiplication says that column 1 is eliminated by

$$ EA =
\left[\begin{array}{cc}
1 & 0 \\
-\frac{c}{a} & I \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & D \\
\end{array}\right] =
\left[\begin{array}{cc}
a & b \\
0 & D - \frac{cb}{a} \\
\end{array}\right]
$$

In Problem 29, what numbers go into $c$ and $D$ and what is $D - \dfrac{cb}{a}$?

31. With $i^2 = -1$, the product of $(A + iB)$ and $(x + iy)$ is
    $Ax + iBx + iAy - By$. Use blocks to separate the real part without $i$ from
    the imaginary part that multiplies $i$:

$$
\left[\begin{array}{cc}
A & -B \\
\text{?} & \text{?} \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}Ax - By\\\text{?}\end{bmatrix} \quad
\begin{array}{l}
\text{ real part } \\
\text{ imaginary part } \\
\end{array}
$$

32. _(Very important)_ Suppose you solve $Ax = b$ for three special right sides
    $b$:

$$ Ax_1 = \begin{bmatrix}{}1\\0\\0\end{bmatrix} \quad \text{ and } \quad Ax_2 = \begin{bmatrix}{}0\\1\\0\end{bmatrix} \quad \text{ and } \quad Ax_3 = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

If the three solutions $x_1, x_2, x_3$ are the columns of a matrix $X$, what is
$A$ times $X$?

33. If the three solutions in Question 32 are $x_1 = (1, 1, 1)$ and
    $x_2 = (0, 1, 1)$ and $x_3 = (0, 0, 1)$, solve $Ax = b$ when
    $b = (3, 5, 8)$. Challenge problem: What is $A$?

34. Find all matrices
    $A = \left[\begin{array}{cc}a & b \\c & d \\\end{array}\right]$ that satisfy
    $A\left[\begin{array}{cc}1 & 1\\1 & 1\\\end{array}\right] = \left[\begin{array}{cc}1 & 1\\1 & 1\\\end{array}\right]A$.

35. Suppose a "circle graph" has 4 nodes connected (in both directions) by edges
    around a circle. What is its adjacency matrix $S$ from Worked Example 2.4 A?
    What is $S^2$? Find all the 2-step paths predicted by $S^2$.
