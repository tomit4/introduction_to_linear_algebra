Page 265

## Problem Set 5.1

**Questions 1-12 are about the rules for determinants.**

1. If a $4$ by $4$ matrix has $\det A = \frac{1}{2}$, find $\det(2A)$ and
   $\det(-A)$ and $\det(A^2)$ and $\det(A^{-1})$.

_Solution:_

$$ \det A = \frac{1}{2} $$

Find $\det(2A)$:

$$ \det(2A) = \det(A + A) \neq \det(A) + \det(A) $$

$$ \det(2A) = 2^n \to \det(2A) = 2^4 = 16 $$

Find $\det(-A)$:

By rule 2, we can take any scalar $t$ out of each row of a matrix and multiply
it by the resulting determinant of the remaining matrix, which gives us the
overall determinant. Think on it this way:

$$ \det(-A) = \det(-1A) $$

Thus we are multiplying _every_ row by $-1$, and we can pull out a $-1$ _per
row_, this leaves us with:

$$ \det(-A) = (-1)^4(\det A) = 1\left(\frac{1}{2}\right) = \frac{1}{2} $$

Find $\det(A^2)$:

$$ \det(A^2) = \det(A \cdot A) = \det(A) \cdot \det(A) = \frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4} $$

Find $\det(A{-1})$:

$$ \det{A^{-1}} = \frac{1}{\det A} = \frac{1}{\dfrac{1}{2}} = 2 $$

2. If a $3$ by $3$ matrix has $\det A = -1$, find
   $\det\left(\dfrac{1}{2}A\right)$ and $\det(-A)$ and $\det(A^2)$ and
   $\det(A^{-1})$.

_Solution:_

Find $\det\left(\dfrac{1}{2}A\right)$:

$$ \det\left(\dfrac{1}{2}A\right) = \left(\frac{1}{2}\right)^3 \cdot \det(A) = \frac{1}{8} \cdot -1 = -\frac{1}{8} $$

Find $\det(-A)$:

$$ \det(-A) = (-1)^3 \cdot \det(A) = (-1) \cdot (-1) = 1 $$

Find $\det(A^2)$:

$$ \det(A^2) = \det(A \cdot A) = \det(A) \cdot \det(A) = (-1) \cdot (-1) = 1 $$

Find $\det(A^{-1})$:

$$ \det(A^{-1}) = \frac{1}{\det(A)} = \frac{1}{-1} = -1 $$

3. True or false, with a reason if true or a counterexample if false:

a. The determinant of $I + A$ is $1 + \det A$.

False, $\det(A + B) \neq \det(A) + \det(B)$

Consider:

$$ \det(I + I) \neq 1 + 1 $$

Except when $n = 1$.

b. The determinant of $ABC$ is $|A||B||C|$.

True. This is true by rule 9 (The determinant of $AB$ is $\det A$ _times_
$\det B$.

c. The determinant of $4A$ is $4|A|$.

False, the determinant of $4A$ is $4^n \cdot |A|$.

d. The determinant of $AB - BA$ is zero. Try an example with
$A =\left[\begin{array}{cc}0 & 0 \\0 & 1 \\\end{array}\right]$.

False, if we were to say that $|AB| - |BA| = 0$, this would more likely be
true(?).

Consider $B$ as a simple 2 by 2 permutation matrix:

$$ B =
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right]
$$

Then:

$$ AB =
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 0 \\
1 & 0 \\
\end{array}\right]
$$

$$ BA =
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right]
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right]
$$

$$ AB - BA =
\left[\begin{array}{cc}
0 & 0 \\
1 & 0 \\
\end{array}\right] -
\left[\begin{array}{cc}
0 & 1 \\
1 & 0 \\
\end{array}\right] =
\left[\begin{array}{rr}
0 & -1 \\
0 & 0 \\
\end{array}\right]
$$

$$ |AB - BA| = (0)(0) - (-1)(0) = 0 $$

This is odd. Strang's answer (which we use his $B$) here actually supports the
opposite of the claim that this is false. Moving on anyways.

Omitted.

4. Which row exchanges show that these "reverse identity matrices" $J_3$ and
   $J_4$ have $|J_3| = -1$ but $|J_4| = +1$?

$$
\det\left[\begin{array}{ccc}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right] = -1
$$

but

$$
\det\left[\begin{array}{cccc}
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0 \\
\end{array}\right] = +1
$$

_Solution:_

$J_3$ clearly switches rows 3 and 1, which is a single row exchange, by rule 2,
the determinant of the resulting matrix in this case would be $-1$.

$J_4$ exchanges rows 1 and 4, and also rows 2 and 3. This is 2 row exchanges,
and since the amount of row exchanges is _even_, the determinant is $1$.

5. For $n = 5, 6, 7$, count the row exchanges to permute the reverse identity
   $J_n$ to the identity matrix $I_n$. Propose a rule for every size $n$ and
   predict whether $J{101}$ has determinant $+1$ or $-1$.

_Solution:_

For $n = 5$:

Consider the $5$ by $5$ identity matrix:

