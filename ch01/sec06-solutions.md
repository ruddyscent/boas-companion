# 1-6. Convergence Tests for Series of Positive Terms; Absolute Convergence

This section uses four tests:

- **Comparison Test**
- **Integral Test**
- **Ratio Test**
- **Special Comparison Test**

## A. Comparison Test: Problems 1-6

### Problem 1. Factorials Eventually Dominate Powers of 2

Base case: $4! = 24 > 16 = 2^{4}$.

Assume $n!>2^{n}$ for some $n\ge 4$. Then

$$
(n+1)! = (n+1)n! > (n+1)2^{n} > 2\cdot 2^{n}=2^{n+1}.
$$

Therefore $n!>2^{n}$ for all $n\ge 4$.

### Problem 2. Harmonic Series

Group the harmonic series in powers of 2:

$$
1+\frac12+\left(\frac13+\frac14\right)
+\left(\frac15+\frac16+\frac17+\frac18\right)+\cdots.
$$

Each group is at least $\frac12$:

$$
\frac13+\frac14>\frac14+\frac14=\frac12,\qquad
\frac15+\cdots+\frac18>4\cdot\frac18=\frac12.
$$

Since infinitely many groups each contribute at least $\frac12$, the harmonic series **diverges**.

### Problem 3. Reciprocal-Square Series

Group terms with $2^{k}\le n\le 2^{k+1}-1$. There are $2^{k}$ terms, and each is at most $1/(2^{k})^{2}$:

$$
\sum_{n=2^{k}}^{2^{k+1}-1}\frac{1}{n^{2}}
\le 2^{k}\cdot\frac{1}{4^{k}}
=\frac{1}{2^{k}}.
$$

Thus

$$
\sum_{n=1}^{\infty}\frac{1}{n^{2}}
\le \sum_{k=0}^{\infty}\frac{1}{2^{k}}=2,
$$

so the series **converges**.

### Problem 4. Compare with Geometric Series

(a)

$$
\frac{1}{2^{n}+3^{n}}\le \frac{1}{3^{n}}.
$$

Since $\sum 1/3^{n}$ converges, $\displaystyle\sum_{n=1}^{\infty}\frac{1}{2^{n}+3^{n}}$ **converges**.

(b)

$$
\frac{1}{n2^{n}}\le \frac{1}{2^{n}}.
$$

Since $\sum 1/2^{n}$ converges, $\displaystyle\sum_{n=1}^{\infty}\frac{1}{n2^{n}}$ **converges**.

### Problem 5. Compare with the Harmonic Series

(a) Since $\sqrt n\le n$ for $n\ge 1$,

$$
\frac{1}{\sqrt n}\ge \frac{1}{n}.
$$

So $\displaystyle\sum_{n=1}^{\infty}\frac{1}{\sqrt n}$ **diverges**.

(b) Since $\ln n<n$ for $n\ge 2$,

$$
\frac{1}{\ln n}>\frac{1}{n}.
$$

So $\displaystyle\sum_{n=2}^{\infty}\frac{1}{\ln n}$ **diverges**.

### Problem 6. Harmonic Series by Number of Digits

There are $9\cdot 10^{d-1}$ integers with $d$ digits, and each reciprocal is at least $1/10^{d}$. Therefore each digit block contributes at least

$$
9\cdot 10^{d-1}\cdot\frac{1}{10^{d}}=\frac{9}{10}.
$$

Infinitely many blocks each contribute at least $9/10$, so the harmonic series **diverges**.

## B. Integral Test: Problems 7-17

For a positive decreasing function $f$, the series $\sum f(n)$ and the improper integral $\int f(x)\,dx$ have the same convergence behavior.

### Problem 7

$$
\int_{2}^{\infty}\frac{dx}{x\ln x}
=\bigl[\ln(\ln x)\bigr]_{2}^{\infty}
=\infty.
$$

Therefore the series **diverges**.

### Problem 8

$$
\int_{1}^{\infty}\frac{x\,dx}{x^{2}+4}
=\frac12\bigl[\ln(x^{2}+4)\bigr]_{1}^{\infty}
=\infty.
$$

Therefore the series **diverges**.

### Problem 9

Use

$$
\frac{1}{x^{2}-4}
=\frac14\left(\frac{1}{x-2}-\frac{1}{x+2}\right).
$$

Then

$$
\int_{3}^{\infty}\frac{dx}{x^{2}-4}
=\frac14\Bigl[\ln\frac{x-2}{x+2}\Bigr]_{3}^{\infty}
=\frac{\ln 5}{4}<\infty.
$$

Therefore the series **converges**.

### Problem 10

Let $u=e^{x}$, so $du=e^{x}\,dx$:

$$
\int_{1}^{\infty}\frac{e^{x}\,dx}{e^{2x}+9}
=\int_{e}^{\infty}\frac{du}{u^{2}+9}
=\frac13\bigl[\arctan(u/3)\bigr]_{e}^{\infty}<\infty.
$$

Therefore the series **converges**.

### Problem 11

Let $u=1+\ln x$, so $du=dx/x$:

$$
\int_{1}^{\infty}\frac{dx}{x(1+\ln x)^{3/2}}
=\int_{1}^{\infty}u^{-3/2}\,du
=\bigl[-2u^{-1/2}\bigr]_{1}^{\infty}
=2.
$$

Therefore the series **converges**.

### Problem 12

$$
\int_{1}^{\infty}\frac{x\,dx}{(x^{2}+1)^{2}}
=\Bigl[-\frac{1}{2(x^{2}+1)}\Bigr]_{1}^{\infty}
=\frac14.
$$

Therefore the series **converges**.

### Problem 13

$$
\int_{1}^{\infty}\frac{x^{2}\,dx}{x^{3}+1}
=\frac13\bigl[\ln(x^{3}+1)\bigr]_{1}^{\infty}
=\infty.
$$

Therefore the series **diverges**.

### Problem 14

$$
\int_{1}^{\infty}\frac{dx}{\sqrt{x^{2}+9}}
=\bigl[\ln(x+\sqrt{x^{2}+9})\bigr]_{1}^{\infty}
=\infty.
$$

Therefore the series **diverges**.

### Problem 15. The $p$-Series Test

For $p\ne 1$,

$$
\int_{1}^{\infty}x^{-p}\,dx
=\Bigl[\frac{x^{1-p}}{1-p}\Bigr]_{1}^{\infty}
$$

If $p>1$, then $x^{1-p}\to 0$, so

$$
\int_{1}^{\infty}x^{-p}\,dx
=\frac{1}{p-1}<\infty.
$$

If $p<1$, then $x^{1-p}\to\infty$, so the integral diverges. For $p=1$,

$$
\int_{1}^{\infty}\frac{dx}{x}=\infty.
$$

Therefore $\sum_{n=1}^{\infty}1/n^p$ **converges for $p>1$** and **diverges for $p\le 1$**.

### Problem 16. Do Not Start the Integral at 0

The integral test checks the tail of a series, not behavior near 0. The student's integral

$$
\int_{0}^{\infty}n^{-2}\,dn
$$

is infinite only because $n^{-2}$ blows up near 0. The correct tail integral is

$$
\int_{1}^{\infty}x^{-2}\,dx=1<\infty.
$$

So $\sum 1/n^{2}$ **converges**.

### Problem 17

For $x\ge 1$, $x^{2}\ge x$, so $e^{-x^{2}}\le e^{-x}$. Hence

$$
\int_{1}^{\infty}e^{-x^{2}}\,dx
\le \int_{1}^{\infty}e^{-x}\,dx
=e^{-1}<\infty.
$$

Therefore $\sum e^{-n^{2}}$ **converges** by the integral test.

## C. Ratio Test: Problems 18-30

If

$$
\rho=\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|,
$$

then $\rho<1$ gives absolute convergence, $\rho>1$ gives divergence, and $\rho=1$ is inconclusive.

### Problem 18

For $a_n=2^n/n^2$,

$$
\frac{a_{n+1}}{a_n}
=2\left(\frac{n}{n+1}\right)^2
\to 2>1.
$$

Therefore the series **diverges**.

### Problem 19

Rewrite the series as

$$
\sum \frac{3^n}{2^{2n}}
=\sum \left(\frac34\right)^n.
$$

This is a geometric series with ratio $3/4<1$, so it **converges**.

### Problem 20

