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

---

Page 29

## Problem Set 1.2

1. Calculate the dot products $u \cdot v$ and $u \cdot w$ and $u \cdot (v + w)$
   and $w \cdot v$:

$$ u = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \quad v = \begin{bmatrix}{}4\\3\end{bmatrix} \quad w = \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ u \cdot v = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \cdot \begin{bmatrix}{}4\\3\end{bmatrix} $$

$$ = (-.6)(4) + (.8)(3) = -2.4 + 2.4 = 0 $$

$$ u \cdot w = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \cdot \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = (-.6)(1) + (.8)(2) = -.6 + 1.6 = 1 $$

$$ u \cdot (v + w) = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \cdot \left(\begin{bmatrix}{}4\\3\end{bmatrix} + \begin{bmatrix}{}1\\2\end{bmatrix}\right) $$

$$ = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \cdot \begin{bmatrix}{}5\\5\end{bmatrix} $$

$$ = (-.6)(5) + (.8)(5) = -3 + 4 = -1 $$

$$ w \cdot v = \begin{bmatrix}{}4\\3\end{bmatrix} \cdot \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = (4)(1) + (3)(2) = 4 + 6 = 10 $$

2. Compute the lengths $\|u\|$ and $\|v\|$ and $\|w\|$ of those vectors. Check
   the Schwarz inequalities $|u \cdot v| \leq \|u\|\|v\|$ and
   $|v \cdot w| \leq \|v\|\|w\|$.

$$ \|u\| = \sqrt{u \cdot u} $$

$$ u \cdot u = \begin{bmatrix}{}-.6\\.8\end{bmatrix} \cdot \begin{bmatrix}{}-.6\\.8\end{bmatrix} $$

$$ = (-.6)(-.6) + (.8)(.8) $$

$$ = .36 + .64 = 1 $$

$$ \|u\| = \sqrt{1} $$

$$ \|u\| = 1 $$

$$ \|v\| = \sqrt{v \cdot v} $$

$$ v \cdot v = \begin{bmatrix}{}4\\3\end{bmatrix} \cdot \begin{bmatrix}{}4\\3\end{bmatrix} $$

$$ = (4)(4) + (3)(3) = 16 + 9 = 25 $$

$$ \|v\| = \sqrt{25} $$

$$ = 5 $$

$$ \|w\| = \sqrt{w \cdot w} $$

$$ w \cdot w = \begin{bmatrix}{}1\\2\end{bmatrix} \cdot \begin{bmatrix}{}1\\2\end{bmatrix} $$

$$ = (1)(1) + (2)(2) = 1 + 4 = 5 $$

$$ \|w\| = \sqrt{5} $$

Checking Schwarz inequality $|u \cdot v | \leq \|u\|\|v\|$:

By exercise 1:

$$ |u \cdot v| = |0| = 0 $$

And by this exercise:

$$ \|u\|\|v\| = (1)(5) = 5 $$

So:

$$ |u \cdot v| = 0 \leq 5 = \|u\|\|v\| $$

Checking Schwarz inequality $|v \cdot w| \leq \|v\|\|w\|$:

By part 1:

$$ w \cdot v = v \cdot w = 10 $$

so:

$$ |v \cdot w| = |10| = 10 $$

By this exercise:

$$ \|v\|\|w\| = (5)(\sqrt{5}) = 5\sqrt{5} \approx 11.1803 $$

So:

$$ |v \cdot w| = 10 \leq 5\sqrt{5} = \|v\|\|w\| $$

3. Find unit vectors in the directions of $v$ and $w$ in Problem 1, and the
   cosine of the angle $\theta$. Choose vectors $a$, $b$, $c$ that make
   $0\degree$, $90\degree$, and $180\degree$ angles with $w$.

Find unit vector in directions of $v$:

Generic unit vector formula:

$$ u_v = \frac{v}{\|v\|} $$

By exercise 2, we know that:

$$ \|v\| = 5 $$

so:

$$ u = \frac{v}{\|v\|} = \begin{bmatrix}{}\frac{4}{5}\\\frac{3}{5}\end{bmatrix} $$

Find unit vectors in direction $w$:

$$ u_w = \frac{w}{\|w\|} $$

By exercise 2, we know that:

$$ \|w\| = \sqrt{5} $$

so:

$$ u_w = \frac{w}{\|w\|} = \begin{bmatrix}{}\frac{1}{\sqrt{5}}\\\frac{2}{\sqrt{5}}\end{bmatrix} $$

Find the cosine of angle $\theta$ (for $v$ and $w$):

Generic cosine formula is:

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

By exercise 1:

$$ w \cdot v = v \cdot w = 10 $$

By exercise 2:

$$ \|v\| = 5, \|w\| = \sqrt{5} $$

So:

$$ \cos\theta = \frac{10}{5\sqrt{5}} $$

$$ = \frac{2}{\sqrt{5}} $$

$$ = \frac{2\sqrt{5}}{5} $$

Choose vectors $a, b, c$ that make $0\degree, 90\degree$, and $180\degree$
angles with $w$:

For $0\degree$, we can simply apply a scalar value to $w$, so:

$$ a = 2w = 2\begin{bmatrix}{}1\\2\end{bmatrix} = \begin{bmatrix}{}2\\4\end{bmatrix} $$

We know that when the dot product of any two vectors equals $0$ means those two
vectors are perpendicular, and therefore there is a $90\degree$ angle between
them. Thus we need to find some vector $b$ that satisfies:

$$ b \cdot w = 0 $$

Equivalently:

$$ \begin{bmatrix}{}b_1\\b_2\end{bmatrix} \cdot \begin{bmatrix}{}1\\2\end{bmatrix} = 0 $$

$$ (b_1)(1) + (b_2)(2) = 0 $$

So, let $b_1 = -1, b_2 = \dfrac{1}{2}$, then:

$$ (-1)(1) + \left(\frac{1}{2}\right)(2) = 0 $$

Thus:

$$ b = \begin{bmatrix}{}-1\\\frac{1}{2}\end{bmatrix} $$

To find a vector $c$ that forms a $180\degree$ with $w$, simply apply $-1$ (or
any negative value) as a scalar to $w$:

$$ c = -1(w) = -1\begin{bmatrix}{}1\\2\end{bmatrix} = \begin{bmatrix}{}-1\\-2\end{bmatrix} $$

---

4. For any _unit_ vectors $v$ and $w$, find the dot products (actual numbers) of

a. $v$ and $-v$

Since $v$ is a unit vector:

$$ v \cdot v = 1 $$

We are trying to find:

$$ v \cdot (-v) $$

$$ = v \cdot v \cdot -1 $$

$$ = (v \cdot v)(-1) $$

By substitution:

