## Euclidean Norm

In this chapter, Strang assumes your knowledge of Euclidean Norms. Let's review
(since you don't actually know what these are).

In the context of Linear Algebra, the Euclidean Norm is simply the distance of
the vector itself. Take some vector $\vec{u}$, defined as follows:

$$ \vec{u} = \begin{bmatrix}{}a\\b\end{bmatrix} $$

Then, we know that this vector, which is in $\R^2$, forms a triangle on the
standard Cartesian plane, where the hypotenuse $h$ is defined such that:

$$ h^2 = a^2 + b^2 $$

by the Pythagorean Theorem.

Now, to find the length of $h$, we take the square root of $a^2 + b^2$:

$$ h = \sqrt{a^2 + b^2} $$

And this is the length of $h$, so we can denote it using the Euclidean notation,
substituting in our $\vec{u}$ for $h$:

$$ \|\vec{u}\| = \sqrt{a^2 + b^2} $$

Note that this Euclidean Norm will always reside within $\R^+$.

Now, consider if $\vec{u}$ is defined in $\R^3$, then:

$$ \|\vec{u}\| = \sqrt{a^2 + b^2 + c^2} $$

More generally, let's say that $\vec{u}$ is defined in $\R^n$, then:

$$ \|\vec{u}\| = \sqrt{a_1^2 + a_2^2 + \cdots + a_n^2} $$

This is generally denoted using Sigma/Summation notation as:

$$ \|\vec{u}\| = \left(\sum_{n}^{i = 1}{a_i^2}\right)^{\frac{1}{2}} $$

Now, for some specific examples to really hammer this home, consider:

$$ \vec{u} = \begin{bmatrix}{}1\\1\end{bmatrix} $$

Then:

$$ \|\vec{u}\| = \sqrt{1^1 + 1^1} = \sqrt{2} $$

Another example:

$$ \vec{u} = \begin{bmatrix}{}-1\\3\end{bmatrix} $$

$$ \|\vec{u}\| = \sqrt{(-1)^2 + 3^2} = \sqrt{10} $$

Another thing to note is that when $\|\vec{u}\| = 0$, this means that the
coordinates are $\mathbf{0}$ (the zero vector).

These notes were garnered from watching this
[Archimedes Notes Video](https://www.youtube.com/watch?v=NXfqOol1Ku0).

---
