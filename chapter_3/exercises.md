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

---

Page 153

## Problem Set 3.2

1. Reduce $A$ and $B$ to their triangular echelon forms $U$. Which variables are
   free?

a.

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
1 & 2 & 3 & 6 & 9 \\
0 & 0 & 1 & 2 & 3 \\
\end{array}\right]
$$

_Solution:_

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
1 & 2 & 3 & 6 & 9 \\
0 & 0 & 1 & 2 & 3 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 1 & 2 & 3 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivot variables are $x_1, x_3$, free variables are $x_2, x_4, x_5$.

b.

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 8 & 8 \\
\end{array}\right]
$$

_Solution:_

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 8 & 8 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivots are $x_1, x_2$ and free variables are $x_3$.

2. For the matrices in Problem 1, find a special solution for each free
   variable. (Set the free variable to $1$. Set the other free variables to
   zero.)

_Solution:_

a.

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivot variables are $x_1, x_3$, free variables are $x_2, x_4, x_5$.

So, set $x_2 = 1, x_4 = 0, x_5 = 0$:

$$ 1x_3 + 2x_4 + 3x_5 = 0 \Rightarrow  1x_3 + 2(0) + 3(0) = 0 \Rightarrow x_3 = 0 $$

$$ x_1 + 2x_2 + 2x_3 + 4x_4 + 6x_5 = 0 \Rightarrow x_1 + 2(1) + 2(0) + 4(0) + 6(0) = 0 \Rightarrow x_1 + 2 = 0 \Rightarrow x_1 = -2 $$

$$ s = \begin{bmatrix}{}-2\\1\\0\\0\\0\end{bmatrix} $$

b.

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivots are $x_1, x_2$ and free variables are $x_3$.

Pick $x_3 = 1$, then:

$$ 4x_2 + 4x_3 = 0 \Rightarrow 4x_2 + 4(1) = 0 \Rightarrow 4x_2 = -4 \Rightarrow x_2 = -1 $$

$$ 2x_1 + 4x_2 + 2x_3 = 0 \Rightarrow 2x_1 + 4(-1) + 2(1) = 0 \Rightarrow 2x_1 - 4 + 2 = 0 \Rightarrow 2x_1 - 2 = 0 \Rightarrow 2x_1 = 2 \Rightarrow x_1 = 1 $$

$$ s = \begin{bmatrix}{}1\\-1\\1\end{bmatrix} $$

3. By further row operations on each $U$ in Problem 1, find the reduced echelon
   form $R$. _True or flase with a reason:_ The nullspace of $R$ equals the
   nullspace of $U$.

_Solution:_

a.

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivot variables are $x_1, x_3$, free variables are $x_2, x_4, x_5$.

_Find reduced row echelon matrix $R$ (by both/either use pivot rows to eliminate
upward in $R$/divide the whole pivot row by its pivot.):_

$$ U =
\left[\begin{array}{ccccc}
1 & 2 & 2 & 4 & 6 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

Subtract 2 times row 2 from row 1:

$$ R =
\left[\begin{array}{ccccc}
1 & 2 & 0 & 0 & 0 \\
0 & 0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

_True or false with a reason. The nullspace of $R$ equals the nullspace of $U$:_

Yes, the nullspace of $R$ equals the nullspace of $U$ as throughout the
evaluation that gets us from $U$ to $R$, at no point does the values for any
$x_j$ change relations to any other $x_j$. (This is because all row operations
remain invertible).

b.

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

Pivots are $x_1, x_2$ and free variables are $x_3$.

Find $R$:

$$ B =
\left[\begin{array}{ccc}
2 & 4 & 2 \\
0 & 4 & 4 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

Divide row 1 by 2:

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 1 \\
0 & 4 & 4 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Divide row 2 by 4:

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 1 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Subtract 2 times row 2 from row 1:

$$ R =
\left[\begin{array}{rrr}
1 & 0 & -1 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

_True or false with a reason. The nullspace of $R$ equals the nullspace of $U$:_

Yes, the nullspace of $R$ equals the nullspace of $U$ as throughout the
evaluation that gets us from $U$ to $R$, at no point does the values for any
$x_j$ change relations to any other $x_j$. (This is because all row operations
remain invertible).

4. For the same $A$ and $B$, find the special solutions to $Ax = \mathbf{0}$ and
   $Bx = \mathbf{0}$. For an $m$ by $n$ matrix, the number of pivot variables
   plus the number of free variables is ____. This is the **Counting Theorem:**
   $r + (n - r) = n$.

a.

$$ A =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
-2 & 6 & 10 \\
\end{array}\right]
$$

_Solution:_

_For the same $A$ and $B$, find the special solutions to $Ax = \mathbf{0}$ and
$Bx = \mathbf{0}$:_

$$ A =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
-2 & 6 & 10 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{rrr}
1 & -3 & -5 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Choose $x_2 = 1$, then $x_3 = 0$ and:

$$ 1x_1 - 3x_2 - 5x_3 = 0 \Rightarrow x_1 - 3(1) - 5(0) = 0 \Rightarrow x_1 - 3 = 0 \Rightarrow x_1 = 3 $$

So, special solution $s_1$ is:

$$ s_1 = \begin{bmatrix}{}3\\1\\0\end{bmatrix} $$

Second special solution, choose $x_3 = 1$, then $x_2 = 0$ and:

$$ 1x_1 - 3x_2 - 5x_3 = 0 \Rightarrow x_1 - 3(0) - 5(1) = 0 \Rightarrow x_1 - 5 = 0 \Rightarrow x_1 = 5 $$

So, special solution $s_1$ is:

$$ s_2 = \begin{bmatrix}{}5\\0\\1\end{bmatrix} $$

b.

$$ B =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
-2 & 6 & 7 \\
\end{array}\right]
$$

_Solution:_

_For the same $A$ and $B$, find the special solutions to $Ax = \mathbf{0}$ and
$Bx = \mathbf{0}$:_

$$ B =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
-2 & 6 & 7 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrr}
-1 & 3 & 5 \\
0 & 0 & -3 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrr}
1 & -3 & -5 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{rrr}
1 & -3 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Pivot variables are $x_1, x_3$ and free variables are $x_2$.

Choose $x_2 = 1$, then:

$$ 1x_1 - 3x_2 + 0x_3 = 0 \Rightarrow x_1 - 3(1) + 0(0) = 0 \Rightarrow x_1 - 3 = 0 \Rightarrow x_1 = 3 $$

So, special solution $s$ is:

$$ s = \begin{bmatrix}{}3\\1\\0\end{bmatrix} $$

_Overall solution:_

_For an $m$ by $n$ matrix, the number of pivot variables plus the number of free
variables is (?):_

The number of pivot variables plus the number of free variables is equal to the
number of columns $n$.

**Questions 5-14 are about free variables and pivot variables.**

5. True or false (with reason if true or example to show it is false):

a. A square matrix has no free variables.

False, consider this square matrix:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 2 \\
3 & 5 & 5 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & -4 & -4 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Here we have pivots $x_1, x_2$ and free variable $x_3$.

b. An invertible matrix has no free variables.

True. Because an invertible matrix has a nonzero determinant, it follows that no
row goes to zero during elimination, resulting in there being no row without a
pivot, and thus there is no free variable.

c. An $m$ by $n$ matrix has no more than $n$ pivot variables.

True, since $n$ represents the amount of columns in the matrix, it follows that
there cannot be more than $n$ pivot variables after elimination.

d. An $m$ by $n$ matrix has no more than $m$ pivot variables.

True, since $m$ represents the amount of rows in the matrix, it follows that
there can't be more than $m$ pivot variables after elimination. (note that since
both parts \(c\) and (d) are true, this means that there can't be more than
$\text{min}(m, n)$ pivots).

6. Put as many $1$'s as possible in a 4 by 7 echelon matrix $U$ whose pivot
   columns are

a. $2, 4, 5$

_Solution:_

$$ U =
\left[\begin{array}{ccccccc}
0 & 1 & 1 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

b. $1, 3, 6, 7$

_Solution:_

$$ U =
\left[\begin{array}{ccccccc}
1 & 1 & 1 & 1 & 1 & 1 & 1 \\
0 & 0 & 1 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

c. $4$ and $6$

_Solution:_

$$ U =
\left[\begin{array}{ccccccc}
0 & 0 & 0 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

7. Put as many $1$'s as possible in a 4 by 8 _reduced_ echelon matrix $R$ so
   that the free columns are

a. $2, 4, 5, 6$

_Solution:_

$$ R =
\left[\begin{array}{cccccccc}
1 & 1 & 0 & 1 & 1 & 1 & 0 & 0 \\
0 & 0 & 1 & 1 & 1 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

b. $1, 3, 6, 7, 8$

_Solution:_

$$ R =
\left[\begin{array}{cccccccc}
0 & 1 & 1 & 0 & 0 & 1 & 1 & 1 \\
0 & 0 & 0 & 1 & 0 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

8. Suppose column 4 f a 3 by 5 matrix is all zero. Then $x_4$ is certainly a
   ____ variable. The special solution for this variable is the vector $x =$
   ____.

_Solution:_

free; $(0, 0, 0, 1, 0)$, because $1$ will multiply the zero column to give
$Ax = \mathbf{0}$.

9. Suppose the first and last columns of a 3 by 5 matrix are the same (not
   zero). Then ____ is a free variable. Find the special solution for this
   variable.

_Solution:_

$x_5$, since column 1 = column 5, x_5 will be reduced to 0 during elimination.
$s = (-1, 0, 0, 0, 1)$.

10. Suppose an $m$ by $n$ matrix has $r$ pivots. The number of special solutions
    is ____. The nullspace contains only $x = \mathbf{0}$ when $r =$ ____. The
    column space is all of $\R^m$ when $r =$ ____.

_Solution:_

The number of special solutions is $n - r$; the nullspace only contains
$x = \mathbf{0}$ when $r = n$; The column space is all of $R^m$ when $r = m$.

11. The nullspace of a 5 by 5 matrix contains only $x = \mathbf{0}$ when the
    matrix has ____ pivots. The column space is $\R^5$ when there are ____
    pivots. Explain why.

_Solution:_

$5$ pivots; $5$ pivots; This is because when we can solve $Ax = b$, every $b$ is
in the column space.

12. The equation $x - 3y - z = 0$ determines a plane in $\R^3$. What is the
    matrix $A$ in this equation? Which variables are free? The special solutions
    are ____ and ____.

_Solution:_

The matrix $A$ is:

$$ A =
\left[\begin{array}{rrr}
1 & -3 & -1 \\
\end{array}\right]
$$

The free variables are $x_2, x_1$.

The special solutions are $s_1 = (1, 0, 1), s_2 = (3, 1, 0)$

13. (Recommended) The plane $x - 3y - z = 12$ is parallel to $x - 3y - z = 0$.
    One particular point on this plane is $(12, 0, 0)$. All points on the plane
    have the form

$$
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
\begin{bmatrix}{}\\0\\0\end{bmatrix} +
y\begin{bmatrix}{}\\1\\0\end{bmatrix} +
z\begin{bmatrix}{}\\0\\1\end{bmatrix}
$$

_Solution:_

$$
\begin{bmatrix}{}x\\y\\z\end{bmatrix} =
x\begin{bmatrix}{}1\\0\\0\end{bmatrix} +
y\begin{bmatrix}{}3\\1\\0\end{bmatrix} +
z\begin{bmatrix}{}1\\0\\1\end{bmatrix}
$$

14. Suppose
    $\text{column } 1 + \text{column } 3 + \text{column } 5 = \mathbf{0}$ in a 4
    by 5 matrix with four pivots. Which column has no pivot? What is the special
    solution? Describe $N(A)$.

_Solution:_

Since $c_1, c_3, c_5$ sum to $0$, it means that column 5 cannot be a pivot
column since it is just a linear combination of columns 1 and 3,
$c_5 = -c_1 - c_3$, and since $c_5$ comes last in elimination, it follows that
this column cannot have a pivot.

The special solution then is $(1, 0, 1, 0, 1)$.

$N(A)$ simply contains all multiples of this special solution, which is just a
line in $\mathbf{R}^5$.

**Questions 15-22 ask for matrices (if possible) with specific properties.**

15. Construct a matrix for which $N(A) =$ all combinations of $(2, 2, 1, 0)$ and
    $(3, 1, 0, 1)$.

_Solution:_

$$ s_1 = \begin{bmatrix}{}2\\2\\1\\0 \end{bmatrix} $$

$$ s_2 = \begin{bmatrix}{}3\\1\\0\\1 \end{bmatrix} $$

Since $s_1$ has a $1$ in $x_3$ and $0$ in $x_4$, and $s_2$ has $0$ in $x_3$ and
a $1$ in $x_4$, this indicates there are free variables in $x_3, x_4$, and
pivots in $x_1, x_2$. Thus our row echelon matrix $R$ is:

$$ R =
\left[\begin{array}{cccc}
1 & 0 & -2 & -3 \\
0 & 1 & -2 & -1 \\
\end{array}\right]
$$

$A$ can be any 2 by 2 matrix times this $R$.

16. Construct $A$ so that $N(A) =$ all multiples of $(4, 3, 2, 1)$. Its rank is
    ____.

_Solution:_

Since the special solution is $(4, 3, 2, 1)$, we see there is no $0$ in our
solution, and so $1$ is where the free variable is in $R$.

$$ R =
\left[\begin{array}{rrrr}
1 & 0 & 0 & -4 \\
0 & 1 & 0 & -3 \\
0 & 0 & 1 & -2 \\
\end{array}\right]
$$

This is a line through the given solution vector.

17. Construct a matrix whose column space contains $(1, 1, 5)$ and $(0, 3, 1)$
    and whose nullspace contains $(1, 1, 2)$.

_Solution:_

Constructing the column space is simple:

$$
\left[\begin{array}{ccc}
1 & 0 & \\
1 & 3 & \\
5 & 1 & \\
\end{array}\right]
$$

Now, adding the nullspace means we need $Ax = \mathbf{0}$ when $x = (1, 1, 2)$.

So we need column 1 + column 2 + column 3 = 0:

$$ 1c_1 + 1c_2 + 2c_3 = 0 $$

$$ 1(1) + 1(0) + 2c_3 = 0 $$

$$ 1 + 2c_3 = 0 $$

$$ 2c_3 = -1 $$

$$ c_3 = -\frac{1}{2} $$

$$
\left[\begin{array}{ccc}
1 & 0 & -\frac{1}{2} \\
1 & 3 & \\
5 & 1 & \\
\end{array}\right]
$$

Now the other entry:

$$ 1c_1 + 1c_2 + 2c_3 = 0 $$

$$ 1(1) + 1(3) + 2c_3 = 0 $$

$$ 1 + 3 + 2c_3 = 0 $$

$$ 4 + 2c_3 = 0 $$

$$ 2c_3 = -4 $$

$$ c_3 = -2 $$

$$
\left[\begin{array}{ccc}
1 & 0 & -\frac{1}{2} \\
1 & 3 & -2 \\
5 & 1 & \\
\end{array}\right]
$$

$$ 1c_1 + 1c_2 + 2c_3 = 0 $$

$$ 1(5) + 1(1) + 2c_3 = 0 $$

$$ 5 + 1 + 2c_3 = 0 $$

$$ 6 + 2c_3 = 0 $$

$$ 2c_3 = -6 $$

$$ c_3 = -3 $$

$$ A =
\left[\begin{array}{ccc}
1 & 0 & -\frac{1}{2} \\
1 & 3 & -2 \\
5 & 1 & -3 \\
\end{array}\right]
$$

18. Construct a matrix whose column space contains $(1, 1, 0)$ and $(0, 1, 1)$
    and whose nullspace contains $(1, 0, 1)$ and $(0, 0, 1)$.

_Solution:_

Examining the special solutions in the nullspace we find $(1, 0, 1)$ and
$(0, 0, 1)$:

$(0, 0, 1)$:

Tells us there is a free variable in $x_3$.

$(1, 0, 1)$:

We cannot determine the free variable here as to find a free variable we must
set a 1 to the first free variable and a 0 everywhere else, but here we have
$(1,0,1)$.

The construction of this is impossible for a 3 by 3 matrix (and we cannot
construct a larger matrix since all columns given have 3 entries, or in other
words, 3 rows).

19. Construct a matrix whose column space contains $(1, 1, 1)$ and whose
    nullspace is the line of multiples of $(1, 1, 1, 1)$.

_Solution:_

Since the column space contains 3 rows, we know that the number of rows in $A$
is 3. Since the nullspace contains 4 entries in a single special solution, we
know that the amount of free variables is 1 (equal to the number of special
solutions), and we know that the number of pivots is 4 - (number of free
variables), so we have 3 pivots.

$$ R =
\left[\begin{array}{cccc}
1 & 0 & 0 & ? \\
0 & 1 & 0 & ? \\
0 & 0 & 1 & ? \\
\end{array}\right]
$$

We need to set the free variable $c_4$, whatever will cancel out the $1$'s to
give us our solution $0$:

$$ R =
\left[\begin{array}{cccc}
1 & 0 & 0 & -1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & -1 \\
\end{array}\right]
$$

This can be $A$.

20. Construct a 2 by 2 matrix whose nullspace equals its column space. This is
    possible.

_Solution:_

For the nullspace and column space to be the same, they must have the same
solutions or some linear combination of the same solutions.

Let's start off simple:

$$ A =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right]
$$

Here the column space is $(1, 1)$ and all linear combinations of that vector. If
we now eliminate to find $U$, we get:

$$ U =
\left[\begin{array}{cc}
1 & 1 \\
0 & 0 \\
\end{array}\right]
$$

We can set $x_2$ to anything, as it is a free variable so try $x_2 = 1$, then
$x_1 = -1$, and so our nullspace becomes $(-1, 1)$, which does not occupy the
same space as our column space of $(1, 1)$. Let's try:

$$ A =
\left[\begin{array}{rr}
-1 & -1 \\
1 & 1 \\
\end{array}\right]
$$

Here $C(A)$ is $(-1, 1)$, now eliminate:

$$ U =
\left[\begin{array}{rr}
-1 & -1 \\
0 & 0 \\
\end{array}\right]
$$

Set $x_2 = 1$, then
$-x_1 + -1(1) = 0 \Rightarrow -x_1 = 1 \Rightarrow x_1 = -1$. So nullspace is
$(-1, 1)$, so this is the same as our column space. All good.

21. Why does no 3 by 3 matrix have a nullspace that equals its column space?

_Solution:_

Recall that the complete solution to $Ax = \mathbf{0}$ is a combination of the
$n - r$ special solutions (where $n$ is the number of columns and $r$ is the
number of pivots).

This means the nullspace is $n - r$, but the number of vectors in the column
space is $r$, this leaves us with:

$$ \text{the number of solutions in the nullspace } = n - r = r = \text{the number of vectors in the column space} $$

So now, we know we have a 3 by 3 matrix, which means we have 3 columns, so
$n = 3$, then:

$$ 3 - r = r $$

$$ 3 = 2r $$

$$ r = \frac{3}{2} $$

Which is not possible, since the number of pivots is always a whole integer.

22. If $AB = 0$ then the column space of $B$ is contained in the ____ of $A$.
    Why?

nullspace;

The reason why is because after multiplication all $Ab_i = 0$, and this is in
the nullspace of $A$, by definition of what it means for a column to be in the
nullspace of a matrix.

23. The reduced form $R$ of a 3 by 3 matrix with randomly chosen entries is
    almost sure to be ____. What $R$ is virtually certain if the random $A$ is 4
    by 3?

$I$.

$$ R =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Note that when rows exceed columns, you don't quite get I, but a row of $0$'s
below is generated as you go from $U$ to $R$.

24. Show by example that these three statements are generally _false_:

a. $A$ and $A^{\mathbf{T}}$ have the same nullspace.

Briefly, this is false intuitively, taking the transpose of any matrix will
usually mix up the pivots and create a different nullspace.

$$ A =
\left[\begin{array}{cc}
2 & 1 \\
0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & \frac{1}{2} \\
0 & 0 \\
\end{array}\right]
$$

$$ N(A) = \left\{\begin{bmatrix}{}-\dfrac{1}{2}\\1\end{bmatrix}\right\} $$

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
2 & 0 \\
1 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cc}
2 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ N(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}0\\1\end{bmatrix}\right\}$$

So $N(A) \neq N(A^{\mathbf{T}})$.

b. $A$ and $A^{\mathbf{T}}$ have the same free variables.

$$ A =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

Free variables are $x_1$.

$$ A^{\mathbf{T}} =
\left[\begin{array}{cc}
0 & 0 \\
1 & 0 \\
\end{array}\right]
$$

Free variables are $x_2$.

c. If $R$ is the reduced form $\mathbf{rref}(A)$ then $R^{\mathbf{T}}$ is
$\mathbf{rref}(A^{\mathbf{T}})$.

Part (a) also demonstrated that this is not true.

25. If $N(A) =$ all multiples of $x = (2, 1, 0, 1)$, what is $R$ and what is its
    rank?

_Solution:_

$$  R =
\left[\begin{array}{rrrr}
1 & 0 & 0 & -2 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
$$

$R$ has 3 pivots (one free variable/special solution at $x_4$).

26. If the special solutions to $Rx = \mathbf{0}$ are in the columns of these
    nullspace matrices $N$, go backwards to find the nonzero rows of the reduced
    matrices $R$:

$$ N =
\left[\begin{array}{cc}
2 & 3 \\
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

and

$$ N =
\left[\begin{array}{c}
0 \\
0 \\
1 \\
\end{array}\right]
$$

and

$$ N =
\left[\begin{array}{c}
 \\
 \\
 \\
\end{array}\right]
$$

(empty 3 by 1).

_Solution:_

_First:_

$$ N =
\left[\begin{array}{cc}
2 & 3 \\
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

These are special solutions, so:

$$ s_1 = \begin{bmatrix}{}2\\1\\0\end{bmatrix} $$

$$ s_2 = \begin{bmatrix}{}3\\0\\1\end{bmatrix} $$

Free variables at $x_2, x_3$.

Note that in $R$, this means that $x_1$ must be expressed as a $1$, so:

$$ R =
\left[\begin{array}{ccc}
1 & c_2 & c_3 \\
\end{array}\right]
$$

If we choose $x_2 = 1$, then we are left with $s_1$, so:

$$ 2c_1 + 1c_2 + 0c_3 = 0 \Rightarrow 2(1) + 1c_2 + 0(0) = 0 \Rightarrow 2 + c_2 = 0 \Rightarrow c_2 = -2 $$

If we choose $x_3 = 1$a, then we are left with $s_2$, so:

$$ 3c_1 + 0c_2 + 1c_3 = 0 \Rightarrow 3(1) + 0(0) + 1c_3 = 0 \Rightarrow c_3 = -3 $$

Thus our final $R$ is:

$$ R =
\left[\begin{array}{ccc}
1 & -2 & -3 \\
\end{array}\right]
$$

_Second:_

$$ N =
\left[\begin{array}{c}
0 \\
0 \\
1 \\
\end{array}\right]
$$

We just have one solution in $N$, so:

$$ s_1 = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

Thus we have a free variable in $x_3$, and two pivot variables $x_1, x_2$. In
our $R$, we must have all pivots equal $1$, so $x_1 = 1, x_2 = 1$

$$ R =
\left[\begin{array}{ccc}
1 & c_{12} & c_{13} \\
0 & 1 & c_{23} \\
\end{array}\right]
$$

Starting in the second row, we have:

$$ 1x_2 + c_{23}x_3 = 0 $$

Since we have one solution, we know that $x_2 = 0, x_3 = 1$ , so:

$$ 1(0) + c_{23}(1) = 0 $$

$$ c_{23} = 0 $$

So our updated $R$ is:

$$ R =
\left[\begin{array}{ccc}
1 & c_{12} & c_{13} \\
0 & 1 & 0 \\
\end{array}\right]
$$

In the first row, we use our special solution again:

$$ c_{11}x_1 + c_{12}x_2 + c_{13}x_3 = 0 $$

$$ 1(0) + c_{12}(0) + c_{13}(1) = 0 $$

$$ c_{13} = 0 $$

Updated $R$ again:

$$ R =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

_Third:_

$$ N =
\left[\begin{array}{c}
 \\
 \\
 \\
\end{array}\right]
$$

(empty 3 by 1).

The nullspace is empty, or so it seems. Recall that all spaces contain
$\mathbf{0}$. So there is no special solution, but if there were, it would have
3 rows (since it is an empty 3 by 1). This tells us there are 3 pivots and no
free variables. Since $R$ must have a $1$ at the pivot after further
transformation from $U$, this means that:

$$ R =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I_3
$$

27.

a. What are the five 2 by 2 reduced matrices $R$ whose entries are all $0$'s and
$1$'s?

_Solution:_

$$ R =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

b. What are the eight 1 by 3 matrices containing only $0$'s and $1$'s? Are all
eight of them reduced echelon matrices $R$?

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
1 & 1 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
1 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
0 & 1 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
0 & 0 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
0 & 1 & 0 \\
\end{array}\right]
$$

All eight matrices are $R$'s

28. Explain why $A$ and $-A$ always have the same reduced echelon form $R$.

_Solution:_

Because multiplying every entry of $A$ by $-1$ does not change the location of
the pivots, and ultimately does not change the outcome of the normalization
process of going from $A$ or $-A$ to $U$ to $R$.

29. If $A$ is 4 by 4 and invertible, describe the nullspace of the 4 by 8 matrix
    $B = \left[\begin{array}{cc}A & A \\\end{array}\right]$.

_Solution:_

First, establish $Bx$ where $x$ is some 8 by 1 vector, as equaling $0$ in order
to find the nullspace.

$$ Bx = \mathbf{0} $$

Since $B$ is simply two block matrices of identical 4 by 4 matrices $A$, we can
say that $B$ is the sum of two $A$ by two separate $x$ vectors (4 by 1 vectors):

$$ Ax_1 + Ax_2 = \mathbf{0} $$

$$ A(x_1 + x_2) = \mathbf{0} $$

Multiplying both sides by $A^{-1}$ yields:

$$ A^{-1}A(x_1 + x_2) = A^{-1}\mathbf{0} $$

$$ I(x_1 + x_2) = \mathbf{0} $$

$$ x_1 + x_2 = \mathbf{0} $$

Evaluating further reveals:

$$ x_1 = -x_2 $$

$$ x_2 = -x_1 $$

Thus all vectors $x$ are in the $N(B)$ of the form
$x = \begin{bmatrix}{}-x_2\\x_2\end{bmatrix}$ for $x_2 \in \mathbf{R}^4$.

30. How is the nullspace $N(C)$ related to the spaces $N(A)$ and $N(B)$, if
    $C = \left[\begin{array}{c}A \\B \\\end{array}\right]$?

_Solution:_

If $C(x) = \mathbf{0}$, then this means that $A(x) = \mathbf{0}$ and
$B(x) = \mathbf{0}$. In other words, the nullspace of $C$ is the intersection of
the nullspace of $A$ with the nullspace of $B$: $N(C) = N(A) \cap N(B)$.

31. Find the reduced row echelon forms $R$ and the rank of these matrices:

a. The 3 by 4 matrix with all entries equal to 4.

_Solution:_

$$ A =
\left[\begin{array}{cccc}
4 & 4 & 4 & 4 \\
4 & 4 & 4 & 4 \\
4 & 4 & 4 & 4 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccc}
4 & 4 & 4 & 4 \\
0 & 0 & 0 & 0 \\
4 & 4 & 4 & 4 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccc}
4 & 4 & 4 & 4 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

The rank of $A$ is 1, $r = 1$.

b. The 3 by 4 matrix with $a_{ij} = i + j - 1$.

_Solution:_

$$ A =
\left[\begin{array}{cccc}
1 & 2 & 3 & 4 \\
2 & 3 & 4 & 5 \\
3 & 4 & 5 & 6 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrr}
1 & 2 & 3 & 4 \\
0 & -1 & -2 & -3 \\
0 & -2 & -4 & -6 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrr}
1 & 2 & 3 & 4 \\
0 & -1 & -2 & -3 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrr}
1 & 2 & 3 & 4 \\
0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{rrrr}
1 & 0 & -1 & -2 \\
0 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

The rank of $A$ is $2$, $r = 2$.

c. The 3 by 4 matrix with $a_{ij} = (-1)^j$.

$$ A =
\left[\begin{array}{rrrr}
-1 & 1 & -1 & 1 \\
-1 & 1 & -1 & 1 \\
-1 & 1 & -1 & 1 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrr}
-1 & 1 & -1 & 1 \\
0 & 0 & 0 & 0 \\
-1 & 1 & -1 & 1 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrr}
-1 & 1 & -1 & 1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{rrrr}
1 & -1 & 1 & -1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

