Page 19

## Problem Set 1.1

**Problems 1-9 are about addition of vectors and linear combination.**

1. Describe geometrically (line, plane, or all of $\mathbf{R}^3$) all linear
   combinations of

a. $\begin{bmatrix}{}1\\2\\3\end{bmatrix}$ and
$\begin{bmatrix}{}3\\6\\9\end{bmatrix}$

b. $\begin{bmatrix}{}1\\0\\0\end{bmatrix}$ and
$\begin{bmatrix}{}0\\2\\3\end{bmatrix}$

c. $\begin{bmatrix}{}2\\0\\0\end{bmatrix}$ and
$\begin{bmatrix}{}0\\2\\2\end{bmatrix}$ and
$\begin{bmatrix}{}2\\2\\3\end{bmatrix}$

a. A line of $\mathbf{R}^3$.

Notice that the second vector is just $3$ times the first.

Let $v$ be the first vector and $w$ be the second vector:

$$ v \text{ and } w $$

Which is really just:

$$ v \text{ and } 3v $$

In essence, this is the same line, just $w$ is 3 times as long as $v$.

b. A plane of $\mathbf{R}^3$.

Notice that these two vectors point in two independent directions (regardless of
multiples $c$ and $d$), this creates a plane. A plane is essentially a 2D axes
in $\mathbf{R}^3$. (through the origin in this case).

c. All of $R^{3}$

Notice that the first two vectors point in two different directions (a plane).
The third vector then could then result in this linear combination remaining on
the established plane if it was a multiple of either the first ($c$) vector or
the second ($d$) vector (or a multiple of the sum of multiples of the first and
second, _i.e._ $c + d$).

This is not the case, however, all three vectors point in different directions,
and thus this linear combination spans all of $\mathbf{R}^3$.

2. Draw $v = \begin{bmatrix}{}4\\1\end{bmatrix}$ and
   $w = \begin{bmatrix}{}-2\\2\end{bmatrix}$ and $v + w$ and $v - w$ in a single
   $xy$ plane.

(Done by hand.)

3. If $v + w = \begin{bmatrix}{}5\\1\end{bmatrix}$ and
   $v - w = \begin{bmatrix}{}1\\5\end{bmatrix}$, compute and draw the vectors
   $v$ and $w$.

Since $v + w = \begin{bmatrix}{}5\\1\end{bmatrix}$ and
$v - w = \begin{bmatrix}{}1\\5\end{bmatrix}$, this means that $v$ and $w$ can be
expressed as:

$$ v = \begin{bmatrix}{}v_1\\v_2\end{bmatrix}, w = \begin{bmatrix}{}w_1\\w_2\end{bmatrix} $$

Thus:

$$ v + w = \begin{bmatrix}{}v_1\\v_2\end{bmatrix} + \begin{bmatrix}{}w_1\\w_2\end{bmatrix} = \begin{bmatrix}{}5\\1\end{bmatrix} $$

and:

$$ v - w = \begin{bmatrix}{}v_1\\v_2\end{bmatrix} - \begin{bmatrix}{}w_1\\w_2\end{bmatrix} = \begin{bmatrix}{}1\\5\end{bmatrix} $$

So we have:

$$ v_1 + w_1 = 5, v_1 - w_1 = 1 $$

and:

$$ v_2 + w_2 = 1, v_2 - w_2 = 5 $$

Solving for $v_1, w_1$:

$$ v_1 + w_1 = 5, v_1 - w_1 = 1 $$

$$ v_1 - w_1 = 1 \Rightarrow v_1 = w_1 + 1 $$

By substitution:

$$ v_1 + w_1 = (w_1 + 1) + w_1 = 5 $$

$$ 2w_1 + 1 = 5 $$

$$ 2w_1 = 4 $$

$$ w_1 = 2 $$

Again, substitution again:

$$ v_1 + w_1 = 5 $$

$$ v_1 + 2 = 5 $$

$$ v_1 = 3 $$

Now solving for $v_2, w_2$:

$$ v_2 + w_2 = 1, v_2 - w_2 = 5 $$

$$ v_2 - w_2 = 5 $$

$$ v_2 = w_2 + 5 $$

substitution:

$$ v_2 + w_2 = 1 $$

$$ (w_2 + 5) + w_2 = 1 $$

$$ 2w_2 + 5 = 1 $$

$$ 2w_2 = -4 $$

$$ w_2 = -2 $$

substitution:

$$ v_2 + w_2 = 1 $$

$$ v_2 + (-2) = 1 $$

$$ v_2 - 2 = 1 $$

$$ v_2 = 3 $$

Thus:

$$ v = \begin{bmatrix}{}3\\3\end{bmatrix}, w = \begin{bmatrix}{}2\\-2\end{bmatrix} $$

(Drawing omitted.)

4. From $v = \begin{bmatrix}{}2\\1\end{bmatrix}$ and
   $w = \begin{bmatrix}{}1\\2\end{bmatrix}$, find the components of $3v + w$ and
   $cv + dw$.

$$ 3v + w = 3\begin{bmatrix}{}2\\1\end{bmatrix} + \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = \begin{bmatrix}{}6\\3\end{bmatrix} + \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = \begin{bmatrix}{}7\\5\end{bmatrix}$$

Thus the components of $3v + w$, denoted $(3v + w)_1, (3v + w)_2$ are:

$$ (3v + w)_1 = 7, (3v + w)_2 = 5 $$

Now for the components of $cv + dw$:

$$ cv + dw = c\begin{bmatrix}{}2\\1\end{bmatrix} + d\begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = \begin{bmatrix}{}2c\\c\end{bmatrix} + \begin{bmatrix}{}d\\2d\end{bmatrix} $$

$$ = \begin{bmatrix}{}2c + d\\c + 2d\end{bmatrix} $$

Thus the components of $cv + dw$ are $2c + d$ and $c + 2d$.

5. Compute $u + v + w$ and $2u + 2v + w$. How do you know $u, v, w$ lie in a
   plane?

These lie in a plane because $w = cu + dv$. Find $c$ and $d$

$$ u = \begin{bmatrix}{}1\\2\\3\end{bmatrix}, v = \begin{bmatrix}{}-3\\1\\-2\end{bmatrix}, w = \begin{bmatrix}{}2\\-3\\-1\end{bmatrix} $$

Computing for $c$ and $d$:

$$ cu + dv = c\begin{bmatrix}{}1\\2\\3\end{bmatrix} + d\begin{bmatrix}{}-3\\1\\-2\end{bmatrix} = \begin{bmatrix}{}2\\-3\\-1\end{bmatrix} $$

This results in the three equations:

$$ c - 3d = 2 $$

$$ 2c + d = -3 $$

$$ 3c - 2d = -1 $$

Solving for $c$ and $d$ just using the first two of the equations:

$$ c - 3d = 2 $$

$$ c = 2 + 3d $$

Substitution:

$$ 2c + d = -3 $$

$$ 2(2 + 3d) + d = -3 $$

$$ 4 + 6d + d = -3 $$

$$ 4 + 7d = -3 $$

$$ 7d = -7 $$

$$ d = -1 $$

Solving for $c$:

$$ c - 3d = 2 $$

$$ c - 3(-1) = 2 $$

$$ c + 3 = 2 $$

$$ c = -1 $$

Verifying $c = -1, d = -1$ in third equation:

$$ 3c - 2d = -1 $$

$$ 3(-1) - 2(-1) = -1 $$

$$ -3 - (-2) = -1 $$

$$ -3 + 2 = -1 $$

$$ -1 = -1 $$

Verified. Thus $c$ and $d$ have been found:

$$ c = -1, d = -1 $$

6. Every combination of $v = (1, -2, 1)$ and $w = (0, 1, -1)$ has components
   that add to ____. Find $c$ and $d$ so that $cv + dw = (3, 3, -6)$. Why is
   $(3, 3, 6)$ impossible?

add to $0$.

This is shown by calculating the sum of $cv + dw$:

$$ cv + dw = c\begin{bmatrix}{}1\\-2\\1\end{bmatrix} + d\begin{bmatrix}{}0\\1\\-1\end{bmatrix} $$

$$ = \begin{bmatrix}{}c\\-2c + d\\c - d\end{bmatrix} $$

Then add these three components together to get:

$$ c + (-2c + d) + (c - d) = -c + d + (c - d) = -c + c + d - d = 0 $$

Now, to find $cv + dw = (3, 3, -6)$:

$$ cv + dw = \begin{bmatrix}{}3\\3\\-6\end{bmatrix} $$

$$ c\begin{bmatrix}{}1\\-2\\1\end{bmatrix} + d\begin{bmatrix}{}0\\1\\-1\end{bmatrix} = \begin{bmatrix}{}3\\3\\-6\end{bmatrix} $$

$$ = \begin{bmatrix}{}c\\-2c + d\\c - d\end{bmatrix} = \begin{bmatrix}{}3\\3\\-6\end{bmatrix} $$

$$ c = 3 $$

$$ -2c + d = 3 $$

$$ c - d = -6 $$

Solving:

$$ -2c + d = 3 $$

$$ -2(3) + d = 3 $$

$$ -6 + d = 3 $$

$$ d = 9 $$

Confirming 3<sup>rd</sup> equation:

$$ c - d \stackrel{?}{=} -6 $$

$$ 3 - 9 \stackrel{?}{=} -6 $$

$$ -6 = -6 $$

Why is $(3, 3, 6)$ impossible?

The first two components are fine, as was just previously shown, however, in the
confirmation phase, this would change to:

$$ c - d = 6 $$

Since we used the same first two components to solve for $c$ and $d$, we know
that $c = 3$ and $d = 9$, so, by substitution:

$$ 3 - 9 \stackre{?}{=} 6 $$

$$ -6 \neq 6 $$

It follows that since $-6 \neq 6$, that $cv + dw \neq (3, 3, 6)$.

More simply, one could note that since the components add to $0$, that since
$3 + 3 + 6 = 12 \neq 0$, that $(3, 3, 6)$ is an impossible solution to
$cv + dw$.

7. In the $xy$ plane mark all nine of these linear combinations:

$$ c\begin{bmatrix}{}2\\1\end{bmatrix} + d\begin{bmatrix}{}0\\1\end{bmatrix} \text{ with } c = 0, 1, 2 \text{ and } d = 0, 1, 2 $$

(Done by hand.)

8. The parallelogram in Figure 1.1 has diagonal $v + w$. What is its other
   diagonal? What is the sum of the two diagonals? Draw that vector sum.

(see page 14 for Figure 1.1)

The other diagonal in Figure 1.1 is $v - w$.

The sum of the two diagonals is $(v + w) + (v - w) = 2v$

In the given example, $v = \begin{bmatrix}{}4\\2\end{bmatrix}$, so:

$$ (v + w) + (v - w) = 2v = 2\begin{bmatrix}{}4\\2\end{bmatrix} = \begin{bmatrix}{}8\\4\end{bmatrix} $$

Graph done by hand, but notice that $(v + w) + (v - w) = 2v$ lies _inbetween_
$v + w$ and $v - w$. This indicates that $v + w$ and $v - w$ _bisect_ one
another.

This demonstrates that the diagonals of any two parallelograms bisect each
other, a fundamental property of geometry.

9. If three corners of a parallelogram are $(1, 1)$, $(4, 2)$, and $(1, 3)$,
   what are all three of the possible fourth corners? Draw two of them.

The three possible fourth corners are $(4, 4), (-3, 2), (4, 0)$. Notice that we
find these by matching midpoints.

**Problems 10-14 are about special vectors on cubes and clocks in Figure 1.4.**

(See page 20 for Figure 1.4)

10. Which point of the cube is $i + j$? Which point is the vector sum of
    $i = (1, 0, 0)$ and $j = (0, 1, 0)$ and $k = (0, 0, 1)$? Describe all points
    $(x, y, z)$ in the cube.

$$ i + j = \begin{bmatrix}{}1\\0\\0\end{bmatrix} + \begin{bmatrix}{}0\\1\\0\end{bmatrix} $$

$$ = \begin{bmatrix}{}1\\1\\0\end{bmatrix} $$

Notice on Figure 1.4 that $i + j$ is the corner towards the bottom right.

Now, $i + j + k$:

$$ i + j + k = \begin{bmatrix}{}1\\0\\0\end{bmatrix} + \begin{bmatrix}{}0\\1\\0\end{bmatrix} + \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}1 + 0 + 0\\0 + 1 + 0\\0 + 0 + 1\end{bmatrix} $$

$$ = \begin{bmatrix}{}1\\1\\1\end{bmatrix} $$

Notice in Figure 1.4 that this is the right point of the cube just above $j$.

Describing all points $(x, y, z)$ in the cube:

$i + j = (1, 1, 0)$ is the base ($x$-$y$ plane). $i + j + k = (1, 1, 1)$ is the
opposite corner from $(0, 0, 0)$. Points in the cube have
$0 \leq x \leq 1, 0 \leq y \leq 1, 0 \leq z \leq 1$.

From the note on the Figure 1.4 "Notice the illusion...", the reason we can now
tell which is the top or the bottom ($(1, 1, 1)$ or $(0, 0, 0)$) is because of
our above analysis. We can now say that $(0, 0, 0)$ is the bottom corner and
that $(1, 1, 1)$ is the top, since we traveled along the $x$, $y$, $z$ axes
respectively away from the origin (_i.e._ $(0, 0, 0)$).

11. Four corners of this unit cube are
    $(0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1)$. What are the other four
    corners? Find the coordinates of the center point of the cube. The center
    points of the six faces are ____. The cube has how many edges?

Remaining four corners are:

$$ (1, 1, 0), (1, 0, 1), (1, 1, 1), (0, 1, 1) $$

The coordinates of the center point of the cube:

$$ \left(\frac{1}{2}, \frac{1}{2}, \frac{1}{2}\right) $$

The center point of the six faces are:

$$ \left(\frac{1}{2}, \frac{1}{2}, 0\right), \left(\frac{1}{2}, \frac{1}{2}, 1\right), \left(0, \frac{1}{2}, \frac{1}{2}\right), \left(1, \frac{1}{2}, \frac{1}{2}\right), \left(\frac{1}{2}, 0, \frac{1}{2}\right), \left(\frac{1}{2}, 1, \frac{1}{2}\right) $$

The cube has 12 edges.

12. _Review Question_. In $xyz$ space, where is the plane of all linear
    combinations of $i = (1, 0, 0)$ and $i + j = (1, 1, 0)$?

Notice that since $i + j = (1, 1, 0)$ that since $i = (1, 0, 0)$, this means
that $j = (0, 1, 0)$. Neither $i$ nor $j$ occupy the $z$ axes, and thus it can
be said that the plane of all linear combinations of $i$ and $i + j$ span the
$xy$ plane. This is because $z = 0$ in both $i$ and $j$, and thus $i + j$ forces
$z = 0$.

13.

(See page 20 for Figure 1.4)

a. What is the sum $V$ of the twelve vectors that go from the center of a clock
to the hours 1:00, 2:00, $\dots$, 12:00?

Since all the vectors in Figure 1.4 have an equidistant length and lie along
opposing angles of another vector, the sum of the vectors must be the zero
vector, $\mathbf{0}$.

b. If the 2:00 vector is removed, why do the 11 remaining vectors add to 8:00?

Since the 2:00 vector has been removed, it stands by part (a) that only the
remaining vectors add to $\mathbf{0} - \text{the coordinate values of 2:00}$,
and thus only the remaining vector must be the vector that points to 8:00 (the
opposite vector of 2:00).

This can be expressed algebraically as:

$$ V - v_{\text{2:00}} = \mathbf{0} - v_{\text{2:00}} = -v_{\text{2:00}} = v_{\text{8:00}} $$

c. What are the $x, y$ components of that 2:00 vector
$v = (\cos\theta, \sin\theta)$?

Since a clock is a circle, it has $360\degree$, each hour moves the long hand by
$\dfrac{360}{12} = 30\degree = \dfrac{\pi}{6} \text{radians}$.

Starting from 12:00 on a standard clockface, we start at
$90\degree = \dfrac{\pi}{2}$ radians. We then travel 2 hours, which, as
established is
$2\left(\frac{\pi}{6}\right) = \dfrac{\pi}{3} \text{ radians } = 60\degree$.

$$ 90\degree - 60\degree = 30\degree = \frac{\pi}{6} \text{ radians} $$

