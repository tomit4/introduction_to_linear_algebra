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

_Solution:_

$BA$:

Since any matrix multiplied by another must have the number of columns in the
first matrix equal the number of rows in the second matrix:

$$ B_{5 \times 3} \cdot A_{3 \times 5} $$

is possible since $3 = 3$, and results in a solution of the following
dimensions:

$$ (BA)_{5 \times 5} $$

The result then is:

$$ BA =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccccc}
1 & 1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccccc}
3 & 3 & 3 & 3 & 3 \\
3 & 3 & 3 & 3 & 3 \\
3 & 3 & 3 & 3 & 3 \\
3 & 3 & 3 & 3 & 3 \\
3 & 3 & 3 & 3 & 3 \\
\end{array}\right]
$$

$AB$:

Since $A$ is 3 x 5 matrix and $B$ is a 5 x 3 matrix, this is possible since
$5 = 5$, $AB$ will have dimensions:

$$ A_{3 \times 5} \cdot B_{5 \times 3} = (AB)_{3 \times 3} $$

The solution then is:

$$ AB =
\left[\begin{array}{ccccc}
1 & 1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
5 & 5 & 5 \\
5 & 5 & 5 \\
5 & 5 & 5 \\
\end{array}\right]
$$

$ABD$:

From the previous part, we know that $AB$ is 3 x 3, and since $D$ is 3 x 1, this
is possible since $3 = 3$, and will result in a matrix of the following
dimensions:

$$ ABD_{3 \times 1} $$

The solution then is:

$$ ABD =
\left[\begin{array}{ccc}
5 & 5 & 5 \\
5 & 5 & 5 \\
5 & 5 & 5 \\
\end{array}\right]
\left[\begin{array}{c}
1 \\
1 \\
1 \\
\end{array}\right] =
\left[\begin{array}{c}
15 \\
15 \\
15 \\
\end{array}\right]
$$

$DC$:

Since $D$ is 3 X 1 and $C$ is 5 X 1, this is not possible since $1 \neq 5$.

$A(B + C)$:

$B$ and $C$ cannot be added as matrix addition requires both matrices to have
the same number of rows _and_ same number of columns, and $B$ is 5 x 3 and $C$
is 5 x 1.

2. What rows or columns or matrices do you multiply to find

a. the second column of $AB$?

all rows of $A$ times the second column of $B$, or more succinctly:

$$ A(B_{i2}) $$

b. the first row of $AB$?

$$ A_{1j}B $$

c. the entry in row 3, column 5 of $AB$?

$$ A_{3j}B_{i5} $$

d. the entry in row 1, column 1 of $CDE$?

$$ (C_{1j}D)E_{i1} $$

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

_Solution:_

$$ AB =
\left[\begin{array}{cc}
1 & 5 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 2 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 7 \\
0 & 7 \\
\end{array}\right]
$$

$$ AC =
\left[\begin{array}{cc}
1 & 5 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 1 \\
6 & 2 \\
\end{array}\right]
$$

$$ AB + AC =
\left[\begin{array}{cc}
0 & 7 \\
0 & 7 \\
\end{array}\right] +
\left[\begin{array}{cc}
3 & 1 \\
6 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 8 \\
6 & 9 \\
\end{array}\right]
$$

$$ B + C =
\left[\begin{array}{cc}
0 & 2 \\
0 & 1 \\
\end{array}\right] +
\left[\begin{array}{cc}
3 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 3 \\
0 & 1 \\
\end{array}\right]
$$

$$ A(B + C) =
\left[\begin{array}{cc}
1 & 5 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 3 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 8 \\
6 & 9 \\
\end{array}\right] = AB + AC
$$

This demonstrates the distributive law of matrices.

4. In Problem 3, multiply $A$ times $BC$. Then multiply $AB$ times $C$.

_Solution:_

$$ BC =
\left[\begin{array}{cc}
0 & 2 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ A(BC) =
\left[\begin{array}{cc}
1 & 5 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

From problem 3, we know that:

$$ AB =
\left[\begin{array}{cc}
0 & 7 \\
0 & 7 \\
\end{array}\right]
$$

$$ (AB)C =
\left[\begin{array}{cc}
0 & 7 \\
0 & 7 \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right] = A(BC)
$$

This demonstrates the associative law of matrices.

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

_Solution:_

_First definition for $A$:_

$$ A =
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right]
$$

$$ A^2 =
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2b \\
0 & 1 \\
\end{array}\right]
$$

$$ A^3 = (A^2)A =
\left[\begin{array}{cc}
1 & 2b \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 3b \\
0 & 1 \\
\end{array}\right]
$$

Prediction for $A^5$:

$$
\left[\begin{array}{cc}
1 & 5b \\
0 & 1 \\
\end{array}\right]
$$

Prediction for $A^n$:

$$
\left[\begin{array}{cc}
1 & nb \\
0 & 1 \\
\end{array}\right]
$$

_Second definition for $A$:_

$$ A =
\left[\begin{array}{cc}
2 & 2 \\
0 & 0 \\
\end{array}\right]
$$

$$ A^2 =
\left[\begin{array}{cc}
2 & 2 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 2 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
4 & 4 \\
0 & 0 \\
\end{array}\right]
$$

$$ A^3 = (A^2)A =
\left[\begin{array}{cc}
4 & 4 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 2 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
8 & 8 \\
0 & 0 \\
\end{array}\right]
$$

Prediction for $A^5$:

$$ A^5 =
\left[\begin{array}{cc}
2^5 & 2^5 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
32 & 32 \\
0 & 0 \\
\end{array}\right]
$$

Prediction for $A^n$:

$$ A^n =
\left[\begin{array}{cc}
2^n & 2^n \\
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

_Solution:_

_Show that $(A + B)^2$ is different from $A^2 + 2AB + B^2$:_

$$ A + B =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 2 \\
3 & 0 \\
\end{array}\right]
$$

$$ (A + B)^2 =
\left[\begin{array}{cc}
2 & 2 \\
3 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 2 \\
3 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
10 & 4 \\
6 & 6 \\
\end{array}\right]
$$

$$ A^2 =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right]
$$

$$ B^2 =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right]
$$

$$ AB =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
7 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ 2AB =
2\left[\begin{array}{cc}
7 & 0 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
14 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ A^2 + 2AB + B^2 =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
14 & 0 \\
0 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
16 & 2 \\
3 & 0 \\
\end{array}\right] \neq
\left[\begin{array}{cc}
10 & 4 \\
6 & 6 \\
\end{array}\right] = (A + B)^2
$$

_Write down the correct rule for $(A + B)(A + B) = A^2 +$ (?) + $B^2$:_

We can still FOIL out $(A + B)(A + B)$, we just have to keep in mind that matrix
multiplication is not commutative, so:

$$ (A + B)(A + B) = \boxed{A^2 + AB + BA + B^2} $$

7. True or false. Give a specific example when false:

a. If columns 1 and 3 of $B$ are the same, so are columns 1 and 3 of $AB$.

$$ B =
\left[\begin{array}{ccc}
a & b & a \\
c & d & c \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{cc}
e & f \\
g & h \\
\end{array}\right]
$$

$$ AB =
\left[\begin{array}{cc}
e & f \\
g & h \\
\end{array}\right]
\left[\begin{array}{ccc}
a & b & a \\
c & d & c \\
\end{array}\right] =
\left[\begin{array}{ccc}
ae + cg & be + df & ae + cg \\
ag + ch & bg + dh & ag + ch \\
\end{array}\right]
$$

Yes, this is true.

b. If rows 1 and 3 of $B$ are the same, so are rows 1 and 3 of $AB$.

I guess this is false.

$$ A =
\left[\begin{array}{ccc}
e & f & g \\
h & i & j \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
a & b \\
c & d \\
a & b \\
\end{array}\right]
$$

$$ AB =
\left[\begin{array}{ccc}
e & f & g \\
h & i & j \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
a & b \\
\end{array}\right] =
\left[\begin{array}{ccc}
ae + cf + ag & be + df + bg \\
ah + ci + aj & bh + di + bj \\
\end{array}\right]
$$

So definitely false, especially since there is no row 3 of $AB$ (which is
allowed since the matrix multiplication is correct and $A$ is never given any
constraints, $A$ can be any matrix which can be multiplied such that $AB$
exists.)

c. If rows 1 and 3 of $A$ are the same, so are rows 1 and 3 of $ABC$.

Perhaps true.

$$ A =
\left[\begin{array}{c}
a \\
b \\
a \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
c & d & e \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{c}
f \\
g \\
h \\
\end{array}\right]
$$

$$ AB =
\left[\begin{array}{c}
a \\
b \\
a \\
\end{array}\right]
\left[\begin{array}{ccc}
c & d & e \\
\end{array}\right] =
\left[\begin{array}{c}
ac & ad & ae \\
bc & bd & be \\
ac & ad & ae \\
\end{array}\right]
$$

$$ ABC = (AB)C =
\left[\begin{array}{c}
ac & ad & ae \\
bc & bd & be \\
ac & ad & ae \\
\end{array}\right]
\left[\begin{array}{c}
f \\
g \\
h \\
\end{array}\right] =
\left[\begin{array}{c}
acf + adg + aeh \\
bcf + bdg + beh \\
acf + adg + aeh \\
\end{array}\right]
$$

So yes, this is true.

d. $(AB)^2 = A^2B^2$.

This is false since $AB^2 = ABAB = (AB)(AB) \neq (AA)(BB) = AABB = A^2B^2$.

Example omitted (this just demonstrates how matrix associativity works).

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

_Solution:_

_How is each row of $DA$ and $EA$ related to the rows of $A$?:_

$$ DA =
\left[\begin{array}{cc}
3 & 0 \\
0 & 5 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
3a & 3b \\
5c & 5d \\
\end{array}\right]
$$

$$ EA =
\left[\begin{array}{cc}
0 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
c & d \\
c & d \\
\end{array}\right]
$$

Each row of $DA$ is related to $A$ in that row $(DA)_{1j}$ multiplies row
$A_{1j}$ by $3$, and row $(DA)_{2j}$ multiplies row $A_{2j}$ by $5$.$and

Each row of $EA$ is related to $A$ in that each row of $EA$ is equal to row
$A_{2j}$.

_How is each column of $AD$ and $AE$ related to the columns of $A$?:_

$$ AD =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 0 \\
0 & 5 \\
\end{array}\right] =
\left[\begin{array}{cc}
3a & 5b \\
3c & 5d \\
\end{array}\right]
$$

$$ AE =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & a + b \\
0 & c + d \\
\end{array}\right]
$$

Each column of $AD$ is related to columns of $A$ by multiplying column $A_{i1}$
by $3$ to get $(AD)_{i1}$. Similarly, multiplying column $A_{i2}$ by $5$ to get
$(AD)_{i2}$.

Each column of $AE$ is related to columns of $A$ by adding $A_{i1}$ to $A_{i2}$
to get $(AE)_{i2}$. Note that $(AE)_{i1} = 0$, which is the same as $E_{i1}$.

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

_Solution:_

$$ AF =
\left[\begin{array}{ccc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
a & a + b \\
c & c + d \\
\end{array}\right]
$$

$$ E(AF) =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & a + b \\
c & c + d \\
\end{array}\right] =
\left[\begin{array}{cc}
a & a + b \\
a + c & a + b + c + d \\
\end{array}\right] = (EA)F
$$

b. Compare with $(EA)F$. What law is obeyed by matrix multiplication?

_Solution:_

The law of associativity.

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

_Solution:_

$$ FA =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a + c & b + d \\
c & d \\
\end{array}\right]
$$

Adding row 1 of $FA$ to row 2 is to apply $E$:

$$ E(FA) =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a + c & b + d \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a + c & b + d \\
a + 2c & b + 2d \\
\end{array}\right] \neq
\left[\begin{array}{cc}
2a + c & 2b + d \\
a + c & b + d \\
\end{array}\right] = F(EA)
$$

b. What law is or is not obeyed by matrix multiplication?

_Solution:_

This demonstrates that matrix multiplication does not obey the laws of
commutativity.

11. This fact still amazes me. IF you do a row operation on $A$ and then a
    column operation, the result is the same as if you did the column operation
    first. (Try it.) Why is this true?

_Solution:_

Let $A$ be the $A$ from the previous 2 problems:

$$ A = \left[\begin{array}{cc} a & b \\ c & d \\ \end{array}\right] $$

Now apply a row operation, let's call this operation matrix $R$ (row operations
go to the left in matrix multiplication):

$$ RA =
\left[\begin{array}{cc}
2 & 0 \\
0 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
2a & 2b\\
2c & 2d \\
\end{array}\right]
$$

Now apply a column operation $C$ on $RA$ (column operations go on the right side
of matrix multiplication):

$$ (RA)C =
\left[\begin{array}{cc}
2a & 2b\\
2c & 2d \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 0 \\
0 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
6a & 6b \\
6c & 6d \\
\end{array}\right]
$$

Now, do the column operation first, _i.e._ compute $AC$ (again, column goes on
the right):

$$ AC =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 0 \\
0 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
3a & 3b \\
3c & 3d \\
\end{array}\right]
$$

Then apply $R$ (again, row operations on the left), $R(AC)$:

$$ R(AC) =
\left[\begin{array}{cc}
2 & 0 \\
0 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
3a & 3b \\
3c & 3d \\
\end{array}\right] =
\left[\begin{array}{cc}
6a & 6b \\
6c & 6d \\
\end{array}\right] = (RA)C
$$

This is true because the fact that the row and column operations determine the
order in which the matrix multiplication occurs means that regardless of whether
you start with rows or columns, which matrix goes on the left or the right will
always be the same regardless of which multiplication you do first. This is yet
another demonstration of the law of associativity.

12. (3 by 3 matrices) Choose the only $B$ so that for every matrix $A$

a. $BA = 4A$

$$ B = 4 \cdot I =
\left[\begin{array}{ccc}
4 & 0 & 0 \\
0 & 4 & 0 \\
0 & 0 & 4 \\
\end{array}\right]
$$

b. $BA = 4B$

$$ B = \mathbf{0} $$

c. $BA$ has rows 1 and 3 of $A$ reversed and row 2 unchanged

$$ B =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

d. All rows of $BA$ are the same as row 1 of $A$.

$$ B =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 0 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

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

_Solution:_

_Proof:_

Suppose $A$, $B$, and $C$ are matrices defined as follows:

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

$$
B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$
C =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

Furthermore, suppose that $AB = BA$ (_i.e._ $A$ and $B$ are commutative), and
also suppose that $AC = CA$ (_i.e._ $A$ and $C$ are commutative).

It is to be shown that $a = d$ and $b = c = 0$.

Consider what happens when $AB$ and $BA$ are multiplied via demonstration:

$$ AB =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
a & 0 \\
c & 0 \\
\end{array}\right]
$$

$$ BA =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right]
$$

By the supposition, $AB = BA$, thus it follows that:

$$
AB =
\left[\begin{array}{cc}
a & 0 \\
c & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right] = BA
$$

By the laws of equality, this means that $b = c = 0$.

Similarly, computing $AC$ and $CA$ yields:

$$ AC =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & a \\
0 & c \\
\end{array}\right]
$$

$$ CA =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
c & d \\
0 & 0 \\
\end{array}\right]
$$

By the supposition, since $AC = CA$, the following equality holds:

$$ AC =
\left[\begin{array}{cc}
0 & a \\
0 & c \\
\end{array}\right] =
\left[\begin{array}{cc}
c & d \\
0 & 0 \\
\end{array}\right] = CA
$$

Once again, it follows by the laws of equality that $a = d$.

Thus both $a = d$ and $b = c = 0$ have been demonstrated, and this is what was
to be shown.

Q.E.D.

14. Which of the following matrices are guaranteed to equal $(A - B)^2$:
    $A^2 - B^2$, $(B - A)^2$, $A^2 - 2AB + B^2$, $A(A - B) - B(A - B)$,
    $A^2 - AB - BA + B^2$?

To easily see which ones, let's FOIL out $(A - B)^2$:

$$ (A - B)^2 = (A - B)(A - B) $$

$$ = A^2 - AB - BA + B^2 $$

Easily we can see the first option $A^2 - B^2 \neq A^2 - AB - BA + B^2$.

The second option, $(B - A)^2$ can be evaluated similarly via FOIL:

$$ (B - A)^2 = (B - A)(B - A) $$

$$ = B^2 - BA - AB + A^2 = A^2 - AB - BA + B^2 $$

So this second option is equivalent.

The third option $A^2 - 2AB + B^2 \neq A^2 - AB - BA + B^2$ as matrix
multiplication does not conform to the laws of commutativity.

The fourth option $A(A - B) - B(A - B)$ can be FOILed out:

$$ A(A - B) - B(A - B) = A^2 - AB - BA + B^2 $$

So this is equal.

The fifth option is the fully foiled out version of $(A - B)^2$ and thus is
equal.

15. True or false:

a. If $A^2$ is defined then $A$ is necessarily square.

True, since $A_{r \times c} \cdot A_{c \times r}$ must hold, by the laws of
matrix multiplication, this means that $r = c$, which means that $A$ is a square
matrix.

b. If $AB$ and $BA$ are defined then $A$ and $B$ are square.

Not necessarily, no, this is false, consider:

$$ A_{1 \times 2} \cdot B_{2 \times 1} = (AB)_{1 \times 1} $$

This is valid, as $A$'s columns is $2$ which is equal to $B$'s rows. Thus matrix
multiplication of $AB$ is valid.

Similarly, as $B$'s columns and $A$'s rows are both equal to $1$, this is also
valid matrix multiplication

$AB$ is indeed square (a 1 x 1 matrix), and $BA$ is indeed square (a 2 x 2
matrix), but neither $A$ nor $B$ are square.

c. If $AB$ and $BA$ are defined then $AB$ and $BA$ are square.

By part (b), this is true, but let's establish a more general sense as to why:

$$ A_{m \times n} \cdot B_{n \times m} = (AB)_{m \times m}  $$

$$ B_{n \times m} \cdot A_{m \times n} = (BA)_{n \times n} $$

Both of these are square matrices.

d. If $AB = B$ then $A = I$.

Not necessarily, if $B = \mathbf{0}$, then $AB = B = \mathbf{0} \neq I$. So this
is false.

16. IF $A$ is $m$ by $n$, how many separate multiplications are involved when

a. $A$ multiplies a vector $x$ with $n$ components?

$mn$ (use every entry of $A$).

b. $A$ multiplies an $n$ by $p$ matrix $B$?

$mnp$ (part (a) by the rows of $B$, which is $p$)

c. $A$ multiplies itself to produce $A^2$? Here $m = n$.

$n^3$ ($n^2$ dot products.)

_Note:_ Interestingly, if you think about this, this means matrix multiplication
have terrible time complexity (roughly $O(n^3)$ according to research). This is
why GPU's make use of parallelization in data science and graphics processing
tasks to by pass this poor time efficiency.

17. For $A = \left[\begin{array}{cc}2 & -1 \\3 & -2\\\end{array}\right]$ and
    $B = \left[\begin{array}{cc}1 & 0 & 4 \\1 & 0 & 6\\\end{array}\right]$,
    compute these answers _and nothing more_:

Recall problem 2, this is similar.

a. column 2 of $AB$

$$ A(B_{i2}) $$

$$ (AB)_{i2} = \begin{bmatrix}{}0\\0\end{bmatrix} $$

b. row 2 of $AB$

$$ A_{2j}B $$

$$ (AB)_{2j} =
\left[\begin{array}{ccc}
1 & 0 & 0\\
\end{array}\right]
$$

c. row 2 of $AA = A^2$

$$ A_{2j}A $$

$$ (AA)_{2j} =
\left[\begin{array}{cc}
0 & 1 \\
\end{array}\right]
$$

d. row 2 of $AAA = A^3$

$$ (AA)_{2j}A $$

$$ (AAA)_{2j} =
\left[\begin{array}{cc}
3 & -2 \\
\end{array}\right]
$$

**Problems 18-20 use $a_{ij}$ for the entry in row $i$, column $j$ of $A$.**

18. Write down the 3 by 3 matrix $A$ whose entries are

Throughout this, keep in mind that $i = 1, 2, 3$ and $j = 1, 2, 3$.

a. $a_{ij} = \text{ minimum of } i \text{ and } j$

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

b. $a_{ij} = (-1)^{i + j}$

$$ A =
\left[\begin{array}{rrr}
1 & -1 & 1 \\
-1 & 1 & -1 \\
1 & -1 & 1 \\
\end{array}\right]
$$

c. $a_{ij} = \dfrac{i}{j}$

$$ A =
\left[\begin{array}{ccc}
1 & \frac{1}{2} & \frac{1}{3} \\
2 & 1 & \frac{2}{3} \\
3 & \frac{3}{2} & 1 \\
\end{array}\right]
$$

19. What words would you use to describe each of these classes of matrices? Give
    a 3 by 3 example in each class. Which matrix belongs to all four classes?

_Note:_

Base example:

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33} \\
\end{array}\right]
$$

a. $a_{ij} = 0 \text{ if } i \neq j$

$$ A =
\left[\begin{array}{ccc}
a_{11} & 0 & 0 \\
0 & a_{22} & 0 \\
0 & 0 & a_{33} \\
\end{array}\right]
$$

This is a Diagonal Matrix, where only the diagonal can be nonzero.

b. $a_{ij} = 0 \text{ if } i < j$

$$ A =
\left[\begin{array}{ccc}
a_{11} & 0 & 0 \\
a_{21} & a_{22} & 0 \\
a_{31} & a_{32} & a_{33} \\
\end{array}\right]
$$