The rank of $A$ is $1$, $r = 1$.

32. Kirchhoff's Current Law $A^{\mathbf{T}}y = \mathbf{0}$ says that
    $\textit{current in } = \textit{ current out}$ at every node. At node 1 this
    is $y_3 = y_1 + y_4$. Write the four eequations for Kirchhoff's Law at the
    four nodes (arrows show the positive direction of each $y$). Reduce
    $A^{\mathbf{T}}$ to $R$ and find three special solutions in the nullspace of
    $A^{\mathbf{T}}$ (4 by 6 matrix).

(See Page 156 for graph.)

$$ A =
\left[\begin{array}{rrrr}
-1 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
1 & 0 & -1 & 0 \\
-1 & 0 & 0 & 1 \\
0 & -1 & 0 & 1 \\
0 & 0 & -1 & 1 \\
\end{array}\right]
$$

_Solution:_

At Node 1, one current, $y_3$, inputs, while at node 1, two currents output,
$y_1, y_4$, thus the equation at node 1 is $y_3 = y_1 + y_4$.

At Node 2, $y_1$ inputs, while $y_2, y_5$ output, so, the equation at node 2 is
$y_1 = y_2 + y_5$.

At node 3, $y_2 = y_3 + y_6$.

At node 4...this graph is wrong, nothing leaves node 4.

Omitted.

33. Which of these rules gives a correct definition of the _rank_ of $A$?

a. The number of nonzero rows in $R$.

This gives the rank of $A$, as these nonzero rows are guaranteed to have pivots
(which is what we are counting with rank/$r$).

b. The number of columns minus the total number of rows.

False.

c. The number of columns minus the number of free columns.

This gives the correct definition of the rank, as $r$ or rank, simply refers to
the total number of pivots in $A$, which can be calculated by taking the total
number of columns and subtracting the number of free columns.

d. The number of $1$'s in the matrix $R$.

False, there might be $1$'s in the nonpivot columns.

34. Find the reduced $R$ for each of these (block) matrices:

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
0 & 0 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
A & A \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{cc}
A & A \\
A & 0 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
0 & 0 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{ccc}
2 & 4 & 6 \\
0 & 0 & 3 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 6 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & 2 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

_Second:_

$$ B =
\left[\begin{array}{cc}
A & A \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cccccc}
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 3 \\
2 & 4 & 6 & 2 & 4 & 6 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccccc}
2 & 4 & 6 & 2 & 4 & 6 \\
0 & 0 & 3 & 0 & 0 & 3 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccccc}
2 & 4 & 6 & 2 & 4 & 6 \\
0 & 0 & 1 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccccc}
1 & 2 & 3 & 1 & 2 & 3 \\
0 & 0 & 1 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cccccc}
1 & 2 & 0 & 1 & 2 & 0 \\
0 & 0 & 1 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

_Third:_

$$ C =
\left[\begin{array}{cc}
A & A \\
A & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{cccccc}
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 3 \\
2 & 4 & 6 & 2 & 4 & 6 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 0 \\
2 & 4 & 6 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{cccccc}
2 & 4 & 6 & 2 & 4 & 6 \\
2 & 4 & 6 & 0 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 3 \\
0 & 0 & 3 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cccccc}
2 & 4 & 6 & 2 & 4 & 6 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 3 & 0 & 0 & 3 \\
0 & 0 & 3 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrrrr}
2 & 4 & 6 & 2 & 4 & 6 \\
0 & 0 & 3 & 0 & 0 & 3 \\
0 & 0 & 0 & 0 & 0 & -3 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{rrrrrr}
1 & 2 & 3 & 1 & 2 & 3 \\
0 & 0 & 1 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{rrrrrr}
1 & 2 & 0 & 1 & 2 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

35. Suppose all the pivot variables come _last_ instead of first. Describe all
    four blocks in reduced echelon form (the block $B$ should be $r$ by $r$):

$$ R =
\left[\begin{array}{cc}
A & B \\
C & D \\
\end{array}\right]
$$

What is the nullspace matrix $N$ containing the special solutions?

_Solution:_

If all the pivot variables come _last_ instead of first, then the reduced row
echelon form becomes:

$$ R =
\left[\begin{array}{cc}
0 & I \\
0 & 0 \\
\end{array}\right]
$$

The nullspace matrix $N$ containing the special solutions takes the form of:

$$ N =
\left[\begin{array}{c}
I \\
0 \\
\end{array}\right]
$$

36. (Silly problem) Describe all 2 by 3 matrices $A_1$ and $A_2$, with row
    echelon forms $R_1$ and $R_2$, such that $R_1 + R_2$ is the row echelon form
    ,of $A_1 + A_2$. Is it true that $R_1 = A_1$ and $R_2 = A_2$ in this case?
    Does $R_1 - R_2$ equal $\mathbf{rref}(A_1 -A_2)$?

Omitted. This problem simply demonstrates that row reduction doesn't distribute.

37. If $A$ has $r$ pivot columns, how do you know that $A^{\mathbf{T}}$ has $r$
    pivot columns? Give a 3 by 3 example with different column numbers in
    _pivcol_ for $A$ and $A^{\mathbf{T}}$.

_Solution:_

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

1 Pivots

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
1 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

1 Pivot

The point is that even when you transpose a matrix, the amount of pivots remain
the same.

38. What are the special solutions to $Rx = \mathbf{0}$ and
    $y^{\mathbf{T}}R = \mathbf{0}$ for these $R$?

$$ R =
\left[\begin{array}{cccc}
1 & 0 & 2 & 3 \\
0 & 1 & 4 & 5 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ R =
\left[\begin{array}{cccc}
1 & 0 & 2 & 3 \\
0 & 1 & 4 & 5 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ x_2 + 4x_3 + 5x_4 = 0 $$

Choose $x_3 = 1, x_4 = 0$:

$$ x_2 + 4(1) + 5(0) = 0 $$

$$ x_2 = -4 $$

Then:

$$ x_1 + 2x_3 + 3x_4 = 0 $$

$$ x_1 + 2(1) + 3(0) = 0 $$

$$ x_1 + 2 = 0 $$

$$ x_1 = -2 $$

$$ s_1 = \begin{bmatrix}{}-2\\-4\\1\\0\end{bmatrix} $$

Choose $x_3 = 0, x_4 = 1$:

$$ x_2 + 4(0) + 5(1) = 0 $$

$$ x_2 = -5 $$

$$ x_1 + 2(0) + 3(1) = 0 $$

$$ x_1 = -3 $$

$$ s_2 = \begin{bmatrix}{}-3\\-5\\0\\1\end{bmatrix} $$

Now:

$$ y^{\mathbf{T}}R = 0 $$

$$
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 2 & 3 \\
0 & 1 & 4 & 5 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cccc}
y_1 & y_2 & 2y_1 + 4y_2 & 3y_1 + 5y_2 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

$$
y_1 = 0 \\
y_2 = 0 \\
$$

$y_3$ is free, so:

$$ y_3 = 1 $$

Then, one (and only, since there was only one free variable) solution for $y$
is:

$$ y = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

_Second:_

$$ R =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ 0(x_1) + 1(x_2) + 2x_3 = 0 $$

Choose $x_1 = 1, x_3 = 0$:

$$ 0(1) + x_2 + 2(0) = 0 $$

$$ x_2 = 0 $$

$$ s_1 = \begin{bmatrix}{}1\\0\\0\end{bmatrix} $$

Choose $x_1 = 0, x_3 = 1$:

$$ 0(0) + x_2 + 2(1) = 0 $$

$$ x_2 = -2 $$

$$ s_2 = \begin{bmatrix}{}0\\-2\\1\end{bmatrix} $$

Now:

$$ y^{\mathbf{T}}R = \mathbf{0} $$

$$
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 2 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
\end{array}\right]
$$

$$ =
\left[\begin{array}{ccc}
0 & y_1 & 2y_1 \\
\end{array}\right]
$$

$$ y_1 = 0 $$

Free variables $y_2, y_3$.

Choose $y_2 = 1, y_3 = 0$, then:

$$ s_3 = \begin{bmatrix}{}0\\1\\0\end{bmatrix} $$

Choose $y_2 = 0, y_3 = 1$, then:

$$ s_4 = \begin{bmatrix}{}0\\0\\1\end{bmatrix} $$

39. Fill out these matrices so that they have rank 1:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 4 \\
2 & & \\
4 & & \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{rrr}
& 9 & \\
1 & & \\
2 & 6 & -3 \\
\end{array}\right]
$$

and

$$ M =
\left[\begin{array}{cc}
a & b \\
c & \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 4 \\
2 & 4 & 6 \\
4 & 8 & 16 \\
\end{array}\right]
$$

_Second:_

$$ B =
\left[\begin{array}{rrr}
3 & 9 & -\frac{1}{2} \\
1 & 3 & -\frac{3}{2} \\
2 & 6 & -3 \\
\end{array}\right]
$$