Thus our angle of interest for $\theta$ is:

$$ \theta = \frac{\pi}{6} $$

And thus:

$$ v = (\cos\theta, \sin\theta) $$

$$ = \left(\cos\left(\frac{\pi}{6}\right), \sin\left(\frac{\pi}{6}\right)\right) $$

$$ = \left(\frac{\sqrt{3}}{2}, \frac{1}{2}\right) $$

14. Suppose the twelve vectors start from 6:00 at the bottom instead of $(0, 0)$
    at the center. The vector to 12:00 is doubled to $(0, 2)$. The new twelve
    vectors add to ____.

Moving the origin to 6:00 moves adds $j = (0, 1)$ to each vector, thus sum of
the new twelve vectors goes from $\mathbf{0}$ to $(0, 12)$.

**Problems 15-19 go further with linear combinations of $v$ and $w$ (Figure
1.5a).**

(See page 20 for Figure 1.5)

15. Figure 1.5a shows $\dfrac{1}{2}v + \dfrac{1}{2}w$. Mark the points
    $\dfrac{3}{4}v + \dfrac{1}{4}w$ and $\dfrac{1}{4}v + \dfrac{1}{4}w$ and
    $v + w$.

(done by hand.)

16. Mark the point $-v + 2w$ and any other combination $cv + dw$ with
    $c + d = 1$. Draw the line of all combinations that have $c + d = 1$.

All combinations with $c + d = 1$ are on the line that passes through $v$ and
$w$. The point $V = -v + 2w$ is on that line but it is beyond $w$.

17. Locate $\dfrac{1}{3}v + \drac{1}{3}w$ and $\dfrac{2}{3}v + \dfrac{2}{3}w$.
    The combinations $cv + cw$ fill out what line?

Graphing these two points shows that $cv + cw$ will fill out the line indicated
by $u$. We are just scaling $v + w$ by $c$ when $c = d$.

18. Restricted by $0 \leq c \leq 1$ and $0 \leq d \leq 1$, shade in all
    combinations $cv + dw$.

Restricting $c$ and $d$ to $[0, 1]$ shades in all combinations of $cv + dw$ as
the entire parallelogram formed, with $v$ and $w$ being edges of the
parallelogram.

19. Restricted only by $c \geq 0$ and $d \geq 0$ draw the "cone" of all
    combinations $cv + dw$.

Restricting $c$ and $d$ to $[0, \infty)$ shades a "cone" of all combinations of
$cv + dw$ with $v$ and $w$ being the edges that define the cone's "limits".

**Problems 20-25 deal with $u, v, w$ in three-dimensional space (see Figure
1.5b).

(See page 20 for Figure 1.5)

20. Locate $\dfrac{1}{3}u + \dfrac{1}{3}v + \dfrac{1}{3}w$ and
    $\dfrac{1}{2}u + \dfrac{1}{2}w$ in Figure 1.5b. _(Challenge Problems are
    omitted.)_

$\dfrac{1}{3}u + \dfrac{1}{3}v + \dfrac{1}{3}w$ lies in the center of the
"triangle" (in 3d space this looks like a pyramid).
$\dfrac{1}{2}u + \dfrac{1}{2}w$ is a point that lies inbetween $u$ and $w$.

21. The three sides of the dashed triangle are $v - u$ and $w - v$ and $u - w$.
    Their sum is ____. Draw the head-to-tail addition around a plane triangle of
    $(3, 1)$ plus $(-1, 1)$ plus $(-2, -2)$.

Their sum is $\mathbf{0}$.

Those three sides of the triangle are in the same plane since
$(3, 1) + (-1, 1) + (-2, -2) = \mathbf{0}$.

22. Shade in the pyramid of combinations $cu + dv + ew$ with
    $c \geq 0, d \geq 0, e \geq 0$ and $c + d + e \leq 1$. Mark the vector
    $\dfrac{1}{2}(u + v + w)$ as inside or outside this pyramid.

The shaded combinations in the pyramid of $cu + dv + ew$ with $c \geq 0$,
$d \geq 0$, and $e \geq 0$ would be the entire pyramid and then shaded off into
$\infty$ were it not for the limitation of $c + d + e \leq 1$. Since the sum of
their coefficients is $\leq 1$, this limits the shaded region to within a shaded
tetrahedron with vertices $0, u, v, w$.

