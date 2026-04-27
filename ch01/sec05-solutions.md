# 1-5. Testing Series for Convergence; the Preliminary Test

> **Preliminary test**: if $a_n$ does not tend to 0, then $\sum a_n$ diverges. If $a_n\to 0$, the test is inconclusive.

### Problem 1. Terms Do Not Tend to 0

$$
a_n=(-1)^{n+1}\frac{n^2}{n^2+1},
\qquad
|a_n|\to 1.
$$

The terms do not approach 0, so the series **diverges**.

### Problem 2. Preliminary Test Is Inconclusive

$$
a_n=\frac{\sqrt{n+1}}{n}
=\sqrt{\frac{1}{n}+\frac{1}{n^2}}
\to 0.
$$

The preliminary test gives no conclusion. A later comparison would show divergence, since $a_n\sim 1/\sqrt n$.

### Problem 3. Preliminary Test Is Inconclusive

$$
a_n=\frac{n+3}{n^2+10n}
=\frac{1+3/n}{n(1+10/n)}
\to 0.
$$

The preliminary test gives no conclusion. In fact, $a_n\sim 1/n$, so the series diverges.

### Problem 4. Terms Do Not Tend to 0

$$
|a_n|
=\frac{n^2}{(n+1)^2}
=\left(1-\frac{1}{n+1}\right)^2
\to 1.
$$

Thus $a_n$ does not tend to 0. The series **diverges**.

### Problem 5. Terms Tend to 1

$$
a_n=\frac{n!}{n!+1}
=\frac{1}{1+1/n!}
\to 1\ne 0.
$$

The series **diverges**.

### Problem 6. Preliminary Test Is Inconclusive

$$
a_n=\frac{n!}{(n+1)!}
=\frac{1}{n+1}
\to 0.
$$

The preliminary test gives no conclusion. This is a harmonic tail, so the series actually diverges.

### Problem 7. Preliminary Test Is Inconclusive

$$
|a_n|
=\frac{n}{\sqrt{n^3+1}}
=\frac{1}{\sqrt{n+1/n^2}}
\to 0.
$$

The preliminary test gives no conclusion. This series is handled later by the alternating series test.

### Problem 8. Preliminary Test Is Inconclusive

$$
a_n=\frac{\ln n}{n}\to 0.
$$

The preliminary test gives no conclusion. Since $\ln n>1$ for $n\ge 3$, this series is larger than a harmonic tail and diverges.

### Problem 9. Terms Tend to 1

$$
a_n=\frac{3^n}{2^n+3^n}
=\frac{1}{(2/3)^n+1}
\to 1.
$$

The series **diverges**.

### Problem 10. Terms Tend to 1

$$
a_n=1-\frac{1}{n^2}\to 1.
$$

The series **diverges**.

### Problem 11. Proof of the Preliminary Test

If $\sum a_n$ converges to $S$, then its partial sums satisfy $S_n\to S$. Since

$$
a_n=S_n-S_{n-1},
$$

we get

$$
\lim_{n\to\infty}a_n
=\lim_{n\to\infty}S_n-\lim_{n\to\infty}S_{n-1}
=S-S=0.
$$

Therefore, if $a_n$ does not tend to 0, the series cannot converge.

The converse is false: $1/n\to 0$, but $\sum 1/n$ diverges.