_Third:_

$$ M =
\left[\begin{array}{cc}
a & b \\
c & \frac{bc}{a} \\
\end{array}\right]
$$

40. If $A$ is an $m$ by $n$ matrix with $r = 1$, its columns are multiples of
    one column and its rows are multiples of one row. The column space is a ____
    in $\R^m$. The nullspace is a ____ in $\R^n$. The nullspace matrix $N$ has
    shape ____.

_Solution:_

line;plane;$n$ by $n - 1$ (with $n - 1$ being special special solutions in its
columns)

41. Choose vectors $u$ and $v$ so that $A = uv^{\mathbf{T}} =$ column times row:

$$ A =
\left[\begin{array}{ccc}
3 & 6 & 6 \\
1 & 2 & 2 \\
4 & 8 & 8 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{rrrr}
2 & 2 & 6 & 4 \\
-1 & -1 & -3 & -2 \\
\end{array}\right]
$$

$A = uv^{\mathbf{T}}$ _is the natural form for every matrix that has rank
$r = 1$_.

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
3 & 6 & 6 \\
1 & 2 & 2 \\
4 & 8 & 8 \\
\end{array}\right]
$$

Since $A$'s columns are all multiples of the first, this indicates that $u$ is a
vector that represents the fact that $A$ is rank 1. Thus $u$ can be represented
by this first column:

$$ u = \begin{bmatrix}{}3\\1\\4\end{bmatrix} $$

So, to get $uv^{\mathbf{T}} = A$, we need to multiply $u$ by some vector which
will give us $A$, it follows that we can multiply by the base row in $A$ that is
the base off of which the other rows are multiples, in this case that is row 2:

$$ v^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 2 & 2 \\
\end{array}\right]
$$

Thus:

$$ uv^{\mathbf{T}} =
\begin{bmatrix}{}3\\1\\4\end{bmatrix}
\left[\begin{array}{ccc}
1 & 2 & 2 \\
\end{array}\right] =
\left[\begin{array}{ccc}
3 & 6 & 6 \\
1 & 2 & 2 \\
4 & 8 & 8 \\
\end{array}\right] = A
$$

_Second:_

$$ A =
\left[\begin{array}{rrrr}
2 & 2 & 6 & 4 \\
-1 & -1 & -3 & -2 \\
\end{array}\right]
$$

Similar to the first:

$$ u = \begin{bmatrix}{}2\\-1\end{bmatrix} $$

And:

$$ v^{\mathbf{T}} =
\left[\begin{array}{rrrr}
1 & 1 & 3 & 2 \\
\end{array}\right]
$$

Note here we choose $v$ after we divide by $-1$ to get it into reduced form.

$$ uv^{\mathbf{T}} =
\begin{bmatrix}{}2\\-1\end{bmatrix}
\left[\begin{array}{rrrr}
1 & 1 & 3 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
2 & 2 & 6 & 4 \\
-1 & -1 & -3 & -2 \\
\end{array}\right] = A
$$

42. If $A$ is a rank one matrix, the second row of $R$ is ____. Do an example.

a zero row.

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 0 \\
\end{array}\right]
$$

**Problems 43-45 are about $r$ by $r$ invertible matrices inside $A$.**

43. _If $A$ has rank $r$, then it has an $r$ by $r$ submatrix $S$ that is
    invertible._ Remove $m - r$ rows and $n - r$ columns to find an invertible
    submatrix $S$ inside $A$, $B$, and $C$. You could keep the pivot rows and
    pivot columns:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 2 & 4 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
1 & 2 & 4 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & 2 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

Remove $m - r$ rows is remove $2 - 2 = 0$ rows, and $n - r$ columns is
$3 - 2 = 1$ columns to find an invertible submatrix inside $A$, $S$:

$$ S =
\left[\begin{array}{cc}
1 & 3 \\
1 & 4 \\
\end{array}\right]
$$

Notice we removed the pivot column.

_Second:_

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Remove $2 - 1 = 1$ rows and $3 - 1 = 2$ columns to find $S$.

$$ S =
\left[\begin{array}{c}
1 \\
\end{array}\right]
$$

_Third:_

$$ C =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Remove $3 - 2 = 1$ rows and $3 - 2 = 1$ columns to get $S$:

$$ S =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

44. Suppose $P$ contains only the $r$ pivot columns of an $m$ by $n$ matrix.
    Explain why this $m$ by $r$ submatrix $P$ has rank $r$.

_Solution:_

Since $P$ only contains the $r$ pivot columns from the original matrix,
elimination will produce the same pivot columns in $P$ as elimination did in the
original.

45. Transpose $P$ in Problem 44. Find the $r$ pivot columns of $P^{\mathbf{T}}$
    (which is $r$ by $m$). Transposing back, **this produces an $r$ by $r$
    invertible submatrix $S$ inside $P$ and $A$**:

For

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
2 & 4 & 7 \\
\end{array}\right]
$$

find $P$ (3 by 2) and then the invertible $S$ (2 by 2).

_Solution:_

_Find $P$ (3 by 2):_

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
2 & 4 & 7 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & 2 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Now find $P$ (only the $r$ pivot columns of $A$). Remove $n - r = 3 - 2 = 1$
(non pivot) columns of $A$, from $R$ we have.

$$ R =
\left[\begin{array}{ccc}
1 & 0 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

Now apply to $R$ to $A$ to find $P$:

$$ R =
\left[\begin{array}{ccc}
1 & 3 \\
2 & 6 \\
2 & 7 \\
\end{array}\right]
$$

_Find invertible $S$ (2 by 2):_

Remove the $m - r = 3 - 2 = 1$ rows:

$$ S =
\left[\begin{array}{ccc}
1 & 3 \\
2 & 7 \\
\end{array}\right]
$$

**Problems 46-51 show that rank $(AB)$ is not greater than rank $(A)$ or rank
$(B)$.**

46. Find the ranks of $AB$ and $AC$ (rank one matrix times rank one matrix):

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
2 & 1 & 4 \\
3 & 1.5 & 6 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{cc}
1 & b \\
c & bc \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ AB =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 4 \\
3 & 1.5 & 6 \\
\end{array}\right] =
\left[\begin{array}{ccc}
8 & 4 & 16 \\
16 & 8 & 32 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
8 & 4 & 16 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{ccc}
1 & \frac{1}{2} & 2 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ r_{AB} = 1 $$

_Second:_

$$ AC =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & b \\
c & bc \\
\end{array}\right] =
\left[\begin{array}{cc}
1 + 2c & b + 2bc \\
2 + 4c & 2b + 4bc \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{cc}
1 + 2c & b + 2bc \\
0 & 0 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & b \\
0 & 0 \\
\end{array}\right]
$$

$$ r_{AC} = 1 $$

47. The rank one matrix $uv^{\mathbf{T}}$ times the rank one matrix
    $wz^{\mathbf{T}}$ is $uz^{\mathbf{T}}$ times the number ____. This product
    $uv^{\mathbf{T}}wz^{\mathbf{T}}$ also has rank one unless ____ $= 0$.

_Solution:_

$$ (uv^{\mathbf{T}})(wz^{\mathbf{T}}) = uz^{\mathbf{T}} \cdot \text{(?)} $$

$$ u(v^{\mathbf{T}}w)z^{\mathbf{T}} = uz^{\mathbf{T}} \cdot \text{(?)} $$

Note here that $(v^{\mathbf{T}}w)$ is a scalar here, and thus the laws of
commutativity are fine to apply:

$$ u(v^{\mathbf{T}}w)z^{\mathbf{T}} = uz^{\mathbf{T}} \cdot v^{\mathbf{T}}w $$

This product has rank one unless $v^{\mathbf{T}}w = 0$.

48.

a. Suppose column $j$ of $B$ is a combination of previous columns of $B$. Show
that column $j$ of $AB$ is the same combination of previous columns of $AB$.
Then $AB$ cannot have new pivot columns, so
$\textbf{rank}(AB) \leq \textbf{rank}(B)$.

_Solution:_

By matrix multiplication, every column of $AB$ is a combination of the column of
$A$ times the corresponding column of $B$. Since column $j$ of $B$ is a
combination of the previous columns, it follows that when $B$ is multiplied by
$A$, that same column $j$ in $AB$ is the same combination of previous columns of
$AB$. Then $\text{rank}(AB) \leq \text{rank}(B)$, and so it follows that $AB$
cannot have any new pivot columns.

b. Find $A_1$ and $A_2$ so that $\text{rank}(A_1B) = 1$ and
$\text{rank}(A_2B) = 0$ for
$B =\left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$.

_Solution:_

$$ A_1B =
\left[\begin{array}{cc}
1 & 0 \\
1 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
3 & 3 \\
\end{array}\right]
$$

$$ \text{rank}(A_1B) = 1 $$

$$ A_2B =
\left[\begin{array}{cc}
1 & -1 \\
1 & -1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ \text{rank}(A_2B) = 0 $$

49. Problem 48 proved that $\text{rank}(AB) \leq \text{rank}(B)$. Then the same
    reasoning gives
    $\text{rank}(B^{\mathbf{T}}A^{\mathbf{T}}) \leq \text{rank}(A^{\mathbf{T}})$.
    How do you deduce that $\text{rank}(AB) \leq \text{rank}A$?

_Solution:_

Since transposes retain the same rank as their original matrices, it follows
that since
$\text{rank}(B^{\mathbf{T}}A^{\mathbf{T}}) \leq \text{rank}(A^{\mathbf{T}})$
that $\text{rank}(AB) \leq \text{rank}(A)$.

50. (Important) Suppose $A$ and $B$ are $n$ by $n$ matrices, and $AB = I$. Prove
    from $\text{rank}(AB) \leq \text{rank}(A)$ that the rank of $A$ is $n$. So
    $A$ is invertible and $B$ must be its two-sided inverse (Section 2.5).
    Therefore $BA = I$ (_which is not so obvious!_)

_Solution:_

**Proof:**

Suppose $A$ and $B$ are any two matrices of dimensions $n$ by $n$ (where $n$ is
an integer). Furthermore, suppose $AB = I$.

It is to be shown that the rank of $A$ is $n$ and that $BA = I$.

By matrix multiplication, it is known that $AB$ is an $n$ by $n$ matrix, and by
the supposition, since $AB = I$, it follows that
$\text{rank}(I) = \text{rank}(AB) = n$.

By problem 48, we know that $\text{rank}(AB) \leq \text{rank}(A)$, which forces
the rank of $A$ to be $n$.

Since $A$ is an $n$ by $n$ matrix of rank $n$, it follows that $A$ is
invertible.

Furthermore, by the definition for inverses, since $AB = I$, it follows that
$B = A^{-1}$, and this means that $B$ is $A$'s two-sided inverse.

It therefore follows that $BA = I$.

Q.E.D.

51. If $A$ is 2 by 3 and $B$ is 3 by 2 and $AB = I$, show from its rank that
    $BA \neq I$. Give an example of $A$ and $B$ with $AB = I$. For $m < n$, a
    right inverse is not a left inverse.

_Solution:_

**Proof:**

Suppose $A$ is a 2 by 3 matrix, $B$ is a 3 by 2 matrix, and $AB = I$.

It is to be shown that $BA \neq I$.

Since $A$ is a 2 by 3 matrix, it follows that $\text{rank}(A) \leq 2$.

Similarly, since $B$ is a 3 by 2 matrix, it follows that
$\text{rank}(B) \leq 2$.

It follows from problem 48 that $\text{rank}(AB) = \text{rank}(I) \leq 2$.

Now, by matrix multiplication, the dimensions of $BA$ are 3 by 3. By similar
logic, this means that $\text{rank}(BA) \leq 3$.

Now, by problem 48 again, we know that
$\text{rank}(BA) \leq \text{rank}(A) \leq 2$, which means that
$\text{rank}(BA) \leq 2 < 3$. Now, a 3 by 3 identity matrix has a rank of $3$,
and so it follows that
$\text{rank}(BA) \leq 2 \neq \text{rank}(I_{3 \times 3}) = 3$.

It can thus be concluded that $BA \neq I$.

This is what was to be shown.

Q.E.D.

Example:

$$ AB =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

52. Suppose $A$ and $B$ have the _same_ reduced row echelon form $R$.

a. Show that $A$ and $B$ have the same nullspace and the same row space.

_Solution:_

Since $A$ and $B$ have the same $R$, it follows that they have the same
nullspace (since the nullspace is derived from $R$), and they share the same row
space since row operations on either $A$ and $B$ do not change $R$.

b. We know $E_1A = R$ and $E_2B = R$. So $A$ equals an ____ matrix times $B$.

_Solution:_

invertible

53. Express $A$ and then $B$ as the sum of two rank one matrices:

$$ \textbf{rank} = 2 $$

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 4 \\
1 & 1 & 8 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
2 & 2 \\
2 & 3 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 4 \\
1 & 1 & 8 \\
\end{array}\right]
$$

$A = (\text{pivot columns})(\text{nonzero rows of } R) = uv^{\mathbf{T}}$

$$ R =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
1 & 4 \\
1 & 8 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 0 \\
1 & 1 & 0 \\
\end{array}\right] +
\left[\begin{array}{ccc}
0 & 0 & 0 \\
0 & 0 & 4 \\
0 & 0 & 8 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 4 \\
1 & 1 & 8 \\
\end{array}\right] = A
$$

_Second:_

$$ B =
\left[\begin{array}{cc}
2 & 2 \\
2 & 3 \\
\end{array}\right]
$$

$$ R =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{c}
2 & 2 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 0 \\
2 & 0 \\
\end{array}\right] +
\left[\begin{array}{cc}
0 & 2 \\
0 & 3 \\
\end{array}\right] = B
$$

54. Answer the same questions as in Worked Example 3.2C for

$$ A =
\left[\begin{array}{cccc}
1 & 1 & 2 & 2 \\
2 & 2 & 4 & 4 \\
1 & c & 2 & 2 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
1 - c & 2 \\
0 & 2 - c \\
\end{array}\right]
$$

Omitted.

55. What is the nullspace matrix $N$ (containing the special solutions) for
    $A, B, C$?

Block matrices

$$ A =
\left[\begin{array}{cc}
I & I \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
I & I \\
0 & 0 \\
\end{array}\right]
$$

and

$$ C =
\left[\begin{array}{ccc}
I & I & I \\
\end{array}\right]
$$

_Solution:_

$N(A) = \begin{bmatrix}{}I\\-I\end{bmatrix}, $N(B) = N(A)$$

$$ N(C) =
\left[\begin{array}{cc}
I & -I \\
I & 0 \\
0 & I \\
\end{array}\right]
$$

56. _Neat fact_ _Every $m$ by $n$ matrix of rank $r$ reduces to ($m$ by $r$)
    **times** ($r$ by $n$):_

> $A = (\text{pivot columns of } A)(\text{first } r \text{ rows of } R) = (\textbf{COL})(\textbf{ROW})$

Write the 3 by 4 matrix $A$ of all ones as the product of the 3 by 1 matrix from
the pivot columns and the 1 by 4 matrix from $R$.

Omitted.

---

Page 169

## Problem Set 3.3

1. (Recommended ) Execute the six steps of Worked Example 3.3A to describe the
   column space and nullspace of $A$ and the complete solution to $Ax = b$:

$$ A =
\left[\begin{array}{cccc}
2 & 4 & 6 & 4 \\
2 & 5 & 7 & 6 \\
2 & 3 & 5 & 2 \\
\end{array}\right]
$$

$$ b =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix} =
\begin{bmatrix}{}4\\3\\5\end{bmatrix}
$$

_Solution:_

Refer to the six steps here:

(1) Reduce $\left[\begin{array}{cc}A & b\\\end{array}\right]$ to
$\left[\begin{array}{cc}U & c\\\end{array}\right]$, so that $Ax = b$ becomes a
triangular system $Ux = c$.

(2) Find the condition on $b_1, b_2, b_3$ for $Ax = b$ to have a solution.

(3) Describe the column space of $A$. Which plane in $\R^3$?

(4) Describe the nullspace of $A$. Which special solutions in $\R^4$?

(5) Reduce $\left[\begin{array}{cc}U & c\\\end{array}\right]$ to
$\left[\begin{array}{cc}R & d\\\end{array}\right]$: Special solutions from $R$,
particular solution from $d$.

(6) Find a particular solution to $Ax = (0, 6, -6)$ and then the complete
solution.

_(1):_

Take $Ax = b$ to $Ux = c$:

$$ A =
\left[\begin{array}{cccc}
2 & 4 & 6 & 4 \\
2 & 5 & 7 & 6 \\
2 & 3 & 5 & 2 \\
\end{array}\right]
$$