$$ I_5 =
\left[\begin{array}{ccccc}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

To get the "reverse identity" matrix $J_5$, we'd need to exchange rows 1 and
rows 5, and also rows 2 and rows 4. This results in 2 row exchanges, which is an
even number of row exchanges, and thus by rule 2, $|J_5| = 1$.

For $n = 6$:

$$ I_6 =
\left[\begin{array}{cccccc}
1 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0\\
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Exchange rows 1 and 6, rows 2 and 5, rows 3 and 4. Three row exchanges, means
$|J_6| = -1$.

For $n = 7$:

$$ I_7 =
\left[\begin{array}{cccccc}
1 & 0 & 0 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Exchange rows 1 and 7, 2 and 6, 3 and 5. Three row exchanges, $|J_7| = -1$.

The determinants repeat the pattern of $1, 1, -1, -1$ in cycles of $4$. It
follows that the determinant of $|J{101}| = 1$.

Another way of thinking on this is $|J_n|$ is determined by
$\left\lfloor \dfrac{n}{2} \right\rfloor = 2k \to |J_n| = 1$, or
$\left\lfloor \dfrac{n}{2} \right\rfloor = 2k + 1 \to |J_n| = -1$, for some
$k \in \Z$.

6. Show how Rule 6 (determinant $= 0$ if a row is all zero) comes from Rule 3.

_Solution:_

Rule 3 states that the determinant is a linear function of each row separately.
This is demonstrated more generally by the following example:

$$
\begin{vmatrix}
ta & tb \\
c & d \\
\end{vmatrix} =
t\begin{vmatrix}
a & b \\
c & d \\
\end{vmatrix}
$$

Taking this example, consider what happens when a single row is all $0$'s:

$$
\begin{vmatrix}
(0)a & (0)b \\
c & d \\
\end{vmatrix} =
0\begin{vmatrix}
a & b \\
c & d \\
\end{vmatrix}
$$

Now, the determinant of whatever $ad - bc$ is will be multiplied by $0$, and
result in the final determinant being $0$, thereby demonstrating rule 6.

7. Find the determinants of rotations and reflections:

$$ Q =
\left[\begin{array}{rr}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{array}\right]
$$

and

$$ Q =
\left[\begin{array}{rr}
1 - 2\cos^2\theta & -2\cos\theta\sin\theta \\
-2\cos\theta\sin\theta & 1 - 2\sin^2\theta \\
\end{array}\right]
$$

_Solution:_

Rotations:

$$ Q =
\left[\begin{array}{rr}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{array}\right]
$$

$$ |Q| = (\cos\theta)(\cos\theta) - (-\sin\theta)(\sin\theta) $$

$$ |Q| = (\cos^2\theta) - (-\sin^2\theta) $$

$$ |Q| = \cos^2\theta + \sin^2\theta = 1 $$

Reflections:

$$ Q =
\left[\begin{array}{rr}
1 - 2\cos^2\theta & -2\cos\theta\sin\theta \\
-2\cos\theta\sin\theta & 1 - 2\sin^2\theta \\
\end{array}\right]
$$

$$ |Q| = (1 - 2\cos^2\theta)(1 - 2\sin^2\theta) - (-2\cos\theta\sin\theta)(-2\cos\theta\sin\theta) $$

$$ = (1 - 2\cos^2\theta - 2\sin^2\theta + 4\cos^2\theta\sin^2\theta) - (4\cos^2\theta\sin^2\theta) $$

$$ = 1 - 2\cos^2\theta - 2\sin^2\theta $$

$$ = 1 - 2(\cos^2\theta + \sin^2\theta) $$

$$ = 1 - 2(1) $$

$$ = -1 $$

8. Prove that every orthogonal matrix $(Q^{\mathbf{T}}Q = I)$ has determinant
   $1$ or $-1$.

a. Use the product rule $|AB| = |A||B|$ and the transpose rule
$|Q| = |Q^{\mathbf{T}}|$.

_Solution:_

**Proof:**

Suppose $Q$ is any orthogonal matrix.

It is to be demonstrated that $Q^{\mathbf{T}}Q = I$ has determinant equal to $1$
or $-1$.

By the product rule for determinants:

$$ |Q^{\mathbf{T}}Q| = |Q^{\mathbf{T}}||Q| $$

By the transpose rule:

$$ |Q^{\mathbf{T}}Q| = |Q^{\mathbf{T}}||Q| = |Q||Q| = |Q|^2 $$

Now, from the identity property of orthogonal matrices $Q^{\mathbf{T}}Q = I$, we
can say that:

$$ |Q^{\mathbf{T}}Q| = |I| $$

And thus we can also say that:

$$ |Q|^2 = |I| $$

Since $|I| = 1$, by substitution:

$$ |Q|^2 = 1 $$

Then, take the square root of both sides:

$$ \sqrt{|Q|^2} = \sqrt{1} $$

$$ |Q| = \pm 1 $$

This is what was to be demonstrated.

Q.E.D.

b. Use only the product rule. If $|\det Q| > 1$ then $\det Q^n = (\det A)^n$
blows up. How do you know this can't happen to $Q^n$?

_Solution:_

**Proof (by contradiction):**

Suppose $Q$ is any orthogonal matrix.

Then suppose $|\det Q| > 1$ (read as "the absolute value of the determinant of
$Q$ is greater than $1$").

A contradiction is to be derived to demonstrate that $|\det Q| \leq 1$.

By the product rule, this means that
$\det Q^n = (\det Q)(\det Q)(\det Q) \cdots$ until $n$ $\det Q$'s have been
multiplied, resulting in a product of $\det Q^n = (\det Q)^n$. And since we
start with $\det Q > 1$, this determinant grows exponentially.

Now, by the identity property of orthogonal matrices:

$$ Q^{\mathbf{T}}Q = I $$

And by the matrix property of invertible, this means that:

$$ Q^{-1}Q = I \Rightarrow Q^{\mathbf{T}} = Q^{-1} $$

This means that $Q$ is invertible, and it's columns are orthonormal unit
vectors.

By the definition of orthonormal unit vectors, this means that whenever $Q$ is
multiplied with itself, no matter how many times, the resulting product matrix's
determinant is bounded. In other words, the product of $Q$'s can only ever
rotate and/or reflect. This results in the determinant of $Q$ never growing.
This contradicts our findings by the product rule, which were derived by the
supposition.

Since a contradiction to the supposition has been demonstrated, it can be
concluded that the supposition is false, and therefore $|\det Q| \leq 1$.

Q.E.D.

9. Do these matrices have determinant $0, 1, 2$ or $3$?

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

_Solution:_

$|A|$:

$$ A =
\left[\begin{array}{ccc}
0 & 0 & 1 \\
1 & 0 & 0 \\
0 & 1 & 0 \\
\end{array}\right]
$$

This is just $I$ with a permutation matrix applied, (or it just simply is that
$P$). We can see that to return it to $I$, we would have to exchange rows 1 and
2, then rows 2 and 3. So 2 row exchanges are even, and thus $|A| = 1$.

$|B|$:

$$ B =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}\right]
$$

Here we can use the fact that $|B| = \text{the product of the pivots of } U$
after elimination.

$$ B =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right]
$$

Before moving on, mark the row swap, we had 1 row swap before proceeding with
standard elimination, thus we need to multiply our final answer by $-1$.

$$ \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & -1 & 1 \\
0 & 1 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 1 & 0 \\
0 & -1 & 1 \\
0 & 0 & 2 \\
\end{array}\right] = U
$$

