Page 213

## Problem Set 4.1

**Questions 1-12 grow out of Figures 4.2 and 4.3 with four subspaces.**

1. Construct any 2 by 3 matrix of rank one. Copy Figure 4.2 and put one vector
   in each subspace (and put two in the nullspace). Which vectors are
   orthogonal?

_Solution:_

Done by hand.

Both nullspace vectors will be orthogonal to the row space vector in $\R^3$. The
column space of $A$ and the nullspace of $A^{\mathbf{T}}$ are perpendicular
lines in $\R^2$ because rank $= 1$.

2. Redraw Figure 4.3 for a $3$ by $2$ matrix of rank $r = 2$. Which subspace is
   $\Z$ (zero vector only)? The nullspace part of any vector $x$ in $\R^2$ is
   $x_n =$ ____.

_Solution:_

Done by hand.

The nullspace of a $3$ by $2$ matrix with rank $2$ is $\Z$ (only the zero vector
because the $2$ columns are independent). So $x_n = \mathbf{0}$, and row space
$= \R^2$. Column space $=$ plane perpendicular to left nullspace $=$ line in
$\R^3$ (because the rank is $2$).

3. Construct a matrix with the required property or say why that is impossible:

a. Column space contains $\begin{bmatrix}{}1\\2\\-3\end{bmatrix}$ and
$\begin{bmatrix}{}2\\-3\\5\end{bmatrix}$, nullspace contains
$\begin{bmatrix}{}1\\1\\1\end{bmatrix}$

_Solution:_

One way is to use these columns directly, but since the nullspace has a single
vector in it, we need to have a free column.

$$ A =
\left[\begin{array}{rrr}
1 & 2 & a \\
2 & -3 & b \\
-3 & 5 & c \\
\end{array}\right]
$$

Now, if we say that the third column with $a, b, c$ is the free column, then we
can simply set $x = 1, y = 1, z = 1$ and solve for $a, b, c$ to find a matrix
that fulfills these constraints.

$$ 1x + 2y + az = 0 \Rightarrow 1 + 2 + a = 0 \Rightarrow a = -3 $$

$$ 2x - 3y + bz = 0 \Rightarrow 2(1) - 3(1) + 1b = 0 \Rightarrow -1 + b = 0 \Rightarrow b = 1 $$

$$ -3x + 5y + cz = 0 \Rightarrow -3(1) + 5(1) + 1c = 0 \Rightarrow 2 + c = 0  \Rightarrow c = -2 $$

So our final matrix $A$ that will satisfy the given constraints is:

$$ A =
\left[\begin{array}{rrr}
1 & 2 & -3 \\
2 & -3 & 1 \\
-3 & 5 & -2 \\
\end{array}\right]
$$

b. Row space contains $\begin{bmatrix}{}1\\2\\-3\end{bmatrix}$ and
$\begin{bmatrix}{}2\\-3\\5\end{bmatrix}$, nullspace contains
$\begin{bmatrix}{}1\\1\\1\end{bmatrix}$

_Solution:_

Consider that the row space is:

$$ C(A^{\mathbf{T}}) = \text{span}\left\{\begin{bmatrix}{}1\\2\\-3\end{bmatrix}, \begin{bmatrix}{}2\\-3\\5\end{bmatrix}\right\} $$

and consider that the nullspace is:

$$ N(A) = \text{span}\left\{\begin{bmatrix}{}1\\1\\1\end{bmatrix}\right\} $$

Since $C(A^{\mathbf{T}})$ is orthogonal to $N(A)$, this means that every vector
in $C(A^{\mathbf{T}})$ is perpendicular to every vector in $N(A)$, and this
means that any vector in the row space times any vector in the nullspace must
equal $0$. So, let's evaluate that:

$$
\left[\begin{array}{rrr}
1 & 2 & -3\\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = [0]
$$

So this vector $(1, 2, -3)$ is perpendicular to $(1, 1, 1)$, so far so good, now
the next one:

$$
\left[\begin{array}{rrr}
2 & -3 & 5 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = [4] \neq [0]
$$

So here we can see that constructing such a matrix for the given constraints is
not possible.

c. $Ax = \begin{bmatrix}{}1\\1\\1\end{bmatrix}$ has a solution and
$A^{\mathbf{T}}\begin{bmatrix}{}1\\0\\0\end{bmatrix} = \begin{bmatrix}{}0\\0\\0\end{bmatrix}$

_Solution:_

Since:

$$ Ax =
\begin{bmatrix}{}1\\1\\1\end{bmatrix}
$$

This means that $(1, 1, 1)$ is in $C(A)$.

Since

$$ A^{\mathbf{T}}\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

This means that $(1, 0, 0)$ is in $N(A^{\mathbf{T}})$.

It is known that $C(A)$ is orthogonal to $N(A^{\mathbf{T}})$, and thus their dot
product must be zero:

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = [1] \neq [0]
$$

Once again, as their dot product does not equal $0$, it follows that these two
vectors are not perpendicular, and thus such a matrix cannot be constructed.

d. Every row is orthogonal to every column ($A$ is not the zero matrix)

_Solution:_

To find such a matrix, this means that every column vector times every row
vector would have to equal $0$, in other words, for such a matrix $A$ to exist,
the following equality must hold:

$$ AA = \mathbf{0} $$

Consider the following $2$ by $2$ matrix:

$$ A =
\left[\begin{array}{rr}
1 & -1 \\
1 & -1 \\
\end{array}\right]
$$

Then:

$$ AA =
\left[\begin{array}{rr}
1 & -1 \\
1 & -1 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & -1 \\
1 & -1 \\
\end{array}\right] =
\left[\begin{array}{rr}
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

This matrix $A$ satisfies the conditions given.

e. Columns add up to a column of zeros, rows add to a row of $1$'s.

_Solution:_

If the columns add up to $\mathbf{0}$, then this is the same as summing all the
columns and getting $0$, so $Ax = 0$ would mean we have $x = (1, 1, \dots, 1)$
since multiplying by $1$ simply yields the sum of all the columns, and since
this solves for $Ax = 0$, this means that $(1, 1, \dots, 1) \in N(A)$.

If all the rows add to a row of $1$'s, this also means that
$(1, 1, \dots, 1) \in C(A^{\mathbf{T}})$. This follows because this means that
$A^{\mathbf{T}}(1, 1, \dots, 1) = (1, 1, \dots, 1)$.

But since $N(A)$ is orthogonal to $C(A^{\mathbf{T}})$, it follows that any
vector in $N(A)$ cannot also be in $C(A^{\mathbf{T}})$ except for $\mathbf{0}$.
Thus this matrix cannot be constructed.

4. If $AB = 0$ then the columns of $B$ are in the ____ of $A$. The rows of $A$
   are in the ____ of $B$. With $AB = 0$, why can't $A$ and $B$ be $3$ by $3$
   matrices of rank $2$?

_Solution:_

_If $AB = 0$ then the columns of $B$ are in the (?) of $A$:_

nullspace

_The rows of $A$ are in the (?) of $B$:_

left nullspace

_With $AB = 0$, why can't $A$ and $B$ be $3$ by $3$ matrices of rank $2$?:_

If rank $= 2$, all those four subspaces have dimension at least 2 which is
impossible for 3 by 3.

Consider if $A$ has rank $2$, this means that it's nullspace, $N(A)$, has
dimension $n - r = 3 - 2 = 1$. Now, since $B$ is in the nullspace of $A$, and
since $B$ has rank $2$, this means that the dimension of $B$ is $2$, but the
dimension of $N(A)$ is $1$. Since $2 \neq 1$, this is a contradiction.

5.

a. If $Ax = b$ has a solution and $A^{\mathbf{T}}y = \mathbf{0}$, _is_
($y^{\mathbf{T}}x = 0$) _or_ ($y^{\mathbf{T}}b = 0$)?

_Solution:_

If $Ax = b$ has a solution, this means that $b \in C(A)$. If
$A^{\mathbf{T}}y = \mathbf{0}$, this means that $y \in N(A^{\mathbf{T}})$.

These two subspaces are orthogonal, and this means that any two vectors in those
two subspaces when multiplied (dot product), they will equal $0$. Those two
vectors are $y^{\mathbf{T}}$ and $b$, so the correct choice is:

$$ y^{\mathbf{T}}b = 0 $$

b. If $A^{\mathbf{T}}y = (1, 1, 1)$ has a solution and $Ax = \mathbf{0}$, then
____.

_Solution:_

If $Ax = \mathbf{0}$, then this means that $x \in N(A)$. If
$A^{\mathbf{T}}y = (1, 1, 1)$, then that means that
$(1, 1, 1) \in C(A^{\mathbf{T}})$.

These two subspaces are orthogonal. This means that their vector(s)' dot
product(s) must equal $0$, in other words:

$$
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]x = 0
$$

6. This system of equations $Ax = b$ has _no solution_ (they lead to $0 = 1$):

$$
x + 2y + 2z = 5 \\
2x + 2y + 3z = 5 \\
3x + 4y + 5z = 9 \\
$$

Find numbers $y_1, y_2, y_3$ to multiply the equations so they add to $0 = 1$.
You have found a vector $y$ in which subspace? Its dot product $y^{\mathbf{T}}b$
is $1$, so no solution $x$.

_Solution:_

_Find numbers $y_1, y_2, y_3$ to multiply the equations so they add to $0 = 1$:_

To find such a vector $y$, it must be shown that:

$$
y^{\mathbf{T}}\left[\begin{array}{cc}
A & b \\
\end{array}\right] =
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{ccc|c}
1 & 2 & 2 & 5 \\
2 & 2 & 3 & 5 \\
3 & 4 & 5 & 9 \\
\end{array}\right]
$$

Is unsolvable because it resolves to $0 = 1$. In other words, we have
$y^{\mathbf{T}}A = 0$, while $y^{\mathbf{T}}b = 1$.

We are thus tasked with finding $y_1, y_2, y_3$ that satisfies these two
equalities (and thus proving that the system is unsolvable).

$$
y^{\mathbf{T}}A =
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 2 & 2 \\
2 & 2 & 3 \\
3 & 4 & 5 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1y_1 + 2y_2 + 3y_3 & 2y_1 + 2y_2 + 4y_3 & 3y_1 + 4y_2 + 5y_3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
\end{array}\right]
$$

We have a few options here, we can simply choose for $y_2, y_3$ and solve for
$y_1$. We could also transpose $A$, row reduce it to upper echelon form, then
choose for $y_2, y_3$ (here, since $A$ is a square matrix, we don't need to
invert it, but that is a bad habit we don't want to form).

Let's go for the first option (solve for the three $y$'s):

$$
y_1 + 2y_2 + 3y_3 = 0 \\
2y_1 + 2y_2 + 4y_3 = 0 \\
3y_1 + 4y_2 + 5y_3 = 0 \\
$$

Let's express this as a matrix (which is just $A$...):

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 2 \\
2 & 2 & 3 \\
3 & 4 & 5 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & -2 & -1 \\
0 & -2 & -1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 2 & 2 \\
0 & -2 & -1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Choose $y_3 = 1$:

$$ -2y_2 + (-1)y_3 = 0 \Rightarrow -2y_2 + (-1)(1) = 0 \Rightarrow -2y_2 = 1 \Rightarrow y_2 = -\frac{1}{2} $$

$$ y_1 + 2y_2 + 2y_3 = 0 \Rightarrow y_1 + 2\left(-\frac{1}{2}\right) + 2(1) = 0 \Rightarrow y_1 - 1 + 2 = 0 \Rightarrow y_1 = -1 $$

So a proper choice for $y^{\mathbf{T}}A = 0$ would be
$y = \left[\begin{array}{rrr}-1 & -\frac{1}{2} & 1 \\\end{array}\right]$.

To verify that this is unsolvable, it must be shown that
$y^{\mathbf{T}}b \neq 0$:

$$ y^{\mathbf{T}}b =
\left[\begin{array}{rrr}
-1 & -\frac{1}{2} & 1 \\
\end{array}\right]
\begin{bmatrix}{}5\\5\\9\end{bmatrix} =
[(-1)(5) + \left(-\frac{1}{2}\right)(5) + (1)(9)] =
[-5 - \frac{5}{2} + 9] =
\left[\frac{3}{2}\right]
$$

Of course, we can take any scalar multiple of any vector that lives within the
left nullspace, so let $c = \dfrac{2}{3}$, and then we get
$y^{\mathbf{T}}b = 1 \neq 0 = y^{\mathbf{T}}A$.

_You have found a vector $y$ in which subspace?:_

left nullspace

7. Every system with no solution is like the one in Problem 6. There are numbers
   $y_1, \dots, y_m$ that multiply the $m$ equations so they add up to $0 = 1$.
   This is called **Fredholm's Alternative**:

**Exactly one of these problems has a solution**

$$ Ax = b \quad \textbf{OR} \quad A^{\mathbf{T}}y = \mathbf{0} \text{ with } y^{\mathbf{T}}b = 1 $$

If $b$ is not in the column space of $A$, it is not orthogonal to the nullspace
of $A^{\mathbf{T}}$. Multiply the equations $x_1 - x_2 = 1$ and $x_2 - x_3 = 1$
and $x_1 - x_3 = 1$ by the numbers $y_1, y_2, y_3$ chosen so that the equations
add up to $0 = 1$.

_Solution:_

For this to be solved, we must find $y$ such that

$$ y^{\mathbf{T}}A =
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & -1 & 0 \\
0 & 1 & -1 \\
1 & 0 & -1 \\
\end{array}\right] = 0
$$

And we must also find $y$ such that:

$$ y^{\mathbf{T}}b =
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = 1
$$

Let's solve the first one:

$$ y^{\mathbf{T}}A =
\left[\begin{array}{ccc}
y_1 & y_2 & y_3 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & -1 & 0 \\
0 & 1 & -1 \\
1 & 0 & -1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
y_1 + y_3 & y_2 - y_1 & -y_2 - y_3 \\
\end{array}\right] =
\left[\begin{array}{ccc}
0 & 0 & 0 \\
\end{array}\right]
$$

This means we get:

$$
y_1 + y_3 = 0 \\
y_2 - y_1 = 0 \\
-y_2 - y_3 = 0 \\
$$

If we row reduced $A^{\mathbf{T}}$, we would see that the third row is all $0$'s
(they are dependent). SO choose $y_3 = 1$, and solve for $y_2, y_1$:

$$ -y_2 - y_3 = 0 \Rightarrow -y_2 - (1) = 0 \Rightarrow -y_2 = 1 \Rightarrow y_2 = -1 $$

$$ y_2 - y_1 = 0 \Rightarrow (-1) - y_1 = 0 \Rightarrow y_1 = -1 $$

So, for $y_{\mathbf{T}} = 0$, a choice for $y$ would be $(-1, -1, 1)$.

Now, let's verify that $y^{\mathbf{T}} = 1$ (as before, we might need a scalar
$c$):

$$ y^{\mathbf{T}}b =
\left[\begin{array}{rrr}
-1 & -1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} =
[(-1)(1) + (-1)(1) + (1)(1)] =
[-1 - 1 + 1] =
[-1]
$$

Now, since $y^{\mathbf{T}} \in N(A^{\mathbf{T}})$, we can multiply this by
$c = -1$, to get $y^{\mathbf{T}}b = 1 \neq 0 = y^{\mathbf{T}}A$.

8. In Figure 4.3, how do we know that $Ax_r$ is equal to $Ax$? How do we know
   that this vector is in the column space? If
   $A = \left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$ and
   $x = \begin{bmatrix}{}1\\0\end{bmatrix}$ what is $x_r$?

_Solution:_

_How do we know that $Ax_r$ is equal to $Ax$?:_

Since $x_r \in C(A^{\mathbf{T}})$ and since $x_n \in N(A)$. And since
$Ax_n = \mathbf{0}$, it follows that
$Ax = Ax_r + Ax_n = Ax_r + \mathbf{0} = Ax_r$.

_How do we know that this vector is in the column space?:_

Here, Strang is not asking if $x_r \in C(A)$, but rather is asking if
$Ax_r \in C(A)$.

Since $Ax = Ax_r$, and since $Ax = b$, it follows that since $b \in C(A)$, then
$Ax_r \in C(A)$.

_If $A = \left[\begin{array}{cc}1 & 1 \\1 & 1 \\\end{array}\right]$ and
$x = \begin{bmatrix}{}1\\0\end{bmatrix}$ what is $x_r$?:_

Recall that $x = x_r + x_n$.

This means that:

$$ -x_r = x_n - x $$

$$ x_r = x - x_n $$

Since $x_n \in N(A)$, we can take some scalar multiple $c$:

$$ x_r = x - cx_n $$

Now, we know that $x = \begin{bmatrix}{}1\\0\end{bmatrix}$, so:

$$ x_r = \begin{bmatrix}{}1\\0\end{bmatrix} - cx_n $$

If we eliminate $A$, we get:

$$ A =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc}
1 & 1 \\
0 & 0 \\
\end{array}\right] = U = R
$$

So the four subspaces for $A$ are:

$$ C(A) = \left\{\begin{bmatrix}{}1\\1\end{bmatrix}\right\} $$

$$ N(A) = \left\{\begin{bmatrix}{}-1\\1\end{bmatrix}\right\} $$

$$ C(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\1\end{bmatrix}\right\} $$

$$ N(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\-1\end{bmatrix}\right\} $$

Since $x_r \in C(A^{\mathbf{T}})$, it follows that
$x_r = \begin{bmatrix}{}1\\1\end{bmatrix}$, but we must choose some $c$ and some
$x_n$ so that the above equality follows.

$$ x_r = \begin{bmatrix}{}1\\0\end{bmatrix} - cx_n $$

Now $x_n \in N(A)$, so $x_n = \begin{bmatrix}{}-1\\1\end{bmatrix}$.

$$ \begin{bmatrix}{}x_{r_1}\\x_{r_2}\end{bmatrix} = \begin{bmatrix}{}1\\0\end{bmatrix} - c\begin{bmatrix}{}-1\\1\end{bmatrix} $$

$$
x_{r_1} = 1 - c(-1) \\
x_{r_2} = 0 - c(1) \\
$$

Now, since $x_r = \begin{bmatrix}{}1\\1\end{bmatrix}$, this means that
$x_{r_1} = x_{r_2}$.

$$
x_{r_1} = 1 - c(-1) \\
x_{r_1} = 0 - c(1) \\
$$

Thus:

$$ 1 - c(-1) = 0 - c(1) $$

$$ 1 + c = -c $$

$$ 1 = -2c $$

$$ -\frac{1}{2} = c $$

Thus:

$$ x_r = x - cx_n $$

$$ x_r = \begin{bmatrix}{}1\\0\end{bmatrix} - \left(-\frac{1}{2}\right)\begin{bmatrix}{}-1\\1\end{bmatrix}$$

$$ x_r = \begin{bmatrix}{}1\\0\end{bmatrix} - \begin{bmatrix}{}\frac{1}{2}\\-\frac{1}{2}\end{bmatrix} $$

$$ \boxed{x_r = \begin{bmatrix}{}\frac{1}{2}\\\frac{1}{2}\end{bmatrix}} $$

9. If $A^{\mathbf{T}}Ax = \mathbf{0}$ then $Ax = \mathbf{0}$. Reason: $Ax$ is
   the nullspace of $A^{\mathbf{T}}$ and also in the ____ of $A$ and those
   spaces are ____. _Conclusion:_ $A^{\mathbf{T}}A$ _has the same nullspace as
   $A$. This key fact is repeated in the next section._

_Solution:_

_$Ax$ is the nullspace of $A^{\mathbf{T}}$ and also in the (?) of $A$:_

column space

_and those spaces are (?):_

perpendicular

10. Suppose $A$ is a symmetric matrix ($A^{\mathbf{T}} = A$).

a. Why is its column space perpendicular to its nullspace?

Normally the column space of $A$ is perpendicular to the nullspace of
$A^{\mathbf{T}}$. However, since $A^{\mathbf{T}} = A$, it follows that the
column space of $A$ is perpendicular to the nullspace of $A$.

b. If $Ax = \mathbf{0}$ and $Az = 5z$, which subspaces contain these
"eigenvectors" $x$ and $z$? **Symmetric matrices have perpendicular eigenvectors
$x^{\mathbf{T}}z = 0$.**

So, since $Ax = \mathbf{0}$, this means that $x \in N(A)$. Similarly, since
$Az = 5z$, this means that $5z \in C(A)$, but since $5$ is just a scalar value,
this further implies that $z \in C(A)$.

By the supposition, $A = A^{\mathbf{T}}$, so $x \in N(A)$ and
$x \in N(A^{\mathbf{T}})$, and $z \in C(A)$ and $z \in C(A^{\mathbf{T}})$.

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

_Solution:_

We'll draw these by hand later (kind of a pointless exercise since once you find
the four subspaces, it's rather trivial to draw them so as to see visually their
orthogonality, but whatever).

_For $A$:_

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
3 & 6 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
3 & 6 \\
\end{array}\right] \to
\left[\begin{array}{cc}
1 & 2 \\
0 & 0 \\
\end{array}\right]
$$

$$ C(A) = \left\{\begin{bmatrix}{}1\\3\end{bmatrix}\right\} $$

$$ N(A) = \left\{\begin{bmatrix}{}-2\\1\end{bmatrix}\right\}  $$

$$ C(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\2\end{bmatrix}\right\} $$

$$ N(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}-3\\1\end{bmatrix}\right\} $$

_For $B$:_

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cc}
1 & 0 \\
3 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ C(B) = \left\{\begin{bmatrix}{}1\\3\end{bmatrix}\right\} $$

$$ N(B) = \left\{\begin{bmatrix}{}0\\1\end{bmatrix}\right\} $$

$$ C(B^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\0\end{bmatrix}\right\} $$

$$ N(B^{\mathbf{T}}) = \left\{\begin{bmatrix}{}-3\\1\end{bmatrix}\right\} $$

(Drawings done by hand.)

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

_Solution:_

Recall $x = x_r + x_n$. Since $x_n \in N(A)$, then $x = x_r + cx_n$ for some
scalar multiple $c$. We'll need to find $N(A)$ to help determine $x_n$.

Similarly, since $x_r \in C(A^{\mathbf{T}})$, we'll need to find
$C(A^{\mathbf{T}})$ to help determine $x_r$:

$$ A =
\left[\begin{array}{rr}
1 & -1 \\
0 & 0 \\
0 & 0 \\
\end{array}\right]
$$

Already eliminated, so:

$$ C(A^{\mathbf{T}}) = \left\{\begin{bmatrix}{}1\\-1\end{bmatrix}\right\} $$

$$ N(A) = \left\{\begin{bmatrix}{}1\\1\end{bmatrix}\right\} $$

Thus since $x_r \in C(A^{\mathbf{T}})$, it follows that
$x_r = \begin{bmatrix}{}1\\-1\end{bmatrix}$. Similarly, since $x_n \in N(A)$, it
follows that $x_n = \begin{bmatrix}{}1\\1\end{bmatrix}$. So, let's check against
$x$:

$$ x = x_r + x_n $$

$$ \begin{bmatrix}{}2\\0\end{bmatrix} = \begin{bmatrix}{}1\\-1\end{bmatrix} + \begin{bmatrix}{}1\\1\end{bmatrix} $$