$$ b =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix} =
\begin{bmatrix}{}4\\3\\5\end{bmatrix}
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc}
2 & 4 & 6 & 4 & b_1 \\
2 & 5 & 7 & 6 & b_2 \\
2 & 3 & 5 & 2 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{llll|l}
2 & 4 & 6 & 4 & b_1 \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & -1 & -1 & -2 & b_3 - b_1 \\
\end{array}\right] \to
\left[\begin{array}{llll|l}
2 & 4 & 6 & 4 & b_1 \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & 0 & 0 & 0 & b_3 + b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

_(2):_

For $Ax = b$ to have a solution, the last row indicates that the following
equality must hold: $b_3 + b_2 - 2b_1 = 0$, then $0 = 0$.

_(3):_

The column space is the plane containing all combinations of the pivot columns.
Here, that is specifically $(2, 2, 2)$ and $(4, 5, 3)$. The pivots are in
columns 1 and 2. Another description would be that the column space contains all
vectors with $b_3 + b_2 - 2b_1 = 0$, which makes $Ax = b$ solvable, so $b$ is in
the column space. Since all columns of $A$ pass this test of
$b_3 + b_2 - 2b_1 = 0$, this is the equation for the plane. _(4):_

_(4):_

To find the special solutions, set free variables $x_3 = 1, x_4 = 0$, as well as
$x_3 = 0, x_4 = 1$ in $Ux = 0$:

$$
\left[\begin{array}{llll|l}
2 & 4 & 6 & 4 & b_1 \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & 0 & 0 & 0 & b_3 + b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

$x_3 = 1, x_4 = 0$:

$$ 1(x_2) + 1(x_3) + 2(x_4) = 0 \Rightarrow x_2 + 1(1) + 2(0) = 0 \Rightarrow x_2 + 1 = 0 \Rightarrow x_2 = -1 $$

$$ 2x_1 + 4x_2 + 6x_3 + 4x_4 = 0 \Rightarrow 2x_1 + 4(-1) + 6(1) + 4(0) = 0 \Rightarrow 2x_1 - 4 + 6 = 0 \Rightarrow 2x_1 + 2 = 0 \Rightarrow 2x_1 = -2 \Rightarrow x_1 = -1 $$

$$ s_1 = \begin{bmatrix}{}-1\\-1\\1\\0\end{bmatrix} $$

$x_3 = 0, x_4 = 1$:

$$ 1(x_2) + 1(x_3) + 2(x_4) = 0 \Rightarrow x_2 + 1(0) + 2(1) = 0 \Rightarrow x_2 + 2 = 0 \Rightarrow x_2 = -2 $$

$$ 2x_1 + 4x_2 + 6x_3 + 4x_4 = 0 \Rightarrow 2x_1 + 4(-2) + 6(0) + 4(1) = 0 \Rightarrow 2x_1 - 8 + 4 = 0 \Rightarrow 2x_1 - 4 = 0 \Rightarrow 2x_1 = 4 \Rightarrow x_1 = 2 $$

$$ s_2 = \begin{bmatrix}{}2\\-2\\0\\1\end{bmatrix} $$

And thus the nullspace $N(A)$ in $\R^4$ contains all $x_n = c_1s_1 + c_2s_2$.

_(5):_

Reduce $Ux = c$ to $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{llll|l}
2 & 4 & 6 & 4 & b_1 \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & 0 & 0 & 0 & b_3 + b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{llll|l}
2 & 0 & 2 & -4 & 5b_1 - 4b_2 \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & 0 & 0 & 0 & b_3 + b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{llll|l}
1 & 0 & 1 & -2 & \frac{5b_1 - 4b_2}{2} \\
0 & 1 & 1 & 2 & b_2 - b_1 \\
0 & 0 & 0 & 0 & b_3 + b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

Here, we now solve by actually plugging in for $b$ to find $d$:

$$
\left[\begin{array}{cc}
R & d \\
\end{array}\right] =
\left[\begin{array}{llll|l}
1 & 0 & 1 & -2 & \frac{5(4) - 4(3)}{2} \\
0 & 1 & 1 & 2 & (3) - (4) \\
0 & 0 & 0 & 0 & (5) + (3) - 2(4) \\
\end{array}\right] \to
\left[\begin{array}{rrrr|r}
1 & 0 & 1 & -2 & 4 \\
0 & 1 & 1 & 2 & -1 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right]
$$

_(6):_

Find the particular solution $x_p$ where free variables are set to $0$. Back
substitute in $Ux = c$. This yields:

$$ x_p = \begin{bmatrix}{}4\\-1\\0\\0\end{bmatrix} $$

Finally, the complete solution is expressed as:

$$ x_{\text{complete}} = x_p + c_1s_1 + c_2s_2 $$

(You can expand this out if desired, but this is the general form.)

2. Carry out the same six steps for this matrix $A$ with rank one. You will find
   _two_ conditions on $b_1, b_2, b_3$ for $Ax = b$ to be solvable. Together
   these two conditions put $b$ into the ____ space (two planes give a line):

$$ A =
\begin{bmatrix}{}1\\3\\2\end{bmatrix}
\left[\begin{array}{ccc}
2 & 1 & 3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 3 \\
6 & 3 & 9 \\
4 & 2 & 6 \\
\end{array}\right]
$$

$$ b =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix} =
\begin{bmatrix}{}10\\30\\20\end{bmatrix}
$$

_Solution:_

_(1):_

$$ A =
\begin{bmatrix}{}1\\3\\2\end{bmatrix}
\left[\begin{array}{ccc}
2 & 1 & 3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 3 \\
6 & 3 & 9 \\
4 & 2 & 6 \\
\end{array}\right]
$$

$$ b =
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix} =
\begin{bmatrix}{}10\\30\\20\end{bmatrix}
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
6 & 3 & 9 & b_2 \\
4 & 2 & 6 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 3b_1 \\
4 & 2 & 6 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

_(2):_

For $Ax = b$ to have a solution both $b_3 - 2b_1 = 0$ and $b_2 - 3b_1 = 0$ must
hold (then $0 = 0$ for both conditions).

_(3):_

$$ C(A) = \begin{bmatrix}{}2\\6\\4\end{bmatrix} $$

So the column space is the _line_ containing all combinations of the pivot
columns $(2, 6, 4)$.

_(4):_

Find special solutions from $Ux = 0$ by setting $x_2 = 1, x_3 = 0$ and
$x_2 = 0, x_3 = 1$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_1 \\
\end{array}\right]
$$

$x_2 = 1, x_3 = 0$:

$$ 2x_1 + 1x_2 + 3x_3 = 0 \Rightarrow 2x_1 + 1(1) + 3(0) = 0 \Rightarrow 2x_1 + 1 = 0 \Rightarrow 2x_1 = -1 \Rightarrow x_1 = -\frac{1}{2} $$

$$ s_1 = \begin{bmatrix}{}-\frac{1}{2}\\1\\0\end{bmatrix} $$

$x_2 = 0, x_3 = 1$:

$$ 2x_1 + 1x_2 + 3x_3 = 0 \Rightarrow 2x_1 + 1(0) + 3(1) = 0 \Rightarrow 2x_1 + 3 = 0 \Rightarrow 2x_1 = -3 \Rightarrow x_1 = -\frac{3}{2} $$

$$ s_2 = \begin{bmatrix}{}-\frac{3}{2}\\0\\1\end{bmatrix} $$

The nullspace $N(A)$ in $\R^3$ is $x_n = c_1s_1 + c_2s_2$.

_(5):_

Reduce $Ux = c$ to $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & \frac{1}{2} & \frac{3}{2} & \frac{b_1}{2} \\
0 & 0 & 0 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

To find the particular solution for $d$, plug in for $b$ to find $d$:

$$
\left[\begin{array}{cc}
R & d \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 1 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & \frac{1}{2} & \frac{3}{2} & \frac{(10)}{2} \\
0 & 0 & 0 & (30) - 3(10) \\
0 & 0 & 0 & (20) - 2(10) \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & \frac{1}{2} & \frac{3}{2} & 5 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

This shows that $5$ is in $x_p$.

_(6):_

To find $x_p$, take the particular solution for $Rx = d$ and plug in the pivots
in their respective positions, and $0$'s in the positions of the free variables:

$$ x_p = \begin{bmatrix}{}5\\0\\0\end{bmatrix} $$

The complete solution is:

$$ x_{\text{complete}} = x_p + c_1s_1 + c_2s_2 $$

The two conditions of $b_3 - 2b_1 = 0$ and $b_2 - 3b_1 = 0$ must lie within the
_column_ space of $A$.

**Questions 3-15 are about the solution of $Ax = b$. Follow the steps in the
text to $x_p$ and $x_n$. Start from the augmented matrix with last column $b$.**

3. Write the complete solution as $x_p$ plus any multiple of $s$ in the
   nullspace:

$$
x + 3y + 3z = 1 \\
2x + 6y + 9z = 5 \\
-x - 3y + 3z = 5
$$

_Solution:_

Note that here we don't generalize $b$ since the conditions under which $Ax = b$
are solvable is not asked by the problem statement.

$$
x + 3y + 3z = 1 \\
2x + 6y + 9z = 5 \\
-x - 3y + 3z = 5
$$

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 3 & 3 & 1 \\
2 & 6 & 9 & 5 \\
-1 & -3 & 3 & 5 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 3 & 3 & 1 \\
0 & 0 & 3 & 3 \\
-1 & -3 & 3 & 5 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 3 & 3 & 1 \\
0 & 0 & 3 & 3 \\
0 & 0 & 6 & 6 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 3 & 3 & 1 \\
0 & 0 & 3 & 3 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Find $N(A)$:

For there to be a solution $x_3 = 1$, then choose $x_2 = 1$ (note here that
setting $x_2 = 0$ gives only a trivial solution and is not checked since there
is only one free variable).

$x_2 = 1$:

$$ 1x_1 + 3x_2 + 3x_3 = 0 \Rightarrow x_1 + 3(1) + 3(1) = 0 \Rightarrow x_1 + 6 = 0 \Rightarrow x_1 = -6 $$

$$ s = \begin{bmatrix}{}-6\\1\\1\end{bmatrix} $$

Find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 3 & 3 & 1 \\
0 & 0 & 3 & 3 \\
0 & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 3 & 0 & -2 \\
0 & 0 & 3 & 3 \\
0 & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 3 & 0 & -2 \\
0 & 0 & 1 & 1 \\
0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

Find $x_p$, which again, is the same as $Rx = d$, just with $0$'s in the free
variable positions:

$$ x_p = \begin{bmatrix}{}-2\\0\\1\end{bmatrix} $$

Then, the complete solution is:

$$ x_{\text{complete}} = x_p + x_2s $$

Specifically in this case:

$$ x_{\text{complete}} = \begin{bmatrix}{}-2\\0\\1\end{bmatrix} + x_2\begin{bmatrix}{}-6\\1\\1\end{bmatrix} $$

4. Find the complete solution (also called the _general solution_) to

$$
\left[\begin{array}{cccc}
1 & 3 & 1 & 2 \\
2 & 6 & 4 & 8 \\
0 & 0 & 2 & 4 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\begin{bmatrix}{}1\\3\\1\end{bmatrix}
$$

_Solution:_

Same process as problem 3.

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc|c}
1 & 3 & 1 & 2 & 1 \\
2 & 6 & 4 & 8 & 3 \\
0 & 0 & 2 & 4 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 3 & 1 & 2 & 1 \\
0 & 0 & 2 & 4 & 1 \\
0 & 0 & 2 & 4 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 3 & 1 & 2 & 1 \\
0 & 0 & 2 & 4 & 1 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Find $N(A)$ by back substitution through $Ux = c$ and setting free variable(s)
to $1, 0$:

Free variables are $x_2, x_4$, so set $x_2 = 1, x_4 = 0$ and $x_2 = 0, x_4 = 1$:

$x_2 = 1, x_4 = 0$:

$$ 2x_3 + 4x_4 = 0 \Rightarrow 2x_3 + 4(0) = 0 \Rightarrow 2x_3 = 0 \Rightarrow x_3 = 0 $$

$$ 1x_1 + 3x_2 + 1x_3 + 2x_4 = 0 \Rightarrow x_1 + 3(1) + 1(0) + 4(0) = 0 \Rightarrow x_1 + 3 = 0 \Rightarrow x_1 = -3 $$

$$ s_1 = \begin{bmatrix}{}-3\\1\\0\\0\end{bmatrix} $$

$x_2 = 0, x_4 = 1$:

$$ 2x_3 + 4x_4 = 0 \Rightarrow 2x_3 + 4(1) = 0 \Rightarrow 2x_3 + 4 = 0 \Rightarrow 2x_3 = -4 \Rightarrow x_3 = -2 $$

$$ 1x_1 + 3x_2 + 1x_3 + 2x_4 = 0 \Rightarrow x_1 + 3(0) + 1(-2) + 4(1) = 0 \Rightarrow x_1 - 2 + 4 = 0 \Rightarrow x_1 + 2 = 0 \Rightarrow x_1 = -2 $$

$$ s_2 = \begin{bmatrix}{}-2\\0\\-2\\1\end{bmatrix} $$

Find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{cccc|c}
1 & 3 & 1 & 2 & 1 \\
0 & 0 & 2 & 4 & 1 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 3 & 0 & 0 & -\frac{1}{2} \\
0 & 0 & 2 & 4 & 1 \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 3 & 0 & 0 & -\frac{1}{2} \\
0 & 0 & 1 & 2 & \frac{1}{2} \\
0 & 0 & 0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

$$ x_p = \begin{bmatrix}{}-\frac{1}{2}\\0\\\frac{1}{2}\\0\end{bmatrix} $$

$$ x_{\text{complete}} = x_p + x_2s_1 + x_4s_2 $$

$$ x_{\text{complete}} = \begin{bmatrix}{}-\frac{1}{2}\\0\\\frac{1}{2}\\0\end{bmatrix} + x_2\begin{bmatrix}{}-3\\1\\0\\0\end{bmatrix} + x_4\begin{bmatrix}{}-2\\0\\-2\\1\end{bmatrix} $$

5. Under what condition on $b_1, b_2, b_3$ is this system solvable? Include $b$
   as a fourth column in elimination. Find all solutions when that condition
   holds:

$$
x + 2y - 2z = b_1 \\
2x + 5y - 4z = b_2 \\
4x + 9y - 8z = b_3
$$

_Solution:_

Here we do have to find the conditions using a generalized $b$, then solve the
complete solution.

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 2 & -2 & b_1 \\
2 & 5 & -4 & b_2 \\
4 & 9 & -8 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{rrr|l}
1 & 2 & -2 & b_1 \\
0 & 1 & 0 & b_2 - 2b_1 \\
4 & 9 & -8 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{rrr|l}
1 & 2 & -2 & b_1 \\
0 & 1 & 0 & b_2 - 2b_1 \\
0 & 1 & 0 & b_3 - 4b_1 \\
\end{array}\right] \to
$$

$$
\left[\begin{array}{rrr|l}
1 & 2 & -2 & b_1 \\
0 & 1 & 0 & b_2 - 2b_1 \\
0 & 0 & 0 & b_3 - b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

So, the condition on which $Ax = b$ is solvable is $b_3 - b_2 - 2b_1 = 0$.

Now to find all solutions when this condition holds.

First find $N(A)$:

Two pivots, one free variable $= x_3$. Choose $x_3 = 1$, then:

$$ 1x_2 + 0x_3 = 0 \Rightarrow x_2 + 0(1) = 0 \Rightarrow x_2 = 0 $$

$$ 1x_1 + 2x_2 + (-2)x_3 = 0 \Rightarrow x_1 + 2(0) + (-2)(1) = 0 \Rightarrow x_1 - 2 = 0 \Rightarrow x_1 = 2 $$

$$ s = \begin{bmatrix}{}2\\0\\1\end{bmatrix} $$

Now, find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{rrr|l}
1 & 2 & -2 & b_1 \\
0 & 1 & 0 & b_2 - 2b_1 \\
0 & 0 & 0 & b_3 - b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{rrr|l}
1 & 0 & -2 & 5b_1 - 2b_2 \\
0 & 1 & 0 & b_2 - 2b_1 \\
0 & 0 & 0 & b_3 - b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

So $x_p$ is:

$$ x_p = \begin{bmatrix}{}5b_1 - 2b_2\\b_2 - 2b_1\\0\end{bmatrix} $$

$$ x_{\text{complete}} = x_p + x_3s $$

$$ x_{\text{complete}} = \begin{bmatrix}{}5b_1 - 2b_2\\b_2 - 2b_1\\0\end{bmatrix} + x_3\begin{bmatrix}{}2\\0\\1\end{bmatrix} $$

6. What conditions on $b_1, b_2, b_3, b_4$ make each system solvable? Find $x$
   in that case:

$$
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
2 & 5 \\
3 & 9 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\\b_4\end{bmatrix}
$$

$$
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
2 & 4 & 7 \\
3 & 9 & 12 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\\b_4\end{bmatrix}
$$

_Solution:_

_First:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 2 & b_1 \\
2 & 4 & b_2 \\
2 & 5 & b_3 \\
3 & 9 & b_4 \\
\end{array}\right] \to
\left[\begin{array}{cc|l}
1 & 2 & b_1 \\
0 & 0 & b_2 - 2b_1 \\
0 & 1 & b_3 - 2b_1 \\
0 & 3 & b_4 - 3b_1 \\
\end{array}\right] \to
\left[\begin{array}{cc|l}
1 & 2 & b_1 \\
0 & 1 & b_3 - 2b_1 \\
0 & 3 & b_4 - 3b_1 \\
0 & 0 & b_2 - 2b_1 \\
\end{array}\right] \to
$$

$$
\left[\begin{array}{cc|l}
1 & 2 & b_1 \\
0 & 1 & b_3 - 2b_1 \\
0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

So, the conditions on which this system is solvable are $b_2 - 2b_1 = 0$ and
$b_4 - 3b_3 + 3b_1 = 0$.

Now to solve for $x$ (complete):

Find $N(A)$:

We have two pivots and no free variables, so $N(A) = \mathbf{0}$.

Now find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{cc|l}
1 & 2 & b_1 \\
0 & 1 & b_3 - 2b_1 \\
0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{cc|l}
1 & 0 & 5b_1 - 2b_3 \\
0 & 1 & b_3 - 2b_1 \\
0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

$$ x_p = \begin{bmatrix}{}5b_1 - 2b_3\\b_3 - 2b_1\end{bmatrix} $$

And:

$$ x_{\text{complete}} = x_p $$

$$ x_{\text{complete}} = \begin{bmatrix}{}5b_1 - 2b_3\\b_3 - 2b_1\end{bmatrix} $$

_Second:_

$$
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 4 & 6 \\
2 & 4 & 7 \\
3 & 9 & 12 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_2\\b_3\\b_4\end{bmatrix}
$$

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & b_1 \\
2 & 4 & 6 & b_2 \\
2 & 5 & 7 & b_3 \\
3 & 9 & 12 & b_4 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
2 & 5 & 7 & b_3 \\
3 & 9 & 12 & b_4 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
0 & 1 & 1 & b_3 - 2b_1 \\
3 & 9 & 12 & b_4 \\
\end{array}\right] \to
$$

$$
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
0 & 1 & 1 & b_3 - 2b_1 \\
0 & 3 & 3 & b_4 - 3b_1 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 1 & 1 & b_3 - 2b_1 \\
0 & 3 & 3 & b_4 - 3b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 1 & 1 & b_3 - 2b_1 \\
0 & 0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

So the conditions on which $Ax = b$ is solvable are $b_4 - 3b_3 + 3b_1 = 0$ and
$b_2 - 2b_1 = 0$.

Find $N(A)$:

We have two pivots and 1 free variable $= x_3$. So, set $x_3 = 1$, and then:

$$ 1x_2 + 1x_3 = 0 \Rightarrow x_2 + 1(1) = 0 \Rightarrow x_2 + 1 = 0 \Rightarrow x_2 = -1 $$

$$ 1x_1 + 2x_2 + 3x_3 = 0 \Rightarrow x_1 + 2(-1) + 3(1) = 0 \Rightarrow x_1 - 2 + 3 = 0 \Rightarrow x_1 + 1 = 0 \Rightarrow x_1 = -1 $$

$$ s = \begin{bmatrix}{}-1\\-1\\1\end{bmatrix} $$

Find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc|l}
1 & 2 & 3 & b_1 \\
0 & 1 & 1 & b_3 - 2b_1 \\
0 & 0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 0 & 1 & 5b_1 - 2b_3 \\
0 & 1 & 1 & b_3 - 2b_1 \\
0 & 0 & 0 & b_4 - 3b_3 + 3b_1 \\
0 & 0 & 0 & b_2 - 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

$$ x_p = \begin{bmatrix}{}5b_1 - 2b_3\\b_3 - 2b_1\\0\end{bmatrix} $$

$$ x_{\text{complete}} = x_p + x_3s $$