Since $c + d + e \leq 1$, it follows that the vector $\dfrac{1}{2}(u + v + w)$
would lie outside the shaded regionsince
$\dfrac{1}{2} + \dfrac{1}{2} + \dfrac{1}{2} = \dfrac{3}{2} > 1$, and we
established that $cu + dv + ew$ is the shaded region inside the tetrahedron.

23. If you look at _all_ combinations of those $u$, $v$, and $w$, is there any
    vector that can't be produced from $cu + dv + ew$? Different answer if
    $u, v, w$ are all in ____.

No, there is not a vector that can't be produced from $cu + dv + ew$. Consider
$cu + dv$, this fills a plane in \mathbf{R}^2 starting from $(0, 0)$. Then
adding $ew$ fills the \mathbf{R}^3 space.

However, the answer is different if $u, v, w$ are all in the same plane, then
their combinations could not span $\mathbf{R}^3$.

24. Which vectors are combinations of $u$ and $v$, and _also_ combinations of
    $v$ and $w$?

The vectors that are combinations of $u$ and $v$ are a plane, as are the
combinations of $v$ and $w$. The points along which they meet form a line,
namely on the vector $v$ which both planes share.

25. Draw vectors $u, v, w$ so that their combinations $cu + dv + ew$ fill only a
    line. Find vectors $u, v, w$ so that their combinations $cu + dv = ew$ fill
    only a plane.

(Done by hand.)

Note that for a line, simply draw any line where $u = v = w \neq \mathbf{0}$. A
simple example could be:

$$ u = \begin{bmatrix}{}1\\0\\0\end{bmatrix}, v = \begin{bmatrix}{}2\\0\\0\end{bmatrix}, w = \begin{bmatrix}{}-1\\0\\0\end{bmatrix} $$

Notice that they only differ along their $x$-coordinates and lie along the same
$y, z$-coordinates. This forms a line in 3-dimensional space, and essentially
what we've done is established 3 parallel vectors.

For a plane, consider $u \neq v$ with $w = u + v$. A simple example could be:

$$ u = \begin{bmatrix}{}1\\0\\0\end{bmatrix}, v = \begin{bmatrix}{}0\\1\\0\end{bmatrix} $$

Then:

$$ w = \begin{bmatrix}{}1\\1\\0\end{bmatrix} $$

Plotted along a 3-dimensional graph, we find that $u$ lies along the $x$-axes,
$v$ along the $y$-axes, and $w$ points diagonally between them, establishing a
plane along which their linear combination $cu + dv + ew$ fills.

Note that this is because since $w = u + v$, $w$ does not add any further
direction (as long as $u \neq dv \forall d \in \mathbf{R}$ _i.e._ they are not
parallel).

26. What combination
    $c\begin{bmatrix}{}1\\2\end{bmatrix} + d\begin{bmatrix}{}3\\1\end{bmatrix}$
    produces $\begin{bmatrix}{}14\\8\end{bmatrix}$? Express this question as two
    equations for the coefficients $c$ and $d$ in the linear combination.

$$ c\begin{bmatrix}{}1\\2\end{bmatrix} + d\begin{bmatrix}{}3\\1\end{bmatrix} = \begin{bmatrix}{}14\\8\end{bmatrix} $$

$$ \begin{bmatrix}{}c + 3d\\2c + d\end{bmatrix} = \begin{bmatrix}{}14\\8\end{bmatrix} $$

$$ c + 3d = 14 $$

$$ 2c + d = 8 $$

$$ d = 8 - 2c $$

$$ c + 3(8 - 2c) = 14 $$

$$ c + 14 - 6c = 14 $$

$$ -5c = -10 $$

$$ c = 2$$

$$ d = 8 - 2(2) $$

$$ d = 8 - 4 $$

$$ d = 4 $$

So:

$$ 2\begin{bmatrix}{}1\\2\end{bmatrix} + 4\begin{bmatrix}{}3\\1\end{bmatrix} = \begin{bmatrix}{}14\\8\end{bmatrix} $$