This is in lower triangular form, and thus is a Lower Triangular Matrix.

c. $a_{ij} = a_{ji}$

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{21} & a_{31} \\
a_{12} & a_{22} & a_{32} \\
a_{13} & a_{23} & a_{33} \\
\end{array}\right]
$$

This matrix is a Symmetric matrix, the entries are mirrored along the main
diagonal.

d. $a_{ij} = a_{1j}$

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{11} & a_{12} & a_{13} \\
a_{11} & a_{12} & a_{13} \\
\end{array}\right]
$$

This matrix has the same entries in each of its columns, and each row is the
same.

_Which matrix belongs to all four classes?:_

The $\mathbf{0}$ matrix.

20. The entries of $A$ are $a_{ij}$. Assuming that zeros don't appear, what is

a. the first pivot?

$a_{11}$

b. the multiplier $\ell_{31}$ of row 1 to be subtracted from row 3?

$\dfrac{a_{31}}{a_{11}}$

c. the new entry that replaces $a_{32}$ after that subtraction?

$$ a_{32} - \dfrac{a_{31}a_{12}}{a_{11}} $$

d. the second pivot?

$$ a_{22} - \dfrac{a_{21}a_{12}}{a_{11}} $$

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

$A^2$:

$$ A^2 =
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 0 & 4 & 0 \\
0 & 0 & 0 & 4 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$A^3$:

$$ A^3 = (A^2)A =
\left[\begin{array}{cccc}
0 & 0 & 4 & 0 \\
0 & 0 & 0 & 4 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 0 & 0 & 8 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$A^4$:

$$ A^4 = (A^3)A =
\left[\begin{array}{cccc}
0 & 0 & 0 & 8 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right] = \mathbf{0}
$$

$Av$:

$$ Av =
\left[\begin{array}{cccc}
0 & 2 & 0 & 0 \\
0 & 0 & 2 & 0 \\
0 & 0 & 0 & 2 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}2y\\2z\\2t\\0\end{bmatrix}
$$

$A^2v$:

$$ A^2v =
\left[\begin{array}{cccc}
0 & 0 & 4 & 0 \\
0 & 0 & 0 & 4 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}4z\\4t\\0\\0\end{bmatrix}
$$

$A^3v$:

$$ A^3v =
\left[\begin{array}{cccc}
0 & 0 & 0 & 8 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}8t\\0\\0\\0\end{bmatrix}
$$

$A^4v$:

$$ A^4v =
\left[\begin{array}{cccc}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}0\\0\\0\\0\end{bmatrix}
$$

22. By trial and error find real nonzero 2 by 2 matrices such that

$$ A^2 = -I \quad BC = 0 \quad DE = -ED(\text{not allowing } DE = 0) $$

$A^2 = -I$:

$$ -I =
-1\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
-1 & 0 \\
0 & -1 \\
\end{array}\right]
$$

$$ A^2 =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a^2 + bc = -1 & ab + bd = 0 \\
ca + dc = 0 & cb + d^2 = -1 \\
\end{array}\right]
$$

$$
a^2 + bc = -1 \\
ca + dc = 0 \\
ab + bd = 0 \\
cb + d^2 = -1 \\
$$

Infinitely many solutions, just find one that works, set $a = 0$ and $d = 0$,
then:

$$
(0)^2 + bc = -1 \\
c(0) + (0)c = 0 \\
(0)b + b(0) = 0 \\
cb + (0)^2 = -1 \\
$$

$$
bc = -1 \\
cb = -1 \\
$$

So either $b = 1, c = -1$ or $b = -1, c = 1$.

Choose $b = 1, c = -1$, then:

$$ A =
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
$$

Check:

$$ A^2 =
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
-1 & 0 \\
0 & -1 \\
\end{array}\right] = -I
$$

$BC = \mathbf{0}$:

$$ BC =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
e & f \\
g & i \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$
ae + bg = 0 \\
ce + dg = 0 \\
af + bi = 0 \\
cf + di = 0 \\
$$

By evaluation, we can go slowly and find entries that will work:

$$
ae + bg = 0 \\
(-1)(1) + (-1)(-1) = 0 \\
ce + dg = 0 \\
(-1)(1) + (-1)(-1) = 0 \\
af + bi = 0 \\
(-1)(-1) + (-1)(1) = 0 \\
cf + di = 0 \\
(-1)(-1) + (-1)(1) = 0 \\
$$

$$ a = -1, b = -1, c = -1, d = -1, e = 1, f = -1, g = -1, i = 1 $$

This works, so:

$$ BC =
\left[\begin{array}{cc}
-1 & -1 \\
-1 & -1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & -1 \\
-1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$DE = -ED$ (not allowing $DE$ = 0):

Doing this got complex, try $A$ from earlier:

$$ A = E =
\left[\begin{array}{rr}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
$$

Try the permutation matrix for $D$:

$$ D =
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right]
$$

Then:

$$ DE =
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right]
\left[\begin{array}{rr}
0 & 1 \\
-1 & 0 \\
\end{array}\right] =
\left[\begin{array}{rr}
-1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

Then find $ED$:

$$ ED =
\left[\begin{array}{rr}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{rr}
1 & 0 \\
0 & -1 \\
\end{array}\right]
$$

Then find $-ED$:

$$ -ED =
-1\left[\begin{array}{rr}
1 & 0 \\
0 & -1 \\
\end{array}\right] =
\left[\begin{array}{rr}
-1 & 0 \\
0 & 1 \\
\end{array}\right] = DE
$$

23.

a. Find a nonzero matrix $A$ for which $A^2 = 0$.

$$ A^2 =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$
a^2 + bc = 0 \\
ca + dc = 0 \\
ab + bd = 0 \\
cb + d^2 = 0 \\
$$

Choose $a = -1, b = 1, c = -1, d = 1$, then:

$$
a^2 + bc = (-1)(-1) + (1)(-1) = 0 \\
ca + dc = (-1)(-1) + (1)(-1) = 0 \\
ab + bd = (-1)(1) + (1)(1) = 0 \\
cb + d^2 = (-1)(1) + (1)(1) = 0 \\
$$

So this works, let's fill in:

$$ A =
\left[\begin{array}{cc}
-1 & 1 \\
-1 & 1 \\
\end{array}\right]
$$

Checking:

$$ A^2 =
\left[\begin{array}{cc}
-1 & 1 \\
-1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
-1 & 1 \\
-1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

b. Find a matrix that has $A^2 \neq 0$ but $A^3 = 0$.

Try an upper triangular matrix:

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 0\\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

As seen in problem 21, this will eventually become $\mathbf{0}$ the more we
continually exponentiate upon it:

$$ A^2 =
\left[\begin{array}{ccc}
0 & 1 & 0\\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0\\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ A^3 = (A^2)A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0\\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0\\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

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

$A_1$:

$$ A_1 =
\left[\begin{array}{cc}
2 & 1 \\
0 & 1 \\
\end{array}\right]
$$

$$ A_1^2 =
\left[\begin{array}{cc}
2 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
4 & 3 \\
0 & 1 \\
\end{array}\right]
$$

$$ A_1^3 = (A_1^2)A_1 =
\left[\begin{array}{cc}
4 & 3 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
8 & 7 \\
0 & 1 \\
\end{array}\right]
$$

$$ A_1^n =
\left[\begin{array}{cc}
2^n & 2^n - 1 \\
0 & 1 \\
\end{array}\right]
$$

$A_2$:

$$ A_2 =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
$$

$$ A_2^2 =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 2 \\
2 & 2 \\
\end{array}\right]
$$

$$ A_2^3 = (A_2^2)A_2 =
\left[\begin{array}{cc}
2 & 2 \\
2 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
4 & 4 \\
4 & 4 \\
\end{array}\right]
$$

$$ A_2^n =
\left[\begin{array}{cc}
2^{n - 1} & 2^{n - 1} \\
2^{n - 1} & 2^{n - 1} \\
\end{array}\right]
$$

$A_3$:

$$ A_3 =
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right]
$$

$$ A_3^2 =
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
a^2 & ab \\
0 & 0 \\
\end{array}\right]
$$

$$ A_3^3 = (A_3^2)A_3 =
\left[\begin{array}{cc}
a^2 & ab \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
a^3 & a^2b \\
0 & 0 \\
\end{array}\right]
$$

$$ A^n =
\left[\begin{array}{cc}
a^n & a^{n - 1}b \\
0 & 0 \\
\end{array}\right]
$$

**Problems 25-31 use column-row multiplication and block multiplication.**

25. Multiply $A$ times $I$ using columns of $A$ (3 by 3) times rows of $I$.

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33} \\
\end{array}\right]
$$

$$ I =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Column-row multiplication of $AI$:

$$ \begin{bmatrix}{}a_{11}\\a_{21}\\a_{31}\end{bmatrix} \left[\begin{array}{ccc}1 & 0 & 0\end{array}\right] + \begin{bmatrix}{}a_{12}\\a_{22}\\a_{32}\end{bmatrix} \left[\begin{array}{ccc}0 & 1 & 0\end{array}\right] + \begin{bmatrix}{}a_{13}\\a_{23}\\a_{33}\end{bmatrix} \left[\begin{array}{ccc}0 & 0 & 1\end{array}\right] $$

$$
\left[\begin{array}{ccc}
a_{11} & 0 & 0 \\
a_{21} & 0 & 0 \\
a_{31} & 0 & 0 \\
\end{array}\right] +
\left[\begin{array}{ccc}
0 & a_{12} & 0 \\
0 & a_{22} & 0 \\
0 & a_{32} & 0 \\
\end{array}\right] +
\left[\begin{array}{ccc}
0 & 0 & a_{13} \\
0 & 0 & a_{23} \\
0 & 0 & a_{33} \\
\end{array}\right] =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33} \\
\end{array}\right] = A
$$

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
\begin{bmatrix}{}1\\2\\2\end{bmatrix}
\left[\begin{array}{ccc}
3 & 3 & 0 \\
\end{array}\right] + \text{(?)} = \text{(?)}
$$

_Solution:_

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
\begin{bmatrix}{}1\\2\\2\end{bmatrix}
\left[\begin{array}{ccc}
3 & 3 & 0 \\
\end{array}\right] +
\begin{bmatrix}{}0\\4\\1\end{bmatrix}
\left[\begin{array}{ccc}
1 & 2 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc}
3 & 3 & 0 \\
6 & 6 & 0 \\
6 & 6 & 0 \\
\end{array}\right] +
\left[\begin{array}{ccc}
0 & 0 & 0 \\
4 & 8 & 4 \\
1 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
3 & 3 & 0 \\
10 & 14 & 4 \\
7 & 8 & 1 \\
\end{array}\right] = AB
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

_Solution:_

_Proof (using row times columns):_

Suppose $A$ and $B$ are upper triangular matrices where:

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
0 & a_{22} & a_{23} \\
0 & 0 & a_{33} \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
b_{11} & b_{12} & b_{13} \\
0 & b_{22} & b_{23} \\
0 & 0 & b_{33} \\
\end{array}\right]
$$

It is to be shown that $AB$ is always an upper triangular matrix.

Consider the product as it stands:

$$ AB =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
0 & a_{22} & a_{23} \\
0 & 0 & a_{33} \\
\end{array}\right]
\left[\begin{array}{ccc}
b_{11} & b_{12} & b_{13} \\
0 & b_{22} & b_{23} \\
0 & 0 & b_{33} \\
\end{array}\right] =
\left[\begin{array}{ccc}
a_{11}b_{11} & a_{11}b_{12} + a_{12}b_{22} & a_{11}b_{13} + a_{12}b_{23} + a_{13}b_{33} \\
0 & a_{22}b_{22} & a_{22}b_{23} + a_{23}b_{33} \\
0 & 0 & a_{33}b_{33} \\
\end{array}\right]
$$

By the definition of an upper triangular matrix, where $0$'s span in the entries
below the diagonal, $AB$ is an upper triangular matrix. This is what was to be
shown.

Q.E.D.

28. Draw the cuts in $A$ (2 by 3) and $B$ (3 by 4) and $AB$ to show how each of
    the four multiplication rules is really a block multiplication:

_Note:_

Basis matrices:

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cccc}
b_{11} & b_{12} & b_{13} & b_{14} \\
b_{21} & b_{22} & b_{23} & b_{24} \\
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

(1) Matrix $A$ times columns of $B$. **Columns of $AB$**

$$ A =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
$$

$$ B_C =
\left[\begin{array}{c|c|c|c}
b_{11} & b_{12} & b_{13} & b_{14} \\
b_{21} & b_{22} & b_{23} & b_{24} \\
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

To denote this, consider $B_{j}$ where $j$ represents the column of $B$:

$$ AB =
\left[\begin{array}{c|c|c|c}
AB_1 & AB_2 & AB_3 & AB_4 \\
\end{array}\right]
$$

Or, more specifically:

$$ AB =
A\left[\begin{array}{c|c|c|c}
b_{11} & b_{12} & b_{13} & b_{14} \\
b_{21} & b_{22} & b_{23} & b_{24} \\
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

(2) Rows of $A$ times the matrix $B$. **Rows of $AB$**

Denote the rows of $A$ as $A_R$, then:

$$ A_R =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
\hline
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
$$

$$ A_RB =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
\hline
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
\left[\begin{array}{cccc}
b_{11} & b_{12} & b_{13} & b_{14} \\
b_{21} & b_{22} & b_{23} & b_{24} \\
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

(3) Rows of $A$ times columns of $B$. **Inner products** (numbers in $AB$)

$$ A_RB_C =
\left[\begin{array}{ccc}
a_{11} & a_{12} & a_{13} \\
\hline
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
\left[\begin{array}{c|c|c|c}
b_{11} & b_{12} & b_{13} & b_{14} \\
b_{21} & b_{22} & b_{23} & b_{24} \\
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

This is the standard dot product method.

(4) Columns of $A$ times rows of $B$. **Outer products** (matrices add to $AB$)

$$ A_CB_R =
\left[\begin{array}{c|c|c}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
\end{array}\right]
\left[\begin{array}{cccc}
b_{11} & b_{12} & b_{13} & b_{14} \\
\hline
b_{21} & b_{22} & b_{23} & b_{24} \\
\hline
b_{31} & b_{32} & b_{33} & b_{34} \\
\end{array}\right]
$$

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

_Solution:_

_Which matrices $E_{21}$ produce zeros in the $(2, 1)$ position of $E_{21}A$?:_

$$ A =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
-2 & 0 & 1 \\
8 & 5 & 3 \\
\end{array}\right]
$$

To produce zeros in the $(2,1)$ entry of $A$ (row $2$, column $1$ of $A$),
$E_{21}$ should add 1 times row 1 to row 2.

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

_Which matrix $E_{31}$ produce zeros in the $(3, 1)$ position of $E_{31}A$?:_

To produce zeros in the $(3, 1)$ position of $A$, $E_{31}$ should subtract 4
times row 1 from row 3:

$$ E_{31} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
$$

_Find the single matrix $E = E_{31}E_{21}$ that produces both zeros at once:_

$$ E = E_{31}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
$$

_Multiply $EA$:_

$$ EA =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 0 \\
-2 & 0 & 1 \\
8 & 5 & 3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 1 & 1 \\
0 & 1 & 3 \\
\end{array}\right]
$$

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

_Solution:_

$$ c =
\left[\begin{array}{r}
-2 \\
8 \\
\end{array}\right]
$$

$$ D =
\left[\begin{array}{cc}
0 & 1 \\
5 & 3 \\
\end{array}\right]
$$

$$ D - \dfrac{cb}{a} =
\left[\begin{array}{cc}
1 & 1 \\
1 & 3 \\
\end{array}\right]
$$

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

Omitted.

32. _(Very important)_ Suppose you solve $Ax = b$ for three special right sides
    $b$:

$$ Ax_1 = \begin{bmatrix}{}1\\0\\0\end{bmatrix} \quad \text{ and } \quad Ax_2 = \begin{bmatrix}{}0\\1\\0\end{bmatrix} \quad \text{ and } \quad Ax_3 = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

If the three solutions $x_1, x_2, x_3$ are the columns of a matrix $X$, what is
$A$ times $X$?

_Solution:_

So, let's break this down a bit, let's first define $X$:

$$ X =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Notice that this is the identity matrix, so, $AX = I$.

This means that $X = A^{-1}$, since any matrix multiplied by it's own inverse is
$I$.

33. If the three solutions in Question 32 are $x_1 = (1, 1, 1)$ and
    $x_2 = (0, 1, 1)$ and $x_3 = (0, 0, 1)$, solve $Ax = b$ when
    $b = (3, 5, 8)$. Challenge problem: What is $A$?

_Solution:_

Evaluating the question yields:

$$ A\begin{bmatrix}{}1\\1\\1\end{bmatrix} =
\begin{bmatrix}{}1\\0\\0\end{bmatrix}
$$

$$ A\begin{bmatrix}{}0\\1\\1\end{bmatrix} =
\begin{bmatrix}{}0\\1\\0\end{bmatrix}
$$

$$ A\begin{bmatrix}{}0\\0\\1\end{bmatrix} =
\begin{bmatrix}{}0\\0\\1\end{bmatrix}
$$

This means that $X$ from problem 32 is:

$$ X =
\left[\begin{array}{ccc}
1 & 0 & 0\\
1 & 1 & 0\\
1 & 1 & 1 \\
\end{array}\right]
$$

Now, we're trying to find little $x$.

We know that:

$$ Ax = b $$

$$ Ax = \begin{bmatrix}{}3\\5\\8\end{bmatrix} $$

In problem 32, we established that $X = A^{-1}$. Let's go step by step:

$$ Ax = b $$

$$ A^{-1}(Ax) = A^{-1}b $$

$$ Ix = A^{-1}b $$

Since $Ix = x$:

$$ x = A^{-1}b $$

And since $X = A^{-1}$:

$$ x = Xb $$

So now:

$$ x =
\left[\begin{array}{ccc}
1 & 0 & 0\\
1 & 1 & 0\\
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}3\\5\\8\end{bmatrix} =
\begin{bmatrix}{}3\\8\\16\end{bmatrix}
$$

Challenge problem omitted.

34. Find all matrices
    $A = \left[\begin{array}{cc}a & b \\c & d \\\end{array}\right]$ that satisfy
    $A\left[\begin{array}{cc}1 & 1\\1 & 1\\\end{array}\right] = \left[\begin{array}{cc}1 & 1\\1 & 1\\\end{array}\right]A$.

_Solution:_

If we consider $A$ as given:

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

Let $O$ represent the $1$'s matrix given:

$$ O =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
$$

Then $AO$ is:

$$ AO =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
a + b & a + b \\
c + d & c + d \\
\end{array}\right]
$$

Then $OA$ is:

$$ OA =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a + c & b + d \\
a + c & b + d \\
\end{array}\right]
$$

So, in order for $AO = OA$, the following must be true:

$$
a + b = a + c \\
c + d = a + c \\
a + b = b + d \\
c + d = b + d \\
$$

Simplifying:

$$
b = c \\
d = a \\
a = d \\
c = b \\
$$

So, as long as $a = d$ and $b = c$, $AO = OA$, thus:

$$ A =
\left[\begin{array}{cc}
a & b \\
b & a \\
\end{array}\right]
$$

35. Suppose a "circle graph" has 4 nodes connected (in both directions) by edges
    around a circle. What is its adjacency matrix $S$ from Worked Example 2.4 A?
    What is $S^2$? Find all the 2-step paths predicted by $S^2$.

Omitted.

---

Page 103

## Problem Set 2.5

1. Find the inverses (directly or from the 2 by 2 formula) of $A, B, C$:

$$ A =
\left[\begin{array}{cc}
0 & 3 \\
4 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
2 & 0 \\
4 & 2 \\
\end{array}\right]
$$

and

$$ C =
\left[\begin{array}{cc}
3 & 4 \\
5 & 7 \\
\end{array}\right]
$$

_Solution:_

$A^{-1}$:

$$ A =
\left[\begin{array}{cc}
0 & 3 \\
4 & 0 \\
\end{array}\right]
$$

$$ \det A = (0)(0) - (3)(4) = -12 $$

$$ A^{-1} = \frac{1}{-12}
\left[\begin{array}{cc}
0 & -3 \\
-4 & 0 \\
\end{array}\right]
$$

$$ A^{-1} =
\left[\begin{array}{cc}
0 & \frac{1}{4} \\
\frac{1}{3} & 0 \\
\end{array}\right]
$$

$B^{-1}$:

$$ B =
\left[\begin{array}{cc}
2 & 0 \\
4 & 2 \\
\end{array}\right]
$$

$$ \det B = (2)(2) - (0)(4) = 4 $$

$$ B^{-1} = \frac{1}{4}
\left[\begin{array}{cc}
2 & -0 \\
-4 & 2 \\
\end{array}\right]
$$

$$ B^{-1} =
\left[\begin{array}{cc}
\frac{1}{2} & 0 \\
-1 & \frac{1}{2} \\
\end{array}\right]
$$

$C^{-1}$:

$$ C =
\left[\begin{array}{cc}
3 & 4 \\
5 & 7 \\
\end{array}\right]
$$

$$ \det C = (3)(7) - (4)(5) = 1 $$

$$ C^{-1} = \frac{1}{1}
\left[\begin{array}{cc}
7 & -4 \\
-5 & 3 \\
\end{array}\right]
$$

$$ C^{-1} =
\left[\begin{array}{cc}
7 & -4 \\
-5 & 3 \\
\end{array}\right]
$$

2. For these "permutation matrices" find $P^{-1}$ by trial and error (with $1$'s
   and $0$'s):

$$ P =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

and

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

_Solution:_

_First $P$:_

$$ P =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

Row exchanges yield $I$:

$$ P =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

So $P^{-1} = P$.

_Second $P$:_

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ \left[\begin{array}{cc}P & I \\\end{array}\right] =
\left[\begin{array}{ccc|ccc}
0 & 1 & 0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 & 1 & 0 \\
1 & 0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Swap row 3 and row 1:

$$ \left[\begin{array}{cc}P & I \\\end{array}\right] =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 0 & 0 & 1 \\
0 & 1 & 0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 & 1 & 0 \\
\end{array}\right]
$$

And now we have $\left[\begin{array}{cc}I & P^{-1} \\\end{array}\right]$:

$$ P^{-1} =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

3. Solve for the first column $(x, y)$ and second column $(t, z)$ of $A^{-1}$:

$$
\left[\begin{array}{cc}
10 & 20 \\
20 & 50 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}1\\0\end{bmatrix}
$$

and

$$
\left[\begin{array}{cc}
10 & 20 \\
20 & 50 \\
\end{array}\right]
\begin{bmatrix}{}t\\z\end{bmatrix} =
\begin{bmatrix}{}0\\1\end{bmatrix}
$$

_Solution:_

_Solving for $(x, y)$:_

$$
10x + 20y = 1 \\
20x + 50y = 0 \\
$$

$$
\left[\begin{array}{rr}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{rr|r}
10 & 20 & 1 \\
20 & 50 & 0 \\
\end{array}\right] =
\left[\begin{array}{rr|r}
10 & 20 & 1 \\
0 & 10 & -2 \\
\end{array}\right]
$$

Back substitute:

$$ 10y = -2 \Rightarrow y = -\frac{1}{5} $$

$$ 10x + 20\left(-\frac{1}{5}\right) = 1 \Rightarrow 10x - 4 = 1 \Rightarrow 10x = 5 \Rightarrow x = \frac{1}{2} $$

$$
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}\frac{1}{2}\\-\frac{1}{5}\end{bmatrix}
$$

_Solving for $(t, z)$:_

$$
10t + 20z = 0 \\
20t + 50z = 1 \\
$$

$$
\left[\begin{array}{rr}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc|c}
10 & 20 & 0 \\
20 & 50 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc|c}
10 & 20 & 0 \\
0 & 10 & 1 \\
\end{array}\right]
$$