$$ x_{\text{complete}} = \begin{bmatrix}{}5b_1 - 2b_3\\b_3 - 2b_1\\0\end{bmatrix} + \begin{bmatrix}{}-1\\-1\\1\end{bmatrix} $$

7. Show by elimination that $(b_1, b_2, b_3)$ is in the column space if
   $b_3 - 2b_2 + 4b_1 = 0$.

$$ A =
\left[\begin{array}{ccc}
1 & 3 & 1 \\
3 & 8 & 2 \\
2 & 4 & 0 \\
\end{array}\right]
$$

What combination of the rows of $A$ gives the zero row?

_Solution:_

_Show by elimination that $(b_1, b_2, b_3)$ is in the column space if
$b_3 - 2b_2 + 4b_1 = 0$:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 3 & 1 & b_1 \\
3 & 8 & 2 & b_2 \\
2 & 4 & 0 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 3 & 1 & b_1 \\
0 & -1 & -1 & b_2 - 3b_1 \\
2 & 4 & 0 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 3 & 1 & b_1 \\
0 & -1 & -1 & b_2 - 3b_1 \\
0 & -2 & -2 & b_3 - 2b_1 \\
\end{array}\right] \to
$$

$$
\left[\begin{array}{ccc|l}
1 & 3 & 1 & b_1 \\
0 & -1 & -1 & b_2 - 3b_1 \\
0 & 0 & 0 & b_3 - 2b_2 + 4b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Thus, by elimination, $(b_1, b_2, b_3)$ is in the column space if
$b_3 - 2b_2 + 4b_1 = 0$.

_What combination of the rows of $A$ gives the zero row?:_

The above elimination steps show the combination, in essence we have
$(\text{row } 3) -
2(\text{row } 2) + 4(\text{row } 1)$.

8. Which vectors $(b_1, b_2, b_3)$ are in the column space of $A$? Which
   combinations of the rows of $A$ give zero?

a.

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 1 \\
2 & 6 & 3 \\
0 & 2 & 5 \\
\end{array}\right]
$$

_Solution:_

_Which vectors $(b_1, b_2, b_3)$ are in the column space of $A$?:_

We can find the column space of $A$ by taking $Ax = b \to Ux = c$ and looking at
the pivots.

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 1 & b_1 \\
2 & 6 & 3 & b_2 \\
0 & 2 & 5 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 1 & b_1 \\
0 & 2 & 1 & b_2 - 2b_1 \\
0 & 2 & 5 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 2 & 1 & b_1 \\
0 & 2 & 1 & b_2 - 2b_1 \\
0 & 0 & 4 & b_3 - b_2 + 2b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

So all 3 columns of $A$ are in the column space of $A$ (since there are no free
rows in $Ux = c$):

$$ C(A) = \text{span}\left\{\begin{bmatrix}{}1\\2\\0\end{bmatrix}, \begin{bmatrix}{}2\\6\\2\end{bmatrix}, \begin{bmatrix}{}1\\3\\5\end{bmatrix}\right\} $$

_Which combinations of the rows of $A$ give zero?:__

The only combinations of the rows of $A$ that give zero is $\mathbf{0}$ (since
there are no free rows).

b.

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 4 \\
2 & 4 & 8 \\
\end{array}\right]
$$

_Solution:_

_Which vectors $(b_1, b_2, b_3)$ are in the column space of $A$?:_

Again, we can find the column space of $A$ by going from $Ax = b \to Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 1 & 1 & b_1 \\
1 & 2 & 4 & b_2 \\
2 & 4 & 8 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 1 & 1 & b_1 \\
0 & 1 & 3 & b_2 - b_1 \\
2 & 4 & 8 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|l}
1 & 1 & 1 & b_1 \\
0 & 1 & 3 & b_2 - b_1 \\
0 & 2 & 6 & b_3 - 2b_1 \\
\end{array}\right] \to
$$

$$
\left[\begin{array}{ccc|l}
1 & 1 & 1 & b_1 \\
0 & 1 & 3 & b_2 - b_1 \\
0 & 0 & 0 & b_3 - 2b_2 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

So, we can see that the third column is a free column, and thus the column space
of $A$ spans all linear combinations of the first two columns of $A$:

$$ C(A) = \text{span}\left\{\begin{bmatrix}{}1\\1\\2\end{bmatrix}, \begin{bmatrix}{}1\\2\\4\end{bmatrix}\right\} $$

_Which combinations of the rows of $A$ give zero?:__

The combinations of the rows of $A$ that give zero are
$\text{row } 3 - 2\text{row } 2 = 0$.

9.

a. The Worked Example 3.3A reached
$\left[\begin{array}{cc}U & c \\\end{array}\right]$ from
$\left[\begin{array}{cc}A & b \\\end{array}\right]$. Put the multipliers into
$L$ and verify that $LU$ equals $A$ and $Lc$ equals $b$.

_Solution:_

Let's examine step 1 of 3A first, that way we can find the various $E$'s in the
elimination step, then take their inverse (and reverse order) to find $L$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc|c}
1 & 2 & 3 & 5 & b_1 \\
2 & 4 & 8 & 12 & b_2 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right]
$$

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc|c}
1 & 2 & 3 & 5 & b_1 \\
2 & 4 & 8 & 12 & b_2 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{cccc|l}
1 & 2 & 3 & 5 & b_1 \\
0 & 0 & 2 & 2 & b_2 - 2b_1 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right]
$$

$$ E_{31} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
-3 & 0 & 1 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cccc|c}
1 & 2 & 3 & 5 & b_1 \\
2 & 4 & 8 & 12 & b_2 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{cccc|l}
1 & 2 & 3 & 5 & b_1 \\
0 & 0 & 2 & 2 & b_2 - 2b_1 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{rrrr|l}
1 & 2 & 3 & 5 & b_1 \\
0 & 0 & 2 & 2 & b_2 - 2b_1 \\
0 & 0 & -2 & -2 & b_3 - 3b_1 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

_Put the multipliers into $L$:_

So now to find $L$ by reversing the order of the $E$'s and taking their
inverses:

$$ L = E_{31}^{-1}E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
$$

_Verify that $LU$ equals $A$ and $Lc$ equals $b$:_

$$
L\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
3 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr|l}
1 & 2 & 3 & 5 & b_1 \\
0 & 0 & 2 & 2 & b_2 - 2b_1 \\
0 & 0 & -2 & -2 & b_3 - 3b_1 \\
\end{array}\right] =
\left[\begin{array}{cccc|l}
1 & 2 & 3 & 5 & b_1 \\
2 & 4 & 8 & 12 & b_2 \\
3 & 6 & 7 & 13 & b_3 \\
\end{array}\right] =
\left[\begin{array}{cc}
A & b \\
\end{array}\right]
$$

b. Combine the pivot columns of $A$ with the numbers $-9$ and $3$ in the
particular solution $x_p$. What is the linear combination and why?

_Solution:_

_Combine the pivot columns of $A$ with the numbers $-9$ and $3$ in the
particular solution $x_p$:_

In 3A, it was found that the pivot columns were $x_1, x_3$, with free variables
being $x_2, x_4$, so, if $-9$ and $3$ are combined with these pivot columns to
find $x_p$, this means that $x_p$ is:

$$ x_p = \begin{bmatrix}{}-9\\0\\3\\0\end{bmatrix} $$

_What is the linear combination and why?:_

The linear combination then takes $x_p$ and multiplies the pivots by the column
space vectors and then sums them together:

$$ -9\begin{bmatrix}{}1\\2\\3\end{bmatrix} + 3\begin{bmatrix}{}3\\8\\7\end{bmatrix} = \begin{bmatrix}{}-9\\-18\\-27\end{bmatrix} + \begin{bmatrix}{}9\\24\\21\end{bmatrix} = \begin{bmatrix}{}0\\6\\-6\end{bmatrix} $$

Notice that this is the particular solution $x_p$ that was found in step 6 of
3A. In other words this is $Ax_p = b$.

10. Construct a 2 by 3 system $Ax = b$ with particular solution
    $x_p = (2, 4, 0)$ and homogeneous solution $x_n =$ any multiple of
    $(1, 1, 1)$.

_Solution:_

Note that "homogeneous solution" means the nullspace solutions.

_Construct a 2 by 3 system $Ax = b$ with particular solution $x_p = (2, 4, 0)$:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 0 & -2 & b_1 \\
0 & 4 & -4 & b_2 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Let's confirm:

First, find $N(A)$, there are two pivots and 1 free variable $= x_3$, so choose
$x_3 = 1$:

$$ 4x_2 + (-4)x_3 = 0 \Rightarrow 4x_2 + (-4)(1) = 0 \Rightarrow 4x_2 - 4 = 0 \Rightarrow 4x_2 = 4 \Rightarrow x_2 = 1 $$

$$ 2x_1 + 0x_2 + (-2)x_3 = 0 \Rightarrow 2x_1 + 0(2) + (-2)(1) = 0 \Rightarrow 2x_1 - 2 = 0 \Rightarrow 2x_1 = 2 \Rightarrow x_1 = 1 $$

$$ s = \begin{bmatrix}{}1\\1\\1\end{bmatrix} $$

Thus $x_n$ is a multiple of $(1, 1, 1)$.

Now, find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
2 & 0 & -2 & b_1 \\
0 & 4 & -4 & b_2 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 0 & -1 & \frac{b_1}{2} \\
0 & 1 & -1 & \frac{b_2}{4} \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

So $x_p$ is:

$$ x_p = \begin{bmatrix}{}2\\4\\0\end{bmatrix} $$

Thus the particular solution is validated.

11. Why can't a $1$ by $3$ system have $x_p = (2, 4, 0)$ and $x_n =$ any
    multiple of $(1, 1, 1)$?

_Solution:_

By the problem statement, we're saying that $Ax = b$ has $x_p = (2, 4, 0)$ as a
solution with two pivots and one free variable, the same in fact as problem 10.
But a 1 by 3 matrix can have at most 1 pivot (since there is only 1 row), thus
this is not possible.

12.

a. If $Ax = b$ has two solutions $x_1$ and $x_2$, find two solutions to
$Ax = \mathbf{0}$.

_Solution:_

Since $Ax = b$ has solutions $x_1, x_2$, it follows that:

$$ Ax_1 = b \text{ and } Ax_2 = b $$

It follows that if we are to say that $b = 0$, then:

$$ Ax_1 = 0 \text{ and } Ax_2 = 0 $$

Now, consider:

$$ A(x_1 - x_2) = A(x_1) - A(x_2) = b - b = 0 $$

Similarly $x_2 - x_1$ is also a solution, but it is a linear combination of
$x_1 - x_2$ (because it's just $-1$ times $x_1 - x_2$), and thus is not a
separate solution.

The other solution is (trivially) when $x = \mathbf{0}$.

So, two solutions are $x_1 - x_2$ and $x = \mathbf{0}$.

b. Then find another solution to $Ax = \mathbf{0}$ and another solution to
$Ax = b$.

_Solution:_

Any multiple of $A(x_1 - x_2)$ is another solution to $Ax = \mathbf{0}$:

$$ A(2(x_1 - x_2)) = A(2x_1 - 2x_2) = A(2x_1) - A(2x_2) = 2b - 2b = 2(0) - 2(0) = 0 - 0 = 0 $$

Any addition of $x_1$ is also another solution to $Ax = b$:

$$ A(2x_1 - x_2) = 2(A(x_1)) - (A(x_2)) = 2b - b = b $$

13. Explain why these are all false:

a. The complete solution is any linear combination of $x_p$ and $x_n$.

No, because $x_p$ has no multiple other than $1$.

b. A system $Ax = b$ has at most one particular solution.

No, if $r = m$ and $r < n$ (_i.e._ the matrix is "short and wide"), then
$Ax = b$ has $\infty$ solutions.

Also, if $r < m$ and $r < n$ (_i.e._ the matrix is not full rank), then $Ax = b$
has either $0$ or $\infty$ solutions.

c. The solution $x_p$ with all free variables zero is the shortest solution
(minimum length $||x||$). Find a 2 by 2 counterexample.

No, since $x = x_p + x_n$, this suggests that
$\text{length}(x_p) \leq \text{length}(x_p) + \text{length}(x_n)$, but it is
possible that $\text{length}(x_n) < \text{length}(x_p)$.

Consider:

$$
\left[\begin{array}{cc|c}
3 & 3 & 6 \\
3 & 3 & 6 \\
\end{array}\right]
$$

This reduces to $Ux = c$:

$$
\left[\begin{array}{cc|c}
3 & 3 & 6 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Then, $N(A)$ is:

$$ 3x_1 + 3x_2 = 0 \Rightarrow 3x_1 + 3(1) = 0 \Rightarrow 3x_1 = -3 \Rightarrow x_1 = -1 $$

$$ s = \begin{bmatrix}{}-1\\1\end{bmatrix} $$

Then, $Rx = d$ yields:

$$
\left[\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 0 \\
\end{array}\right]
$$

So,

$$ x_p = \begin{bmatrix}{}2\\0\end{bmatrix} $$

Then:

$$ x = x_p + x_n $$

$$ x = \begin{bmatrix}{}2\\0\end{bmatrix} + \begin{bmatrix}{}-1\\1\end{bmatrix} = \begin{bmatrix}{}1\\1\end{bmatrix}$$

To calculate the length, simply take the Euclidiean distance of the two
coordinates:

$$ ||x_p|| = \sqrt{(2)^2 + (0)^2} = \sqrt{4} = 2 $$

$$ ||x_p + x_n|| = \sqrt{(1)^2 + (1)^2} = \sqrt{2} $$

Now, simply observe that:

$$ ||x_p|| = 2 \geq \sqrt{2} = ||x_p + x_n|| $$

Thus $x_p$ is not the shortest solution.

d. If $A$ is invertible there is no solution $x_n$ in the nullspace.

The only homogeneous solution in the nullspace is $x_n = \mathbf{0}$ when $A$ is
invertible. An invertible matrix indicates that $A$ is a square matrix, and thus
is full rank (both full column and full row), it follows that there are no free
variables in $A$, and thus the only vector that spans $N(A)$ is $\mathbf{0}$.

14. Suppose column $5$ of $U$ has no pivot. Then $x_5$ is a ____ variable. The
    zero vector (is) (is not) the only solution to $Ax = \mathbf{0}$. If
    $Ax = b$ has a solution, then it has ____ solutions.

free; is not (since there is a free variable); infinite (because it has any
multiple of the nullspace solution)

15. Suppose row 3 of $U$ has no pivot. Then that row is ____. The equation
    $Ux = c$ is only solvable provided ____. The equation $Ax = b$ (is)(is
    not)(might not be) solvable.

a $0$ row; $c_3 = 0$; might not be (not solvable if $c_3 \neq 0$ or any other
$0$ row where $c_i \neq 0$).

**Questions 16-20 are about matrices of "full rank" $r = m$ or $r = n$.**

16. The largest possible rank of a 3 by 5 matrix is ____. Then there is a pivot
    in every ____ of $U$ and $R$. The solution to $Ax = b$ (always exists) (is
    unique). The column space of $A$ is ____. An example is $A =$ ____.

$3$; row; always exists; all of $\R^3$; $A = [\begin{array}{c}I & F\end{array}]$
for any 3 by 2 matrix $F$.

17. The largest possible rank of a 6 by 4 matrix is ____. Then there is a pivot
    in every ____ of $U$ and $R$. The solution to $Ax = b$ (always exists) (is
    unique). The nullspace of $A$ is ____. An example is $A =$ ____.

$4$; column; is unique; only $\mathbf{0}$;
$\left[\begin{array}{c}I\\ \mathbf{0}\end{array}\right]$ where $I$ is a 4 by 4
identity matrix, and $\mathbf{0}$ is a 2 by 4 zero matrix.

18. Find by elimination the rank of $A$ and also the rank of $A^{\mathbf{T}}$:

$$ A =
\left[\begin{array}{rrr}
1 & 4 & 0 \\
2 & 11 & 5 \\
-1 & 2 & 10 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 1 \\
1 & 1 & 2 \\
1 & 1 & q \\
\end{array}\right]
$$

(rank depends on $q$).

_Solution:_

_First:_

$$ A =
\left[\begin{array}{rrr}
1 & 4 & 0 \\
2 & 11 & 5 \\
-1 & 2 & 10 \\
\end{array}\right]
$$

Rank of $A$:

$$ A =
\left[\begin{array}{rrr}
1 & 4 & 0 \\
2 & 11 & 5 \\
-1 & 2 & 10 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 4 & 0 \\
0 & 3 & 5 \\
-1 & 2 & 10 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 4 & 0 \\
0 & 3 & 5 \\
0 & 6 & 10 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 4 & 0 \\
0 & 3 & 5 \\
0 & 0 & 0 \\
\end{array}\right] \to
$$

So $r(A) = 2$.

Rank of $A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 2 & -1 \\
4 & 11 & 2 \\
0 & 5 & 10 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -1 \\
0 & 3 & 6 \\
0 & 5 & 10 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -1 \\
0 & 3 & 6 \\
0 & 0 & 0 \\
\end{array}\right] \to
$$

So $r(A^{\mathbf{T}}) = 2$.

_Second:_

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 1 \\
1 & 1 & 2 \\
1 & 1 & q \\
\end{array}\right]
$$

(rank depends on $q$).

Rank of $A$:

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 1 \\
1 & 1 & 2 \\
1 & 1 & q \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 1 \\
1 & 1 & q \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 1 \\
0 & 1 & q - 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 1 \\
0 & 1 & 1 \\
0 & 0 & q - 2 \\
\end{array}\right]
$$

So if $q - 2 = 0 \to q = 2$, then $r(A) = 2$, otherwise $r(A) = 3$.

Rank of $A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
1 & 2 & q \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & q \\
0 & 1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & q - 1 \\
0 & 1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & q - 1 \\
0 & 0 & 2 - q \\
\end{array}\right] \to
$$

Similarly if $2 - q = 0 \to q = 2$, then $r(A^{\mathbf{T}}) = 2$, otherwise
$r(A^{\mathbf{T}}) = 3$.

19. Find the rank of $A$ and also of $A^{\mathbf{T}}A$ and also of
    $AA^{\mathbf{T}}$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 0 & 1 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{cc}
2 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 0 & 1 \\
\end{array}\right]
$$

$r(A)$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 5 \\
0 & -1 & -4 \\
\end{array}\right]
$$

so $r(A) = 2$

$r(A^{\mathbf{T}}A)$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 \\
1 & 0 \\
5 & 1 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
1 & 1 \\
1 & 0 \\
5 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 1 & 6 \\
1 & 1 & 5 \\
6 & 5 & 26 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
2 & 1 & 6 \\
1 & 1 & 5 \\
6 & 5 & 26 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
2 & 1 & 6 \\
0 & \frac{1}{2} & 2 \\
6 & 5 & 26 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
2 & 1 & 6 \\
0 & \frac{1}{2} & 2 \\
0 & 2 & 8 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
2 & 1 & 6 \\
0 & \frac{1}{2} & 2 \\
0 & 0 & 0 \\
\end{array}\right]
$$