This equality holds, and thus we have found $x_r, x_n$.

**Questions 13-23 are about orthogonal subspaces.**

13. Put bases for the subspaces $V$ and $W$ into the columns of matrices $V$ an
    $W$. Explain why the test for orthogonal subspaces an be written
    $V^{\mathbf{T}}W =$ zero matrix. This matches $v^{\mathbf{T}}w = 0$ for
    orthogonal vectors.

_Solution:_

Since $V^{\mathbf{T}}W = \mathbf{0}$, it follows that $W \in N(V^{\mathbf{T}})$,
which is orthogonal to $C(V)$. This means that every basis vector in $V$ is
orthogonal to every basis vector in $W$.

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

_Solution:_

Let's consider what it means for some vector to be in both $C(A)$ and $C(B)$.

This means that $Ax = v$ and $B\hat{x} = v$, where
$v \in C(A) \wedge v \in C(B)$.

But, observe that:

$$ Ax = v = B\hat{x} $$

$$ Ax = B\hat{x} $$

Now, since this equality must hold, it follows that:

$$ Ax - B\hat{x} = \mathbf{0} $$

So:

$$
\left[\begin{array}{cc}
1 & 2 \\
1 & 3 \\
1 & 2 \\
\end{array}\right]
\vec{x} -
\left[\begin{array}{cc}
5 & 4 \\
6 & 3 \\
5 & 1 \\
\end{array}\right]
\vec{\hat{x}} = \mathbf{0}
$$

Now, by the laws of matrix multiplcation both $\vec{x}$ and $\vec{\hat{x}}$ must
have $2$ components since both $A$ and $B$ have $2$ columns.

$$
\left[\begin{array}{cc}
1 & 2 \\
1 & 3 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} -
\left[\begin{array}{cc}
5 & 4 \\
6 & 3 \\
5 & 1 \\
\end{array}\right]
\begin{bmatrix}{}\hat{x}_1\\\hat{x}_2\end{bmatrix} = \mathbf{0}
$$

Evaluating this will hopefully yield values for
$x_1, x_2, \hat{x}_1, \hat{x}_2$:

$$ =
\left[\begin{array}{c}
x_1 + 2x_2 \\
x_1 + 3x_2 \\
x_1 + 2x_2 \\
\end{array}\right] -
\left[\begin{array}{c}
5\hat{x}_1 + 4\hat{x}_2 \\
6\hat{x}_1 + 3\hat{x}_2 \\
5\hat{x}_1 + 1\hat{x}_2 \\
\end{array}\right] = \mathbf{0}
$$

So we get:

$$
x_1 + 2x_2 - (5\hat{x}_1 + 4\hat{x}_2) = 0 \\
x_1 + 3x_2 - (6\hat{x}_1 + 3\hat{x}_2) = 0 \\
x_1 + 2x_2 - (5\hat{x}_1 + 1\hat{x}_2) = 0 \\
$$

We'll need to eliminate in order to find our free variable(s):

$$
\left[\begin{array}{rrrr}
1 & 2 & -5 & -4 \\
1 & 3 & -6 & -3 \\
1 & 2 & -5 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & -5 & -4 \\
0 & 1 & -1 & 1 \\
1 & 2 & -5 & -1 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & -5 & -4 \\
0 & 1 & -1 & 1 \\
0 & 0 & 0 & 3 \\
\end{array}\right]
$$

So we have a free variable, namely that of $\hat{x}_1$.

Let $\hat{x}_1 = 1$, then:

$$ 3\hat{x}_2 = 0 \Rightarrow \hat{x}_2 = 0 $$

$$ x_2 - \hat{x}_1 + \hat{x}_2 = 0 \Rightarrow x_2 - 1 + 0 = 0 \Rightarrow x_2 = 1 $$

$$ x_1 + 2x_2 - 5\hat{x}_1 - 4\hat{x}_2 = 0 \Rightarrow x_1 + 2(1) - 5(1) - 4(0) = 0 \Rightarrow x_1 + 2 - 5= 0 \Rightarrow x_1 = 3 $$

$$ x = \begin{bmatrix}{}3\\1\end{bmatrix}, \hat{x} = \begin{bmatrix}{}1\\0\end{bmatrix} $$

Now, we have two vectors $x$ and $\hat{x}$ that we can use to check to see if
$Ax = B\hat{x}$:

$$ Ax =
\left[\begin{array}{cc}
1 & 2 \\
1 & 3 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}3\\1\end{bmatrix} =
\left[\begin{array}{c}
1(3) + 2(1) \\
1(3) + 3(1) \\
1(3) + 2(1) \\
\end{array}\right] =
\left[\begin{array}{c}
5 \\
6 \\
5 \\
\end{array}\right]
$$

$$ B\hat{x} =
\left[\begin{array}{cc}
5 & 4 \\
6 & 3 \\
5 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\end{bmatrix} =
\left[\begin{array}{c}
5(1) + 4(0) \\
6(1) + 3(0) \\
5(1) + 1(0) \\
\end{array}\right] =
\left[\begin{array}{c}
5 \\
6 \\
5 \\
\end{array}\right] = Ax
$$

Thus the vector in the column space of both matrices is:

$$ \boxed{v = \begin{bmatrix}{}5\\6\\5\end{bmatrix}} $$

15. Extend Problem 14 to a $p$-dimensional subspace $V$ and a $q$-dimensional
    subspace $W$ of $\R^n$. What inequality on $p + q$ guarantees that $V$
    intersects $W$ in a nonzero vector? These subspaces cannot be orthogonal.

_Solution:_

The sum of two vectors $p$ and $q$, $p + q$ share at least a line in $\R^n$ if
$p + q > n$. This makes sense if you think on it for a bit. If the dimension of
$V$ is $p$, and if $V$ is a subspace of $\R^n$, it follows that there remains
$n - p$ dimensions for all other non-intersecting subspaces of $\R^n$.

Similarly, if $W$ has $q$ dimensions, and $W$ is a subspace of $\R^n$, then
there remains $n - q$ dimensions for all other non-intersecting subspaces of
$R^n$.

If $p$ and $q$ do not intersect, then when added together, their sum can only be
less than or equal to $n$. Or, more succinctly, $p + q \leq n$.

It follows that if $p$ and $q$ do intersect, then they share at least a line in
$\R^n$ if $p + q > n$. In other words, $p + q$ share a nonzero vector (that is
the aforementioned line).

These subspaces cannot be orthogonal. Think on this, $V$ and $W$ cannot be
orthogonal because if $V$ and $W$ were orthogonal, they would not share any
nonzero vector, but it has just been shown that they do.

16. Prove that every $y$ in $N(A^{\mathbf{T}})$ is perpendicular to every $Ax$
    in the column space, using the matrix shorthand of equation (2). Start from
    $A^{\mathbf{T}}y = \mathbf{0}$.

_Solution:_

For reference equation (2) states:

**Nullspace orthogonal row space**

$$ x^{\mathbf{T}}(A^{\mathbf{T}}y) = (Ax)^{\mathbf{T}}y = \mathbf{0}^{\mathbf{T}}y = 0 $$

**Proof:**

Suppose $y \in N(A^{\mathbf{T}})$ for any matrix $A$.

It is to be shown that $y$ is perpendicular to every $Ax$ in the column space,
$C(A)$.

It follows from the supposition that $A^{\mathbf{T}}y = \mathbf{0}$.

From example (2), we have $(Ax)^{\mathbf{T}}y$, if we take the transpose and
"distribute" it across $Ax$, we get:

$$ x^{\mathbf{T}}A^{\mathbf{T}}y $$

Now, by substitution, we get:

$$ x^{\mathbf{T}}\mathbf{0} = 0 $$

By the definition of perpendicular, this demonstrates that $y$ is perpendicular
to every $Ax \in C(A)$.

This is what was to be shown.

Q.E.D.

17. If $S$ is the subspace of $\R^3$ containing only the zero vector, what is
    $S^{\perp}$? If $S$ is spanned by $(1, 1, 1)$, what is $S^{\perp}$? If $S$
    is spanned by $(1, 1, 1)$ and $(1, 1, -1)$, what is a basis for $S^{\perp}$?

_Solution:_

_If $S$ is the subspace of $\R^3$ containing only the zero vector, what is
$S^{\perp}$?:_

Every vector in $\R^3$.

_If $S$ is spanned by $(1, 1, 1)$, what is $S^{\perp}$?:_

By the definition of perpendicular this means that the dot product of $(1,1,1)$
and $S^{\perp}$ must be $0$.

$$
\left[\begin{array}{ccc}
s_1 & s_2 & s_3 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = 0
$$

This means that $s_1 + s_2 + s_3 = 0$. Thus $S^{\perp}$ is any row vector with
$3$ components that sum to $0$. (this is a plane through $(0, 0, 0)$ in $\R^3$)

_If $S$ is spanned by $(1, 1, 1)$ and $(1, 1, -1)$, what is a basis for
$S^{\perp}$?:_

By the definition of perpendicular, this means that the dot product of
$(1, 1, 1)$ and $S^{\perp}$ must be $0$, and also that the dot product of
$(1, 1, -1)$ and $S^{\perp}$ is also $0$.

From the previous part, we know that for $(1, 1, 1)$ and $S^{\perp}$ to be
perpendicular, the three components of $S^{\perp}$, $s_1, s_2, s_3$, must sum to
$0$ ($s_1 + s_2 + s_3 = 0$).

Now, for the next part:

$$
\left[\begin{array}{ccc}
s_1 & s_2 & s_3\\
\end{array}\right]
\begin{bmatrix}{}1\\1\\-1\end{bmatrix} = 0
$$

Thus $s_1 + s_2 - s_3 = 0$ must also hold.

Notice that this means that $s_1 + s_2 = s_3$. So, by substitution into our
first equation, we get:

$$ s_1 + s_2 + s_3 = 0 \Rightarrow s_1 + s_2 + (s_1 + s_2) = 0 \Rightarrow 2s_1 + 2s_2 = 0 \Rightarrow 2s_1 = -2s_2 \Rightarrow s_1 = -s_2 $$

Thus $S^{\perp}$ takes the form of
$\begin{bmatrix}{}s_1\\-s_1\\s_1 + (-s_1)\end{bmatrix}$. We can infer the basis
for $S^{\perp}$ is $\begin{bmatrix}{}1\\-1\\0\end{bmatrix}$.

18. Suppose $S$ only contains two vectors $(1, 5, 1)$ and $(2, 2, 2)$ (not a
    subspace). Then $S^{\perp}$ is the nullspace of a matrix $A =$ ____.
    $S^{\perp}$ is a subspace even if $S$ is not.

_Solution:_

_Then $S^{\perp}$ is the nullspace of a matrix $A =$ (?):_

Since:

$$ S = \left\{\begin{bmatrix}{}1\\5\\1\end{bmatrix}, \begin{bmatrix}{}2\\2\\2\end{bmatrix}\right\} $$

Thus, to find $S^{\perp}$, we must find a basis vector where the dot product
with each of these vectors equals $0$.

$$
\left[\begin{array}{ccc}
s_1 & s_2 & s_3 \\
\end{array}\right]
\begin{bmatrix}{}1\\5\\1\end{bmatrix} = 0
$$

So:

$$ s_1 + 5s_2 + s_3 = 0 $$

must hold.

Similarly:

$$
\left[\begin{array}{ccc}
s_1 & s_2 & s_3 \\
\end{array}\right]
\begin{bmatrix}{}2\\2\\2\end{bmatrix} = 0
$$

$$ 2s_1 + 2s_2 + 2s_3 = 0 $$

must also hold.

Put together this is:

$$
s_1 + 5s_2 + s_3 = 0
2s_1 + 2s_2 + 2s_3 = 0
$$

We can align these in a matrix as follows:

$$
\left[\begin{array}{ccc}
1 & 5 & 1 \\
2 & 2 & 2 \\
\end{array}\right]
$$

$$
\left[\begin{array}{ccc}
1 & 5 & 1 \\
2 & 2 & 2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 5 & 1 \\
0 & -8 & 0 \\
\end{array}\right]
$$

Choose $s_3 = 1$:

$$ -8s_2 + 0s_3 = 0 \Rightarrow -8s_2 = 0 \Rightarrow s_2 = 0 $$

$$ s_1 + 5s_2 + s_3 = 0 \Rightarrow s_1 + 5(0) + 1 = 0 \Rightarrow s_1 + 1 = 0 \Rightarrow s_1 = -1 $$

So $S^{\perp} = \begin{bmatrix}{}-1\\0\\1\end{bmatrix}$, and this is the
nullspace of $A$ when:

$$ A =
\left[\begin{array}{ccc}
1 & 5 & 1 \\
2 & 2 & 2 \\
\end{array}\right]
$$

19. Suppose $L$ is a one-dimensional subspace (a line) in $\R^3$. Its orthogonal
    complement $L^{\perp}$ is the ____ perpendicular to $L$. Then
    $(L^{\perp})^{\perp}$ is a ____ perpendicular to $L^{\perp}$. In fact
    $(L^{\perp})^{\perp}$ is the same as ____.

_Solution:_

_Its orthogonal complement $L^{\perp}$ is the (?) perpendicular to $L$:_

2 dimensional subspace of $\R^3$, which is a _plane_.

_Then $(L^{\perp})^{\perp}$ is a (?) perpendicular to $L^{\perp}$:_

1 dimensional subspace of $\R^3$, which is a _line_.

_In fact $(L^{\perp})^{\perp}$ is the same as (?):_

$L$

20. Suppose $V$ is the whole space $\R^4$. Then $V^{\perp}$ contains only the
    vector ____. Then $(V^{\perp})^{\perp}$ is ____. So $(V^{\perp})^{\perp}$ is
    the same as ____.

_Solution:_

_Then $V^{\perp}$ contains only the vector (?):_

$\mathbf{0}$

_Then $(V^{\perp})^{\perp}$ is (?):_

$\R^4$

_So $(V^{\perp})^{\perp}$ is the same as (?):_

$V$

21. Suppose $S$ is spanned by the vectors $(1, 2, 2, 3)$ and $(1, 3, 3, 2)$.
    Find two vectors that span $S^{\perp}$. This is the same as solving
    $Ax = \mathbf{0}$ for which $A$?

_Solution:_

_Find two vectors that span $S^{\perp}$:_

From problem 18, we know that we can find a basis for $S^{\perp}$ by simply
defining a matrix $A$ as having rows of the given vectors in $S$, so:

$$ A =
\left[\begin{array}{cccc}
1 & 2 & 2 & 3 \\
1 & 3 & 3 & 2 \\
\end{array}\right]
$$

Now, row reduce and solve for $S^{\perp}$:

$$ A =
\left[\begin{array}{cccc}
1 & 2 & 2 & 3 \\
1 & 3 & 3 & 2 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & 2 & 3 \\
0 & 1 & 1 & -1 \\
\end{array}\right]
$$

We have two free variables, which is fortunate, this gives us the two vectors in
$S^{\perp}$.

Choose $s_3 = 1, s_4 = 0$:

$$ s_2 + s_3 - s_4 = 0 \Rightarrow s_2 + 1 - 0 = 0 \Rightarrow s_2 = -1 $$

$$ s_1 + 2s_2 + 2s_3 + 3s_4 = 0 \Rightarrow s_1 + 2(-1) + 2(1) + 3(0) = 0 \Rightarrow s_1 - 2 + 2 = 0 \Rightarrow s_1 = 0 $$

Choose $s_3 = 0, s_4 = 1$:

$$ s_2 + s_3 - s_4 = 0 \Rightarrow s_2 + 0 - 1 = 0 \Rightarrow s_2 = 1 $$

$$ s_1 + 2s_2 + 2s_3 + 3s_4 = 0 \Rightarrow s_1 + 2(1) + 2(0) + 3(1) = 0 \Rightarrow s_1 + 2 + 3 = 0 \Rightarrow s_1 = -5 $$

So:

$$ S^{\perp} = \left\{\begin{bmatrix}{}0\\-1\\1\\0\end{bmatrix}, \begin{bmatrix}{}-5\\1\\0\\1\end{bmatrix}\right\} $$

_This is the same as solving $Ax = \mathbf{0}$ for which $A$?:_

This was established earlier as:

$$ A =
\left[\begin{array}{cccc}
1 & 2 & 2 & 3 \\
1 & 3 & 3 & 2 \\
\end{array}\right]
$$

22. If $P$ is the plane of vectors in $\R^4$ satisfying
    $x_1 + x_2 + x_3 + x_4 = 0$, write a basis for $P^{\perp}$. Construct a
    matrix that has $P$ as its nullspace.

_Solution:_

The basis for $P^{\perp}$ is $\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix}$ since:

$$
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\\x_4\end{bmatrix} = x_1 + x_2 + x_3 + x_4 = 0
$$

A matrix $A$ with $N(A) = P$ is:

$$ A =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
\end{array}\right]
$$

23. If a subspace $S$ is contained in a subspace $V$, prove that $S^{\perp}$
    contains $V^{\perp}$.

_Solution:_

**Proof:**

Suppose $S$ is a subspace contained in a subspace $V$.

It is to be shown that $S^{\perp}$ contains $V^{\perp}$.

Let $x \in V^{\perp}$.

Then $x$ is perpendicular to every vector in $V$.

Since $V$ contains $S$, it follows that $x$ is perpendicular to every vector in
$S$.

So every $x$ in $V^{\perp}$ is also in $S^{\perp}$, and it can be concluded that
$S^{\perp}$ contains $V^{\perp}$. This is what was to be shown.

Q.E.D.

**Questions 24-30 are about perpendicular columns and rows.**

24. Suppose an $n$ by $n$ matrix is invertible: $AA^{-1} = I$. Then the first
    column of $A^{-1}$ is orthogonal to the space spanned by which rows of $A$?

_Solution:_

The first column of $A^{-1}$ is orthogonal to all rows of $A$ except for the
first row.

25. Find $A^{\mathbf{T}}A$ if the columns of $A$ are unit vectors, all mutually
    perpendicular.

_Solution:_

If the columns of $A$ are unit vectors, then $A^{\mathbf{T}}A = I$. Note that we
write $Q$ for such a matrix.

26. Construct a $3$ by $3$ matrix $A$ with no zero entries whose columns are
    mutually perpendicular. Compute $A^{\mathbf{T}}A$. Why is it a diagonal
    matrix?

Omitted.

27. The lines $3x + y = b_1$ and $6x + 2y = b_2$ are ____. They are the same
    line if ____. In that case $(b_1, b_2)$ is perpendicular to the vector ____.
    The nullspace of the matrix is the line $3x + y =$ ____. One particular
    vector in that nullspace is ____.

_Solution:_

_The lines $3x + y = b_1$ and $6x + 2y = b_2$ are (?):_

parallel (since they are scalar multiples on the left hand sides)

_They are the same line if (?):_

$b_2 = 2b_1$

_In that case $(b_1, b_2)$ is perpendicular to the vector (?):_

$(-2, 1)$

_The nullspace of the matrix is the line $3x + y =$ (?):_

$$ \mathbf{0} $$

_One particular vector in that nullspace is (?):_

$(-1, 3)$

28. Why is each of these statements false?

a. $(1, 1, 1)$ is perpendicular to $(1, 1, -2)$ so the planes $x + y + z = 0$
and $x + y - 2z = 0$ are orthogonal subspaces.

_Solution:_

$$
x + y + z = 0 \\
x + y - 2z = 0 \\
$$

Choose $y = 1, z = 0$:

$$
x + 1 + 0 = 0 \to x = -1 \\
x + 1 - 2(0) = 0 \to x = -1 \\
$$

$s_1 = (-1, 1, 0)$

Choose $y = 0, z = 1$:

$$
x + 0 + 1 = 0 \to x = -1 \\
x + 0 - 2(1) = 0 \to x = 2 \\
$$

$s_2 = (-1, 0, 1)$

These two vectors are in both planes. Normal vectors are perpendicular, but
planes still intersect. Two planes in $\R^3$ can't be orthogonal.

b. The subspace spanned by $(1, 1, 0, 0, 0)$ and $(0, 0, 0, 1, 1)$ is the
orthogonal complement of the subspace spanned by $(1, -1, 0, 0, 0)$ and
$(2, -2, 3, 4, -4)$.

_Solution:_

You need three orthogonal vectors to span the whole orthogonal complement in
$\R^5$.

c. Two subspaces that meet only in the zero vector are orthogonal.

_Solution:_

Lines meeting in $\R^3$ at the zero vector can not be orthogonal.

29. Find a matrix with $v = (1, 2, 3)$ in the row space and the column space.
    Find another matrix with $v$ in the nullspace and column space. Which pairs
    of subspaces can $v$ _not_ be in?

Omitted.

---

Page 225

## Problem Set 4.2

**Questions 1-9 ask for projections $p$ onto lines. Also errors $e = b - p$ and
matrices $P$.**

1. Project the vector $b$ onto the line through $a$. Check that $e$ is
   perpendicular to $a$:

a. $b = \begin{bmatrix}{}1\\2\\2\end{bmatrix}$ and
$a = \begin{bmatrix}{}1\\1\\1\end{bmatrix}$

_Solution:_

When Strang says "project the _vector_ onto the _line_", he means find $p$,
which in turns means finding $\hat{x}$.

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ \hat{x} = \frac{5}{3} $$

$$ p = \hat{x}a = \frac{5}{3}a = \begin{bmatrix}{}\frac{5}{3}\\\frac{5}{3}\\\frac{5}{3}\end{bmatrix} $$

Check that $e \perp a$:

$$ e = b - p $$

$$ e = \begin{bmatrix}{}1\\2\\2\end{bmatrix} - \begin{bmatrix}{}\frac{5}{3}\\\frac{5}{3}\\\frac{5}{3}\end{bmatrix} $$

$$ e = \begin{bmatrix}{}-\frac{2}{3}\\\frac{1}{3}\\\frac{1}{3}\end{bmatrix} $$

so $e^{\mathbf{T}} \cdot a = 0$ if $e \perp a$:

$$ e^{\mathbf{T}} \cdot a =
\left[\begin{array}{ccc}
-\frac{2}{3} & \frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
\cdot \begin{bmatrix}{}1\\1\\1\end{bmatrix} =
\left(-\frac{2}{3}\right)(1) + \left(\frac{1}{3}\right)(1) + \left(\frac{1}{3}\right)(1) = 0
$$

So indeed $e \perp a$.

b. $b = \begin{bmatrix}{}1\\3\\1\end{bmatrix}$ and
$a = \begin{bmatrix}{}-1\\-3\\-1\end{bmatrix}$

_Solution:_

Again, Strang wants us to find $p$, which means first finding $\hat{x}$

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ \hat{x} = \frac{-11}{11} = -1 $$

$$ p = \hat{x}a $$

$$ p = (-1)\begin{bmatrix}{}-1\\-3\\-1\end{bmatrix} $$

$$ p = \begin{bmatrix}{}1\\3\\1\end{bmatrix} $$

Check that $e \perp a$:

$$ e = b - p $$

$$ e = \begin{bmatrix}{}1\\3\\1\end{bmatrix} - \begin{bmatrix}{}1\\3\\1\end{bmatrix} = \begin{bmatrix}{}0\\0\\0\end{bmatrix} $$

Note that since $e = 0$, this means that $Ax = b$ is solvable!

$$ e^{\mathbf{T}} \cdot a = 0 \Leftrightarrow e \perp a $$

Since $\mathbf{0}$ is perpendicular to any vector, $e \perp a$.

2. _Draw_ the projection of $b$ onto $a$ and also compute it from
   $p = \hat{x}a$:

a. $b = \begin{bmatrix}{}\cos\theta\\\sin\theta\end{bmatrix}$ and
$a = \begin{bmatrix}{}1\\0\end{bmatrix}$

_Solution:_

This isn't all that different from Problem 1, find $p$, which means find
$\hat{x}$.

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ \hat{x} = \frac{\cos\theta}{1} $$

$$ \hat{x} = \cos\theta $$

$$ p = \hat{x}a $$

$$ p = \cos\theta \cdot \begin{bmatrix}{}1\\0\end{bmatrix} $$

$$ p = \begin{bmatrix}{}\cos\theta\\0\end{bmatrix} $$

b. $b = \begin{bmatrix}{}1\\1\end{bmatrix}$ and
$a = \begin{bmatrix}{}1\\-1\end{bmatrix}$

_Solution:_

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ \hat{x} = \frac{0}{2} = 0 $$

$$ p = \hat{x}a $$

$$ p = 0 \cdot \begin{bmatrix}{}1\\-1\end{bmatrix} $$

$$ p = \begin{bmatrix}{}0\\0\end{bmatrix} $$

3. In Problem 1, find the projection matrix
   $P = aa^{\mathbf{T}}/a^{\mathbf{T}}a$ onto the line through each vector $a$.
   Verify in both cases that $P^2 = P$. Multiply $Pb$ in each case to compute
   the projection $p$.

a.

_Solution:_

$$ b = \begin{bmatrix}{}1\\2\\2\end{bmatrix}, a = \begin{bmatrix}{}1\\1\\1\end{bmatrix} $$

Here we are tasked with finding the projection matrix $P$ onto the line through
$a$.

Now, recall that the formula for finding the Projection matrix $P$ is:

$$ P = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

Thus, for this case, $P$ is:

$$ aa^{\mathbf{T}} =
\begin{bmatrix}{}1\\1\\1\end{bmatrix}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

$$ P =
\frac{1}{3}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

Now, we must verify that $P^2 = P$

$$ P^2 = P \cdot P
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\end{array}\right] =
\left[\begin{array}{ccc}
\frac{3}{9} & \frac{3}{9} & \frac{3}{9} \\
\frac{3}{9} & \frac{3}{9} & \frac{3}{9} \\
\frac{3}{9} & \frac{3}{9} & \frac{3}{9} \\
\end{array}\right] =
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\end{array}\right] = P
$$

Now we must compute $Pb = p$:

$$ Pb =
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\frac{1}{3} & \frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\2\end{bmatrix} =
\begin{bmatrix}{}\frac{5}{3}\\\frac{5}{3}\\\frac{5}{3}\end{bmatrix} =
\frac{1}{3}\begin{bmatrix}{}5\\5\\5\end{bmatrix} = p
$$

Note that this $p$ matches our solution in Problem 1a.

b.

_Solution:_

$$ b = \begin{bmatrix}{}1\\3\\1\end{bmatrix}, a = \begin{bmatrix}{}-1\\-3\\-1\end{bmatrix} $$

$$ P = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

$$ aa^{\mathbf{T}} =
\begin{bmatrix}{}-1\\-3\\-1\end{bmatrix}
\left[\begin{array}{rrr}
-1 & -3 & -1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 3 & 1 \\
3 & 9 & 3 \\
1 & 3 & 1 \\
\end{array}\right]
$$

$$ P =
\frac{1}{11}
\left[\begin{array}{ccc}
1 & 3 & 1 \\
3 & 9 & 3 \\
1 & 3 & 1 \\
\end{array}\right]
$$

Verify that $P^2 = P$

$$ P^2 = P \cdot P =
\left[\begin{array}{ccc}
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\frac{3}{11} & \frac{9}{11} & \frac{3}{11} \\
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\end{array}\right]
\left[\begin{array}{ccc}
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\frac{3}{11} & \frac{9}{11} & \frac{3}{11} \\
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\end{array}\right] =
\left[\begin{array}{ccc}
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\frac{3}{11} & \frac{9}{11} & \frac{3}{11} \\
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\end{array}\right] = P
$$

Show that $Pb = p$:

$$ Pb =
\left[\begin{array}{ccc}
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\frac{3}{11} & \frac{9}{11} & \frac{3}{11} \\
\frac{1}{11} & \frac{3}{11} & \frac{1}{11} \\
\end{array}\right]
\begin{bmatrix}{}1\\3\\1\end{bmatrix} =
\begin{bmatrix}{}1\\3\\1\end{bmatrix} = p
$$

And again, this matches $p$ in Problem 1b.

4. Construct the projection matrices $P_1$ and $P_2$ onto the lines through the
   $a$'s in Problem 2. Is it true that $(P_1 + P_2)^2 = P_1 + P_2$? This _would_
   be true if $P_1P_2 = 0$.

_Solution:_

a. $a = \begin{bmatrix}{}1\\0\end{bmatrix}$

$$ P_1 = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

$$ P_1 = \frac{aa^{\mathbf{T}}}{1} $$

$$ P_1 = aa^{\mathbf{T}} =
\begin{bmatrix}{}1\\0\end{bmatrix}
\left[\begin{array}{cc}
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

b. $a = \begin{bmatrix}{}1\\-1\end{bmatrix}$

$$ P_2 = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

$$ P_2 = \frac{1}{2}aa^{\mathbf{T}} =
\frac{1}{2}
\begin{bmatrix}{}1\\-1\end{bmatrix}
\left[\begin{array}{cc}
1 & -1 \\
\end{array}\right] =
\frac{1}{2}
\left[\begin{array}{rr}
1 & -1 \\
-1 & 1 \\
\end{array}\right]
$$

_Is it true that $(P_1 + P_2)^2 = P_1 + P_2$? This _would_ be true if
$P_1P_2 = 0$:_

$$ P_1 + P_2 =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right] +
\left[\begin{array}{rr}
\frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right] =
\left[\begin{array}{rr}
\frac{3}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right]
$$

$$ (P_1 + P_2)^2 =
\left[\begin{array}{rr}
\frac{3}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right]
\left[\begin{array}{rr}
\frac{3}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right] =
\left[\begin{array}{cc}
\frac{5}{2} & -1 \\
-1 & \frac{1}{2} \\
\end{array}\right] \neq (P_1 + P_2)
$$

5. Compute the projection matrices $aa^{\mathbf{T}}/a^{\mathbf{T}}a$ onto the
   lines through $a_1 = (-1, 2, 2)$ and $a_2 = (2, 2, -1)$. Multiply those
   projection matrices and explain why their product $P_1P_2$ is what it is.

_Solution:_

$$ a_1 = \begin{bmatrix}{}-1\\2\\2\end{bmatrix}, a_2 = \begin{bmatrix}{}2\\2\\-1\end{bmatrix} $$

$$ P_1 = \frac{a_1(a_1)^{\mathbf{T}}}{(a_1)^{\mathbf{T}}a_1} $$

$$ P_1 = \frac{1}{9}a_1(a_1)^{\mathbf{T}} $$

$$ a_1(a_1)^{\mathbf{T}} =
\begin{bmatrix}{}-1\\2\\2\end{bmatrix}
\left[\begin{array}{rrr}
-1 & 2 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & -2 & -2 \\
-2 & 4 & 4 \\
-2 & 4 & 4 \\
\end{array}\right]
$$

$$ P_1 =
\frac{1}{9}
\left[\begin{array}{rrr}
1 & -2 & -2 \\
-2 & 4 & 4 \\
-2 & 4 & 4 \\
\end{array}\right]
$$

$$ P_2 = \frac{a_2(a_2)^{\mathbf{T}}}{(a_2)^{\mathbf{T}}a_2} $$

$$ P_2 = \frac{1}{9}a_2(a_2)^{\mathbf{T}} $$

$$ a_2(a_2)^{\mathbf{T}} =
\begin{bmatrix}{}2\\2\\-1\end{bmatrix}
\left[\begin{array}{rrr}
2 & 2 & -1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
4 & 4 & -2 \\
4 & 4 & -2 \\
-2 & -2 & 1 \\
\end{array}\right]
$$

$$ P_2 =
\frac{1}{9}
\left[\begin{array}{rrr}
4 & 4 & -2 \\
4 & 4 & -2 \\
-2 & -2 & 1 \\
\end{array}\right]
$$

_Multiply those projection matrices and explain why their product $P_1P_2$ is
what it is:_

$$ P_1P_2 =
\left(
\frac{1}{9}
\left[\begin{array}{rrr}
1 & -2 & -2 \\
-2 & 4 & 4 \\
-2 & 4 & 4 \\
\end{array}\right]
\right) \cdot
\left(
\frac{1}{9}
\left[\begin{array}{rrr}
4 & 4 & -2 \\
4 & 4 & -2 \\
-2 & -2 & 1 \\
\end{array}\right]
\right)
$$

$$ P_1P_2 =
\frac{1}{81}
\left[\begin{array}{ccc}
0 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{array}\right] = \mathbf{0}
$$

Since $P_1P_2 = \mathbf{0}$, this means that $a_1 \perp a_2$.

6. Project $b = (1, 0, 0)$ onto the lines through $a_1$ and $a_2$ in Problem 5
   and also onto $a_3 = (2, -1, 2)$. Add up the three projections
   $p_1 + p_2 + p_3$.

_Solution:_

$$ p_1 = P_1b $$

$$ P_1b =
\frac{1}{9}
\left[\begin{array}{rrr}
1 & -2 & -2 \\
-2 & 4 & 4 \\
-2 & 4 & 4 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\frac{1}{9}
\begin{bmatrix}{}1\\-2\\-2\end{bmatrix} =
\begin{bmatrix}{}\frac{1}{9}\\-\frac{2}{9}\\-\frac{2}{9}\end{bmatrix} = p_1
$$

$$ p_2 = P_2b $$

$$ P_2b =
\frac{1}{9}
\left[\begin{array}{rrr}
4 & 4 & -2 \\
4 & 4 & -2 \\
-2 & -2 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\frac{1}{9}
\begin{bmatrix}{}4\\4\\-2\end{bmatrix} =
\begin{bmatrix}{}\frac{4}{9}\\\frac{4}{9}\\-\frac{2}{9}\end{bmatrix} = p_2
$$

$$ a_3 = \begin{bmatrix}{}2\\-1\\2\end{bmatrix} $$

$$ p_3 = P_3b $$

$$ P_3 = \frac{a_3(a_3)^{\mathbf{T}}}{(a_3)^{\mathbf{T}}a_3} $$

$$ P_3 = \frac{1}{9}a_3(a_3)^{\mathbf{T}} $$

$$ a_3(a_3)^{\mathbf{T}} =
\begin{bmatrix}{}2\\-1\\2\end{bmatrix}
\left[\begin{array}{rrr}
2 & -1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
4 & -2 & 4 \\
-2 & 1 & -2 \\
4 & -2 & 4 \\
\end{array}\right]
$$

$$ P_3 =
\frac{1}{9}
\left[\begin{array}{rrr}
4 & -2 & 4 \\
-2 & 1 & -2 \\
4 & -2 & 4 \\
\end{array}\right]
$$

$$ P_3b =
\frac{1}{9}
\left[\begin{array}{rrr}
4 & -2 & 4 \\
-2 & 1 & -2 \\
4 & -2 & 4 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\\0\end{bmatrix} =
\frac{1}{9}
\begin{bmatrix}{}4\\-2\\4\end{bmatrix} =
\begin{bmatrix}{}\frac{4}{9}\\-\frac{2}{9}\\\frac{4}{9}\end{bmatrix} = p_3
$$

_Add up the three projections $p_1 + p_2 + p_3$:_

$$ p_1 + p_2 + p_3 =
\begin{bmatrix}{}\frac{1}{9}\\-\frac{2}{9}\\-\frac{2}{9}\end{bmatrix} +
\begin{bmatrix}{}\frac{4}{9}\\\frac{4}{9}\\-\frac{2}{9}\end{bmatrix} +
\begin{bmatrix}{}\frac{4}{9}\\-\frac{2}{9}\\\frac{4}{9}\end{bmatrix} =
\begin{bmatrix}{}1\\0\\0\end{bmatrix} = b
$$

7. Continuing Problems 5-6, find the projection matrix $P_3$ onto
   $a_3 = (2, -1, 2)$. Verify that $P_1 + P_2 + P_3 = I$. This is because the
   basis $a_1, a_2, a_3$ is orthogonal!

(See Page 226 for figures)

Omitted, but take note of what is being said here.

8. Project the vector $b = (1, 1)$ onto the lines through $a_1 = (1, 0)$ and
   $a_2 = (1, 2)$. Draw the projections $p_1$ and $p_2$ and add $p_1 + p_2$. The
   projections do not add to $b$ because the $a$'s are not orthogonal.

_Solution:_

$$ p_1 = a_1\hat{x}_1 = a_1\frac{(a_1)^{\mathbf{T}}b}{(a_1)^{\mathbf{T}}a_1} = P_1b $$

$$ p_1 = a_1\frac{(a_1)^{\mathbf{T}}b}{1} = P_1b $$

$$ p_1 = a_1(a_1)^{\mathbf{T}}b = P_1b $$

$$ a_1(a_1)^{\mathbf{T}} =
\begin{bmatrix}{}1\\0\end{bmatrix}
\left[\begin{array}{cc}
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ p_1 = a_1(a_1)^{\mathbf{T}}b =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\end{bmatrix} =
\begin{bmatrix}{}1\\0\end{bmatrix} = P_1b
$$

$$ p_2 = a_2\hat{x}_2 = a_2\frac{(a_2)^{\mathbf{T}}b}{(a_2)^{\mathbf{T}}a_2} = P_2b $$

$$ p_2 = \frac{1}{5}a_2(a_2)^{\mathbf{T}}b = P_2b $$

$$ a_2(a_2)^{\mathbf{T}} =
\begin{bmatrix}{}1\\2\end{bmatrix}
\left[\begin{array}{cc}
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
$$

$$ p_2 = \frac{1}{5}a_2(a_2)^{\mathbf{T}}b =
\frac{1}{5}
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\end{bmatrix} =
\frac{1}{5}
\begin{bmatrix}{}3\\6\end{bmatrix} =
\frac{3}{5}
\begin{bmatrix}{}1\\2\end{bmatrix} = P_2b
$$

_Add $p_1 + p_2$:_

$$ p_1 + p_2 =
\begin{bmatrix}{}1\\0\end{bmatrix} +
\frac{3}{5}
\begin{bmatrix}{}1\\2\end{bmatrix} =
\frac{1}{5}
\begin{bmatrix}{}8\\6\end{bmatrix} \neq b
$$

9. In Problem 8, the projection of $b$ onto the _plane_ of $a_1$ and $a_2$ will
   equal $b$. Find $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ for
   $A = \left[\begin{array}{cc}a_1 & a_2 \\\end{array}\right] = \left[\begin{array}{cc}1 & 1 \\0 & 2 \\\end{array}\right] =$
   invertible matrix.

_Solution:_

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
1 & 0 \\
1 & 2 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
1 & 5 \\
\end{array}\right]
$$

Now use Gauss-Jordan elimination to find $(A^{\mathbf{T}}A)^{-1}$:

$$
\left[\begin{array}{cc|cc}
1 & 1 & 1 & 0 \\
1 & 5 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 1 & 1 & 0 \\
0 & 4 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 1 & 1 & 0 \\
0 & 1 & -\frac{1}{4} & \frac{1}{4} \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 0 & \frac{5}{4} & -\frac{1}{4} \\
0 & 1 & -\frac{1}{4} & \frac{1}{4} \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{rr}
\frac{5}{4} & -\frac{1}{4} \\
-\frac{1}{4} & \frac{1}{4}
\end{array}\right] = (A^{\mathbf{T}}A)^{-1}
$$

$$ A(A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{cc}
1 & 1 \\
0 & 2 \\
\end{array}\right]
\left[\begin{array}{rr}
\frac{5}{4} & -\frac{1}{4} \\
-\frac{1}{4} & \frac{1}{4}
\end{array}\right] =
\left[\begin{array}{rr}
1 & 0 \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right]
$$

$$ A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\left[\begin{array}{rr}
1 & 0 \\
-\frac{1}{2} & \frac{1}{2} \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

The easier thing to do is to recognize that we can rewrite
$(A^{\mathbf{T}}A)^{-1}$ as $A^{-1}(A^{\mathbf{T}})^{-1}$. Note that we can only
do this because $A$ is invertible (otherwise this is _not_ allowed). Once we do
that though, everything cancels out and leaves us with $I$.

10. Project $a_1 = (1, 0)$ onto $a_2 = (1, 2)$. Then project the result back
    onto $a_1$. Draw these projections and multiply the projection matrices
    $P_1P_2$: Is this a projection?

_Solution:_

Here, don't get confused, "Project some vector onto some other vector" here
means treat $b$ as the first vector prior to the wording "onto", and $a$ as the
other vector after the wording "onto".

The classic formula:

$$ P = \frac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a} $$

Becomes:

$$ P_2 = \frac{a_2(a_2)^{\mathbf{T}}}{(a_2)^{\mathbf{T}}a_2} $$

Now to solve:

$$ P_2 = \frac{1}{5}a_2(a_2)^{\mathbf{T}}$$

$$ a_2(a_2)^{\mathbf{T}} =
\begin{bmatrix}{}1\\2\end{bmatrix}
\left[\begin{array}{cc}
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
$$

$$ P_2 = \frac{1}{5}a_2(a_2)^{\mathbf{T}} =
\frac{1}{5}
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
$$

$$ P_2a_1 =
\frac{1}{5}
\left[\begin{array}{cc}
1 & 2 \\
2 & 4 \\
\end{array}\right]
\begin{bmatrix}{}1\\0\end{bmatrix} =
\frac{1}{5}
\begin{bmatrix}{}1\\2\end{bmatrix} =
\begin{bmatrix}{}\frac{1}{5}\\\frac{2}{5}\end{bmatrix}
$$

_Then project the result back onto $a_1$:_

$$ P_1 = \frac{a_1(a_1)^{\mathbf{T}}}{(a_1)^{\mathbf{T}}a_1} $$

$$ P_1 = \frac{a_1(a_1)^{\mathbf{T}}}{1} $$

$$ P_1 = a_1(a_1)^{\mathbf{T}} =
\begin{bmatrix}{}1\\0\end{bmatrix}
\left[\begin{array}{cc}
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
$$

$$ P_1P_2a_1 =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}\frac{1}{5}\\\frac{2}{5}\end{bmatrix} =
\begin{bmatrix}{}\frac{1}{5}\\0\end{bmatrix} \neq a_1 = (1, 0)
$$

_Draw these projections and multiply the projection matrices $P_1P_2$. Is this a
projection?:_

$$ P_1P_2 =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
\frac{1}{5} & \frac{2}{5} \\
\frac{2}{5} & \frac{4}{5} \\
\end{array}\right] =
\left[\begin{array}{cc}
\frac{1}{5} & \frac{2}{5} \\
0 & 0 \\
\end{array}\right]
$$

No, this is not a projection, since $P_1P_2 \neq (P_1P_2)^2$.

**Questions 11-20 ask for projections, and projection matrices, onto
subspaces.**

11. Project $b$ onto the column space of $A$ by solving
    $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$ and $p = A\hat{x}$:

Find $e = b - p$. It should be perpendicular to the columns of $A$.

a. $A = \left[\begin{array}{cc}1 & 1 \\0 & 1 \\0 & 0 \\\end{array}\right]$ and
$b = \begin{bmatrix}{}2\\3\\4\end{bmatrix}$

_Solution:_

Here, solve for $\hat{x}$ by solving $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$,
then compute $p = A\hat{x}$.

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}Ax =
\left[\begin{array}{cc}
1 & 1 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\end{bmatrix} =
\begin{bmatrix}{}x_1 + x_2\\x_1 + 2x_2\end{bmatrix}
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}b_1\\b_2\\b_3\end{bmatrix} =
\begin{bmatrix}{}b_1\\b_1 + b_2\end{bmatrix} =
\begin{bmatrix}{}2\\2 + 3\end{bmatrix} =
\begin{bmatrix}{}2\\5\end{bmatrix}
$$

$$ A^{\mathbf{T}}Ax = \begin{bmatrix}{}x_1 + x_2\\x_1 + 2x_2\end{bmatrix} = \begin{bmatrix}{}2\\5\end{bmatrix} = A^{\mathbf{T}}b $$

$$
x_1 + x_2 = 2 \\
x_1 + 2x_2 = 5 \\
$$

$$ (x_1 + 2x_2 = 5) - (x_1 + x_2 = 2) \Rightarrow x_2 = 3 $$

$$ x_1 + (3) = 2 \Rightarrow x_1 = -1 $$

Check:

$$ (-1) + 2(3) = -1 + 6 = 5 = 5 $$

So:

$$ \hat{x} = \begin{bmatrix}{}-1\\3\end{bmatrix} $$

Now solve $p = A\hat{x}$:

$$ p = A\hat{x} =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}-1\\3\end{bmatrix} =
\begin{bmatrix}{}2\\3\\0\end{bmatrix}
$$

_Find $e = b - p$:_

$$ e = b - p =
\begin{bmatrix}{}2\\3\\4\end{bmatrix} - \begin{bmatrix}{}2\\3\\0\end{bmatrix} = \begin{bmatrix}{}0\\0\\4\end{bmatrix}
$$

$$ A^{\mathbf{T}}e =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}0\\0\\4\end{bmatrix} =
\begin{bmatrix}{}0\\0\end{bmatrix} = \mathbf{0} \Rightarrow e \perp C(A)
$$

b. $A = \left[\begin{array}{cc}1 & 1 \\1 & 1 \\0 & 1 \\\end{array}\right]$ and
$b = \begin{bmatrix}{}4\\4\\6\end{bmatrix}$

_Solution:_

$$ A^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 2 \\
2 & 3 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
2 & 2 \\
2 & 3 \\
\end{array}\right]
\begin{bmatrix}{}\hat{x}_1\\\hat{x}_2\end{bmatrix} =
\begin{bmatrix}{}2\hat{x}_1 + 2\hat{x}_2\\2\hat{x}_1 + 3\hat{x}_2\end{bmatrix}
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}4\\4\\6\end{bmatrix} =
\begin{bmatrix}{}8\\14\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\begin{bmatrix}{}2\hat{x}_1 + 2\hat{x}_2\\2\hat{x}_1 + 3\hat{x}_2\end{bmatrix} =
\begin{bmatrix}{}8\\14\end{bmatrix} =
A^{\mathbf{T}}b
$$

$$
2\hat{x}_1 + 2\hat{x}_2 = 8 \\
2\hat{x}_1 + 3\hat{x}_2 = 14 \\
$$

$$
(2\hat{x}_1 + 3\hat{x}_2 = 14) - (2\hat{x}_1 + 2\hat{x}_2 = 8) \Rightarrow \hat{x}_2 = 6
$$

