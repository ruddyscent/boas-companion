# 1-4. Convergent and Divergent Series

For each problem, list $a_n$, $S_n$, and $R_n=S-S_n$, then take limits.

### Problem 1. Geometric Series

For $\displaystyle\sum_{n=1}^{\infty}1/2^n$,

$$
a_n=\frac{1}{2^n},\qquad
S_n=1-\frac{1}{2^n},\qquad
R_n=\frac{1}{2^n}.
$$

Thus $S_n\to 1$ and $R_n\to 0$. The series **converges**, with $S=1$.

### Problem 2. Geometric Series Starting at 0

For $\displaystyle\sum_{n=0}^{\infty}1/5^n$,

$$
a_n=\frac{1}{5^n},\qquad
S_n=\frac{1-(1/5)^{n+1}}{1-1/5}
=\frac54\left(1-\frac{1}{5^{n+1}}\right),
$$

and

$$
R_n=\frac54\cdot\frac{1}{5^{n+1}}
=\frac{1}{4\cdot 5^n}.
$$

The series **converges**, with $S=5/4$.

### Problem 3. Alternating Geometric Series

For $1-\tfrac12+\tfrac14-\tfrac18+\cdots$, $r=-1/2$:

$$
a_n=\left(-\frac12\right)^{n-1},\qquad
S_n=\frac{1-(-1/2)^n}{1-(-1/2)}
=\frac23\left(1-\left(-\frac12\right)^n\right),
$$

and

$$
R_n=\frac23\left(-\frac12\right)^n.
$$

The series **converges**, with $S=2/3$.

### Problem 4. Exponential Form

Since $e^{-\ln 3}=1/3$,

$$
e^{-n\ln 3}=\left(\frac13\right)^n.
$$

Therefore

$$
a_n=\frac{1}{3^n},\qquad
S_n=\frac12\left(1-\frac{1}{3^n}\right),\qquad
R_n=\frac{1}{2\cdot 3^n}.
$$

The series **converges**, with $S=1/2$.

### Problem 5. Trigonometric Exponential Form

Since $\sin(\pi/3)=\sqrt3/2$,

$$
e^{2n\ln\sin(\pi/3)}
=\left(\frac{\sqrt3}{2}\right)^{2n}
=\left(\frac34\right)^n.
$$

Thus

$$
a_n=\left(\frac34\right)^n,\qquad
S_n=4-3\left(\frac34\right)^n,\qquad
R_n=3\left(\frac34\right)^n.
$$

The series **converges**, with $S=4$.

### Problem 6. Telescoping Series

Use

$$
\frac{1}{n(n+1)}
=\frac{1}{n}-\frac{1}{n+1}.
$$

Then

$$
a_n=\frac{1}{n(n+1)},\qquad
S_n=1-\frac{1}{n+1}
=\frac{n}{n+1},
$$

and

$$
R_n=1-S_n=\frac{1}{n+1}.
$$

The series **converges**, with $S=1$.

### Problem 7. Alternating Telescoping Series

The general term is

$$
a_n=(-1)^{n+1}\frac{2n+1}{n(n+1)}
=(-1)^{n+1}\left(\frac{1}{n}+\frac{1}{n+1}\right).
$$

The partial sums simplify to

$$
S_n=1+\frac{(-1)^{n+1}}{n+1}.
$$

Hence $S_n\to 1$, and

$$
R_n=1-S_n
=\frac{(-1)^n}{n+1}.
$$

The series **converges**, with $S=1$. It is not absolutely convergent, since $|a_n|\sim 2/n$.
