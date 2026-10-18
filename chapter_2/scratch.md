## Chapter 2.3 Elimination Using Matrices

**Basics of Matrix Multiplication:**

$$
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 4 & 1\\
0 & 0 & 3 \\
0 & 6 & 5 \\
\end{array}\right] = \text{?}
$$

Divide each column of the second matrix into its individual columns and then
treat this as matrix-vector multiplication.

$$
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}2\\0\\0\end{bmatrix} =
\begin{bmatrix}{}2\\0\\0\end{bmatrix}
$$

This is the first column of our answer matrix.

$$
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}4\\0\\6\end{bmatrix} =
\begin{bmatrix}{}4\\6\\0\end{bmatrix}
$$

This is the second column of our answer matrix.

$$
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\begin{bmatrix}{}1\\3\\5\end{bmatrix} =
\begin{bmatrix}{}1\\5\\3\end{bmatrix}
$$

This is the third column of our answer matrix.

Thus our answer is:

$$
\left[\begin{array}{ccc}
1 & 0 & 0\\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{ccc}
2 & 4 & 1\\
0 & 0 & 3 \\
0 & 6 & 5 \\
\end{array}\right] =
\left[\begin{array}{ccc}
2 & 4 & 1\\
0 & 6 & 5 \\
0 & 0 & 3 \\
\end{array}\right]
$$

---

$$ E_{21} =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
$$

$$ P_{32} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
$$

$$
\left[\begin{array}{c}A & b\end{array}\right] =
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
4 & 8 & 9 & 3 \\
0 & 3 & 2 & 1 \\
\end{array}\right]
$$

Apply $E_{21}$:

$$ E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
4 & 8 & 9 & 3 \\
0 & 3 & 2 & 1 \\
\end{array}\right]
$$

Notice that $E_{21}$ goes to the right of
$\left[\begin{array}{cc}A & b\end{array}\right]$.

$$ E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right]
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
4 & 8 & 9 & 3 \\
0 & 3 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
0 & 0 & 1 & -1 \\
0 & 3 & 2 & 1 \\
\end{array}\right]
$$

Again, this was done by taking the matrix
$\left[\begin{array}{rr}A & b\end{array}\right]$ and multiplying it by each
column of the matrix $E_{21}$and then outputting a corresponding column in the
output matrix, this can be treated by multiplying the
$\left[\begin{array}{rr}A & b\end{array}\right]$ by each column as if it were a
vector.

Apply $P_{32}$ to $E_{21}\left[\begin{array}{rr}A & b\end{array}\right]$:

$$ P_{32}E_{21}\left[\begin{array}{cc}A & b\end{array}\right]=
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
0 & 0 & 1 & -1 \\
0 & 3 & 2 & 1 \\
\end{array}\right]
$$

Again, notice how we put $P_{32}$ on the left of
$E_{21}\left[\begin{array}{cc}A & b\end{array}\right]$.

$$ P_{32}E_{21}\left[\begin{array}{cc}A & b\end{array}\right] =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
0 & 0 & 1 & -1 \\
0 & 3 & 2 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrrr}
1 & 2 & 2 & 1 \\
0 & 3 & 2 & 1 \\
0 & 0 & 1 & -1 \\
\end{array}\right]
$$

Now, we have applied an elimination matrix followed by a permutation matrix
here. If we combine $P_{32}E_{21}$ into a single matrix, we are left with a
matrix that does both operations at once:

$$ P_{32}E_{21} =
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{array}\right]
\left[\begin{array}{rrr}
1 & 0 & 0 \\
-4 & 1 & 0 \\
0 & 0 & 1 \\
\end{array}\right] =
\left[\begin{array}{rrr}
1 & 0 & 0 \\
0 & 0 & 1 \\
-4 & 1 & 0 \\
\end{array}\right]
$$

Applying $P_{32}E_{21}$ to $\left[\begin{array}{cc}A & b\end{array}\right]$ will
result in the $P_{32}E_{21}\left[\begin{array}{cc}A & b\end{array}\right]$ that
we got before.