Back substitution:

$$ 10z = 1 \Rightarrow z = \frac{1}{10} $$

$$ 10t + 20\left(\frac{1}{10}\right) = 0 \Rightarrow 10t + 2 = 0 \Rightarrow 10t = -2 \Rightarrow t = -\frac{1}{5} $$

$$
\begin{bmatrix}{}t\\z\end{bmatrix} =
\begin{bmatrix}{}-\frac{1}{5}\\\frac{1}{10}\end{bmatrix}
$$

Thus $A^{-1}$ is:

$$
\begin{bmatrix}{}t\\z\end{bmatrix} =
\begin{bmatrix}{}-\frac{1}{5}\\\frac{1}{10}\end{bmatrix}
$$

$$ A^{-1} =
\left[\begin{array}{cc}
\frac{1}{2} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{1}{10} \\
\end{array}\right]
$$

$$ A^{-1} = \frac{1}{10}
\left[\begin{array}{cc}
5 & -2 \\
-2 & 1 \\
\end{array}\right]
$$

4. Show that $\left[\begin{array}{cc}1 & 2 \\3 & 6 \\\end{array}\right]$ is not
   invertible by trying to solve $AA^{-1} = I$ for column 1 of $A^{-1}$:

$$
\left[\begin{array}{cc}
1 & 2 \\
3 & 6 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}1\\0\end{bmatrix}
$$

(_For a different_ $A$, could column 1 of $A^{-1}$ be possible to find but not
column 2?)

_Solution:_

$$ A =
\left[\begin{array}{cc|c}
1 & 2 & 1 \\
3 & 6 & 0 \\
\end{array}\right]
$$

$$ E_{12}A =
\left[\begin{array}{cc}
1 & 0 \\
-3 & 1 \\
\end{array}\right]
\left[\begin{array}{cc|c}
1 & 2 & 1 \\
3 & 6 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 2 & 1 \\
0 & 0 & -3 \\
\end{array}\right]
$$

By elimination we are left with $0y = -3$, for which there is _no solution._
Thus $A$ is not invertible.

It is not possible to find a different $A$ where column 1 of $A^{-1}$ is
possible to find but not column 2 (this is because $y$ is a scalar of $x$ in the
second row).

5. Find an upper triangular $U$ (not diagonal) with $U^2 = I$ which gives
   $U = U^{-1}$.

$$ U =
\left[\begin{array}{cc}
1 & 1 \\
0 & -1 \\
\end{array}\right]
$$

Then:

$$ U^2 =
\left[\begin{array}{cc}
1 & 1 \\
0 & -1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & -1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

Since $UU = I$, it follows by the property of inverse matrices that
$U = U^{-1}$.

6.

a. If $A$ is invertible and $AB = AC$, prove quickly that $B = C$.

**Proof:**

Suppose $A$ is any matrix where $A$ is invertible and $AB = AC$ .

It must be shown that $B = C$.

Since $A$ is invertible (by the supposition), this means there exists some
inverse matrix, $A^{-1}$ such that $A^{-1}A = I$.

Multiplying both sides of $AB = AC$ by $A^{-1}$ (in effect applying $A^{-1}$ _on
the left_) yields:

$$ A^{-1}(AB) = A^{-1}(AC) $$

By the law of associativity, this can be rewritten as:

$$ (A^{-1}A)B = (A^{-1}A)C $$

By the definition of invertible matrices, $A^{-1}A = I$, and thus it follows by
substitution that:

$$ (I)B = (I)C $$

And by the definition of the identity matrix, any matrix multiplied by the
identity matrix is equal to itself, and thus:

$$ (I)B = B = C = (I)C $$

By the definition of equality, this means that:

$$ B = C $$

Which is what was to be shown.

Q.E.D.

b. If $A = \left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$, find two
different matrices such that $AB = AC$.

Since $\det A = (1)(1) - (1)(1) = 0 $, $A^{-1}$ does not exist. Thus any
matrices $B$ and $C$ where the form of $B - C$ takes the form of
$B - C = \left[\begin{array}{cc}
x & y \\
-x & - y\\
\end{array}\right]$ will satisfy the property that $AB = AC$.

This insight is garnered by the fact that we're trying to get to $AB = AC$:

$$ AB = AC \Rightarrow AB - AC = \mathbf{0} \Rightarrow A(B - C) = \mathbf{0} $$

Consider:

$$ B - C =
\left[\begin{array}{cc}
3 & 4 \\
2 & 3 \\
\end{array}\right] -
\left[\begin{array}{cc}
2 & 3 \\
3 & 4 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
-1 & -1 \\
\end{array}\right]
$$

Then:

$$ AB =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
3 & 4 \\
2 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
5 & 7 \\
5 & 7 \\
\end{array}\right]
$$

$$ AC =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 3 \\
3 & 4 \\
\end{array}\right] =
\left[\begin{array}{cc}
5 & 7 \\
5 & 7 \\
\end{array}\right]
$$

Thus $AB = AC$.

7. (Important) If $A$ has row 1 + row 2 = row 3, show that $A$ is not
   invertible:

a. Explain why $Ax = (0, 0, 1)$ cannot have a solution. Add eqn 1 + eqn 2.

b. Which right sides $(b_1, b_2, b_3)$ might allow a solution to $Ax = b$?

c. In elimination, what happens to equation 3?

_Solution:_

Show that $A$ is not invertible:

Consider the following definition for $A$ row 1 + row 2 = row 3:

$$ A =
\left[\begin{array}{ccc}
3 & 2 & 1 \\
1 & 2 & 3 \\
4 & 4 & 4 \\
\end{array}\right]
$$

a.

Since row 1 + row 2 = row 3, in elimination eventually, row 3 is reduced to 0
since it is the sum of rows 1 and 2, and thus row 3 becomes an expression of
$0z \neq 0$, which has no solution.

b. If $b_1 + b_2 = b_3$, then there might be a solution allowed for $Ax = b$.

c.

Consider the following:

$$ Ax =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 0 \\
3 & 2 & 1 & 0 \\
4 & 4 & 4 & 1 \\
\end{array}\right]
$$

Then, we begin elimination on $Ax$ with $E_{12}$:

$$ E_{12}Ax =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 0 \\
3 & 2 & 1 & 0 \\
4 & 4 & 4 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -4 & -8 & 0 \\
4 & 4 & 4 & 1 \\
\end{array}\right]
$$

Then, continue elimination with $E_{13}$:

$$ E_{13}E_{12}Ax =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -4 & -8 & 0 \\
4 & 4 & 4 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -4 & -8 & 0 \\
0 & -4 & -8 & 1 \\
\end{array}\right]
$$

Further elimination causes equation 3 to to be zeroed out to the form of
$0z = 1$, which has _no solution._

8. If $A$ has column 1 + column 2 = column 3, show that $A$ is not invertible:

a. Find a nonzero solution $x$ to $Ax = \mathbf{0}$. The matrix is 3 by 3.

b. Elimination keeps column 1 + column 2 = column 3. Explain why there is no
third pivot.

_Solution:_

Show that $A$ is not invertible:

Consider the following definition for $A$ where column 1 + column 2 = column 3:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 3 & 5 \\
3 & 4 & 7 \\
\end{array}\right]
$$

a.

Consider:

$$ Ax =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 0 \\
2 & 3 & 5 & 0 \\
3 & 4 & 7 & 0 \\
\end{array}\right]
$$

Let's find $x$.

$$ E_{21}Ax =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 0 \\
2 & 3 & 5 & 0 \\
3 & 4 & 7 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -1 & -1 & 0 \\
3 & 4 & 7 & 0 \\
\end{array}\right]
$$

$$ E_{31}E_{21}Ax =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -1 & -1 & 0 \\
3 & 4 & 7 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -1 & -1 & 0 \\
0 & -2 & -2 & 0 \\
\end{array}\right]
$$

$$ E_{23}E_{31}E_{21}Ax =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -1 & -1 & 0 \\
0 & -2 & -2 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & 3 & 0 \\
0 & -1 & -1 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

Thus $z$ can be any number, let $z = 1$ and back substitute:

$$ -y + -1(1) = 0 \Rightarrow -y - 1 = 0 \Rightarrow -y = 1 \Rightarrow y = -1 $$

$$ x + 2(-1) + 3(1) = 0 \Rightarrow x - 2 + 3 = 0 \Rightarrow x + 1 = 0 \Rightarrow x = -1 $$

$$ \boxed{x = \begin{bmatrix}{}-1\\-1\\1\end{bmatrix}} $$

b.

The reason there is no third pivot is because if column 1 + column 2 = column 3,
this means that during elimination, the third row will always end up being a
scalar multiple of row 2 or row 1, resulting in a final elimination result of
$0z = 0$ (_i.e._ infinite solutions for $z$).

9. Suppose $A$ is invertible and you exchange its first two rows to reach $B$.
   Is the new matrix $B$ invertible? How would you find $B^{-1}$ from $A^{-1}$?

**Proof:**

Suppose $A$ is any matrix such that it is invertible. Furthermore suppose the
first two rows of $A$ are exchanged to reach a new matrix $B$.

It is to be shown that $B$ is invertible, and it is to be demonstrated how one
might find $B^{-1}$ from $A^{-1}$.

Consider this general form for $A$:

$$ A =
\left[\begin{array}{cccc}
a_{11} & a_{12} & \dots & a_{1j} \\
a_{21} & a_{22} & \dots & a_{2j} \\
\vdots & \vdots & \vdots & \vdots \\
a_{i1} & a_{i2} & \dots & a_{ij} \\
\end{array}\right]
$$

By the supposition, $A$ is invertible, thus there exists some inverse matrix
$A^{-1}$, where the following property of inverses is true:

$$ AA^{-1} =
\left[\begin{array}{cccc}
a_{11} & a_{12} & \dots & a_{1j} \\
a_{21} & a_{22} & \dots & a_{2j} \\
\vdots & \vdots & \vdots & \vdots \\
a_{i1} & a_{i2} & \dots & a_{ij} \\
\end{array}\right]
\left[\begin{array}{cccc}
(a^{-1})_{11} & (a^{-1})_{12} & \dots & (a^{-1})_{1j} \\
(a^{-1})_{21} & (a^{-1})_{22} & \dots & (a^{-1})_{2j} \\
\vdots & \vdots & \vdots & \vdots \\
(a^{-1})_{i1} & (a^{-1})_{i2} & \dots & (a^{-1})_{ij} \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & \dots & 0 \\
0 & 1 & \dots & 0 \\
\vdots &\vdots & \ddots & 0 \\
0 & 0 & \dots & 1 \\
\end{array}\right] = I
$$

Now, since $B$ is simply $A$ with it's first two rows exchanged, this means that
$B$ is:

$$ B =
\left[\begin{array}{cccc}
a_{21} & a_{22} & \dots & a_{2j} \\
a_{11} & a_{12} & \dots & a_{1j} \\
\vdots & \vdots & \vdots & \vdots \\
a_{i1} & a_{i2} & \dots & a_{ij} \\
\end{array}\right]
$$

To get $B$, there is a permutation matrix $P_{12}$ that exchanges rows 1 and 2:

$$ P_{12} =
\left[\begin{array}{cccc}
0 & 1 & \dots & 0 \\
1 & 0 & \dots & 0 \\
\vdots & \vdots & \vdots & \vdots \\
0 & 0 & \dots & 1 \\
\end{array}\right]
$$

When $P_{12}$ is applied to $A$, the result is $B$.

$$ P_{12}A = B $$

Since $B = P_{12}A$, by substitution, $B^{-1}$ can be expressed as:

$$ B^{-1} = (P_{12}A)^{-1} $$

And by the "distributive" property of inverses:

$$ B^{-1} = A^{-1}(P_{12})^{-1} $$

By problem 2, it is known that any permutation matrix that exchanges 2 rows is
its own inverse, and thus the product of any permutation matrix (that has this
property) with itself will result in the identity matrix.

It follows by substitution that:

$$ B^{-1} = A^{-1}P_{12} $$

By the supposition and by the definition for $P_{12}$, $B^{-1}$ is well defined,
and thus it has been shown that $B^{-1}$ exists, and therefore $B$ is
invertible.

The above formula also demonstrates how one might find $B^{-1}$.

Q.E.D.

10. Find the inverses (in any legal way) of

$$ A =
\left[\begin{array}{cccc}
0 & 0 & 0 & 2 \\
0 & 0 & 3 & 0 \\
0 & 4 & 0 & 0 \\
5 & 0 & 0 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cccc}
3 & 2 & 0 & 0 \\
4 & 3 & 0 & 0 \\
0 & 0 & 6 & 5 \\
0 & 0 & 7 & 6 \\
\end{array}\right]
$$

_Solution:_

_Finding $A^{-1}$:_

$$ A =
\left[\begin{array}{cccc}
0 & 0 & 0 & 2 \\
0 & 0 & 3 & 0 \\
0 & 4 & 0 & 0 \\
5 & 0 & 0 & 0 \\
\end{array}\right]
$$

Since all other entries on each row are $0$, $A^{-1}$ can be found by simply
finding the inverse of each number and leaving them in their appropriate entry
place.

$$ A^{-1} =
\left[\begin{array}{cccc}
0 & 0 & 0 & \frac{1}{2} \\
0 & 0 & \frac{1}{3} & 0 \\
0 & \frac{1}{4} & 0 & 0 \\
\frac{1}{5} & 0 & 0 & 0 \\
\end{array}\right]
$$

_Finding $B^{-1}$:_

$$ B =
\left[\begin{array}{cccc}
3 & 2 & 0 & 0 \\
4 & 3 & 0 & 0 \\
0 & 0 & 6 & 5 \\
0 & 0 & 7 & 6 \\
\end{array}\right]
$$

Here, solve for the two 2 x 2 blocks through the determinant formula:

$$ B_{1}
\left[\begin{array}{cc}
3 & 2 \\
4 & 3 \\
\end{array}\right]
$$

$$ \det B_{1} = (3)(3) - (2)(4) = 9 - 8 = 1 $$

$$ (B_{1})^{-1} =
1
\left[\begin{array}{cc}
3 & -2 \\
-4 & 3 \\
\end{array}\right]
$$

$$ (B_{1})^{-1} =
\left[\begin{array}{cc}
3 & -2 \\
-4 & 3 \\
\end{array}\right]
$$

Now the other block:

$$ B_{2}  =
\left[\begin{array}{cc}
6 & 5 \\
7 & 6 \\
\end{array}\right]
$$

$$ \det B_{2} = (6)(6) - (5)(7) = 36 - 35 = 1 $$

$$ (B_{2})^{-1} =
1
\left[\begin{array}{cc}
6 & -5 \\
-7 & 6 \\
\end{array}\right]
$$

$$ (B_{2})^{-1} =
\left[\begin{array}{cc}
6 & -5 \\
-7 & 6 \\
\end{array}\right]
$$

So:

$$ B^{-1} =
\left[\begin{array}{rrrr}
3 & -2 & 0 & 0 \\
-4 & 3 & 0 & 0 \\
0 & 0 & 6 & -5 \\
0 & 0 & -7 & 6 \\
\end{array}\right]
$$

11.

a. Find invertible matrices $A$ and $B$ such that $A + B$ is not invertible.

If $B = -A$, then $A + B = A + (-A) = \mathbf{0}$, which is not invertible.

So:

$$ A =
\left[\begin{array}{cc}
2 & 1 \\
4 & 3 \\
\end{array}\right]
$$

Then:

$$ \det A = (2)(3) - (1)(4) = 2 $$

$$ A^{-1} =
\frac{1}{2}\left[\begin{array}{cc}
3 & -1 \\
-4 & 2\\
\end{array}\right]
$$

$$ A^{-1} =
\left[\begin{array}{cc}
\frac{3}{2} & -\frac{1}{2} \\
-2 & 1 \\
\end{array}\right]
$$

Then, since $B = -A$:

$$ B =
-1
\left[\begin{array}{cc}
2 & 1 \\
4 & 3 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
-2 & -1 \\
-4 & -3 \\
\end{array}\right]
$$

$$ \det B = (-2)(-3) - (-1)(-4) = 2 $$

$$ B^{-1} =
\frac{1}{2}
\left[\begin{array}{cc}
-3 & 1 \\
4 & -2 \\
\end{array}\right]
$$

$$ B^{-1} =
\left[\begin{array}{cc}
-\frac{3}{2} & \frac{1}{2} \\
2 & -1 \\
\end{array}\right]
$$

So both $A$ and $B$ are invertible, but:

$$ A + B =
\left[\begin{array}{cc}
2 & 1 \\
4 & 3 \\
\end{array}\right] +
\left[\begin{array}{cc}
-2 & -1 \\
-4 & -3 \\
\end{array}\right] = \mathbf{0}
$$

And thus $A + B$ is not invertible.

b. Find singular matrices $A$ and $B$ such that $A + B$ is invertible.

For $A + B$ to be invertible, it must be that $(A + B)(A + B)^{-1} = I$ or
$(A + B)^{-1}(A + B) = I$.

To keep it simple, let:

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

and let:

$$ B =
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right]
$$

Both $A$ and $B$ are singular, and thus are not invertible, but:

$$ A + B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

And since $A + B = I$, $A + B$ is invertible since $(A + B)^{-1} = I$ also.

12. If the product $C = AB$ is invertible ($A$ and $B$ are square), then $A$
    itself is invertible. Find a formula for $A^{-1}$ that involves $C^{-1}$ and
    $B$.

_Solution:_

Suppose $C = AB$ is invertible and that $A$ is invertible.

By equality, it is trivial that:

$$ C^{-1} = C^{-1} $$

Then, apply $C$ to both sides:

$$ CC^{-1} = CC^{-1} $$

Then, substitute $C = AB$ to one side:

$$ (AB)C^{-1} = CC^{-1} $$

By the identity property for inverses:

$$(AB)C^{-1} = I $$

By the associative property of matrix multiplication:

$$ ABC^{-1} = I $$

By the supposition, $A^{-1}$ exists, and $ABC^{-1} = I$ implies that
$A^{-1} = BC^{-1}$ since $AA^{-1} = I$.

Thus a formula for $A^{-1}$ that involves $C^{-1}$ and $B$ is:

$$ \boxed{A^{-1} = BC^{-1}} $$

13. If the product $M =ABC$ of three square matrices is invertible, then $B$ is
    invertible. (So are $A$ and $C$.) Find a formula for $B^{-1}$ that involves
    $M^{-1}$ and $A$ and $C$.

_Solution:_

By the supposition $M = ABC$ is invertible, and $B$ is invertible.

$$ M = ABC $$

$$ A^{-1}M = A^{-1}(ABC) $$

$$ A^{-1}M = (A^{-1}A)BC $$

$$ A^{-1}M = (I)BC $$

$$ A^{-1}M = BC $$

$$ A^{-1}MC^{-1} = BCC^{-1} $$

$$ A^{-1}MC^{-1} = B(CC^{-1}) $$

$$ A^{-1}MC^{-1} = B(I) $$

$$ A^{-1}MC^{-1} = B $$

$$ (A^{-1}MC^{-1})^{-1} = B^{-1} $$

$$ CM^{-1}A = B^{-1} $$

$$ B^{-1} = CM^{-1}A $$

