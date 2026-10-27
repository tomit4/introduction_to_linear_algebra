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

_Solution:_

The supposition is saying that:

$$
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} +
\begin{bmatrix}{}y_1\\y_2\end{bmatrix} =
\begin{bmatrix}{}x_1 + y_2\\x_2 + y_1\end{bmatrix}
$$

and also that:

$$
c\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}cx_1\\cx_2\end{bmatrix}
$$

_Rule 1 is not satisfied since:_

$x + y = (x_1 + y_2, x_2 + y_1)$ means that $y + x = (y_1 + x_2, y_2 + x_1)$,
which can only be true if $x_1 + y_2 = y_1 + x_2$, which is not _generally_
true, thus rule 1 is not satisfied.

_Rule 2 is not satisfied since:_

$$ x + (y + z) = (x + y) + z $$

is what rule 2 states. Now, let's expand what this means in the context of the
supposition given, the left-hand side of the above equation would be:

$$ x + (y + z) = (x_1 + (y_1 + z_2), x_2 + (y_2 + z_1)) $$

and the right-hand side of the above equation would be:

$$ (x + y) + z = ((x_1 + y_2) + z_1, (x_2 + y_1) + z_2) $$

So for Rule 2 to be satisfied, these two sides would have to be equal

$$ (x_1 + (y_1 + z_2), x_2 + (y_2 + z_1)) = ((x_1 + y_2) + z_1, (x_2 + y_1) + z_2) $$

When we remove these extra parentheses, we are left with:

$$ (x_1 + y_1 + z_2, x_2 + y_2 + z_1) = (x_1 + y_2 + z_1, x_2 + y_1 + z_2) $$

But for this to be true, then the following equalities would have to hold:

$$
x_1 + y_1 + z_2 = x_1 + y_2 + z_2 \\
x_2 + y_2 + z_1 = x_2 + y_1 + z_2 \\
$$

And this is not generally true, thus rule 2 is not satisfied.

Rules 3 through 7 are satisfied since $cx = (cx_1, cx_2)$ holds.

_Rule 8 is not satisfied:_

Rule 8 states:

$$ (c_1 + c_2)x = c_1x + c_2x $$

However by the supposition, the left-hand side expands to:

$$ (c_1 + c_2)x = ((c_1 + c_2)x_1, (c_1 + c_2)x_2) $$

While the right-hand side expands to:

$$ c_1x + c_2x = (c_1x_1, c_1x_2) + (c_2x_1, c_2x_2) $$

and apply the supposition's addition property:

$$ = (c_1x_1 + c_2x_2, c_1x_2 + c_2x_1) $$

So now set them side by side, distribute on the left, and compare the
equalities:

$$ ((c_1 + c_2)x_1, (c_1 + c_2)x_2) = (c_1x_1 + c_2x_2, c_1x_2 + c_2x_1) $$

$$ (c_1x_1 + c_2x_1, c_1x_2 + c_2x_2) = (c_1x_1, c_1x_2) + (c_2x_1, c_2x_2) $$

This is not generally true, thus rule 8 is not satisfied.

2. Suppose the multiplication $cx$ is defined to produce $(cx_1, 0)$ instead of
   $(cx_1, cx_2)$. With the usual addition in $\mathbf{R}^2$, are the eight
   conditions satisfied?

_Solution:_

None of the addition rules (rules 1 through 4) are broken by this supposition.
The only rule that is broken is rule 5, which states that:

$$ 1x = x $$

Since the supposition states that $cx_2 = 0$ for any $cx$, which is not
generally true.

3.

a. Which rules are broken if we keep only the positive numbers $x > 0$ in
$\mathbf{R}^1$? Every $c$ must be allowed. The half-line is not a subspace.

_Solution:_

Since any scalar multiple $c$ is allowed, rules 3 and 4 are broken.

Rule 3 is broken because by the definition of the supposed subspace, only
positive numbers $x > 0$ (not $x \geq 0$) are allowed.

Rule 4 is broken since $x$ must be a positive number within the supposed
half-line subspace, and thus there cannot exist some unique vector $-x$ within
such a space where $x + (-x) = \mathbf{0}$.