Now, just multiply the pivots:

$$ (1)(-1)(2) = -2 $$

And multiply by $-1$ to account for our single row exchange:

$$ (-2)(-1) = 2 $$

$$ |B| = 2 $$

$|C|$:

$$ C =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 1 \\
1 & 1 & 1 \\
\end{array}\right]
$$

Here, it is obvious that the rows are dependent, and because of this $|C| = 0$.

10. If the entries in every row of $A$ add to zero, solve $Ax = \mathbf{0}$ to
    prove $\det A = 0$. If those entries add to one, show that
    $\det(A - I) = 0$. Does this mean $\det A = 1$?

_Solution:_

_If the entries in every row of $A$ add to zero, solve $Ax = \mathbf{0}$ to
prove $\det A = 0$:_

**Proof:**

Suppose $A$ is any matrix where every row of $A$, when summed together, adds to
$0$. If we then solve $Ax = \mathbf{0}$, we will find that the $1$'s vector
$(1, 1, \dots, 1) \in N(A)$. In other words, $N(A)$ does not contain only the
$\mathbf{0}$ vector. This demonstrates that $A$ is singular, and by that fact,
it can be concluded that $\det A = 0$.

Q.E.D.

_If those entries add to one, show that $\det(A - I) = 0$:_

**Proof:**

Suppose $A$ is any matrix whose rows, when summed together, add up to $1$.

Then, when we consider $A - I$, this means that the sum of all the rows of
$A - I$ sum to $0$.

By the previous proof, we can further conclude that $\det(A - I) = 0$.

Q.E.D.

_Does this mean $\det A = 1$?:_

No, this question is meant to reinforce that the general inequality holds:

$$ \det(A + B) \neq \det(A) + \det(B) $$

Just because $\det(A - I) = 0$ and the fact that $\det(I) = 1$, we cannot
necessarily conclude that $\det(A) = 1$. This conclusion does not necessarily
follow the logic of the previous proofs.

11. Suppose that $CD = -DC$ and find the flaw in this reasoning: Taking
    determinants gives $|C||D| = -|D||C|$. Therefore $|C| = 0$ or $|D| = 0$. One
    or both of the matrices must be singular. (That is not true.)

_Solution:_

Okay, so let's work through this informally.

We have:

$$ CD = -DC $$

Then, Strang demonstrates simply that:

$$ |C||D| = -|D||C| $$

Since the above equality holds. We can say, by algebra, that:

$$ |C||D| + |D||C| = 0 $$

And since determinants are just numbers, we can apply commutative and
associative laws to this equality. This evaluates to:

$$ 2|C||D| = 0 $$

Which means that:

$$ |C||D| = 0 $$

$$ |CD| = 0 $$

But this only means that the product $CD$ is singular, not necessarily that $C$
or $D$ is singular by themselves.

12. The inverse of a $2$ by $2$ matrix seems to have determinant $= 1$:

$$ \det A^{-1} =
\det \frac{1}{ad - bc}
\left[\begin{array}{rr}
d & -b \\
-c & a \\
\end{array}\right] =
\frac{ad - bc}{ad - bc} = 1
$$

What is wrong with this calculation? What is the correct $\det A^{-1}$?

_Solution:_

The flaw in the logic is a common mistake. Recall that when we apply some scalar
$t$ to a matrix, we can indeed multiply the resulting determinant by that scalar
_per row_. This emphasized, _per row_, is the key issue here. By evaluating the
given equation, we can see that we're simply applying:

$$ \frac{1}{ad - bc}(ad - bc) = \frac{ad - bc}{ad - bc} = 1 $$

But here we have 2 rows, each of which is multiplied by this scalar
$\dfrac{1}{ad - bc}$. Therefore, the correct equation to find the $\det(A^{-1})$
is to square this denominator (since there are $2$ rows):

$$ \det(A^{-1}) = \frac{ad - bc}{(ad - bc)^2} = \frac{1}{ad - bc} $$

Similar logic can be taken to disprove this equality from the simple fact that
we know that $\det(A^{-1}) = \dfrac{1}{\det A}$, which results in the same
finding.