$$ = (1)(-1) $$

$$ = -1 $$

b. $v + w$ and $v - w$

Again, since $v$ and $w$ are unit vectors, we know:

$$ v \cdot v = 1 $$

and:

$$ w \cdot w = 1 $$

We are trying to find:

$$ (v + w) \cdot (v - w) $$

$$ = (v + w)(v - w) $$

$$ = v^2 + vw - vw - w^2 $$

$$ = v^2 - w^2 $$

$$ = (v \cdot v) - (w \cdot w) $$

By substitution:

$$ = (1) - (1) $$

$$ = 1 - 1 $$

$$ = 0 $$

c. $v - 2w$ and $v + 2w$

Again:

$$ v \cdot v = 1 $$

$$ w \cdot w = 1 $$

So:

$$ (v - 2w) \cdot (v + 2w) $$

$$ = (v - 2w)(v + 2w) $$

$$ = v^2 - 4w^2 $$

$$ = (v \cdot v) - 4(w \cdot w) $$

$$ = (1) - 4(1) $$

$$ = 1 - 4 $$

$$ = -3 $$

5. Find unit vectors $u_1$ and $u_2$ in the directions of $v = (1, 3)$ and
   $w = (2, 1, 2)$. Find unit vectors $U_1$ and $U_2$ that are perpendicular to
   $u_1$ and $u_2$.

Find $u_1$:

Generic unit vector formula:

$$ u = \frac{v}{\|v\|} $$

So:

$$ u_1 = \frac{v}{\|v\|} $$

Find $\|v\|$:

$$ \|v\| = \sqrt{v \cdot v} $$

$$ v \cdot v = \begin{bmatrix}{}1\\3\end{bmatrix} \cdot \begin{bmatrix}{}1\\3\end{bmatrix} $$

$$ = (1)(1) + (3)(3) = 1 + 9 = 10 $$

$$ \|v\| = \sqrt{10} $$

$$ u_1 = \frac{v}{\|v\|} = \begin{bmatrix}{}\frac{1}{\sqrt{10}}\\\frac{3}{\sqrt{10}}\end{bmatrix} $$

Find $u_2$:

$$ u_2 = \frac{w}{\|w\|} $$

$$ \|w\| = \sqrt{w \cdot w} $$

$$ w \cdot w = \begin{bmatrix}{}2\\1\\2\end{bmatrix} \cdot \begin{bmatrix}{}2\\1\\2\end{bmatrix} $$

$$ = (2)(2) + (1)(1) + (2)(2) = 4 + 1 + 4 = 9 $$

$$ \|w\| = \sqrt{9} = 3 $$

$$ u_2 = \frac{w}{\|w\|} = \begin{bmatrix}{}\frac{2}{3}\\\frac{1}{3}\\\frac{2}{3}\end{bmatrix} $$

Find $U_1$:

$$ U_1 \cdot u_1 = 0 $$

$$ \begin{bmatrix}{}(U_1)_1\\(U_1)_2\end{bmatrix} \cdot \begin{bmatrix}{}\frac{1}{\sqrt{10}}\\\frac{3}{\sqrt{10}}\end{bmatrix} = 0 $$

$$ (U_1)_1\left(\frac{1}{\sqrt{10}}\right) + (U_1)_2\left(\frac{3}{\sqrt{10}}\right) = 0 $$

$$ \left(\frac{(U_1)_1}{\sqrt{10}}\right) + \left(\frac{3(U_1)_2}{\sqrt{10}}\right) = 0 $$

$$ (U_1)_1 + 3(U_1)_2 = (0)(\sqrt{10}) $$

$$ (U_1)_1 + 3(U_1)_2 = 0 $$

Choose $(U_1)_2 = 1$, then:

$$ (U_1)_1 + 3(1) = 0 $$

$$ (U_1)_1 + 3 = 0 $$

$$ (U_1)_1 = -3 $$

So one choice for $U_1$ is:

$$ U_1 = \begin{bmatrix}{}-3\\1\end{bmatrix} $$

But, since $U_1$ must be a unit vector:

$$ \|U_1\| = \sqrt{(-3)(-3) + (1)(1)} = \sqrt{9 + 1} = \sqrt{10} $$

$$ U_1 = \begin{bmatrix}{}\frac{-3}{\sqrt{10}}\\\frac{1}{\sqrt{10}}\end{bmatrix} $$

Find $U_2$:

$$ U_2 \cdot u_2 = 0 $$

$$ \begin{bmatrix}{}(U_2)_1\\(U_2)_2\\(U_2)_3\end{bmatrix} \cdot \begin{bmatrix}{}\frac{2}{3}\\\frac{1}{3}\\\frac{2}{3}\end{bmatrix} = 0 $$

$$ (U_2)_1\left(\frac{2}{3}\right) + (U_2)_2\left(\frac{1}{3}\right) + (U_2)_3\left(\frac{2}{3}\right) = 0 $$

$$ 2(U_2)_1 + (U_2)_2 + 2(U_2)_3 = 3(0) $$

$$ 2(U_2)_1 + (U_2)_2 + 2(U_2)_3 = 0 $$

Choose $(U_2)_1 = 1, (U_2)_3 = 0$, then:

$$ 2(1) + (U_2)_2 + 2(0) = 0 $$

$$ 2 + (U_2)_2 = 0 $$

$$ (U_2)_2 = -2 $$

So one possible choice for $U_2$ is:

$$ U_2 = \begin{bmatrix}{}1\\-2\\0\end{bmatrix} $$

And again, since $U_2$ must be a unit vector:

$$ \|U_2\| = \sqrt{(1)(1) + (-2)(-2) + (0)(0)} = \sqrt{1 + 4} = \sqrt{5} $$

$$ U_2 = \begin{bmatrix}{}\frac{1}{\sqrt{5}}\\\frac{-2}{\sqrt{5}}\\\frac{0}{\sqrt{5}}\end{bmatrix} $$

$$ U_2 = \begin{bmatrix}{}\frac{\sqrt{5}}{5}\\-\frac{2\sqrt{5}}{5}\\0\end{bmatrix} $$

6.

a. Describe every vector $w = (w_1, w_2)$ that is perpendicular to
$v = (2, -1)$.

For $w$ to be perpendicular to $v$:

$$ w \cdot v = 0 $$

$$ \begin{bmatrix}{}w_1\\w_2\end{bmatrix} \cdot \begin{bmatrix}{}2\\-1\end{bmatrix} = 0 $$

$$ 2(w_1) + (-1)(w_2) = 0 $$

$$ 2w_1 - w_2 = 0 $$

$$ 2w_1 = w_2 $$

So every vector of the form:

$$ \begin{bmatrix}{}2c\\c\end{bmatrix} $$