b. The positive numbers with $x + y$ and $cx$ redefined to equal the usual $xy$
and $x^c$ _do_ satisfy the eight rules. Test rule 7 when $c = 3, x = 2, y = 1$.
(Then $x + y = 2$ and $cx = 8$.) Which number acts as the "zero vector"?

_Solution:_

_Test rule 7 when $c = 3, x = 2, y = 1$:_

By the supposition, $x + y = xy$ and $cx = x^c$.

Rule 7 states:

$$ c(x + y) = cx + cy $$

Substituting these values with our supposition values, we get:

$$ c(x + y) = (x + y)^c = x^c + y^c = cx + cy $$

Evaluating this, we get:

$$ c(x + y) = x^c + y^c = (x^c)(y^c) = cx + cy $$

$$ c(x + y) = x^c + y^c = (x + y)^c = cx + cy $$

And this equality holds, thus Rule 7 is satisfied.

_Which number acts as the "zero vector"?:_

To find this, consider the fact that Strang makes it clear that this is a valid
subspace, thus all the suppositions for $c, x, y$ will follow all 8 rules.

Since we are looking for a "zero vector", consider rule 3, which states that
$x + \mathbf{0} = x$ for all $x$. $$ x + \text{some vector} = x $$

With the suppositions' custom addition, we know that $x + y = xy$, thus:

$$ x + \text{some vector} = x \cdot \text{some vector} $$

As unintuitive as it sounds, this means that $x = 1$. This is because
$x \cdot 1 = x$, and in this subspace, by the supposition, $x + 1 = x \cdot 1$.

_Note:_

Here, we are breaking many presumptions, $x$ and $y$ are simply positive numbers
that exist within $\mathbf{R}^1$, and the subspace is all positive numbers
within $\mathbf{R}^1$. They are _also vectors_ in this subspace and _also
vectors_ in $\mathbf{R}^1$. It is worth emphasizing that they _are NOT
coordinates in $\mathbf{R}^2$_.

4. The matrix $A = \left[\begin{array}{cc}2 & -2 \\2 & -2 \\\end{array}\right]$
   is a "vector" in the space $\mathbf{M}$ of all 2 by 2 matrices. Write down
   the zero vector in this space, the vector $\dfrac{1}{2}A$, and the vector
   $-A$. What matrices are in the smallest subspace containing $A$?

_Write down the zero vector in this space:_

$$
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

_the vector $\dfrac{1}{2}A$:_

$$ \frac{1}{2}A =
\frac{1}{2}
\left[\begin{array}{cc}
2 & -2 \\
2 & -2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & -1 \\
1 & -1 \\
\end{array}\right]
$$

_and the vector $-A$:_

$$ -A =
-1
\left[\begin{array}{cc}
2 & -2 \\
2 & -2 \\
\end{array}\right] =
\left[\begin{array}{cc}
-2 & 2 \\
-2 & 2 \\
\end{array}\right]
$$

_What matrices are in the smallest subspace containing $A$?:_

The smallest subspace containing $A$ is all matrices of the form $cA$ for any
scalar multiple $c$.

5.

a. Describe a subspace of $\mathbf{M}$ that contains
$A = \left[\begin{array}{cc}1 & 0\\0 & 0\\\end{array}\right]$ but not
$B = \left[\begin{array}{cc}0 & 0\\0 & -1\\\end{array}\right]$.

_Solution:_

Let $V$ represent the subspace of $M$ as defined above. Then, $V$ is defined as
all linear combinations of $A$, namely $cA$ for any scalar multiple, and $V$ is
defined as all solutions of $M$ that include $A$ but not $B$.

b. If a subspace of $\mathbf{M}$ does not contain $A$ and $B$, must it contain
$I$?

_Solution:_

Yes, since $A, B \in M$, and since $A + B$ is possible by the axioms of closure,
and because $c = -1$ is possible and $cB$ is possible it follows that:

$$ A + cB =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] +
(-1)\left[\begin{array}{cc}
0 & 0 \\
0 & -1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

And thus $I \in M$ as well.

c. Describe a subspace of $\mathbf{M}$ that contains no nonzero diagonal
matrices.

_Solution:_

This subspace would include all 2 x 2 real matrices with $0$'s along the main
diagonal.

6. The functions $f(x) = x^2$ and $g(x) = 5x$ are "vectors" in $\mathbf{F}$.
   This is the vector of all real functions. (The functions are defined for
   $-\infty < x < \infty$.) The combination $3f(x) - 4g(x)$ is the function
   $h(x) =$ ____.

_Solution:_

$$ h(x) = 3f(x) - 4g(x) $$

$$ = 3(x^2) - 4(5x) $$

$$ = 3x^2 - 20x $$

7. Which rule is broken if multiplying $f(x)$ by $c$ gives the function $f(cx)$?
   Keep the usual addition $f(x) + g(x)$.

_Solution:_

The supposition for this "space" claims:

$$ cf(x) = f(cx) $$

Consider rule 8:

$$ (c_1 + c_2)x = c_1x + c_2x $$

By the supposition, applying these terms from rule 8 on the left-hand side
results in:

$$ (c_1 + c_2)f(x) = f((c_1 + c_2)x) $$

Then on the right:

$$ c_1f(x) + c_2f(x) = f(c_1x) + f(c_2x) $$

For the supposition to hold, these two must be equal:

$$ f((c_1 + c_2)x) = f(c_1x) + f(c_2x) $$

But this is not generally true, and thus rule 8 is broken.

8. If the sum of the "vectors" $f(x)$ and $g(x)$ is defined to be the function
   $f(g(x))$, then the "zero vector" is $g(x) = x$. Keep the usual scalar
   multiplication $cf(x)$ and find two rules that are broken.

_Solution:_

By the supposition:

$$ f(x) + g(x) = f(g(x)) \to g(x) = x $$

And since $g(x) = x$ (_i.e._ the identity function), it follows that:

$$ f(g(x)) = f(x) $$

And therefore :

$$ f(x) + g(x) = f(x) $$

Similarly,

$$ g(x) + f(x) = g(f(x)) = g(x) $$

Rule 1 states:

$$ x + y = y + x $$

But as we have just demonstrated:

$$ f(x) + g(x) = f(x) $$

and:

$$ g(x) + f(x) = g(x) $$

Because it is not generally true that $f(x) = g(x)$, rule 1 has not been
satisfied.

Rule 7 states:

$$ c(x + y) = cx + cy $$

When applied to the left side we get:

$$ c(f(x) + g(x)) $$

By the supposition:

$$ c(f(x) + g(x)) = c(f(x)) $$

Then the right hand side:

$$ c(f(x)) + c(g(x)) $$

For rule 7 to hold, these two must be equal:

$$ c(f(x)) = c(f(x)) + c(g(x)) $$

But this is not generally true, thus rule 7 is not satisfied.

**Questions 9-18 are about the "subspace requirements": $x + y$ and $cx$ (and
then all linear combinations $cx + dy$) stay in the subspace.**

9. One requirement can be met while the other fails. Show this by finding

a. A set of vectors in $\mathbf{R}^2$ for which $x + y$ stays in the set but
$\dfrac{1}{2}x$ may be outside.

The set of all vectors of two integer components. $x + y$ will be an integer by
the sum of integers, but multiplying $\dfrac{1}{2}$ by any integer will result
in a fraction, which is not an integer

b. A set of vectors $\mathbf{R}^2$ (other than two quarter-planes) for which
every $cx$ stays in the set but $x + y$ may be outside.

The set of all vectors that lie on either the $x$ or $y$ axes, then any scalar
multiple of that vector will still lie on its respective axis, but adding two of
these vectors might result in a vector that lies on neither axes.

10. Which of the following subsets of $\mathbf{R}^3$ are actually subspaces?

a. The plane of vectors $(b_1, b_2, b_3)$ with $b_1 = b_2$.

This is a subspace, it simply includes all vectors where its two initial
components are equal.

b. The plane of vectors with $b_1 = 1$.

No, since $(0, 0, 0)$ must be in $\mathbf{R}^3$, a supposed subspace where the
initial component must be $1$ would not satisfy rules 3 and 4.

c. The vectors with $b_1b_2b_3 = 0$.

No, this violates the closure axioms, consider
$(1, 1, 0) + (0, 2, 1) = (1, 3, 1)$, where $1(1)(0) = 0, (0)(2)(1) = 0$, but
$1(3)(1) = 3 \neq 0$. For this to be a proper subspace $(1, 3, 1)$ would have to
also be in the set of vectors, but this is not possible under the definitions of
the supposed subspace.

d. All linear combinations of $v = (1, 4, 0)$ and $w = (2, 2, 2)$.

Yes, this is a proper subspace, which is defined being any vectors where for any
scalar multiples $c$ and $d$, $cv + dw$ is in the vector space, which it would
be.

e. All vectors that satisfy $b_1 + b_2 + b_3 = 0$.

Yes, this is a proper subspace, it does not violate any of the 8 rules nor does
it violate any axioms regarding $\mathbf{R}^3$. Notably, these vectors would
constitute as always being a plane through the origin.

f. All vectors with $b_1 \leq b_2 \leq b_3$.

No, consider $(1, 2, 3)$. Since this is supposedly a proper subspace in
$\mathbf{R}^3$, we should be able to scale this vector by any multiple and the
resulting vector should remain within the supposed subspace. So, consider
$c = -1$, then $c(1, 2, 3) = (-1, -2, -3)$, but $-1 > -2 > -3$, which violates
the supposition.

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

_Solution:_

All matrices of the form:

$$
\left[\begin{array}{cc}
a & b \\
0 & 0 \\
\end{array}\right]
$$

Where $a, b \in \mathbf{R}$.

b.

$$
\left[\begin{array}{cc}
1 & 1 \\
0 & 0 \\
\end{array}\right]
$$

_Solution:_

Any matrix of the form:

$$
\left[\begin{array}{cc}
a & a \\
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

_Solution:_

Any matrix of the form:

$$
\left[\begin{array}{cc}
a & 0 \\
0 & b \\
\end{array}\right]
$$

or all 2 by 2 diagonal matrices.

12. Let $P$ be the plane in $\mathbf{R}^3$ with equation $x + y - 2z = 4$. The
    origin $(0, 0, 0)$ is not in $P$! Find two vectors in $P$ and check that
    their sum is not in $P$.

_Solution:_

Choose $(8, 6, 5)$ and $(9, 5, 5)$, then:

$$ 8 + 6 - 2(5) = 4 $$

and:

$$ 9 + 5 - 2(5) = 4 $$

Now:

$$ (8, 6, 5) + (9, 5, 5) = (17, 11, 10) $$

But $(17) + 11 - 2(10) = 8 \neq 4$.

_Note:_ $P$ is not a subspace.

13. Let $\mathbf{P}_0$ be the plane through $(0, 0, 0)$ parallel to the previous
    plane $P$. What is the equation for $\mathbf{P}_0$? Find two vectors in
    $\mathbf{P}_0$ and check that their sum is in $\mathbf{P}_0$.

_Solution:_

For $\mathbf{P}_{0}$ to be parallel to the previous plane $P$ (from problem 12),
it must both satisfy $x + y - 2z$, but it must go through the origin
$(0, 0, 0)$. Thus every vector in $\mathbf{P}_{0}$ must satisfy
$x + y - 2z = 0$.

Choose $(9, 3, 6)$ and $(4, 6, 5)$, then:

$$ 9 + 3 - 2(6) = 0 $$

and

$$ 4 + 6 - 2(5) = 0 $$

then:

$$ (9, 3, 6) + (4, 6, 5) = (13, 9, 11) $$

and:

$$ 13 + 9 - 2(11) = 0 $$

_Note:_ $\mathbf{P}_{0}$ is a subspace.

14. The subspaces of $\mathbf{R}^3$ are planes, lines, $\mathbf{R}^3$ itself, or
    $\mathbf{Z}$ containing only $(0, 0, 0)$.

a. Describe the three types of subspaces of $\mathbf{R}^2$.

_Solution:_

The subspaces of $\mathbf{R}^2$ are lines through $(0, 0)$, $\mathbf{R}^2$
itself, or $\mathbf{Z}$ containing only $(0, 0)$.

b. Describe all subspaces of $\mathbf{D}$, the space of 2 by 2 diagonal
matrices.

_Solution:_

The subspaces of $\mathbf{D}$ are $\mathbf{D}$ itself, the 2 by 2 zero matrix
$\mathbf{0}$ by itself, and all one-dimensional subspaces that contain the fixed
matrix:

$$
c\left[\begin{array}{cc}
d_1 & 0 \\
0 & d_2 \\
\end{array}\right]
$$

for all scalar multiples $c$.

15.

a. The intersection of two planes through $(0, 0, 0)$ is probably a ____ in
$\mathbf{R}^3$ but it could be a ____. It can't be $\mathbf{Z}$!

_Solution:_

probably a line; could be a plane.

b. The intersection of a plane through $(0, 0, 0)$ with a line through
$(0, 0, 0)$ is probably a ____ but it could be a ____.

point; line

c. If $\mathbf{S}$ and $\mathbf{T}$ are subspaces of $\mathbf{R}^5$, prove that
their intersection $\mathbf{S} \cap \mathbf{T}$ is a subspace of $\mathbf{R}^5$.
Here $\mathbf{S} \cap \mathbf{T}$ consists of the vectors that lie in both
subspaces. _Check that $x + y$ and $cx$ are in $\mathbf{S} \cap \mathbf{T}$ if
$x$ and $y$ are in both spaces._

**Proof:**

Suppose $\mathbf{S}$ and $\mathbf{T}$ are both subspaces of $\mathbf{R}^5$.

It is to be shown that $\mathbf{S} \cap \mathbf{T}$ is a subspace of
$\mathbf{R}^5$.

Let $x, y \in \mathbf{S} \cap \mathbf{T}$.

Since $x$ and $y$ are in both $\mathbf{S}$ and $\mathbf{T}$ (by the definition
of $\cap$), and since both $\mathbf{S}$ and $\mathbf{T}$ are both subspaces of
$\mathbf{R}^{5}$ (by the supposition), it follows that the vector addition
$x + y$ and the scalar multiple of $cx$ and $dy$ for any scalar multiples $c$
and $d$ are also vectors in the subspace of $\mathbf{S}$ and $\mathbf{T}$, or,
more succinctly, in $\mathbf{S} \cap \mathbf{T}$.

This means that $\mathbf{S} \cap \mathbf{T}$ is a subspace of $\mathbf{R}^5$,
which is what was to be shown.

Q.E.D.

16. Suppose $\mathbf{P}$ is a plane through $(0, 0, 0)$ and $\mathbf{L}$ is a
    line through $(0, 0, 0)$. The smallest vector space containing both
    $\mathbf{P}$ and $\mathbf{L}$ is either ____ or ____.

_Solution:_

a plane (when $\mathbf{L} \in \mathbf{P}$); all of $\mathbf{R}^3$ (when
$\mathbf{L} \notin \mathbf{P}$).

17.

a. Show that the set of _invertible_ matrices in $\mathbf{M}$ is not a subspace.

**Proof (by contradiction):**

Suppose $\mathbf{I}$ is the set of all invertible matrices in the set of all 2
by 2 matrices $\mathbf{M}$.

A contradiction is to be derived to demonstrate that $\mathbf{I}$ is not a
subspace.

For $\mathbf{I}$ to be a subspace of $\mathbf{M}$, it follows that the zero
matrix:

$$
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

which is in $\mathbf{M}$, must also be in $\mathbf{I}$.

But by the definition for $\mathbf{I}$, this means that the zero matrix must be
invertible. It follows that the zero matrix must have a determinant that does
not equal $0$ (by the definition for invertible matrices). But the determinant
for the zero matrix is $0$ (by the formula for the determinant on 2 by 2
matrices), and thus the zero matrix is not in $\mathbf{I}$.

This demonstrates that there exists at least one matrix in $\mathbf{M}$ (namely
the zero matrix), that does not exist in the supposed subspace $\mathbf{I}$, and
therefore $\mathbf{I}$ is not a subspace, which contradicts the supposition.

Since a contradiction to the supposition has been derived, it can be concluded
that the supposition is false and that $\mathbf{I}$ is not a subspace.

Q.E.D.

b. Show that the set of _singular_ matrices in $\mathbf{M}$ is not a subspace.

**Proof (by contradiction):**

Suppose $\mathbf{S}$ is the set of singular matrices in the space of all 2 by 2
matrices, $\mathbf{M}$.

A contradiction is to be derived to prove that $\mathbf{S}$ is not a subspace.

Let $A, B \in \mathbf{S}$, and define them as:

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] \quad
B =
\left[\begin{array}{cc}
0 & 1\\
0 & 0 \\
\end{array}\right]
$$

Now, both $A$ and $B$ are indeed in $\mathbf{S}$ as their respective
determinants are $0$, and both $A$ and $B$ are in $\mathbf{M}$ since they are
both 2 by 2 matrices.

By the definition for subspaces, it follows that $A + B \in \mathbf{S}$:

$$ A + B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
0 & 0\\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

But the resulting matrix (the identity matrix) is not in $\mathbf{S}$, because
it's determinant is not $0$, and this means that $\mathbf{S}$ is not a subspace,
which is a contradiction.

Since a contradiction to the supposition has been derived, it can be concluded
that $\mathbf{S}$ is not a subspace.

Q.E.D.

18. True or false (check addition in each case by an example):

a. The symmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} = A$) form a
subspace.

