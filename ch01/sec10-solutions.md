# 1-10. Power Series

> For a power series, first use the ratio/root/geometric test to find the radius of convergence. Then test each endpoint separately.

### Problem 1. Geometric Series

$$
\sum_{n=0}^{\infty}(-1)^n x^n
=\sum_{n=0}^{\infty}(-x)^n.
$$

This converges when $|-x|<1$, so $|x|<1$.
At $x=1$ or $x=-1$, the terms do not tend to 0.

The interval of convergence is

$$
(-1,1).
$$

### Problem 2. Geometric Series

$$
\sum_{n=0}^{\infty}\frac{(2x)^n}{3^n}
=\sum_{n=0}^{\infty}\left(\frac{2x}{3}\right)^n.
$$

This converges when

$$
\left|\frac{2x}{3}\right|<1,
\qquad |x|<\frac32.
$$

At $x=\pm 3/2$, the terms do not tend to 0.

The interval of convergence is

$$
\left(-\frac32,\frac32\right).
$$

### Problem 3. Ratio Test and Endpoints

$$
\sum_{n=1}^{\infty}\frac{(-1)^n x^n}{n(n+1)}
$$

has radius $R=1$. At $x=1$,

$$
\sum_{n=1}^{\infty}\frac{(-1)^n}{n(n+1)}
$$

converges absolutely. At $x=-1$,

$$
\sum_{n=1}^{\infty}\frac{1}{n(n+1)}
$$

also converges.

The interval of convergence is

$$
[-1,1].
$$

### Problem 4. Substitute $y=x^2/2$

$$
\sum_{n=1}^{\infty}\frac{x^{2n}}{2^n n^2}
=\sum_{n=1}^{\infty}\frac{(x^2/2)^n}{n^2}.
$$

This converges when $|x^2/2|<1$, so $|x|<\sqrt2$.
At $x=\pm\sqrt2$, the series becomes

$$
\sum_{n=1}^{\infty}\frac{1}{n^2},
$$

which converges.

The interval of convergence is

$$
[-\sqrt2,\sqrt2].
$$

### Problem 5. Ratio Test

For

$$
a_n=\frac{x^n}{(n!)^2},
$$

we have

$$
\left|\frac{a_{n+1}}{a_n}\right|
=\frac{|x|}{(n+1)^2}
\to 0.
$$

Thus the series converges for every real $x$.

The interval of convergence is

$$
(-\infty,\infty).
$$

### Problem 6. Ratio Test

For

$$
a_n=\frac{(-1)^n x^n}{(2n)!},
$$

we have

$$
\left|\frac{a_{n+1}}{a_n}\right|
=\frac{|x|}{(2n+2)(2n+1)}
\to 0.
$$

Thus the series converges for every real $x$.

The interval of convergence is

$$
(-\infty,\infty).
$$

### Problem 7. Substitute $y=x^3$

$$
\sum_{n=1}^{\infty}\frac{x^{3n}}{n}
=\sum_{n=1}^{\infty}\frac{(x^3)^n}{n}.
$$

This converges when $|x^3|<1$, so $|x|<1$.
At $x=1$, the series is harmonic and diverges. At $x=-1$, it becomes

$$
\sum_{n=1}^{\infty}\frac{(-1)^n}{n},
$$

which converges.

The interval of convergence is

$$
[-1,1).
$$

### Problem 8. Alternating Endpoint

$$
\sum_{n=1}^{\infty}\frac{(-1)^n x^n}{\sqrt n}
=\sum_{n=1}^{\infty}\frac{(-x)^n}{\sqrt n}.
$$

The radius is $R=1$. At $x=1$, the series

$$
\sum_{n=1}^{\infty}\frac{(-1)^n}{\sqrt n}
$$

converges by the alternating series test. At $x=-1$, the series

$$
\sum_{n=1}^{\infty}\frac{1}{\sqrt n}
$$

diverges.

The interval of convergence is

$$
(-1,1].
$$

### Problem 9. Polynomial Factor

$$
\sum_{n=1}^{\infty}(-1)^n n^3 x^n
$$