**Questions 13-27 use the rules to compute specific determinants.**

13. Reduce $A$ to $U$ and find $\det A =$ product of the pivots:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 2 & 3 \\
3 & 3 & 3 \\
\end{array}\right]
$$

_Solution:_

First $A$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 2 & 2 \\
1 & 2 & 3 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
1 & 2 & 3 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 1 & 2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & 1 & 1 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{array}\right] = U
$$

$$ |A| = 1 \cdot 1 \cdot 1 = 1^3 = 1 $$

Second $A$:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
2 & 2 & 3 \\
3 & 3 & 3 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -2 & -3 \\
3 & 3 & 3 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -2 & -3 \\
0 & -3 & -6 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & 2 & 3 \\
0 & -2 & -3 \\
0 & 0 & -\frac{3}{2} \\
\end{array}\right] = U
$$

$$ |A| = 1 \cdot (-2) \cdot \left(-\frac{3}{2}\right) = 3 $$

14. By applying row operations to produce an upper triangular $U$, compute

$$
\det\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
2 & 6 & 6 & 1 \\
-1 & 0 & 0 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right]
$$

$$
\det\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
-1 & 2 & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

_Solution:_

For the sake of notational simplicity, denote each of these matrices as $A$.

First determinant:

$$ A =
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
2 & 6 & 6 & 1 \\
-1 & 0 & 0 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
-1 & 0 & 0 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
0 & 2 & 3 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
0 & 0 & 0 & 3 \\
0 & 2 & 0 & 7 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
0 & 2 & 0 & 7 \\
0 & 0 & 0 & 3 \\
\end{array}\right]
$$

Note our row exchange, here, we have 1 row exchange, so multiply $-1$ by the
final determinant.

$$ \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
0 & 0 & 0 & 6 \\
0 & 0 & 0 & 3 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
1 & 2 & 3 & 0 \\
0 & 2 & 0 & 1 \\
0 & 0 & 0 & 6 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

We get a $0$ row, thus $A$ is singular, and $\det(A) = 0$.

Second determinant:

$$ A =
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
-1 & 2 & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & -1 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & 0 & 2 & -1 \\
0 & 0 & -1 & 2 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{rrrr}
2 & -1 & 0 & 0 \\
0 & \frac{3}{2} & -1 & 0 \\
0 & 0 & 2 & -1 \\
0 & 0 & 0 & \frac{3}{2} \\
\end{array}\right]
$$

$$ |A| = 2\left(\frac{3}{2}\right)(2)\left(\frac{3}{2}\right) = 9 $$

15. Use row operations to simplify and compute these determinants:

$$
\det\left[\begin{array}{ccc}
101 & 201 & 301 \\
102 & 202 & 302 \\
103 & 203 & 303 \\
\end{array}\right]
$$

and

$$
\det\left[\begin{array}{ccc}
1 & t & t^2 \\
t & 1 & t \\
t^2 & t & 1 \\
\end{array}\right]
$$

_Solution:_

Again, denote each matrix $A$.

First determinant:

$$ A =
\left[\begin{array}{ccc}
101 & 201 & 301 \\
102 & 202 & 302 \\
103 & 203 & 303 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
101 & 201 & 301 \\
1 & 1 & 1 \\
103 & 203 & 303 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
101 & 201 & 301 \\
1 & 1 & 1 \\
2 & 2 & 2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
101 & 201 & 301 \\
1 & 1 & 1 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Thus $\det(A) = 0$ since $A$ is singular.

Second determinant:

$$ A =
\left[\begin{array}{ccc}
1 & t & t^2 \\
t & 1 & t \\
t^2 & t & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & t & t^2 \\
0 & 1 - t^2 & t - t^3 \\
t^2 & t & 1 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & t & t^2 \\
0 & 1 - t^2 & t - t^3 \\
0 & t - t^3 & 1 - t^4 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{ccc}
1 & t & t^2 \\
0 & 1 - t^2 & t - t^3 \\
0 & t(1 - t^2) & 1 - t^4 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & t & t^2 \\
0 & 1 - t^2 & t - t^3 \\
0 & 0 & 1 - t^2 \\
\end{array}\right] = U
$$

$$ |A| = 1(1 - t^2)(1 - t^2) = 1 - 2t^2 + t^4 $$

16. Find the determinants of a rank one matrix and a skew-symmetric matrix:

$$ A =
\begin{bmatrix}{}1\\2\\3\end{bmatrix}
\left[\begin{array}{rrr}
1 & -4 & 5 \\
\end{array}\right]
$$

and

$$ A =
\left[\begin{array}{rrr}
0 & 1 & 3 \\
-1 & 0 & 4 \\
-3 & -4 & 0 \\
\end{array}\right]
$$

_Solution:_

First $A$:

$$ A =
\begin{bmatrix}{}1\\2\\3\end{bmatrix}
\left[\begin{array}{rrr}
1 & -4 & 5 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & -4 & 5 \\
2 & -8 & 10 \\
3 & -12 & 15 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{rrr}
1 & -4 & 5 \\
2 & -8 & 10 \\
3 & -12 & 15 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
1 & -4 & 5 \\
0 & 0 & 0 \\
3 & -12 & 15 \\
\end{array}\right]
$$

Thus $\det(A) = 0$ since $A$ is singular.

Second $A$:

$$ A =
\left[\begin{array}{rrr}
0 & 1 & 3 \\
-1 & 0 & 4 \\
-3 & -4 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
-3 & -4 & 0 \\
0 & 1 & 3 \\
-1 & 0 & 4 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
-3 & -4 & 0 \\
-1 & 0 & 4 \\
0 & 1 & 3 \\
\end{array}\right] \to
$$

Note the two row exchanges, multiply $1$ on last determinant (do nothing).

$$ \to
\left[\begin{array}{rrr}
-3 & -4 & 0 \\
0 & \frac{4}{3} & 4 \\
0 & 1 & 3 \\
\end{array}\right] \to
\left[\begin{array}{rrr}
-3 & -4 & 0 \\
0 & \frac{4}{3} & 4 \\
0 & 0 & 0 \\
\end{array}\right]
$$

Thus $|A| = 0$ since $A$ is singular.

17. A skew-symmetric matrix has $A^{\mathbf{T}} = -A$. Insert $a, b, c$ for
    $1, 3, 4$ in Question 16 and show that $|A| = 0$. Write down a $4$ by $4$
    example with $|A| = 1$.

_Solution:_

_Insert $a, b, c$ for $1, 3, 4$ in Question 16 and show that $|A| = 0$:_

$$ A =
\left[\begin{array}{rrr}
0 & a & b \\
-a & 0 & c \\
-b & -c & 0 \\
\end{array}\right]
$$

Now, we establish that any skew-symmetric matrix has $A^{\mathbf{T}} = -A$. And
since we also know that $|A^{\mathbf{T}}| = |A|$, we can say that:

$$ |A| = |A^{\mathbf{T}}| = |-A| = (-1)^m|A| $$

The last part, with $(-1)^m|A|$ follows from $-A$. To get back $A$, we simply
take out a scalar $-1$ from _each row_. Then we multiply that by $|A|$ to get
our solution:

$$ |A| = |A^{\mathbf{T}}| = |-A| = (-1)^3|A| = -|A| $$

Since $|A| = -|A|$,it follows that:

$$ |A| = -|A| $$

$$ 2|A| = 0 $$

$$ |A| = 0 $$

_Write down a $4$ by $4$ example with $|A| = 1$:_

$$ A =
\left[\begin{array}{rrrr}
0 & 1 & 0 & 0 \\
-1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & -1 & 0 \\
\end{array}\right]
$$

$$ A =
\left[\begin{array}{rrrr}
0 & 1 & 0 & 0 \\
-1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & -1 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
-1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & -1 & 0 \\
\end{array}\right] \to
\left[\begin{array}{rrrr}
-1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right] = U
$$

Two row exchanges, so $1$ times last determinant (do nothing).

$$ |A| = (-1)(1)(-1)(1) = 1 $$

18. Use row operations to show that the $3$ by $3$ "Vandermonde determinant" is

$$
\det\left[\begin{array}{ccc}
1 & a & a^2 \\
1 & b & b^2 \\
1 & c & c^2 \\
\end{array}\right] = (b - a)(c - a)(c - b)
$$

_Solution:_

$$ A =
\left[\begin{array}{ccc}
1 & a & a^2 \\
1 & b & b^2 \\
1 & c & c^2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & a & a^2 \\
0 & b - a & b^2 - a^2 \\
1 & c & c^2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & a & a^2 \\
0 & b - a & b^2 - a^2 \\
0 & c - a & c^2 - a^2 \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{ccc}
1 & a & a^2 \\
0 & b - a & b^2 - a^2 \\
0 & c - a & c^2 - a^2 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
1 & a & a^2 \\
0 & b - a & b^2 - a^2 \\
0 & 0 & ? \\
\end{array}\right] \to \dots
$$

Evaluating:

$$ (c^2 - a^2) - \left(\frac{c - a}{b - a}\right)(b^2 - a^2) = ? $$

$$ (c^2 - a^2) - \left(\frac{(c - a)(b + a)(b - a)}{b - a}\right) = ? $$

$$ (c^2 - a^2) - (c - a)(b + a) = ? $$

$$ (c + a)(c - a) - (c - a)(b + a) = ? $$

$$ (c - a)((c + a) - (b + a)) = ? $$

$$ (c - a)(c + a - b - a) = ? $$

$$ (c - a)(c - b) = ? $$

$$ \to
\left[\begin{array}{ccc}
1 & a & a^2 \\
0 & b - a & b^2 - a^2 \\
0 & 0 & (c - a)(c - b) \\
\end{array}\right] \to \dots
$$

Thus $|A| = (1)(b - a)(c - a)(c - b) = (b - a)(c - a)(c - b)$.

19. Find the determinants of $U$ and $U^{-1}$ and $U^2$:

$$ U =
\left[\begin{array}{ccc}
1 & 4 & 6 \\
0 & 2 & 5 \\
0 & 0 & 3 \\
\end{array}\right]
$$

and

$$ U =
\left[\begin{array}{cc}
a & b \\
0 & d \\
\end{array}\right]
$$

_Solution:_

First $U$:

$$ U =
\left[\begin{array}{ccc}
1 & 4 & 6 \\
0 & 2 & 5 \\
0 & 0 & 3 \\
\end{array}\right]
$$

$$ |U| = (1)(2)(3) = 6 $$

$$ |U^{-1}| = \frac{1}{|U|} = \frac{1}{6} $$

$$ |U^2| = |U \cdot U| = |U||U| = (6)(6) = 36 $$

Second $U$:

$$ U =
\left[\begin{array}{cc}
a & b \\
0 & d \\
\end{array}\right]
$$

$$ |U| = (a)(d) = ad $$

$$ |U^{-1}| = \frac{1}{|U|} = \frac{1}{ad} $$

$$ |U^2| = |U \cdot U| = |U||U| = (ad)(ad) = a^2d^2 $$

20. Suppose you do two row operations at once, going from

$$
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right] \quad \text{ to } \quad
\left[\begin{array}{rr}
a - Lc & b - Ld \\
c - la & d - lb \\
\end{array}\right]
$$