True, since $A^{\mathbf{T}} = A$ does not cause any of $A^\mathbf{T}$'s vector's
to violate any of the 8 general rules for subspaces, and since
$A^{\mathbf{T}}$'s rows and column count does not change from being 2 by 2 (thus
$A^{\mathbf{T}} \in \mathbf{M}$), it follows that all matrices where
$A^{\mathbf{T}} = A$ is a subspace of $\mathbf{M}$.

For the addition, let $A + B$ be in the defined subspace, we have to show that
$(A + B)^{\mathbf{T}}$ is also in the defined subspace.

$$ (A + B)^{\mathbf{T}} = A^{\mathbf{T}} + B^{\mathbf{T}} $$

Now, by the supposition of the subspace, $A^{\mathbf{T}} = A$, and
$B^{\mathbf{T}} = B$, so:

$$ = A + B $$

Which is in the defined subspace.

b. The skew-symmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} = -A$) form
a subspace.

True, this is a subspace. Any matrix of the form:

$$ A =
\left[\begin{array}{cc}
0 & a \\
-a & 0 \\
\end{array}\right]
$$

Will yield:

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & -a \\
a & 0 \\
\end{array}\right]
$$

and:

$$ -A =
\left[\begin{array}{cc}
0 & -a \\
a & 0 \\
\end{array}\right] = A^{\mathbf{T}}
$$

