# 1-12. Taylor's Series

> Use the same method used for (12.5): write
> $f(x)=\sum_{n=0}^{\infty}a_nx^n$, differentiate repeatedly, and set
> $x=0$. Equivalently,
>
> $$
> a_n=\frac{f^{(n)}(0)}{n!}.
> $$

### Problem 1. Verify the Basic Series

The series (13.1) for $\sin x$ is the one obtained by the method used for (12.5), so here we verify the remaining basic series (13.2) to (13.5) by computing the Maclaurin coefficients.

#### (13.2) The Series for $\cos x$

Let

$$
\cos x=\sum_{n=0}^{\infty}a_nx^n.
$$

The derivatives repeat in the cycle

$$
\cos x,\quad -\sin x,\quad -\cos x,\quad \sin x,\quad \cos x,\ldots
$$

At $x=0$,

$$
\cos 0=1,\qquad -\sin 0=0,\qquad -\cos 0=-1,\qquad \sin 0=0.
$$

Thus the odd coefficients are zero, and

$$
a_{2n}=\frac{(-1)^n}{(2n)!}.
$$

Therefore

$$
\cos x
=\sum_{n=0}^{\infty}\frac{(-1)^n x^{2n}}{(2n)!}
=1-\frac{x^2}{2!}+\frac{x^4}{4!}-\frac{x^6}{6!}+\cdots .
$$

The ratio test gives convergence for all $x$.

#### (13.3) The Series for $e^x$

Let

$$
e^x=\sum_{n=0}^{\infty}a_nx^n.
$$

Since every derivative of $e^x$ is again $e^x$,

$$
f^{(n)}(0)=e^0=1.
$$

Hence

$$
a_n=\frac{1}{n!}.
$$

Therefore

$$
e^x
=\sum_{n=0}^{\infty}\frac{x^n}{n!}
=1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+\frac{x^4}{4!}+\cdots .
$$

The ratio test gives convergence for all $x$.

#### (13.4) The Series for $\ln(1+x)$

Let

$$
f(x)=\ln(1+x).
$$

Then

$$
f'(x)=\frac{1}{1+x},\qquad
f''(x)=-\frac{1}{(1+x)^2},\qquad
f'''(x)=\frac{2!}{(1+x)^3}.
$$

In general, for $n\ge 1$,

$$
f^{(n)}(x)=(-1)^{n-1}\frac{(n-1)!}{(1+x)^n}.
$$

Thus

$$
f(0)=0,
\qquad
f^{(n)}(0)=(-1)^{n-1}(n-1)!.
$$

So

$$
a_0=0,\qquad
a_n=\frac{f^{(n)}(0)}{n!}
=\frac{(-1)^{n+1}}{n}
\quad (n\ge 1).
$$

Therefore

$$
\ln(1+x)
=\sum_{n=1}^{\infty}\frac{(-1)^{n+1}x^n}{n}
=x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}+\cdots .
$$

The power series has radius $1$. At $x=1$ it becomes the alternating harmonic series, so it converges. At $x=-1$ it becomes

$$
-\sum_{n=1}^{\infty}\frac1n,
$$

so it diverges. Hence the interval is

$$
(-1,1].
$$

#### (13.5) The Binomial Series

Let

$$
f(x)=(1+x)^p,
$$

where $p$ is any real number. The derivatives are

$$
f'(x)=p(1+x)^{p-1},
$$

$$
f''(x)=p(p-1)(1+x)^{p-2},
$$

$$
f'''(x)=p(p-1)(p-2)(1+x)^{p-3}.
$$

In general,

$$
f^{(n)}(x)=p(p-1)(p-2)\cdots(p-n+1)(1+x)^{p-n}.
$$

Thus

$$
f^{(n)}(0)=p(p-1)(p-2)\cdots(p-n+1).
$$

Therefore

$$
a_n
=\frac{p(p-1)(p-2)\cdots(p-n+1)}{n!}
=\binom pn.
$$

So

$$
(1+x)^p
=\sum_{n=0}^{\infty}\binom pn x^n
$$

or, written out,

$$
(1+x)^p
=1+px+\frac{p(p-1)}{2!}x^2
+\frac{p(p-1)(p-2)}{3!}x^3+\cdots .
$$

For a general real $p$, the binomial series converges for

$$
|x|<1.
$$

Endpoint behavior depends on $p$, but the basic binomial expansion is the power series about $x=0$ with radius $1$ unless the series terminates.