has radius $R=1$. At $x=1$ and $x=-1$, the terms do not tend to 0 because their size is $n^3$.

The interval of convergence is

$$
(-1,1).
$$

### Problem 10. Substitute $y=x^2$

$$
\sum_{n=1}^{\infty}\frac{(-1)^n x^{2n}}{(2n)^{3/2}}
=\sum_{n=1}^{\infty}\frac{(-x^2)^n}{(2n)^{3/2}}.
$$

This converges when $|x|<1$. At $x=\pm1$, the series converges absolutely since

$$
\sum_{n=1}^{\infty}\frac{1}{(2n)^{3/2}}
$$

is a convergent $p$-series.

The interval of convergence is

$$
[-1,1].
$$

### Problem 11. Logarithmic Power Series

$$
\sum_{n=1}^{\infty}\frac{1}{n}\left(\frac{x}{5}\right)^n
$$

converges when $|x/5|<1$, so $|x|<5$.
At $x=5$, it is the harmonic series and diverges. At $x=-5$, it is the alternating harmonic series and converges.

The interval of convergence is

$$
[-5,5).
$$

### Problem 12. Ratio Test

$$
\sum_{n=1}^{\infty} n(-2x)^n
$$

has radius condition

$$
|-2x|<1,
\qquad |x|<\frac12.
$$

At $x=\pm 1/2$, the terms have size $n$, so they do not tend to 0.

The interval of convergence is

$$
\left(-\frac12,\frac12\right).
$$

### Problem 13. Endpoint Test

$$
\sum_{n=1}^{\infty}\frac{n(-x)^n}{n^2+1}
$$

has radius $R=1$. At $x=1$,

$$
\sum_{n=1}^{\infty}\frac{n(-1)^n}{n^2+1}
$$

converges by the alternating series test. At $x=-1$,

$$
\sum_{n=1}^{\infty}\frac{n}{n^2+1}
\sim \sum_{n=1}^{\infty}\frac1n
$$

diverges.

The interval of convergence is

$$
(-1,1].
$$

### Problem 14. Ratio Test

$$
\sum_{n=1}^{\infty}\frac{n}{n+1}\left(\frac{x}{3}\right)^n
$$

has radius condition $|x/3|<1$, so $|x|<3$.
At $x=3$ and $x=-3$, the terms do not tend to 0 because

$$
\frac{n}{n+1}\to 1.
$$

The interval of convergence is

$$
(-3,3).
$$

### Problem 15. Geometric Series

$$
\sum_{n=1}^{\infty}\frac{(x-2)^n}{3^n}
=\sum_{n=1}^{\infty}\left(\frac{x-2}{3}\right)^n.
$$

This converges when

$$
\left|\frac{x-2}{3}\right|<1,
\qquad -1<x<5.
$$

At $x=-1$ and $x=5$, the terms do not tend to 0.

The interval of convergence is

$$
(-1,5).
$$

### Problem 16. Geometric Series

$$
\sum_{n=1}^{\infty}\frac{(x-1)^n}{2^n}
=\sum_{n=1}^{\infty}\left(\frac{x-1}{2}\right)^n.
$$

This converges when

$$
\left|\frac{x-1}{2}\right|<1,
\qquad -1<x<3.
$$

At $x=-1$ and $x=3$, the terms do not tend to 0.

The interval of convergence is

$$
(-1,3).
$$

### Problem 17. Alternating Endpoint

$$
\sum_{n=1}^{\infty}\frac{(-1)^n(x+1)^n}{n}
=\sum_{n=1}^{\infty}\frac{[-(x+1)]^n}{n}.
$$

The radius condition is $|x+1|<1$, so $-2<x<0$.
At $x=0$, the series is the alternating harmonic series and converges. At $x=-2$, it is the harmonic series and diverges.

The interval of convergence is

$$
(-2,0].
$$

### Problem 18. Substitute $y=-2(2x+1)$

$$
\sum_{n=1}^{\infty}\frac{(-2)^n(2x+1)^n}{n^2}
=\sum_{n=1}^{\infty}\frac{[-2(2x+1)]^n}{n^2}.
$$

This converges when