For the addition, suppose $A + B$ is in the defined subspace, and show that
$(A + B)^{\mathbf{T}} = -(A + B)$ is also in the defined subspace.

$$ (A + B)^{\mathbf{T}} = A^{\mathbf{T}} + B^{\mathbf{T}} $$

$$ = -A + (-B) = -A - B $$

and the right side of the proposed equality is:

$$ -(A + B) $$

$$ -A - B $$

The two sides are equal, so $(A + B)^{\mathbf{T}}$ and $-(A + B)$ are in the
subspace, and it can be concluded that the supposed subspace is indeed a
subspace.

c. The unsymmetric matrices in $\mathbf{M}$ (with $A^{\mathbf{T}} \neq A$) form
a subspace.

False.

Consider two unsymmetric 2 by 2 matrices:

$$ A =
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
0 & -1 \\
1 & 0 \\
\end{array}\right]
$$

Both are unsymmetric since:

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & -1 \\
1 & 0 \\
\end{array}\right] \neq A
$$

and

$$ B^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right] \neq B
$$

However, when added:

$$ A + B =
\left[\begin{array}{cc}
0 & 1 \\
-1 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
0 & -1 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

And $\mathbf{0}$ is symmetric since $\mathbf{0}^{\mathbf{T}} = \mathbf{0}$. Thus
$\mathbf{0}$ is not in the supposed subspace, while both $A$ and $B$ are. It can
be concluded that the supposed subspace is not a subspace.

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

_Solution:_

_First:_

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

The column space $C(A)$ is a line along the $x$-axis in $\mathbf{R}^3$, defined
by $c(x, 0, 0)$ for all $c$.

_Second:_

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
0 & 2 \\
0 & 0 \\
\end{array}\right]
$$