So $r(A^{\mathbf{T}}A) = 2$ .

$r(AA^{\mathbf{T}})$:

$$ AA^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 & 5 \\
1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 \\
1 & 0 \\
5 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
27 & 6 \\
6 & 2 \\
\end{array}\right]
$$

$$ AA^{\mathbf{T}} =
\left[\begin{array}{cc}
27 & 6 \\
6 & 2 \\
\end{array}\right] \to
\left[\begin{array}{cc}
27 & 6 \\
0 & \frac{2}{3} \\
\end{array}\right]
$$

So $r(AA^{\mathbf{T}}) = 2$.

_Second:_

$$ A =
\left[\begin{array}{cc}
2 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$r(A)$:

$$ A =
\left[\begin{array}{cc}
2 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] \to
\left[\begin{array}{cc}
2 & 0 \\
0 & 1 \\
1 & 2 \\
\end{array}\right] \to
\left[\begin{array}{cc}
2 & 0 \\
0 & 1 \\
0 & 2 \\
\end{array}\right] \to
\left[\begin{array}{cc}
2 & 0 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

So $r(A) = 2$.

$r(A^{\mathbf{T}}A)$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
2 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
2 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
2 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
6 & 3 \\
3 & 5 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
6 & 3 \\
3 & 5 \\
\end{array}\right] \to
\left[\begin{array}{cc}
6 & 3 \\
0 & \frac{7}{2} \\
\end{array}\right]
$$

So $r(A^{\mathbf{T}}A) = 2$.

$r(AA^{\mathbf{T}})$:

$$ AA^{\mathbf{T}} =
\left[\begin{array}{cc}
2 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right] =
\left[\begin{array}{ccc}
4 & 2 & 2 \\
2 & 2 & 3 \\
2 & 3 & 5 \\
\end{array}\right]
$$

$$ AA^{\mathbf{T}} =
\left[\begin{array}{ccc}
4 & 2 & 2 \\
2 & 2 & 3 \\
2 & 3 & 5 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
4 & 2 & 2 \\
0 & 1 & 2 \\
2 & 3 & 5 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
4 & 2 & 2 \\
0 & 1 & 2 \\
0 & 2 & 4 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
4 & 2 & 2 \\
0 & 1 & 2 \\
0 & 0 & 0 \\
\end{array}\right] \to
$$

So $r(AA^{\mathbf{T}}) = 2$.

20. Reduce $A$ to its echelon form $U$. Then find a triangular $L$ so that
    $A = LU$.

$$ A =
\left[\begin{array}{cccc}
3 & 4 & 1 & 0 \\
6 & 5 & 2 & 1 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{cccc}
1 & 0 & 1 & 0 \\
2 & 2 & 0 & 3 \\
0 & 6 & 5 & 4 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{cccc}
3 & 4 & 1 & 0 \\
6 & 5 & 2 & 1 \\
\end{array}\right]
$$

_Reduce $A$ to its echelon form $U$:_

$$ A =
\left[\begin{array}{cccc}
3 & 4 & 1 & 0 \\
6 & 5 & 2 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
3 & 4 & 1 & 0 \\
0 & -3 & 0 & 1 \\
\end{array}\right] = U
$$

_Then find a triangular $L$ so that $A = LU$:_

$$ E_{21} =
\left[\begin{array}{rr}
1 & 0 \\
-2 & 1 \\
\end{array}\right]
$$

$$ L = E_{21}^{-1} =
\left[\begin{array}{rr}
1 & 0 \\
2 & 1 \\
\end{array}\right]
$$

$$ LU =
\left[\begin{array}{rr}
1 & 0 \\
2 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
3 & 4 & 1 & 0 \\
0 & -3 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
3 & 4 & 1 & 0 \\
6 & 5 & 2 & 1 \\
\end{array}\right] = A
$$

_Second:_

$$ A =
\left[\begin{array}{cccc}
1 & 0 & 1 & 0 \\
2 & 2 & 0 & 3 \\
0 & 6 & 5 & 4 \\
\end{array}\right]
$$

_Reduce $A$ to its echelon form $U$:_

$$ A =
\left[\begin{array}{cccc}
1 & 0 & 1 & 0 \\
2 & 2 & 0 & 3 \\
0 & 6 & 5 & 4 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 0 & 1 & 0 \\
0 & 2 & -2 & 3 \\
0 & 6 & 5 & 4 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 0 & 1 & 0 \\
0 & 2 & -2 & 3 \\
0 & 0 & 11 & -5 \\
\end{array}\right] = U
$$

_Then find a triangular $L$ so that $A = LU$:_

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
0 & -3 & 1 \\
\end{array}\right]
$$

$$ L = E_{32}^{-1}E_{21}^{-1} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 3 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 3 & 1 \\
\end{array}\right]
$$

$$ LU =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
2 & 1 & 0 \\
0 & 3 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
1 & 0 & 1 & 0 \\
0 & 2 & -2 & 3 \\
0 & 0 & 11 & -5 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & 1 & 0 \\
2 & 2 & 0 & 3 \\
0 & 6 & 5 & 4 \\
\end{array}\right] = A
$$

21. Find the complete solution in the form $x_p + x_n$ to these full rank
    systems:

a. $x + y + z = 4$

_Solution:_

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Find $N(A)$:

We have one pivot and 2 free variables $y, z$, so let $y = 1, z = 0$ and
$y = 0, z = 1$:

$y = 1, z = 0$:

$$ 1x + 1y + 1z = 0 \Rightarrow x + 1(1) + 1(0) = 0 \Rightarrow x + 1 = 0 \Rightarrow x = -1 $$

$$ s_1 = \begin{bmatrix}{}-1\\1\\0\end{bmatrix} $$

$y = 0, z = 1$:

$$ 1x + 1y + 1z = 0 \Rightarrow x + 1(0) + 1(1) = 0 \Rightarrow x + 1 = 0 \Rightarrow x = -1 $$

$$ s_2 = \begin{bmatrix}{}-1\\0\\1\end{bmatrix} $$

Find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 1 & 1 & 4 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

So $x_p$ is:

$$ x_p = \begin{bmatrix}{}4\\0\\0\end{bmatrix} $$

So:

$$ x = x_p + ys_1 + zs_2 $$

$$ x = \begin{bmatrix}{}4\\0\\0\end{bmatrix} + y\begin{bmatrix}{}-1\\1\\0\end{bmatrix} + z\begin{bmatrix}{}-1\\0\\1\end{bmatrix} $$

b.

$$
x + y + z = 4 \\
x - y + z = 4 \\
$$

_Solution:_

Find $Ux = c$:

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
1 & -1 & 1 & 4 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & -2 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
U & c \\
\end{array}\right]
$$

Find $N(A)$:

There are two pivots and 1 free variable $z$, so set $z = 1$:

$$ -2y + 0z = 0 \Rightarrow -2y = 0 \Rightarrow y = 0 $$

$$ 1x + 1y + 1z = 0 \Rightarrow x + 1(0) + 1(1) = 0 \Rightarrow x + 1 = 0 \Rightarrow x = -1 $$

$$ s = \begin{bmatrix}{}-1\\0\\1\end{bmatrix} $$

Find $Rx = d$:

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{rrr|r}
1 & 1 & 1 & 4 \\
0 & -2 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 0 & 1 & 4 \\
0 & 2 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr|r}
1 & 0 & 1 & 4 \\
0 & 1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
R & d \\
\end{array}\right]
$$

So $x_p$ is:

$$ x_p = \begin{bmatrix}{}4\\0\\0\end{bmatrix} $$

Then:

$$ x = x_p + zs $$

$$ x = \begin{bmatrix}{}4\\0\\0\end{bmatrix} + z\begin{bmatrix}{}-1\\0\\1\end{bmatrix} $$

22. If $Ax = b$ has infinitely many solutions, why is it impossible for $Ax = B$
    (new right side) to have only one solution? Could $Ax = B$ have no solution?

_Solution:_

Consider $A(x_1 - x_2) = \mathbf{0}$, then we can add $x_1 - x_2$ to $B$, but
the solution will not be unique. There will be no solution to $Ax = B$ unless
$B$ is in the column space of $A$ (in which case $B$ is one of the solutions of
$b$).

23. Choose the number $q$ so that (if possible) the ranks are (a) 1, (b) 2,
    \(c\) 3:

$$ A =
\left[\begin{array}{rrr}
6 & 4 & 2 \\
-3 & -2 & -1 \\
9 & 6 & q \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{ccc}
3 & 1 & 3 \\
q & 2 & q \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ A =
\left[\begin{array}{rrr}
6 & 4 & 2 \\
-3 & -2 & -1 \\
9 & 6 & q \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{rrr}
6 & 4 & 2 \\
-3 & -2 & -1 \\
9 & 6 & q \\
\end{array}\right] \to
\left[\begin{array}{rrr}
6 & 4 & 2 \\
0 & 0 & 0 \\
9 & 6 & q \\
\end{array}\right] \to
\left[\begin{array}{lll}
6 & 4 & 2 \\
0 & 0 & 0 \\
0 & 0 & q - 3 \\
\end{array}\right]
$$

a. $r(A) = 1$

$$ q - 3 = 0 \to q = 3 $$

b. $r(A) = 2$

$$ q - 3 \neq 0 $$

c. $r(A) = 3$

Not possible, there is a single free row that makes it so the highest rank is 2.

_Second:_

$$ B =
\left[\begin{array}{ccc}
3 & 1 & 3 \\
q & 2 & q \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
3 & 1 & 3 \\
q & 2 & q \\
\end{array}\right] \to
\left[\begin{array}{lll}
3 & 1 & 3 \\
q - 3 & 1 & q - 3 \\
\end{array}\right]
$$

a. $r(B) = 1$

Then elimination must take a different route from above:

$$ B =
\left[\begin{array}{ccc}
3 & 1 & 3 \\
q & 2 & q \\
\end{array}\right] \to
\left[\begin{array}{lll}
3 & 1 & 3 \\
q - 6  & 0 & q - 6 \\
\end{array}\right]
$$

So to have $r(B) = 1$, $q - 6 = 0 \to q = 6$.

b. $r(B) = 2$

Then the original elimination stands, and $q - 3 = 0 \to q = 3$ to have
$r(B) = 2$.

c. $r(B) = 3$

There cannot be rank 3 as there are only 2 rows and 3 columns.

24. Give examples of matrices $A$ for which the number of solutions to $Ax = b$
    is

a. $0$ or $1$, depending on $b$

_Solution:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{c|c}
1 & b_1 \\
1 & b_2 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{c|c}
1 & b_1 \\
1 & b_2 \\
\end{array}\right] \to
\left[\begin{array}{c|c}
1 & b_1 \\
0 & b_2 - b_1 \\
\end{array}\right]
$$

So, there are $0$ solutions if $b_2 - b_1 \neq 0$, and $1$ solution if
$b_2 - b_1 = 0$.

b. $\infty$, regardless of $b$

_Solution:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
1 & 2 & 1 & 3 \\
\end{array}\right]
$$

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
1 & 2 & 1 & 3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 1 & 1 & 1 \\
0 & 1 & 0 & 2 \\
\end{array}\right]
$$

So we have 1 free variable, which ensures that there is at least one non zero
vector special solution in the nullspace, and any multiple times that solution
is also a solution, ad infinitum.

c. $0$ or $\infty$, depending on $b$

_Solution:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc|c}
1 & 2 & 3 & b_1 \\
1 & 3 & 3 & b_2 \\
2 & 4 & 6 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 2 & 3 & b_1 \\
0 & 1 & 0 & b_2 - b_1 \\
2 & 4 & 6 & b_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 2 & 3 & b_1 \\
0 & 1 & 0 & b_2 - b_1 \\
0 & 0 & 0 & b_3 - b_1 \\
\end{array}\right]
$$

Here, the matrix is not full rank ($r < m$ and $r < n$), if in the second row
after elimination $b_3 - b_1 \neq 0$, then there are no solutions, however if
$b_3 - b_1 = 0$, then there are infinitely many (as then the nullspace is filled
by some nonzero special solution as column 3 is free).

d. $1$, regardless of $b$

_Solution:_

$$
\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{cc|c}
1 & 2 & b_1 \\
1 & 5 & b_2 \\
\end{array}\right] \to
\left[\begin{array}{cc|c}
1 & 2 & b_1 \\
0 & 3 & b_2 - b_1 \\
\end{array}\right]
$$

Here, the matrix is square and invertible ($r = m$ and $r = n$). There is
exactly one solution where $3x_2 = b_2 - b_1 \to x_2 = \dfrac{b_2 - b_1}{3}$,
and thus the sole solution can be derived from
$x_1 + 2\left(\dfrac{b_2 - b_1}{3}\right) = b_1$.

25. Write down all the known relations between $r$ and $m$ and $n$ if $Ax = b$
    has

a. no solution for some $b$

_Solution:_

$r < m$

b. infinitely many solutions for every $b$

_Solution:_

$r < n$

c. exactly one solution for some $b$, no solution for other $b$

_Solution:_

$r < m$ and $r = n$

d. exactly one solution for every $b$

_Solution:_

$r = m$ and $r = n$

**Questions 26-33 are about Gauss-Jordan elimination (upwards as well as
downwards and the reduced echelon matrix $R$.**

26. Continue elimination from $U$ to $R$. Divide rows by pivots so the new
    pivots are all $1$. Then produce zeros _above_ those pivots to reach $R$:

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 0 \\
\end{array}\right]
$$

and

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 5 \\
\end{array}\right]
$$

_Solution:_

_First:_

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 1 & 2 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 0 & -2 \\
0 & 1 & 2 \\
0 & 0 & 0 \\
\end{array}\right] = R
$$

_Second:_

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 5 \\
\end{array}\right]
$$