$$ 2\hat{x}_1 + 3(6) = 14 \Rightarrow 2\hat{x}_1 + 18 = 14 \Rightarrow 2\hat{x}_1 = -4 \Rightarrow \hat{x}_1 = -2 $$

Check:

$$ 2(-2) + 2(6) = -4 + 12 = 8 = 8 $$

$$ \hat{x} = \begin{bmatrix}{}-2\\6\end{bmatrix} $$

$$ p = A\hat{x} =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}-2\\6\end{bmatrix} =
\begin{bmatrix}{}4\\4\\6\end{bmatrix}
$$

_Find $e = b - p$:_

$$ e = b - p =
\begin{bmatrix}{}4\\4\\6\end{bmatrix} -
\begin{bmatrix}{}4\\4\\6\end{bmatrix} = \mathbf{0} \Rightarrow b \in C(A)
$$

12. Compute the projection matrices $P_1$ and $P_2$ onto the column spaces in
    Problem 11. Verify that $P_1b$ gives the first projection $p_1$. Also verify
    $P_2^2 = P_2$.

_Solution:_

a.

_Compute the projection matrices $P_1$ and $P_2$ onto the column spaces in
Problem 11:_

Recall the generic Projection matrix formula:

$$ P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} $$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

Use Gauss-Jordan elimination to find $(A^{\mathbf{T}}A)^{-1}$:

$$
\left[\begin{array}{cc|cc}
1 & 1 & 1 & 0 \\
1 & 2 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 1 & 1 & 0 \\
0 & 1 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 0 & 2 & -1 \\
0 & 1 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr}
2 & -1 \\
-1 & 1 \\
\end{array}\right]
= (A^{\mathbf{T}}A)^{-1}
$$

$$ A(A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{rr}
2 & -1 \\
-1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
-1 & 1 \\
0 & 0 \\
\end{array}\right]
$$

$$ A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\left[\begin{array}{cc}
1 & 0 \\
-1 & 1 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right] = P_1
$$

This is the projection matrix onto $C(A)$, which in this case is the $xy$ plane.

_Verify that $P_1b$ gives the first projection $p_1$:_

$$ P_1b =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}2\\3\\4\end{bmatrix} =
\begin{bmatrix}{}2\\3\\0\end{bmatrix} = p
$$

b.

_Compute the projection matrices $P_1$ and $P_2$ onto the column spaces in
Problem 11:_

$$ A^\mathbf{T}A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 2 \\
2 & 3 \\
\end{array}\right]
$$

Use Gauss-Jordan elimination to find $(A^\mathbf{T}A)^{-1}$:

$$
\left[\begin{array}{cc|cc}
2 & 2 & 1 & 0 \\
2 & 3 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
2 & 2 & 1 & 0 \\
0 & 1 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 1 & \frac{1}{2} & 0 \\
0 & 1 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 0 & \frac{3}{2} & -1 \\
0 & 1 & -1 & 1 \\
\end{array}\right]
$$

$$
\to
\left[\begin{array}{rr}
\frac{3}{2} & -1 \\
-1 & 1 \\
\end{array}\right] = (A^{\mathbf{T}}A)^{-1}
$$

$$ A(A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{rr}
\frac{3}{2} & -1 \\
-1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
\frac{1}{2} & 0 \\
\frac{1}{2} & 0 \\
-1 & 1 \\
\end{array}\right]
$$

$$ A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\left[\begin{array}{cc}
\frac{1}{2} & 0 \\
\frac{1}{2} & 0 \\
-1 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
\frac{1}{2} & \frac{1}{2} & 0 \\
\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 0 & 1 \\
\end{array}\right] = P_2
$$

_Also verify $P_2^2 = P_2$:_

$$ P_2^2 = P_2 \cdot P_2 =
\left[\begin{array}{ccc}
\frac{1}{2} & \frac{1}{2} & 0 \\
\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{ccc}
\frac{1}{2} & \frac{1}{2} & 0 \\
\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
\frac{1}{2} & \frac{1}{2} & 0 \\
\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 0 & 1 \\
\end{array}\right] = P_2
$$

13. (Quick and Recommended) Suppose $A$ is the $4$ by $4$ identity matrix with
    its last column removed. $A$ is $4$ by $3$. Project $b = (1, 2, 3, 4)$ onto
    the column space of $A$. What shape is the projection matrix $P$ and what is
    $P$?

_Solution:_

$$ A =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ C(A) = \left\{\begin{bmatrix}{}1\\0\\0\\0\end{bmatrix}, \begin{bmatrix}{}0\\1\\0\\0\end{bmatrix}, \begin{bmatrix}{}0\\0\\1\\0\end{bmatrix}\right\} $$

Now, compute $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$:

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] = I
$$

So:

$$ P = A(I)A^{\mathbf{T}} $$

$$ P = AA^{\mathbf{T}} $$

$$ AA^{\mathbf{T}} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right] = P
$$

Then, calculate the projection of $Pb$, which will give us the projection of $b$
on $C(A)$.

$$ Pb =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\3\\4\end{bmatrix} =
\begin{bmatrix}{}1\\2\\3\\0\end{bmatrix}
$$

The shape of the projection matrix $P$ is $4$ by $4$, and it is the projection
onto the $x, y, z$ plane of $A$.

14. Suppose $b$ equals $2$ times the first column of $A$. What is the projection
    of $b$ onto the column space of $A$? Is $P = I$ for sure in this case?
    Compute $p$ and $P$ when $b = (0, 2, 4)$ and the columns of $A$ are
    $(0, 1, 2)$ and $(1, 2, 0)$.

_Solution:_

_What is the projection of $b$ onto the column space of $A$?:_

In the standard formula of $Ax = b$, since $b$ is $2a_{i1} \in A$, it follows
that $b \in C(A)$, and so the projection of $b$ onto $C(A)$ is $b$ itself.

_Is $P = I$ for sure in this case?:_

Not necessarily, in order for $P = I$, $A$ must be an invertible square matrix,
which is not defined in the problem statement.

_Compute $p$ and $P$ when $b = (0, 2, 4)$ and the columns of $A$ are $(0, 1, 2)$
and $(1, 2, 0)$:_

$$ A =
\left[\begin{array}{cc}
0 & 1 \\
1 & 2 \\
2 & 0 \\
\end{array}\right]
$$

$$ P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} $$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
0 & 1 & 2 \\
1 & 2 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
1 & 2 \\
2 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
5 & 2 \\
2 & 5 \\
\end{array}\right]
$$

Now via Gauss-Jordan elimination, find $(A^{\mathbf{T}}A)^{-1}$:

$$
\left[\begin{array}{cc|cc}
5 & 2 & 1 & 0 \\
2 & 5 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
5 & 2 & 1 & 0 \\
0 & \frac{21}{5} & -\frac{2}{5} & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
5 & 2 & 1 & 0 \\
0 & 1 & -\frac{2}{21} & \frac{5}{21} \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & \frac{2}{5} & \frac{1}{5} & 0 \\
0 & 1 & -\frac{2}{21} & \frac{5}{21} \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{cc|cc}
1 & 0 & \frac{5}{21} & -\frac{2}{21} \\
0 & 1 & -\frac{2}{21} & \frac{5}{21} \\
\end{array}\right] \to
\left[\begin{array}{rr}
\frac{5}{21} & -\frac{2}{21} \\
-\frac{2}{21} & \frac{5}{21} \\
\end{array}\right] = (A^{\mathbf{T}}A)^{-1}
$$

$$ A(A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{cc}
0 & 1 \\
1 & 2 \\
2 & 0 \\
\end{array}\right]
\left[\begin{array}{rr}
\frac{5}{21} & -\frac{2}{21} \\
-\frac{2}{21} & \frac{5}{21} \\
\end{array}\right] =
\left[\begin{array}{rr}
-\frac{2}{21} & \frac{5}{21} \\
\frac{1}{21} & \frac{8}{21} \\
\frac{10}{21} & -\frac{4}{21} \\
\end{array}\right]
$$

$$ A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\frac{1}{21}
\left[\begin{array}{rr}
-2 & 5 \\
1 & 8 \\
10 & -4 \\
\end{array}\right]
\left[\begin{array}{ccc}
0 & 1 & 2 \\
1 & 2 & 0 \\
\end{array}\right] =
\frac{1}{21}
\left[\begin{array}{rrr}
5 & 8 & -4 \\
8 & 17 & 2 \\
-4 & 2 & 20 \\
\end{array}\right] = P
$$

$$ Pb =
\frac{1}{21}
\left[\begin{array}{rrr}
5 & 8 & -4 \\
8 & 17 & 2 \\
-4 & 2 & 20 \\
\end{array}\right]
\begin{bmatrix}{}0\\2\\4\end{bmatrix} =
\frac{1}{21}
\begin{bmatrix}{}0\\42\\84\end{bmatrix} =
\begin{bmatrix}{}0\\2\\4\end{bmatrix} = p = b
$$

15. If $A$ is doubled, then $P = 2A(4A^{\mathbf{T}}A)^{-1}2A^{\mathbf{T}}$. This
    is the same as $A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$. The column space of
    $2A$ is the same as ____. Is $\hat{x}$ the same for $A$ and $2A$?

_Solution:_

_The column space of $2A$ is the same as (?):_

$A$

_Is $\hat{x}$ the same for $A$ and $2A$?:_

Consider that:

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

So when we apply $2A$

$$ \hat{x} = \frac{(2a)^{\mathbf{T}}b}{(2a)^{\mathbf{T}}2a} $$

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}2a} $$

So actually $\hat{x}$ is not the same for $A$ as for $2A$, in fact $\hat{x}$ is
halved for $2A$.

16. What linear combination of $(1, 2, -1)$ and $(1, 0, 1)$ is closest to
    $b = (2, 1, 1)$?

_Solution:_

Put the two given vectors in a matrix $A$, then solve for
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:

$$ A =
\left[\begin{array}{rr}
1 & 1 \\
2 & 0 \\
-1 & 1 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrr}
1 & 2 & -1 \\
1 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & 1 \\
2 & 0 \\
-1 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
6 & 0 \\
0 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
6 & 0 \\
0 & 2 \\
\end{array}\right]
\begin{bmatrix}{}\hat{x}_1\\\hat{x}_2\end{bmatrix} =
\begin{bmatrix}{}6\hat{x}_1\\2\hat{x}_2\end{bmatrix}
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{rrr}
1 & 2 & -1 \\
1 & 0 & 1 \\
\end{array}\right]
\begin{bmatrix}{}2\\1\\1\end{bmatrix} =
\begin{bmatrix}{}3\\3\end{bmatrix}
$$

$$
6\hat{x}_1 = 3 \\
2\hat{x}_2 = 3 \\
$$

$$
\hat{x}_1 = \frac{1}{2} \\
\hat{x}_2 = \frac{3}{2} \\
$$

$$ \hat{x} =
\frac{1}{2}
\begin{bmatrix}{}1\\3\end{bmatrix}
$$

So, the closest linear combination to $b$ is:

$$ p = A\hat{x} = \frac{1}{2}\begin{bmatrix}{}1\\2\\-1\end{bmatrix} + \frac{3}{2}\begin{bmatrix}{}1\\0\\1\end{bmatrix} $$

17. (_Important_) If $P^2 = P$ show that $(I - P)^2 = I - P$. When $P$ projects
    onto the column space of $A$, $I - P$ projects onto the ____.

_Solution:_

_If $P^2 = P$ show that $(I - P)^2 = I - P$:_

**Proof:**

Suppose $P^2 = P$.

It is to be shown that $(I - P)^2 = I - P$.

Consider that:

$$ (I - P)^2 = (I - P)(I - P) $$

$$ = I^2 - PI  - IP + P^2 $$

Since the any matrix multiplied by the identity matrix $I$ returns that matrix,
it follows that $I^2 = I$.

$$ = I - PI  - IP + P^2 $$

By the supposition, since $P^2 = P$, we can substitute as follows:

$$ = I - PI  - IP + P $$

Once again, since $I$ multiplied by any matrix returns that matrix, we have:

$$ = I - P - P + P $$

$$ = I - 2P + P $$

$$ = I - P $$

This is what was to be shown.

Q.E.D.

_When $P$ projects onto the column space of $A$, $I - P$ projects onto the (?):_

left nullspace, $N(A^{\mathbf{T}})$.

This follows as $(I - P)b = b - Pb = b - p = e$. As long as $e \neq 0$, it
follows that $e \in N(A^{\mathbf{T}})$.

18.

a. If $P$ is the $2$ by $2$ projection matrix onto the line through $(1, 1)$,
then $I - P$ is the projection matrix onto ____.

_Solution:_

We need a vector that when multiplied by $(1, 1)$ gives $0$.

$$ \begin{bmatrix}{}v_1\\v_2\end{bmatrix} \cdot \begin{bmatrix}{}1\\1\end{bmatrix} = 0 $$

$$ v_1(1) + v_2(1) = 0 $$

$$ v_1 + v_2 = 0 $$

$$ v_1 = -v_2 $$

So $v = \begin{bmatrix}{}1\\-1\end{bmatrix}$.

So if $P$ projects onto the line through $(1, 1)$, then $I - P$ is the
projection matrix onto $(1, -1)$.

b. If $P$ is the $3$ by $3$ projection matrix onto the line through $(1, 1, 1)$,
then $I - P$ is the projection matrix onto ____.

_Solution:_

$I - P$ is the projection matrix onto the plane:

$$ x + y + z = 0 $$

which is perpendicular to $(1, 1, 1)$.

19. To find the projection matrix onto the plane $x - y - 2z = 0$, choose two
    vectors in that plane and make them the columns of $A$. The plane will be
    the column space of $A$! Then compute
    $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$.

_Solution:_

_To find the projection matrix onto the plane $x - y - 2z = 0$, choose two
vectors in that plane and make them the columns of $A$:_

$$ x - y - 2z = 0 $$

Choose $y = 1, z = 0$:

$$ x - (1) - 2(0) = 0 \Rightarrow x = 1 $$

one vector then is $\begin{bmatrix}{}1\\1\\0\end{bmatrix}$

Choose $y = 0, z = 1$:

$$ x - (0) - 2(1) = 0 \Rightarrow x = 2 $$

another vector then is $\begin{bmatrix}{}2\\0\\1\end{bmatrix}$

Now make them the columns of $A$:

$$ A =
\left[\begin{array}{cc}
1 & 2 \\
1 & 0 \\
0 & 1 \\
\end{array}\right]
$$

_Then compute $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$:_

$$ A^{\mathbf{T}}A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 2 \\
1 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
2 & 2 \\
2 & 5 \\
\end{array}\right]
$$

Find $(A^{\mathbf{T}}A)^{-1}$ via Guass-Jordan:

$$
\left[\begin{array}{cc|cc}
2 & 2 & 1 & 0 \\
2 & 5 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
2 & 2 & 1 & 0 \\
0 & 3 & -1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
2 & 2 & 1 & 0 \\
0 & 1 & -\frac{1}{3} & \frac{1}{3} \\
\end{array}\right] \to
\left[\begin{array}{cc|cc}
1 & 1 & \frac{1}{2} & 0 \\
0 & 1 & -\frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{cc|cc}
1 & 0 & \frac{5}{6} & -\frac{1}{3} \\
0 & 1 & -\frac{1}{3} & \frac{1}{3} \\
\end{array}\right] \to
\left[\begin{array}{rr}
\frac{5}{6} & -\frac{1}{3} \\
-\frac{1}{3} & \frac{1}{3} \\
\end{array}\right] = (A^{\mathbf{T}}A)^{-1}
$$

$$ A(A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{cc}
1 & 2 \\
1 & 0 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{rr}
\frac{5}{6} & -\frac{1}{3} \\
-\frac{1}{3} & \frac{1}{3} \\
\end{array}\right] =
\left[\begin{array}{rr}
\frac{1}{6} & \frac{1}{3} \\
\frac{5}{6} & -\frac{1}{3} \\
-\frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
$$

$$ A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\left[\begin{array}{rr}
\frac{1}{6} & \frac{1}{3} \\
\frac{5}{6} & -\frac{1}{3} \\
-\frac{1}{3} & \frac{1}{3} \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 1 & 0 \\
2 & 0 & 1 \\
\end{array}\right] =
\frac{1}{6}
\left[\begin{array}{rrr}
5 & 1 & 2 \\
1 & 5 & -2 \\
2 & -2 & 2 \\
\end{array}\right] = P
$$

20. To find the projection matrix $P$ onto the same plane $x - y - 2z = 0$,
    write down a vector $e$ that is perpendicular to that plane. Compute the
    projection $Q = ee^{\mathbf{T}}/e^{\mathbf{T}}e$ and then $P = I - Q$.

_Solution:_

With $e$ being perpendicular to the plane $x - y - 2z = 0$, it is sufficient to
define $e$ as a vector with those coefficients as its components:

$$ e = \begin{bmatrix}{}1\\-1\\-2\end{bmatrix} $$

Now, to compute $Q$:

$$ ee^{\mathbf{T}} =
\begin{bmatrix}{}1\\-1\\-2\end{bmatrix}
\left[\begin{array}{ccc}
1 & -1 & -2 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & -1 & -2 \\
-1 & 1 & 2 \\
-2 & 2 & 4 \\
\end{array}\right]
$$

$$ e^{\mathbf{T}}e =
\left[\begin{array}{ccc}
1 & -1 & -2 \\
\end{array}\right]
\begin{bmatrix}{}1\\-1\\-2\end{bmatrix} =
(1)(1) + (-1)(-1) + (-2)(-2) =
1 + 1 + 4 = 6
$$

$$ Q = \frac{ee^{\mathbf{T}}}{e^{\mathbf{T}}e} =
\frac{1}{6}
\left[\begin{array}{rrr}
1 & -1 & -2 \\
-1 & 1 & 2 \\
-2 & 2 & 4 \\
\end{array}\right]
$$

Now compute $P = I - Q$:

$$ I - Q =
\left[\begin{array}{cc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] -
\frac{1}{6}
\left[\begin{array}{rrr}
1 & -1 & -2 \\
-1 & 1 & 2 \\
-2 & 2 & 4 \\
\end{array}\right] =
\left[\begin{array}{rrr}
\frac{5}{6} & \frac{1}{6} & \frac{1}{3} \\
\frac{1}{6} & \frac{5}{6} & -\frac{1}{3} \\
\frac{1}{3} & -\frac{1}{3} & \frac{1}{3} \\
\end{array}\right] = P
$$

This matches the $P$ from problem 19.

**Questions 21-26 show that projection matrices satisfy $P^2 = P$ and
$P^{\mathbf{T}} = P$.**

21. Multiply the matrix $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ by itself.
    Cancel to prove that $P^2 = P$. Explain why $P(Pb)$ always equals $Pb$: The
    vector $Pb$ is in the column space of $A$ so its projection onto that column
    space is ____.

_Solution:_

_Multiply the matrix $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ by itself.
Cancel to prove that $P^2 = P$:_

$$ (A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}})(A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}) $$

$$ = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} $$

$$ = A(A^{\mathbf{T}}A)^{-1}IA^{\mathbf{T}} $$

$$ = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} = P $$

_Explain why $P(Pb)$ always equals $Pb$: The vector $Pb$ is in the column space
of $A$ so its projection onto that column space is (?):_

$Pb$

22. Prove that $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ is symmetric by
    computing $P^{\mathbf{T}}$. Remember that the inverse of a symmetric matrix
    is symmetric.

_Solution:_

**Proof:**

Suppose $P$ is a projection onto a matrix $A$. It is to be shown that $P$ is
symmetric. This is demonstrated by showing that $P = P^{\mathbf{T}}$.

By the definition of a projection:

$$ P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} $$

If we then take the transpose of $P$, $P^{\mathbf{T}}$:

$$ P^{\mathbf{T}} = (A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}})^{\mathbf{T}} $$

By the "distributive" property of transposition:

$$ P^{\mathbf{T}} = (A^{\mathbf{T}})^{\mathbf{T}}((A^{\mathbf{T}}A)^{-1})^{\mathbf{T}}(A^{\mathbf{T}}) $$

Now, transpose of a transpose negates that transposition, so:

$$ P^{\mathbf{T}} = A((A^{\mathbf{T}}A)^{-1})^{\mathbf{T}}A^{\mathbf{T}} $$

Since $(A^{\mathbf{T}}A)^{-1}$ is symmetric, it follows that
$((A^{\mathbf{T}}A)^{-1})^{\mathbf{T}} = (A^{\mathbf{T}}A)^{-1}$:

$$ P^{\mathbf{T}} = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} = P $$

By the definition of symmetric, it can be concluded that $P$ is symmetric.

This is what was to be shown.

Q.E.D.

23. If $A$ is square and invertible, the warning against splitting
    $(A^{\mathbf{T}}A)^{-1}$ does not apply. Is it true that
    $AA^{-1}(A^{\mathbf{T}})^{-1}A^{\mathbf{T}} = I$. _When $A$ is invertible,
    why is $P = I$_? _What is the error $e$?_

_Solution:_

_When $A$ is invertible, why is $P = I$?:_

When $A$ is invertible, this means that $C(A) = R^n$. In other words, the column
space of $A$ is all of $R^n$.

_What is the error $e$?:_

This results in $P = I$, and thus $e = \mathbf{0}$.

24. The nullspace of $A^{\mathbf{T}}$ is ____ to the column space $C(A)$. So if
    $A^{\mathbf{T}}b = \mathbf{0}$, the projection of $b$ onto $C(A)$ should be
    $p =$ ____. Check that $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ gives
    this answer.

_Solution:_

_The nullspace of $A^{\mathbf{T}}$ is (?) to the column space $C(A)$:_

orthogonal

_So if $A^{\mathbf{T}}b = \mathbf{0}$, the projection of $b$ onto $C(A)$ should
be $p =$ (?):_

$\mathbf{0}$

_Check that $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ gives this answer:_

$$ Pb = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}b $$

$$ Pb = A(A^{\mathbf{T}}A)^{-1}\mathbf{0} $$

$$ Pb = \mathbf{0} $$

25. The projection matrix $P$ onto an $n$-dimensional subspace of $\R^m$ has
    rank $r = n$. _Reason:_ The projections $Pb$ fill the subspace $S$. So $S$
    is the ____ of $P$.

_Solution:_

_So $S$ is the (?) of $P$:_

column space

26. If an $m$ by $m$ matrix has $A^2 = A$ and its rank is $m$, prove that
    $A = I$.

**Proof:**

Suppose $A$ is any $m$ by $m$ matrix where $A$'s rank is $m$, $r = m$.
Furthermore, suppose $A^2 = A$.

It is to be demonstrated that $A = I$.

Since $r = m$, it follows that $A$ is invertible, in other words, $A^{-1}$
exists.

Since we know that $A^{-1}$ exists, multiply $A^2 = A$ by $A^{-1}$:

$$ A^2(A^{-1}) = AA^{-1} $$

By the definition of inverses and identity, we can substitute the right-hand
side of this equation as shown:

$$ A^2(A^{-1}) = I $$

Now, simply expand out $A^2$:

$$ AA(A^{-1}) = I $$

$$ AI = I $$

$$ A = I $$

This is what was to be shown.