$C(B)$ is the $xy$ plane in $\mathbf{R}^3$ where $z = 0$.

_Third:_

$$ C =
\left[\begin{array}{cc}
1 & 0 \\
2 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$C(C)$ is a line of vectors in $\mathbf{R}^3$ where each vector is $c(1, 2, 0)$,
for all $c$.

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

_Solution:_

$$
2x_1 + 8x_2 + 4x_2 = b_2 \\
-x_1 - 4x_2 - 2x_3 = b_3 \\
$$

$$
(-x_1 - 4x_2 - 2x_3 = b_3) + \\
\frac{1}{2}(2x_1 + 8x_2 + 4x_2 = b_2)
\\ \Rightarrow 0 = b_3 + \frac{1}{2}b_2 \\
\Rightarrow b_3 = -\frac{1}{2}b_2
$$

and:

$$
x_1 + 4x_2 + 2x_3 = b_1 \\
2x_1 + 8x_2 + 4x_2 = b_2
$$

$$ (x_1 + 4x_2 + 2x_3 = b_1) \\

- \frac{1}{2}(2x_1 + 8x_2 + 4x_2 = b_2) \\ \Rightarrow 0 = b_1 - \frac{1}{2}b_2
  \\ \Rightarrow b_1 = \frac{1}{2}b_2 $$

Put together this means:

$$
b_1 =\frac{1}{2}b_2
b_3 = -\frac{1}{2}b_2
$$

Or:

$$ b_2 = 2b_1 = -2b_3 $$

This equality must hold for there to be a solution to the given systems. :

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

_Solution:_

$$
\left[\begin{array}{cc|c}
1 & 4 & b_1 \\
2 & 9 & b_2 \\
-1 & -4 & b_3 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|c}
1 & 4 & b_1 \\
0 & 1 & b_2 \\
-1 & -4 & b_3 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc|c}
1 & 4 & b_1 \\
0 & 1 & b_2 - 2b_1 \\
0 & 0 & b_3 + b_1 \\
\end{array}\right]
$$