Find the second determinant. Does it equal $ad - bc$?

_Solution:_

$$ |A| = (a - Lc)(d - lb) - (b - Ld)(c - la) $$

$$ = (ad - Ldc - lab + Llbc) - (bc - Ldc - lab + Llad) $$

$$ = ad - Ldc - lab + Llbc - bc + Ldc + lab - Llad $$

$$ = ad + Llbc - bc - Llad $$

$$ = ad - bc + Llbc - Llad $$

$$ = ad - bc + Ll(bc - ad) $$

$$ = ad - bc - Ll(ad - bc) $$

$$ = (ad - bc)(1 - Ll) \neq ad - bc $$

21. _Row exchange_: Add row $1$ of $A$ to row $2$, then subtract row $2$ from
    row $1$. Then add row $1$ to row $2$ and multiply row $1$ by $-1$ to reach
    $B$. Which rule show

$$
\det B =
\begin{vmatrix}
c & d \\
a & d \\
\end{vmatrix} \quad \text{equals} \quad
-\det A =
-\begin{vmatrix}
a & b \\
c & d \\
\end{vmatrix}\text{?}
$$

Those rules could replace Rule 2 in the definition of the determinant.

Omitted.

22. From $ad - bc$, find the determinants of $A$ and $A^{-1}$ and
    $A - \lambda I$:

$$ A =
\left[\begin{array}{cc}
2 & 1 \\
1 & 2 \\
\end{array}\right]
$$

and

$$ A^{-1} =
\frac{1}{3}
\left[\begin{array}{rr}
2 & -1 \\
-1 & 2 \\
\end{array}\right]
$$

and

$$ A - \lambda I =
\left[\begin{array}{cc}
2 - \lambda & 1 \\
1 & 2 - \lambda \\
\end{array}\right]
$$

Which two numbers $\lambda$ to $\det(A - \lambda I) = 0$? Write down the matrix
$A - \lambda I$ for each of those numbers $\lambda$ - it should not be
invertible.

_Solution:_

For $A$:

$$ A =
\left[\begin{array}{cc}
2 & 1 \\
1 & 2 \\
\end{array}\right]
$$

$$ |A| = (2)(2) - (1)(1) = 4 - 1 = 3 $$

For $A^{-1}$:

$$ A^{-1} =
\frac{1}{3}
\left[\begin{array}{rr}
2 & -1 \\
-1 & 2 \\
\end{array}\right]
$$

$$ |A^{-1}| = \frac{1}{|A|} = \frac{1}{3} $$

For $A - \lambda I$:

$$ A - \lambda I =
\left[\begin{array}{cc}
2 - \lambda & 1 \\
1 & 2 - \lambda \\
\end{array}\right]
$$

$$ |A - \lambda I| = (2 - \lambda)(2 - \lambda) - (1)(1) $$

$$ = (4 - 4\lambda + \lambda^2) - 1 $$

$$ = 3 - 4\lambda + \lambda^2 $$

_Which two numbers $\lambda$ to $\det(A - \lambda I) = 0$?:_

$$ \lambda^2 - 4\lambda + 3 = 0 $$

$$ (\lambda - 3)(\lambda - 1) = 0 $$

$$ \lambda = 3, 1 $$

_Write down the matrix $A - \lambda I$ for each of those numbers $\lambda$ - it
should not be invertible:_

$$ A - \lambda I =
\left[\begin{array}{cc}
2 - (3) & 1 \\
1 & 2 - (3) \\
\end{array}\right] =
\left[\begin{array}{cc}
-1 & 1 \\
1 & -1 \\
\end{array}\right] \to \det(A - \lambda I) = 0
$$

$$ A - \lambda I =
\left[\begin{array}{cc}
2 - (1) & 1 \\
1 & 2 - (1) \\
\end{array}\right] =
\left[\begin{array}{cc}
1 & 1 \\
1 & 1 \\
\end{array}\right] \to \det(A - \lambda I) = 0
$$

23. From $A = \left[\begin{array}{cc}4 & 1 \\2 & 3 \\\end{array}\right]$ find
    $A^2$ and $A^{-1}$ and $A - \lambda I$ and their determinants. Which two
    numbers $\lambda$ lead to $\det(A - \lambda I) = 0$?

_Solution:_

$$ A^2 =
\left[\begin{array}{cc}
4 & 1 \\
2 & 3 \\
\end{array}\right]
\left[\begin{array}{cc}
4 & 1 \\
2 & 3 \\
\end{array}\right] =
\left[\begin{array}{cc}
18 & 7 \\
14 & 11 \\
\end{array}\right]
$$

$$ |A^2| = (18)(11) - (7)(14) = 198 - 98 = 100 $$

Find $A^{-1}$ by Gauss-Jordan:

$$
\left[\begin{array}{rr|rr}
4 & 1 & 1 & 0 \\
2 & 3 & 0 & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
4 & 1 & 1 & 0 \\
0 & \frac{5}{2} & -\frac{1}{2} & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
1 & \frac{1}{4} & \frac{1}{4} & 0 \\
0 & \frac{5}{2} & -\frac{1}{2} & 1 \\
\end{array}\right] \to
\left[\begin{array}{rr|rr}
1 & \frac{1}{4} & \frac{1}{4} & 0 \\
0 & 1 & -\frac{1}{5} & \frac{2}{5} \\
\end{array}\right] \to
$$