Q.E.D.

27. The important fact that ends the section is this: _If
    $A^{\mathbf{T}}Ax = \mathbf{0}$ then $Ax = \mathbf{0}$_. _New Proof_: The
    vector $Ax$ is in the nullspace of ____. $Ax$ is always in the column space
    of ____. To be in both of those perpendicular spaces, $Ax$ must be zero.

_Solution:_

_The vector $Ax$ is in the nullspace of (?):_

$A^{\mathbf{T}}$

_$Ax$ is always in the column space of (?):_

$A$

28. Use $P^{\mathbf{T}} = P$ and $P^2 = P$ to prove that the length squared of
    column $2$ always equals the diagonal entry $P_{22}$. This number is
    $\dfrac{2}{6} = \dfrac{4}{36} + \dfrac{4}{36} + \dfrac{4}{36}$ for

$$ P =
\frac{1}{6}\left[\begin{array}{rrr}
5 & 2 & -1 \\
2 & 2 & 2 \\
-1 & 2 & 5 \\
\end{array}\right]
$$

_Solution:_

Note that here "length" of a column refers to the Euclidean norm of the three
coordinates (see [scratch.md](./scratch.md))

Thus
$\|\text{col } 2\|^2 = \left(\dfrac{2}{6}\right)^2 + \left(\dfrac{2}{6}\right)^2 + \left(\dfrac{2}{6}\right)^2 = \dfrac{2}{6} = P_{22}$.

**Proof:**

Since $P^2 = P = P^{\mathbf{T}}$, we can write $P^2 = P^{\mathbf{T}}P = P$.

Now, consider especially $P^{\mathbf{T}}P$, when we multiply these two
projection matrices together, we get the dot product of $P$'s rows times $P$'s
columns. If we then consider the length of column $2$, this will always be the
Euclidean norm length, which sums all the components of the second column of
$P^{\mathbf{T}}P$ squared.

It follows that since $P^{\mathbf{T}}P = P$, that the $(2, 2)$ entry of
$P^{\mathbf{T}}P = P_{22}$. Thus it follows that $\|\text{col } 2\|^2 = P_{22}$.

Q.E.D.

29. If $B$ has rank $m$ (full row rank, independent rows) show that
    $BB^{\mathbf{T}}$ is invertible.

$A^{\mathbf{T}}$ has independent columns so $A^{\mathbf{T}}A$ (which is
$BB^{\mathbf{T}}$) must be invertible.

---

Page 240

## Problem Set 4.3

**Problems 1-11 use four data points $b = (0, 8, 8, 20)$ to bring out the key
ideas.**

(See Page 240 for Figure 4.9)

1. With $b = 0, 8, 8, 20$ at $t = 0, 1, 3, 4$, set up and solve the normal
   equations $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$. For the best straight
   line in Figure 4.9a, find its four heights $p_i$ and four errors $e_i$. What
   is the minimum value $E = e_1^2 + e_2^2 + e_3^2 + e_4^2$?

_Solution:_

_With $b = 0, 8, 8, 20$ at $t = 0, 1, 3, 4$, set up and solve the normal
equations $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:_

Recall slope intercept form from algebra: $y = mx + b$. This is the same as what
Strang presents as the equation for a line: $b = C + Dt$, where
$y \leftrightarrow b, m \leftrightarrow D, x \leftrightarrow t, b \leftrightarrow C$.

Thus when defining a matrix $A$ (we are given $b$), we are concerned with these
two columns, $C$ and $Dt$. Since the coefficient of $C$ never changes in this
case of fitting a line, the first column of $A$ is always just all $1$'s. The
only number that changes is $D$, which has coefficients based off the input,
$t$.

Thus, define $A$ and $b$ as :

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
1 & 3 \\
1 & 4 \\
\end{array}\right],
b = \begin{bmatrix}{}0\\8\\8\\20\end{bmatrix}
$$

We are now ready to set up $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$, and solve
for $\hat{x}$.

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
0 & 1 & 3 & 4 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
1 & 3 \\
1 & 4 \\
\end{array}\right] =
\left[\begin{array}{cc}
4 & 8 \\
8 & 26 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
0 & 1 & 3 & 4 \\
\end{array}\right]
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} =
\begin{bmatrix}{}36\\112\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
4 & 8 \\
8 & 26 \\
\end{array}\right]
\begin{bmatrix}{}\hat{x}_1\\\hat{x}_2\end{bmatrix} =
\begin{bmatrix}{}36\\112\end{bmatrix} =
A^{\mathbf{T}}b
$$

$$
4\hat{x}_1 + 8\hat{x}_2 = 36 \\
8\hat{x}_1 + 26\hat{x}_2 = 112 \\
$$

Let's just use a little elimination here:

$$
\left[\begin{array}{cc|c}
4 & 8 & 36 \\
8 & 26 & 112 \\
\end{array}\right] \to
\left[\begin{array}{cc|c}
4 & 8 & 36 \\
0 & 10 & 40 \\
\end{array}\right]
$$

So:

$$ 10\hat{x}_2 = 40 \to \hat{x}_2 = 4 $$

Then:

$$ 4\hat{x}_1 + 8\hat{x}_2 = 36 \to 4\hat{x}_1 + 8(4) = 36 \to 4\hat{x}_1 = 4 \to \hat{x}_1 = 1 $$

Thus:

$$ \boxed{\hat{x} = \begin{bmatrix}{}1\\4\end{bmatrix}} $$

And the best line fit is $b = 1 + 4t$.

_For the best straight line in Figure 4.9a, find its four heights $p_i$ and four
errors $e_i$:_

Recall that $p = A\hat{x}$. So;

$$ p = A\hat{x} =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
1 & 3 \\
1 & 4 \\
\end{array}\right]
\begin{bmatrix}{}1\\4\end{bmatrix} =
\begin{bmatrix}{}1\\5\\13\\17\end{bmatrix}
$$

Thus the four heights are $p_1 = 1, p_2 = 5, p_3 = 13, p_4 = 17$.

Recall also that $e = b - p$, so:

$$ e = b - p =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} -
\begin{bmatrix}{}1\\5\\13\\17\end{bmatrix} =
\begin{bmatrix}{}-1\\3\\-5\\3\end{bmatrix}
$$

Thus the four errors are $e_1 = -1, e_2 = 3, e_3 = -5, e_4 = 3$.

_What is the minimum value $E = e_1^2 + e_2^2 + e_3^2 + e_4^2$?:_

Simply calculate $E$:

$$ E = \|e\|^2 = (-1)^2 + (3)^2 + (-5)^2 + (3)^2 = 1 + 9 + 25 + 9 = 44 $$

2. (Line $C + Dt$ does go through $p$'s) With $b = 0, 8, 8, 20$ at times
   $t = 0, 1, 3, 4$, write down the four equations $Ax = b$ (unsolvable). Change
   the measurements to $p = 1, 5, 13, 17$ and find an exact solution to
   $A\hat{x} = p$.

_Solution:_

Here, we simply write out our vector for $x$, which is
$\begin{bmatrix}{}C\\D\end{bmatrix}$, set $Ax = b$, and note that it is
unsolvable:

$$ Ax =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
1 & 3 \\
1 & 4 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} = b
$$

The most obvious reason this is unsolvable is the fact that both $C + D = 8$ and
$C + 3D = 8$.

Since $p$ is the projection of $b$ onto $C(A)$, $A\hat{x} = p$ has an exact
solution.

$$ p = \begin{bmatrix}{}1\\5\\13\\17\end{bmatrix} $$

We can then replace $b$ with $p$ and solve for the best possible $x$, $\hat{x}$
(as we did in problem 1), and get
$\hat{x} = \begin{bmatrix}{}1\\4\end{bmatrix}$.

3. Check that $e = b - p = (-1, 3, -5, 3)$ is perpendicular to both columns of
   the same matrix $A$. What is the shortest distance $\|e\|$ from $b$ to the
   column space of $A$?

_Solution:_

_Check that $e = b - p = (-1, 3, -5, 3)$ is perpendicular to both columns of the
same matrix $A$:_

$$ e_{\mathbf{T}}A_{i1} =
\left[\begin{array}{rrrr}
-1 & 3 & -5 & 3 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} =
(-1)(1) + (3)(1) + (-5)(1) + (3)(1) = -1 + 3 - 5 + 3 = 0
$$

$$ e_{\mathbf{T}}A_{i2} =
\left[\begin{array}{rrrr}
-1 & 3 & -5 & 3 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix} =
(-1)(0) + (3)(1) + (-5)(3) + (3)(4) = 0 + 3 - 15 + 12 = 0
$$

Thus $e \perp A_{i1}$ and $e \perp A_{i2}$.

_What is the shortest distance $\|e\|$ from $b$ to the column space of $A$?:_

As calculated in problem 1 for $E$, we determined that $E = \|e\|^2 = 44$. Thus
the shortest distance $\|e\|$ is:

$$ \|e\| = \sqrt{44} $$

This follows from the definition of euclidean norm distances and by extension,
the Pythagorean theorem.

4. (By calculus) Write down $E = \|Ax - b\|^2$ as a sum of four squares - the
   last one is $(C + 4D - 20)^2$. Find the derivative equations
   $\dfrac{\partial E}{\partial C} = 0$ and
   $\dfrac{\partial E}{\partial D} = 0$. Divide by $2$ to obtain the normal
   equations $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

_Solution:_

_(By calculus) Write down $E = \|Ax - b\|^2$ as a sum of four squares - the last
one is $(C + 4D - 20)^2$:_

$$ E = (C + 0D - 0)^2 + (C + 1D - 8)^2 + (C + 3D - 8)^2 + (C + 4D - 20)^2 $$

_Find the derivative equations $\dfrac{\partial E}{\partial C} = 0$ and
$\dfrac{\partial E}{\partial D} = 0$:_

$$ \frac{\partial E}{\partial C} = 2C + 2(C + D - 8) + 2(C + 3D - 8) + 2(C + 4D - 20) = 0 $$

$$ \frac{\partial E}{\partial D} = 0 + [1 \cdot 2(C + D - 8)] + [3 \cdot 2(C + 3D - 8)] + [4 \cdot 2(C + 4D - 20)] = 0 $$

Note that partial derivatives are generally covered in calculus 3 (which I
haven't taken). That said, note that this is simply applying the chain rule and
understanding that partial derivatives treat the "non-given" variables as
constants instead of variables, and we only solve for the variable that is
"given".

_Divide by $2$ to obtain the normal equations
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:_

$$ \frac{\partial E}{\partial C} \cdot \frac{1}{2} = C + (C + D - 8) + (C + 3D - 8) + (C + 4D - 20) = 4C + 8D - 36 = 0 $$

$$ \frac{\partial E}{\partial D} \cdot \frac{1}{2} = (C + D - 8) + 3(C + 3D - 8) + 4(C + 4D - 20) = 8C + 26D - 112 = 0 $$

First, notice that this evaluates to:

$$
4C + 8D = 36 \\
8C + 26D = 112 \\
$$

Notice that we can line these equations up to form:

$$
\left[\begin{array}{cc}
4 & 8 \\
8 & 26 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}36\\112\end{bmatrix}
$$

And this is what we used to solve for $\hat{x}$ in problem 1. In other words
this is the final form of solving $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

5. Find the height $C$ of the best _horizontal line_ to fit $b = (0, 8, 8, 20)$.
   An exact fit would solve the unsolvable equations
   $C = 0, C = 8, C = 8, C = 20$. Find the $4$ by $1$ matrix $A$ in these
   equations and solve $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$. Draw the
   horizontal line at height $\hat{x} = C$ and the four errors in $e$.

_Solution:_

_Find the height $C$ of the best horizontal line to fit $b = (0, 8, 8, 20)$:_

To find the height of the best horizontal line, simply remove the second vector
$t$ from $A$, and only consider the first column of all $1$'s. This is us solely
considering the vector $C$:

$$ A =
\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix}
$$

Then, solve for $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} = [4]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} = [36]
$$

$$ A^{\mathbf{T}}A\hat{x} =
[4][C] = [36] \to \boxed{C = 9}
$$

_Find the $4$ by $1$ matrix $A$ in these equations and solve
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:_

We just did that, we found $C$ above.

_Draw the horizontal line at height $\hat{x} = C$ and the four errors in $e$:_

Notice that this changes $e$:

$$ e = b - p =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} - \begin{bmatrix}{}9\\9\\9\\9\end{bmatrix} =
\begin{bmatrix}{}-9\\-1\\-1\\11\end{bmatrix}
$$

Notice that when multiplied by each column of $A$, we still get $0$, and thus
$e \perp A_{ij}$.

6. Project $b = (0, 8, 8, 20)$ onto the line through $a = (1, 1, 1, 1)$. Find
   $\hat{x} = \dfrac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}$ and the projection
   $p = \hat{x}a$. Check that $e = b - p$ is perpendicular to $a$, and find the
   shortest distance $\|e\|$ from $b$ to the line through $a$.

_Solution:_

_Project $b = (0, 8, 8, 20)$ onto the line through $a = (1, 1, 1, 1)$. Find
$\hat{x} = \dfrac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}$ and the projection
$p = \hat{x}a$:_

Recall that to calculate a projection, it is sufficient to calculate $\hat{x}$:

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ a^{\mathbf{T}}b =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} = [36]
$$

$$ a^{\mathbf{T}}a =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} = [4]
$$

$$ \hat{x} = \frac{36}{4} = 9 $$

And thus the projection, which is $p = \hat{x}a$ is:

$$ p = \hat{x}a =
9 \cdot \begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} = \begin{bmatrix}{}9\\9\\9\\9\end{bmatrix}
$$

_Check that $e = b - p$ is perpendicular to $a$:_

$$ e = b - p =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} - \begin{bmatrix}{}9\\9\\9\\9\end{bmatrix} =
\begin{bmatrix}{}-9\\-1\\-1\\11\end{bmatrix}
$$

$$ e^{\mathbf{T}} \cdot a =
\left[\begin{array}{rrrr}
-9 & -1 & -1 & 11 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\\1\end{bmatrix} = 0
$$

And thus $e \perp a$.

_And find the shortest distance $\|e\|$ from $b$ to the line through $a$:_

$$ E = \|e\|^2 = (-9)^2 + (-1)^2 + (-1)^2 + (11)^2 = 204 $$

$$ \|e\| = \sqrt{204} $$

7. Find the closest line $b = Dt$, _through the origin_, to the same four
   points. An exact fit would solve
   $D \cdot 0 = 0, D \cdot 1 = 8, D \cdot 3 = 8, D \cdot 4 = 20$. Find the $4$
   by $1$ matrix and solve $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$. Redraw
   Figure 4.9a showing the best line $b = Dt$ and the $e$'s.

_Solution:_

_Find the closest line $b = Dt$, through the origin, to the same four points. An
exact fit would solve
$D \cdot 0 = 0, D \cdot 1 = 8, D \cdot 3 = 8, D \cdot 4 = 20$:_

This is similar to problem 5, where we found the best _horizontal line_ to fit
$b$. Instead here, we are tasked with finding the closest line $b = Dt$, so
simply make $A$ the sole column of $t$.

$$ A =
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix}
$$

Then solve $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cccc}
0 & 1 & 3 & 4 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix} = 26
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{cccc}
0 & 1 & 3 & 4 \\
\end{array}\right]
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} = 112
$$

_Find the $4$ by $1$ matrix and solve
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$:_

$$ 26\hat{x} = 112 \to \hat{x} = \frac{56}{13} = D $$

Note that $D$ is a scalar, to find the vector $p$: $p = D \cdot a$:

$$ p = D \cdot t =
\frac{56}{13}
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix} =
\begin{bmatrix}{}0\\\frac{56}{13}\\\frac{168}{13}\\\frac{224}{13}\end{bmatrix}
$$

_Redraw Figure 4.9a showing the best line $b = Dt$ and the $e$'s:_

$$ e = b - p =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} -
\begin{bmatrix}{}0\\\frac{56}{13}\\\frac{168}{13}\\\frac{224}{13}\end{bmatrix} =
\begin{bmatrix}{}0\\\frac{48}{13}\\-\frac{64}{13}\\\frac{36}{13}\end{bmatrix}
$$

Drawing done by hand.

8. Project $b = (0, 8, 8, 20)$ onto the line through $a = (0, 1, 3, 4)$. Find
   $\hat{x} = D$ and $p = \hat{x}a$. The best $C$ in Problems 5-6 and the best
   $D$ i Problems 7-8 do _not_ agree with the best $(C, D)$ in Problems 1-4.
   That is because $(1, 1, 1, 1)$ and $(0, 1, 3, 4)$ are ____ perpendicular.

_Project $b = (0, 8, 8, 20)$ onto the line through $a = (0, 1, 3, 4)$. Find
$\hat{x} = D$ and $p = \hat{x}a$:_

$$ \hat{x} = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a} $$

$$ a^{\mathbf{T}}b =
\left[\begin{array}{cccc}
0 & 1 & 3 & 4 \\
\end{array}\right]
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} = 112
$$

$$ a^{\mathbf{T}}a =
\left[\begin{array}{cccc}
0 & 1 & 3 & 4 \\
\end{array}\right]
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix} = 26
$$

$$ \hat{x} = \frac{112}{26} = \frac{56}{13}  $$

Recall from problem 8, that this is $\hat{x} = D$.

Recall that we solved $p = \hat{x}a$ in problem 8 as well as:

$$ p = D \cdot t =
\frac{56}{13}
\begin{bmatrix}{}0\\1\\3\\4\end{bmatrix} =
\begin{bmatrix}{}0\\\frac{56}{13}\\\frac{168}{13}\\\frac{224}{13}\end{bmatrix}
$$

_The best $C$ in Problems 5-6 and the best $D$ in Problems 7-8 do _not_ agree
with the best $(C, D)$ in Problems 1-4. That is because $(1, 1, 1, 1)$ and
$(0, 1, 3, 4)$ are (?) perpendicular:_

not

9. For the closest parabola $b = C + Dt + Et^2$ to the same four points, write
   down the unsolvable equations $Ax = b$ in three unknowns $x = (C, D, E)$. Set
   up the three normal equations $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$
   (solution not required). In Figure 4.9a you are now fitting a parabola to $4$
   points - what is happening in Figure 4.9b?

_Solution:_

_For the closest parabola $b = C + Dt + Et^2$ to the same four points, write
down the unsolvable equations $Ax = b$ in three unknowns $x = (C, D, E)$:_

Recall that by least squares, since we have three terms, we need a third column
for $t^2$ in $A$:

$$ Ax = b \to
\left[\begin{array}{cc}
1 & 0 & 0 \\
1 & 1 & 1 \\
1 & 3 & 9 \\
1 & 4 & 16 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\\E\end{bmatrix} =
\begin{bmatrix}{}0\\8\\8\\20\end{bmatrix}
$$

_Set up the three normal equations $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$
(solution not required):_

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
0 & 1 & 3 & 4 \\
0 & 1 & 9 & 16 \\
\end{array}\right]
\left[\begin{array}{ccc}
1 & 0 & 0 \\
1 & 1 & 1 \\
1 & 3 & 9 \\
1 & 4 & 16 \\
\end{array}\right] =
\left[\begin{array}{ccc}
4 & 8 & 26 \\
8 & 26 & 92 \\
26 & 92 & 338 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b = \left[\begin{array}{cccc} 1 & 1 & 1 & 1 \\ 0 & 1 & 3 & 4 \\
0 & 1 & 9 & 16 \\ \end{array}\right] \begin{bmatrix}{}0\\8\\8\\20\end{bmatrix} =
\begin{bmatrix}{}36\\112\\400\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{ccc}
4 & 8 & 26 \\
8 & 26 & 92 \\
26 & 92 & 338 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\\E\end{bmatrix} =
\begin{bmatrix}{}36\\112\\400\end{bmatrix} = A^{\mathbf{T}}b
$$

_In Figure 4.9a you are now fitting a parabola to $4$ points - what is happening
in Figure 4.9b?:_

In the original 4.9b, the closest line $C + Dt$ matched $Ca_1 + Da_2$ in $\R^4$.
Here, we are fitting the closest parabola $C + Dt + Et^2$ matched
$Ca_1 + Da_2 + Ea_3$ in $\R^4$. With four points and three unknowns, the
parabola still resides within $\R^4$.

10. For the closest cubic $b = C + Dt + Et^2 + Ft^3$ to the same four points,
    write down the four equations $Ax = b$. Solve them by elimination. In Figure
    4.9a this cubic now goes exactly through the points. What are $p$ and $e$?

_Solution:_

_For the closest cubic $b = C + Dt + Et^2 + Ft^3$ to the same four points, write
down the four equations $Ax = b$. Solve them by elimination:_

$$ Ax = b \to
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
1 & 1 & 1 & 1 \\
1 & 3 & 9 & 27 \\
1 & 4 & 16 & 64 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\\E\\F\end{bmatrix} = \begin{bmatrix}{}0\\8\\8\\20\end{bmatrix}
$$

Solving by elimination:

$$
\left[\begin{array}{cccc|c}
1 & 0 & 0 & 0 & 0 \\
1 & 1 & 1 & 1 & 8 \\
1 & 3 & 9 & 27 & 8 \\
1 & 4 & 16 & 64 & 20 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 1 & 1 & 8 \\
0 & 3 & 9 & 27 & 8 \\
0 & 4 & 16 & 64 & 20 \\
\end{array}\right] \to
\left[\begin{array}{cccc|c}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 1 & 1 & 8 \\
0 & 3 & 9 & 27 & 8 \\
0 & 4 & 16 & 64 & 20 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{cccc|r}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 1 & 1 & 8 \\
0 & 0 & 6 & 24 & -16 \\
0 & 4 & 16 & 64 & 20 \\
\end{array}\right] \to
\left[\begin{array}{cccc|r}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 1 & 1 & 8 \\
0 & 0 & 6 & 24 & -16 \\
0 & 0 & 0 & 12 & 20 \\
\end{array}\right] = U
$$

Thus we are left with:

$$
1C + 0D + 0E + 0F = 0 \\
0C + 1D + 1E + 1F = 8 \\
0C + 0D + 6E + 24F = -16 \\
0C + 0D + 0E + 12F = 20 \\
$$

Solving:

$$ 12F = 20 \Rightarrow F = \frac{5}{3} $$

$$ 6E + 24F = -16 \Rightarrow 6E + 24\left(\frac{5}{3}\right) = -16 \Rightarrow 6E + 40 = -16 \Rightarrow 6E = -56 \Rightarrow E = -\frac{28}{3} $$

$$ 1D + 1E + 1F = 8 \Rightarrow D + \left(-\frac{28}{3}\right) + \left(\frac{5}{3}\right) = 8 \Rightarrow D - \frac{23}{3} = 8 \Rightarrow D = \frac{47}{3} $$

$$ 1C + 0D + 0E + 0F = 0 \Rightarrow C = 0 $$

Thus:

$$ x = \begin{bmatrix}{}0\\\frac{47}{3}\\-\frac{28}{3}\\\frac{5}{3}\end{bmatrix} $$

_In Figure 4.9a this cubic now goes exactly through the points. What are $p$ and
$e$?:_

Since $b \in C(A)$, it follows that $p = b$ and $e = \mathbf{0}$.

11. The average of the four times is
    $\hat{t} = \dfrac{1}{4}(0 + 1 + 3 + 4) = 2$. The average of the four $b$'s
    is $\hat{b} = \dfrac{1}{4}(0 + 8 + 8 + 20) = 9$.

a. Verify that the best line goes through the center point
$(\hat{t}, \hat{b}) = (2, 9)$.

_Solution:_

Recall that our best line fit from Problem 1 was determined to be $b = 1 + 4t$.

The center point $(\hat{t}, \hat{b}) = (2, 9)$ indeed satisfies this best line
equation:

$$ b = 1 + 4t $$

$$ 9 = 1 + 4(2) $$

$$ 9 = 9 $$

b. Explain why $C + D\hat{t} = \hat{b}$ comes from the first equation in
$A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

_Solution:_

Consider that the first equation can be interpreted as:

$$ Cm + D\sum{t_i} = \sum_{b_i} $$

Where $m$ is simply the number of points, then if we divide by $m$ (getting the
average of both $b$ and $t$, yielding $\hat{b}$ and $\hat{t}$ respectively),
this yields:

$$ C + D\hat{t} = \hat{b} $$

This shows that the best line goes through $\hat{b}$ at time $\hat{t}$.

**Questions 12-16 introduce basic ideas of statistics - the foundation for least
squares.**

12. (Recommended) This problem projects $b = (b_1, \dots, b_m)$ onto the line
    through $a = (1, \dots, 1)$. We solve $m$ equations $ax = b$ in $1$ unknown
    (by least squares).

a. Solve $a^{\mathbf{T}}a\hat{x} = a^{\mathbf{T}}b$ to show that $\hat{x}$ is
the _mean_ (the average) of the $b$'s.

_Solution:_

$$ a^{\mathbf{T}}a\hat{x} = a^{\mathbf{T}}b $$

Consider that since $a = (1, \dots, 1)$, this means that $a^{\mathbf{T}}a = m$,
where $m$ is simply the number of coordinates in $a$ (that importantly also
corresponds to the number of coordinates in $b$).

Additionally, $a^{\mathbf{T}}b = \sum_{i = 1}^{m}{b_i}$ by similar reasoning
(that $a$ simply dot products all the $b$'s by $1$'s).

Thus we have:

$$ m\hat{x} = \sum_{i = 1}^{m}{b_i} $$

By algebra then:

$$ \hat{x} = \frac{1}{m}\sum_{i = 1}^{m}{b_i} $$

This is the average/mean of the $b$'s (the sum of all $b$'s divided by the
number of coordinates in all of $b$).