So $b_1 = -b_3$ must hold for the system to be solvable.

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

_Solution:_

First and foremost, express the combination of the columns of $A$ generally:

$$ c_1\begin{bmatrix}{}1\\2\end{bmatrix} + c_2\begin{bmatrix}{}2\\4\end{bmatrix} $$

Note that since $\begin{bmatrix}{}2\\4\end{bmatrix}$ is just
$2\begin{bmatrix}{}1\\2\end{bmatrix}$, this is a line through
$\begin{bmatrix}{}1\\2\end{bmatrix}$.

A combination of the columns of $C$ is generally expressed as:

$$ c_1\begin{bmatrix}{}1\\2\end{bmatrix} + c_2\begin{bmatrix}{}3\\6\end{bmatrix} $$

Note that $\begin{bmatrix}{}3\\6\end{bmatrix}$ is just
$3\begin{bmatrix}{}1\\2\end{bmatrix}$, and thus $C$ is also a line through
$\begin{bmatrix}{}1\\2\end{bmatrix}$.

Thus all linear combinations of the columns of $C$ are also combinations of
columns of $A$ since they both lie on the same line.

Thus both $A$ and $C$ have the same column space.

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
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

_Solution:_

_First:_

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

This is already in upper triangular form with a nonzero solution for
$x_3 = b_3$, thus this system is solvable for all $b$.

_Second:_

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

This system is already in upper triangular, but with $0x_3 = b_3$, so there is
only a solution when $b_3 = 0$.

_Third:_

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 0 & 1 \\
0 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix}
$$

This is already in upper triangular, but with $x_2 = b_2$ and $x_3 = b_3$, this
is only solvable when $b_2 = b_3$ (since both the second and third row are
identical).

23. (Recommended) If we add an extra column $b$ to a matrix $A$, then the column
    space gets larger unless ____. Give an example where the column space gets
    larger and an example where it doesn't. Why is $Ax = b$ solvable exactly
    when the column space _doesn't_ get larger - it is the same for $A$ and
    $\left[\begin{array}{cc}A & b\\\end{array}\right]$?

_Solution:_

$b$ is already in the column space.

Consider the following example where the column space gets larger:

$$
\left[\begin{array}{c|c}
A & b \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 2 & 3 \\
2 & 4 & 9 \\
\end{array}\right]
$$

Consider the following example where the column space doesn't gets larger:

$$
\left[\begin{array}{c|c}
A & b \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 2 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

Now, let's address why $Ax = b$ remains solvable if the column space doesn't get
larger. If we add a vector whose column space is a linear combination that is
the same as another vector's within the existing matrix to which it is being
added, then that vector lies on the same line and/or plane of another vector and
can simply be expressed as some scalar or linear combination of the existing
columns.

On the other hand, $Ax = b$ is definitively not solvable if the column space
does get larger. In this case, the new vector being added to the matrix cannot
be expressed as some linear combination of one of the previous columns, and thus
the solution for this new matrix cannot exist.

24. The column of $AB$ are combinations of the columns of $A$. This means: _The
    column space of $AB$ is contained in_ (possible equal to) _the column space
    of_ $A$. Give an example where the column spaces of $A$ and $AB$ are not
    equal.

_Solution:_

$$ A =
\left[\begin{array}{cc}
1 & 3 \\
2 & 6 \\
\end{array}\right]
$$

Then $A$ has the column space where ever vector is
$c\begin{bmatrix}{}1\\2\end{bmatrix}$ for any $c$.

$$ B =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ AB =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

Here $AB$ is not in the same column space as $A$, as $\mathbf{0}$, while a
subset of $C(A)$, only has the column space of $\Z$, and does not span the
entire $C(A)$.

25. Suppose $Ax = b$ and $Ay = b^*$ are both solvable. Then $Az = b + b^*$ is
    solvable. What is $z$? This translates into: If $b$ and $b^*$ are in the
    column space $C(A)$, _then_ $b + b^*$ is in $C(A)$.

_Solution:_

If $Ax = b$ and $Ay = b^*$ are both solvable, and the claim is that
$Ax = b + b^*$ is also solvable, then $z = x + y$ since
$A(x + y) = Ax + Ay = b + b^*$.

26. If $A$ is any 5 by 5 invertible matrix, then its column space is ____. Why?

The whole of $\R^5$. Since $Ax = b$ is solvable by $x = A^{-1}b$, this spans all
of $\R^5$.

27. True or false (with a counterexample if false):

a. The vectors $b$ that are not in the column space $C(A)$ form a subspace.

False. Since $C(A)$ is by definition a subspace, and any subspace includes
$\mathbf{0}$, then $b$ does not occupy $C(A)$, and thus does not include
$\mathbf{0}$, which contradicts rule 3 of the general rules for vector spaces.

b. If $C(A)$ contains only the zero vector, then $A$ is the zero matrix.

True, this means that $C(A) = \Z$, and by definition of $\Z$, the only vector
that spans $\Z$ is the zero vector, thus if $C(A)$, then $A = \mathbf{0}$.

c. The column space of $2A$ equals the column space of $A$.

True, this is simply scaling $A$ by $2$, so any vector that spans $C(A)$ also
spans $C(2A)$.

d. The column space of $A - I$ equals the column space of $A$ (test this).

False. Consider:

$$ A - I =
\left[\begin{array}{cc}
1 & 3 \\
2 & 6 \\
\end{array}\right] -
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 3 \\
2 & 5 \\
\end{array}\right]
$$

Note that $C(A)$ lies on the line of the vector $(1, 2)$, but $C(A - I)$ does
not.

28. Construct a 3 by 3 matrix whose column space contains $(1, 1, 0)$ and
    $(1, 0, 1)$ but not $(1, 1, 1)$. Construct a 3 by 3 matrix whose column
    space is only a line.

_Solution:_

_Construct a 3 by 3 matrix whose column space contains $(1, 1, 0)$ and
$(1, 0, 1)$ but not $(1, 1, 1)$:_

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

Directly, $C(A)$ has $(1, 1, 0)$ and $(1, 0, 1)$, but does not have $(1, 1, 1)$.
This follows from the following evaluation:

$$ c_1(1, 1, 0) + c_2(1, 0, 1) = (c_1 + c_2, c_1, c_2) $$

If set this vector next to $(1, 1, 1)$:

$$
\begin{bmatrix}{}c_1 +c_2\\c_1\\c_2\end{bmatrix} =
\begin{bmatrix}{}1\\1\\1\end{bmatrix}
$$

We easily see there is no solution, as $c_1 = 1, c_2 = 1$, which means that
$c_1 + c_2 \neq 1$. Since there is no solution, it can be concluded that
$(1, 1, 1)$ is not in $C(A)$.

_Construct a 3 by 3 matrix whose column space is only a line:_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 2 & 3 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Here, $C(A)$ spans a line through $(1, 1, 0)$.

29. If the 9 by 12 system $Ax = b$ is solvable for every $b$, then $C(A) =$
    ____.

_Solution:_

$\R^9$