14. If you add row 1 of $A$ to row 2 to get $B$, how do you find $B^{-1}$ from
    $A^{-1}$?

Notice the order.

The inverse of
$B =\left[\begin{array}{cc}1 & 0 \\1 & 1 \\\end{array}\right]\left[\begin{array}{c}A \\\end{array}\right]$
is ____.

_Solution:_

$$ B^{-1} =
\left(
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{c}
A \\
\end{array}\right]
\right)^{-1}
$$

By the "distributive" property of inverse:

$$ B^{-1} =
\left[\begin{array}{c}
A \\
\end{array}\right]^{-1}
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]^{-1}
$$

Now, the augmented matrix with just $A^{-1}$ is simply $A^{-1}$. The inverse of
the elimination matrix follows from the logic of the statement. Since $B$ is
derived from adding row 1 of $A$ to row 2 of $A$, it follows that $A$ is derived
from subtracting row 1 of $B$ from row 2 of $B$, thus $B^{-1}$ is:

$$ B^{-1} =
A^{-1}
\left[\begin{array}{cc}
1 & 0 \\
-1 & 1 \\
\end{array}\right]
$$

15. Prove that a matrix with a column of zeros cannot have an inverse.

**Proof (by contradiction):**

Suppose $A$ is any matrix with a column of zeros, and suppose that $A$ is
invertible.

Let $k$ be the column of $A$ with all zeros.

Now suppose $x$ is a vector with a $1$ in the position $k$. So,
$x_k = 1 \neq 0$. Now, because there are all $0$'s in $k$, it follows that
$Ax = 0$.

Now, apply $A^{-1}$ to both sides of $Ax = 0$:

$$ A^{-1}Ax = A^{-1}0 $$

$$ Ix = 0 $$

$$ x = 0 $$

So $x_k = 1 \neq 0$ and $x_k = 0$. This is a contradiction.

Since a contradiction has been derived, the supposition must be false and
therefore a matrix with a column of zeros cannot have an inverse.

Q.E.D.

16. Multiply $\left[\begin{array}{cc}a & b \\c & d \\\end{array}\right]$ times
    $\left[\begin{array}{cc}d & -b \\-c & a \\\end{array}\right]$. What is the
    inverse of each matrix if $ad \neq bc$?

_Solution:_

Denote the given matrices $A$ and $B$, then:

$$ AB =
\left[\begin{array}{rr}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{rr}
d & -b \\
-c & a \\
\end{array}\right] =
\left[\begin{array}{cc}
ad - bc & 0 \\
0 & ad - bc \\
\end{array}\right]
$$

Now, if we factor out $ad - bc$:

$$ AB =
(ad - bc)
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

Which gives us $AB = (ad - bc)I$.

It follows that since $AA^{-1} = I$ that:

$$ \frac{1}{ad - bc }AB = I $$

Then:

$$ A\left(\frac{1}{ad - bc }B\right) = I $$

$$ A^{-1} = \frac{1}{ad - bc}B $$

Similarly:

$$ B\left(\frac{1}{ad - bc }A\right) = I $$

$$ B^{-1} = \frac{1}{ad - bc }A $$

17.

a. What 3 by 3 matrix $E$ has the same effect as these three steps? Subtract row
1 from row 2, subtract row 1 from row 3, then subtract row 2 from row 3.

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{23}E_{31}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
-1 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
$$

$$ E =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
$$

b. What single matrix $L$ has the same effect as these three reverse steps? Add
row 2 to row 3, add row 1 to row 3, then add row 1 to row 2.

$$ L = E^{-1} =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
-1 & 1 & 0 & 0 & 1 & 0 \\
0 & -1 & 1  & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ L =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & 1 & 1 & 0 \\
0 & -1 & 1  & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ L =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & 1 & 1 & 0 \\
0 & 0 & 1  & 0 & 1 & 1 \\
\end{array}\right]
$$

$$ L =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
$$

18. If $B$ is the inverse of $A^2$, show that $AB$ is the inverse of $A$.

**Proof:**

Suppose $A$ and $B$ are any matrices such that $B$ is the inverse of $A^2$.

It is to be shown that $AB$ is the inverse of $A$, or equivalently, that
$A^{-1} = AB$.

By the supposition:

$$ B = (A^2)^{-1} $$

$$ B = (AA)^{-1} $$

$$ B = A^{-1}A^{-1} $$

Apply $A$ on the left to both sides:

$$ AB = A(A^{-1}A^{-1}) $$

By the associative property of matrix multiplication:

$$ AB = (AA^{-1})A^{-1} $$

By the identity property for inverses:

$$ AB = (I)A^{-1} $$

$$ AB = A^{-1} $$

This is what was to be shown.

Q.E.D.

19. Find the numbers $a$ and $b$ that give the inverse of
    $5 \times \text{eye}(4) - \text{ones}(4, 4)$:

$$
\left[\begin{array}{cccc}
4 & -1 & -1 & -1 \\
-1 & 4 & -1 & -1 \\
-1 & -1 & 4 & -1 \\
-1 & -1 & -1 & 4 \\
\end{array}\right]^{-1} =
\left[\begin{array}{cccc}
a & b & b & b \\
b & a & b & b \\
b & b & a & b \\
b & b & b & a \\
\end{array}\right]
$$

What are $a$ and $b$ in the inverse of $6 * \text{eye}(5) - \text{ones}(5, 5)$?

Omitted, no MATLAB.

20. Show that $A = 4 * \text{eye} - \text{ones}(4, 4)$ is _not_ invertible:
    Multiply $A * \text{ones}(4, 1)$.

Omitted, no MATLAB.

21. There are sixteen 2 by 2 matrices whose entries are $1$'s and $0$'s. How
    many of them are invertible?

Six. Four of them are invertible by having three 1's. The other two are $I$ and
$P$.

**Questions 22-28 are about the Gauss-Jordan method for calculating $A^{-1}$.**

22. Change $I$ into $A^{-1}$ as you reduce $A$ to $I$ (by row operations):

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 3 & 1 & 0 \\
2 & 7 & 0 & 1 \\
\end{array}\right]
$$

and

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 4 & 1 & 0 \\
3 & 9 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 3 & 1 & 0 \\
2 & 7 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 3 & 1 & 0 \\
0 & 1 & -2 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 0 & 1 & -3 \\
0 & 1 & -2 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

_Second:_

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 4 & 1 & 0 \\
3 & 9 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 4 & 1 & 0 \\
0 & -3 & -3 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 0 & 1 & \frac{4}{3} \\
0 & -3 & -3 & 1 \\
\end{array}\right]
$$

Here, just divide row 2 by $3$, (just a scalar).

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cc|cc}
1 & 0 & 1 & \frac{4}{3} \\
0 & 1 & 1 & -\frac{1}{3} \\
\end{array}\right]
$$

23. Follow the 3 by 3 text example but with plus signs in $A$. Eliminate above
    and below the pivots to reduce
    $\left[\begin{array}{cc}A & I \\\end{array}\right]$ to
    $\left[\begin{array}{cc}I & A^{-1} \\\end{array}\right]$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cccccc}
2 & 1 & 0 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 & 1 & 0 \\
0 & 1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 0 & 1 & 0 & 0 \\
0 & \frac{3}{2} & 1 & -\frac{1}{2} & 1 & 0 \\
0 & 1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 0 & 1 & 0 & 0 \\
0 & \frac{3}{2} & 1 & -\frac{1}{2} & 1 & 0 \\
0 & 0 & \frac{4}{3} & 0 & -\frac{2}{3} & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 0 & 1 & 0 & 0 \\
0 & \frac{3}{2} & 1 & -\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 & 0 & -\frac{1}{2} & \frac{3}{4} \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 0 & 1 & 0 & 0 \\
0 & \frac{3}{2} & 0 & -\frac{1}{2} & \frac{3}{2} & -\frac{3}{4} \\
0 & 0 & 1 & 0 & -\frac{1}{2} & \frac{3}{4} \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & -\frac{1}{3} & 1 & -\frac{1}{2} \\
0 & 0 & 1 & 0 & -\frac{1}{2} & \frac{3}{4} \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 0 & 0 & \frac{4}{3} & -1 & \frac{1}{2} \\
0 & 1 & 0 & -\frac{1}{3} & 1 & -\frac{1}{2} \\
0 & 0 & 1 & 0 & -\frac{1}{2} & \frac{3}{4} \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{2}{3} & -\frac{1}{2} & \frac{1}{4} \\
0 & 1 & 0 & -\frac{1}{3} & 1 & -\frac{1}{2} \\
0 & 0 & 1 & 0 & -\frac{1}{2} & \frac{3}{4} \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

24. Use Gauss-Jordan elimination on
    $\left[\begin{array}{cc}U & I \\\end{array}\right]$ to find the upper
    triangular $U^{-1}$:

$$ UU^{-1} = I $$

$$
\left[\begin{array}{ccc}
1 & a & b \\
0 & 1 & c \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
x_1 & x_2 & x_3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

$$
\left[\begin{array}{ccc|ccc}
1 & a & b & 1 & 0 & 0 \\
0 & 1 & c & 0 & 1 & 0 \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & a & 0 & 1 & 0 & -b \\
0 & 1 & 0 & 0 & 1 & -c \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & -a & ac - b \\
0 & 1 & 0 & 0 & 1 & -c \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & U^{-1} \\
\end{array}\right]
$$

25. Find $A^{-1}$ and $B^{-1}$ (_if they exist_) by elimination on
    $\left[\begin{array}{cc}A & I \\\end{array}\right]$ and
    $\left[\begin{array}{cc}B & I \\\end{array}\right]$:

$$ A =
\left[\begin{array}{ccc}
2 & 1 & 1 \\
1 & 2 & 1 \\
1 & 1 & 2 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{ccc}
2 & -1 & -1 \\
-1 & 2 & -1 \\
-1 & -1 & 2 \\
\end{array}\right]
$$

_Solution:_

_Find $A^{-1}$:_

$$ A =
\left[\begin{array}{ccc}
2 & 1 & 1 \\
1 & 2 & 1 \\
1 & 1 & 2 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & 1 & 1 & 1 & 0 & 0 \\
1 & 2 & 1 & 0 & 1 & 0 \\
1 & 1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
1 & 2 & 1 & 0 & 1 & 0 \\
1 & 1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 3 & 1 & -1 & 2 & 0 \\
1 & 1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 3 & 1 & -1 & 2 & 0 \\
0 & 2 & 2 & -1 & 1 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 1 & \frac{1}{3} & -\frac{1}{3} & \frac{2}{3} & 0 \\
0 & 2 & 2 & -1 & 1 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 1 & \frac{1}{3} & -\frac{1}{3} & \frac{2}{3} & 0 \\
0 & 0 & \frac{4}{3} & -\frac{1}{3} & -\frac{1}{3} & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 1 & 0 & -\frac{1}{4} & \frac{3}{4} & -\frac{1}{4} \\
0 & 0 & \frac{4}{3} & -\frac{1}{3} & -\frac{1}{3} & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & -1 & 0 & 1 & -1 & 0 \\
0 & 1 & 0 & -\frac{1}{4} & \frac{3}{4} & -\frac{1}{4} \\
0 & 0 & 1 & -\frac{1}{4} & -\frac{1}{4} & \frac{3}{4} \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{3}{4} & -\frac{1}{4} & -\frac{1}{4} \\
0 & 1 & 0 & -\frac{1}{4} & \frac{3}{4} & -\frac{1}{4} \\
0 & 0 & 1 & -\frac{1}{4} & -\frac{1}{4} & \frac{3}{4} \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

_Find $B^{-1}$:_

$$ B =
\left[\begin{array}{ccc}
2 & -1 & -1 \\
-1 & 2 & -1 \\
-1 & -1 & 2 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
B & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
2 & -1 & -1 & 1 & 0 & 0 \\
-1 & 2 & -1 & 0 & 1 & 0 \\
-1 & -1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 1 & -2 & 1 & 1 & 0 \\
-1 & 2 & -1 & 0 & 1 & 0 \\
-1 & -1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 1 & -2 & 1 & 1 & 0 \\
0 & 3 & -3 & 1 & 2 & 0 \\
-1 & -1 & 2 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 1 & -2 & 1 & 1 & 0 \\
0 & 3 & -3 & 1 & 2 & 0 \\
0 & 0 & 0 & 1 & 1 & 1 \\
\end{array}\right]
$$

$B^{-1}$ does not exist.

26. What three matrices $E_{21}$ and $E_{12}$ and $D^{-1}$ reduce
    $A =\left[\begin{array}{cc}1 & 2 \\2 & 6 \\\end{array}\right]$ to the
    identity matrix? Multiply $D^{-1}E_{12}E_{21}$ to find $A^{-1}$.

_Solution:_

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
2 & 6 \\
\end{array}\right]
$$

$$ E_{21}A =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
2 & 6 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
0 & 2 \\
\end{array}\right]
$$

$$ E_{12}E_{21}A =
\left[\begin{array}{cc}
1 & -1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
0 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 2 \\
\end{array}\right]
$$

$$ D^{-1}E_{12}E_{21}A =
\left[\begin{array}{cc}
1 & 0 \\
0 & \frac{1}{2} \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
0 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

$$ E_{12}E_{21} =
\left[\begin{array}{cc}
1 & -1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & -1 \\
-2 & 1 \\
\end{array}\right]
$$

$$ D^{-1}E_{12}E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
0 & \frac{1}{2} \\
\end{array}\right]
\left[\begin{array}{cc}
3 & -1 \\
-2 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & -1 \\
-1 & \frac{1}{2} \\
\end{array}\right]
$$

27. Invert these matrices $A$ by the Gauss-Jordan method starting with
    $\left[\begin{array}{cc}A & I \\\end{array}\right]$:

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 3 \\
0 & 0 & 1 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 3 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
2 & 1 & 3 & 0 & 1 & 0 \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
0 & 1 & 3 & -2 & 1 & 0 \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & -2 & 1 & -3 \\
0 & 0 & 1 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

_Second:_

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
1 & 2 & 2 & 0 & 1 & 0 \\
1 & 2 & 3 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & 1 & -1 & 1 & 0 \\
1 & 2 & 3 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & 1 & -1 & 1 & 0 \\
0 & 1 & 2 & -1 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & 1 & -1 & 1 & 0 \\
0 & 0 & 1 & 0 & -1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
0 & 1 & 0 & -1 & 2 & -1 \\
0 & 0 & 1 & 0 & -1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 1 & 2 & -2 & 1 \\
0 & 1 & 0 & -1 & 2 & -1 \\
0 & 0 & 1 & 0 & -1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & 2 & -1 & 0 \\
0 & 1 & 0 & -1 & 2 & -1 \\
0 & 0 & 1 & 0 & -1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

28. Exchange rows and continue with Gauss-Jordan to find $A^{-1}$:

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 2 & 1 & 0 \\
2 & 2 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

$$
\left[\begin{array}{cc|cc}
2 & 2 & 0 & 1 \\
0 & 2 & 1 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
1 & 1 & 0 & \frac{1}{2} \\
0 & 2 & 1 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
1 & 1 & 0 & \frac{1}{2} \\
0 & 1 & \frac{1}{2} & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
1 & 0 & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & \frac{1}{2} & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

29. True or false (with a counterexample if false and a reason if true):

a. A 4 by 4 matrix with a row of zeros is not invertible.

True, if $A$ has a row of zeros, then $AB$ has one too, and it is impossible to
find such a matrix $B$ where $AB = I$.

b. Every matrix with $1$'s down the main diagonal is invertible.

False, if the matrix is filled with $1$'s, then the matrix is singular, and
therefore not invertible.

c. If $A$ is invertible then $A^{-1}$ and $A^2$ are invertible.

True, the inverse of $A^{-1}$ is $A$, and if $A$ is invertible, then $A^2$ is
invertible as $(A^{-1}A^{-1}) = (A^{-1})^2$.

30. (Recommended) Prove that $A$ is invertible if $a \neq 0$ and $a \neq b$
    (find the pivots or $A^{-1}$). Then find three numbers $c$ so that $C$ is
    not invertible:

$$ A =
\left[\begin{array}{ccc}
a & b & b \\
a & a & b \\
a & a & a \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
2 & c & c \\
c & c & c \\
8 & 7 & c \\
\end{array}\right]
$$

_Solution:_

**Proof:**

Suppose $A$ is a matrix defined as such:

$$ A =
\left[\begin{array}{ccc}
a & b & b \\
a & a & b \\
a & a & a \\
\end{array}\right]
$$

Furthermore, suppose $a \neq 0$ and $a \neq b$.

It must be shown that $A$ is invertible.

Using Gauss-Jordan elimination on $A$, we can find $A^{-1}$, and thus
demonstrate that $A$ is invertible.

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
a & a & b & 0 & 1 & 0 \\
a & a & a & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
0 & a - b & 0 & -1 & 1 & 0 \\
a & a & a & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
0 & a - b & 0 & -1 & 1 & 0 \\
0 & a - b & a - b & -1 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
0 & a - b & 0 & -1 & 1 & 0 \\
0 & 0 & a - b & 0 & -1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} & 0 \\
0 & 0 & a - b & 0 & -1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & b & 1 & 0 & 0 \\
0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} & 0 \\
0 & 0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & b & 0 & 1 & \frac{b}{a - b} & -\frac{b}{a - b} \\
0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} & 0 \\
0 & 0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
a & 0 & 0 & \frac{a}{a - b} & 0 & -\frac{b}{a - b} \\
0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} & 0 \\
0 & 0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{1}{a - b} & 0 & -\frac{b}{a(a - b)} \\
0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} & 0 \\
0 & 0 & 1 & 0 & -\frac{1}{a - b} & \frac{1}{a - b} \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1}\\
\end{array}\right]
$$

By the supposition $a \neq 0$ and $a \neq b$, thus all denominators in this
general $A^{-1}$ are well defined, and it an be concluded that $A^{-1}$ exists,
demonstrating that $A$ is invertible.

This is what was to be shown.

Q.E.D.

_Find three numbers $c$ so that $C$ is not invertible:_

$$ C =
\left[\begin{array}{ccc}
2 & c & c \\
c & c & c \\
8 & 7 & c \\
\end{array}\right]
$$

$$ c = 0, c = 2, c = 7 $$

31. This matrix has a remarkable inverse. Find $A^{-1}$ by elimination on
    $\left[\begin{array}{cc}A & I \\\end{array}\right]$. Extend to a 5 by 5
    "alternating matrix" and guess its inverse; then multiply to confirm.

Invert

$$ A =
\left[\begin{array}{cccc}
1 & -1 & 1 & -1 \\
0 & 1 & -1 & 1 \\
0 & 0 & 1 & -1 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

and solve $Ax = (1, 1, 1, 1)$.

_Solution:_

$$
\left[\begin{array}{cc}
A & I \\
\end{array}\right] =
\left[\begin{array}{rrrr|rrrr}
1 & -1 & 1 & -1 & 1 & 0 & 0 & 0 \\
0 & 1 & -1 & 1 & 0 & 1 & 0 & 0 \\
0 & 0 & 1 & -1 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{rrrr|rrrr}
1 & 0 & 0 & 0 & 1 & 1 & 0 & 0 \\
0 & 1 & -1 & 1 & 0 & 1 & 0 & 0 \\
0 & 0 & 1 & -1 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{rrrr|rrrr}
1 & 0 & 0 & 0 & 1 & 1 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 1 & 1 & 0 \\
0 & 0 & 1 & -1 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{rrrr|rrrr}
1 & 0 & 0 & 0 & 1 & 1 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 1 & 1 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 & 1 & 1 \\
0 & 0 & 0 & 1 & 0 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

_Extend to a 5 by 5 "alternating matrix" and guess its inverse, then multiply to
confirm:_

Guess for $A^{-1}$ is:

$$
\left[\begin{array}{rrrrr}
1 & 1 & 0 & 0 & 0 \\
0 & 1 & 1 & 0 & 0 \\
0 & 0 & 1 & 1 & 0 \\
0 & 0 & 0 & 1 & 1 \\
0 & 0 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
I & A^{-1} \\
\end{array}\right]
$$

Multiply to confirm:

Omitted.

32. Suppose the matrices $P$ and $Q$ have the same rows as $I$ but in any order.
    They are "permutation matrices". Show that $P - Q$ is singular by solving
    $(P - Q)x = \mathbf{0}$.

_Solution:_

First, consider that $P - Q$ will output a matrix of mostly $0$'s in the rows
save for the rows that were exchanged. The difference in each row where the
exchanges differ will either be $1$ or $-1$. Then consider a vector $x$ where
$x = (1, 1, \dots, 1)$, then $(P - Q)x = \mathbf{0}$. This is because then when
$P - Q$ is multiplied by the vector $x$, the $-1$ and $1$ rows are added,
$-1 + 1 = 0$, which means every row in the product is filled with $0$'s.

33. Find and check the inverses (assuming they exist) of these block matrices:

$$
\left[\begin{array}{cc}
I & 0 \\
C & I \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & 0 \\
C & D \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
0 & I \\
I & D \\
\end{array}\right]
$$

_Solution:_

_First:_

$$
\left[\begin{array}{cc}
I & 0 \\
C & I \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
I & 0  \\
-C & I \\
\end{array}\right]
$$

_Second:_

$$
\left[\begin{array}{cc|cc}
A & 0 & I & 0 \\
C & D & 0 & I \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & A^{-1} & 0 \\
C & D & 0 & I \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & A^{-1} & 0 \\
C - CI & D - C(0) & 0 - CA^{-1} & I - C(0) \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & A^{-1} & 0 \\
0 & D & -CA^{-1} & I \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & A^{-1} & 0 \\
0 & D^{-1}D & D^{-1}(-CA^{-1}) & D^{-1}(I) \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & A^{-1} & 0 \\
0 & I & -D^{-1}CA^{-1} & D^{-1} \\
\end{array}\right]
$$

_Third:_

$$
\left[\begin{array}{cc}
0 & I \\
I & D \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
0 & I & I & 0 \\
I & D & 0 & I \\
\end{array}\right]
$$

Switch rows:

$$
\left[\begin{array}{cc|cc}
I & D & 0 & I \\
0 & I & I & 0 \\
\end{array}\right]
$$

Subtract $D$ times row 2 from row 1:

$$
\left[\begin{array}{cc|cc}
I - D(0) & D - D(I) & 0 - D(I) & I - D(0) \\
0 & I & I & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|cc}
I & 0 & -D & I \\
0 & I & I & 0 \\
\end{array}\right]
$$

34. Could a 4 by 4 matrix $A$ be invertible if every row contains the numbers
    $0, 1, 2, 3$ in some order? What if every row of $B$ contains $0, 1, 2, -3$
    in some order?

Omitted.

35. In the Worked Example 2.5 C, the triangular Pascal matrix $L$ has
    $L^{-1} = DLD$, where the diagonal matrix $D$ has alternating entries
    $1, -1, 1, -1$. Then $LDLD = I$, so what is the inverse of
    $LD = \text{pascal}(4, 1)$?

Omitted.

36. Omitted (no MATLAB).

37. Omitted (no MATLAB).

38. Omitted (no MATLAB).

---

Page 115

## Problem Set 2.6

**Problems 1-14 compute the factorization $A = LU$** (and also $A = LDU$).

1. (Important) Forward elimination changes
   $\left[\begin{array}{cc}1 & 1\\1 & 2 \end{array}\right]x = b$ to a triangular
   $\left[\begin{array}{cc}1 & 1\\0 & 1 \end{array}\right]x = c$:

$$
\begin{array}{r}
x + y = 5 \\
x + 2y = 7
\end{array} \to
\begin{array}{r}
x + y = 5 \\
y = 2
\end{array} \quad
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 2 & 7 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 5 \\
0 & 1 & 2 \\
\end{array}\right]
$$