b. Find $e = b - a\hat{x}$ and the _variance_ $\|e\|^2$ and the _standard
deviation_ $\|e\|$.

_Solution:_

$$ e = b - a\hat{x} $$

Since $a\hat{x}$ is just $(1, \dots, 1)$ multiplied by the mean of $b$, this is
just the mean of $b$. This means that the Euclidean norm of $e$ can be expressed
as:

$$ \|e\|^2 = \sum_{i = 1}^{m}{\left(b_i - \frac{1}{m}\sum_{i = 1}^{m}{b_i}\right)^2} $$

And this means that the variance $\|e\|$, denoted $\sigma$, can be expressed as
the square root of this:

$$ \sigma = \|e\| = \sqrt{\sum_{i = 1}^{m}{\left(b_i - \frac{1}{m}\sum_{i = 1}^{m}{b_i}\right)^2}} $$

c. The horizontal line $\hat{b} = 3$ is closest to $b = (1, 2, 6)$. Check that
$p = (3, 3, 3)$ is perpendicular to $e$ and find the $3$ by $3$ projection
matrix $P$.

_Solution:_

$$ e = b - p $$

$$ e = \begin{bmatrix}{}1\\2\\6\end{bmatrix} - \begin{bmatrix}{}3\\3\\3\end{bmatrix} =
\begin{bmatrix}{}-2\\-1\\3\end{bmatrix}
$$

$$ e^{\mathbf{t}} \cdot p =
\left[\begin{array}{rrr}
-2 & -1 & 3 \\
\end{array}\right]
\begin{bmatrix}{}3\\3\\3\end{bmatrix} =
(-2)(3) + (-1)(3) + (3)(3) = 0 \to e \perp p
$$

Recall that $P = \dfrac{aa^{\mathbf{T}}}{a^{\mathbf{T}}a}$.

Now, we know that since $b$ has $3$ components, then $a$ must also have three
components, and by the problem statement we know that every component of $a$ is
$1$, so:

$$ aa^{\mathbf{T}} =
\begin{bmatrix}{}1\\1\\1\end{bmatrix}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

$$ a^{\mathbf{T}}a =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = 3
$$

Thus we can express $P$ as:

$$ P =
\frac{1}{3}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

13. First assumption behind least squares: $Ax = b$ - (_noise $e$ with mean
    zero_). Multiply the error vectors $e = b - Ax$ by
    $(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ to get $\hat{x} - x$ on the right.
    The estimation errors $\hat{x} - x$ also average zero. The estimate
    $\hat{x}$ is _unbiased_.

_Solution:_

$$ e = b - p $$

$$ e = b - A\hat{x} $$

$$ (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}e = (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}(b - A\hat{x}) $$

Notice that $e = b - Ax \to b = Ax + e$, thus, by substitution:

$$ = (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}(Ax + e - A\hat{x}) $$

Distribution is messy, but:

$$ = (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}(Ax) + (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}e - (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}A\hat{x} $$

$$ = Ix + Ie - I\hat{x} $$

$$ = x + e - \hat{x} $$

Now, so far we have:

$$ (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}e = x + e - \hat{x}$$

Evaluating:

$$ (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}e - e = x - \hat{x} $$

14. Second assumption behind least squares: The $m$ errors $e_i$ are independent
    with variance $\sigma^2$, so the average of $(b - Ax)(b - Ax)^{\mathbf{T}}$
    is $\sigma^2I$. Multiply on the left by
    $(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ and on the right by
    $A(A^{\mathbf{T}}A)^{-1}$ to show that the average matrix
    $(\hat{x} - x)(\hat{x} - x)^{\mathbf{T}}$ is
    $\sigma^2(A^{\mathbf{T}}A)^{-1}$. This is the _covariance matrix $W$_ in
    Section 10.2.

_Solution:_

This one I just take from Strang, it's not intuitive:

The matrix $(\hat{x} - x)(\hat{x} - x)^{\mathbf{T}}$ is
$(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}(b - Ax)(b - Ax)^{\mathbf{T}}A(A^{\mathbf{T}}A)^{-1}$.
When the average of $(b - Ax)(b - Ax)^{\mathbf{T}}$ is $\sigma^2I$, the average
of $(\hat{x} - x)(\hat{x} - x)^{\mathbf{T}}$ will be the _output covariance
matrix_ $(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}\sigma^2AA(A^{\mathbf{T}}A)^{-1}$
which simplifies to $\sigma^2(A^{\mathbf{T}}A)^{-1}$. That gives the average of
the squared output errors $\hat{x} - x$.

15. A doctor takes $4$ readings of your heart rate. The best solution to
    $x = b_1, \dots, x = b_4$ is the average $\hat{x}$ of $b_1, \dots, b_4$. The
    matrix $A$ is a column of $1$'s. Problem 14 gives the expected error
    $(\hat{x} - x)^2$ as $\sigma^2(A^{\mathbf{T}}A)^{-1} =$ ____. _By averaging,
    the variance drops from $\sigma^2$ to $\dfrac{\sigma^2}{4}$_ .

_Solution:_

Strang gives us the solution:

$$ \sigma^2(A^{\mathbf{T}}A)^{-1} = \frac{\sigma^2}{4} $$

When the columns of $A$'s are all $1$' and there are $4$ components.

In layman's terms, since the doctor took 4 measurements, the variance (the
variance in accuracy from the true heart rate) is divided by $4$. In short, the
more measurements one takes, the closer to the accurate heart rate we get.

16. If you know the average $\hat{x}_9$ of $9$ numbers $b_1, \dots, b_9$, how
    can you quickly find the average $\hat{x}_{10}$ with one more number
    $b_{10}$? The idea of _recursive_ least squares is to avoid adding $10$
    numbers. What number multiplies $\hat{x}_9$ in computing $\hat{x}_{10}$?

$$ \hat{x}_{10} = \frac{1}{10}b_{10} + \text{\_\_\_\_}\hat{x}_9 = \frac{1}{10}(b_1 + \cdots + b_{10}) $$

as in Worked Example 4.2 C.

_Solution:_

We are working in averages, if we know that we have $10$ components/data points,
and we already know the average of the previous $9$ data points, then it stands
to reason that we can simply take the average of the single data point and sum
it with the previous. This can be expressed as:

$$ \frac{1}{10}b_{10} + \frac{9}{10}\hat{x}_9 = \frac{1}{10}(b_1 + \cdots + b_{10}) $$

**Questions 17-24 give more practice with $\hat{x}$ and $p$ and $e$.**

17. Write down three equations for the line $b = C + Dt$ to go through $b = 7$
    at $t = -1$, $b = 7$ at $t = 1$, and $b = 21$ at $t = 2$. Find the least
    squares solution $\hat{x} = (C, D)$ and draw the closest line.

_Solution:_

$$
C - D = 7 \\
C + D = 7 \\
C + 2D = 21 \\
$$

$$
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}7\\7\\21\end{bmatrix}
$$

Notice that this is unsolvable (3 independent points, 2 unknowns).

Thus we find $\hat{x}$:

$$ A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b $$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}7\\7\\21\end{bmatrix} =
\begin{bmatrix}{}35\\42\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}35\\42\end{bmatrix} = A^{\mathbf{T}}b
$$

And now we solve by elimination:

$$
\left[\begin{array}{cc|c}
3 & 2 & 35 \\
2 & 6 & 42 \\
\end{array}\right] \to
\left[\begin{array}{cc|c}
3 & 2 & 35 \\
0 & \frac{14}{3} & \frac{56}{3} \\
\end{array}\right] \to
$$

$$ \frac{14}{3}D = \frac{56}{3} \Rightarrow D = 4 $$

$$ 3C + 2D = 35 \Rightarrow 3C + 2(4) = 35 \Rightarrow 3C + 8 = 35 \Rightarrow 3C = 27 \Rightarrow C = 9 $$

Thus $\hat{x} = \begin{bmatrix}{}9\\4\end{bmatrix}$.

18. Find the projection $p = A\hat{x}$ in Problem 17. This gives the three
    heights of the closest line. Show that the error vector is $e = (2, -6, 4)$.
    Why is $Pe = \mathbf{0}$?

_Solution:_

$$ p = A\hat{x} =
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}9\\4\end{bmatrix} =
\begin{bmatrix}{}5\\13\\17\end{bmatrix}
$$

$$ e = b - p $$

$$ e =
\begin{bmatrix}{}7\\7\\21\end{bmatrix} -
\begin{bmatrix}{}5\\13\\17\end{bmatrix} =
\begin{bmatrix}{}2\\-6\\4\end{bmatrix}
$$

Consider:

$$ Pe = P(b - p) = Pb - Pp = p - p = \mathbf{0} $$

Briefly, the reason $Pp = p$ is because $p \in C(A)$, so projecting it again
does nothing.

19. Suppose the measurements at $t = -1, 1, 2$ are the errors $2, -6, 4$ in
    Problem 18. Compute $\hat{x}$ and the closest line to these new
    measurements. Explain the answer: $b = (2, -6, 4)$ is perpendicular to ____
    so the projection is $p = \mathbf{0}$.

Here only $b$ changes from Problems 17/18, so:

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}2\\-6\\4\end{bmatrix} =
\begin{bmatrix}{}0\\0\end{bmatrix}
$$

Solving for $\hat{x}$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}0\\0\end{bmatrix} = A^{\mathbf{T}}b
$$

Solving by elimination:

$$
\left[\begin{array}{cc|c}
3 & 2 & 0 \\
2 & 6 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cc|c}
3 & 2 & 0 \\
0 & \frac{14}{3} & 0 \\
\end{array}\right] \to
$$

So:

$$ \frac{14}{3}D = 0 \Rightarrow D = 0 $$

$$ 3C + 2D = 0 \Rightarrow 3C + 2(0) = 0 \Rightarrow 3C = 0 \Rightarrow C = 0 $$

So our new $\hat{x}$ is:

$$ \hat{x} = \begin{bmatrix}{}0\\0\end{bmatrix} $$

The closest line to these new measurements is $p$:

$$ p = A\hat{x} =
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}0\\0\end{bmatrix} =
\begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

Since $b = e$, it follows that $b \in C(A)$, thus $b \perp p$.

20. Suppose the measurements at $t = -1, 1, 2$ are $b = (5, 13, 17)$. Compute
    $\hat{x}$ and the closest line and $e$. The error is $e = \mathbf{0}$
    because this $b$ is ____.

_Solution:_

$$ A =
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{rrr}
1 & 1 & 1 \\
-1 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}5\\13\\17\end{bmatrix} =
\begin{bmatrix}{}35\\42\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{cc}
3 & 2 \\
2 & 6 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}35\\42\end{bmatrix} = A^{\mathbf{T}}b
$$

$$
\left[\begin{array}{cc|c}
3 & 2 & 35 \\
2 & 6 & 42 \\
\end{array}\right] \to
\left[\begin{array}{cc|c}
3 & 2 & 35 \\
0 & \frac{14}{3} & \frac{56}{3} \\
\end{array}\right]
$$

$$ \frac{14}{3}D = \frac{56}{3} \Rightarrow D = 4 $$

$$ 3C + 2D = 35 \Rightarrow 3C + 2(4) = 35 \Rightarrow 3C + 8 = 35 \Rightarrow 3C = 27 \Rightarrow C = 9 $$

$$ \hat{x} = \begin{bmatrix}{}9\\4\end{bmatrix} $$

$$ p = A\hat{x} =
\left[\begin{array}{rr}
1 & -1 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}9\\4\end{bmatrix} =
\begin{bmatrix}{}5\\13\\17\end{bmatrix} = b
$$

$$ e = b - p =
\begin{bmatrix}{}5\\13\\17\end{bmatrix} - \begin{bmatrix}{}5\\13\\17\end{bmatrix} = \mathbf{0}
$$

The error is $e = \mathbf{0}$ because this $b$ is $p$. In other words
$b \in C(A)$.

21. Which of the four subspaces contains the error vector $e$? Which contains
    $p$? Which contains $\hat{x}$? What is the nullspace of $A$?

_Solution:_

_Which of the four subspaces contains the error vector $e$?:_

$$ N(A^{\mathbf{T}}) $$

_Which contains $p$?:_

$C(A)$

_Which contains $\hat{x}$?:_

$C(A^{\mathbf{T}})$

_What is the nullspace of $A$?:_

$$ N(A) = \{\mathbf{0}\} $$

22. Find the best line $C + Dt$ to fit $b = 4, 2, -1, 0, 0$ at times
    $t = -2, -1, 0, 1, 2$.

_Solution:_

Find $\hat{x}$ and apply it to $b = C + Dt$.

$$ A =
\left[\begin{array}{rr}
1 & -2 \\
1 & -1 \\
1 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrrrr}
1 & 1 & 1 & 1 & 1 \\
-2 & -1 & 0 & 1 & 2 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & -2 \\
1 & -1 \\
1 & 0 \\
1 & 1 \\
1 & 2 \\
\end{array}\right] =
\left[\begin{array}{rr}
5 & 0 \\
0 & 10 \\
\end{array}\right]
$$

$$ A^{\mathbf{T}}b =
\left[\begin{array}{rrrrr}
1 & 1 & 1 & 1 & 1 \\
-2 & -1 & 0 & 1 & 2 \\
\end{array}\right]
\begin{bmatrix}{}4\\2\\-1\\0\\0\end{bmatrix} =
\begin{bmatrix}{}5\\-10\end{bmatrix}
$$

$$ A^{\mathbf{T}}A\hat{x} =
\left[\begin{array}{rr}
5 & 0 \\
0 & 10 \\
\end{array}\right]
\begin{bmatrix}{}C\\D\end{bmatrix} =
\begin{bmatrix}{}5\\-10\end{bmatrix} = A^{\mathbf{T}}b
$$

$$
\left[\begin{array}{rr|r}
5 & 0 & 5 \\
0 & 10 & -10 \\
\end{array}\right]
$$

$$ 10D = -10 \Rightarrow D = -1 $$

$$ 5C + 0D = 5 \Rightarrow 5C = 5 \Rightarrow C = 1 $$

$$ \hat{x} = \begin{bmatrix}{}1\\-1\end{bmatrix} $$

So our best answer is $b = 1 - t$.

23. Is the error vector $e$ orthogonal to $b$ or $p$ or $e$ or $\hat{x}$? Show
    that $\|e\|^2$ equals $e^{\mathbf{T}}b$ which equals
    $b^{\mathbf{T}}b - p^{\mathbf{T}}b$. This is the smallest total error $E$.

_Solution:_

_Is the error vector $e$ orthogonal to $b$ or $p$ or $e$ or $\hat{x}$?:_

$e$ is orthogonal to $p \in R^m$.

_Show that $\|e\|^2$ equals $e^{\mathbf{T}}b$ which equals
$b^{\mathbf{T}}b - p^{\mathbf{T}}b$:_

Then
$\|e\|^2 = e^{\mathbf{T}}(b - p) = e^{\mathbf{T}}b = b^{\mathbf{T}}b - b^{\mathbf{T}}p$.

24. The partial derivatives of $\|Ax\|^2$ with respect to $x_1, \dots, x_n$ fill
    the vector $2A^{\mathbf{T}}Ax$. The derivatives of $2b^{\mathbf{T}}Ax$ fill
    the vector $2A^{\mathbf{T}}b$. So the derivatives of $\|Ax - b\|^2$ are zero
    when ____.

Omitted.

---

Page 253

## Problem Set 4.4

**Problems 1-12 are about orthogonal vectors and orthogonal matrices.**

1. Are these pairs of vectors orthonormal or only orthogonal or only
   independent?

a. $\begin{bmatrix}{}1\\0\end{bmatrix}$ and
$\begin{bmatrix}{}-1\\1\end{bmatrix}$

b. $\begin{bmatrix}{}.6\\.8\end{bmatrix}$ and
$\begin{bmatrix}{}.4\\-.3\end{bmatrix}$

c. $\begin{bmatrix}{}\cos\theta\\\sin\theta\end{bmatrix}$ and
$\begin{bmatrix}{}-\sin\theta\\\cos\theta\end{bmatrix}$

Change the second vector when necessary to produce orthonormal vectors.

_Solution:_

a. $\begin{bmatrix}{}1\\0\end{bmatrix}$ and
$\begin{bmatrix}{}-1\\1\end{bmatrix}$

Not orthogonal, therefore not orthonormal, but yes independent.

New second vector to produce orthonormal vectors:

$$ \begin{bmatrix}{}0\\1\end{bmatrix} $$

b. $\begin{bmatrix}{}.6\\.8\end{bmatrix}$ and
$\begin{bmatrix}{}.4\\-.3\end{bmatrix}$

Orthogonal (since $(0.6)(0.4) + (.8)(-.3) = 0$). Not orthonormal, since the
second vector's euclidean norm is $\sqrt{.4^2 + (-.3)^2} = 0.5 \neq 1$. They are
independent.

New second vector to produce orthonomral vectors:

$$ \begin{bmatrix}{}.8\\-.6\end{bmatrix} $$

c. $\begin{bmatrix}{}\cos\theta\\\sin\theta\end{bmatrix}$ and
$\begin{bmatrix}{}-\sin\theta\\\cos\theta\end{bmatrix}$

Orthogonal since $(\cos\theta(-\sin\theta)) + \sin\theta\cos\theta = 0$.
Orthonormal since $\sqrt{\cos^2\theta + \sin^2\theta} = 1$. Independent.

Additionally we have
$\sqrt{(-\sin\theta)^2 + \cos^2\theta} = \sqrt{\sin^2\theta + \cos^2\theta} = 1$.

Both of these follow from the Pythagorean identity for cosine/sine:
$\cos^2\theta + \sin^2\theta = 1$.

2. The vectors $(2, 2, -1)$ and $(-1, 2, 2)$ are orthogonal. Divide them by
   their lengths to find orthonormal vectors $q_1$ and $q_2$. Put those into the
   columns of $Q$ and multiply $Q^{\mathbf{T}}Q$ and $QQ^{\mathbf{T}}$.

_Solution:_

_The vectors $(2, 2, -1)$ and $(-1, 2, 2)$ are orthogonal. Divide them by their
lengths to find orthonormal vectors $q_1$ and $q_2$:_

Let's denote these vectors $A$ and $B$ as such:

$$ A = \begin{bmatrix}{}2\\2\\-1\end{bmatrix}, B = \begin{bmatrix}{}-1\\2\\2\end{bmatrix} $$

Then:

$$ q_1 = \frac{A}{\|A\|} $$

$$ \|A\| = \sqrt{(2)^2 + (2)^2 + (-1)^2} = \sqrt{9} = 3 $$

$$ q_1 = \frac{1}{3}\begin{bmatrix}{}2\\2\\-1\end{bmatrix} = \begin{bmatrix}{}\frac{2}{3}\\\frac{2}{3}\\-\frac{1}{3}\end{bmatrix} $$

$$ q_2 = \frac{B}{\|B\|} $$

$$ \|B\| = \sqrt{(-1)^2 + (2)^2 + (2)^2} = \sqrt{9} = 3 $$

$$ q_2 = \frac{1}{3}\begin{bmatrix}{}-1\\2\\2\end{bmatrix} = \begin{bmatrix}{}-\frac{1}{3}\\\frac{2}{3}\\\frac{2}{3}\end{bmatrix} $$

_Put those into the columns of $Q$ and multiply $Q^{\mathbf{T}}Q$ and
$QQ^{\mathbf{T}}$:_

$$ Q =
\frac{1}{3}\left[\begin{array}{rr}
2 & -1 \\
2 & 2 \\
-1 & 2 \\
\end{array}\right]
$$

$$ Q^{\mathbf{T}}Q =
\frac{1}{3}
\left[\begin{array}{rrr}
2 & 2 & -1 \\
-1 & 2 & 2 \\
\end{array}\right]
\frac{1}{3}
\left[\begin{array}{rr}
2 & -1 \\
2 & 2 \\
-1 & 2 \\
\end{array}\right]  =
\frac{1}{9}
\left[\begin{array}{cc}
9 & 0 \\
0 & 9 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
0 & 1 \\
\end{array}\right] = I
$$

$$ QQ^{\mathbf{T}} =
\frac{1}{3}
\left[\begin{array}{rr}
2 & -1 \\
2 & 2 \\
-1 & 2 \\
\end{array}\right]
\frac{1}{3}
\left[\begin{array}{rrr}
2 & 2 & -1 \\
-1 & 2 & 2 \\
\end{array}\right] =
\frac{1}{9}
\left[\begin{array}{rrr}
5 & 2 & -4 \\
2 & 8 & 2 \\
-4 & 2 & 5 \\
\end{array}\right]
$$

3.

a. If $A$ has three orthogonal columns each of length $4$, what is
$A^{\mathbf{T}}A$?

