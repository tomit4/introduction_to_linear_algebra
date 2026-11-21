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

---

## Problem Set 5.2

**Problems 1-10 use the big formula with $n!$ terms:
$|A| = \sum\pm a_{1\alpha}a_{2\beta} \cdots a_{n\omega}$. Every term uses each
row and each column once.**

1. Compute the determinants of $A, B, C$ from six terms. Are their rows
   independent?

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
3 & 1 & 2 \\
3 & 2 & 1 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 4 & 4 \\
5 & 6 & 7 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

_Solution:_

For $A$:

$$ A =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
3 & 1 & 2 \\
3 & 2 & 1 \\
\end{array}\right]
$$

$$ |A| = (+1)[(1)(1)(1)] + (-1)[(1)(2)(2)] + (-1)[(2)(3)(1)] + (+1)[(2)(2)(3)] + (+1)[(3)(3)(2)] + (-1)[(3)(1)(3)] = 12 $$

Rows are independent.

For $B$:

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 4 & 4 \\
5 & 6 & 7 \\
\end{array}\right]
$$

$$ |B| = (+1)[(1)(4)(7)] + (-1)[(1)(4)(6)] + (-1)[(2)(4)(7)] + (+1)[(2)(4)(5)] + (+1)[(3)(4)(6)] + (-1)[(3)(4)(5)] = 0 $$

The rows are dependent (you can also see that row 3 is the sum of row 1 + row
2).

For $C$:

$$ C =
\left[\begin{array}{ccc}
1 & 1 & 1 \\
1 & 1 & 0 \\
1 & 0 & 0 \\
\end{array}\right]
$$

$$ |C| = (+1)[(1)(1)(0)] + (-1)[(1)(0)(0)] + (-1)[(1)(1)(0)] + (+1)[(1)(0)(1)] + (+1)[(1)(1)(0)] + (-1)[(1)(1)(1)] = -1 $$

Rows are independent. Notice that you can omit all but the last term as the rest
contain $0$'s.

2. Compute the determinants of $A, B, C, D$. Are their columns independent?

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 \\
\end{array}\right]
$$

$$ C =
\left[\begin{array}{cc}
A & 0 \\
0 & A \\
\end{array}\right]
$$

$$ D =
\left[\begin{array}{cc}
A & 0 \\
0 & B \\
\end{array}\right]
$$

_Solution:_

For $A$:

$$ A =
\left[\begin{array}{ccc}
1 & 1 & 0 \\
1 & 0 & 1 \\
0 & 1 & 1 \\
\end{array}\right]
$$

$$ A = (-1)[(1)(1)(1)] + (-1)[(1)(1)(1)] = -2 $$

Here, notice we omitted multiplications that had a $0$ in it.

$A$ is linearly independent.

For $B$:

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 \\
\end{array}\right]
$$

$$ |B| = (+1)[(1)(5)(9)] + (-1)[(1)(6)(8)] + (-1)[(2)(4)(9)] + (+1)[(2)(6)(7)] + (+1)[(3)(4)(8)] + (-1)[(3)(5)(7)] = 0 $$

The columns of $B$ are dependent.

For $C$:

$$ C =
\left[\begin{array}{cc}
A & 0 \\
0 & A \\
\end{array}\right]
$$

$$ |C| = (+1)[|A||A|] + (-1)[(0)(0)] = 4 $$

Independent.

For $D$:

$$ D =
\left[\begin{array}{cc}
A & 0 \\
0 & B \\
\end{array}\right]
$$

$$ |D| = (+1)[|A||B|] = 0 $$

Dependent.

3. Show that $\det A = 0$, regardless of the five nonzeros marked by $x$'s:

$$ A =
\left[\begin{array}{ccc}
x & x & x \\
0 & 0 & x \\
0 & 0 & x \\
\end{array}\right]
$$

What are the cofactors of row $1$?

What is the rank of $A$?

What are the $6$ terms in $\det A$?

_Solution:_

_What are the cofactors of row $1$?:_

$$
C_{11} = (+1)[0x] + (-1)[x0] = 0 \\
C_{12} = (-1)[0x] + (+1)[x0] = 0 \\
C_{13} = (+1)[00] + (-1)[00] = 0 \\
$$

_What is the rank of $A$?:_

$$ r = 2 $$

_What are the $6$ terms in $\det A$?:_

All $6$ terms in $\det A$ are $0$.

4. Find two ways to choose nonzeros from four different rows and columns:

$$ A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 1 \\
0 & 1 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 0 & 0 & 1 \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{cccc}
1 & 0 & 0 & 2 \\
0 & 3 & 4 & 5 \\
5 & 4 & 0 & 3 \\
2 & 0 & 0 & 1 \\
\end{array}\right]
$$

($B$ has the same zeros as $A$).

Is $\det A$ equal to $1 + 1$ or $1 - 1$ or $-1 - 1$? What is $\det B$?

_Solution:_

For four different rows, you can choose $a_{11}a_{23}a_{32}a_{44}$. This takes
one row exchange, so the determinant of this choice is $-1[(1)(1)(1)(1)] = -1$.

For columns, you can choose $a_{14}a_{23}a_{32}a_{11}$. This takes two row
exchanges, so the determinant of this choice is $+1$.

The
$\det A = |a_{11}a_{23}a_{32}a_{44}| + |a_{14}a_{23}a_{32}a_{11}| = (-1) + 1 = 0$.

The $\det B = (-1)[(1)(4)(4)(1)] + (+1)[(2)(4)(4)(2)] = 48 $$

Notice that despite the $0$'s being in the same place for both $A$ and $B$ does
_not_ mean that $|A| = |B|$.