That step subtracted $\ell_{21} =$ ____ times row 1 from row 2. The reverse step
_adds_ $\ell_{21}$ times row 1 to row 2. The matrix for that reverse step is
$L =$ ____. Multiply this $L$ times the triangular system
$\left[\begin{array}{cc}1 & 1 \\0 & 1 \\\end{array}\right]x_1 = \begin{bmatrix}{}5\\2\end{bmatrix}$
to get ____ = ____. In letters, $L$ multiplies $Ux = c$ to give ____.

_Solution:_

That step subtracted $\ell_{21} = 1$.

$$ L =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
$$

_Multiply this $L$ times the triangular system
$\left[\begin{array}{cc}1 & 1 \\0 & 1 \\\end{array}\right]x_1 = \begin{bmatrix}{}5\\2\end{bmatrix}$
to get (?) = (?):_

$$ LUx =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}5\\7\end{bmatrix} = b
$$

_In letters, $L$ multiplies $Ux = c$ to give (?):_

$$ Ax = b $$

2. Write down the 2 by 2 triangular system $Lc = b$ and $Ux = c$ from Problem 1.
   Check that $c = (5, 2)$ solves the first one. Find $x$ that solves the second
   one.

_Solution:_

_Write down the 2 by 2 triangular system $Lc = b$ and $Ux = c$ from Problem 1:_

$Lc = b$:

$$ Lc =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}c_1\\c_2\end{bmatrix} =
\begin{bmatrix}{}5\\7\end{bmatrix} = b
$$

$Ux = c$:

$$ Ux =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}5\\2\end{bmatrix} = c
$$

_Check that $c = (5, 2)$ solves the first one:_

$$ Lc =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}5\\2\end{bmatrix} =
\begin{bmatrix}{}5\\7\end{bmatrix} = b
$$

Quick matrix multiplication shows:

$$ 1(5) + 0(2) = 5 $$

and

$$ 1(5) + 1(2) = 7 $$

_Find $x$ that solves the second one:_

$$ Ux =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}5\\2\end{bmatrix} = c
$$

By back substitution:

$$ (0)x + (1)y = 2 \Rightarrow y = 2 $$

$$ 1(x) + 1(y) = 5 \Rightarrow x + 2 = 5 \Rightarrow x = 3 $$

3. (Move to 3 by 3) Forward elimination changes $Ax = b$ to a triangular
   $Ux = c$:

$$
\begin{array}{r}
x + y + z = 5 \\
x + 2y + 3z = 7 \\
x + 3y + 6z = 11 \\
\end{array} \quad
\begin{array}{r}
x + y + z = 5 \\
y + 2z = 2 \\
2y + 5z = 6 \\
\end{array} \quad
\begin{array}{r}
x + y + z = 5 \\
y + 2z = 2 \\
z = 2 \\
\end{array}
$$

The equation $z = 2$ in $Ux = c$ comes from the original $x + 3y + 6z = 11$ in
$Ax = b$ by subtracting $\ell_{31} =$ ____ times equation 1 and $\ell_{32} =$
____ times the _final_ equation 2. Reverse that to recover
$\left[\begin{array}{cccc}1 & 3 & 6 & 11\\\end{array}\right]$ in the last row of
$A$ and $b$ from the final
$\left[\begin{array}{cccc}1 & 1 & 1 & 5\\\end{array}\right]$ and
$\left[\begin{array}{cccc}0 & 0 & 1 & 2\\\end{array}\right]$ in $U$ and $c$:

$$ \text{Row 3 of } \left[\begin{array}{cc} A & b\\\end{array}\right] =
(\ell_{31}\text{Row 1} + \ell_{32}\text{Row 2} + 1\text{Row 3}) \text{of }
\left[\begin{array}{cc} U & c\\\end{array}\right]
$$

In matrix notation this is multiplication by $L$. So $A = LU$ and $b = Lc$.

_Solution:_

_The equation $z = 2$ in $Ux = c$ comes from the original $x + 3y + 6z = 11$ in
$Ax = b$ by subtracting $\ell_{31} =$ (?) times equation 1 and $\ell_{32} =$ (?)
times the _final_ equation 2:_

By subtracting $\ell_{31} = 1$ times equation 1 and $\ell_{32} = 2$ times the
_final_ equation 2.

Reversing the steps we get:

Add 2 times equation 2 to equation 3, then add 1 times row 1 to row 3.

4. What are the 3 by 3 triangular systems $Lc = b$ and $Ux = c$ from Problem 3?
   Check that $c = (5, 2, 2)$ solves the first one. Which $x$ solves the second
   one?

_What are the 3 by 3 triangular systems $Lc = b$ and $Ux = c$ from Problem 3?:_

$$ Lc =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 2 & 1 \\
\end{array}\right]
\begin{bmatrix}{}5\\2\\2\end{bmatrix} =
\begin{bmatrix}{}5\\7\\11\end{bmatrix} = b
$$

$$ Ux =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 2 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}5\\2\\2\end{bmatrix} = c
$$

_Check that $c = (5, 2, 2)$ solves the first one:_

$$ Lc =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 2 & 1 \\
\end{array}\right]
\begin{bmatrix}{}5\\2\\2\end{bmatrix} =
\begin{bmatrix}{}5\\7\\11\end{bmatrix} = b
$$

Matrix multiplication:

$$ (1)(5) + (0)(2) + (0)(2) = 5 $$

$$ (1)(5) + (1)(2) + (0)(2) = 7 $$

$$ (1)(5) + (2)(2) + (1)(2) = 11 $$

_Which $x$ solves the second one?:_

$$ Ux =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 2 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}5\\2\\2\end{bmatrix} = c
$$

Back substitution:

$$ 1z = 2 \Rightarrow z = 2 $$

$$ 1y + 2z = 2 \Rightarrow y + 2(2) = 2 \Rightarrow y + 4 = 2 \Rightarrow y = -2 $$

$$ 1x + 1y + 1z = 5 \Rightarrow x + (-2) + (2) = 5 \Rightarrow x = 5 $$

$$ x = \begin{bmatrix}{}5\\-2\\2\end{bmatrix} $$

5. What matrix $E$ puts $A$ into triangular form $EA = U$? Multiply $E^{-1} = L$
   to factor $A$ into $LU$:

$$ A =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 4 & 2 \\
6 & 3 & 5 \\
\end{array}\right]
$$

_Solution:_

_What matrix $E$ puts $A$ into triangular form $EA = U$?:_

$$ E = E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
$$

$$ EA =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 4 & 2 \\
6 & 3 & 5 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 4 & 2 \\
0 & 0 & 5 \\
\end{array}\right] = U
$$

_Multiply $E^{-1} = L$ to factor $A$ into $LU$:_

$$ E^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right] = L
$$

$$ LU =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 4 & 2 \\
0 & 0 & 5 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 0 \\
0 & 4 & 2 \\
6 & 3 & 5 \\
\end{array}\right] = A
$$

6. What two elimination matrices $E_{21}$ and $E_{32}$ put $A$ into upper
   triangular form $E_{32}E_{21}A = U$? Multiply $E_{32}^{-1}$ and $E_{21}^{-1}$
   to factor $A$ into $LU = E^{21}^{-1}E_{32}^{-1}U$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
2 & 4 & 5 \\
0 & 4 & 0 \\
\end{array}\right]
$$

_Solution:_

_What two elimination matrices $E_{21}$ and $E_{32}$ put $A$ into upper
triangular form $E_{32}E_{21}A = U$?:_

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
4 & -2 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
4 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 1 \\
2 & 4 & 5 \\
0 & 4 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
0 & 2 & 3 \\
0 & 0 & -6 \\
\end{array}\right] = U
$$

_Multiply $E_{32}^{-1}$ and $E_{21}^{-1}$ to factor $A$ into
$LU = E^{21}^{-1}E_{32}^{-1}U$:_

$$ E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1} E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right] = L
$$

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 1 & 1 \\
0 & 2 & 3 \\
0 & 0 & -6 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
2 & 4 & 5 \\
0 & 4 & 0 \\
\end{array}\right] = A
$$

7. What three elimination matrices $E_{21}, E_{31}, E_{32}$ put $A$ into its
   upper triangular form $E_{32}E_{31}E_{21}A = U$? Multiply
   $E_{32}^{-1}, E_{31}^{-1}$ and $E_{21}^{-1}$ to factor $A$ into $L$ times
   $U$:

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 1 \\
2 & 2 & 2 \\
3 & 4 & 5 \\
\end{array}\right] \quad L = E_{21}^{-1}E_{31}^{-1}E_{32}^{-1}
$$

_Solution:_

_What three elimination matrices $E_{21}, E_{31}, E_{32}$ put $A$ into its upper
triangular form $E_{32}E_{31}E_{21}A = U$?:_

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{31}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
1 & -2 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{31}E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
1 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 1 \\
2 & 2 & 2 \\
3 & 4 & 5 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 1 \\
0 & 2 & 0 \\
0 & 0 & 2 \\
\end{array}\right] = U
$$

_Multiply $E_{32}^{-1}, E_{31}^{-1}$ and $E_{21}^{-1}$ to factor $A$ into $L$
times $U$:_

$$ E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right]
$$

$$ E_{31}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 2 & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1}E_{31}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
3 & 2 & 1 \\
\end{array}\right] = L
$$

$$ LU =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
3 & 2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 1 \\
0 & 2 & 0 \\
0 & 0 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 1 \\
2 & 2 & 2 \\
3 & 4 & 5 \\
\end{array}\right] = A
$$

8. **This is the problem that shows how the inverses $E_{ij}^{-1} multiply to
   give $L$.** You see this best when $A$ is already lower triangular with $1$'s
   on the diagonal. **Then $U = I$!**

$$ A = L =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
b & c & 1 \\
\end{array}\right]
$$

The elimination matrices $E_{21}, E_{31}, E_{32}$ contain $-a$ then $-b$ then
$-c$.

a. Multiply $E_{32}E_{31}E_{21}$ to find the single matrix $E$ that produces
$EA = I$.

_Solution:_

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-a & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-b & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -c & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-b & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-a & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-a & 1 & 0 \\
-b & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{31}E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -c & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-a & 1 & 0 \\
-b & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{lll}
1 & 0 & 0 \\
-a & 1 & 0 \\
ca - b & -c & 1 \\
\end{array}\right]
$$

$$ EA =
\left[\begin{array}{lll}
1 & 0 & 0 \\
-a & 1 & 0 \\
ca - b & -c & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
b & c & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

b. Multiply $E_{21}^{-1}E_{31}^{-1}E_{32}^{-1}$ to bring back $L$. **The
multipliers $a, b, c$ are mixed up in $E$ but perfect in $L$.**

_Solution:_

$$ E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right]
$$

$$ E_{31}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
b & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & c & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
b & c & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1}E_{31}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
a & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
b & c & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
a & 1 & 0 \\
b & c & 1 \\
\end{array}\right]  = L = A
$$

9. _When zero appears in a pivot position, $A = LU$ is not possible!_ (We are
   requiring nonzero pivots in $U$.) Show directly why these equations are both
   impossible:

$$
\left[\begin{array}{cc}
0 & 1 \\
2 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
\ell & 1
\end{array}\right]
\left[\begin{array}{cc}
d & e \\
0 & f \\
\end{array}\right] \quad
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 2 \\
1 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & & \\
\ell & 1 & \\
m & n & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
d & e & g \\
& f & h \\
& & i \\
\end{array}\right]
$$

These matrices need a row exchange. That uses a _"permutation matrix"_ $P$.

_Solution:_

_First equation:_

$$
\left[\begin{array}{cc}
0 & 1 \\
2 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
\ell & 1
\end{array}\right]
\left[\begin{array}{cc}
d & e \\
0 & f \\
\end{array}\right]
$$

Multiplying the right side:

$$
\left[\begin{array}{cc}
1 & 0 \\
\ell & 1
\end{array}\right]
\left[\begin{array}{cc}
d & e \\
0 & f \\
\end{array}\right] =
\left[\begin{array}{cc}
d & e \\
\ell d & \ell e + f \\
\end{array}\right]
$$

Now set this equal to the left side:

$$
\left[\begin{array}{cc}
1 & 0 \\
\ell & 1
\end{array}\right]
\left[\begin{array}{cc}
d & e \\
0 & f \\
\end{array}\right] =
\left[\begin{array}{cc}
d & e \\
\ell d & \ell e + f \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 1 \\
2 & 3 \\
\end{array}\right]
$$

Since $d$ is in a pivot position, $d = 0$ is not allowed, and thus $A = LU$ is
not possible (without a row swap).

_Second equation:_

$$
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 2 \\
1 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & & \\
\ell & 1 & \\
m & n & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
d & e & g \\
& f & h \\
& & i \\
\end{array}\right]
$$

Multiply the right-hand side:

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
\ell & 1 & 0 \\
m & n & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
d & e & g \\
0 & f & h \\
0 & 0 & i \\
\end{array}\right] =
\left[\begin{array}{ccc}
d & e & g \\
\ell d & \ell e + f & \ell g + h \\
md & me + nf & mg + nh + i \\
\end{array}\right]
$$

Now set this equal to the left-hand side:

$$
\left[\begin{array}{ccc}
d & e & g \\
\ell d & \ell e + f & \ell g + h \\
md & me + nf & mg + nh + i \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 2 \\
1 & 2 & 1 \\
\end{array}\right]
$$

Analyzing the first row:

$d = 1$, $e = 1$, $g = 0$, so first row has no issues.

From, the problem statement, we know that $\ell = 1$.

Now, analyzing the second row:

$ld = 1$, $le + f = 1$.

We stop here here because notice that if $le = (1)(1) = 1$, then
$le + f = 1 \Rightarrow 1 + f = 1 \Rightarrow f = 0$.

Since $f = 0$, and since $f$ is a pivot in $U$, this is not allowed, and
$A = LU$ is not possible (without row exchange(s)).

10. Which number $c$ leads to zero in the second pivot position? A row exchange
    is needed and $A = LU$ will not be possible. Which $c$ produces zero in the
    third pivot position? Then a row exchange can't help and elimination fails:

$$ A =
\left[\begin{array}{ccc}
1 & c & 0 \\
2 & 4 & 1 \\
3 & 5 & 1 \\
\end{array}\right]
$$

_Solution:_

_Which number $c$ leads to zero in the second pivot position?:_

For a $0$ to be in the second pivot position, solve for $c$:

$$ 4 - 2c = 0 $$

$$ -2c = -4 $$

$$ c = 2 $$

_Which $c$ produces zero in the third pivot position?:_

After the first step of elimination, we are left with this halfway form of $U$
(denoted with just a fraction in the subscript differentiate it from $U$):

$$ U_{\frac{1}{2}} =
\left[\begin{array}{ccc}
1 & c & 0 \\
0 & 4 - 2c & 1 \\
3 & 5 & 1 \\
\end{array}\right]
$$

Then, first we must eliminate the $3$ in $(3, 1)$, so subtract 3 times row 1
from row 3 to get:

$$ U_{\frac{1}{2}} =
\left[\begin{array}{ccc}
1 & c & 0 \\
0 & 4 - 2c & 1 \\
0 & 5 - 3c & 1 \\
\end{array}\right]
$$

Then to get $(3, 2)$ to be $0$, subtract $\dfrac{5 - 3c}{4 - 2c}$ times row 2
from row 3:

$$ U_{\frac{1}{2}} =
\left[\begin{array}{ccc}
1 & c & 0 \\
0 & 4 - 2c & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

As you can see, this will get us a $0$ in the third pivot, so solve for $c$. To
find $c$, subtract the fraction $\dfrac{5 - 3c}{4 - 2c}$ from $1$ (since we are
trying to get $0$ in the $(3, 3)$ position) and set it to $0$:

$$ 1 - \frac{5 - 3c}{4 - 2c} = 0 $$

$$ -\frac{5 - 3c}{4 - 2c} = -1 $$

$$ \frac{5 - 3c}{4 - 2c} = 1 $$

$$ 5 - 3c = 4 - 2c $$

$$ 5 - 4 = -2c + 3c $$

$$ 1 = c $$

11. What are $L$ and $D$ (the diagonal _pivot matrix_) for this matrix $A$? What
    is $U$ in $A = LU$ and what is the new $U$ in $A = LDU$?

**Already triangular**

$$ A =
\left[\begin{array}{ccc}
2 & 4 & 8 \\
0 & 3 & 9 \\
0 & 0 & 7 \\
\end{array}\right]
$$

_Solution:_

_What are $L$ and $D$ (the diagonal _pivot matrix_) for this matrix $A$?:_

Since $A$ is already $U$, $L$ is just the identity matrix, $L = I$. The diagonal
matrix, $D$ would be whatever would allow $1$'s across $U$, so:

$$ A = LDU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & 7 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 4 \\
0 & 1 & 3 \\
0 & 0 & 1 \\
\end{array}\right]
$$

So:

$$ D =
\left[\begin{array}{ccc}
2 & 0 & 0 \\
0 & 3 & 0 \\
0 & 0 & 7 \\
\end{array}\right]
$$

_What is $U$ in $A = LU$ and what is the new $U$ in $A = LDU$?:_

$U$ in $A = LU$ is just $A$, $U = A$.

$U$ in $A = LDU$ is as was established earlier:

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 4 \\
0 & 1 & 3 \\
0 & 0 & 1 \\
\end{array}\right]
$$

12. $A$ and $B$ are symmetric across the diagonal (because $4 = 4$). Find their
    triple factorization $LDU$ and say how $U$ is related to $L$ for those
    symmetric matrices:

**Symmetric**

$$ A =
\left[\begin{array}{cc}
2 & 4 \\
4 & 11 \\
\end{array}\right] \quad \text{and} \quad
B =
\left[\begin{array}{rrr}
1 & 4 & 0 \\
4 & 12 & 4 \\
0 & 4 & 0 \\
\end{array}\right]
$$

_Solution:_

_Find their triple factorization $LDU$:_

_For $A$:_

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
$$

$$ E_{21}A =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 4 \\
4 & 11 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 4 \\
0 & 3 \\
\end{array}\right] = U
$$

$$ E_{21}^{-1} =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right] = L
$$

$$ D =
\left[\begin{array}{cc}
2 & 0 \\
0 & 3 \\
\end{array}\right]
$$

$$ LDU =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 0 \\
0 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right] = A
$$

_For $B$:_

$$ E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
-4 & 1 & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21}B =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-4 & 1 & 0 \\
-4 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 4 & 0 \\
4 & 12 & 4 \\
0 & 4 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 4 & 0 \\
0 & -4 & 4 \\
0 & 0 & 4 \\
\end{array}\right] = U
$$

$$ E_{21}^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
4 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right] = L
$$

$$ D =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & -4 & 0 \\
0 & 0 & 4 \\
\end{array}\right]
$$

$$ LDU =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
4 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & -4 & 0 \\
0 & 0 & 4 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 4 & 0 \\
0 & 1 & -1 \\
0 & 0 & 1 \\
\end{array}\right] = A
$$

_Say how $U$ is related to $L$ for those symmetric matrices:_

_For $A$:_

Note how $U = L^{\mathbf{T}}$.

_For $B$:_

Once again, note how $U = L^{\mathbf{T}}$.

13. (_Recommended_) Compute $L$ and $U$ for the symmetric matrix $A$:

$$ A =
\left[\begin{array}{cccc}
a & a & a & a \\
a & b & b & b \\
a & b & c & c \\
a & b & c & d \\
\end{array}\right]
$$