$$
|-2(2x+1)|<1,
\qquad -\frac34<x<-\frac14.
$$

At both endpoints, the series becomes a convergent $p$-series up to signs.

The interval of convergence is

$$
\left[-\frac34,-\frac14\right].
$$

### Problem 19. Substitute $y=x^2-1$

$$
\sum_{n=0}^{\infty}8^{-n}(x^2-1)^n
=\sum_{n=0}^{\infty}\left(\frac{x^2-1}{8}\right)^n.
$$

This converges when

$$
\left|\frac{x^2-1}{8}\right|<1,
\qquad |x^2-1|<8.
$$

Thus $x^2<9$, so $|x|<3$. At $x=\pm3$, the terms do not tend to 0.

The convergence set is

$$
(-3,3).
$$

### Problem 20. Factorial Denominator

$$
\sum_{n=0}^{\infty}(-1)^n\frac{2^n}{n!}(x^2+1)^{2n}
=\sum_{n=0}^{\infty}\frac{[-2(x^2+1)^2]^n}{n!}.
$$

This is an exponential-type series and converges for every real value of $x$.

The convergence set is

$$
(-\infty,\infty).
$$

### Problem 21. Substitute $y=\sqrt{x}$

For real-valued terms, take $x\ge 0$ and let $y=\sqrt{x}$. Then

$$
\sum_{n=2}^{\infty}\frac{(-1)^n x^{n/2}}{n\ln n}
=\sum_{n=2}^{\infty}\frac{(-1)^n y^n}{n\ln n}.
$$

The corresponding power series has radius $1$ in $y$.
Thus $0\le x<1$. At $x=1$,

$$
\sum_{n=2}^{\infty}\frac{(-1)^n}{n\ln n}
$$

converges by the alternating series test.

The convergence set is

$$
[0,1].
$$

### Problem 22. Substitute $y=-1/x$

$$
\sum_{n=0}^{\infty}\frac{n!(-1)^n}{x^n}
=\sum_{n=0}^{\infty} n!\left(-\frac1x\right)^n.
$$

The power series $\sum n!y^n$ has radius $0$. Therefore, for every finite real $x$, the terms fail to tend to 0.

There is no finite real $x$ for which the series converges.

### Problem 23. Substitute $y=3/(x+1)$

$$
\sum_{n=0}^{\infty}\frac{3^n(n+1)}{(x+1)^n}
=\sum_{n=0}^{\infty}(n+1)\left(\frac{3}{x+1}\right)^n.
$$

This converges when

$$
\left|\frac{3}{x+1}\right|<1,
\qquad |x+1|>3.
$$

At $x=2$ and $x=-4$, the terms do not tend to 0.

The convergence set is

$$
(-\infty,-4)\cup(2,\infty).
$$

### Problem 24. Root Test

$$
\sum_{n=0}^{\infty}\left(\sqrt{x^2+1}\right)^n\frac{2^n}{3^n+n^3}.
$$

By the root test,

$$
\lim_{n\to\infty}\sqrt[n]{\left|\left(\sqrt{x^2+1}\right)^n\frac{2^n}{3^n+n^3}\right|}
=\frac{2\sqrt{x^2+1}}{3}.
$$

So the series converges when

$$
\frac{2\sqrt{x^2+1}}{3}<1,
\qquad x^2<\frac54.
$$

At $x=\pm\sqrt5/2$, the terms tend to $1$, so the series diverges.

The convergence set is

$$
\left(-\frac{\sqrt5}{2},\frac{\sqrt5}{2}\right).
$$

### Problem 25. Geometric Series in $\sin x$

$$
\sum_{n=0}^{\infty}(\sin x)^n(-1)^n2^n
=\sum_{n=0}^{\infty}(-2\sin x)^n.
$$

This converges when

$$
|-2\sin x|<1,
\qquad |\sin x|<\frac12.
$$

At $|\sin x|=1/2$, the terms do not tend to 0.

The convergence set is

$$
\bigcup_{k\in\mathbb Z}\left(k\pi-\frac{\pi}{6},\,k\pi+\frac{\pi}{6}\right).
$$
