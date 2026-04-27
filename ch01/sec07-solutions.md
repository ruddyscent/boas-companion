# 1-7. Alternating Series

> **Alternating Series Test**: if $a_n>0$, $a_n$ decreases, and $a_n\to 0$, then $\sum (-1)^n a_n$ converges. Absolute convergence always implies convergence.

### Problem 1. Conditional Convergence

For $\sum (-1)^n/\sqrt n$, the absolute values $1/\sqrt n$ decrease to 0. So the series **converges** by the alternating series test.

### Problem 2. Divergence

For $\sum (-2)^n/n^2$,

$$
|a_n|=\frac{2^n}{n^2}\to\infty.
$$

The terms do not tend to 0, so the series **diverges**.

### Problem 3. Absolute Convergence

For $\sum (-1)^n/n^2$,

$$
\sum |a_n|=\sum \frac{1}{n^2}
$$

converges. Therefore the series is **absolutely convergent**.

### Problem 4. Absolute Convergence

For $\sum (-3)^n/n!$,

$$
\frac{|a_{n+1}|}{|a_n|}
=\frac{3}{n+1}
\to 0.
$$

So the series is **absolutely convergent**.

### Problem 5. Conditional Convergence

For $\sum_{n\ge 2}(-1)^n/\ln n$, the terms $1/\ln n$ decrease to 0. Thus the series **converges** by the alternating series test.

### Problem 6. Divergence

For $\sum (-1)^n n/(n+5)$,

$$
|a_n|=\frac{n}{n+5}\to 1.
$$

The terms do not tend to 0, so the series **diverges**.

### Problem 7. Conditional Convergence

For $\sum_{n\ge 0}(-1)^n n/(1+n^2)$,

$$
\frac{n}{1+n^2}\to 0,
\qquad
\frac{n}{1+n^2}\sim \frac{1}{n}.
$$

The terms are eventually decreasing, so the alternating series test gives **convergence**.

### Problem 8. Conditional Convergence

For $\sum (-1)^n\sqrt{10n}/(n+2)$,

$$
\frac{\sqrt{10n}}{n+2}
\sim \frac{\sqrt{10}}{\sqrt n}
\to 0.
$$

The terms are eventually decreasing, so the series **converges** by the alternating series test.

### Problem 9. Absolute Convergence Implies Convergence

Let $b_n=a_n+|a_n|$. Then

$$
0\le b_n\le 2|a_n|.
$$

If $\sum |a_n|$ converges, then $\sum b_n$ also converges by comparison. Hence

$$
\sum a_n
=\sum (b_n-|a_n|)
=\sum b_n-\sum |a_n|
$$

converges.

### Problem 10. Monotonicity Matters

(a)

$$
2-\frac12+\frac23-\frac14+\frac25-\frac16+\cdots
$$

The absolute values are not decreasing: $\frac12<\frac23$. Pairing terms gives

$$
\frac{2}{2k-1}-\frac{1}{2k}
=\frac{2k+1}{2k(2k-1)}
\sim \frac{1}{2k}.
$$

So the paired series diverges like the harmonic series.

(b)

$$
\frac{1}{\sqrt2}-\frac12+\frac{1}{\sqrt3}-\frac13+\frac{1}{\sqrt4}-\frac14+\cdots
$$

Again, the alternating series test does not apply because the positive magnitudes are not decreasing; for example,

$$
\frac12<\frac{1}{\sqrt3}.
$$