5. Place the smallest number of zeros in a $4$ by $4$ matrix that will guarantee
   $\det A = 0$. Place as many zeros as possible while still allowing
   $\det A \neq 0$.

_Solution:_

_Place the smallest number of zeros in a $4$ by $4$ matrix that will guarantee
$\det A = 0$:_

$$ A =
\left[\begin{array}{cccc}
1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 \\
1 & 1 & 1 & 1 \\
0 & 0 & 0 & 0 \\
\end{array}\right]
$$

Simply having a row of $0$'s (4 $0$'s) will guarantee the determinant is $0$
(you could also have a column of $0$'s).

_Place as many zeros as possible while still allowing $\det A \neq 0$:_

$$ A =
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Notice that this is just $I$, but this is the most amount of $0$'s allowed
($16 - 4 = 12$) while still having $\det A \neq 0$.

6.

a. If $a_{11} = a_{22} = a_{33} = 0$, how many of the six terms in $\det A$ will
be zero?

$4$. Visualize it mentally, if we have $0$'s along the diagonal and fill the
rest with $1$'s, the six terms with non-zero values will be all multiples along
the opposite diagonals, with exception of $a_{11}a_{23}a_{32}$ since
$a_{11} = 0$.

$$ A =
\left[\begin{array}{ccc}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}\right]
$$

$$
a_{11}a_{22}a_{33} = 0 \\
a_{11}a_{23}a_{32} = 0 \\
a_{12}a_{21}a_{33} = 0 \\
a_{12}a_{23}a_{31} = 1 \\
a_{13}a_{21}a_{32} = 1 \\
a_{13}a_{22}a_{31} = 0 \\
$$

b. If $a_{11} = a_{22} = a_{33} = a_{44} = 0$, how many of the $24$ products
$a_{1j}a_{2k}a_{3l}a_{4m}$ are sure to be zero?

Just visualize this one to help:

$$ A =
\left[\begin{array}{cccc}
0 & 1 & 1 & 1 \\
1 & 0 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 0 \\
\end{array}\right]
$$

For sake of expediency, the answer is $24 - 9 = 15$.

There is a general derangement formula that will give you this, but is beyond
the scope of this chapter:

$$ D_n = n!\sum_{k = 0}^{n}{\frac{(-1)^{k}}{k!}} $$

7. How many $5$ by $5$ permutation matrices have $\det P = +1$? Those are even
   permutations. Find one that needs four exchanges to reach the identity
   matrix.

_Solution:_

_How many $5$ by $5$ permutation matrices have $\det P = +1$?:_

There are $\frac{5!}{2} = 60$ 5 by 5 permutation matrices that have
$\det P = +1$.

_Find one that needs four exchanges to reach the identity matrix:_

$$ P =
\left[\begin{array}{ccccc}
0 & 0 & 0 & 1 & 0 \\
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 \\
\end{array}\right]
$$

8. If $\det A$ is not zero, at least one of the $n!$ terms in formula (8) is not
   zero. Deduce from the big formula that some ordering of the rows of $A$
   leaves no zeros on the diagonal. (Don't use $P$ from elimination; that $PA$
   can have zeros on the diagonal.)

_Solution:_

The big formula is:

$$ \sum(\det P)a_{1\alpha}a_{2\beta} \cdots a_{n \omega} $$

It follows that at least one of the $n!$ terms of the above summation is not $0$
if $\det A \neq 0$. Via permutation (row exchanges), it makes sense that we can
move rows $1, 2, \dots, n$ to rows $\alpha, \beta, \dots, \omega$ until there
are no $0$'s along the main diagonal if $\det A \neq 0$.

9. Show that $4$ is the largest determinant for a $3$ by $3$ matrix of $1$'s and
   $-1$'s.

_Solution:_

We know there are $3! = 6$ possible permutations from 3 by 3 matrix. Let $q$ be
the number of $-1$ terms in the Big Formula and $6 - q$ $1$ terms. Then the
$\det A = q + 6 - q = 6 = \text{even}$, so any non-even determinant is not
possible, and $\det A = 6$ is also not possible since not all permutations are
even nor are all permutations odd. If $3$ permutations are odd, and $3$
permutations are even, if this $A$ had all $1$'s or all $-1$'s, the determinant
would be $0$. Thus it follows that the maximum determinant must be $4$.

10. How many permutations of $(1, 2, 3, 4)$ are even and what are they? Extra
    credit: What are all the possible $4$ by $4$ determinants of
    $I + P_{\text{even}}$?

_Solution:_

_How many permutations of $(1, 2, 3, 4)$ are even and what are they?:_

There are $\frac{4!}{2} = 12$ even permutations.

$$ (1, 2, 3, 4), (4, 3, 2, 1), (3, 1, 4, 2), (2, 1, 4, 3) $$

and $8$ other permutations where one number stays in place.

**Problems 11-22 use cofactors $C_{ij} = (-1)^{i + j}\det M_{ij}$. Remove row
$i$ and column $j$.**

11. Find all cofactors and put them into cofactor matrices $C, D$. Find $AC$ and
    $\det B$.

$$ A =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
$$

$$ B =
\left[\begin{array}{ccc}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 0 & 0 \\
\end{array}\right]
$$

_Solution:_

First let's find $C$ from $A$:

$$
C_{11} = (-1)^{1 + 1}\det([d]) = 1 \cdot |d| = |d| = d \\
C_{12} = (-1)^{1 + 2}\det([c]) = (-1) \cdot |c| = -c \\
C_{21} = (-1)^{2 + 1}\det([b]) = (-1) \cdot |b| = -b \\
C_{22} = (-1)^{2 + 2}\det([a]) = (1) \cdot |a| = a \\
$$