for any real number $c$ will be perpendicular to $v$.

b. All vectors perpendicular to $V = (1, 1, 1)$ lie on a ____ in 3 dimensions.

All vectors $(x, y, z)$ where $(x, y, z) \cdot (1, 1, 1) = 0$, this is:

$$ (x)(1) + (y)(1) + (z)(1) = x + y + z = 0 $$

Thus $(x, y, z)$ represents a plane through the origin in 3 dimensional space.

Answer: plane

c. The vectors perpendicular to both $(1, 1, 1)$ and $(1, 2, 3)$ lie on a ____.

This means that there exists some vector $v$ such that if $v = (v_1, v_2, v_3)$:

$$ (v_1, v_2, v_3) \cdot (1, 1, 1) = 0 $$

and

$$ (v_1, v_2, v_3) \cdot (1, 2, 3) = 0 $$

So:

$$ v_1 + v_2 + v_3 = 0 $$

and:

$$ v_1 + 2v_2 + 3v_3 = 0 $$

Now, subtracting one from the other yields:

$$ (v_1 + 2v_2 + 3v_3) - (v_1 + v_2 + v_3) = v_2 + 2v_3 = 0 \Rightarrow v_2 = -2v_3 $$

Substituting back in for $v_2$:

$$ v_1 + (-2v_3) + v_3 = 0 $$

$$ v_1 - v_3 = 0 $$

$$ v_1 = v_3 $$

Thus if we say $v_1 = v_3 = t$, and $v_2 = -2v_3 = -2t$, we get a vector of the
form:

$$ v = \begin{bmatrix}{}t\\-2t\\t\end{bmatrix} $$

Since this vector is simply scaled by $t$, we can say that this is a line.

Answer: line.

7. Find the angle $\theta$ (from its cosine) between these pairs of vectors:

Recall that the generic cosine formula is:

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

a. $v = \begin{bmatrix}{}1\\\sqrt{3}\end{bmatrix}$ and
$w = \begin{bmatrix}{}1\\0\end{bmatrix}$

$$ v \cdot w = \begin{bmatrix}{}1\\\sqrt{3}\end{bmatrix} \cdot \begin{bmatrix}{}1\\0\end{bmatrix} $$

$$ = (1)(1) + (\sqrt{3})(0) = 1 + 0 = 1 $$

$$ \|v\| = \sqrt{v \cdot v} = \sqrt{(1)(1) + (\sqrt{3})(\sqrt{3})} = \sqrt{1 + 3} = \sqrt{4} = 2 $$

$$ \|w\| = \sqrt{w \cdot w} = \sqrt{(1)(1) + (0)(0)} = \sqrt{1} = 1 $$

$$ \cos\theta = \frac{1}{(2)(1)} = \frac{1}{2} $$

$$ \theta = \cos^{-1}\left(\frac{1}{2}\right) $$

$$ \theta = \frac{\pi}{3} $$

b. $v = \begin{bmatrix}{}2\\2\\-1\end{bmatrix}$ and
$w = \begin{bmatrix}{}2\\-1\\2\end{bmatrix}$

$$ v \cdot w = \begin{bmatrix}{}2\\2\\-1\end{bmatrix} \cdot \begin{bmatrix}{}2\\-1\\2\end{bmatrix} $$

$$ = (2)(2) + (2)(-1) + (-1)(2) = 4 - 2 - 2 = 0 $$

$$ \|v\| = \sqrt{v \cdot v} = \sqrt{(2)(2) + (2)(2) + (-1)(-1)} = \sqrt{4 + 4 + 1} = \sqrt{9} = 3 $$

$$ \|w\| = \sqrt{w \cdot w} = \sqrt{(2)(2) + (-1)(-1) + (2)(2)} = \sqrt{4 + 1 + 4} = \sqrt{9} = 3 $$

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

$$ \cos\theta = \frac{0}{(3)(3)} = \frac{0}{9} = 0 $$

$$ \theta = \cos^{-1}(0) = \frac{\pi}{2} $$

c. $v = \begin{bmatrix}{}1\\\sqrt{3}\end{bmatrix}$ and
$w = \begin{bmatrix}{}-1\\\sqrt{3}\end{bmatrix}$

$$ v \cdot w = (1)(-1) + (\sqrt{3})(\sqrt{3}) = -1 + 3 = 2 $$

$$ \|v\| = \sqrt{(1)(1) + (\sqrt{3})(\sqrt{3})} = \sqrt{1 + 3} = \sqrt{4} = 2 $$

$$ \|w\| = \sqrt{(-1)(-1) + (\sqrt{3})(\sqrt{3})} = \sqrt{1 + 3} = \sqrt{4} = 2 $$

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

$$ \cos\theta = \frac{2}{(2)(2)} = \frac{2}{4} = \frac{1}{2} $$

$$ \theta = \cos^{-1}\left(\frac{1}{2}\right) = \frac{\pi}{3} $$

d. $v = \begin{bmatrix}{}3\\1\end{bmatrix}$ and
$w = \begin{bmatrix}{}-1\\-2\end{bmatrix}$

$$ v \cdot w = (3)(-1) + (1)(-2) = -3 - 2 = -5 $$

$$ \|v\| = \sqrt{v \cdot v} = \sqrt{(3)(3) + (1)(1)} = \sqrt{9 + 1} = \sqrt{10} $$

$$ \|w\| = \sqrt{w \cdot w} = \sqrt{(-1)(-1) + (-2)(-2)} = \sqrt{1 + 4} = \sqrt{5} $$

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

$$ \cos\theta = \frac{-5}{(\sqrt{10})(\sqrt{5})} $$

$$ \cos\theta = \frac{-5}{5\sqrt{2}} $$

$$ \cos\theta = \frac{-1}{\sqrt{2}} $$

$$ \cos\theta = -\frac{\sqrt{2}}{2} $$

$$ \theta = \cos^{-1}\left(-\frac{\sqrt{2}}{2}\right) $$

$$ \theta = \frac{3\pi}{4} $$

8. True or false (give a reason if true or find a counterexample if false):

a. If $u = (1, 1, 1)$ is perpendicular to $v$ and $w$, then $v$ is parallel to
$w$.

**Disproof (by counterexample):**

Suppose $u = \begin{bmatrix}{}1\\1\\1\end{bmatrix}$, and $u$ is perpendicular to
some vertex $v$ and also perpendicular to some vertex $w$.

It must be shown that $v$ is parallel to $w$.

Since $u$ is perpendicular to $v$ and $w$:

$$ u \cdot v = 0 $$

and:

$$ u \cdot w = 0 $$

To visualize this better, let us use subscript notation to get an idea of what
is happening:

$$ u \cdot v = (1, 1, 1) \cdot (v_1, v_2, v_3) = 0 $$

So:

$$ v_1(1) + v_2(1) + v_3(1) = v_1 + v_2 + v_3 = 0 $$

Similarly:

$$ u \cdot w = w_1 + w_2 + w_3 = 0 $$

In order for $v$ and $w$ to be parallel, one must be a scalar multiple of the
other, by some real number. In other words:

$$ v = cw $$

for some scalar $c \in \mathbf{R}$.

However, just because $v_1 + v_2 + v_3 = 0$, does not necessarily mean that
$v_1 = cw_1, v_2 = cw_2, v_3 = cw_3$, thus a counterexample must exist.

Let $v_1 = 3, v_2 = -2, v_3 = -1$, and also let $w_1 = 4, w_2 = -3, w_3 = -1$.

Now, if $v$ and $w$ were parallel, then there would be a consistent scalar $c$
that would equate the two:

$$ v_1(c) = w_1, v_2(c) = w_2, v_3(c) = w_3 $$

$$ 3c = 4, -2c = -3, -1c = -1 $$

But as you can see, solving for $c$ yields:

$$ c = \frac{4}{3}, c = \frac{3}{2}, c = 1 $$

Since $c$ cannot equal all of these different values at once (by the laws of
equality), it follows that this counterexample suitable disproves the
conclusion.

Q.E.D.

b. If $u$ is perpendicular to $v$ and $w$, then $u$ is perpendicular to
$v + 2w$.

**Proof:**

Suppose $u$ is any vector such that it is perpendicular to $v$ and $w$.

It must be shown that $u$ is perpendicular to $v + 2w$, equivalently, it must be
shown that:

$$ u \cdot (v + 2w) = 0 $$

By the supposition, $u$ is perpendicular to $v$ and $w$, in other words:

$$ u \cdot v = 0 $$

and:

$$ u \cdot w = 0 $$

Now, notice that:

$$ u \cdot (v + 2w) = uv + 2uw $$

$$ = (u \cdot v) + 2(u \cdot w) $$

Then, by substitution:

$$ = (0) + 2(0) $$

$$ = 0 + 0 $$

$$ = 0 $$

Thus it has been shown that $u \cdot (v + 2w) = 0$, and therefore $u$ is
perpendicular to $v + 2w$.

Q.E.D.

c. If $u$ and $v$ are perpendicular unit vectors then $\|u - v \| = \sqrt{2}$ .
_Yes!_

**Proof:**

Suppose $u$ and $v$ are any perpendicular unit vectors.

It must be shown that $\|u - v\| = \sqrt{2}$.

Since the norm of any vector is nonnegative, $\|u - v\|$ is nonnegative. It
follows that it suffices to show:

$$ \|u - v\|^2 = 2 $$

Recall that $\|u - v\| = \sqrt{(u - v) \cdot (u - v)}$, and thus:

$$ \|u - v\|^2 = (u - v) \cdot (u - v) $$

$$ = u^2 - 2uv + v^2 $$

$$ = (u \cdot u) - 2(u \cdot v) + (v \cdot v) $$

By the supposition, since $u$ and $v$ are perpendicular, it follows that:

$$ u \cdot v = 0 $$

Thus, by substitution:

$$ \|u - v\|^2 = (u \cdot u) - 2(0) + (v \cdot v) $$

$$ = (u \cdot u) + (v \cdot v) $$

By the supposition, both $u$ and $v$ are unit vectors, which means that their
lengths are equal to $1$.

$$ \|u\| = 1, \|v\| = 1 $$

Again, since the norm of any vector is nonnegative, it follows that:
$\|u\|^2 = u \cdot u$ and $\|v\|^2 = v \cdot v$, and thus:

$$ u \cdot u = 1, v \cdot v = 1 $$

Then, by substitution:

$$ \|u - v\|^2 = (u \cdot u) + (v \cdot v) $$

$$ = (1) + (1) $$

$$ = 2 $$

This is what was to be shown.

Q.E.D.

9. The slopes of the arrows from $(0, 0)$ to $(v_1, v_2)$ and $(w_1, w_2)$ are
   $\dfrac{v_2}{v_1}$ and $\dfrac{w_2}{w_1}$. **Suppose the product
   $\dfrac{v_2w_2}{v_1w_1}$ of the slopes is $-1$**. Show that $v \cdot w = 0$
   and the vectors are perpendicular (The line $y = 4x$ is perpendicular to
   $y = -\dfrac{1}{4}x$.)

**Proof:**

Suppose $v$ and $w$ are two vectors along a standard Cartesian plane such that
$v$ goes from the origin, $(0, 0)$, to $(v_1, v_2)$ and $w$ goes from the origin
$(0, 0)$, to $(w_1, w_2)$.

Then, the slopes of these vectors are $\dfrac{v_2}{v_1}$ and $\dfrac{w_2}{w_1}$.

Suppose the product of these two slopes is $-1$:

$$ \frac{v_2}{v_1} \cdot \frac{w_2}{w_1} = \frac{v_2w_2}{v_1w_1} = -1 $$

It must be shown that $v \cdot w = 0$ and the vectors are perpendicular. Since
these two statements are logically equivalent, it suffices to show that
$v \cdot w = 0$.

Now, by the definition of the dot product:

$$ v \cdot w = \begin{bmatrix}{}v_1\\v_2\end{bmatrix} \cdot \begin{bmatrix}{}w_1\\w_2\end{bmatrix} $$

$$ = v_1w_1 + v_2w_2 $$

By the supposition:

$$ \frac{v_2w_2}{v_1w_1} = -1 $$

which means that:

$$ v_2w_2 = -v_1w_1 $$

So, by substitution:

$$ v \cdot w = v_1w_1 + v_2w_2 $$

$$ v \cdot w = v_1w_1 + (-v_1w_1) $$

$$ v \cdot w = 0 $$

This is what was to be shown.

Q.E.D.

10. Draw arrows from $(0, 0)$ to the points $v = (1, 2)$ and $w = (-2, 1)$.
    Multiply their slopes. That answer is a signal that $v \cdot w = 0$ and the
    arrows are ____.

$$ v_{\text{slope}} = \frac{2}{1} = 2 $$

$$ w_{\text{slope}} = \frac{1}{-2} = -\frac{1}{2} $$

$$ v_{\text{slope}} \cdot w_{\text{slope}} = 2 \cdot \left(-\frac{1}{2}\right) = -1 $$

By the proof of exercise 9, it has been shown that when the product of two
vectors' slopes is $-1$, that $v \cdot w = 0$.

By the definition of perpendicular vectors, this means that these two arrows are
_perpendicular_.

Answer: perpendicular

