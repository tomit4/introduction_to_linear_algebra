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

(LEFT OFF HERE).

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

40. If $A$ is an $m$ by $n$ matrix with $r = 1$, its columns are multiples of
    one column and its rows are multiples of one row. The column space is a ____
    in $\R^m$. The nullspace is a ____ in $\R^n$. The nullspace matrix $N$ has
    shape ____.

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

42. If $A$ is a rank one matrix, the second row of $R$ is ____. Do an example.

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

44. Suppose $P$ contains only the $r$ pivot columns of an $m$ by $n$ matrix.
    Explain why this $m$ by $r$ submatrix $P$ has rank $r$.

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

47. The rank one matrix $uv^{\mathbf{T}}$ times the rank one matrix
    $wz^{\mathbf{T}}$ is $uz^{\mathbf{T}}$ times the number ____. This product
    $uv^{\mathbf{T}}wz^{\mathbf{T}}$ also has rank one unless ____ $= 0$.

48.

a. Suppose column $j$ of $B$ is a combination of previous columns of $B$. Show
that column $j$ of $AB$ is the same combination of previous columns of $AB$.
Then $AB$ cannot have new pivot columns, so
$\textbf{rank}(AB) \leq \textbf{rank}(B)$.

b. Find $A_1$ and $A_2$ so that $\text{rank}(A_1B) = 1$ and
$\text{rank}(A_2B) = 0$ for
$B =\left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$.

49. Problem 48 proved that $\text{rank}(AB) \leq \text{rank}(B)$. Then the same
    reasoning gives
    $\text{rank}(B^{\mathbf{T}}A^{\mathbf{T}}) \leq \text{rank}(A^{\mathbf{T}})$.
    How do you deduce that $\text{rank}(AB) \leq \text{rank}A$?

50. (Important) Suppose $A$ and $B$ are $n$ by $n$ matrices, and $AB = I$. Prove
    from $\text{rank}(AB) \leq \text{rank}(A)$ that the rank of $A$ is $n$. So
    $A$ is invertible and $B$ must be its two-sided inverse (Section 2.5).
    Therefore $BA = I$ (_which is not so obvious!_)

51. If $A$ is 2 by 3 and $B$ is 3 by 2 and $AB = I$, show from its rank that
    $BA \neq I$. Give an example of $A$ and $B$ with $AB = I$. For $m < n$, a
    right inverse is not a left inverse.

52. Suppose $A$ and $B$ have the _same_ reduced row echelon form $R$.

a. Show that $A$ and $B$ have the same nullspace and the same row space.

b. We know $E_1A = R$ and $E_2B = R$. So $A$ equals an ____ matrix times $B$.

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

56. _Neat fact_ _Every $m$ by $n$ matrix of rank $r$ reduces to ($m$ by $r$)
    **times** ($r$ by $n$):_

> $A = (\text{pivot columns of } A)(\text{first } r \text{ rows of } R) = (\textbf{COL})(\textbf{ROW})$

Write the 3 by 4 matrix $A$ of all ones as the product of the 3 by 1 matrix from
the pivot columns and the 1 by 4 matrix from $R$.