Now assemble cofactor matrix $C$:

$$ C =
\left[\begin{array}{rr}
d & -c \\
-b & a \\
\end{array}\right]
$$

Now find $AC$:

$$ AC =
\left[\begin{array}{cc}
a & b \\
c & d \\
\end{array}\right]
\left[\begin{array}{rr}
d & -c \\
-b & a \\
\end{array}\right] =
\left[\begin{array}{cc}
ad - b^2 & ba - ac \\
cd - db & ad - c^2 \\
\end{array}\right]
$$

Now define $D$ from $B$:

$$
D_{11} = (-1)^{1 + 1}\det\left[\begin{array}{cc}5 & 6 \\0 & 0 \\\end{array}\right] = 1 \cdot 0 = 0 \\
D_{12} = (-1)^{1 + 2}\det\left[\begin{array}{cc}4 & 6 \\7 & 0 \\\end{array}\right] = (-1) \cdot (-42) = 42 \\
D_{13} = (-1)^{1 + 3}\det\left[\begin{array}{cc}4 & 5 \\7 & 0 \\\end{array}\right] = 1 \cdot (-35) = -35 \\
D_{21} = (-1)^{2 + 1}\det\left[\begin{array}{cc}2 & 3 \\0 & 0 \\\end{array}\right] = (-1) \cdot 0 = 0 \\
D_{22} = (-1)^{2 + 2}\det\left[\begin{array}{cc}1 & 3 \\7 & 0 \\\end{array}\right] = 1 \cdot (-21) = -21 \\
D_{23} = (-1)^{2 + 3}\det\left[\begin{array}{cc}1 & 2 \\7 & 0 \\\end{array}\right] = (-1) \cdot (-14) = 14 \\
D_{31} = (-1)^{3 + 1}\det\left[\begin{array}{cc}2 & 3 \\5 & 6 \\\end{array}\right] = 1 \cdot (-3) = -3 \\
D_{32} = (-1)^{3 + 2}\det\left[\begin{array}{cc}1 & 3 \\4 & 6 \\\end{array}\right] = (-1) \cdot (-6) = 6 \\
D_{33} = (-1)^{3 + 3}\det\left[\begin{array}{cc}1 & 2 \\4 & 5 \\\end{array}\right] = 1 \cdot (-3) = -3 \\
$$

So cofactor matrix $D$ is:

$$ D =
\left[\begin{array}{rrr}
0 & 42 & -35 \\
0 & -21 & 14 \\
-3 & 6 & -3 \\
\end{array}\right]
$$

Now find $\det B$:

$$ \det B = b_{i1}D_{i1} + b_{i2}D_{i2} + \cdots + b_{in}D_{in} $$

so:

$$ \det B = (1)(0) + (2)(42) + (3)(-35) = -21 $$

You can use any row, but only one row to evaluate $\det B$. Note here that the
reason we don't sum ALL of them is because each evaluation of each $b_{ij}$
yields $D_{ij}$ from the 2 by 2 submatrix left on the remaining rows.

12. Find the cofactor matrix $C$ and multiply $A$ times $C^{\mathbf{T}}$.
    Compare $AC^{\mathbf{T}}$ with $A^{-1}$:

$$ A =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right]
$$

