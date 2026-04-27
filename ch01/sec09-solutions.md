# 1-9. Useful Facts About Series

> First check whether the general term tends to 0. Then choose a suitable test: comparison, ratio, integral, special comparison, absolute convergence, or alternating series.

### Problem 1. Harmonic Order

$$
\frac{n-1}{(n+2)(n+3)}\sim \frac{1}{n}.
$$

So the series **diverges**.

### Problem 2. Terms Tend to 1

$$
\frac{n^2-1}{n^2+1}\to 1.
$$

The series **diverges**.

### Problem 3. $p$-Series

$$
\sum \frac{1}{n^{\ln 3}},
\qquad
\ln 3>1.
$$

So the series **converges**.

### Problem 4. Harmonic Order

$$
\frac{n^2}{n^3+4}\sim \frac{1}{n}.
$$

So the series **diverges**.

### Problem 5. $p=2$ Order

$$
\frac{n}{n^3-4}\sim \frac{1}{n^2}.
$$

So the series **converges**.

### Problem 6. Ratio Test

For $a_n=(n!)^2/(2n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{(n+1)^2}{(2n+1)(2n+2)}
\to \frac14.
$$

The series **converges**.

### Problem 7. Ratio Test

For $a_n=(2n)!/[3^n(n!)^2]$,

$$
\frac{a_{n+1}}{a_n}
=\frac{2(2n+1)}{3(n+1)}
\to \frac43.
$$

The series **diverges**.

### Problem 8. Ratio Test

For $a_n=n^5/5^n$,

$$
\frac{a_{n+1}}{a_n}
=\frac15\left(\frac{n+1}{n}\right)^5
\to \frac15.
$$

The series **converges**.

### Problem 9. Ratio Test

For $a_n=n^n/n!$,

$$
\frac{a_{n+1}}{a_n}
=\left(1+\frac{1}{n}\right)^n
\to e.
$$

The series **diverges**.

### Problem 10. Terms Do Not Tend to 0

$$
\left|\frac{(-1)^n n}{n-1}\right|
=\frac{n}{n-1}
\to 1.
$$

The series **diverges**.

### Problem 11. Harmonic Order

$$
\frac{2n}{n^2-9}\sim \frac{2}{n}.
$$

So the series **diverges**.

### Problem 12. Telescoping

$$
\frac{1}{n^2-n}
=\frac{1}{n(n-1)}
=\frac{1}{n-1}-\frac{1}{n}.
$$

The partial sums tend to 1, so the series **converges**.

### Problem 13. $p=2$ Order

$$
\frac{n}{(n^2+4)^{3/2}}
\sim \frac{n}{n^3}
=\frac{1}{n^2}.
$$

So the series **converges**.

### Problem 14. Absolute Convergence

$$
\left|\frac{(-1)^n}{n^2-n}\right|
\sim \frac{1}{n^2}.
$$

So the series is **absolutely convergent**.

### Problem 15. Terms Grow

For $a_n=(-1)^n n!/10^n$,

$$
\frac{|a_{n+1}|}{|a_n|}
=\frac{n+1}{10}
\to\infty.
$$

The terms do not tend to 0, so the series **diverges**.

### Problem 16. Compare with $1/n^2$

Since $2+(-1)^n$ is either 1 or 3,

$$
\left|\frac{2+(-1)^n}{n^2+7}\right|
\le \frac{3}{n^2+7}
\le \frac{3}{n^2}.
$$

The series **converges absolutely**.

### Problem 17. Ratio Test

For $a_n=(n!)^3/(3n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{(n+1)^3}{(3n+1)(3n+2)(3n+3)}
\to \frac{1}{27}.
$$

The series **converges**.

### Problem 18. Alternating $p$-Series

Since

$$
2^{\ln n}=n^{\ln 2},
$$

the absolute values are $1/n^{\ln 2}$, where $\ln 2<1$. The alternating series test gives convergence, but the absolute series diverges. Therefore the series is **conditionally convergent**.

### Problem 19. Difference of Geometric Series

$$
\sum_{k=2}^{\infty}\frac{1}{2^k}
-\sum_{k=2}^{\infty}\frac{1}{3^k}
=\frac{1/4}{1-1/2}-\frac{1/9}{1-1/3}
=\frac12-\frac16
=\frac13.
$$

The series **converges**, with sum $1/3$.

### Problem 20. Pair Terms

Pairing the given series gives

$$
\sum_{k=2}^{\infty}(-1)^k\left(\frac{1}{k}+\frac{1}{k^2}\right).
$$

The terms decrease to 0, so the alternating series test gives convergence. Since $\sum 1/k$ diverges, the convergence is **conditional**.

### Problem 21. Recursive Ratio

From

$$
a_{n+1}=\frac{n}{2n+3}a_n,
$$

we get $a_{n+1}/a_n\to 1/2$. The series **converges**.

### Problem 22. Reduce to a $p$-Series

Use

$$
k^{\ln n}=e^{\ln k\,\ln n}=n^{\ln k}.
$$

Thus $\sum 1/k^{\ln n}$ behaves like $\sum 1/n^{\ln k}$.

(a) If $k=3$, then $\ln 3>1$, so the series **converges**.

(b) If $k=2$, then $\ln 2<1$, so the series **diverges**.

(c) The series converges exactly when

$$
\ln k>1,
\qquad\text{that is,}\qquad
k>e.
$$

For integer $k$, this means $k\ge 3$.