$$ \to
\left[\begin{array}{rr|rr}
1 & 0 & \frac{3}{10} & -\frac{1}{10} \\
0 & 1 & -\frac{1}{5} & \frac{2}{5} \\
\end{array}\right]
$$

$$ A^{-1} =
\left[\begin{array}{rr}
\frac{3}{10} & -\frac{1}{10} \\
-\frac{1}{5} & \frac{2}{5} \\
\end{array}\right]
$$

$$ |A^{-1}| = \left(\frac{3}{10}\right)\left(\frac{2}{5}\right) - \left(-\frac{1}{10}\right)\left(-\frac{1}{5}\right) = \frac{1}{10} $$

$$ A - \lambda I =
\left[\begin{array}{cc}
4 & 1 \\
2 & 3 \\
\end{array}\right] -
\left[\begin{array}{cc}
\lambda & 0 \\
0 & \lambda \\
\end{array}\right] =
\left[\begin{array}{cc}
4 - \lambda & 1 \\
2 & 3 - \lambda \\
\end{array}\right]
$$

$$ |A - \lambda I| = (4 - \lambda)(3 - \lambda) - (1)(2) $$

$$ |A - \lambda I| = 12 - 7\lambda + \lambda^2 - 2 $$

$$ |A - \lambda I| = \lambda^2 - 7\lambda + 10 $$

_Which two numbers $\lambda$ lead to $\det(A - \lambda I) = 0$?:_

$$ \lambda^2 - 7\lambda + 10 = 0 $$

$$ (\lambda - 5)(\lambda - 2) = 0 $$

$$ \lambda = 5, 2 \to |A - \lambda I| = 0 $$

24. Elimination reduces $A$ to $U$. Then $A = LU$:

$$ A =
\left[\begin{array}{rrr}
3 & 3 & 4 \\
6 & 8 & 7 \\
-3 & 5 & -9 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
2 & 1 & 0 \\
-1 & 4 & 1 \\
\end{array}\right]
\left[\begin{array}{rrr}
3 & 3 & 4 \\
0 & 2 & -1 \\
0 & 0 & -1 \\
\end{array}\right] = LU
$$

Find the determinants of $L, U, A, U^{-1}, L^{-1}$, and $U^{-1}L^{-1}A$.

_Solution:_

$\det L$:

$$ |L| = (1)(1)(1) = 1 $$

$\det U$:

$$ |U| = (3)(2)(-1) = -6 $$

$\det A$:

Since no row exchanges are necessary to find $U$ from $A$, we can determine
that:

$$ |A| = |U| = -6 $$

$\det U^{-1}$:

$$ |U^{-1}| = \frac{1}{|U|} = -\frac{1}{6} $$

$\det L^{-1}$:

$$ |L^{-1}| = \frac{1}{|L|} = \frac{1}{1} = 1 $$

$\det U^{-1}L^{-1}A$:

$$ |U^{-1}L^{-1}A| = |U^{-1}||L^{-1}||A| = \left(-\frac{1}{6}\right)(1)(-6) = 1 $$

25. If the $i, j$ entry of $A$ is $i$ times $j$, show that $\det A = 0$.
    (Exception when $A = [1]$.)

_Solution:_

When every $i, j$ entry of $A$ is $i \cdot j$, this means that every row is
dependent. It follows that $A$ is singular, and therefore $\det A = 0$.

26. If the $i, j$ entry of $A$ is $i + j$, show that $\det A = 0$. (Exception
    when $n = 1$ or $2$.)

_Solution:_

Again, when every $i, j$ entry of $A$ is $i + j$, this also means that every row
is dependent. The same logic applies, and therefore $\det A = 0$.

Both 25 and 26 are Strang demonstrating that when any $i, j$ entry creates a
linear combination of $i$ and $j$, that the rows are dependent, the matrix is
singular, and therefore the determinant is zero.

27. Compute the determinants of these matrices by row operations:

$$ A =
\left[\begin{array}{ccc}
0 & a & 0 \\
0 & 0 & b \\
c & 0 & 0 \\
\end{array}\right]
$$

and

$$ B =
\left[\begin{array}{cccc}
0 & a & 0 & 0 \\
0 & 0 & b & 0 \\
0 & 0 & 0 & c \\
d & 0 & 0 & 0 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
a & a & a \\
a & b & b \\
a & b & c \\
\end{array}\right]
$$

_Solution:_

For $A$:

$$ A =
\left[\begin{array}{ccc}
0 & a & 0 \\
0 & 0 & b \\
c & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
c & 0 & 0 \\
0 & 0 & b \\
0 & a & 0 \\
\end{array}\right] \to
\left[\begin{array}{ccc}
c & 0 & 0 \\
0 & a & 0 \\
0 & 0 & b \\
\end{array}\right]
$$

After 2 row exchanges, (multiply last determinant by 1 since 2 is even, i.e. do
nothing).

The matrix $A$ is already in $LU$ form, so:

$$ |A| = cab $$

For $B$:

$$ B =
\left[\begin{array}{cccc}
0 & a & 0 & 0 \\
0 & 0 & b & 0 \\
0 & 0 & 0 & c \\
d & 0 & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cccc}
d & 0 & 0 & 0 \\
0 & 0 & b & 0 \\
0 & 0 & 0 & c \\
0 & a & 0 & 0 \\
\end{array}\right] \to
\left[\begin{array}{cccc}
d & 0 & 0 & 0 \\
0 & a & 0 & 0 \\
0 & 0 & 0 & c \\
0 & 0 & b & 0 \\
\end{array}\right] \to
\left[\begin{array}{cccc}
d & 0 & 0 & 0 \\
0 & a & 0 & 0 \\
0 & 0 & b & 0 \\
0 & 0 & 0 & c \\
\end{array}\right]
$$