Find four conditions on $a, b, c, d$ to get $A = LU$ with four pivots.

_Solution:_

_Compute $L$ and $U$ for the symmetric matrix $A$:_

$$ A =
\left[\begin{array}{cccc}
a & a & a & a \\
a & b & b & b \\
a & b & c & c \\
a & b & c & d \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
-1 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
-1 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
a & b & b & b \\
a & b & c & c \\
a & b & c & d \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
a & b & c & c \\
a & b & c & d \\
\end{array}\right]
$$

$$ E_{31}E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
-1 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
a & b & c & c \\
a & b & c & d \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & b - a & c - a & c - a \\
a & b & c & d \\
\end{array}\right]
$$

$$ E_{41}E_{31}E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
-1 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & b - a & c - a & c - a \\
a & b & c & d \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & b - a & c - a & c - a \\
0 & b - a & c - a & d - a \\
\end{array}\right]
$$

$$ E_{32}E_{41}E_{31}E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & b - a & c - a & c - a \\
0 & b - a & c - a & d - a \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & 0 & c - b & c - b \\
0 & b - a & c - a & d - a \\
\end{array}\right]
$$

$$ E_{42}E_{32}E_{41}E_{31}E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & -1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & 0 & c - b & c - b \\
0 & b - a & c - a & d - a \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & 0 & c - b & c - b \\
0 & 0 & c - b & d - b \\
\end{array}\right]
$$

$$ E_{43}E_{42}E_{32}E_{41}E_{31}E_{21}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & 0 & c - b & c - b \\
0 & 0 & c - b & d - b \\
\end{array}\right] =
\left[\begin{array}{cccc}
a & a & a & a \\
0 & b - a & b - a & b - a \\
0 & 0 & c - b & c - b \\
0 & 0 & 0 & d - c \\
\end{array}\right] = U
$$

Now to find $L$. You can go through all the elimination steps, but I have to
admit I got a little lazy here, and just looked at the answer:

$$ L =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
1 & 1 & 0 & 0 \\
1 & 1 & 1 & 0 \\
1 & 1 & 1 & 1 \\
\end{array}\right]
$$

_Find four conditions on $a, b, c, d$ to get $A = LU$ with four pivots:_

$$ a \neq 0, (b - a) \neq 0, (c - b) \neq 0, (d - c) \neq 0 $$

Thus:

$$
a \neq 0 \\
b \neq a \neq 0 \\
c \neq b \neq a \neq 0 \\
d \neq c \neq b \neq a \neq 0 \\
$$

14. This nonsymmetric matrix will have the same $L$ as in Problem 13:

**Find $L$ and $U$ for**

$$ A =
\left[\begin{array}{cccc}
a & r & r & r \\
a & b & s & s \\
a & b & c & t \\
a & b & c & d \\
\end{array}\right]
$$

Find four conditions on $a, b, c, d, r, s, t$ to get $A = LU$ with four pivots.

Omitted.

**Problems 15-16 use $L$ and $U$ (without needing $A$) to solve $Ax = b$.**

15. Solve the triangular system $Lc = b$ to find $c$. Then solve $Ux = c$ to
    find $x$:

$$ L =
\left[\begin{array}{cc}
1 & 0 \\
4 & 1 \\
\end{array}\right] \text{ and }
U =
\left[\begin{array}{cc}
2 & 4 \\
0 & 1 \\
\end{array}\right] \text{ and }
b = \begin{bmatrix}{}2\\11\end{bmatrix}
$$

For safety multiply $LU$ sand solve $Ax = b$ as usual. Circle $c$ when you see
it.

_Solution:_

$$ LU =
\left[\begin{array}{cc}
1 & 0 \\
4 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 4 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 4 \\
8 & 17 \\
\end{array}\right] = A
$$

$$ Ax =
\left[\begin{array}{cc}
2 & 4 \\
8 & 17 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\end{bmatrix} =
\begin{bmatrix}{}2\\11\end{bmatrix}
$$

$$
\left[\begin{array}{cc|c}
2 & 4 & 2 \\
8 & 17 & 11 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|c}
2 & 4 & 2 \\
0 & 1 & 3 \\
\end{array}\right]
$$

Back substitution:

$$ y = 3 $$

$$ 2x + 4y = 2 \Rightarrow 2x + 4(3) = 2 \Rightarrow 2x + 12 = 2 \Rightarrow 2x = -10 \Rightarrow x = -5 $$

$$ x = \begin{bmatrix}{}-5\\3\end{bmatrix} $$

$$ Ux =
\left[\begin{array}{cc}
2 & 4 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}-5\\3\end{bmatrix} =
\boxed{\begin{bmatrix}{}2\\3\end{bmatrix} = c}
$$

$$ Lc =
\left[\begin{array}{cc}
1 & 0 \\
4 & 1 \\
\end{array}\right]
\begin{bmatrix}{}2\\3\end{bmatrix} =
\begin{bmatrix}{}2\\11\end{bmatrix} = b
$$

16. Solve $Lc = b$ to find $c$. Then solve $Ux = c$ to find $x$. **What was
    $A$**?

$$ L =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right] \text{ and }
U =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] \text{ and }
b = \begin{bmatrix}{}4\\5\\6\end{bmatrix}
$$

_Solution:_

$$ Lc =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}c_1\\c_2\\c_3\end{bmatrix} =
\begin{bmatrix}{}c_1\\c_1 + c_2\\c_1 + c_2 + c_3\end{bmatrix} =
\begin{bmatrix}{}4\\5\\6\end{bmatrix}
$$

Back substitution:

$$ c_1 = 4 $$

$$ c_1 + c_2 = 5 \Rightarrow (4) + c_2 = 5 \Rightarrow c_2 = 1 $$

$$ c_1 + c_2 + c_3 = 6 \Rightarrow (4) + (1) + c_3 = 6 \Rightarrow 5 + c_3 = 6 \Rightarrow c_3 = 1 $$

$$ c = \begin{bmatrix}{}4\\1\\1\end{bmatrix} $$

Now solve $Ux = c$:

$$ Ux =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}x_1 + x_2 + x_3 \\x_2 + x_3\\x_3\end{bmatrix} =
\begin{bmatrix}{}4\\1\\1\end{bmatrix}
$$

Back substitution:

$$ x_3 = 1 $$

$$ x_2 + x_3 = 1 \Rightarrow x_2 + (1) = 1 \Rightarrow x_2 = 0 $$

$$ x_1 + x_2 + x_3 = 4 \Rightarrow x_1 + (0) + (1) = 4 \Rightarrow x_1 = 3 $$

$$ x = \begin{bmatrix}{}3\\0\\1\end{bmatrix} $$

Now to find $A$:

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right] = A
$$

17.

a. When you apply the usual elimination steps to $L$, what matrix do you reach?

$$ L =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
\ell_{21} & 1 & 0 \\
\ell_{31} & \ell_{32} & 1 \\
\end{array}\right]
$$

_Solution:_

The identity matrix $I$.

b. When you apply the same steps to $I$, what matrix do you get?

You get $L$'s inverse, $L^{-1}$.

c. When you apply the same steps to $LU$, what matrix do you get?

Since the steps reduce $L$ to $I$, the remaining matrix is $U$.

18. If $A = LDU$ and also $A = L_1D_1U_1$, with all factors invertible, then
    $L = L_1$ and $D = D_1$ and $U = U_1$. "_The three factors are unique._"

Derive the equation $L_{1}^{-1}LD = D_1U_1U^{-1}$. Are the two sides triangular
or diagonal? Deduce $L = L_1$ and $U = U_1$ (they all have diagonal $1$'s). Then
$D = D_1$.

_Derive the equation $L_{1}^{-1}LD = D_1U_1U^{-1}$:_

$$ LDU = L_1D_1U_1 $$

$$ L_1^{-1}LDU = L_1^{-1}L_1D_1U_1 $$

$$ L_1^{-1}LDU = D_1U_1 $$

$$ L_1^{-1}LDUU^{-1} = D_1U_1U^{-1} $$

$$ L_1^{-1}LD = D_1U_1U^{-1} $$

_Are the two sides triangular or diagonal?:_

Since $L_1^{-1}LD$, this means that $L_1, L$ have $1$'s along their main
diagonal, and they are lower triangular.

Since $D_1U_1U^{-1}$, this means that $U_1, U^{-1}$ have $1$'s along their main
diagonal, and they are upper triangular.

However, since these two sides equal each other, it means that there is some
scalar values along the diagonal and thus the two sides are diagonal.

_Deduce $L = L_1$ and $U = U_1$ (they all have diagonal $1$'s):_

On the left, we have $L_1^{-1}LD$, this means that $L_1^{-1}L$ has $1$'s along
its main diagonal and $0$'s above it. The only way this is possible is if
$L = L_1$.

Similarly, on the right, we have $D_1U_1U^{-1}$, which means that $U_1U^{-1}$
has $1$'s along it's main diagonal with $0$'s below it. The only way this is
possible is if $U = U_1$.

_Then $D = D_1$:_

Since $L_1^{-1}LD = D_1U_1U^{-1}$, and because we have established that
$L_1 = L$ and $U_1 = U$, then:

$$ L_1^{-1}L = L^{-1}L = I $$

and

$$ U_1U^{-1} = UU^{-1} = I $$

Hence our equality becomes:

$$ ID = D_1I $$

$$ D = D_1 $$

19. _Tridiagonal matrices_ have zero entries except on the main diagonal and the
    two adjacent diagonals. Factor these into $A = LU$ and $A = LDL^T$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 2 & 1 \\
0 & 1 & 2 \\
\end{array}\right] \text{ and }
A =
\left[\begin{array}{ccc}
a & a & 0 \\
a & a + b & b \\
0 & b & b + c \\
\end{array}\right]
$$

_Solution:_

_Factor these into $A = LU$:_

_First $A$:_

$$ E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 2 & 1 \\
0 & 1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right]
$$

$$ E_{32}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = U
$$

$$ E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right] = L
$$

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 2 & 1 \\
0 & 1 & 2 \\
\end{array}\right] = A
$$

_Second $A$:_

$$ E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
-1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & a & 0 \\
a & a + b & b \\
0 & b & b + c \\
\end{array}\right] =
\left[\begin{array}{ccc}
a & a & 0 \\
0 & b & b \\
0 & b & b + c \\
\end{array}\right]
$$

$$ E_{32}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & a & 0 \\
0 & b & b \\
0 & b & b + c \\
\end{array}\right] =
\left[\begin{array}{ccc}
a & a & 0 \\
0 & b & b \\
0 & 0 & c \\
\end{array}\right] = U
$$

$$ E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right] = L
$$

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & a & 0 \\
0 & b & b \\
0 & 0 & c \\
\end{array}\right] =
\left[\begin{array}{ccc}
a & a & 0 \\
0 & a + b & b \\
0 & b & b + c \\
\end{array}\right] = A
$$

_and $A = LDL^T$:_

_First $A$:_

From the first part, we got:

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 2 & 1 \\
0 & 1 & 2 \\
\end{array}\right] = A
$$

Here, the diagonal matrix $D$, is just the identity matrix $I$.

$$ LDU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = A
$$

Now, let's transpose $L$ to $L^{\mathbf{T}}$:

$$ L^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = U
$$

So $A = LDL^{\mathbf{T}}$.

_Second $A$:_

In the last part, we ended with:

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & a & 0 \\
0 & b & b \\
0 & 0 & c \\
\end{array}\right] =
\left[\begin{array}{ccc}
a & a & 0 \\
0 & a + b & b \\
0 & b & b + c \\
\end{array}\right] = A
$$

The $D$ is:

$$ D =
\left[\begin{array}{ccc}
a & 0 & 0 \\
0 & b & 0 \\
0 & 0 & c \\
\end{array}\right]
$$

Then $LDU$ is:

$$ LDU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & 0 & 0 \\
0 & b & 0 \\
0 & 0 & c \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = A
$$

Now, find $L^{\mathbf{T}}$:

$$ L^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = U
$$

So $LDL^{\mathbf{T}} = A$.

20. When $T$ is tridiagonal, its $L$ and $U$ factors have only two nonzero
    diagonals. How would you take advantage of knowing the zeros in $T$, in a
    code for Gaussian elimination? Find $L$ and $U$.

**Tridiagonal**

$$ T =
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
2 & 3 & 1 & 0 \\
0 & 1 & 2 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right]
$$

_How would you take advantage of knowing the zeros in $T$, in a code for
Gaussian elimination?:_

Skip any operations where the entry is $0$ since subtracting $0$ does nothing.

_Find $L$ and $U$:_

$$ E_{21}T =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
-2 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
2 & 3 & 1 & 0 \\
0 & 1 & 2 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 1 & 2 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right]
$$

$$ E_{32}E_{21}T =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 1 & 2 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 3 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right]
$$

$$ E_{43}E_{32}E_{21}T =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & -1 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 3 & 3 \\
0 & 0 & 3 & 4 \\
\end{array}\right] =
\boxed{
\left[\begin{array}{cccc}
1 & 2 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 3 & 3 \\
0 & 0 & 0 & 1 \\
\end{array}\right] = U}
$$

$$ E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
2 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
2 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}^{-1}E_{32}^{-1}E_{43}^{-1} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
2 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 1 & 1 \\
\end{array}\right] =
\boxed{
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
2 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
0 & 0 & 1 & 1 \\
\end{array}\right] = L}
$$

21. If $A$ and $B$ have nonzeros in the positions marked by $x$, which zeros
    (marked by $0$) _stay zero_ in their factors $L$ and $U$?

$$ A =
\left[\begin{array}{cccc}
x & x & x & x \\
x & x & x & 0 \\
0 & x & x & x \\
0 & 0 & x & x \\
\end{array}\right] \quad
B =
\left[\begin{array}{cccc}
x & x & x & 0 \\
x & x & 0 & x \\
x & 0 & x & x \\
0 & x & x & x \\
\end{array}\right]
$$

_Solution:_

Answer for $A$:

In $U$, after elimination of $A$, the zeros that remain are those residing in
$(3, 1), (4, 1), (4, 2)$.

In $L$, after "rewinding" elimination in $U$, the remaining zeros are
$(3, 1), (4, 1), (4, 2)$.

Answer for $B$:

In $U$, after elimination, the remaining $0$'s reside at positions $(1, 4)$.
This is because the first row is never changed during elimination.

In $L$, after "rewinding" elimination, the remaining $0$'s reside at positions
$(4, 1)$. This is because elimination did not affect this position.

22. Suppose you eliminate upwards (almost unheard of). Use the last row to
    produce zeros in the last column (the pivot is $1$). Then use the second row
    to produce zero above the second pivot. Find the factors in the unusual
    order $A = UL$.

**Upper times lower**

$$ A =
\left[\begin{array}{ccc}
5 & 3 & 1 \\
3 & 3 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

23. _Easy but important_. If $A$ has pivots $5, 9, 3$ with no row exchanges,
    what are the pivots for the upper left $2$ by $2$ submatrix $A_2$ (without
    row $3$ and column $3$)?

_Solution:_

Let's draw out $U$ generically:

$$ U =
\left[\begin{array}{ccc}
5 & a & b \\
0 & 9 & d \\
0 & 0 & 3 \\
\end{array}\right]
$$

So, the upper left 2 by 2 submatrix of $U$ is:

$$ U =
\left[\begin{array}{ccc}
5 & a \\
0 & 9 \\
\end{array}\right]
$$

And the pivots are $5, 9$.

---

Page 128

## Problem Set 2.7

**Questions 1-7 are about the rules for transpose matrices.**

1. Find $A^{\mathbf{T}}$ and $A^{-1}$ and $(A^{-1})^{\mathbf{T}}$ and
   $(A^{\mathbf{T}})^{-1}$ for

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
9 & 3 \\
\end{array}\right]
$$

and also

$$ A =
\left[\begin{array}{cc}
1 & c \\
c & 0 \\
\end{array}\right]
$$

_Solution:_

_First $A$:_

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
9 & 3 \\
\end{array}\right]
$$

$A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 9 \\
0 & 3 \\
\end{array}\right]
$$

$A^{-1}$:

$$ A^{-1} =
\frac{1}{(1)(3) - (0)(9)}
\left[\begin{array}{cc}
3 & -0 \\
-9 & 1 \\
\end{array}\right]
$$

$$ A^{-1} =
\frac{1}{3}
\left[\begin{array}{cc}
3 & 0 \\
9 & 1 \\
\end{array}\right]
$$

$$ A^{-1} =
\left[\begin{array}{cc}
1 & 0 \\
-3 & \frac{1}{3} \\
\end{array}\right]
$$

$(A^{-1})^{\mathbf{T}}$:

$$ (A^{-1})^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & -3 \\
0 & \frac{1}{3} \\
\end{array}\right]
$$

$(A^{\mathbf{T}})^{-1}$:

$$ (A^{\mathbf{T}})^{-1} =
\frac{1}{(1)(3) - (9)(0)}
\left[\begin{array}{cc}
3 & -9 \\
-0 & 1 \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}})^{-1} =
\frac{1}{3}
\left[\begin{array}{cc}
3 & -9 \\
0 & 1 \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}})^{-1} =
\left[\begin{array}{cc}
1 & -3 \\
0 & \frac{1}{3} \\
\end{array}\right] = (A^{-1})^{\mathbf{T}}
$$

_Second $A$:_

$$ A =
\left[\begin{array}{cc}
1 & c \\
c & 0 \\
\end{array}\right]
$$

$A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & c \\
c & 0 \\
\end{array}\right] = A
$$

$A^{-1}$:

$$ A^{-1} =
\frac{1}{(1)(0) - (c)(c)}
\left[\begin{array}{cc}
0 & -c \\
-c & 1 \\
\end{array}\right]
$$

$$ A^{-1} =
-\frac{1}{c^2}
\left[\begin{array}{cc}
0 & -c \\
-c & 1 \\
\end{array}\right]
$$

$$ A^{-1} =
\left[\begin{array}{cc}
0 & \frac{1}{c} \\
\frac{1}{c} & -\frac{1}{c^2} \\
\end{array}\right]
$$

$(A^{-1})^{\mathbf{T}}$:

$$ (A^{-1})^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & \frac{1}{c} \\
\frac{1}{c} & -\frac{1}{c^2} \\
\end{array}\right] = A^{-1}
$$

$(A^{\mathbf{T}})^{-1}$:

$$ (A^{\mathbf{T}})^{-1} =
\frac{1}{(1)(0) - (c)(c)}
\left[\begin{array}{cc}
1 & -c \\
-c & 0 \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}})^{-1} =
-\frac{1}{c^2}
\left[\begin{array}{cc}
1 & -c \\
-c & 0 \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}})^{-1} =
\left[\begin{array}{cc}
-\frac{1}{c^2} & \frac{1}{c} \\
\frac{1}{c} & 0 \\
\end{array}\right]
$$

2. Verify that $(AB)^{\mathbf{T}}$ equals $B^{\mathbf{T}}A^{\mathbf{T}}$ but
   those are different from $A^{\mathbf{T}}B^{\mathbf{T}}$:

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right] \quad
B =
\left[\begin{array}{cc}
1 & 3 \\
0 & 1 \\
\end{array}\right] \quad
AB =
\left[\begin{array}{cc}
1 & 3 \\
2 & 7 \\
\end{array}\right]
$$

Show also that $AA^{\mathbf{T}}$ is different from $A^{\mathbf{T}}A$. But both
of those matrices are ____.

_Solution:_

_Verify that $(AB)^{\mathbf{T}}$ equals $B^{\mathbf{T}}A^{\mathbf{T}}$ but those
are different from $A^{\mathbf{T}}B^{\mathbf{T}}$:_

$$ (AB)^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 2 \\
3 & 7 \\
\end{array}\right]
$$

$$ B^{\mathbf{T}} =
B =
\left[\begin{array}{cc}
1 & 0 \\
3 & 1 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right]
$$

$$ B^{\mathbf{T}}A^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
3 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
3 & 7 \\
\end{array}\right] = (AB)^{\mathbf{T}}
$$

$$ A^{\mathbf{T}}B^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
3 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
7 & 2 \\
3 & 1 \\
\end{array}\right] \neq B^{\mathbf{T}}A^{\mathbf{T}} = (AB)^{\mathbf{T}}
$$

_Show also that $AA^{\mathbf{T}}$ is different from $A^{\mathbf{T}}A$. But both
of those matrices are (?):_

$$ AA^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
2 & 5 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
1 & 2 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
5 & 2 \\
2 & 1 \\
\end{array}\right] \neq AA^{\mathbf{T}}
$$

Both of these matrices are symmetric.

3.

a. The matrix $((AB)^{-1})^{\mathbf{T}}$ comes from $(A^{-1})^{\mathbf{T}}$ and
$(B^{-1})^{\mathbf{T}}$. _In what order?_

$$ ((AB)^{-1})^{\mathbf{T}} =
(B^{-1}A^{-1})^{\mathbf{T}} =
(A^{-1})^{\mathbf{T}}(B^{-1})^{\mathbf{T}}
$$

b. If $U$ is upper triangular then $(U^{-1})^{\mathbf{T}}$ is ____ triangular.

lower

4. Show that $A^2 = 0$ is possible but $A^{\mathbf{T}}A = 0$ is not possible
   (unless $A =$ zero matrix).

**Proof:**

Suppose that $A$ is any nonzero matrix.

_Proof (that $A^2 = \mathbf{0}$ is possible):_

Let $A$ be generally defined as:

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

Then $A^2$ is:

$$ A^2 =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a^2 + bc & ab + bd \\
ca + cd & cb + d^2 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