11. If $v \cdot w$ is negative, what does this say about the angle between $v$
    and $w$? Draw a 3-dimensional vector $v$ (an arrow), and show where to find
    all $w$'s with $v \cdot w < 0$.

When $v \cdot w < 0$, this implies by the cosine formula that the angle between
$v$ and $w$, $\theta$, is $\theta > 90\degree$.

The reason for this comes from the cosine formula:

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

Equivalently, notice that this is:

$$ v \cdot w = \cos\theta(\|v\|\|w\|) $$

By the definition of norm, $\|v\|\|w\| > 0$, so since $v \cdot w < 0$, this
means that $\cos\theta < 0$. Consulting a basic unit circle will show that
$\cos^{-1}(0) = \dfrac{\pi}{2} = 90\degree$, so $\theta > 90\degree$.

Once $v$ is drawn in $\mathbf{R}^3$, one can find all $w$'s in half of
$\mathbf{R}^3$.

Geometrically, the plane through the origin perpendicular to $v$ divides
$\mathbf{R}^3$ into two half-spaces. All vectors $w$ in the half-space opposite
the direction of $v$ make an obtuse angle with $v$, so $v \cdot w < 0$; the
dividing plane itself is excluded because there $v \dot w = 0$.

12. With $v = (1, 1)$ and $w = (1, 5)$ choose a number $c$ so that $w - cv$ is
    perpendicular to $v$. Then find the formula for $c$ starting from _any_
    nonzero $v$ and $w$.

For $w - cv$ and $v$ to be perpendicular, it must be true that:

$$ v \cdot (w - cv) = 0 $$

Equivalently:

$$ \begin{bmatrix}{}1\\1\end{bmatrix} \cdot \left(\begin{bmatrix}{}1\\5\end{bmatrix} - c\begin{bmatrix}{}1\\1\end{bmatrix}\right) = 0 $$

$$ \begin{bmatrix}{}1\\1\end{bmatrix} \cdot \left(\begin{bmatrix}{}1\\5\end{bmatrix} - \begin{bmatrix}{}c\\c\end{bmatrix}\right) = 0 $$

$$ \begin{bmatrix}{}1\\1\end{bmatrix} \cdot \begin{bmatrix}{}1 - c\\5 - c\end{bmatrix} = 0 $$

$$ (1)(1 - c) + (1)(5 - c) = 0 $$

$$ 1 - c + 5 - c = 0 $$

$$ 6 - 2c = 0 $$

$$ 6 = 2c $$

$$ 3 = c $$

$$ c = 3 $$

For the more general formula, start from the beginning again:

$$ v \cdot (w - cv) = 0 $$

$$ (v \cdot w) - (v \cdot v \cdot c) = 0 $$

$$ (v \cdot w) - (\|v\|^2 \cdot c) = 0 $$

$$ v \cdot w = \|v\|^2 \cdot c $$

$$ \frac{v \cdot w}{\|v\|^2} = c $$

$$ c = \frac{v \cdot w}{\|v\|^2} $$

13. Find nonzero vectors $v$ and $w$ that are perpendicular to $(1, 0, 1)$ and
    to each other.

$$ v \cdot \begin{bmatrix}{}1\\0\\1\end{bmatrix} = 0 $$

and:

$$ w \cdot \begin{bmatrix}{}1\\0\\1\end{bmatrix} = 0 $$

and:

$$ v \cdot w = 0 $$

First, evaluate $v$:

$$ v \cdot (1, 0, 1) = \begin{bmatrix}{}v_1\\v_2\\v_3\end{bmatrix} \cdot \begin{bmatrix}{}1\\0\\1\end{bmatrix} = 0 $$

$$ v_1(1) + v_2(0) + v_3(1) = 0 $$

$$ v_1 + v_3 = 0 $$

$$ v_1 = -v_3 $$

Thus:

$$ v = (v_1, v_2, -v_1) $$

Now similarly, for $w$, we can do the same:

$$ w = (w_1, w_2, -w_1) $$

Now, since $v \cdot w = 0$:

$$ v_1w_1 + v_2w_2 + (-v_1)(-w_1) = 0 $$

$$ v_1w_1 + v_2w_2 + v_1w_1 = 0 $$

$$ 2v_1w_1 + v_2w_2 = 0 $$

So, choose $v_1 = 0, v_2 = 1, v_3 = 0$, and $w_1 = 1, w_2 = 0, w_3 = -1$.

Check each:

$$ v \cdot (1, 0, 1) = (0)(1) + (1)(0) + (0)(1) = 0 $$

$$ w \cdot (1, 0, 1) = (1)(1) + (0)(0) + (-1)(1) = 0 $$

$$ v \cdot w = (0)(1) + (1)(0) + (0)(-1) = 0 $$

Thus:

$$ v = \begin{bmatrix}{}0\\1\\0\end{bmatrix}, w = \begin{bmatrix}{}1\\0\\-1\end{bmatrix} $$

14. Find nonzero vectors $u, v, w$ that are perpendicular to $(1, 1, 1, 1)$ and
    to each other.

Omitted.

15. The geometric mean of $x = 2$ and $y = 8$ is $\sqrt{xy} = 4$. The arithmetic
    mean is larger: $\dfrac{1}{2}(x + y) =$ ____. This would come in Example 6
    from the Schwarz inequality for $v = (\sqrt{2}, \sqrt{8})$ and
    $w = (\sqrt{8}, \sqrt{2})$. Find $\cos\theta$ for this $v$ and $w$.

$$ \frac{1}{2}(x + y) = \frac{1}{2}(2 + 8) = \frac{1}{2}(10) = 5 $$

$$ \sqrt{xy} \leq \frac{x + y}{2} $$

$$ \sqrt{2 \cdot 8} \leq \frac{2 + 8}{2} $$

$$ \sqrt{10} \leq \frac{10}{2} $$

$$ \sqrt{10} \approx 3.162277 \leq 5 $$

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

$$ v \cdot w = (\sqrt{2})(\sqrt{8}) + (\sqrt{8})(\sqrt{2}) $$

$$ = 2(\sqrt{2})(\sqrt{8}) $$

$$ = 2(\sqrt{2})(2\sqrt{2}) $$

$$ = 4(\sqrt{2})(\sqrt{2}) $$

$$ = 4(2) $$

$$ = 8 $$

$$ \|v\| = \sqrt{(\sqrt{2})(\sqrt{2}) + (\sqrt{8})(\sqrt{8})} $$

$$ = \sqrt{2 + 8} = \sqrt{10} $$

$$ \|w\| = \sqrt{(\sqrt{8})(\sqrt{8}) + (\sqrt{2})(\sqrt{2})} $$

