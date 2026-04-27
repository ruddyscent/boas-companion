# 1-1. The Geometric Series

### Problem 1. Bouncing Ball

The ball starts 1 m above the floor and rebounds to $\tfrac23$ of its previous height.

**Tenth rebound**

$$
h_{10}=\left(\frac23\right)^{10}
=\frac{1024}{59049}
\approx 0.0173\text{ m}.
$$

**Distance through the tenth floor hit**

After the first 1 m fall, each bounce contributes an up-and-down distance:

$$
D_{10}
=1+2\sum_{k=1}^{9}\left(\frac23\right)^k
=1+2\cdot\frac{(2/3)\bigl[1-(2/3)^9\bigr]}{1-2/3}
=5-4\left(\frac23\right)^9.
$$

Since $(2/3)^9\approx 0.02601$,

$$
D_{10}\approx 4.896\text{ m}.
$$

**Total distance**

$$
D_{\infty}
=1+2\sum_{k=1}^{\infty}\left(\frac23\right)^k
=1+2\cdot\frac{2/3}{1-2/3}
=5\text{ m}.
$$

By the tenth hit, the ball has traveled about $4.896/5=97.9\%$ of the total distance.

### Problem 2. Geometric Sum Formula

Let

$$
S_n=a+ar+ar^2+\cdots+ar^{n-1}.
$$

Multiply by $r$ and subtract:

$$
rS_n=ar+ar^2+\cdots+ar^n,
$$

so

$$
S_n-rS_n=a-ar^n.
$$

Therefore

$$
\boxed{S_n=\frac{a(1-r^n)}{1-r}\quad(r\ne 1).}
$$

If $|r|<1$, then $r^n\to 0$, so

$$
S=\frac{a}{1-r}.
$$

Thus a geometric series converges exactly when $|r|<1$.

## Repeating Decimals to Fractions (Problems 3-11)

Use the same method each time: multiply by a power of 10 and subtract to cancel the repeating block.

### Problem 3. One-Digit Repetend

For $x=0.\overline{5}$,

$$
10x-x=5
\quad\Rightarrow\quad
x=\frac59.
$$

### Problem 4. Two-Digit Repetend

For $x=0.\overline{81}$,

$$
100x-x=81
\quad\Rightarrow\quad
x=\frac{81}{99}=\frac9{11}.
$$

### Problem 5. Mixed Repeating Decimal

For $x=0.58\overline{3}$,

$$
1000x-100x=583-58=525
\quad\Rightarrow\quad
x=\frac{525}{900}=\frac7{12}.
$$

### Problem 6. Mixed Repeating Decimal

For $x=0.6\overline{1}$,

$$
100x-10x=61-6=55
\quad\Rightarrow\quad
x=\frac{55}{90}=\frac{11}{18}.
$$

### Problem 7. Three-Digit Repetend

For $x=0.\overline{185}$,

$$
1000x-x=185
\quad\Rightarrow\quad
x=\frac{185}{999}=\frac5{27}.
$$

### Problem 8. Mixed Repeating Decimal

For $x=0.69\overline{4}$,

$$
10000x-1000x=6944-694=6250
\quad\Rightarrow\quad
x=\frac{6250}{9000}=\frac{25}{36}.
$$

### Problem 9. Repetend of $1/7$

For $x=0.\overline{857142}$,

$$
10^6x-x=857142
\quad\Rightarrow\quad
x=\frac{857142}{999999}=\frac67.
$$

### Problem 10. Six-Digit Repetend

For $x=0.\overline{576923}$,

$$
10^6x-x=576923
\quad\Rightarrow\quad
x=\frac{576923}{999999}=\frac{15}{26}.
$$

### Problem 11. Mixed Repeating Decimal

For $x=0.67\overline{857142}$,

$$
10^8x-10^2x=67857142-67=67857075,
$$

so

$$
x=\frac{67857075}{99999900}=\frac{19}{28}.
$$

### Problem 12. Water Purification

The removed amounts form

$$
\frac1n,\;\frac{1}{n^2},\;\frac{1}{n^3},\;\dots
$$

So the total removed is

$$
T=\sum_{k=1}^{\infty}\frac{1}{n^k}
=\frac{1/n}{1-1/n}
=\frac{1}{n-1}.
$$

- If $n=2$, then $T=1$: all impurity can be removed in theory.
- If $n=3$, then $T=1/2$: at least half remains.

### Problem 13. Monthly Investment

The monthly factor is $1.005$. Depositing \$10 at the beginning of each month for 120 months gives

$$
A=10\sum_{k=1}^{120}(1.005)^k
=10\cdot 1.005\cdot\frac{(1.005)^{120}-1}{0.005}
=2010\bigl[(1.005)^{120}-1\bigr].
$$

Since $(1.005)^{120}\approx 1.81940$,

$$
A\approx \$1{,}647.
$$

The principal is $\$1{,}200$, so the interest is about $\$447$.

### Problem 14. Divergent Geometric Series

For

$$
\sum_{n=0}^{\infty}(-5)^n,
$$

the ratio is $r=-5$, so $|r|>1$. The series **diverges**.

The value $1/6$ comes from applying $a/(1-r)$ without checking the condition $|r|<1$.

### Problem 15. Sierpiński Gasket

At stage $n$, the removed triangles have total area

$$
\frac{3^{n-1}}{4^n}.
$$

Thus the total removed area is

$$
A_{\text{removed}}
=\sum_{n=1}^{\infty}\frac{3^{n-1}}{4^n}
=\frac14\sum_{n=0}^{\infty}\left(\frac34\right)^n
=1.
$$

Therefore the remaining Sierpiński gasket has area 0.

### Problem 16. Partially Reflected Particles

At each endpoint, a fraction $r$ reflects and a fraction $1-r$ escapes.

**Escape at $x=1$**

Arrivals at $x=1$ have sizes $1,r^2,r^4,\dots$, so

$$
P_1=(1-r)\sum_{k=0}^{\infty}r^{2k}
=\frac{1-r}{1-r^2}
=\frac{1}{1+r}.
$$

**Escape at $x=0$**

Returns to $x=0$ have sizes $r,r^3,r^5,\dots$, so

$$
P_0=(1-r)\sum_{k=0}^{\infty}r^{2k+1}
=\frac{(1-r)r}{1-r^2}
=\frac{r}{1+r}.
$$

Check:

$$
P_0+P_1=1.
$$

Since $r/(1+r)$ increases on $0<r<1$,

$$
\sup_{0<r<1}\frac{r}{1+r}
=\frac12.
$$

So less than half of the particles escape at $x=0$, though the fraction can get arbitrarily close to $1/2$.