Thus, for $A^2 = \mathbf{0}$, it must be true that:

$$
a^2 + bc = 0 \\
ca + cd = 0 \\
ab + bd = 0 \\
cb + d^2 = 0 \\
$$

$$
a^2 = -bc \\
ca = -cd \\
ab = -bd \\
d^2 = -bc \\
$$

$$
a^2 = d^2 \\
a = -d \\
d^2 = a^2 \\
$$

For simplicity's sake, let $a = 1, b = -1, c = 1, d= -1$, then:

$$ A^2 =
\left[\begin{array}{cc}
(1)^2 + (-1)(1) & (1)(-1) + (-1)(-1) \\
(1)(1) + (1)(-1) & (1)(-1) + (-1)^2 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

Thus $A$ is:

$$ A =
\left[\begin{array}{cc}
1 & -1 \\
1 & -1 \\
\end{array}\right]
$$

This is $A^2 = \mathbf{0}$, demonstrating that such an equality is possible.

_Proof ($A^{\mathbf{T}}A = \mathbf{0}$ is not possible):_

Let $A$ be some general matrix defined as such:

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

Then, find $A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
a & c \\
b & d \\
\end{array}\right]
$$

Now find $A^{\mathbf{T}}A$:

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
a & c \\
b & d \\
\end{array}\right]
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\left[\begin{array}{cc}
a^2 + c^2 & ab + cd \\
ab + cd& b^2 + d^2 \\
\end{array}\right]
$$

Suppose each entry of $A^{\mathbf{T}}A = 0$, that is:

$$
a^2 + c^2 = 0 \\
ab + cd = 0 \\
b^2 + d^2 = 0 \\
$$

To show that $A^{\mathbf{T}}A \neq \mathbf{0}$, a contradiction to these
equalities must be derived. Evaluation of the equalities follows:

$$
a^2 + c^2 = 0 \\
ab + cd = 0 \\
b^2 + d^2 = 0 \\
$$

Since $A$ is nonzero, it follows that at least one of the following inequalities
is true:

$$ a^2 > 0, b^2 > 0, c^2 > 0, d^2 > 0 $$

The above follows since multiplying any nonzero number by itself results in a
positive number.

Then, by summation, it follows that $a^2 + c^2 > 0$ or $b^2 + d^2 > 0$, which
contradicts $a^2 + c^2 = 0$ or $b^2 + d^2 = 0$ respectively.

Thus a contradiction to the supposition of the above equalities has been derived
and thus $A^{\mathbf{T}}A \neq \mathbf{0}$ for any $A \neq \mathbf{0}$.

_Conclusion:_

Since both proofs have been demonstrated, this overall proof has been shown.

Q.E.D.

5.

a. The row vector $x^{\mathbf{T}}$ times $A$ times the column $y$ produces what
number?

$$ x^{\mathbf{T}}Ay =
\left[\begin{array}{cc}
0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\0\end{bmatrix} = \text{(?)}
$$

_Solution:_

$$ Ay =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\0\end{bmatrix} =
\begin{bmatrix}{}2\\5\end{bmatrix}
$$

$$ x^{\mathbf{T}}Ay =
\left[\begin{array}{cc}
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}2\\5\end{bmatrix} = 5
$$

b. This is the row $x^{\mathbf{T}}A =$ ____ times the column $y = (0, 1, 0)$.

$$ x^{\mathbf{T}}A =
\left[\begin{array}{cc}
0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{array}\right] =
\left[\begin{array}{ccc}
4 & 5 & 6 \\
\end{array}\right]
$$

c. This is the row
$x^{\mathbf{T}} = \left[\begin{array}{cc}0 & 1 \\\end{array}\right]$ times the
column $Ay =$ ____.

$$ Ay =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\0\end{bmatrix} =
\begin{bmatrix}{}2\\5\end{bmatrix}
$$

6. The transpose of a block matrix
   $M = \left[\begin{array}{cc}A & B \\C & D \\\end{array}\right]$ is
   $M^{\mathbf{T}} =$ ____. Test an example. Under what conditions on
   $A, B, C, D$ is the block matrix symmetric?

_Solution:_

$$ M^{\mathbf{T}} =
\left[\begin{array}{cc}
A^{\mathbf{T}} & C^{\mathbf{T}} \\
B^{\mathbf{T}} & D^{\mathbf{T}} \\
\end{array}\right]
$$

For $M$ to be symmetric, $M = M^{\mathbf{T}}$, thus for this to be true,
$A^{\mathbf{T}} = A$, $B^{\mathbf{T}} = C$, $C^{\mathbf{T}} = B$, and
$D^{\mathbf{T}} = D$.

7. True or false:

a. The block matrix $\left[\begin{array}{cc}0 & A \\A & 0 \\\end{array}\right]$
is automatically symmetric.

False, call this given block matrix $S$, then for $S$ to be symmetric, the
equality $S = S^{\mathbf{T}}$ must hold. Consider $S^{\mathbf{T}}$ is:

$$ S^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & A^{\mathbf{T}} \\
A^{\mathbf{T}} & 0 \\
\end{array}\right]
$$

Thus when written out explicitly:

$$ S =
\left[\begin{array}{cc}
0 & A \\
A & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & A^{\mathbf{T}} \\
A^{\mathbf{T}} & 0 \\
\end{array}\right] = S^{\mathbf{T}}
$$

So the only way for $S$ to be symmetric is for $A = A^{\mathbf{T}}$ (_i.e._ the
matrix $A$ must itself be symmetric), which is not automatically the case.

b. If $A$ and $B$ are symmetric then their product $AB$ is symmetric.

False. Not necessarily. Suppose $A$ and $B$ are symmetric, then
$A = A^{\mathbf{T}}$ and $B = B^{\mathbf{T}}$. Thus the product $AB$ is:

$$ AB = A^{\mathbf{T}}B^{\mathbf{T}} $$

But, for the product $AB$ to be symmetric, it must equal its transpose:

$$ AB = (AB)^{\mathbf{T}} $$

Recall that when "distributed", the transpose reverses the order of the given
matrices:

$$ AB = (AB)^{\mathbf{T}} = B^{\mathbf{T}}A^{\mathbf{T}} $$

And because matrices are not commutative, it follows that the following
inequality is potentially true:

$$ AB = A^{\mathbf{T}}B^{\mathbf{T}} \neq B^{\mathbf{T}}A^{\mathbf{T}} = (AB)^{\mathbf{T}} $$

This means that $AB$ is not necessarily symmetric if $A$ and $B$ are symmetric.
In order for this to be true, it would have to mean that:

$$ AB = BA $$

c. If $A$ is not symmetric then $A^{-1}$ is not symmetric.

Suppose not, that is suppose $A^{-1}$ is symmetric, but $A$ is not symmetric.

A contradiction to this supposition is to be derived.

By the definition of the transpose function on an inverse matrix, this means
that:

$$ (A^{-1})^{\mathbf{T}} = (A^{\mathbf{T}})^{-1} $$

Since $A^{-1}$ is symmetric, this means that:

$$ A^{-1} = (A^{-1})^{\mathbf{T}} = (A^{\mathbf{T}})^{-1} $$

$$ A^{-1} = (A^{\mathbf{T}})^{-1} $$

If we then take the inverse of both sides, we arrive at:

$$ (A^{-1})^{-1} = ((A^{\mathbf{T}})^{-1})^{-1} $$

$$ A = A^{\mathbf{T}} $$

Since $A = A^{\mathbf{T}}$, this means that $A$ is also symmetric, which
contradicts the supposition.

Thus the statement is true, that is:

If $A$ is not symmetric, then $A^{-1}$ is not symmetric.

d. When $A, B, C$ are symmetric, the transpose of $ABC$ is $CBA$.

Suppose $A, B, C$ are symmetric matrices.

It is to be shown that the transpose of $ABC$ is $CBA$, or equivalently, that
$(ABC)^{\mathbf{T}} = CBA$.

By the supposition, since $A, B, C$ are symmetric, it follows by the definition
of symmetric matrices that:

$$ A = A^{\mathbf{T}}, B = B^{\mathbf{T}}, C = C^{\mathbf{T}} $$

Consider that:

$$ (ABC)^{\mathbf{T}} = C^{\mathbf{T}}B^{\mathbf{T}}A^{\mathbf{T}} $$

and then, by substitution (from the supposition):

$$ (ABC)^{\mathbf{T}} = CBA $$

This is what was to be shown, and the given statement is true.

**Questions 8-15 are about permutation matrices.**

8. Why are there $n!$ permutation matrices of order $n$?

The $1$ in row 1 has $n$ choices, then the $1$ in row 2 has $n - 1$ choices and
so on, each choice multiplies on the previous, providing the classic
$(n)(n - 1) \cdots (1) = n!$ pattern.

9. If $P_1$ and $P_2$ are permutation matrices, so is $P_1P_2$. This still has
   the rows of $I$ in some order. Give examples with $P_1P_2 \neq P_2P_1$ and
   $P_3P_4 = P_4P_3$.

_Give examples with $P_1P_2 \neq P_2P_1$:_

Let $P_1$ and $P_2$ be defined as:

$$ P_1 =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_2 =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

Then:

$$ P_1P_2 =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

And:

$$ P_2P_1 =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right] \neq
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right] = P_1P_2
$$

_and $P_3P_4 = P_4P_3$:_

Let $P_3$ and $P_4$ be defined as follows:

$$ P_3 =
\left[\begin{array}{cccc}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_4 =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
$$

Notice that both $P$'s permute different rows.

Now:

$$ P_3P_4 =
\left[\begin{array}{cccc}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
$$

And:

$$ P_4P_3 =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cccc}
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{array}\right] = P_3P_4
$$

10. There are 12 "_even_" permutations of $(1, 2, 3, 4)$ with an _even number of
    exchanges_. Two of them are $(1, 2, 3, 4)$ with no exchanges and
    $(4, 3, 2, 1)$ with two exchanges. List the other ten. Instead 9f writing
    each 4 by 4 matrix, just order the numbers.

_Solution:_

In total (12, including the given two permutations):

$$
(1, 2, 3, 4) \\
(2, 1, 3, 4) \to (2, 3, 1, 4) \\
(2, 1, 3, 4) \to (2, 1, 4, 3) \\
(2, 1, 3, 4) \to (4, 1, 3, 2) \\
(3, 2, 1, 4) \to (3, 1, 2, 4) \\
(3, 2, 1, 4) \to (3, 2, 4, 1) \\
(3, 2, 1, 4) \to (4, 2, 1, 3) \\
(4, 2, 3, 1) \to (4, 3, 2, 1) \\
(1, 3, 2, 4) \to (1, 3, 4, 2) \\
(1, 3, 2, 4) \to (1, 4, 2, 3) \\
(1, 4, 3, 2) \to (2, 4, 3, 1) \\
(1, 4, 3, 2) \to (3, 4, 1, 2) \\
$$

11. Which permutation makes $PA$ upper triangular? Which permutations make
    $P_1AP_2$ lower triangular? Multiplying $A$ on the right by $P_2$ exchanges
    the ____ of $A$.

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 6 \\
1 & 2 & 3 \\
0 & 4 & 5 \\
\end{array}\right]
$$

_Solution:_

_Which permutation makes $PA$ upper triangular?:_

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

_Which permutations make $P_1AP_2$ lower triangular?:_

$$ P_1 =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ P_1A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 6 \\
1 & 2 & 3 \\
0 & 4 & 5 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 6 \\
0 & 4 & 5 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$$ P_1AP_2 =
\left[\begin{array}{ccc}
0 & 0 & 6 \\
0 & 4 & 5 \\
1 & 2 & 3 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
6 & 0 & 0 \\
5 & 4 & 0 \\
3 & 2 & 1 \\
\end{array}\right]
$$

_Multiplying $A$ on the right by $P_2$ exchanges the (?) of $A$:_

columns

12. Explain why the dot product of $x$ and $y$ equals the dot product $Px$ and
    $Py$. Then $(Px)^{\mathbf{T}}(Py) = x^{\mathbf{T}}y$ tells us that
    $P^{\mathbf{T}}P = I$ for any permutation. With $x = (1, 2, 3)$ and
    $y = (1, 4, 2)$ choose $P$ to show that $Px \cdot y$ is not always
    $x \cdot Py$.

_Solution:_

_Explain why the dot product of $x$ and $y$ equals the dot product $Px$ and
$Py$:_

Consider $x \cdot y = z$, since $Px$ simply reorders the entries in $x$ and $Py$
reorders the entries in $y$ in the same order that $P$ reordered $x$, it stands
to reason that the dot product, $Px \cdot Py$, would be the same as $x \cdot y$
as the summations during evaluation do not change (they are simply done in a
different order).

_With $x = (1, 2, 3)$ and $y = (1, 4, 2)$ choose $P$ to show that $Px \cdot y$
is not always $x \cdot Py$:_

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ Px =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\3\end{bmatrix} =
\begin{bmatrix}{}2\\3\\1\end{bmatrix}
$$

$$ Px \cdot y =
\begin{bmatrix}{}2\\3\\1\end{bmatrix}
\begin{bmatrix}{}1\\4\\2\end{bmatrix} = 16
$$

$$ Py =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\4\\2\end{bmatrix} =
\begin{bmatrix}{}4\\2\\1\end{bmatrix}
$$

$$ xPy =
\begin{bmatrix}{}1\\2\\3\end{bmatrix}
\begin{bmatrix}{}4\\2\\1\end{bmatrix} = 11 \neq 16 = Px \cdot y
$$

13.

a. Find a 3 by 3 permutation matrix with $P^3 = I$ (but not $P = I$).

$$ P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P^2 =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ P^3 = (P^2)P =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

b. Find a 4 by 4 permutation $\hat{P}$ with $\hat{P}^4 \neq I$.

$$ \hat{P} =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
\end{array}\right]
$$

$$ \hat{P}^2 =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
$$

$$ \hat{P}^4 = (\hat{P}^2)(\hat{P}^2) =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0\\
0 & 0 & 1 & 0\\
0 & 0 & 0 & 1\\
0 & 1 & 0 & 0\\
\end{array}\right] \neq I
$$

14. If $P$ has $1$'s on the antidiagonal form $(1, n)$ to $(n, 1)$, describe
    $PAP$. Note $P = P^{\mathbf{T}}$.

_Solution:_

$P$ swaps reverses the row order of $A$. Then $PAP$ reverses the column order of
$PA$, a complete reflection of the matrix (not the transpose of $A$).

15. All row exchange matrices are symmetric: $P^{\mathbf{T}} = P$. Then
    $P^{\mathbf{T}}P = I$ becomes $P^2 = I$. Other permutation matrices may or
    may not be symmetric.

a. If $P$ sends row 1 to row 4, then $P^{\mathbf{T}}$ sends row ____ to row
____. When $P^{\mathbf{T}} = P$ the row exchanges come in pairs with no overlap.

4 to row 1.

b. Find a 4 by 4 example with $P^{\mathbf{T}} = P$ that moves all four rows.

$$ P =
\left[\begin{array}{cccc}
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
\end{array}\right] = P^{\mathbf{T}}
$$

**Questions 16-21 are about symmetric matrices and their factorizations.**

16. If $A = A^{\mathbf{T}}$ and $B = B^{\mathbf{T}}$, which of these matrices
    are certainly symmetric?

a. $A^2 - B^2$

Consider:

$$ (A^2 - B^2)^{\mathbf{T}} = (A^2)^{\mathbf{T}} - (B^2)^{\mathbf{t}} = A^2 - B^2 $$

Since $A^2 - B^2 = (A^2 - B^2)^{\mathbf{T}}$, by the definition of symmetric
matrices, $A^2 - B^2$ is symmetric.

b. $(A + B)(A - B)$

$$ ((A + B)(A - B))^{\mathbf{T}} $$

$$ = (A - B)^{\mathbf{T}}(A + B)^{\mathbf{T}} $$

$$ = (A^{\mathbf{T}} - B^{\mathbf{T}})(A^{\mathbf{T}} + B^{\mathbf{T}}) $$

$$ = (A - B)(A + B) \neq (A + B)(A - B) $$

This inequality is true since matrix multiplication is not commutative. Thus
$(A + B)(A - B)$ cannot be determined to be symmetric.

c. $ABA$

$$ (ABA)^{\mathbf{T}} = A^{\mathbf{T}}B^{\mathbf{T}}A^{\mathbf{T}} $$

Note that the switching of the order of matrices still happened here, it just
turns out its the same order as the original.

$$ (ABA)^{\mathbf{T}} = ABA $$

Thus it can be concluded that $ABA$ is symmetric.

d. $ABAB$

$$ (ABAB)^{\mathbf{T}} = B^{\mathbf{T}}A^{\mathbf{T}}B^{\mathbf{T}}A^{\mathbf{T}} $$

$$ (ABAB)^{\mathbf{T}} = BABA \neq ABAB $$

Thus $ABAB$ cannot be determined to be symmetric.

17. Find 2 by 2 symmetric matrices $S = S^{\mathbf{T}}$ with these properties:

a. $S$ is not invertible.

$$ S =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
$$

Since $S$'s determinant is $0$.

b. $S$ is invertible but cannot be factored into $LU$ (row exchanges needed).

$$ S =
\left[\begin{array}{cc}
0 & 1 \\
1 & 1 \\
\end{array}\right]
$$

c. $S$ can be factored into $LDL^{\mathbf{T}}$ but not into $LL^{\mathbf{T}}$
(because of negative $D$).

$$ S =
\left[\begin{array}{cc}
1 & 1 \\
1 & 0 \\
\end{array}\right]
$$

Notice that after elimination we get a negative coefficient on the last pivot.

18.

a. How many entries of $S$ can be chosen independently, if $S = S^{\mathbf{T}}$
is 5 by 5?

$$ \binom{5}{2} + 5 = 15 $$

Where $\binom{5}{2}$ is the amount of entries in the lower triangular matrix
$L$, while $5$ are the entries along the diagonal matrix $D$.

b. How do $L$ and $D$ (still 5 by 5) give the same number of choices in
$LDL^{\mathbf{T}}$?

$L$ has 10, while $D$ has 5, giving a total of 15 choices in $LDL^{\mathbf{T}}$.

c. How many entries can be chosen if $A$ is _skew-symmetric_?
($A^{\mathbf{T}} = -A$).

If $A^{\mathbf{T}} = -A$, then $-A$ is symmetric, and the diagonal is all $0$'s
(since $a_{ij} = -a_{ij} \Rightarrow a_{ij} = 0$), forcing the amount of choices
to simply be the upper (or lower) triangular entries, meaning the amount of
choices is reduced to 10.

19. Suppose $A$ is rectangular ($m$ by $n$) and $S$ is symmetric ($m$ by $m$).

a. Transpose $A^{\mathbf{T}}SA$ to show its symmetry. What shape is this matrix?

$$ (A^{\mathbf{T}}SA)^{\mathbf{T}} = A^{\mathbf{T}}S^{\mathbf{T}}(A^{\mathbf{T}})^{\mathbf{T}} = A^{\mathbf{T}}SA $$

Since $A$ is $m \times n$, it's transpose, $A^{\mathbf{T}}$ is $n \times m$.
This leaves the dimensions of $A^{\mathbf{T}}S$ as $(n \times m)(m \times m)$
which means that $A^{\mathbf{T}}S$ is $n \times m$. Then $A^{\mathbf{T}}SA$ is
$(n \times m)(m \times n)$, meaning $A^{\mathbf{T}}SA$ is $n \times n$. This the
shape of this matrix.

b. Show why $A^{\mathbf{T}}A$ has no negative numbers on its diagonal.

$$ (A^{\mathbf{T}}A)_{jj} = (\text{column } j \text{ of } A) \cdot (\text{column } j \text{ of } A) \geq 0 $$

20. Factor these symmetric matrices into $S = LDL^{\mathbf{T}}$. The pivot
    matrix $D$ is diagonal:

$$ S =
\left[\begin{array}{cc}
1 & 3 \\
3 & 2 \\
\end{array}\right]
$$

and

$$ S =
\left[\begin{array}{cc}
1 & b \\
b & c \\
\end{array}\right]
$$

and

$$ S =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ S =
\left[\begin{array}{cc}
1 & 3 \\
3 & 2 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-3 & 1 \\
\end{array}\right]
$$

$$ E_{21}S =
\left[\begin{array}{cc}
1 & 0 \\
-3 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 3 \\
3 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 3 \\
0 & -7 \\
\end{array}\right] = U
$$

$$ L = E_{21}^{-1} =
\left[\begin{array}{cc}
1 & 0 \\
3 & 1 \\
\end{array}\right]
$$

$$ L^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 3 \\
0 & 1 \\
\end{array}\right]
$$

$$ D =
\left[\begin{array}{cc}
1 & 0 \\
0 & -7 \\
\end{array}\right]
$$

$$ DL^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
0 & -7 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 3 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 3 \\
0 & -7 \\
\end{array}\right] = U
$$

$$ LDL^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
3 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 3 \\
0 & -7 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 3 \\
3 & 2 \\
\end{array}\right] = S
$$

_Second:_

$$ S =
\left[\begin{array}{cc}
1 & b \\
b & c \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-b & 1 \\
\end{array}\right]
$$

$$ E_{21}S =
\left[\begin{array}{cc}
1 & 0 \\
-b & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
b & c \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & b \\
0 & c - b^2 \\
\end{array}\right] = U
$$

$$ L = E_{21}^{-1} =
\left[\begin{array}{cc}
1 & 0 \\
b & 1 \\
\end{array}\right]
$$

$$ L^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right]
$$