$$ = \sqrt{8 + 2} = \sqrt{10} $$

$$ \cos\theta = \frac{8}{\sqrt{10} \cdot \sqrt{10}} $$

$$ = \frac{8}{10} $$

$$ = \frac{4}{5} $$

This matches the Schwarz inequality:

$$ |v \cdot w| \leq \|v\|\|w\| $$

$$ |8| \leq (\sqrt{10})(\sqrt{10}) $$

$$ 8 \leq 10 $$

16. How long is the vector $v = (1, 1, \dots, 1)$ in 9 dimensions? Find a unit
    vector $u$ in the same direction as $v$ and a unit vector $w$ that is
    perpendicular to $v$.

Since
$\|v\| = \sqrt{v \cdot v} = \sqrt{\underbrace{(1)(1) + (1)(1) + \cdots + (1)(1)}_{\text{summed 9 times}}} = \sqrt{9} = 3$.

Then, finding the unit vector that is parallel (same direction) to $v$:

$$ u = \frac{v}{\|v\|} = \begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\\vdots\\\frac{1}{3}\end{bmatrix} $$

Then, find a unit vector $w_{\text{vec}}$ perpendicular to $v$:

$$ v \cdot w = 0 $$

$$ (1, 1, \dots, 1) \cdot w = 0 $$

$$ 1w_1 + 1w_2 + \cdots + 1w_9 = 0 $$

$$ w_1 + w_2 + \cdots + w_9 = 0 $$

So, $let w_1 = 1$, $w_2, \dots, w_8 = 0$, and $w_9 = -1$.

Thus far, $w$ is:

$$ w = (1, 0, 0, \dots, 0, -1) $$

Now, to find $w_{\text{uv}}$, a unit vector:

$$ w_{\text{uv}} = \frac{w}{\|w\|} $$

$$ \|w\| = \sqrt{w \cdot w} = \sqrt{(1)(1) + (0)(0) + \cdots + (0)(0) + (-1)(-1)} = \sqrt{1 + 1} = \sqrt{2} $$

$$ w_{\text{uv}} = \left(\frac{1}{\sqrt{2}}, 0, 0 \dots, 0, -\frac{1}{\sqrt{2}}\right) $$

17. What are the cosines of the angles $\alpha, \beta, \theta$ between the
    vector $(1, 0, -1)$ and the unit vectors $i, j, k$ along the axes? Check the
    formula $\cos^2\alpha + \cos^2\beta + \cos^2\theta = 1$.

Recall the generic cosine formula:

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

Now, let's define $i$, j, k$:

$$ i = \begin{bmatrix}{}1\\0\\0\end{bmatrix} $$

$$ j = \begin{bmatrix}{}0\\1\\0\end{bmatrix} $$

$$ k = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