b. If $A$ has three orthogonal columns of length $1, 2, 3$, what is
$A^{\mathbf{T}}A$?

_Solution:_

a. $A^{\mathbf{T}}A = 16I$

This is because when Strang says length, always remember he means Euclidean
Norm! So if
$\|A\| = 4 \Rightarrow 4 = \sqrt{a_1^2 + a_2^2 + \dots + a_n^2} \Rightarrow 4^2 = 16$.

b. $A^{\mathbf{T}}A$ will be diagonal with diagonal entries $1, 4, 9$.

4. Give an example of each of the following:

a. A matrix $Q$ that has orthonormal columns but $QQ^{\mathbf{T}} \neq I$.

$$ Q =
\left[\begin{array}{rr}
1 & 0 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

$$ QQ^{\mathbf{T}} =
\left[\begin{array}{rr}
1 & 0 \\
0 & 1 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right] \neq I
$$

Notice that when choosing each $q$ column, we either had to choose a standard
unit vector or use a fraction that sums up to where their Euclidean Norm Length
ends up being $\sqrt{1} = 1$.

b. Two orthogonal vectors that are not linearly independent.

$$ a = \begin{bmatrix}{}0\\0\end{bmatrix}, b = \begin{bmatrix}{}1\\0\end{bmatrix} $$

c. An orthonormal basis for $\R^3$, including the vector
$q_1 = \dfrac{(1, 1, 1)}{\sqrt{3}}$.

Here, we can use Gram-Schmidt's formula to find $q_2, q_3$.

Let $A = a = \dfrac{1}{\sqrt{3}}\begin{bmatrix}{}1\\1\\1\end{bmatrix}$.

Now starting the Gram-Schmidt formula:

$$ B = b - \frac{A^{\mathbf{T}}b}{A^{\mathbf{T}}A}A $$

Since we don't have a $b$, we have to choose a vector $b$ that is not linearly
dependent on $a$. Say $b = \begin{bmatrix}{}1\\1\\0\end{bmatrix}$.

$$ B = \begin{bmatrix}{}1\\1\\0\end{bmatrix} - \frac{A^{\mathbf{T}}b}{A^{\mathbf{T}}A}A $$

$$ A^{\mathbf{T}}A = \left(\frac{1}{\sqrt{3}}\right)\left(\frac{1}{\sqrt{3}}\right) + \left(\frac{1}{\sqrt{3}}\right)\left(\frac{1}{\sqrt{3}}\right) + \left(\frac{1}{\sqrt{3}}\right)\left(\frac{1}{\sqrt{3}}\right) = \frac{1}{3} + \frac{1}{3} + \frac{1}{3} = 1 $$

$$ A^{\mathbf{T}}b =
\frac{1}{\sqrt{3}}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\0\end{bmatrix} =
\frac{2}{\sqrt{3}}
$$

$$ B = \begin{bmatrix}{}1\\1\\0\end{bmatrix} - \frac{2}{\sqrt{3}}\begin{bmatrix}{}\frac{1}{\sqrt{3}}\\\frac{1}{\sqrt{3}}\\\frac{1}{\sqrt{3}}\end{bmatrix} $$

$$ = \begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} $$

$$ q_2 = \frac{B}{\|B\|} $$

$$ \|B\| = \sqrt{\left(\frac{1}{3}\right)^2 + \left(\frac{1}{3}\right)^2 + \left(-\frac{2}{3}\right)^2} $$

$$ = \frac{\sqrt{6}}{3} $$

$$ q_2 = \frac{3}{\sqrt{6}}\begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} = \begin{bmatrix}{}\frac{1}{\sqrt{6}}\\\frac{1}{\sqrt{6}}\\-\frac{\sqrt{6}}{3}\end{bmatrix}$$

$$ C = c - \frac{A^{\mathbf{T}}c}{A^{\mathbf{T}}A}A - \frac{B^{\mathbf{T}}c}{B^{\mathbf{T}}B}B $$

Keep it simple and choose $c = (0, 0, 1)$. We already know
$A^{\mathbf{T}}A = 1$.

$$ C = c - A^{\mathbf{T}}cA - \frac{B^{\mathbf{T}}c}{B^{\mathbf{T}}B}B $$

$$ A^{\mathbf{T}}c =
\frac{1}{\sqrt{3}}
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}0\\0\\1\end{bmatrix} = \frac{1}{\sqrt{3}}
$$

$$ C = c - A - \frac{B^{\mathbf{T}}c}{B^{\mathbf{T}}B}B $$

$$ B^{\mathbf{T}}B =
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & -\frac{2}{3} \\
\end{array}\right]
\begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} =
\frac{2}{3}
$$

$$ B^{\mathbf{T}}c =
\left[\begin{array}{ccc}
\frac{1}{3} & \frac{1}{3} & -\frac{2}{3} \\
\end{array}\right]
\begin{bmatrix}{}0\\0\\1\end{bmatrix} =
-\frac{2}{3}
$$

$$ C = \begin{bmatrix}{}0\\0\\1\end{bmatrix} - \frac{1}{\sqrt{3}}\begin{bmatrix}{}1\\1\\1\end{bmatrix} - \left(\frac{3}{2}\right)\left(-\frac{2}{3}\right)\begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} $$

$$ = \begin{bmatrix}{}-\frac{1}{\sqrt{3}}\\-\frac{1}{\sqrt{3}}\\1 - \frac{1}{\sqrt{3}}\end{bmatrix} - (-1)\begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} $$

$$ = \begin{bmatrix}{}-\frac{1}{\sqrt{3}}\\-\frac{1}{\sqrt{3}}\\1 - \frac{1}{\sqrt{3}}\end{bmatrix} + \begin{bmatrix}{}\frac{1}{3}\\\frac{1}{3}\\-\frac{2}{3}\end{bmatrix} $$

$$ = \begin{bmatrix}{}\frac{1}{3} -\frac{1}{\sqrt{3}}\\\frac{1}{3} - \frac{1}{\sqrt{3}}\\\frac{1}{3} - \frac{1}{\sqrt{3}}\end{bmatrix}$$

$$ q_3 = \frac{C}{\|C\|} $$

$$ \|C\| = \sqrt{\left(\frac{1}{3} - \frac{1}{\sqrt{3}}\right)^2 + \left(\frac{1}{3} - \frac{1}{\sqrt{3}}\right)^2 + \left(\frac{1}{3} - \frac{1}{\sqrt{3}}\right)^2} $$

$$ = 1 - \frac{1}{\sqrt{3}}$$

$$ q_3 = \frac{1}{1 - \frac{1}{\sqrt{3}}}\begin{bmatrix}{}\frac{1}{3} - \frac{1}{\sqrt{3}}\\\frac{1}{3} - \frac{1}{\sqrt{3}}\\\frac{1}{3} - \frac{1}{\sqrt{3}}\end{bmatrix} $$

$$ q_3 = \begin{bmatrix}{}-3\sqrt{3} - \frac{9}{2}\\-3\sqrt{3} - \frac{9}{2}\\-3\sqrt{3} - \frac{9}{2}\end{bmatrix}$$

Aborted here. We get the idea, and this is getting too messy.

Ultimately omitted.

5. Find two orthogonal vectors in the plane $x + y + 2z = 0$. Make them
   orthonormal.

_Solution:_

_Find two orthogonal vectors in the plane $x + y + 2z = 0$:_

The given vector is:

$$ a_1 = \begin{bmatrix}{}1\\1\\2\end{bmatrix} $$

To find orthogonal vectors to $a_1$, just choose $a_1^{\mathbf{T}}a_2 = 0$, and
same for $a_3$.

Simple ones would be $(1)(2) + (1)(2) + (2)(-2) = 0$, so:

$$ a_2 = \begin{bmatrix}{}2\\2\\-2\end{bmatrix} $$

So here we have $a_1 \perp a_2$, but to choose $a_3$, we'll need $a_1 \perp a_3$
and $a_2 \perp a_3$. We could use Gram-Schmidt, but more simpy will be to choose
any vector that satisfies $x + y + 2z = 0$ that is $\perp a_2$ and $\perp a_1$.
Notice that we are solving for 3 unknowns here, so set up a matrix:

$$
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
2 & 2 & -2 & 0 \\
\end{array}\right]
$$

Now choose a third row that is independent of the third, but satisfies $= 0$ .

$$
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
2 & 2 & -2 & 0 \\
1 & 0 & 0 & 0 \\
\end{array}\right]
$$

Now eliminate:

$$
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
2 & 2 & -2 & 0 \\
1 & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
2 & 2 & -2 & 0 \\
0 & -1 & -2 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
0 & 0 & -6 & 0 \\
0 & -1 & -2 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc|c}
1 & 1 & 2 & 0 \\
0 & -1 & -2 & 0 \\
0 & 0 & -6 & 0 \\
\end{array}\right]
$$

From $-6z = 0 \Rightarrow z = 0$, we plug this into $a_1$ to find
$x + y = 0 \Rightarrow x = -y$, so we can get away with:

$$ a_3 = \begin{bmatrix}{}1\\-1\\0\end{bmatrix} $$

So we found two orthogonal vectors in the plane of $x + y + 2z = 0$, and they
are:

$$ a_2 = \begin{bmatrix}{}2\\2\\-2\end{bmatrix}, a_3 = \begin{bmatrix}{}1\\-1\\0\end{bmatrix} $$

_Make them orthonormal:_

$$ q_2 = \frac{a_2}{\|a_2\|} $$

$$ \|a_2\| = \sqrt{(2)^2 + (2)^2 + (-2)^2} = 2\sqrt{3} $$

$$ q_2 = \frac{1}{2\sqrt{3}}\begin{bmatrix}{}2\\2\\-2\end{bmatrix} = \begin{bmatrix}{}\frac{1}{\sqrt{3}}\\\frac{1}{\sqrt{3}}\\-\frac{1}{\sqrt{3}}\end{bmatrix} $$

$$ q_3 = \frac{a_3}{\|a_3\|} $$

$$ \|a_3\| = \sqrt{(1)^2 + (-1)^2 + (0)^2} = \sqrt{2} $$

$$ q_3 = \frac{1}{\sqrt{2}}\begin{bmatrix}{}1\\-1\\0\end{bmatrix} = \begin{bmatrix}{}\frac{1}{\sqrt{2}}\\-\frac{1}{\sqrt{2}}\\0\end{bmatrix} $$

6. If $Q_1$ and $Q_2$ are orthogonal matrices, show that their product $Q_1Q_2$
   is also an orthogonal matrix. (Use $Q^{\mathbf{T}}Q = I$.)

_Solution:_

**Proof:**

Suppose $Q_1$ and $Q_2$ are both orthogonal matrices.

It is to be shown that $Q_1Q_2$ is orthogonal.

Since, by the supposition, both $Q_1$ and $Q_2$ are orthogonal, it follows that
$Q_1^{\mathbf{T}}Q_1 = I$ and $Q_2^{\mathbf{T}}Q_2 = I$.

Consider then what happens if we take their multiple and attempt to apply the
same principle:

$$ (Q_1Q_2)^{\mathbf{T}}(Q_1Q_2) $$

"Distributing" the transposition results in:

$$ = Q_2^{\mathbf{T}}Q_1^{\mathbf{T}}Q_1Q_2 $$

By the identity property of orthogonal matrices (as stated above), the middle
term $Q_1^{\mathbf{T}}Q_1 = I$, thus by substitution:

$$ = Q_2^{\mathbf{T}}(I)Q_2 $$

And of course, $IQ_2 = Q_2$, so:

$$ = Q_2^{\mathbf{T}}Q_2 $$

And by similar logic, we know that $Q_2^{\mathbf{T}}Q = I$, so, once again, by
substitution:

$$ = I $$

This is what was to be shown.

Q.E.D.

7. If $Q$ has orthonormal columns, what is the least squares solution $\hat{x}$
   to $Qx = b$?

When Gram-Schmidt gives $Q$ with orthonormal columns,
$Q^{\mathbf{T}}Q\hat{x} = Q^{\mathbf{T}}b$. Recall the similarity this has to
the previous section where we covered projection and established solving for
$\hat{x}$ with $A^{\mathbf{T}}A\hat{x} = A^{\mathbf{T}}b$.

Unlike our solution with $A$, however, our solution with $Q$ is a bit more
succinct. Since $Q^{\mathbf{T}}Q = I$, we can simply find $\hat{x}$ like so:

$$ \hat{x} = Q^{\mathbf{T}}b $$

8. If $q_1$ and $q_2$ are orthonormal vectors in $\R^5$, what combination ____
   $q_1 +$ ____ $q_2$ is closest to a given vector $b$?

_Solution:_

_What combination (?) $q_1 +$ (?) $q_2$ is closest to a given vector $b$?:_

We are being asked what linear combination expresses a projection vector $p$
that is closest to $b$. This is just the dot product of each $q$ with $b$.

$$ p = (q_1^{\mathbf{T}}b)q_1 + (q_2^{\mathbf{T}}b)q_2 $$

9.

a. Compute $P = QQ^{\mathbf{T}}$ when $q_1 = (.8, .6, 0)$ and
$q_2 = (-.6, .8, 0)$. Verify that $P^2 = P$.

_Solution:_

$$ P = QQ^{\mathbf{T}} =
\left[\begin{array}{rr}
.8 & -.6 \\
.6 & .8 \\
0 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
.8 & .6 & 0 \\
-.6 & .8 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
$$

$$ P^2 = PP =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0 \\
\end{array}\right] = P
$$

b. Prove that always $(QQ^{\mathbf{T}})^2 = QQ^{\mathbf{T}}$ by using
$Q^{\mathbf{T}}Q = I$. Then $P = QQ^{\mathbf{T}}$ is the projection matrix onto
the column space of $Q$.

_Solution:_

**Proof:**

Suppose $Q$ is an orthogonal matrix.

It is to be demonstrated that $(QQ^{\mathbf{T}})^2 = QQ^{\mathbf{T}}$.

Consider:

$$ (QQ^{\mathbf{T}})^2 $$

By exponentiation, we can "expand" this out to :

$$ = (QQ^{\mathbf{T}})(QQ^{\mathbf{T}}) $$

Remove the parentheses:

$$ = QQ^{\mathbf{T}}QQ^{\mathbf{T}} $$

Now, by the definition of orthogonal matrices $Q^{\mathbf{T}}Q = I$, so, by
substitution:

$$ = Q(I)Q^{\mathbf{T}} $$

And, of course, $I(Q^{\mathbf{T}}) = Q^{\mathbf{T}}$, so:

$$ = QQ^{\mathbf{T}} $$

This is what was to be demonstrated.

Q.E.D.

10. Orthonormal vectors are automatically linearly independent.

a. Vector proof: When $c_1q_1 + c_2q_2 + c_3q_3 = \mathbf{0}$, what dot product
leads to $c_1 = 0$? Similarly $c_2 = 0$ and $c_3 = 0$. Thus the $q$'s are
independent.

_Solution:_

**Proof:**

Suppose $q_1, q_2, q_3$ are orthonormal vectors.

It is to be shown that $q_1, q_2, q_3$ are linearly independent.

Consider a linear equation $c_1q_1 + c_2q_2 + c_3q_3 = \mathbf{0}$. This would
be linearly independent.

If we take the product of this equation with $q_1^{\mathbf{T}}$:

$$ q_1^{\mathbf{T}}(c_1q_1 + c_2q_2 + c_3q_3) = q_1^{\mathbf{T}}\mathbf{0} $$

$$ q_1^{\mathbf{T}}c_1q_1 + q_1^{\mathbf{T}}c_2q_2 + q_1^{\mathbf{T}}c_3q_3 = 0 $$

Recall that orthonormal vectors are defined such that:

$$
q_i^{\mathbf{T}}q_j =
\begin{cases}
0 & \text{when } i \neq j \\
1 & \text{when } i = j
\end{cases}
$$

We can therefore apply this orthnormal property to our linear equation as:

$$ c_1(1) + c_2(0) + c_3(0) = 0 $$

$$ c_1 = 0 $$

Similarly, $c_2 = 0$ and $c_3 = 0$.

This is sufficient to demonstrate that $q_1, q_2, q_3$ are linearly independent.

Q.E.D.

b. Matrix proof: Show that $Qx = \mathbf{0}$ leads to $x = \mathbf{0}$. Since
$Q$ may be rectangular, you can use $Q^{\mathbf{T}}$ but not $Q^{-1}$.

_Solution:_

**Proof:**

Suppose $Q$ is an orthogonal matrix and $x$ is any vector such that:

$$ Qx = \mathbf{0} $$

It is to shown that $x = \mathbf{0}$.

Consider when both sides of $Qx = \mathbf{0}$ are multiplied by
$Q^{\mathbf{T}}$:

$$ Q^{\mathbf{T}}Qx =  \mathbf{0} $$

By the identity property of orthogonal matrices, $Q^{\mathbf{T}}Q = I$, thus by
substitution:

$$ Ix =  \mathbf{0} $$

$$ x = \mathbf{0} $$

This is what was to be shown.

It can be concluded that all columns of $Q$ are linearly independent.

Q.E.D.

11.

a. Gram-Schmidt: Find orthonormal vectors $q_1$ and $q_2$ in the plane spanned
by $a = (1, 3, 4, 5, 7)$ and $b = (-6, 6, 8, 0, 8)$.

$$ q_1 = \frac{a}{\|a\|} $$

$$ \|a\| = \sqrt{(1)^2 + (3)^2 + (4)^2 + (5)^2 + (7)^2} $$

$$ = \sqrt{1 + 9 + 16 + 25 + 49} $$

$$ = \sqrt{100} = 10 $$

$$ q_1 = \frac{1}{10}\begin{bmatrix}{}1\\3\\4\\5\\7\end{bmatrix} $$

To get $q_2$, it's not as straight forward, as we need $q_2 \perp q_1$. To do
this then, we'll need the following formula for Gram-Schmidt on vectors:

$$ q_2 = \frac{b - (q_1^{\mathbf{T}}b)q_1}{\|b - (q_1^{\mathbf{T}}b)q_1\|} $$

$$ q_1^{\mathbf{T}}b =
\frac{1}{10}
\left[\begin{array}{ccccc}
1 & 3 & 4 & 5 & 7 \\
\end{array}\right]
\begin{bmatrix}{}-6\\6\\8\\0\\8\end{bmatrix} =
\frac{1}{10}(100) = 10
$$

$$ (q_1^{\mathbf{T}}b)q_1 = 10q_1 =
10\left(\frac{1}{10}\right)\begin{bmatrix}{}1\\3\\4\\5\\7\end{bmatrix} =
\begin{bmatrix}{}1\\3\\4\\5\\7\end{bmatrix}
$$

$$ b - (q_1^{\mathbf{T}}b)q_1 =
\begin{bmatrix}{}-6\\6\\8\\0\\8\end{bmatrix} - \begin{bmatrix}{}1\\3\\4\\5\\7\end{bmatrix} =
\begin{bmatrix}{}-7\\3\\4\\-5\\1\end{bmatrix}
$$

$$ \|b - (q_1^{\mathbf{T}}b)q_1\| =
\sqrt{(-7)^2 + (3)^2 + (4)^2 + (-5)^2 + (1)^2} = \sqrt{100} = 10
$$

$$ q_2 = \frac{1}{10}\begin{bmatrix}{}-7\\3\\4\\-5\\1\end{bmatrix} $$

b. Which vector in this plane is closest to $(1, 0, 0, 0, 0)$?

_Solution:_

To solve, you must put $q_1, q_2$ as a matrix $Q$, then take
$QQ^{\mathbf{T}}\begin{bmatrix}{}1\\0\\0\\0\\0\end{bmatrix}$ to find the closest
vector.

$$ q_1 = \frac{1}{10}\begin{bmatrix}{}1\\3\\4\\5\\7\end{bmatrix} $$

$$ q_2 = \frac{1}{10}\begin{bmatrix}{}-7\\3\\4\\-5\\1\end{bmatrix} $$

$$ QQ^{\mathbf{T}} =
\frac{1}{10}
\left[\begin{array}{rr}
1 & -7 \\
3 & 3 \\
4 & 4 \\
5 & -5 \\
7 & 1 \\
\end{array}\right]
\frac{1}{10}
\left[\begin{array}{rr}
1 & 3 & 4 & 5 & 7 \\
-7 & 3 & 4 & -5 & 1 \\
\end{array}\right] =
\frac{1}{100}
\left[\begin{array}{rrrrr}
50 & -18 & -24 & 40 & 0 \\
-18 & 18 & 24 & 0 & 24 \\
-24 & 24 & 32 & 0 & 32 \\
40 & 0 & 0 & 50 & 30 \\
0 & 24 & 32 & 30 & 50 \\
\end{array}\right]
$$

$$ QQ^{\mathbf{T}}\begin{bmatrix}{}1\\0\\0\\0\\0\end{bmatrix} = \frac{1}{100}
\left[\begin{array}{rrrrr} 50 & -18 & -24 & 40 & 0 \\ -18 & 18 & 24 & 0 & 24 \\
-24 & 24 & 32 & 0 & 32 \\ 40 & 0 & 0 & 50 & 30 \\ 0 & 24 & 32 & 30 & 50 \\
\end{array}\right] \begin{bmatrix}{}1\\0\\0\\0\\0\end{bmatrix} =
\boxed{\frac{1}{100}
\begin{bmatrix}{}50\\-18\\-24\\40\\0\end{bmatrix}}
$$

12. If $a_1, a_2, a_3$ is a basis for $\R^3$, any vector $b$ can be written as

$$ b = x_1a_1 + x_2a_2 + x_3a_3 $$

or

$$
\left[\begin{array}{ccc}
& & \\
a_1 & a_2 & a_3 \\
& & \\
\end{array}\right]
\begin{bmatrix}{}x_1\\x_2\\x_3\end{bmatrix} = b
$$

a. Suppose the $a$'s are orthonormal. Show that $x_1 = a_1^{\mathbf{T}}b$.

_Solution:_

$$ a_1^{\mathbf{T}}b = a_1^{\mathbf{T}}(x_1a_1 + x_2a_2 + x_3a_3) $$

$$ = a_1^{\mathbf{T}}x_1a_1 + a_1^{\mathbf{T}}x_2a_2 + a_1^{\mathbf{T}}x_3a_3 $$

Again, recall the laws of orthonormal, where each of these dot products is
either $1$ or $0$ ($1$ if $i = j$, $0$ if $i \neq j$):

$$ = a_1^{\mathbf{T}}x_1a_1 + 0 + 0 $$

$$ = x_1(a_1^{\mathbf{T}}a_1) = x_1(1) = x_1 $$

b. Suppose the $a$'s are orthogonal. Show that
$x_1 = \dfrac{a_1^{\mathbf{T}}b}{a_1^{\mathbf{T}}a_1}$.

_Solution:_

As in part (a), we have already shown that $a_1^{\mathbf{T}}a_1 = 1$, this
leaves us to show:

$$ x_1 = a_1^{\mathbf{T}}b $$

And we also showed that in part (a).

This makes sense since in part (a), we assume that all the $a$'s are
orthonormal, which are orthogonal by definition.

c. If the $a$'s are independent, $x_1$ is the first component of ____ times $b$.

_Solution:_

$A^{-1}$