$$ D =
\left[\begin{array}{cc}
1 & 0 \\
0 & c - b^2 \\
\end{array}\right]
$$

$$ DL^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
0 & c - b^2 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & b \\
0 & c - b^2 \\
\end{array}\right] = U
$$

$$ LDL^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
b & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
0 & c - b^2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & b \\
b & c \\
\end{array}\right] = S
$$

_Third:_

$$ S =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}S =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
0 & \frac{3}{2} & -1 \\
0 & -1 & 2 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{2}{3} & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21}S  =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{2}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & -1 & 0 \\
0 & \frac{3}{2} & -1 \\
0 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
0 & \frac{3}{2} & -1 \\
0 & 0 & \frac{4}{3} \\
\end{array}\right] = U
$$

$$ L = E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right]
$$

$$ L^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & -\frac{1}{2} & 0 \\
0 & 1 & -\frac{2}{3} \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ D =
\left[\begin{array}{rrr}
2 & 0 & 0 \\
0 & \frac{3}{2} & 0 \\
0 & 0 & \frac{4}{3} \\
\end{array}\right]
$$

$$ DL^{\mathbf{T}} =
\left[\begin{array}{rrr}
2 & 0 & 0 \\
0 & \frac{3}{2} & 0 \\
0 & 0 & \frac{4}{3} \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & -\frac{1}{2} & 0 \\
0 & 1 & -\frac{2}{3} \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
0 & \frac{3}{2} & -1 \\
0 & 0 & \frac{4}{3} \\
\end{array}\right] = U
$$

$$ LDL^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & -1 & 0 \\
0 & \frac{3}{2} & -1 \\
0 & 0 & \frac{4}{3} \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right] = S
$$

21. After elimination clears out column 1 below the first pivot, find the
    symmetric 2 by 2 matrix that appears in the lower right corner:

Start from

$$ S =
\left[\begin{array}{ccc}
2 & 4 & 8 \\
4 & 3 & 9 \\
8 & 9 & 0 \\
\end{array}\right]
$$

and

$$ S =
\left[\begin{array}{ccc}
1 & b & c \\
b & d & e \\
c & e & f \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ S =
\left[\begin{array}{ccc}
2 & 4 & 8 \\
4 & 3 & 9 \\
8 & 9 & 0 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}S =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 4 & 8 \\
4 & 3 & 9 \\
8 & 9 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 4 & 8 \\
0 & -5 & -7 \\
8 & 9 & 0 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21}S =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-4 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 4 & 8 \\
0 & -5 & -7 \\
8 & 9 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 4 & 8 \\
0 & -5 & -7 \\
0 & -7 & -32 \\
\end{array}\right]
$$

Elimination has cleared out column 1 from the first pivot at this point, so the
symmetric 2 by 2 matrix that appears in the lower right corner is:

$$
\left[\begin{array}{rr}
-5 & -7 \\
-7 & -32 \\
\end{array}\right]
$$

_Second:_

$$ S =
\left[\begin{array}{ccc}
1 & b & c \\
b & d & e \\
c & e & f \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-b & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}S =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-b & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & b & c \\
b & d & e \\
c & e & f \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & b & c \\
0 & d - b^2 & e - bc \\
c & e & f \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-c & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21}S =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-c & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & b & c \\
0 & d - b^2 & e - bc \\
c & e & f \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & b & c \\
0 & d - b^2 & e - bc \\
0 & e - bc & f - c^2 \\
\end{array}\right]
$$

So our symmetric 2 by 2 matrix that appears in the lower right corner is:

$$
\left[\begin{array}{cc}
d - b^2 & e - bc \\
e - bc & f - c^2 \\
\end{array}\right]
$$

**Questions 22-24 are about the factorizations $PA = LU$ and $A = L_1P_1U_1$.

22. Find the $PA = LU$ factorizations (and check them) for

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
2 & 3 & 4 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 0 \\
2 & 4 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
2 & 3 & 4 \\
\end{array}\right]
$$

$$ P_{13} =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P_{13}A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
2 & 3 & 4 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 3 & 4 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}P_{13}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 3 & 4 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 3 & 4 \\
0 & -\frac{3}{2} & -1 \\
0 & 1 & 1 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{2}{3} & 1 \\
\end{array}\right]
$$

$$ E_{32}E_{21}P_{13}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{2}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 3 & 4 \\
0 & -\frac{3}{2} & -1 \\
0 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 3 & 4 \\
0 & -\frac{3}{2} & -1 \\
0 & 0 & \frac{1}{3} \\
\end{array}\right] = U
$$

$$ L = E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right]
$$

$$ LU =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & -\frac{2}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 3 & 4 \\
0 & -\frac{3}{2} & -1 \\
0 & 0 & \frac{1}{3} \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 3 & 4 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right] = P_{13}A
$$

_Second:_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 0 \\
2 & 4 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

$$ P_{12} =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_{12}A =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 0 \\
2 & 4 & 1 \\
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 4 & 1 \\
1 & 2 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
$$

$$ P_{23} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ P_{23}P_{12}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 4 & 1 \\
1 & 2 & 0 \\
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 4 & 1 \\
1 & 1 & 1 \\
1 & 2 & 0 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}P_{23}P_{12}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 4 & 1 \\
1 & 1 & 1 \\
1 & 2 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 4 & 1 \\
0 & -1 & \frac{1}{2} \\
1 & 2 & 0 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-\frac{1}{2} & 0 & 1 \\
\end{array}\right]
$$

$$ E_{31}E_{21}P_{23}P_{12}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-\frac{1}{2} & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 4 & 1 \\
0 & -1 & \frac{1}{2} \\
1 & 2 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 4 & 1 \\
0 & -1 & \frac{1}{2} \\
0 & 0 & -\frac{1}{2} \\
\end{array}\right] = U
$$

$$ L = E_{21}^{-1}E_{31}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
\frac{1}{2} & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
\frac{1}{2} & 0 & 1 \\
\end{array}\right]
$$

$$ LU =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
\frac{1}{2} & 1 & 0 \\
\frac{1}{2} & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 4 & 1 \\
0 & -1 & \frac{1}{2} \\
0 & 0 & -\frac{1}{2} \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 4 & 1 \\
1 & 1 & 1 \\
1 & 2 & 0 \\
\end{array}\right] = P_{23}P_{12}A
$$

23. Find a 4 by 4 permutation matrix (call it $A$) that needs 3 row exchanges to
    reach the end of elimination. For this matrix, what are its factors $P, L$,
    and $U$?

_Solution:_

$$ A =
\left[\begin{array}{cccc}
0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right] = P
$$

$$ L = U = I $$

24. Factor the following matrix into $PA = LU$. Factor it also into
    $A = L_1P_1U_1$ (hold the exchange of row 3 until 3 times row 1 is
    subtracted from row 2):

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right]
$$

_Solution:_

_Factor the following matrix into $PA = LU$:_

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right]
$$

$$ P_{13} =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P_{13}A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 1 \\
0 & 3 & 8 \\
0 & 1 & 2 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -\frac{1}{3} & 1 \\
\end{array}\right]
$$

$$ E_{32}P_{13}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -\frac{1}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 1 \\
0 & 3 & 8 \\
0 & 1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 3 & 8 \\
0 & 0 & -\frac{2}{3} \\
\end{array}\right] = U
$$

$$ L = E_{32}^{-1} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{1}{3} & 1 \\
\end{array}\right]
$$

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & \frac{1}{3} & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 3 & 8 \\
0 & 0 & -\frac{2}{3} \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 3 & 8 \\
0 & 1 & 2 \\
\end{array}\right] = P_{13}A
$$

_Factor it also into $A = L_1P_1U_1$:_

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}A =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
0 & 1 & 2 \\
0 & 0 & 2 \\
2 & 1 & 1 \\
\end{array}\right]
$$

$$ P_{13} =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P_{13}E_{21}A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
0 & 1 & 2 \\
0 & 0 & 2 \\
2 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 0 & 2 \\
0 & 1 & 2 \\
\end{array}\right]
$$

$$ P_{23} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ P_{23}P_{13}E_{21}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 0 & 2 \\
0 & 1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 1 & 2 \\
0 & 0 & 2 \\
\end{array}\right] = U = U_1
$$

$$ L_1 = E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_1 = P_{13}P_{23} =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P_1U_1 =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
2 & 1 & 1 \\
0 & 1 & 2 \\
0 & 0 & 2 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 0 & 2 \\
2 & 1 & 1 \\
\end{array}\right]
$$

$$ L_1P_1U_1 =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 0 & 2 \\
2 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 3 & 8 \\
2 & 1 & 1 \\
\end{array}\right] = A
$$

25. Prove that the identity matrix cannot be the product of three row exchanges
    (or five). It can be the product of two exchanges (or four).

**Proof:**

It is to be shown that the identity matrix $I$ cannot be the product of an odd
number of row exchanges, but can be the product of an even number of exchanges.

Recall that each row exchange multiplies the determinant of a matrix by $-1$.
This follows from the properties of the determinant: swapping any two rows
negates it.

The determinant of the identity matrix is $\det(I) = 1$.

Suppose we apply $k$ row exchanges to $I$, starting from $I$ itself (which has
determinant $1$). Each exchange multiplies the determinant by $-1$, so after $k$
exchanges the determinant is $(-1)^k$.

For the result to equal $I$, the determinant must equal $1$, so we need:

$$ (-1)^k = 1 $$

This holds if and only if $k$ is even.

Therefore, the product of an odd number of row exchanges ($k = 1, 3, 5, \dots$)
gives determinant $-1 \neq 1$, and so cannot equal $I$. The product of an even
number ($k = 2, 4, \dots$) gives determinant $1$, consistent with equaling $I$.

Q.E.D.

26.

a. Choose $E_{21}$ to remove the $3$ below the first pivot. Then multiply
$E_{21}SE_{21}^{\mathbf{T}}$ to remove both $3$'s:

$$ S =
\left[\begin{array}{rrr}
1 & 3 & 0 \\
3 & 11 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
$$

is going toward

$$ D =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

_Choose $E_{21}$ to remove the $3$ below the first pivot:_

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

_Then multiply $E_{21}SE_{21}^{\mathbf{T}}$ to remove both $3$'s:_

$$ E_{21}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & -3 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ SE_{21}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 3 & 0 \\
3 & 11 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & -3 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 2 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
$$

$$ E_{21}SE_{21}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 2 & 4 \\
0 & 4 & 9 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 2 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
$$

b. Choose $E_{32}$ to remove the $4$ below the second pivot. Then $S$ is reduced
to $D$ by $E_{32}E_{21}SE_{21}^{\mathbf{T}}E_{32}^{\mathbf{T}} = D$. Invert the
$E$'s to find $L$ in $S = LDL^{\mathbf{T}}$.

_Solution:_

_Choose $E_{32}$ to remove the $4$ below the second pivot:_

$$ E_{21}SE_{21}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 2 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
$$

$$ E_{32} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
$$

_Then $S$ is reduced to $D$ by
$E_{32}E_{21}SE_{21}^{\mathbf{T}}E_{32}^{\mathbf{T}} = D$:_

$$ E_{32}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & -2 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ E_{21}SE_{21}^{\mathbf{T}}E_{32}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 2 & 4 \\
0 & 4 & 9 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & -2 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 4 & 9 \\
\end{array}\right]
$$

$$ E_{32}E_{21}SE_{21}^{\mathbf{T}}E_{32}^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 4 & 9 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 9 \\
\end{array}\right] = D \text{?}
$$

_Invert the $E$'s to find $L$ in $S = LDL^{\mathbf{T}}$:_

$$ L = E_{21}^{-1}E_{32}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right]
$$

$$ L^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 3 & 0 \\
0 & 1 & 2 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ DL^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 3 & 0 \\
0 & 1 & 2 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 3 & 0 \\
0 & 2 & 4 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ LDL^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
3 & 1 & 0 \\
0 & 2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 3 & 0 \\
0 & 2 & 4 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 3 & 0 \\
3 & 11 & 4 \\
0 & 4 & 9 \\
\end{array}\right] = S
$$

27. If every row of a 4 by 4 matrix contains the numbers $0, 1, 2, 3$ in some
    order, can the matrix be symmetric?

_Solution:_

$$ A =
\left[\begin{array}{cccc}
0 & 1 & 2 & 3 \\
1 & 2 & 3 & 0 \\
2 & 3 & 0 & 1 \\
3 & 0 & 1 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}} =
\left[\begin{array}{cccc}
0 & 1 & 2 & 3 \\
1 & 2 & 3 & 0 \\
2 & 3 & 0 & 1 \\
3 & 0 & 1 & 2 \\
\end{array}\right] = A
$$

28. Prove that no reordering of rows and reordering of columns can transpose a
    typical matrix. (Watch the diagonal entries.)

Omitted.

**The next three questions are about applications of the identity
$(Ax)^{\mathbf{T}}y = x^{\mathbf{T}}(A^{\mathbf{T}}y)$.**

29. Wires go between Boston, Chicago, and Seattle. Those cities are at voltages
    $x_B, x_C, x_S$. With unit resistances between cities, the currents between
    cities are in $y$:

$$ y = Ax $$

is

$$ \begin{bmatrix}{}y_{BC}\\y_{CS}\\y_{BS}\end{bmatrix} =
\left[\begin{array}{rrr}
1 & -1 & 0 \\
0 & 1 & -1 \\
1 & 0 & -1 \\
\end{array}\right]
\begin{bmatrix}{}x_B\\x_C\\x_S\end{bmatrix}
$$

a. Find the total currents $A^{\mathbf{T}}y$ out of the three cities.

_Solution:_

$$ A^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 0 & 1 \\
-1 & 1 & 0 \\
0 & -1 & -1 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}y =
\left[\begin{array}{rrr}
1 & 0 & 1 \\
-1 & 1 & 0 \\
0 & -1 & -1 \\
\end{array}\right]
\begin{bmatrix}{}y_{BC}\\y_{CS}\\y_{BS}\end{bmatrix} =
\begin{bmatrix}{}y_{BC} + y_{BS}\\y_{CS} - y_{BC}\\-y_{CS} - y_{BS}\end{bmatrix}
$$

b. Verify that $(Ax)^{\mathbf{T}}y$ agrees with
$x^{\mathbf{T}}(A^{\mathbf{T}}y)$ - six terms in both.

$$ Ax =
\left[\begin{array}{rrr}
1 & -1 & 0 \\
0 & 1 & -1 \\
1 & 0 & -1 \\
\end{array}\right]
\begin{bmatrix}{}x_B\\x_C\\x_S\end{bmatrix} =
\begin{bmatrix}{}x_B -x_C\\x_C - x_S\\x_B - x_S\end{bmatrix}
$$

$$ (Ax)^{\mathbf{T}} =
\left[\begin{array}{ccc}
x_B - x_C & x_C - x_S & x_B - x_S \\
\end{array}\right]
$$

$$ (Ax)^{\mathbf{T}}y =
\left[\begin{array}{ccc}
x_B - x_C & x_C - x_S & x_B - x_S \\
\end{array}\right]
\begin{bmatrix}{}y_{BC}\\y_{CS}\\y_{BS}\end{bmatrix} =  (x_B - x_C)(y_{BC}) + (x_C - x_S)(y_{CS}) + (x_B - x_S)(y_{BS})
$$

$$ = x_By_{BC} - x_Cy_{BC} + x_Cy_{CS} - x_Sy_{CS} + x_By_{BS} - x_Sy_{BS} $$

$$ x^{\mathbf{T}} =
\left[\begin{array}{ccc}
x_B & x_C & x_S \\
\end{array}\right]
$$

$$ x^{\mathbf{T}}(A^{T}y) =
\left[\begin{array}{ccc}
x_B & x_C & x_S \\
\end{array}\right]
\begin{bmatrix}{}y_{BC} + y_{BS}\\y_{CS} - y_{BC}\\-y_{CS} - y_{BS}\end{bmatrix} =
x_B(y_{BC} + y_{BS}) + x_C(y_{CS} - y_{BC}) + x_S(-y_{CS} - y_{BS})
$$

$$ = x_By_{BC} + x_By_{BS} + x_Cy_{CS} - x_Cy_{BC} - x_Sy_{CS} - x_Sy_{BS} $$

Careful inspection shows that these are the same six terms.

30. Producing $x_1$ trucks and $x_2$ planes needs $x_1 + 50x_2$ tons of steel,
    $40x_1 + 1000x_2$ pounds of rubber, and $2x_1 + 50x_2$ months of labor. If
    the unit costs $y_1, y_2, y_3$ are $700 per ton, $3 per pound, and $3000 per
    month, what are the values of one truck and one plane? Those are the
    components of $A^{\mathbf{T}}y$.

_Solution:_

Let $A$ be the matrix representing the resources necessary:

$$ A =
\left[\begin{array}{cc}
1 & 50 \\
40 & 1000 \\
2 & 50 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 40 & 2 \\
50 & 1000 & 50 \\
\end{array}\right]
$$

Now, let $y$ be a vector that represents that costs, where $y_1$ represents the
costs per ton of steel, $y_2$ represents the costs per pound of rubber, and
$y_3$ represents the costs per month of labor.

$$ y =
\begin{bmatrix}{}700\\3\\3000\end{bmatrix}
$$

The aim is to find the value of one truck and one plane. Strang gives us the
formula for finding it as $A^{\mathbf{T}}y$, let's see what happens:

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 40 & 2 \\
50 & 1000 & 50 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}y =
\left[\begin{array}{ccc}
1 & 40 & 2 \\
50 & 1000 & 50 \\
\end{array}\right]
\begin{bmatrix}{}700\\3\\3000\end{bmatrix} =
\begin{bmatrix}{}6820\\188000\end{bmatrix}
$$

Presumably, the cost for a single truck is $6,820. The cost for a single plane
is $188,000.

31. $Ax$ gives the amount of steel, rubber, and labor to produce $x$ in
    Problem 31. Find $A$. Then $Ax \cdot y$ is the ____ of inputs while
    $x \cdot A^{\mathbf{T}}y$ is the value of ____.

_Solution:_

_Find $A$:_

$$ A =
\left[\begin{array}{cc}
1 & 50 \\
40 & 1000 \\
2 & 50 \\
\end{array}\right]
$$

_Then $Ax \cdot y$ is the (?) of inputs:_

cost

_while $x \cdot A^{\mathbf{T}}y$ is the value of (?):_

outputs/units produced (_cost_ of total units produced)

32. The matrix $P$ that multiplies $(x, y, z)$ to give $(z, x, y)$ is also a
    rotation matrix. Find $P$ and $P^3$. The rotation axis $a = (1, 1, 1)$
    doesn't move, it equals $Pa$. What is the angle of rotation from
    $v = (2, 3, -5)$ to $Pv = (-5, 2, 3)$?

_Solution:_

_Find $P$ and $P^3$:_

$$ P =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ Px =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}z\\x\\y\end{bmatrix}
$$

$$ P^2 =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ P^3 = (P^2)P =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
1 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

_What is the angle of rotation from $v = (2, 3, -5)$ to $Pv = (-5, 2, 3)$?:_

Thinking on this, if $P^3 = I$, this means that after $P^3$ is applied to the
given vector, it returns that vector to its original position, _i.e._
$360\degree$. However, since we are applying $P$, not $P^3$, it stands to reason
that $P$ rotates the given vector $\dfrac{360}{3}\degree = 120\degree$.

33. Write $A = \left[\begin{array}{cc}1 & 2 \\4 & 9 \\\end{array}\right]$ as the
    product $ES$ of an elementary row operation matrix $E$ and a symmetric
    matrix $S$.

_Solution:_

An elementary matrix is an elimination matrix, but in this case the resulting
$U$ must be symmetric. To do so, we must choose an $E$ such that it results in a
symmetric $U$. Considering our simple $A$, we can simply try to get a $2$ in the
$A_{21}$ position, since $A_{12} = 2$.

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
4 & 9 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
$$

$$ E_{21}A =
\left[\begin{array}{cc}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
4 & 9 \\
\end{array}\right] =
\left[\begin{array}{rr}
1 & 2 \\
2 & 5 \\
\end{array}\right] = U
$$

There, now our $U$ is symmetric. We are now tasked as expressing this as
$A = ES$. Since $U$ is symmetric, simply let $S = U$ and since $E_{21}$ has
accomplished the goal of only eliminating enough to get $S$ after $AE$ has been
computed, let us say that $E = E_{21}^{-1}$:

$$ E_{21}^{-1} =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right] = E
$$

$$ ES =
\left[\begin{array}{cc}
1 & 0 \\
2 & 1 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & 2 \\
2 & 5 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
4 & 9 \\
\end{array}\right] = A
$$

This is what was to be shown.

34. Here is a new factorization of A$ into $LS$: _triangular_ (with $1$'s)
    _times symmetric_:

Start from $A = LDU$. Then $A$ equals $L(U^{\mathbf{T}})^{-1}$ times
$S = U^{\mathbf{T}}DU$.

Why is $L(U^{\mathbf{T}})^{-1}$ triangular? Its diagonal is all $1$'s. Why is
$U^{\mathbf{T}}DU$ symmetric?

Omitted.

35. A _group_ of matrices includes $AB$ and $A^{-1}$ if it includes $A$ and $B$.
    "Products and inverses stay in the group." Which of these sets are groups?

Lower triangular matrices $L$ with $1$'s on the diagonal, symmetric matrices
$S$, positive matrices $M$, diagonal invertible matrices $D$, permutation
matrices $P$, matrices with $Q^{\mathbf{T}} = Q^{-1}$. _Invent two more matrix
groups._

Omitted.