Now, $\alpha$ is the angle between $(1, 0, -1)$ (let's denote it $v$) and $i$,
so $\cos\alpha$:

$$ \cos\alpha = \frac{v \cdot i}{\|v\|\|i\|} $$

$$ v \cdot i = (1)(1) + (0)(0) + (0)(-1) = 1 $$

$$ \|v\| = \sqrt{(1)(1) + (0)(0) + (-1)(-1)} = \sqrt{2} $$

$$ \|i\| = \sqrt{(1)(1) + (0)(0) + (0)(0)} = \sqrt{1} = 1 $$

$$ \cos\alpha = \frac{1}{\sqrt{2}(1)} = \frac{1}{\sqrt{2}} = \frac{\sqrt{2}}{2} $$

Now, $\beta$ is the angle between $v$ and $j$, so $\cos\beta$:

$$ \cos\beta = \frac{v \cdot j}{\|v\|\|j\|} $$

$$ v \cdot j = (1)(0) + (0)(1) + (-1)(0) = 0 $$

$$ \|j\| = \sqrt{(0)(0) + (1)(1) + (0)(0)} = \sqrt{1} = 1 $$

$$ \cos\beta = \frac{0}{(\sqrt{2})(1)} = \frac{0}{\sqrt{2}} = 0 $$

Now, $\theta$ is the angle between $v$ and $k$, so $\cos\theta$:

$$ \cos\theta = \frac{v \cdot k}{\|v\|\|k\|} $$

$$ v \cdot k = (1)(0) + (0)(0) + (-1)(1) = -1 $$

$$ \|k\| = \sqrt{(0)(0) + (0)(0) + (-1)(-1)} = \sqrt{1} = 1 $$

$$ \cos\theta = \frac{-1}{(\sqrt{2})(1)} = -\frac{1}{\sqrt{2}} = -\frac{\sqrt{2}}{2} $$

Check that $\cos^2\alpha + \cos^2\beta + \cos^2\theta = 1$:

$$ \cos^2\alpha + \cos^2\beta + \cos^2\theta = \left(\frac{\sqrt{2}}{2}\right)^2 + (0)^2 + \left(-\frac{\sqrt{2}}{2}\right)^2 $$

$$ = \frac{1}{2} + 0 + \frac{1}{2} $$

$$ = \boxed{1} $$

Problems 18-28 lead to the main facts about lengths and angles in triangles.

18. The parallelogram with sides $v = (4, 2)$ and $w = (-1, 2)$ is a rectangle.
    Check the Pythagoras formula $a^2 + b^2 = c^2$ which is for _right triangles
    only_:

$$ (\text{length of } v)^2 + (\text{length of } w)^2 = (\text{length of} v + w)^2 $$

This means:

$$ \|v\|^2 + \|w\|^2 = \|v + w\|^2 $$

$$ \|v\|^2 = v \cdot v = (4)(4) + (2)(2) = 16 + 4 = 20 $$

$$ \|w\|^2 = w \cdot w = (-1)(-1) + (2)(2) = 1 + 4 = 5  $$

$$ \|v + w\|^2 = (v + w) \cdot (v + w) $$

$$ v + w = \begin{bmatrix}{}4 + (-1)\\2 + 2\end{bmatrix} = \begin{bmatrix}{}3\\4\end{bmatrix} $$

$$ \|v + w\|^2 = (v + w) \cdot (v + w) $$

$$ = (3)(3) + (4)(4) = 9 + 16 = 25 $$

So:

$$ \|v\|^2 + \|w\|^2 = \|v + w\|^2 $$

$$ 20 + 5 = 25 $$

$$ \boxed{25 = 25} $$

19. (Rules for dot products) These equations are simple but useful:

(1) $v \cdot w = w \cdot v$

(2) $u \cdot (v + w) = u \cdot v + u \cdot w$

(3) $(cv) \cdot w = c(v \cdot w)$

Use (2) with $u = v + w$ to prove
$\|v + w\|^2 = v \cdot v + 2v \cdot w + w \cdot w$.

**Proof:**

Suppose $u$, $v$, $w$ are any vectors such that
$u \cdot (v + w) = u \cdot v + u \cdot w$ and $u = v + w$.

It must be shown that $\|v + w\|^2 = v \cdot v + 2v \cdot w + w \cdot w$.

By the supposition, since $u = v + w$, by substitution for $u$ into
$u \cdot (v + w) = u \cdot v + u \cdot w$ yields:

$$ (v + w) \cdot (v + w) = (v + w) \cdot v + (v + w) \cdot w $$

By the definition of the length of a vector
$(v + w) \cdot (v + w) = \|v + w\|^2$, so:

$$ \|v + w\|^2 = (v + w) \cdot v + (v + w) \cdot w $$

Then, by algebra:

$$ = (v \cdot v) + (v \cdot w) + (v \cdot w) + (w \cdot w) $$

$$ = v \cdot v + 2 \cdot v \cdot w + w \cdot w $$

This is what was to be shown.

Q.E.D.

20. The "Law of Cosines" comes from
    $(v - w) \cdot (v - w) = v \cdot v - 2v \cdot w + w \cdot w$:

**Cosine Law**

$$ \|v - w\|^2 = \|v\|^2 - 2\|v\|\|w\|\cos\theta + \|w\|^2 $$

Draw a triangle with sides $v$ and $w$ and $v - w$. Which of the angles is
$\theta$?

(Done by hand.)

21. The _triangle inequality_ says:
    $(\text{length of } v + w) \leq (\text{length of } v) + (\text{length of } w)$.

Problem 19 found $\|v + w\|^2 = \|v\|^2 + 2v \cdot w + \|w\|^2$. Increase that
$v \cdot w$ to $\|v\|\|w\|$ to show that $\|\textbf{side 3}\|$ can not exceed
$\|\textbf{side 1}\| + \|\textbf{side 2}\|$:

**Triangle Inequality**

$$ \|v + w\|^2 \leq (\|v\| + \|w\|)^2 \textbf{ or } \|v + w\| \leq \|v\| + \|w\| $$

**Proof:**

Suppose $v$ and $w$ are any vectors.

It must be shown that:

$$ \|v + w\|^2 \leq \left(\|v\| + \|w\|\right)^2 $$

or equivalently:

$$ \|v + w\| \leq \|v\| + \|w\| $$

By problem 19, it has been shown that:

$$ \|v + w\|^2 = \|v\|^2 + 2v \cdot w + \|w\|^2 $$

Increasing the middle term $2v \cdot w$ to $2\|v\|\|w\|$ yields the following
inequality:

$$ \|v + w\|^2 \leq \|v\|^2 + 2\|v\|\|w\| + \|w\|^2 $$

Notice that this is a perfect square, and thus factors into:

$$ \|v + w\|^2 \leq \left(\|v\| + \|w\|\right)\left(\|v\| + \|w\|\right) $$

$$ \|v + w\|^2 \leq \left(\|v\| + \|w\|\right)^2 $$

This is what was to be shown.

Q.E.D.

(See page 31 for Figure)

22. The Schwarz inequality $|v \cdot w \leq \|v\|\|w\|$ by algebra instead of
    trigonometry:

a. Multiply out both sides of
$(v_1w_1 + v_2w_2)^2 \leq \left(v_1^2 + v_2^2\right)\left(w_1^2 + w_2^2\right)$

$$ (v_1w_1 + v_2w_2)^2 \leq \left(v_1^2 + v_2^2\right)\left(w_1^2 + w_2^2\right) $$

Expanding left-hand side:

$$ (v_1w_1 + v_2w_2)^2 = (v_1w_1 + v_2w_2)(v_1w_1 + v_2w_2) $$

$$ = (v_1w_1)^2 + 2(v_1w_1)(v_2w_2) + (v_2w_2)^2 $$

Expanding right-hand side:

$$ \left(v_1^2 + v_2^2\right)\left(w_1^2 + w_2^2\right) $$

$$ = v_1^2w_1^2 + v_2^2w_1^2 + v_1^2w_2^2 + v_2^2w_2^2 $$

Thus the final inequality, multiplied out is:

$$ (v_1w_1)^2 + 2(v_1w_1)(v_2w_2) + (v_2w_2)^2 \leq v_1^2w_1^2 + v_2^2w_1^2 + v_1^2w_2^2 + v_2^2w_2^2 $$

b. Show that the difference between those two sides equals
$(v_1w_2 - v_2w_1)^2$. This cannot be negative since it is a square - so the
inequality is true.

To show that this inequality is true, subtract the left-hand side from the
right-hand side:

$$ (v_1^2w_1^2 + v_2^2w_1^2 + v_1^2w_2^2 + v_2^2w_2^2) - ((v_1w_1)^2 + 2(v_1w_1)(v_2w_2) + (v_2w_2)^2) $$

$$ = v_1^2w_1^2 + v_2^2w_1^2 + v_1^2w_2^2 + v_2^2w_2^2 - (v_1w_1)^2 - 2(v_1w_1)(v_2w_2) - (v_2w_2)^2 $$

$$ = v_1^2w_1^2 + v_2^2w_1^2 + v_1^2w_2^2 + v_2^2w_2^2 - v_1^2w_1^2 - 2v_1w_1v_2w_2 - v_2^2w_2^2 $$

$$ = v_2^2w_1^2 + v_1^2w_2^2 - 2v_1w_1v_2w_2 $$

$$ = v_1^2w_2^2 - 2v_1w_1v_2w_2 + v_2^2w_1^2 $$

Notice that this is a perfect square, factoring this yields:

$$ = (v_1w_2 - v_2w_1)(v_1w_2 - v_2w_1) $$

$$ = \boxed{(v_1w_2 - v_2w_1)^2} $$

As stated in the problem statement, this cannot be negative since it is a
square, and thus the inequality from part (a) holds.

23. The figure shows that $\cos\alpha = \dfrac{v_1}{\|v\|}$ and
    $\sin\alpha = \dfrac{v_2}{\|v\|}$. Similarly $\cos\beta$ is ____ and
    $\sin\beta$ is ____. The angle $\theta$ is $\beta - \alpha$. Substitute into
    the trigonometry formula $\cos\beta\cos\alpha + \sin\beta\sin\alpha$ for
    $\cos(\beta - \alpha)$ to find $\cos\theta = \dfrac{v \cdot w}{\|v\|\|w\|}$.

$$ \cos\beta = \frac{w_1}{\|w\|} $$

$$ \sin\beta = \frac{w_2}{\|w\|} $$

This is one of the many trigonometry identities:

$$ \cos(\beta - \alpha) = \cos\beta\cos\alpha + \sin\beta\sin\alpha $$

So, by substitution:

$$ \cos(\beta - \alpha) = \left(\frac{w_1}{\|w\|}\right)\left(\frac{v_1}{\|v\|}\right) + \left(\frac{w_2}{\|w\|}\right)\left(\frac{v_2}{\|v\|}\right) $$

Now, note that $\beta - \alpha = \theta$ (by the shown figure), so:

$$ \cos(\theta) = \left(\frac{w_1}{\|w\|}\right)\left(\frac{v_1}{\|v\|}\right) + \left(\frac{w_2}{\|w\|}\right)\left(\frac{v_2}{\|v\|}\right) $$

Then, by algebra, we can simplify to a single fraction:

$$ \cos(\theta) = \frac{v_1w_1 + v_2w_2}{\|v\|\|w\|} $$

By the definition for dot product $(v \cdot w) = v_1w_1 + v_2w_2$, thus by
substitution:

$$ \boxed{\cos(\theta) = \frac{v \cdot w}{\|v\|\|w\|}} $$

24. One-line proof of the inequality $|u \cdot U| \leq 1$ for unit vectors
    $(u_1, u_2)$ and $(U_1, U_2)$:

$$ |u \cdot U| \leq |u_1||U_1| + |u_2||U_2| \leq \frac{u_1^2 + U_1^2}{2} + \frac{u_2^2 + U_2^2}{2} = 1 $$

Put $(u_1, u_2) = (.6, .8)$ and $(U_1, U_2) = (.8, .6)$ in that whole line and
find $\cos\theta$.

By substitution:

$$ |u \cdot U| \leq |.6||.8| + |.8||.6| \leq \frac{(.6)^2 + (.8)^2}{2} + \frac{(.8)^2 + (.6)^2}{2} = 1 $$

$$ |u \cdot U| \leq .48 + .48 \leq \frac{.36 + .64}{2} + \frac{.64 + .36}{2} = 1 $$

$$ |u \cdot U| \leq .96 \leq \frac{1}{2} + \frac{1}{2} = 1 $$

$$ |u \cdot U| \leq .96 \leq 1 = 1 $$

$$ |u \cdot U| \leq .96 \leq 1 $$

Recall that the cosine formula (with these variable naming conventions )is:

$$ \cos\theta = \frac{u \cdot U}{\|u\|\|U\|} $$

We have calculated $u \cdot U = .96$, and we know that both $u$ and $U$ are unit
vectors by the problem statement, which means that both their lengths are $1$.
Thus, the denominator $\|u\|\|U\| = (1)(1) = 1$.

It follows that:

$$ \boxed{\cos\theta = .96} $$

25. Why is $|\cos\theta|$ never greater than $1$ in the first place?

Recall that the general formula for cosine states that for any vectors $v$ and
$w$:

$$ \cos\theta = \frac{v \cdot w}{\|v\|\|w\|} $$

The problem statement claims that $\|\cos\theta\| \leq 1$, this is true by the
Schwarz inequality, which itself states that for any given vectors $v$ and $w$:

$$ |v \cdot w| \leq \|v\|\|w\| $$

This means that the numerator of the cosine formula must always be less than or
equal to the denominator, and thus by the laws of fractions, it is known that
this fraction must always be $\leq 1$.

26. (_Recommended_) Draw a parallelogram

(Done by hand.)

27. Parallelogram with two sides $v$ and $w$. Show that the square diagonal
    lengths $\|v + w\|^2 + \|v - w\|^2$ add to the sum of four squared side
    lengths $2\|v\|^2 + 2\|w\|^2$.

$$ \|v + w\|^2 + \|v - w\|^2 $$

$$ = ((v + w) \cdot (v + w)) + ((v - w) \cdot (v - w)) $$

$$ = (v^2 + 2vw + w^2) + (v^2 - 2vw + w^2) $$

$$ = v^2 + w^2 + v^2 + w^2 $$

$$ = 2v^2 + 2w^2 $$

$$ = 2(v \cdot v) + 2(w \cdot w) $$

$$ = \boxed{2\|v\|^2 + 2\|w\|^2} $$

28. If $v = (1, 2)$ draw all vectors $w =(x, y)$ in the $xy$ plane with
    $v \cdot w = x + 2y = 5$. Why do those $w$'s lie along a line? Which is the
    shortest $w$?

$x + 2y$ is a linear equation in $x$ and $y$, and that is why those $w$'s lie
along a line. The shortest $w$ is one that satisfies $v \cdot w = x + 2y = 5$,
which is $w = (1, 2)$.

To verify that this is the shortest $w$, first verify that the two are parallel.
By definition for parallel, $w$ is parallel since $w$ is a scalar multiple of
$1$ of $v$, _i.e._ $w = 1v$. It follows that $w$ is perpendicular to the line
$x + 2y$ since $w = v$, and thus $w = (1, 2)$ is the shortest $w$.

29. (_Recommended_) If $\|v\| = 5$ and $\|w\| = 3$, what are the smallest and
    largest possible values of $\|v - w\|$? What are the smallest and largest
    possible values of $v \cdot w$?

The triangle equality states that for any vectors $v$ and $w$:

$$ \|v + w\| \leq \|v\| + \|w\| $$

Since the length of a vector cannot be negative, it follows that for any vector
$w$ $\|w\| = \|-w\|$, since $-w$ is just vector $180\degree$ from $w$.

$$ \|v + (-w)\| \leq \|v\| + \|w\| $$

$$ \|v - w\| \leq \|v\| + \|w\| $$

By substitution:

$$ \|v - w\| \leq (5) + (3) $$

$$ \|v - w\| \leq 8 $$

So the largest value of $\|v - w\| = 8$.

To find the smallest value, consider the triangle inequality once again, but
replace the standard $\|v\|$ with $\|v - w\|$:

$$ \|v + w\| \leq \|v\| + \|w\| $$

becomes:

$$ \|(v - w) + w\| \leq \|v - w \| + \|w\| $$

Now:

$$ \|v\| \leq \|v - w\| + \|w\| $$

$$ \|v\| - \|w\| \leq \|v - w\| $$

$$ (5) - (3) \leq \|v - w\| $$

$$ 2 \leq \|v - w\| $$

And so $\|v - w\| \geq 2$, thus $2$ is the smallest value for $\|v - w\|$.

By the Schwarz inequality, for any vectors $v$ and $w$:

$$ \|v \cdot w \| \leq \|v\|\|w\| $$

By substitution:

$$ \|v \cdot w \| \leq (5)(3) $$

$$ \|v \cdot w \| \leq 15 $$

Thus the smallest possible value for $v \cdot w = -15$, and the largest value
for $v \cdot w = 15$.
