# 1-2. Definitions and Notation

### Problem 1. Normalize by $n^3$

Divide the numerator and denominator by $n^3$:

$$
\frac{n^{2}+5n^{3}}{2n^{3}+3\sqrt{4+n^{6}}}
= \frac{5+\dfrac{1}{n}}{2+3\sqrt{\dfrac{4}{n^{6}}+1}}
\;\xrightarrow[n\to\infty]{}\;
\frac{5}{2+3} = \boxed{1}.
$$

### Problem 2. Normalize by $n^2$

The numerator and denominator are both of order $n^2$. Divide by $n^2$:

$$
\frac{(n+1)^{2}}{\sqrt{3+5n^{2}+4n^{4}}}
= \frac{\bigl(1+\tfrac{1}{n}\bigr)^{2}}{\sqrt{\tfrac{3}{n^{4}}+\tfrac{5}{n^{2}}+4}}
\;\xrightarrow[n\to\infty]{}\;
\frac{1}{\sqrt{4}} = \boxed{\dfrac{1}{2}}.
$$

### Problem 3. Use Absolute Values

The sign alternates, but the absolute value tends to 0:

$$
\left|\frac{(-1)^{n}\sqrt{n+1}}{n}\right|
= \frac{\sqrt{n+1}}{n}
= \sqrt{\frac{n+1}{n^{2}}}
\;\xrightarrow[n\to\infty]{}\; 0.
$$

So the limit is $\boxed{0}$.

### Problem 4. Exponential Beats Polynomial

For $a_n=2^n/n^2$,

$$
\frac{a_{n+1}}{a_n}
=2\left(\frac{n}{n+1}\right)^2
\;\xrightarrow[n\to\infty]{}\;2>1.
$$

Thus $2^n/n^2\to\infty$.

### Problem 5. Factorial Beats Exponential

For $a_n=10^n/n!$,

$$
\frac{a_{n+1}}{a_n}
=\frac{10}{n+1}
\;\xrightarrow[n\to\infty]{}\;0.
$$

Therefore $a_n\to \boxed{0}$.

### Problem 6. $n^n$ Beats $n!$

For $a_n=n^n/n!$,

$$
\frac{a_{n+1}}{a_n}
= \frac{(n+1)^{n}}{n^{n}}
= \left(1+\frac{1}{n}\right)^{n}
\;\xrightarrow[n\to\infty]{}\;e>1.
$$

Thus $n^n/n!\to\infty$.

### Problem 7. Take Logarithms

Let

$$
L_n=(1+n^2)^{1/\ln n}.
$$

Then

$$
\ln L_n=\frac{\ln(1+n^2)}{\ln n}
\;\xrightarrow[n\to\infty]{}\;2,
$$

because $\ln(1+n^2)=2\ln n+o(1)$. Therefore

$$
L_n\to \boxed{e^2}.
$$

### Problem 8. Central Binomial Coefficient

Let $a_n=(n!)^2/(2n)!$. Then

$$
\frac{a_{n+1}}{a_n}
= \frac{(n+1)^2}{(2n+1)(2n+2)}
= \frac{n+1}{2(2n+1)}
\;\xrightarrow[n\to\infty]{}\;\frac14.
$$

Since the ratio is less than 1, $a_n\to \boxed{0}$.

### Problem 9. Use $\sin x/x$

Set $x=1/n$. Then $x\to 0^+$ and

$$
n\sin\!\frac{1}{n}
=\frac{\sin x}{x}
\;\xrightarrow[x\to 0]{}\;1.
$$

So the limit is $\boxed{1}$.