For $a_n=n!/(2n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{n+1}{(2n+1)(2n+2)}
=\frac{1}{2(2n+1)}
\to 0.
$$

Therefore the series **converges**.

### Problem 21

For $a_n=5^n(n!)^2/(2n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{5(n+1)^2}{(2n+1)(2n+2)}
\to \frac54>1.
$$

Therefore the series **diverges**.

### Problem 22

For $a_n=10^n/(n!)^2$,

$$
\frac{a_{n+1}}{a_n}
=\frac{10}{(n+1)^2}
\to 0.
$$

Therefore the series **converges**.

### Problem 23

For $a_n=n!/100^n$,

$$
\frac{a_{n+1}}{a_n}
=\frac{n+1}{100}
\to \infty.
$$

Therefore the series **diverges**.

### Problem 24

Rewrite the series as

$$
\sum \frac{3^{2n}}{2^{3n}}
=\sum \left(\frac98\right)^n.
$$

This is a geometric series with ratio $9/8>1$, so it **diverges**.

### Problem 25

For $a_n=e^n/\sqrt{n!}$,

$$
\frac{a_{n+1}}{a_n}
=\frac{e}{\sqrt{n+1}}
\to 0.
$$

Therefore the series **converges**.

### Problem 26

For $a_n=(n!)^{3}e^{3n}/(3n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{(n+1)^3e^3}{(3n+1)(3n+2)(3n+3)}
\to \frac{e^3}{27}<1.
$$

Therefore the series **converges**.

### Problem 27

For $a_n=100^n/n^{200}$,

$$
\frac{a_{n+1}}{a_n}
=100\left(\frac{n}{n+1}\right)^{200}
\to 100>1.
$$

Therefore the series **diverges**.

### Problem 28

For $a_n=n!(2n)!/(3n)!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{(n+1)(2n+1)(2n+2)}{(3n+1)(3n+2)(3n+3)}
\to \frac{4}{27}<1.
$$

Therefore the series **converges**.

### Problem 29

For $a_n=\sqrt{(2n)!}/n!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{\sqrt{(2n+1)(2n+2)}}{n+1}
\to 2>1.
$$

Therefore the series **diverges**.

### Problem 30. Ratio Test

If $\rho<1$, choose $\sigma$ with $\rho<\sigma<1$. For all large $n$,

$$
|a_{n+1}|<\sigma |a_n|.
$$

The tail is bounded by a geometric series, so $\sum |a_n|$ converges.

If $\rho>1$, then for all large $n$ the terms grow in absolute value, so $a_n$ does not tend to 0. The series diverges by the preliminary test.

## D. Special Comparison Test: Problems 31-37

If $a_n,b_n>0$ and

$$
\frac{a_n}{b_n}\to L,\qquad 0<L<\infty,
$$

then $\sum a_n$ and $\sum b_n$ have the same convergence behavior.

### Problem 31

Let

$$
a_n=\frac{(2n+1)(3n-5)}{\sqrt{n^2-73}}.
$$

Compare with $b_n=n$:

$$
\frac{a_n}{b_n}
=\frac{(2n+1)(3n-5)}{n\sqrt{n^2-73}}
\to 6.
$$

Since $\sum n$ diverges, the given series **diverges**. In fact, $a_n\to\infty$, so the preliminary test also proves divergence.

### Problem 32

Let

$$
a_n=\frac{n(n+1)}{(n+2)^2(n+3)}.
$$

Compare with $b_n=1/n$:

$$
\frac{a_n}{b_n}
=\frac{n^2(n+1)}{(n+2)^2(n+3)}
\to 1.
$$

Since $\sum 1/n$ diverges, the given series **diverges**.

### Problem 33

Let

$$
a_n=\frac{1}{2^n-n^2}.
$$

Compare with $b_n=1/2^n$:

$$
\frac{a_n}{b_n}
=\frac{1}{1-n^2/2^n}
\to 1.
$$

Since $\sum 1/2^n$ converges, the given series **converges**.

### Problem 34

Let

$$
a_n=\frac{n^2+3n+4}{n^4+7n^3+6n-3}.
$$

Compare with $b_n=1/n^2$. The highest-degree terms give

$$
\frac{a_n}{b_n}
=\frac{n^2(n^2+3n+4)}{n^4+7n^3+6n-3}
\to 1.
$$

Since $\sum 1/n^2$ converges, the given series **converges**.

### Problem 35

Since $n-\ln n\sim n$,

$$
\frac{(n-\ln n)^2}{5n^4-3n^2+1}
\sim \frac{n^2}{5n^4}
=\frac{1}{5n^2}.
$$

Thus the series behaves like $\sum 1/n^2$, so it **converges**.

### Problem 36

Since $\sin n^3$ is bounded,

$$
\frac{\sqrt{n^3+5n-1}}{n^2-\sin n^3}
\sim \frac{n^{3/2}}{n^2}
=\frac{1}{\sqrt n}.
$$

The comparison series $\sum 1/\sqrt n$ diverges, so the given series **diverges**.

### Problem 37. Special Comparison Test

For convergence: if $\sum b_n$ converges and $a_n/b_n\to L<\infty$, then eventually $a_n\le M b_n$ for some constant $M$. By comparison, $\sum a_n$ converges.

For divergence: if $\sum b_n$ diverges and $a_n/b_n\to L>0$, then eventually $a_n\ge m b_n$ for some constant $m>0$. By comparison, $\sum a_n$ diverges.

The condition $L>0$ is needed for the divergence direction. For example, $a_n=1/n^2$ and $b_n=1/n$ give $a_n/b_n\to 0$, but $\sum a_n$ converges while $\sum b_n$ diverges.