$$ U =
\left[\begin{array}{ccc}
2 & 4 & 4 \\
0 & 3 & 6 \\
0 & 0 & 5 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & 1 & 2 \\
0 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 2 & 0\\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

This is a bit tricky, after dividing all rows so you get 1's in the pivots, you
then subtract 2 times row 3 from row 2, then you subtract 2 times row 3 from row
1, then you subtract 2 times row 2 from row 1.

27. If $A$ is a triangular matrix, when is $R = \text{rref}(A)$ equal to $I$?

_Solution:_

$R = I$ when $A$ is a square invertible matrix. In this case, since $A$ is
triangular, this means that all values along the main diagonal must be nonzero.

28. Apply Gauss-Jordan elimination to $Ux = \mathbf{0}$ and $Ux = c$. Reach
    $Rx = \mathbf{0}$ and $Rx = d$:

$$
\left[\begin{array}{cc}
U & \mathbf{0} \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 2 & 3 & \mathbf{0} \\
0 & 0 & 4 & \mathbf{0} \\
\end{array}\right]
$$

and

$$
\left[\begin{array}{cc}
U & c \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 2 & 3 & 5 \\
0 & 0 & 4 & 8 \\
\end{array}\right]
$$

Solve $Rx = \mathbf{0}$ to find $x_n$ (its free variable is $x_2 = 1$). Solve
$Rx = d$ to find $x_p$ (its free variable is $x_2 = 0$).

Omitted.

29. Apply Gauss-Jordan elimination to reduce to $Rx = \mathbf{0}$ and $Rx = d$:

$$
\left[\begin{array}{cc}
& \\
U & 0 \\
& \\
\end{array}\right] =
\left[\begin{array}{cccc}
3 & 0 & 6 & \mathbf{0} \\
0 & 0 & 2 & \mathbf{0} \\
0 & 0 & 0 & \mathbf{0} \\
\end{array}\right]
$$

and

$$
\left[\begin{array}{cc}
& \\
U & c \\
& \\
\end{array}\right] =
\left[\begin{array}{cccc}
3 & 0 & 6 & 9 \\
0 & 0 & 2 & 4 \\
0 & 0 & 0 & 5 \\
\end{array}\right]
$$

Solve $Ux = \mathbf{0}$ or $Rx = \mathbf{0}$ to find $x_n$ (free variable
$= 1$). What are the solutions to $Rx = d$?

Omitted.

30. Reduce to $Ux = c$ (Gaussian elimination) and then $Rx = d$ (Gauss-Jordan):

$$ Ax =
\left[\begin{array}{cccc}
1 & 0 & 2 & 3 \\
1 & 3 & 2 & 0 \\
2 & 0 & 4 & 9 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\\x_4\end{bmatrix} =
\begin{bmatrix}{}2\\5\\10\end{bmatrix} = b
$$

Find a particular solution $x_p$ and all homogeneous solutions $x_n$.

Omitted.

31. Find matrices $A$ and $B$ with the given property or explain why you can't:

a. The only solution of $Ax = \begin{bmatrix}{}1\\2\\3\end{bmatrix}$ is
$x = \begin{bmatrix}{}0\\1\end{bmatrix}$.

_Solution:_

With $b = \begin{bmatrix}{}1\\2\\3\end{bmatrix}$ and
$x = \begin{bmatrix}{}0\\1\end{bmatrix}$, these indicate that $A$ is a 3 by 2
matrix. Since there is 1 solution, this indicates that the nullspace only has
$\mathbf{0}$, and thus there are no free variables. Consider:

$$ A =
\left[\begin{array}{ccc}
1 & 1 \\
0 & 2 \\
0 & 3 \\
\end{array}\right]
$$

Here, we have 2 pivots, no free variables, so check $Ax$:

$$ Ax =
\left[\begin{array}{ccc}
1 & 1 \\
0 & 2 \\
0 & 3 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\end{bmatrix} =
\left[\begin{array}{c}
1 \\
2 \\
3 \\
\end{array}\right] = b
$$

b. The only solution of $Bx = \begin{bmatrix}{}0\\1\end{bmatrix}$ is
$x = \begin{bmatrix}{}1\\2\\3\end{bmatrix}$.

_Solution:_

Since there is $1$ solution, this means that $r = n$

To get $b = \begin{bmatrix}{}0\\1\end{bmatrix}$, the dimensions of $Bx$ must
result in a $m = 2, n = 1$ matrix. Since $x$ is a 3 by 1 matrix, this means that
the dimensions of $Bx$ are expressed as $(2 \times n_1) \times (3 \times 1)$.
Thus $B$ must be a $2 \times 3$ matrix (as it must be the case that $n_1 = 3$).

But for there to be 1 solution, $r = n$, or in this case $r = 3$. But the amount
of rows in $B$ is 2, $m = 2$, so it must be that $r \leq 2$, and thus
$r \neq 3$. This contradicts the requirement for a single solution, and thus
this is not possible.

32. Find the $LU$ factorization of $A$ and the complete solution to $Ax = b$:

$$ A =
\left[\begin{array}{ccc}
1 & 3 & 1 \\
1 & 2 & 3 \\
2 & 4 & 6 \\
1 & 1 & 5 \\
\end{array}\right]
$$

and

$$ b =
\begin{bmatrix}{}1\\3\\6\\5\end{bmatrix}
$$

and then

$$ b =
\begin{bmatrix}{}1\\0\\0\\0\end{bmatrix}
$$

Omitted.

33. The complete solution to $Ax = \begin{bmatrix}{}1\\3\end{bmatrix}$ is
    $x = \begin{bmatrix}{}1\\0\end{bmatrix} + c\begin{bmatrix}{}0\\1\end{bmatrix}$.
    Find $A$.

Omitted.

---

Page 186

## Problem Set 3.4

**Questions 1-10 are about linear independence and linear dependence.**

1. Show that $v_1, v_2, v_3$ are independent but $v_1, v_2, v_3, v_4$ are
   dependent:

$$ v_1 = \begin{bmatrix}{}1\\0\\0\end{bmatrix} \quad v_2 = \begin{bmatrix}{}1\\1\\0\end{bmatrix} \quad v_3 = \begin{bmatrix}{}1\\1\\1\end{bmatrix} \quad v_4 = \begin{bmatrix}{}2\\3\\4\end{bmatrix} $$

Solve $c_1v_1 + c_2v_2 + c_3v_3 + c_4v_4 = \mathbf{0}$ or $Ax = \mathbf{0}$. The
$v$'s go in the columns of $A$.

_Solution:_

_Show that $v_1, v_2, v_3$ are independent:_

Line the first three $v$'s up as columns in a matrix and set them to $0$:

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = 0
$$

Since this is already in $R$ form, this can only be true where
$c_1 = c_2 = c_3 = 0$, and thus $v_1, v_2, v_3$ are independent.

_but $v_1, v_2, v_3, v_4$ are dependent:_

Similar to before, set these up in a matrix:

$$
\left[\begin{array}{ccc}
1 & 1 & 1 & 2 \\
0 & 1 & 1 & 3 \\
0 & 0 & 1 & 4 \\
\end{array}\right] =
\begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

Notice now that we are left with a free column (column 4), so our nullspace is
not only $\mathbf{0}$. This indicates that $v_1, v_2, v_3, v_4$ are dependent.
This will be demonstrated by solving for the $c$ vector in the next part.

_Solve $c_1v_1 + c_2v_2 + c_3v_3 + c_4v_4 = \mathbf{0}$ or $Ax = \mathbf{0}$:_

$$
\left[\begin{array}{ccc}
1 & 1 & 1 & 2 \\
0 & 1 & 1 & 3 \\
0 & 0 & 1 & 4 \\
\end{array}\right] =
\begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

$$
x + y + z + 2a = 0 \\
y + z + 3a = 0 \\
z + 4a = 0 \\
$$

Set $a = 1$:

$$ z + 4a = 0 \Rightarrow z + 4(1) = 0 \Rightarrow z + 4 = 0 \Rightarrow z = -4 $$

$$ y + z + 3a = 0 \Rightarrow y + (-4) + 3(1) = 0 \Rightarrow y - 4 + 3 = 0 \Rightarrow y - 1 = 0 \Rightarrow y = 1 $$

$$ x + y + z + 2a = 0 \Rightarrow x + (1) + (-4) + 2(1) = 0 \Rightarrow x + 1 - 4 + 2 = 0 \Rightarrow x - 1 = 0 \Rightarrow x = 1 $$

So $c_1v_1 + c_2v_2 + c_3v_3 + c_4v_4 = \mathbf{0}$ is solved by
$\begin{bmatrix}{}1\\1\\-4\\1\end{bmatrix}$.

2. (Recommended) Find the largest possible of independent vectors among

$$ v_1 =
\begin{bmatrix}{}1\\-1\\0\\0\end{bmatrix}
$$

$$ v_2 =
\begin{bmatrix}{}1\\0\\-1\\0\end{bmatrix}
$$

$$ v_3 =
\begin{bmatrix}{}1\\0\\0\\-1\end{bmatrix}
$$

$$ v_4 =
\begin{bmatrix}{}0\\1\\-1\\0\end{bmatrix}
$$

$$ v_5 =
\begin{bmatrix}{}0\\1\\0\\-1\end{bmatrix}
$$

$$ v_6 =
\begin{bmatrix}{}0\\0\\1\\-1\end{bmatrix}
$$

_Solution:_

$$
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & -1 \\
\end{array}\right]
$$

So $v_1, v_2, v_3$ are independent, adding any further vectors, or taking other
combinations of the other vectors, introduces dependence. The reason for this is
that each vector is in $\R^4$. Taking linear combinations can only ever add to
$\mathbf{0}$ for vectors to be independent. Notice that adding any of the other
vectors would immediately cause one of the columns to be free, violating the
definition for independence that only $\mathbf{0}$ can span the nullspace.

3. Prove that if $a = 0$ or $d = 0$ or $f = 0$ (3 cases), the columns of $U$ are
   dependent:

$$ U =
\left[\begin{array}{ccc}
a & b & c \\
0 & d & e \\
0 & 0 & f \\
\end{array}\right]
$$

**Proof:**

Suppose $U$ is a matrix defined as follows:

$$ U =
\left[\begin{array}{ccc}
a & b & c \\
0 & d & e \\
0 & 0 & f \\
\end{array}\right]
$$

It is to be shown that if $a = 0$, or if $d = 0$, or if $f = 0$, then the
columns of $U$ are dependent.

_Case ($a = 0$):

In the case that $a = 0$, $U$ becomes:

$$ U =
\left[\begin{array}{ccc}
0 & b & c \\
0 & d & e \\
0 & 0 & f \\
\end{array}\right]
$$

By the definition of independence on 3 vectors in $\R^3$,
$c_1v_1 + c_2v_2 + c_3v_3 = \mathbf{0}$, the vectors are independent if, and
only if, they satisfy $Uc = 0$ where every $c$ equals $0$. But notice that
$v_1 = \mathbf{0}$ in $U$. Any coefficient multiplied by $\mathbf{0}$ equals
$\mathbf{0}$, violating that every $c$ equals $0$. It can be concluded that the
entire set (of columns) is dependent.

_Case ($d = 0$):

In the case that $d = 0$, $U$ becomes:

$$ U =
\left[\begin{array}{ccc}
a & b & c \\
0 & 0 & e \\
0 & 0 & f \\
\end{array}\right]
$$

In this case $v_2$ is a free column, producing a special solution other than
$\mathbf{0}$ that occupies the nullspace. Thus any $c_2$ can be chosen to
multiply $v_2$ as follows: $c_2v_2 = 0$. This, once again, violates the
definition of independence that $c = 0$ for every coefficient that satisfies
$Ux = 0$. It can be concluded that the entire set of columns is dependent.

_Case ($f = 0$):

In the case that $f = 0$, $U$ becomes:

$$ U =
\left[\begin{array}{ccc}
a & b & c \\
0 & d & e \\
0 & 0 & 0 \\
\end{array}\right]
$$

Here $v_3$ is a free column, and similar reasoning applies as was in the
previous case of $d = 0$.

_Conclusion:_

Since all three cases have been demonstrated, it can be concluded that when
$a = 0$, or $d = 0$, or $f = 0$, that the three columns of $U$ are dependent.
This is what was to be shown.

Q.E.D.

4. If $a, d, f$ in Question 3 are all nonzero, show that the only solution to
   $Ux = \mathbf{0}$ is $x = \mathbf{0}$. Then the upper triangular $U$ has
   independent columns.

_Solution:_

**Proof:**

Suppose $U$ is a matrix defined as follows:

$$ U =
\left[\begin{array}{ccc}
a & b & c \\
0 & d & e \\
0 & 0 & f \\
\end{array}\right]
$$

Furthermore, suppose $a \neq 0, d \neq 0, f \neq 0$.

It is to be shown that the only solution to $Ux = \mathbf{0}$ is
$x = \mathbf{0}$.

Consider:

$$ Ux =
\left[\begin{array}{ccc}
a & b & c \\
0 & d & e \\
0 & 0 & f \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} =
\begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

By matrix multiplication this becomes the following algebraic expressions:

$$
ax_1 + bx_2 + cx_3 = 0 \\
0x_1 + dx_2 + ex_3 = 0 \\
0x_1 + 0x_2 + fx_3 = 0 \\
$$

$$
ax_1 + bx_2 + cx_3 = 0 \\
dx_2 + ex_3 = 0 \\
fx_3 = 0 \\
$$

Since, by the supposition, $f \neq 0$, it follows that $fx_3 = 0 \to x_3 = 0$.

Then, since $x_3 = 0$, and since (by the supposition) $d \neq 0$, it follows
that $dx_2 + ex_3 = 0 \to dx_2 + e(0) = 0 \to dx_2 = 0 \to x_2 = 0$.

Then, since $x_2 = 0$, and since (by the supposition) $a \neq 0$, it follows
that
$ax_1 + bx_2 + cx_3 = 0 \to ax_1 + b(0) + c(0) = 0 \to ax_1 = 0 \to x_1 = 0$.

Combining these solutions into the final vector $x$ yields
$x = \begin{bmatrix}{}0\\0\\0\end{bmatrix}$, and thus $x = \mathbf{0}$.

This is what was to be shown.

Q.E.D.

5. Decide the dependence or independence of

a. the vectors $(1, 3, 2)$ and $(2, 1, 3)$ and $(3, 2, 1)$

_Solution:_

Set them up in a matrix.

$$
\left[\begin{array}{ccc}
1 & 2 & 3 \\
3 & 1 & 2 \\
2 & 3 & 1 \\
\end{array}\right]
$$

Note here you can either eliminate or find the determinant, (elimination leading
to $0$ rows or to free columns means dependent, determinant equal $0$ means
dependent). Here, I go with elimination:

$$
\left[\begin{array}{ccc}
1 & 2 & 3 \\
3 & 1 & 2 \\
2 & 3 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -5 & -7 \\
2 & 3 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -5 & -7 \\
0 & -1 & -5 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -5 & -7 \\
0 & 0 & -\frac{18}{5} \\
\end{array}\right]
$$

Since elimination yields no free variables, we can conclude that these vectors
are independent.

b. the vectors $(1, -3, 2)$ and $(2, 1, -3)$ and $(-3, 2, 1)$.

_Solution:_

Again, we set up a matrix with each vector being a column:

$$
\left[\begin{array}{rrr}
1 & 2 & -3 \\
-3 & 1 & 2 \\
2 & -3 & 1 \\
\end{array}\right]
$$

Once again, we eliminate:

$$
\left[\begin{array}{rrr}
1 & 2 & -3 \\
-3 & 1 & 2 \\
2 & -3 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -3 \\
0 & 7 & -7 \\
2 & -3 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -3 \\
0 & 7 & -7 \\
0 & -7 & 7 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -3 \\
0 & 7 & -7 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Here, the third row yielding $0$ means that the third row was a linear
combination of one or both of the other two rows, indicating that these vectors
are dependent.

6. Choose three independent columns of $U$. Then make two other choices. Do the
   same for $A$.

$$ U =
\left[\begin{array}{cccc}
2 & 3 & 4 & 1 \\
0 & 6 & 7 & 0 \\
0 & 0 & 0 & 9 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{cccc}
2 & 3 & 4 & 1 \\
0 & 6 & 7 & 0 \\
0 & 0 & 0 & 9 \\
4 & 6 & 8 & 2 \\
\end{array}\right]
$$

_Solution:_

_Choose three independent columns of $U$. Then make two other choices:_

$$ U =
\left[\begin{array}{cccc}
2 & 3 & 4 & 1 \\
0 & 6 & 7 & 0 \\
0 & 0 & 0 & 9 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

Choices are denoted $C_1, C_2, C_3$.

$C_1$:

$$ C_1 = \left\{\begin{bmatrix}{}2\\0\\0\\0\end{bmatrix}, \begin{bmatrix}{}3\\6\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\0\end{bmatrix}\right\} $$

$C_2$:

$$ C_2 = \left\{\begin{bmatrix}{}2\\0\\0\\0\end{bmatrix}, \begin{bmatrix}{}4\\7\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\0\end{bmatrix}\right\} $$

$C_3$:

$$ C_3 = \left\{\begin{bmatrix}{}3\\6\\0\\0\end{bmatrix}, \begin{bmatrix}{}4\\7\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\0\end{bmatrix}\right\} $$

_Do the same for $A$:_

$$ A =
\left[\begin{array}{cccc}
2 & 3 & 4 & 1 \\
0 & 6 & 7 & 0 \\
0 & 0 & 0 & 9 \\
4 & 6 & 8 & 2 \\
\end{array}\right]
$$

Choices are denoted $C_1, C_2, C_3$.

$C_1$:

$$ C_1 = \left\{\begin{bmatrix}{}2\\0\\0\\4\end{bmatrix}, \begin{bmatrix}{}3\\6\\0\\6\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\2\end{bmatrix}\right\}$$

$C_2$:

$$ C_2 = \left\{\begin{bmatrix}{}2\\0\\0\\4\end{bmatrix}, \begin{bmatrix}{}4\\7\\0\\8\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\2\end{bmatrix}\right\}$$

$C_3$:

$$ C_3 = \left\{\begin{bmatrix}{}3\\6\\0\\6\end{bmatrix}, \begin{bmatrix}{}4\\7\\0\\8\end{bmatrix}, \begin{bmatrix}{}1\\0\\9\\2\end{bmatrix}\right\}$$

Notice that the column choices for $A$ are the same as for $U$ (since $A$
eliminates to $U$).

7. If $w_1, w_2, w_3$ are independent vectors, show that the differences
   $v_1 = w_2 - w_3$ and $v_2 = w_1 - w_3$ and $v_3 = w_1 - w_2$ are
   _dependent_. Find a combination of the $v$'s that gives zero. Which matrix
   $A$ in
   $\left[\begin{array}{ccc}v_1 & v_2 & v_3 \\\end{array}\right] = \left[\begin{array}{ccc}w_1 & w_2 & w_3 \\\end{array}\right]$
   $A$ is singular?

_Solution:_

_If $w_1, w_2, w_3$ are independent vectors, show that the differences
$v_1 = w_2 - w_3$ and $v_2 = w_1 - w_3$ and $v_3 = w_1 - w_2$ are dependent:_

**Proof:**

Suppose $w_1, w_2, w_3$ are independent vectors.

It is to be shown that the differences $v_1 = w_2 - w_3$, $v_2 = w_1 - w_3$, and
$v_3 = w_1 - w_2$ are dependent.

By definition of dependence, this means that it is to be shown that:

$$ c_1v_1 + c_2v_2 + c_3v_3 = \mathbf{0} $$

Where at least one of the following inequalities must hold: $c_1 \neq 0$, or
$c_2 \neq 0$ or $c_3 \neq 0$.

Now, by substitution of the differences into the linear combination above, this
yields:

$$ c_1(w_2 - w_3) + c_2(w_1 - w_3) + c_3(w_1 - w_2) = \mathbf{0} $$

By distribution:

$$ c_1w_2 - c_1w_3 + c_2w_1 - c_2w_3 + c_3w_1 - c_3w_2 = \mathbf{0} $$

Now, group by $w$'s and factor:

$$ c_1w_2 - c_3w_2 - c_1w_3 - c_2w_3 + c_2w_1 + c_3w_1 = \mathbf{0} $$

$$ w_2(c_1 - c_3) - w_3(c_1 + c_2) + w_1(c_2 + c_3) = \mathbf{0} $$

By the supposition, since $w_1, w_2, w_3$ are independent, this means that
$c_1 - c_3 = 0$, $c_1 + c_2 = 0$ and $c_2 + c_3 = 0$.

Evaluating each of these yields:

$$ c_1 - c_3 = 0 \to c_1 = c_3 $$

$$ c_1 + c_2 = 0 \to c_1 = -c_2 $$

$$ c_2 + c_3 = 0 \to c_2 = -c_3 $$

This is true, considering that:

$$ c_2 = -c_3 \to c_1 = -(-c_3) \to c_1 = c_3 $$

So these equalities hold.

Let $t \in \mathbf{R}$ with $t \neq 0$, then:

$$ c_1 = c_3 = t, c_2 = -t $$

It can be concluded that there exists some nonzero number $t$ which is equal to
$c_1, c_3$, and it's negative $-t$ equals $c_2$, and thus the difference vectors
$v_1, v_2, v_3$ are dependent.

This is what was to be shown.

Q.E.D.

_Find a combination of the $v$'s that gives zero:_

Consider:

$$ v_1 - v_2 + v_3 $$

Then, by substitution:

$$ (w_2 - w_3) - (w_1 - w_3) + (w_1 - w_2) $$

$$ w_2 - w_3 - w_1 + w_3 + w_1 - w_2 $$

$$ = \mathbf{0} $$

_Which matrix $A$ in
$\left[\begin{array}{ccc}v_1 & v_2 & v_3 \\\end{array}\right] = \left[\begin{array}{ccc}w_1 & w_2 & w_3 \\\end{array}\right]$
$A$ is singular?:_

Think carefully on what each $v$ means in terms of $w$, each $v$ is a difference
of $w$, so construct a 3 by 3 matrix with this into account.

$$ A =
\left[\begin{array}{ccc}
v_1 & v_2 & v_3 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
(w_2 - w_3) & (w_1 - w_3) & (w_1 - w_2) \\
\end{array}\right]
$$

We are thus trying to find some $A$ that satisfies:

$$ A =
\left[\begin{array}{ccc}
(w_2 - w_3) & (w_1 - w_3) & (w_1 - w_2) \\
\end{array}\right] =
\left[\begin{array}{ccc}
w_1 & w_2 & w_3 \\
\end{array}\right]
$$

Let's consider the first $v_1$:

$$ v_1 = w_2 - w_3 \to v_1 = 0w_1 + 1w_2 + (-1)w_3 \to v_1 = \begin{bmatrix}{}0\\1\\-1\end{bmatrix} $$

As shown above, since $v$ is a vector/column, express this as
$v_1 = \begin{bmatrix}{}0\\1\\-1\end{bmatrix}$.

Similarly for $v_2, v_3$:

$$ v_2 = w_1 - w_3 \to v_2 = 1w_1 + 0w_2 + (-1)w_3 \to v_2 = \begin{bmatrix}{}1\\0\\-1\end{bmatrix} $$

$$ v_3 = w_1 - w_2 \to v_2 = 1w_1 + (-1)w_2 + 0w_3 \to v_3 = \begin{bmatrix}{}1\\-1\\0\end{bmatrix} $$

And so our final $A$ is:

$$ A =
\left[\begin{array}{rrr}
0 & 1 & 1 \\
1 & 0 & -1 \\
-1 & -1 & 0 \\
\end{array}\right]
$$

Note that this combined with our proof shows that if $A$ has dependent columns,
then $A$ is singular.

8. If $w_1, w_2, w_3$ are independent vectors, show that the sums
   $v_1 = w_2 + w_3$ and $v_2 = w_1 + w_3$ and $v_3 = w_1 + w_2$ are
   _independent_. (Write $c_1v_1 + c_2v_2 + c_3v_2 = \mathbf{0}$ in terms of the
   $w$'s. Find and solve equations for the $c$'s, to show they are zero.)

Omitted.

9. Suppose $v_1, v_2, v_3, v_4$ are vectors in $\R^3$.

a. These four vectors are dependent because ____.

These vectors, when lined up in a matrix, form a 3 by 4 matrix. This indicates
that after elimination, at least one column is eliminated to a free column. Thus
the nullspace is not spanned solely by $\mathbf{0}$, which is a clear indicator
that the vectors are dependent.

b. The two vectors $v_1$ and $v_2$ will be dependent if ____.

When set up in a simple block matrix:

$$
\left[\begin{array}{cc}
v_1 & v_2 \\
\end{array}\right]
$$

If this matrix has rank $0$ or rank $1$, then there will be a free
column/variable, and again, the nullspace will not be spanned solely by
$\mathbf{0}$, and thus the two vectors will then be dependent.

c. The vectors $v_1$ and $(0, 0, 0)$ are dependent because ____.

Consider:

$$ c_1v_1 + c_2\begin{bmatrix}{}0\\0\\0\end{bmatrix} = \mathbf{0} $$

This means that $v_1$ and $(0, 0, 0)$ are dependent since it is certainly
possible that $c_2 \neq 0$.

10. Find two independent vectors on the plane $x + 2y - 3z - t = 0$ in $\R^4$.
    Then find three independent vectors. Why not four? This plane is the
    nullspace of what matrix?

_Solution:_

_Find two independent vectors on the plane $x + 2y - 3z - t = 0$ in $\R^4$:_

Simply solving this equation will give vectors in the nullspace, just make sure
that the two solutions you come up with aren't a linear combination of the
other.

Let $y = 1$, then:

$$ x + 2(1) - 3z - t = 0 $$

$$ x - 3z - t + 2 = 0 $$

$$ x - 3z - t = -2 $$

Then let $z = 0$:

$$ x - 3(0) - t = -2 $$

$$ x - t = -2 $$

Then let $t = 0$:

$$ x - 0 = -2 $$

$$ x = -2 $$

So one vector that lies on the plane is
$\begin{bmatrix}{}-2\\1\\0\\0\end{bmatrix}$.

Now, to find the other vector and to ensure it's independent of this first one,
assign from the other end of the variables, in other words, let $t = 1$:

$$ x + 2y - 3z - t = 0 $$

$$ x + 2y - 3z - (1) = 0 $$

$$ x + 2y - 3z = 1 $$

Now, let $z = 0$:

$$ x + 2y - 3(0) = 1 $$

$$ x + 2y = 1 $$

Now, let $y = 0$:

$$ x + 2(0) = 1 $$

$$ x = 1 $$

So another vector is $\begin{bmatrix}{}1\\0\\0\\1\end{bmatrix}$.

Consider that they are independent:

$$ \begin{bmatrix}{}-2\\1\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\0\\0\\1\end{bmatrix} $$

_Then find three independent vectors:_

Another third independent vector can be found by setting $z = 1$, and then
evaluating from there:

$$ x + 2y - 3z - t = 0 $$

$$ x + 2y - 3(1) - t = 0 $$

$$ x + 2y - 3 - t = 0 $$

$$ x + 2y - t = 3 $$

Now set $t = 0$

$$ x + 2y - 0 = 3 $$

$$ x + 2y = 3 $$

And now set $y = 0$:

$$ x + 2(0) = 3 $$

$$ x = 3 $$

And so a third vector is $\begin{bmatrix}{}3\\0\\1\\0\end{bmatrix}$.

Consider all three for independence:

$$ \begin{bmatrix}{}-2\\1\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\0\\0\\1\end{bmatrix}, \begin{bmatrix}{}3\\0\\1\\0\end{bmatrix} $$

_Why not four?:_

There are only three free variables available in any given evaluation for a
special solution (as done above), the fourth variable is determined by the
choices of the previous three variables. This indicates that the nullspace is
occupied by 3 special solution vectors (aside from $\mathbf{0}$), and cannot be
occupied by a fourth.

_This plane is the nullspace of what matrix?:_

This is asking us to find an $A$ such that:

$$ Ax = \mathbf{0} $$

$$ Ax
\left[\begin{array}{rrrr}
1 & 2 & -3 & -1 \\
\end{array}\right]
\begin{bmatrix}{}x\\y\\z\\t\end{bmatrix} =
\mathbf{0}
$$

Thus $A$ is:

$$ A =
\left[\begin{array}{rrrr}
1 & 2 & -3 & -1 \\
\end{array}\right]
$$

**Questions 11-14 are about the space _spanned_ by a set of vectors. Take all
linear combinations of the vectors.**

11. Describe the subspace of $\R^3$ (is it a line or plane or $\R^3$?) spanned
    by

a. the two vectors $(1, 1, -1)$ and $(-1, -1, 1)$

Consider:

$$ c_1\begin{bmatrix}{}1\\1\\-1\end{bmatrix} + c_2\begin{bmatrix}{}-1\\-1\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}c_1 - c_2\\c_1 - c_2\\-c_1 + c_2\end{bmatrix} $$

This can be factored as:

$$ = (c_1 - c_2)\begin{bmatrix}{}1\\1\\-1\end{bmatrix} $$

Thus these two vectors share a scalar multiple (namely $c_1 - c_2$), and they
span a line within $\R^3$.

b. the three vectors $(0, 1, 1)$ and $(1, 1, 0)$ and $(0, 0, 0)$

$$ c_1\begin{bmatrix}{}0\\1\\1\end{bmatrix} + c_2\begin{bmatrix}{}1\\1\\0\end{bmatrix} + c_3\begin{bmatrix}{}0\\0\\0\end{bmatrix} $$

$$ = \begin{bmatrix}{}c_2\\c_1 + c_2\\c_1\end{bmatrix} $$

Notice that the linear combination of these three vectors has a second component
that depends on the addition of the first two, thus we cannot freely choose our
second coordinate. It follows that only $c_1, c_2$ are freely chosen, and it can
be concluded that these vectors span a plane within $\R^3$.

c. all vectors in $\R^3$ with whole number components

These vectors will span all of $\R^3$.

d. all vectors with positive components

These vectors will span all of $\R^3$.

12. The vector $b$ is in the subspace spanned by the columns of $A$ when ____
    has a solution. The vector $c$ is in the row space of $A$ when ____ has a
    solution.

_True or false_: If the zero vector is in the row space, the rows are dependent.

_Solution:_

When $Ax = b$ has a solution; When $A^{\mathbf{T}}y = c$ has a solution.

False, the zero vector is always in the row space.

13. Find the dimensions of these 4 spaces. Which two of the spaces are the same?
    (a) column space of $A$, (b) column space of $U$, \(c\) row space of $A$,
    (d) row space of $U$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 3 & 1 \\
3 & 1 & -1 \\
\end{array}\right]
$$

and

$$ U =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

**Solution:**

a.

$$ A =
\left[\begin{array}{rrr}
1 & 1 & 0 \\
1 & 3 & 1 \\
3 & 1 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & 2 & 1 \\
3 & 1 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & -2 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

$$ U =
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & 2 & 1 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & 1 & \frac{1}{2} \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & \frac{1}{2} \\
0 & 0 & 0 \\
\end{array}\right] = R
$$

Our pivot columns are columns $1$ and $2$ from $A$, thus $C(A)$ is:

$$ C(A) = \left\{\begin{bmatrix}{}1\\1\\3\end{bmatrix}, \begin{bmatrix}{}1\\3\\1\end{bmatrix}\right\} $$

b. Notice that we eliminated $A$ to get $U$ in part (a), thus we can apply the
reasoning of from our derived $R$ to find $C(U)$:

$$ C(U) = \left\{\begin{bmatrix}{}1\\0\\0\end{bmatrix}, \begin{bmatrix}{}1\\2\\1\end{bmatrix}\right\} $$

c. Recall that finding the row space of $A$ is simply finding the column space
of $A^{\mathbf{T}}$.

$$ R(A) = C(A^{\mathbf{T}}) $$

So first, find $A^{\mathbf{T}}$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 1 & 3 \\
1 & 3 & 1 \\
0 & 1 & -1 \\
\end{array}\right]
$$

And now eliminate to $U$ and $R$:

$$ A^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 1 & 3 \\
1 & 3 & 1 \\
0 & 1 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 3 \\
0 & 2 & -2 \\
0 & 1 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 3 \\
0 & 2 & -2 \\
0 & 0 & 0 \\
\end{array}\right] = U
$$

