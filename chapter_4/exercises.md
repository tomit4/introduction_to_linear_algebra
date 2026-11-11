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
$P^{\mathbf{T}} = P$.

(LEFT OFF HERE)

21. Multiply the matrix $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ by itself.
    Cancel to prove that $P^2 = P$. Explain why $P(Pb)$ always equals $Pb$: The
    vector $Pb$ is in the column space of $A$ so its projection onto that column
    space is ____.

22. Prove that $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ is symmetric by
    computing $P^{\mathbf{T}}$. Remember that the inverse of a symmetric matrix
    is symmetric.

23. If $A$ is square and invertible, the warning against splitting
    $(A^{\mathbf{T}}A)^{-1}$ does not apply. Is it true that
    $AA^{-1}(A^{\mathbf{T}})^{-1}A^{\mathbf{T}} = I$. _When $A$ is invertible,
    why is $P = I$_? _What is the error $e$?_

24. The nullspace of $A^{\mathbf{T}}$ is ____ to the column space $C(A)$. So if
    $A^{\mathbf{T}}b = \mathbf{0}$, the projection of $b$ onto $C(A)$ should be
    $p =$ ____. Check that $P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}}$ gives
    this answer.

25. The projection matrix $P$ onto an $n$-dimensional subspace of $\R^m$ has
    rank $r = n$. _Reason:_ The projections $Pb$ fill the subspace $S$. So $S$
    is the ____ of $P$.

26. If an $m$ by $m$ matrix has $A^2 = A$ and its rank is $m$, prove that
    $A = I$.

27. The important fact that ends the section is this: _If
    $A^{\mathbf{T}}Ax = \mathbf{0}$ then $Ax = \mathbf{0}$_. _New Proof_: The
    vector $Ax$ is in the nullspace of ____. $Ax$ is always in the column space
    of ____. To be in both of those perpendicular spaces, $Ax$ must be zero.

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

29. If $B$ has rank $m$ (full row rank, independent rows) show that
    $BB^{\mathbf{T}}$ is invertible.