This follows from the standard $Ax = b$, if we solve for $x$ we get
$x = A^{-1}b$ when $A$ is independent, and thus it follows that the first
component $x_1$ would be the first component of $A^{-1}$ times $b$.

**Problems 13-25 are about the Gram-Schmidt process and $A = QR$.**

13. What multiple of $a = \begin{bmatrix}{}1\\1\end{bmatrix}$ should be
    subtracted from $b = \begin{bmatrix}{}4\\0\end{bmatrix}$ to make the result
    $B$ orthogonal to $a$? Sketch a figure to show $a, b$, and $B$.

_Solution:_

Recall the generic Gram-Schmidt process:

$$ B = b - \frac{A^{\mathbf{T}}b}{A^{\mathbf{T}}A}A $$

When applied to our specific vectors, this is:

$$ B = b - \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}a $$

Let's now evaluate and solve:

$$ a^{\mathbf{T}}a =
\left[\begin{array}{cc}
1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\end{bmatrix} = 2
$$

$$ a^{\mathbf{T}}b =
\left[\begin{array}{cc}
1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}4\\0\end{bmatrix} = 4
$$

$$ B = \begin{bmatrix}{}4\\0\end{bmatrix} - \frac{1}{2}(4)\begin{bmatrix}{}1\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}4\\0\end{bmatrix} - 2\begin{bmatrix}{}1\\1\end{bmatrix} $$

$$ = \begin{bmatrix}{}4\\0\end{bmatrix} - \begin{bmatrix}{}2\\2\end{bmatrix} $$

$$ = \begin{bmatrix}{}2\\-2\end{bmatrix} $$

14. Complete the Gram-Schmidt process in Problem 13 by computing
    $q_1 = \dfrac{a}{\|a\|}$ and $q_2 = \dfrac{B}{\|B\|}$ and factoring into
    $QR$:

$$
\left[\begin{array}{cc}
1 & 4 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
q_1 & q_2 \\
\end{array}\right]
\left[\begin{array}{cc}
\|a\| & \text{?} \\
0 & \|B\| \\
\end{array}\right]
$$

_Solution:_

$$ q_1 = \frac{a}{\|a\|} $$

$$ \|a\| = \sqrt{(1)^2 + (1)^2} = \sqrt{2} $$

$$ q_1 = \frac{1}{\sqrt{2}}\begin{bmatrix}{}1\\1\end{bmatrix} $$

$$ q_1 = \begin{bmatrix}{}\frac{1}{\sqrt{2}}\\\frac{1}{\sqrt{2}}\end{bmatrix} $$

$$ q_2 = \frac{B}{\|B\|} $$

$$ \|B\| = \sqrt{(2)^2 + (-2)^2} = 2\sqrt{2} $$

$$ q_2 = \frac{1}{2\sqrt{2}}\begin{bmatrix}{}2\\-2\end{bmatrix}$$

$$ q_2 = \begin{bmatrix}{}\frac{1}{\sqrt{2}}\\-\frac{1}{\sqrt{2}}\end{bmatrix} $$

$$
\left[\begin{array}{cc}
1 & 4 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}} \\
\end{array}\right]
\left[\begin{array}{cc}
\sqrt{2} & ? \\
0 & 2\sqrt{2} \\
\end{array}\right]
$$

$$ \frac{1}{\sqrt{2}}(?) + \frac{1}{\sqrt{2}}2\sqrt{2} = 4 $$

$$ \frac{1}{\sqrt{2}}(?) + 2 = 4 $$

$$ \frac{1}{\sqrt{2}}(?) = 2 $$

$$ ? = 2\sqrt{2} $$

Thus:

$$ QR =
\left[\begin{array}{cc}
\sqrt{2} & 2\sqrt{2} \\
0 & 2\sqrt{2} \\
\end{array}\right]
$$

15.

a. Find orthonormal vectors $q_1, q_2, q_3$ such that $q_1, q_2$ span the column
space of

$$ A =
\left[\begin{array}{rr}
1 & 1 \\
2 & -1 \\
-2 & 4 \\
\end{array}\right]
$$

_Solution:_

$$ q_1 = \frac{a_1}{\|a_1\|} $$

$$ \|a_1\| = \sqrt{(1)^2 + (2)^2 + (-2)^2} = \sqrt{9} = 3 $$

$$ q_1 = \frac{1}{3}\begin{bmatrix}{}1\\2\\-2\end{bmatrix} = \begin{bmatrix}{}\frac{1}{3}\\\frac{2}{3}\\-\frac{2}{3}\end{bmatrix} $$

$$ q_2 = \frac{a_2 - (q_1^{\mathbf{T}}a_2)q_1}{\|a_2 - (q_1^{\mathbf{T}}a_2)q_1\|} $$

$$ q_1^{\mathbf{T}}a_2 =
\left[\begin{array}{rrr}
\frac{1}{3} & \frac{2}{3} & -\frac{2}{3} \\
\end{array}\right]
\begin{bmatrix}{}1\\-1\\4\end{bmatrix} = -3
$$

$$ (q_1^{\mathbf{T}}a_2)q_1 =
-3
\begin{bmatrix}{}\frac{1}{3}\\\frac{2}{3}\\-\frac{2}{3}\end{bmatrix} =
\begin{bmatrix}{}-1\\-2\\2\end{bmatrix}
$$

$$ a_2 - (q_1^{\mathbf{T}}a_2)q_1 =
\begin{bmatrix}{}1\\-1\\4\end{bmatrix} - \begin{bmatrix}{}-1\\-2\\2\end{bmatrix} =
\begin{bmatrix}{}2\\1\\2\end{bmatrix}
$$

$$ \|a_2 - (q_1^{\mathbf{T}}a_2)q_1\| =
\sqrt{(2)^2 + (1)^2 + (2)^2} = \sqrt{9} = 3
$$

$$ q_2 = \frac{1}{3}\begin{bmatrix}{}2\\1\\2\end{bmatrix} =
\begin{bmatrix}{}\frac{2}{3}\\\frac{1}{3}\\\frac{2}{3}\end{bmatrix}
$$

For $q_3$, we don't have a third column $a_3$, thus we must choose an $a_3$ that
is $\notin C(A)$ or more specifically $\in N(A^{\mathbf{T}})$.

Recall that finding a vector $v \in N(A^{\mathbf{T}})$ has us solving for $v$ in
$A^{\mathbf{T}}v = \mathbf{0}$:

$$ A^{\mathbf{T}}v =
\left[\begin{array}{rrr}
1 & 2 & -2 \\
1 & -1 & 4 \\
\end{array}\right]
$$

Now reduce to reduced row echelon form $R$:

$$ A^{\mathbf{T}}v =
\left[\begin{array}{rrr}
1 & 2 & -2 \\
1 & -1 & 4 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -2 \\
0 & -3 & 6 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & -2 \\
0 & 1 & -2 \\
\end{array}\right] = R
$$

Solve:

$$ 1v_2 + (-2)v_3 = 0 \Rightarrow v_2 - 2v_3 = 0 \Rightarrow v_2 = 2v_3 $$

$$ 1v_1 + 2v_2 + (-2)v_3 = 0 \Rightarrow v_1 + 2(2v_3) - 2v_3 = 0 \Rightarrow v_1 + 4v_3 - 2v_3 = 0 \Rightarrow v_1 + 2v_3 = 0 \Rightarrow v_1 = -2v_3 $$

So, choose $v_3 = 1$, then:

$$ v_1 = -2, v_2 = 2, v_3 = 1 $$

Thus our third column, $v = a_3$, to be chosen is:

$$ a_3 = v = \begin{bmatrix}{}-2\\2\\1\end{bmatrix} $$

Finally! So now follow the Gram-Schmidt formula for vectors for this $a_3$:

$$ q_3 = \frac{a_3 - (q_2^{\mathbf{T}}a_3)q_2}{\|a_3 - (q_2^{\mathbf{T}}a_3)q_2\|} $$

$$ q_2^{\mathbf{T}}a_3 =
\left[\begin{array}{ccc}
\frac{2}{3} & \frac{1}{3} & \frac{2}{3} \\
\end{array}\right]
\begin{bmatrix}{}-2\\2\\1\end{bmatrix} = 0
$$

$$ (q_2^{\mathbf{T}}a_3)q_2 =
0\begin{bmatrix}{}\frac{2}{3}\\\frac{1}{3}\\\frac{2}{3}\end{bmatrix} = \begin{bmatrix}{}0\\0\\0\end{bmatrix}
$$

$$ a_3 - (q_2^{\mathbf{T}}a_3)q_2 =
\begin{bmatrix}{}-2\\2\\1\end{bmatrix} - \begin{bmatrix}{}0\\0\\0\end{bmatrix} =
\begin{bmatrix}{}-2\\2\\1\end{bmatrix}
$$

$$ \|a_3 - (q_2^{\mathbf{T}}a_3)q_2\| =
\sqrt{(-2)^2 + (2)^2 + (1)^2} = \sqrt{9} = 3
$$

$$ q_3 = \frac{1}{3}\begin{bmatrix}{}-2\\2\\1\end{bmatrix} =
\begin{bmatrix}{}-\frac{2}{3}\\\frac{2}{3}\\\frac{1}{3}\end{bmatrix}
$$

b. Which of the four fundamental subspaces contains $q_3$?

_Solution:_

$$ q_3 \in N(A^{\mathbf{T}}) $$

c. Solve $Ax = (1, 2, 7)$ by least squares.

_Solution:_

Recall the basic formula for finding $\hat{x}$:

$$ \hat{x} = (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}b $$

$$ A^{\mathbf{T}}A =
\left[\begin{array}{rrr}
1 & 2 & -2 \\
1 & -1 & 4 \\
\end{array}\right]
\left[\begin{array}{rr}
1 & 1 \\
2 & -1 \\
-2 & 4 \\
\end{array}\right] =
\left[\begin{array}{rr}
9 & -9 \\
-9 & 18 \\
\end{array}\right]
$$

Use Gauss-Jordan to find $(A^{\mathbf{T}}A)^{-1}$:

$$
\left[\begin{array}{rr|rr}
9 & -9 & 1 & 0 \\
-9 & 18 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
9 & -9 & 1 & 0 \\
0 & 9 & 1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
9 & 0 & 2 & 1 \\
0 & 9 & 1 & 1 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{rr|rr}
9 & 0 & 2 & 1 \\
0 & 1 & \frac{1}{9} & \frac{1}{9} \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
1 & 0 & \frac{2}{9} & \frac{1}{9} \\
0 & 1 & \frac{1}{9} & \frac{1}{9} \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}}A)^{-1} =
\left[\begin{array}{rr}
\frac{2}{9} & \frac{1}{9} \\
\frac{1}{9} & \frac{1}{9} \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} =
\left[\begin{array}{rr}
\frac{2}{9} & \frac{1}{9} \\
\frac{1}{9} & \frac{1}{9} \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 2 & -2 \\
1 & -1 & 4 \\
\end{array}\right] =
\left[\begin{array}{rrr}
\frac{1}{3} & \frac{1}{3} & 0 \\
\frac{2}{9} & \frac{1}{9} & \frac{2}{9} \\
\end{array}\right]
$$

$$ (A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}b =
\left[\begin{array}{rrr}
\frac{1}{3} & \frac{1}{3} & 0 \\
\frac{2}{9} & \frac{1}{9} & \frac{2}{9} \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\7\end{bmatrix} =
\boxed{\begin{bmatrix}{}1\\2\end{bmatrix} = \hat{x}}
$$

16. What multiple of $a = (4, 5, 2, 2)$ is closest to $b = (1, 2, 0, 0)$? Find
    orthonormal vectors $q_1$ and $q_2$ in the plane of $a$ and $b$.

_Solution:_

_What multiple of $a = (4, 5, 2, 2)$ is closest to $b = (1, 2, 0, 0)$?:_

This is just finding $p$, recall that $p$ is:

$$ p = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}a $$

$$ a^{\mathbf{T}}a =
\left[\begin{array}{cccc}
4 & 5 & 2 & 2 \\
\end{array}\right]
\begin{bmatrix}{}4\\5\\2\\2\end{bmatrix} = 49
$$

$$ a^{\mathbf{T}}b =
\left[\begin{array}{cccc}
4 & 5 & 2 & 2 \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\0\\0\end{bmatrix} = 14
$$

$$ p = \frac{14}{49}a = \frac{2}{7}a $$

$$ p =
\frac{2}{7}
\begin{bmatrix}{}4\\5\\2\\2\end{bmatrix} =
\begin{bmatrix}{}\frac{8}{7}\\\frac{10}{7}\\\frac{4}{7}\\\frac{4}{7}\end{bmatrix}
$$

_Find orthonormal vectors $q_1$ and $q_2$ in the plane of $a$ and $b$:_

$$ q_1 = \frac{a}{\|a\|} $$

$$ \|a\| = \sqrt{(4)^2 + (5)^2 + (2)^2 + (2)^2} = \sqrt{16 + 25 + 4 + 4} = \sqrt{49} = 7 $$

$$ q_1 = \frac{1}{7}\begin{bmatrix}{}4\\5\\2\\2\end{bmatrix} = \begin{bmatrix}{}\frac{4}{7}\\\frac{5}{7}\\\frac{2}{7}\\\frac{2}{7}\end{bmatrix} $$

$$ q_2 = \frac{b - (q_1^{\mathbf{T}}b)q_1}{\|b - (q_1^{\mathbf{T}}b)q_1\|} $$

$$ q_1^{\mathbf{T}}b =
\left[\begin{array}{cccc}
\frac{4}{7} & \frac{5}{7} & \frac{2}{7} & \frac{2}{7} \\
\end{array}\right]
\begin{bmatrix}{}1\\2\\0\\0\end{bmatrix} = 2
$$

$$ (q_1^{\mathbf{T}}b)q_1 =
2
\begin{bmatrix}{}\frac{4}{7}\\\frac{5}{7}\\\frac{2}{7}\\\frac{2}{7}\end{bmatrix} =
\begin{bmatrix}{}\frac{8}{7}\\\frac{10}{7}\\\frac{4}{7}\\\frac{4}{7}\end{bmatrix}
$$

$$ b - (q_1^{\mathbf{T}}b)q_1 =
\begin{bmatrix}{}1\\2\\0\\0\end{bmatrix} -
\begin{bmatrix}{}\frac{8}{7}\\\frac{10}{7}\\\frac{4}{7}\\\frac{4}{7}\end{bmatrix} =
\begin{bmatrix}{}-\frac{1}{7}\\\frac{4}{7}\\-\frac{4}{7}\\-\frac{4}{7}\end{bmatrix}
$$

$$ \|b - (q_1^{\mathbf{T}}b)q_1\| =
\sqrt{\left(-\frac{1}{7}\right)^2 + \left(\frac{4}{7}\right)^2 + \left(-\frac{4}{7}\right)^2 + \left(-\frac{4}{7}\right)^2} = 1
$$

$$ q_2 = \frac{1}{1}
\begin{bmatrix}{}-\frac{1}{7}\\\frac{4}{7}\\-\frac{4}{7}\\-\frac{4}{7}\end{bmatrix}
$$

Notice that $q_2 = b - p$.

17. Find the projection of $b$ onto the line through $a$:

$$ a = \begin{bmatrix}{}1\\1\\1\end{bmatrix} $$

and

$$ b = \begin{bmatrix}{}1\\3\\5\end{bmatrix} $$

and

$$ p = \text{?} $$

and

$$ e = b - p = \text{?} $$

Compute the orthonormal vectors $q_1 = \dfrac{a}{\|a\|}$ and
$q_2 = \dfrac{e}{\|e\|}$.

_Solution:_

$$ p = \frac{a^{\mathbf{T}}b}{a^{\mathbf{T}}a}a $$

$$ a^{\mathbf{T}}a =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\1\\1\end{bmatrix} = 3
$$

$$ a^{\mathbf{T}}b =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
\end{array}\right]
\begin{bmatrix}{}1\\3\\5\end{bmatrix} = 9
$$

$$ p = \frac{1}{3}(9)a = 3a =
3\begin{bmatrix}{}1\\1\\1\end{bmatrix} = \begin{bmatrix}{}3\\3\\3\end{bmatrix}
$$

$$ e = b - p =
\begin{bmatrix}{}1\\3\\5\end{bmatrix} - \begin{bmatrix}{}3\\3\\3\end{bmatrix} =
\begin{bmatrix}{}-2\\0\\2\end{bmatrix}
$$

$$ q_1 = \frac{a}{\|a\|} $$

$$ \|a\| = \sqrt{(1)^2 + (1)^2 + (1)^2} = \sqrt{3} $$

$$ q_1 = \frac{1}{\sqrt{3}}\begin{bmatrix}{}1\\1\\1\end{bmatrix} =
\begin{bmatrix}{}\frac{1}{\sqrt{3}}\\\frac{1}{\sqrt{3}}\\\frac{1}{\sqrt{3}}\end{bmatrix}
$$

$$ q_2 = \frac{e}{\|e\|} $$

$$ \|e\| = \sqrt{(-2)^2 + (0)^2 + (2)^2} = \sqrt{8} = 2\sqrt{2} $$

$$ q_2 = \frac{1}{2\sqrt{2}}\begin{bmatrix}{}-2\\0\\2\end{bmatrix} =
\begin{bmatrix}{}-\frac{1}{\sqrt{2}}\\0\\\frac{1}{\sqrt{2}}\end{bmatrix}
$$

(LEFT OFF HERE).

18. (Recommended) Find orthogonal vectors $A, B, C$ by Gram-Schmidt from
    $a, b, c$:

$$ a = (1, -1, 0, 0) \quad b = (0, 1, -1, 0) \quad c = (0, 0, 1, -1) $$

$A, B, C$ and $a, b, c$ are bases for the vectors perpendicular to
$d = (1, 1, 1, 1)$.

19. If $A = QR$ then $A^{\mathbf{T}}A = R^{\mathbf{T}}R =$ ____ triangular times
    ____ triangular. _Gram-Schmidt on $A$ corresponds to elimination on
    $A^{\mathbf{T}}A$_. The pivots for $A^{\mathbf{T}}A$ must be the squares of
    diagonal entries of $R$. Find $Q$ and $R$ by Gram-Schmidt for this $A$:

$$ A =
\left[\begin{array}{rr}
-1 & 1 \\
2 & 1 \\
2 & 4 \\
\end{array}\right]
$$

and

$$ A^{\mathbf{T}}A =
\left[\begin{array}{cc}
9 & 9 \\
9 & 18 \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 0 \\
1 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
9 & \\
& 9 \\
\end{array}\right]
\left[\begin{array}{cc}
1 & 1 \\
0 & 1 \\
\end{array}\right]
$$

20. True or false (give an example in either case):

a. $Q^{-1}$ is an orthogonal matrix when $Q$ is an orthogonal matrix.

b. If $Q$ ($3$ by $2$) has orthogonal columns then $\|Qx\|$ always equals
$\|x\|$.

21. Find an orthonormal basis for the column space of $A$:

$$ A =
\left[\begin{array}{rr}
1 & -2 \\
1 & 0 \\
1 & 1 \\
1 & 3 \\
\end{array}\right]
$$

and

$$ b =
\begin{bmatrix}{}-4\\-3\\3\\0\end{bmatrix}
$$

Then compute the projection of $b$ onto that column space.

22. Find orthogonal vectors $A, B, C$ by Gram-Schmidt from

$$ a = \begin{bmatrix}{}1\\1\\2\end{bmatrix} $$

and

$$ b = \begin{bmatrix}{}1\\-1\\0\end{bmatrix} $$

and

$$ c = \begin{bmatrix}{}1\\0\\4\end{bmatrix} $$

23. Find $q_1, q_2, q_3$ (orthonormal) as combinations of $a, b, c$ (independent
    columns). Then write $A$ as $QR$:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 4 \\
0 & 0 & 5 \\
0 & 3 & 6 \\
\end{array}\right]
$$

24.

a. Find a basis for the subspace $S$ in $\R^4$ spanned by all solutions of

$$ x_1 + x_2 + x_3 - x_4 = 0 $$

b. Find a basis for the orthogonal complement $S^{\perp}$.

c. Find $b_1$ in $S$ and $b_2$ in $S^{\perp}$ so that
$b_1 + b_2 = b = (1, 1, 1, 1)$.

25. If $ad - bc > 0$, the entries in $A = QR$ are

$$
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] =
\frac{
\left[\begin{array}{cc}
a & -c \\
c & a \\
\end{array}\right]
\left[\begin{array}{cc}
a^2 + c^2 & ab + cd \\
0 & ad - bc \\
\end{array}\right]
}{
\sqrt{a^2 + c^2} \quad
\sqrt{a^2 + c^2}
}
$$

Write $A = QR$ when $a, b, c, d = 2, 1, 1, 1$ and also $1, 1, 1, 1$. Which entry
of $R$ becomes zero when the columns are dependent and Gram-Schmidt breaks down?

**Problems 26-29 use the $QR$ code in equation (11). It executes Gram-Schmidt.**

26. Show why $C$ (found via $C^*$ in the steps after (11)) is equal to $C$ in
    equation (8).

27. Equation (8) subtracts from $c$ its components along $A$ and $B$. Why not
    subtract the components along $a$ and along $b$?

28. Where are the $mn^2$ multiplications in equation (11)?

29. Omitted (no MATLAB) .

**Problems 30-25 involve orthogonal matrices that are special.**

30. The first four _wavelets_ are in the columns of this wavelet matrix $W$:

$$ W =
\frac{1}{2}
\left[\begin{array}{rrrr}
1 & 1 & \sqrt{2} & 0 \\
1 & 1 & -\sqrt{2} & 0 \\
1 & -1 & 0 & \sqrt{2} \\
1 & -1 & 0 & -\sqrt{2} \\
\end{array}\right]
$$

What is special about the columns? Find the inverse wavelet transform $W^{-1}$.

31.

a. Choose $c$ so that $Q$ is an orthogonal matrix:

$$ Q =
c\left[\begin{array}{rrrr}
1 & -1 & -1 & -1 \\
-1 & 1 & -1 & -1 \\
-1 & -1 & 1 & -1 \\
-1 & -1 & -1 & 1 \\
\end{array}\right]
$$

Project $b = (1, 1, 1, 1)$ onto the first column. Then project $b$ onto the
plane of the first two columns.

32. If $u$ is a unit vector, then $Q = I - 2uu^{\mathbf{T}}$ is a reflection
    matrix (Example 3). Find $Q_1$ from $u = (0, 1)$ and $Q_2$ from
    $u = \left(0, \dfrac{\sqrt{2}}{2}, \dfrac{\sqrt{2}}{2}\right)$. Draw the
    reflections when $Q_1$ and $Q_2$ multiply the vectors $(1, 2)$ and
    $(1, 1, 1)$.

33. Find all matrices that are both orthogonal and lower triangular.

34. $Q = I - 2uu^{\mathbf{T}}$ is a reflection matrix when
    $u^{\mathbf{T}}u = 1$. Two reflections give $Q^2 = I$.

a. Show that $Qu = -u$. The mirror is perpendicular to $u$.

b. Find $Qv$ when $u^{\mathbf{T}}v = 0$. The mirror contains $v$. It reflects to
itself.