$$ U =
\left[\begin{array}{rrr}
1 & 1 & 3 \\
0 & 2 & -2 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 3 \\
0 & 1 & -1 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 0 & 4 \\
0 & 1 & -1 \\
0 & 0 & 0 \\
\end{array}\right] = R
$$

Thus we have pivots in columns 1 and 2 of $A^{\mathbf{T}}$, so:

$$ A^{\mathbf{T}} =
\left[\begin{array}{rrr}
1 & 1 & 3 \\
1 & 3 & 1 \\
0 & 1 & -1 \\
\end{array}\right]
$$

$$ R(A) = C(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\1\\0\end{bmatrix}, \begin{bmatrix}{}1\\3\\1\end{bmatrix}\right\} $$

d. Find the transpose of $U$ first:

$$ U^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 2 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

Now find the upper echelon form of this (denoted $U_e$, I know its confusing but
just go with it):

$$ U^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 2 & 0 \\
0 & 1 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 1 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 0 \\
\end{array}\right] = U_e
$$

Now find $R$:

$$ U_e =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right] = R
$$

Once again, our pivots are in columns 1 and 2, so find them from
$U^{\mathbf{T}}$:

$$ R(U) = C(U^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\1\\0\end{bmatrix}, \begin{bmatrix}{}0\\2\\1\end{bmatrix}\right\} $$

_Conclusion:_

The dimensions of all spaces are 2 (because the pivots in all cases are 2). The
$R(A) = R(U)$ since:

$$ 1\begin{bmatrix}{}1\\1\\0\end{bmatrix} + 1\begin{bmatrix}{}0\\2\\1\end{bmatrix} = \begin{bmatrix}{}1\\3\\1\end{bmatrix} \in R(A) $$

and:

$$ 1\begin{bmatrix}{}1\\3\\1\end{bmatrix} - 1\begin{bmatrix}{}0\\2\\1\end{bmatrix} = \begin{bmatrix}{}1\\1\\0\end{bmatrix} \in R(U) $$

14. $v + w$ and $v - w$ are combinations of $v$ and $w$. Write $v$ and $w$ as
    combinations of $v + w$ and $v - w$. The two pairs of vectors ____ the same
    space. When are they a basis for the same space?

_Solution:_

_Write $v$ and $w$ as combinations of $v + w$ and $v - w$:_

$$ (v + w) + (v - w) $$

$$ = v + w + v - w $$

$$ = 2v $$

This means that:

$$ 2v = (v + w) + (v - w) $$

$$ v = \frac{1}{2}[(v + w) + (v - w)] $$

Similarly:

$$ (v + w) - (v - w) $$

$$ = v + w - v + w $$

$$ = 2w $$

Which means that:

$$ 2w = (v + w) - (v - w) $$

$$ w = \frac{1}{2}[(v + w) - (v - w)] $$

_The two pairs of vectors ____ the same space:_

span

_When are they a basis for the same space?:_

They are a basis when $v$ and $w$ are independent.

(LEFT OFF HERE)

**Questions 15-25 are about the requirements for a basis.**

15. If $v_1, \dots, v_n$ are linearly independent, the space they span has
    dimension ____. These vectors are a ____ for that space. If the vectors are
    the columns of an $m$ by $n$ matrix, then $m$ is ____ than $m$. If $m = n$,
    that matrix is ____.

16. Find a basis for each of these subspaces of $\R^4$:

a. All vectors whose components are equal.

b. All vectors whose components add to zero.

c. All vectors that are perpendicular to $(1, 1, 0, 0)$ and $(1, 0, 1, 1)$.

d. The column space and the nullspace of $I$ (4 by 4).

17. Find three different bases for the column space of
    $U = \left[\begin{array}{ccccc}1 & 0 & 1 & 0 & 1 \\0 & 1 & 0 & 1 & 0  \\\end{array}\right]$.
    Then find two different bases for the row space of $U$.

18. Suppose $v_1, v_2, \dots, v_6$ are six vectors in $\R^4$.

a. Those vectors (do)(do not)(might not) span $\R^4$.

b. Those vectors (are)(are not)(might be) linearly independent.

c. Any four of those vectors (are)(are not)(might be) a basis for $\R^4$.

19. The columns of $A$ are $n$ vectors from $\R^m$. If they are linearly
    independent, what is the rank of $A$? If they span $\R^m$, what is the rank?
    If they are a basis for $\R^m$, what then? _Looking ahead_: The rank $r$
    counts the number of ____ columns.

20. Find a basis for the plane $x - 2y + 3z = 0$ in $\R^3$. Then find a basis
    for the intersection of that plane with the $xy$ plane. Then find a basis
    for all vectors perpendicular to the plane.

21. Suppose the columns of a 5 by 5 matrix $A$ are the basis for $\R^5$.

a. The equation $Ax = \mathbf{0}$ has only the solution $x = 0$ because ____.

b. If $b$ is in $\R^5$ then $Ax = b$ is solvable because the basis vectors ____
$\R^5$.

Conclusion: $A$ is invertible. Its rank is $5$. Its rows are also a basis for
$\R^5$.

22. Suppose $\mathbf{S}$ is a 5-dimensional subspace of $\R^6$. True or false
    (example if false):

a. Every basis for $\mathbf{S}$ can be extended to a basis for $\R^6$ by adding
one more vector.

b. Every basis for $\R^6$ can be reduced to a basis for $\mathbf{S}$ by removing
one vector.

23. $U$ comes from $A$ by subtracting row 1 from row 3:

$$ A =
\left[\begin{array}{ccc}
1 & 3 & 2 \\
0 & 1 & 1 \\
1 & 3 & 2 \\
\end{array}\right]
$$

and

$$ U =
\left[\begin{array}{cc|c}
1 & 3 & 2 \\
0 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Find the bases for the two column spaces. Find bases for the two row spaces.
Find bases for the two nullspaces. Which spaces stay fixed in elimination?

24. True or false (give a good reason):

a. If the columns of a matrix are dependent, so are the rows.

b. The column space of a 2 by 2 matrix is the same as its row space.

c. The column space of a 2 by 2 matrix has the same dimension as its row space.

d. The columns of a matrix are a basis for the column space.

25. For which numbers $c$ and $d$ do these matrices have rank $2$?

$$ A =
\left[\begin{array}{ccccc}
1 & 2 & 5 & 0 & 5 \\
0 & 0 & c & 2 & 2 \\
0 & 0 & 0 & d & 2 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cc}
c & d \\
d & c \\
\end{array}\right]
$$

**Questions 26-30 are about spaces where the "vectors" are matrices.**

a. All diagonal matrices.

b. All symmetric matrices ($A^{\mathbf{T}} = A$).

c. All skew-symmetric matrices ($A^{\mathbf{T}} = -A$).

27. Construct six linearly independent 3 by 3 echelon matrices
    $U_1, \dots, U_6$.

28. Find a basis for the space of all 2 by 3 matrices whose columns add to zero.
    Find a basis for the subspace whose rows also add to zero.

29. What subspace of 3 by 3 matrices is spanned (take all combinations) by

a. the invertible matrices?

b. the rank one matrices?

c. the identity matrix?

30. Find a basis for the space of 2 by 3 matrices whose nullspace contains
    $(2, 1, 1)$.

**Questions 31-35 are about spaces where the "vectors" are functions.**

31.

a. Find all functions that satisfy $\dfrac{dy}{dx} = 0$.

b. Choose a particular function that satisfies $\dfrac{dy}{dx} = 3$.

c. Find all functions that satisfy $\dfrac{dy}{dx} = 3$.

32. The cosine space $\mathbf{F}_3$ contains all combinations
    $y(x) = A\cos x + B\cos 2x + C\cos 3x$. Find a basis for the subspace with
    $y(0) = 0$.

33. Find a basis for the space of functions that satisfy

a. $\dfrac{dy}{dx} - 2y = 0$

b. $\dfrac{dy}{dx} - \dfrac{y}{x} = 0$.

34. Suppose $y_1(x), y_2(x), y_3(x)$ are three different functions of $x$. The
    vector space they span could have dimension $1$, $2$, or $3$. Give an
    example of $y_1, y_2, y_3$ to show each possibility.

35. Find a basis for the space of polynomials $p(x)$ of degree $\leq 3$. Find a
    basis for the subspace with $p(1) = 0$.

36. Find a basis for the space $\mathbf{S}$ of vectors $(a, b, c, d)$ with
    $a + c + d = 0$ and also for the space $\mathbf{T}$ with $a + b = 0$ and
    $c = 2d$. What is the dimension of the intersection
    $\mathbf{S} \cap \mathbf{T}$?

37. If $AS = SA$ for the _shift matrix_ $S$, show that $A$ must have this
    special form:

If

$$
\left[\begin{array}{ccc}
a & b & c \\
d & e & f \\
g & h & i \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
a & b & c \\
d & e & f \\
g & h & i \\
\end{array}\right]
$$

then

$$ A =
\left[\begin{array}{ccc}
a & b & c \\
0 & a & b \\
0 & 0 & a \\
\end{array}\right]
$$

"The subspace of matrices that commute with the shift $S$ has dimension ____."

38. Which of the following are bases for $\R^3$?

a. $(1, 2, 0)$ and $(0, 1, -1)$

b. $(1, 1, -1), (2, 3, 4), (4, 1, -1), (0, 1, -1)$

c. $(1, 2, 2), (-1, 2, 1), (0, 8, 0)$

d. $(1, 2, 2), (-1, 2, 1), (0, 8, 6)$

39. Suppose $A$ is a $5$ by $4$ with rank $4$. Show that $Ax = b$ has no
    solution when the $5$ by $5$ matrix
    $\left[\begin{array}{cc}A & b\\\end{array}\right]$ is invertible. Show that
    $Ax = b$ is solvable when $\left[\begin{array}{cc}A & b\\\end{array}\right]$
    is singular.

40.

a. Find a basis for all solutions to $\dfrac{d^4y}{dx^4} = y(x)$.

b. Find a particular solution to $\dfrac{d^4y}{dx^4} = y(x) + 1$. Find the
complete solution.