$$ A^{-1} =
\frac{1}{4}
\left[\begin{array}{ccc}
3 & 2 & 1 \\
2 & 4 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

_Solution:_

Find all $C_{ij}$:

$$
C_{11} = (-1)^{1 + 1}\det\left[\begin{array}{rr} 2 & -1 \\ -1 & 2 \\ \end{array}\right] = 1 \cdot 3 = 3 \\
C_{12} = (-1)^{1 + 2}\det\left[\begin{array}{rr}-1 & -1 \\0 & 2 \\\end{array}\right] = (-1) \cdot (-2) = 2 \\
C_{13} = (-1)^{1 + 3}\det\left[\begin{array}{rr}-1 & 2 \\0 & -1 \\\end{array}\right] = 1 \cdot 1 = 1 \\
C_{21} = (-1)^{2 + 1}\det\left[\begin{array}{rr}-1 & 0 \\-1 & 2 \\\end{array}\right] = (-1) \cdot (-2) = 2 \\
C_{22} = (-1)^{2 + 2}\det\left[\begin{array}{rr}2 & 0 \\0 & 2 \\\end{array}\right] = 1  \cdot 4 = 4 \\
C_{23} = (-1)^{2 + 3}\det\left[\begin{array}{rr}2 & -1 \\0 & -1 \\\end{array}\right] = (-1) \cdot (-2) = 2 \\
C_{31} = (-1)^{3 + 1}\det\left[\begin{array}{rr}-1 & 0 \\2 & -1 \\\end{array}\right] = 1 \cdot 1 = 1 \\
C_{32} = (-1)^{3 + 2}\det\left[\begin{array}{rr}2 & 0 \\-1 & -1 \\\end{array}\right] = (-1) \cdot (-2) = 2 \\
C_{33} = (-1)^{3 + 3}\det\left[\begin{array}{rr}2 & -1 \\-1 & 2 \\\end{array}\right] = 1 \cdot 3 = 3
$$

Compile into $C$:

$$ C =
\left[\begin{array}{ccc}
3 & 2 & 1 \\
2 & 4 & 2 \\
1 & 2 & 3 \\
\end{array}\right]
$$

Transpose to $C^{\mathbf{T}}$:

$$ C^{\mathbf{T}} =
\left[\begin{array}{ccc}
3 & 2 & 1 \\
2 & 4 & 2 \\
1 & 2 & 3 \\
\end{array}\right] = C
$$

Evaluate $AC^{\mathbf{T}}$:

$$ AC^{\mathbf{T}} =
\left[\begin{array}{rrr}
2 & -1 & 0 \\
-1 & 2 & -1 \\
0 & -1 & 2 \\
\end{array}\right]
\left[\begin{array}{ccc}
3 & 2 & 1 \\
2 & 4 & 2 \\
1 & 2 & 3 \\
\end{array}\right] =
\left[\begin{array}{rrr}
4 & 0 & 0 \\
0 & 4 & 0 \\
0 & 0 & 4 \\
\end{array}\right] = 4I
$$

Notice that $A^{-1} = \frac{1}{4}C^{\mathbf{T}}$.

13. The $n$ by $n$ determinant $C_n$ has $1$'s above and below the main
    diagonal:

$$ C_1 = |0| $$

$$ C_2 =
\begin{vmatrix}
0 & 1 \\
1 & 0 \\
\end{vmatrix}
$$

$$ C_3 =
\begin{vmatrix}
0 & 1 & 0 \\
1 & 0 & 1 \\
0 & 1 & 0 \\
\end{vmatrix}
$$

$$ C_4 =
\begin{vmatrix}
0 & 1 & 0 & 0 \\
1 & 0 & 1 & 0 \\
0 & 1 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{vmatrix}
$$

a. What are these determinants $C_1, C_2, C_3, C_4$?

$$
C_1 = 0, \\
C_2 = -1 \\
$$

$$ C_3 = (-1)^{1 + 2}\det\left[\begin{array}{cc}1 & 1 \\0 & 0 \\\end{array}\right] = (-1) \cdot 0 = 0 $$

$$ C_4 = (-1)^{1 + 2}\det\left[\begin{array}{ccc}1 & 1 & 0 \\0 & 0 & 1 \\0 & 1 & 0 \\\end{array}\right] = (-1) \cdot ((+1)C_2 + (-1)(0)) = (-1) \cdot ((+1)(-1) + 0) = (-1) \cdot (-1) = 1 $$

$$
C_1 = 0, \\
C_2 = -1 \\
C_3 = 0, \\
C_4 = 1 \\
$$

b. By cofactors find the relation between $C_n$ and $C_{n - 1}$ and $C_{n - 2}$.
Find $C_{10}$.

$$ C_1 = 0, C_2 = -1, C_3 = -C_{3 - 2}, C_4 = -C_{4 - 2} $$

$$ C_{10} = -C_8 = C_6 = -C_4 = C_2 = -1 $$

14. The matrices in Problem 13 have $1$'s just above and below the main
    diagonal. Going down the matrix, which order of columns (if any) gives all
    $1$'s? Explain why that permutation is _even_ for $n = 4, 8, 12, \dots$ and
    _odd_ for $n = 2, 6, 10, \dots$. Then

$$ C_n = 0(\text{odd }n) $$

$$ C_n = 1(n = 4, 8, \dots) $$

$$ C_n = -1(n = 2, 6, \cdots) $$

_Solution:_

_Going down the matrix, which order of columns (if any) gives all $1$'s?:_

In order for the columns to give all $1$'s, we must choose an entry that starts
with $1$, and then has diagonals that don't multiply by $0$. These occur where
the column begins with $1$, so that would be column $2$ for $C_2$, $C_3$, $C_4$.
Then, we must pick accordingly so that we don't get $0$, so for $C_2$ we would
choose column $1$, no such entry exists for $C_3$ as that will always result in
$0$, then for $C_4$ we would choose column $2$, then $1$ then $4$, then $3$.

_Explain why that permutation is _even_ for $n = 4, 8, 12, \dots$ and odd for
$n = 2, 6, 10, \dots$:_

It follows that this particular $C$ requires $n/2$ row exchanges to sort it into
the identity matrix.

15. The tridiagonal $1, 1, 1$ matrix of order $n$ has determinant $E_n$:

$$ E_1 = |1| $$

$$ E_2 =
\begin{vmatrix}
1 & 1 \\
1 & 1 \\
\end{vmatrix}
$$

$$ E_3 =
\begin{vmatrix}
1 & 1 & 0 \\
1 & 1 & 1 \\
0 & 1 & 1 \\
\end{vmatrix}
$$

$$ E_4 =
\begin{vmatrix}
1 & 1 & 0 & 0 \\
1 & 1 & 1 & 0 \\
0 & 1 & 1 & 1 \\
0 & 0 & 1 & 1 \\
\end{vmatrix}
$$

a. By cofactors show that $E_n = E_{n - 1} - E_{n - 2}$.

_Solution:_

Since row $1$ of any $E$ is always just two $1$'s followed by endless $0$'s, it
suffices to calculate the coefficient's of only these $1$'s.

$$ C_{11} = (-1)^{1 + 1}\det(E_{n - 1}) $$

$$ C_{12} = (-1)^{1 + 2}\det(E_{n - 2}) $$

So,

$$ E_n = E_{n - 1} - E_{n - 2} $$

b. Starting from $E_1 = 1$ and $E_2 = 0$ find $E_3, E_4, \dots, E_8$.

$$
E_1 = 1, \\
E_2 = 0, \\
E_3 = E_2 - E_1 = -1, \\
E_4 = E_3 - E_2 = -1 \\
E_5 = E_4 - E_3 = 0 \\
E_6 = E_5 - E_4 = 1 \\
E_7 = E_6 - E_5 = 1 \\
E_8 = E_7 - E_6 = 0 \\
$$

c. By noticing how these numbers eventually repeat, find $E_{100}$.

From $E_3$ onward, we notice we have a repeating six cycle. Since the cycle
starts at $E_3$, we can take $100 - 2 = 98$. Then $98 \mod 6 = 2$, This means
that $E_{100} = \text{the second element of the cycle}$, and this means
$E_{100} = E_{2 + 2} = E_4 = -1$.

16. $F_n$ is the determinant of the $1, 1, -1$ tridiagonal matrix of order $n$:

$$ F_2 =
\begin{vmatrix}
1 & -1 \\
1 & 1 \\
\end{vmatrix} = 2
$$

$$ F_3 =
\begin{vmatrix}
1 & -1 & 0 \\
1 & 1 & -1 \\
0 & 1 & 1 \\
\end{vmatrix} = 3
$$

$$ F_4 =
\begin{vmatrix}
1 & -1 &  & \\
1 & 1 & -1 & \\
& 1 & 1 & -1 \\
& & 1 & 1 \\
\end{vmatrix} \neq 4
$$

Expand in cofactors to show that $F_n = F_{n - 1} + F_{n - 2}$. These
determinants are _Fibonacci numbers_ $1, 2, 3, 5, 8, 13, \dots$. The sequence
usually starts $1, 1, 2, 3$ (with two $1$'s) so our $F_n$ is the usual
$F_{n + 1}$.

_Solution:_

For every $F$, the first row is always $(1, -1, 0, 0, 0, \dots, 0)$. It suffices
to simply take the cofactor of these first two elements:

$$ C_{11} = (-1)^{1 + 1}(F_{n - 1}) = F_{n - 1} $$

$$ C_{12} = (-1)^{1 + 2}(F_{n - 2}) = -F_{n - 2} $$

But, since this second $C_{12}$ always starts with a $-1$, this is reversed for
that specific $a_{12}$:

$$ a_{12} = (-1)C_{12} = (-1)[(-1)^{1 + 2}(F_{n - 2})] = F_{n - 2} $$

This leaves a general formula for $F_n$:

$$ F_n = C_{11} + a_{12}C_{12} = F_{n - 1} + (-1)(-F_{n - 2}) = F_{n - 1} + F_{n - 2} $$

17. The matrix $B_n$ is the $-1, 2, -1$ matrix $A_n$ except that $b_{11} = 1$
    instead of $a_{11} = 1$. Using cofactors of the _last_ row of $B_4$ show
    that $|B_4| = 2|B_3| - |B_2| = 1$.

$$ B_4 =
\left[\begin{array}{rrrr}
1 & -1 & & \\
-1 & 2 & -1 & \\
& -1 & 2 & -1 \\
& & -1 & 2 \\
\end{array}\right]
$$

$$ B_3
\left[\begin{array}{rrr}
1 & -1 & \\
-1 & 2 & -1 \\
& -1 & 2 \\
\end{array}\right]
$$

$$ B_3 =
\left[\begin{array}{rr}
1 & -1 \\
-1 & 2 \\
\end{array}\right]
$$

The recursion $|B_n| = 2|B_{n - 1}| - |B_{n - 2}|$ is satisfied when every
$|B_n| = 1$. This recursion is the same as for the $A$'s in Example 6. The
difference 8s in the starting values $1, 1, 1$ for the determinants of sizes
$n = 1, 2, 3$.

_Solution:_

The last row of every $B_n$ is $(0, 0, \dots, 0, -1, 2)$. It suffices to find
the cofactors of these last two elements:

$$ C_{nn} = (-1)^{2n}|B_{n - 1}| = 1(|B_{n - 1}|) = |B_{n - 1}| $$

$$ C_{n, n - 1} = (-1)^{2n - 1}(-|B_{n - 2}|) = -1(-|B_{n - 2}|) = |B_{n - 2}| $$

Note here that the reason we have $|B_{n - 2}|$ and not $-|B_{n - 2}|$ is
because after we eliminate for $C_{nn}$, we are left with the $-1$ in the
remaining entry right above the bottom $2$ is $-1$. We multiply this because it
is the only nonzero entry left in the remaining submatrix.

Now, since last entry of $B_n$, $b_{nn}$, is always $2$, it suffices to multiply
$C_{nn}$ by that to get the first term of $|B_n|$:

$$ |B_n| = 2C_{nn} + \dots = 2|B_{n - 1}| + \dots $$

Similarly, we multiply $-1$ by the $b_{n, n - 1}$ with $C_{n, n - 1}$ to get our
next term:

$$ |B_n| = 2C_{nn} + (-1)C_{n, n - 1} = 2|B_{n - 1}| - |B_{n - 2}| $$

$$ |B_n| = 2|B_{n - 1}| - |B_{n - 2}| $$

Now, if we fill in for $|B_4|$:

$$ |B_4| = 2|B_{4 - 1}| - |B_{4 - 2}| $$

$$ |B_4| = 2|B_3| - |B_2| $$

$$ |B_4| = 2|B_3| - 1 $$

$$ |B_4| = 2(1) - 1 $$

$$ |B_4| = 2 - 1 $$

$$ |B_4| = 1 $$

18. Go back to $B_n$ in Problem 17. It is the same as $A_n$ except for
    $b_{11} = 1$. So use linearity in the first row, where
    $\left[\begin{array}{rrr}1 & -1 & 0 \\\end{array}\right]$ equals
    $\left[\begin{array}{rrr}2 & -1 & 0 \\\end{array}\right]$ minus
    $\left[\begin{array}{rrr}1 & 0 & 0 \\\end{array}\right]$:

$$ |B_n| =
\begin{vmatrix}
1 & -1 & & 0 \\
-1 & & & \\
& & A_{n - 1} & \\
0 & & & & \\
\end{vmatrix} =
\begin{vmatrix}
2 & -1 & & 0 \\
-1 & & & \\
& & A_{n - 1} & \\
0 & & & & \\
\end{vmatrix} =
\begin{vmatrix}
1 & 0 & & 0 \\
-1 & & & \\
& & A_{n - 1} & \\
0 & & & & \\
\end{vmatrix}
$$

Linearity gives $|B_n| = |A_n| - |A_{n - 1}| =$ ____.

$$ (n + 1) - n = 1 $$

19. Explain why the $4$ by $4$ Vandermonde determinant contains $x^3$ but not
    $x^4$ or $x^5$:

$$ V_4 =
\det
\left[\begin{array}{cccc}
1 & a & a^2 & a^3 \\
1 & b & b^2 & b^3 \\
1 & c & c^2 & c^3 \\
1 & x & x^2 & x^3 \\
\end{array}\right]
$$

The determinant is zero at $x =$ ____, ____, and ____. The cofactor of $x^3$ is
$V_3 = (b - a)(c - a)(c - b)$. Then
$V_4 = (b - a)(c - a)(c - b)(x - a)(x - b)(x - c)$.

_Solution:_

Since $x, x^2, x^3$ are all in the same row, they never multiply each other in
$\det V_4$. The determinant is zero at $x = a$ or $b$ or $c$ because of equal
rows! So $\det V$ has factors $(x - a)(x - b)(x - c)$. Multiply by the cofactor
$V_3$. The Vandermonde matrix $V_{ij} = (x_i)^{j - 1}$ is for fitting a
polynomial $p(x) = b$ at the points $x_i$. It has $\det V =$ product of all
$x_k - x_m$ for $k > m$.

20. Find $G_2$ and $G_3$ and then by row operations $G_4$. Can you predict
    $G_n$?

$$ G_2 =
\begin{vmatrix}
0 & 1 \\
1 & 0 \\
\end{vmatrix}
$$

$$ G_3 =
\begin{vmatrix}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{vmatrix}
$$

$$ G_4 =
\begin{vmatrix}
0 & 1 & 1 & 1 \\
1 & 0 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 0 \\
\end{vmatrix}
$$

_Solution:_

Find $G_2$:

$$ G_2 =
\begin{vmatrix}
0 & 1 \\
1 & 0 \\
\end{vmatrix}
$$

$$ G_2 = (0)(0) - (1)(1) = -1 $$

Find $G_3$:

$$ G_3 =
\begin{vmatrix}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0 \\
\end{vmatrix}
$$

$$
C_{11} = (-1)^{1 + 1}G_2 = 1 \cdot (-1) = -1 \\
C_{12} = (-1)^{1 + 2}\det\left[\begin{array}{cc} 1 & 1 \\ 1 & 0 \\ \end{array}\right] = (-1) \cdot [(1)(0) - (1)(1)] = (-1) \cdot (-1) = 1 \\
C_{13} = (-1)^{1 + 3}\det\left[\begin{array}{cc}1 & 0 \\1 & 1 \\\end{array}\right] =  (1) \cdot [(1)(1) - (0)(1)] = 1 \cdot 1 = 1 \\
$$

$$ G_3 = 0C_{11} + 1C_{12} + 1C_{13} $$

$$ G_3 = 0(-1) + 1(1) + 1(1) = 2 $$

Find $G_4$:

$$ G_4 =
\begin{vmatrix}
0 & 1 & 1 & 1 \\
1 & 0 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 0 \\
\end{vmatrix}
$$

This is easier just to get $G_4$ into $U$, multiply the pivots, then multiply by
$\pm 1$ based off permutation.

$$ G_4 =
\begin{vmatrix}
0 & 1 & 1 & 1 \\
1 & 0 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 0 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 1 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 0 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
1 & 1 & 1 & 0 \\
0 & 1 & 1 & 1 \\
1 & 1 & 0 & 1 \\
\end{vmatrix}
$$

Three row exchanges, $-1 \cdot$ final determinant.

$$ \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
1 & 1 & 1 & 0 \\
0 & 1 & 1 & 1 \\
1 & 1 & 0 & 1 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & -1 \\
0 & 1 & 1 & 1 \\
1 & 1 & 0 & 1 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2 \\
1 & 1 & 0 & 1 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2 \\
0 & 1 & -1 & 0 \\
\end{vmatrix}
$$

$$ \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2 \\
0 & 0 & -1 & 1 \\
\end{vmatrix} \to
\begin{vmatrix}
1 & 0 & 1 & 1 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 2 \\
0 & 0 & 0 & 3 \\
\end{vmatrix} = U
$$

So determinant is $(1)(1)(1)(3) = (-1)3 = -3$.

$$ G_4 = -3 $$

The general $G_n$ increments, but multiplies odd number by $-1$. A formula for
this then is:

$$ G_n = (-1)^{n - 1}(n - 1) $$

21. Compute $S_1, S_2, S_3$ for these $1, 3, 1$ matrices. By Fibonacci guess and
    check $S_4$.

$$ S_1 = |3| $$

$$ S_2 =
\begin{vmatrix}
3 & 1 \\
1 & 3 \\
\end{vmatrix}
$$

$$ S_3 =
\begin{vmatrix}
3 & 1 & 0 \\
1 & 3 & 1 \\
0 & 1 & 3 \\
\end{vmatrix}
$$

_Solution:_

$$ S_1 = |3| = 3 $$

$$ S_2 = (3)(3) - (1)(1) = 8 $$

$$ S_3 =
\begin{vmatrix}
3 & 1 & 0 \\
1 & 3 & 1 \\
0 & 1 & 3 \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 \\
0 & \frac{8}{3} & 1 \\
0 & 1 & 3 \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 \\
0 & \frac{8}{3} & 1 \\
0 & 0 & \frac{21}{8} \\
\end{vmatrix} = U
$$

$$ S_3 = (3)\left(\frac{8}{3}\right)\left(\frac{21}{8}\right) = 21 $$

Guess for $S_4$:

Fibonacci goes $1 + 1 + 2 + 3 + 5 + 8 + 13 + 21 + 34 + 55$. It appears $S$ skips
every other fib number.

Thus guess $S_4 = 55$.

Check:

$$ S_4 =
\begin{vmatrix}
3 & 1 & 0 & 1 \\
1 & 3 & 1 & 0 \\
0 & 1 & 3 & 1 \\
1 & 0 & 1 & 3 \\
\end{vmatrix}
$$

$$ S_4 =
\begin{vmatrix}
3 & 1 & 0 & 1 \\
1 & 3 & 1 & 0 \\
0 & 1 & 3 & 1 \\
1 & 0 & 1 & 3 \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 & 1 \\
0 & \frac{8}{3} & 1 & -\frac{1}{3} \\
0 & 1 & 3 & 1 \\
1 & 0 & 1 & 3 \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 & 1 \\
0 & \frac{8}{3} & 1 & -\frac{1}{3} \\
0 & 0 & \frac{21}{8} & \frac{9}{8} \\
1 & 0 & 1 & 3 \\
\end{vmatrix} \to
$$

$$ \to
\begin{vmatrix}
3 & 1 & 0 & 1 \\
0 & \frac{8}{3} & 1 & -\frac{1}{3} \\
0 & 0 & \frac{21}{8} & \frac{9}{8} \\
0 & -\frac{1}{3} & 1 & \frac{8}{3} \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 & 1 \\
0 & \frac{8}{3} & 1 & -\frac{1}{3} \\
0 & 0 & \frac{21}{8} & \frac{9}{8} \\
0 & 0 & 1 & 3 \\
\end{vmatrix} \to
\begin{vmatrix}
3 & 1 & 0 & 1 \\
0 & \frac{8}{3} & 1 & -\frac{1}{3} \\
0 & 0 & \frac{21}{8} & \frac{9}{8} \\
0 & 0 & 0 & \frac{18}{7} \\
\end{vmatrix} = U
$$

$$ S_4 = 3 \cdot \frac{8}{3} \cdot \frac{21}{8} \cdot \frac{18}{7} = 54 $$

Somewhere the math went wrong, who cares, you get the idea.

22. Change $3$ to $2$ in the upper left corner of the matrices in Problem 21.
    Why does that subtract $S_{n - 1}$ from the determinant $S_n$? Show that the
    determinants of the new matrices become the Fibonacci numbers $2, 5, 13$
    (always $F_{2n + 1}$).

_Solution:_

Changing the upper left $3$ to $2$ reduces each count by $1$, causing the fib
sequence to become the true Fibonacci sequence (since we're no longer skipping
every other fib number).

Anyways, the new stupid determinant formula is the classic fib sequence:

$$ S_n - S_{n - 1} = F_{2n + 2} - F_{2n} = F_{2n + 1} $$

**Problems 23-26 are about block matrices and block determinants.**

23. With $2$ by $2$ blocks in $4$ by $4$ matrices, you cannot always use block
    determinants:

$$
\begin{vmatrix}
A & B \\
0 & D \\
\end{vmatrix} = |A||D|
$$

but

$$
\begin{vmatrix}
A & B \\
C & D \\
\end{vmatrix} \neq |A||D| - |C||B|
$$

a. Why is the first statement true? Somehow $B$ doesn't enter.

_Solution:_

$B$ is irrelevant because every entry is entry is multiplied by the $\mathbf{0}$
matrix. Another way of thinking of this is that this is in Upper triangular form
and you can just multiply the "pivots".

b. Show by example that equality fails (as shown) when $C$ enters.

c. Show by example that the answer $\det(AD - CB)$ is also wrong.

_Solution:_

Both (b) and \(c\) can be demonstrated together. Consider:

$$ A =
\left[\begin{array}{cc}
1 & 0 \\
0 & 0 \\
\end{array}\right], \quad
B =
\left[\begin{array}{cc}
0 & 0 \\
1 & 0 \\
\end{array}\right], \quad
C =
\left[\begin{array}{cc}
0 & 1 \\
0 & 0 \\
\end{array}\right], \quad
D =
\left[\begin{array}{cc}
0 & 0 \\
0 & 1 \\
\end{array}\right]
$$

This gives the overall matrix:

$$
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right]
$$

Then, simply permute to the identity:

$$ \to
\left[\begin{array}{cccc}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
\end{array}\right] = I
$$

One row exchange means $-1 \cdot$ final determinant.

This is $-1 \cdot |I| = -1 \cdot 1 = -1$.

Okay, so then what is $|A||D| - |C||B|$?:

$$ |A| = 0, |D| = 0, |C| = 0, |B| = 0 $$

So $|A||D| - |C||B| = (0)(0) - (0)(0) = 0 \neq -1$.

24. With block multiplication, $A = LU$ has $A_k = L_kU_k$ in the top left
    corner:

$$ A =
\left[\begin{array}{cc}
A_k & \text{*} \\
\text{*} & \text{*} \\
\end{array}\right] =
\left[\begin{array}{cc}
L_k & 0 \\
\text{*} & \text{*} \\
\end{array}\right]
\left[\begin{array}{cc}
U_k & \text{*} \\
0 & \text{*} \\
\end{array}\right]
$$

a. Suppose the first three pivots of $A$ are $2, 3, -1$. What are the
determinants of $L_1, L_2, L_3$ (with diagonal $1$'s) and $U_1, U_2, U_3$ and
$A_1, A_2, A_3$?

_Solution:_

Recall that a lower triangular matrix is just the elimination steps multiplied
together (the product of a bunch of $E$'s). This always results in diagonal
pivots of $1$'s. Thus the determinant of all $L$'s is $1$.

For $k = 1$, $\det(A_1) = \det(U_1) = |2| = 2$, for $k = 2$,
$\det(A_2) = \det(U_2) = (2)(3) = 6$, finally for $k = 3$,
$\det(A_3) = \det(U_3 = (2)(3)(-1) = -6$.

b. If $A_1, A_2, A_3$ have determinants $5, 6, 7$ find the three pivots from
equation (3).

_Solution:_

Equation (3) states:

The $k$th pivot is

$$ d_k = \frac{d_1d_2 \cdots d_k}{d_1d_2 \cdots d_{k - 1}} = \frac{\det A_k}{\det A_{k - 1}} $$

$$ d_1 = \det A_1 = 5 $$

$$ d_2 = \det A_2 = \frac{\det A_2}{\det A_{2 - 1}} = \frac{6}{5} $$

$$ d_3 = \det A_3 = \frac{\det A_3}{\det A_{3 - 1}} = \frac{7}{6} $$

25. Block elimination subtracts $CA^{-1}$ times the first row
    $\left[\begin{array}{cc}A & B\end{array}\right]$ from the second row
    $\left[\begin{array}{cc|c}C & D \\\end{array}\right]$. This leaves the
    _Schur complement_ $D - CA^{-1}B$ in the corner:

$$
\left[\begin{array}{rr}
I & 0 \\
-CA^{-1} & I \\
\end{array}\right]
\left[\begin{array}{cc}
A & B \\
C & D \\
\end{array}\right] =
\left[\begin{array}{cc}
A & B \\
0 & D - CA^{-1}B \\
\end{array}\right]
$$

Take determinants of these block matrices to prove correct rules if $A^{-1}$
exists:

$$
\begin{vmatrix}
A & B \\
C & D \\
\end{vmatrix} =
|A||D - CA^{-1}B| =
|AD - CB| \text{ provided } AC = CA
$$

_Solution:_

This looks complicated but consider the first block matrix:

$$
\left[\begin{array}{rr}
I & 0 \\
-CA^{-1} & I \\
\end{array}\right]
$$

This is just $|I| \cdot |I| = 1 \cdot 1 = 1$ since $0 \cdot -CA^{-1} = 0$.

Then consider that the final matrix (on the right of the equality) has a
determinant of:

$$ |A| \cdot |D - CA^{-1}B| $$

The product rule says we can indeed just distribute $|A|$ here to:

$$ |AD - ACA^{-1}B| = |AD - CB| $$

26. If $A$ is $m$ by $n$ and $B$ is $n$ by $m$, block multiplication gives
    $\det M = \det AB$:

$$ M =
\left[\begin{array}{rr}
0 & A \\
-B & I \\
\end{array}\right] =
\left[\begin{array}{cc}
AB & A \\
0 & I \\
\end{array}\right]
\left[\begin{array}{rr}
I & 0 \\
-B & I \\
\end{array}\right]
$$

If $A$ is a single row and $B$ is a single column what is $\det M$? If $A$ is a
column and $B$ is a row what is $\det M$? Do a $3$ by $3$ example of each.

_Solution:_

_If $A$ is a single row and $B$ is a single column what is $\det M$?:_

If $A$ is a single row and $B$ is a single column, then their product is just a
number or single element matrix.

Then the determinant of $M$ is that number, since $ABI =  AB$ and the second
matrix's determinant is just $|I||I| = 1$.

$$ |M| = |AB| \cdot |I| = AB \cdot 1 = AB $$

_If $A$ is a column and $B$ is a row what is $\det M$?:_

In this case, $AB$ is a 3 by 3 matrix, in which case the determinant of $M$ is
$|AB|$.

$$ |M| = |AB| $$

Additionally, note that any column times a row results in a rank 1 matrix,
meaning that it's other two rows are dependent, and this ultimately means that
$AB$ is singular, and thus:

$$ |M| = 0 $$

27. (A calculus question) Show that the derivative of $\det A$ with respect to
    $a_{11}$ is the cofactor $C_{11}$. The other entries are fixed - we are only
    changing $a_{11}$.

Omitted.

28. A $3$ by $3$ determinant has three products "down to the right" and three
    "down to the left" with minus signs. Compute the six terms like
    $(1)(5)(9) = 45$ to find $D$.

(See Page 282 for figure).

Omitted.

29. For $E_4$ in Problem 15, five of the $4! = 24$ terms in the big formula (8)
    are nonzero. Find those five terms to show that $E_4 = -1$.

Omitted.

30. For the $4$ by $4$ tridiagonal second difference matrix (entries
    $-1, 2, -1$) find the five terms in the big formula that give
    $\det A = 16 - 4 - 4 - 4 + 1$.

Omitted.

31. Find the determinant of this cyclic $P$ by cofactors of row $1$ and then the
    "big formula". How many exchanges reorder $4, 1, 2, 3$ into $1, 2, 3, 4$? Is
    $|P^2| = 1$ or $-1$?

$$ P =
\left[\begin{array}{cccc}
0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
\end{array}\right]
$$

$$ P^2 =
\left[\begin{array}{cccc}
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
\end{array}\right] =
\left[\begin{array}{cc}
0 & I \\
I & 0 \\
\end{array}\right]
$$

Omitted.