So we have 3 row exchanges ($-1$ times the last determinant).

The matrix $B$ is already in $LU$ form, so:

$$ |B| = -1(dabc) = -dabc $$

For $C$:

$$ C =
\left[\begin{array}{ccc}
a & a & a \\
a & b & b \\
a & b & c \\
\end{array}\right] \to
\left[\begin{array}{ccc}
a & a & a \\
0 & b - a & b - a \\
a & b & c \\
\end{array}\right] \to
\left[\begin{array}{ccc}
a & a & a \\
0 & b - a & b - a \\
0 & b - a & c - a \\
\end{array}\right]
$$

$$ \to
\left[\begin{array}{ccc}
a & a & a \\
0 & b - a & b - a \\
0 & 0 & (c - a) - (b - a) \\
\end{array}\right] \to
\left[\begin{array}{ccc}
a & a & a \\
0 & b - a & b - a \\
0 & 0 & c - a - b + a \\
\end{array}\right] \to
\left[\begin{array}{ccc}
a & a & a \\
0 & b - a & b - a \\
0 & 0 & c - b\\
\end{array}\right] = U
$$

No row exchanges, so just compute $|C|$:

$$ |C| = (a)(b - a)(c - b) $$

28. True or false (give a reason if true or a $2$ by $2$ example if false):

a. If $A$ is not invertible then $AB$ is not invertible.

This is true.

Since $A$ is not invertible, this means that $|A| = 0$.

Then:

$$ |AB| = |A||B| = 0|B| = 0 $$

b. The determinant of $A$ is always the product of its pivots.

False, if an odd number of row exchanges occurs during the elimination of $A$ to
find its pivots, then the determinant is $-1(\text{the product of its pivots})$.

c. The determinant of $A - B$ equals $\det A - \det B$.

False, this has been demonstrated multiple times, but consider $A = 2I, B = I$,
then $2I - I = I$, and $\det(2I - I) = \det(I) = 1$. But
$\det 2I - \det I = (2)(2)(2) - 1 = 8 - 1 = 7$, and $7 \neq 1$.

d. $AB$ and $BA$ have the same determinant.

True, by the commutative law of numbers, $|AB| = |A||B| = |B||A| = |BA|$.

29. What is wrong with this proof that projection matrices have $\det P = 1$?

$$ P = A(A^{\mathbf{T}}A)^{-1}A^{\mathbf{T}} \quad \text{so} \quad |P| = |A|\frac{1}{|A^{\mathbf{T}}||A|}|A^{\mathbf{T}}| = 1 $$

_Solution:_

This proof looks sound, but this would only be true if $A$ is square. If $A$ is
rectangular, then $\det(A^{\mathbf{T}}A) \neq \det(A^{\mathbf{T}})\det(A)$.

30. (Calculus question) Show that the partial derivatives of $\ln(\det A)$ give
    $A^{-1}$!

$$ f(a, b, c, d) = \ln(ad - bc) \quad \text{leads to} \quad
\left[\begin{array}{cc}
\frac{\partial f}{\partial a} & \frac{\partial f}{\partial c} \\
\frac{\partial f}{\partial b} & \frac{\partial f}{\partial d} \\
\end{array}\right] = A^{-1}
$$

Omitted.

31. Omitted (no MATLAB).

32. Omitted (no MATLAB).

33. Omitted (no MATLAB).

34. If you know that $\det A = 6$, what is the determinant of $B$?

$$ \text{From }
\det A =
\begin{vmatrix}
\text{row } 1 \\
\text{row } 2 \\
\text{row } 3 \\
\end{vmatrix} = 6 \text{ find } \det B =
\begin{vmatrix}
\text{row } 3 + \text{row } 2 + \text{row } 1 \\
\text{row } 2 + \text{row } 1 \\
\text{row } 1 \\
\end{vmatrix}
$$

_Solution:_

Consider that we can reduce $B$ as follows:

$$ B =
\left[\begin{array}{c}
\text{row } 3 + \text{row } 2 + \text{row } 1\\
\text{row } 2 + \text{row } 1\\
\text{row } 1\\
\end{array}\right] \to
\left[\begin{array}{c}
\text{row } 1\\
\text{row } 2 + \text{row } 1\\
\text{row } 3 + \text{row } 2 + \text{row } 1\\
\end{array}\right]
$$

We have only had to do $1$ row exchange (multiply final determinant by $-1$),
now try to get this to be $A$:

$$ \to
\left[\begin{array}{c}
\text{row } 1\\
\text{row } 2 + \text{row } 1\\
\text{row } 3 + \text{row } 2 + \text{row } 1 - (\text{row } 2 + \text{row } 1) \\
\end{array}\right] \to
\left[\begin{array}{c}
\text{row } 1\\
\text{row } 2 + \text{row } 1\\
\text{row } 3 \\
\end{array}\right] \to
\left[\begin{array}{c}
\text{row } 1\\
\text{row } 2 + \text{row } 1 - (\text{row } 1) \\
\text{row } 3 \\
\end{array}\right] \to
$$

$$ \to
\left[\begin{array}{c}
\text{row } 1\\
\text{row } 2 \\
\text{row } 3 \\
\end{array}\right] = A
$$

Since we get to $A$ by elimination and a single row exchange, we can conclude
that $\det B = -\det A$, and thus $\det B = -6$.
