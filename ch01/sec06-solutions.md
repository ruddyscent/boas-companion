# 1-6. Convergence Tests for Series of Positive Terms; Absolute Convergence

> 본 절은 네 가지 판정법을 차례로 다룬다 — **비교판정(A)**, **적분판정(B)**, **비율판정(C)**, **특수 비교판정(D)**. 문제도 그 순서대로 묶여 있다.

---

## A. 비교판정 (Comparison Test) — 문제 1–6

## 문제 1. $n! > 2^{n}$ ($n>3$) — 귀납법

기저: $4! = 24 > 16 = 2^{4}$. 귀납가정 $n!>2^{n}$ ($n\ge 4$)에서 $n+1$ 단계로 갈 때 $n!$ 은 $n+1$ 배($\ge 5$), $2^{n}$ 은 $2$ 배가 곱해지므로

$$
(n+1)! = (n+1)\cdot n! \;>\; (n+1)\cdot 2^{n} \;>\; 2\cdot 2^{n} = 2^{\,n+1}.
$$

따라서 모든 $n\ge 4$ 에서 $n!>2^{n}$.

## 문제 2. 조화급수의 발산 — 이항분리 묶기로 비교

힌트의 보조 급수는

$$
1+\tfrac12 + (\tfrac14+\tfrac14) + (\tfrac18+\tfrac18+\tfrac18+\tfrac18) + (\text{8개 each } \tfrac{1}{16}) + \cdots
= 1 + \tfrac12+\tfrac12+\tfrac12+\cdots
$$

이며 부분합이 무한대로 발산한다. 한편 조화급수는

$$
1 + \tfrac12 + (\tfrac13+\tfrac14) + (\tfrac15+\tfrac16+\tfrac17+\tfrac18) + \cdots
$$

각 묶음의 항이 보조 급수의 대응 항보다 같거나 크다($\tfrac13>\tfrac14,\;\tfrac14=\tfrac14$ 이므로 $\tfrac13+\tfrac14 > \tfrac14+\tfrac14 = \tfrac12$ 등). 따라서 비교판정에 의해 조화급수도 발산.

## 문제 3. $\sum 1/n^{2}$ 의 수렴 — 같은 방식의 묶기

$2^{k}$ 개씩 묶으면 $k$번째 묶음의 모든 항은 $\le 1/(2^{k})^{2} = 1/4^{k}$ 이므로

$$
\sum_{n=2^{k}}^{2^{k+1}-1}\frac{1}{n^{2}} \;\le\; 2^{k}\cdot\frac{1}{4^{k}} = \frac{1}{2^{k}}.
$$

따라서 $\displaystyle\sum_{n=1}^{\infty}\frac{1}{n^{2}} \le \sum_{k=0}^{\infty}\frac{1}{2^{k}} = 2$. 유한한 상계가 있으므로 수렴.

## 문제 4. 등비급수와의 비교

(a) $\displaystyle\sum_{n=1}^{\infty}\frac{1}{2^{n}+3^{n}}$ : 분모 $\ge 3^{n}$ 이므로 $a_n \le 1/3^{n}$. $\sum 1/3^{n}$ (등비, $r=1/3$) 이 수렴하므로 **수렴**.

(b) $\displaystyle\sum_{n=1}^{\infty}\frac{1}{n\,2^{n}}$ : $1/(n\,2^{n})\le 1/2^{n}$, 등비급수와 비교해 **수렴**.

## 문제 5. 조화급수와의 비교

(a) $\displaystyle\sum_{n=1}^{\infty}\frac{1}{\sqrt{n}}$ : $n\ge\sqrt{n}$ 이므로 $1/\sqrt{n}\ge 1/n$. 조화급수 발산을 이용해 **발산**. (힌트: $n>\sqrt{n}$.)

(b) $\displaystyle\sum_{n=2}^{\infty}\frac{1}{\ln n}$ : $\ln n < n$ 이므로 $1/\ln n > 1/n$. **발산**.

## 문제 6. 자릿수 묶기로 본 조화급수의 발산

자릿수 $d$ 인 자연수는 정확히 $9\cdot 10^{d-1}$ 개. 그 자연수들의 역수는 모두 $\ge 1/10^{d}$. 따라서 묶음별 합은

$$
\underbrace{\tfrac{1}{1}+\cdots+\tfrac{1}{9}}_{9\text{개},\ \ge 9/10}
+\underbrace{\tfrac{1}{10}+\cdots+\tfrac{1}{99}}_{90\text{개},\ \ge 9/10}
+\underbrace{\tfrac{1}{100}+\cdots+\tfrac{1}{999}}_{900\text{개},\ \ge 9/10}+\cdots.
$$

각 묶음이 $9/10$ 이상이고 묶음의 개수는 무한이므로 부분합 $\to\infty$. **발산**.

---

## B. 적분판정 (Integral Test) — 문제 7–17

> 양의 단조감소 함수 $f$ 에 대하여 $\sum_{n\ge a} f(n)$ 과 $\int_{a}^{\infty} f(x)\,dx$ 는 **수렴/발산이 같다.**

## 문제 7. $\sum 1/(n\ln n)$ — $\ln(\ln x)$ 로 발산

$$
\int_{2}^{\infty}\frac{dx}{x\ln x} = \bigl[\ln(\ln x)\bigr]_{2}^{\infty} = \infty.\quad\text{**발산**.}
$$

## 문제 8. $\sum n/(n^{2}+4)$ — 본질적으로 $1/n$

$$
\int_{1}^{\infty}\frac{x\,dx}{x^{2}+4} = \tfrac{1}{2}\bigl[\ln(x^{2}+4)\bigr]_{1}^{\infty} = \infty.\quad\text{**발산**.}
$$

## 문제 9. $\sum_{n\ge 3} 1/(n^{2}-4)$ — 부분분수 + 적분판정

$\dfrac{1}{x^{2}-4} = \tfrac{1}{4}\!\left(\dfrac{1}{x-2}-\dfrac{1}{x+2}\right)$ 이므로

$$
\int_{3}^{\infty}\frac{dx}{x^{2}-4} = \tfrac{1}{4}\Bigl[\ln\tfrac{x-2}{x+2}\Bigr]_{3}^{\infty}
= \tfrac{1}{4}\bigl(0-\ln\tfrac{1}{5}\bigr) = \tfrac{\ln 5}{4}<\infty.\quad\text{**수렴**.}
$$

## 문제 10. $\sum e^{n}/(e^{2n}+9)$ — $u=e^{x}$ 치환

$u=e^{x}$ 로 치환하면

$$
\int_{1}^{\infty}\frac{e^{x}\,dx}{e^{2x}+9} = \int_{e}^{\infty}\frac{du}{u^{2}+9}
= \tfrac{1}{3}\bigl[\arctan(u/3)\bigr]_{e}^{\infty}
= \tfrac{1}{3}\bigl(\tfrac{\pi}{2}-\arctan\tfrac{e}{3}\bigr)<\infty.\quad\text{**수렴**.}
$$

## 문제 11. $\sum 1/[n(1+\ln n)^{3/2}]$ — $u=1+\ln x$

$u=1+\ln x$, $du=dx/x$ :

$$
\int_{1}^{\infty}\frac{dx}{x(1+\ln x)^{3/2}}
= \int_{1}^{\infty}\frac{du}{u^{3/2}}
= \bigl[-2u^{-1/2}\bigr]_{1}^{\infty} = 2<\infty.\quad\text{**수렴**.}
$$

## 문제 12. $\sum n/(n^{2}+1)^{2}$

$$
\int_{1}^{\infty}\frac{x\,dx}{(x^{2}+1)^{2}} = \Bigl[-\tfrac{1}{2(x^{2}+1)}\Bigr]_{1}^{\infty} = \tfrac{1}{4}.\quad\text{**수렴**.}
$$

## 문제 13. $\sum n^{2}/(n^{3}+1)$ — 본질적으로 $1/n$

$$
\int_{1}^{\infty}\frac{x^{2}\,dx}{x^{3}+1} = \tfrac{1}{3}\bigl[\ln(x^{3}+1)\bigr]_{1}^{\infty}=\infty.\quad\text{**발산**.}
$$

## 문제 14. $\sum 1/\sqrt{n^{2}+9}$ — 본질적으로 $1/n$

$$
\int_{1}^{\infty}\frac{dx}{\sqrt{x^{2}+9}} = \bigl[\ln(x+\sqrt{x^{2}+9})\bigr]_{1}^{\infty}=\infty.\quad\text{**발산**.}
$$

## 문제 15. $p$-급수 판정의 증명

$p\ne 1$ 일 때

$$
\int_{1}^{\infty} x^{-p}\,dx = \Bigl[\tfrac{x^{1-p}}{1-p}\Bigr]_{1}^{\infty}
= \begin{cases} \dfrac{1}{p-1}, & p>1\;(\text{유한})\\[2pt] \infty, & p<1.\end{cases}
$$

$p=1$ 인 경우는 $\int_{1}^{\infty} dx/x = \ln x \to\infty$, 즉 발산. 정리하면

$$
\sum_{n=1}^{\infty}\frac{1}{n^{p}} \;\text{는}\;\;
\begin{cases}\text{수렴} & p>1\\ \text{발산} & p\le 1.\end{cases}
$$

## 문제 16. 적분 하한 0의 함정

학생이 사용한 $\displaystyle\int_{0}^{\infty} n^{-2}\,dn$ 은 **하한 $0$** 때문에 $1/n^2$ 의 0 근방 발산이 끼어들어 무한대가 된 것이다. 적분판정은 "꼬리"의 거동만을 보는 것이므로 $f$가 단조감소·양인 임의의 $a>0$ 에서 $\int_{a}^{\infty} f(x)\,dx$ 의 유한성으로 판정해야 한다. 실제로 $\int_{1}^{\infty} x^{-2}dx = 1<\infty$ 이므로 $\sum 1/n^{2}$ 은 수렴한다.

## 문제 17. $\sum e^{-n^{2}}$ — 비교적분으로 유한

$n\ge 1$ 에서 $n^{2}\ge n$ 이므로 $e^{-n^{2}}\le e^{-n}$. 따라서

$$
\int_{1}^{\infty} e^{-x^{2}}\,dx \;\le\; \int_{1}^{\infty} e^{-x}\,dx = e^{-1}<\infty.
$$

적분이 유한하므로(즉 그 값을 못 구해도 유한임은 보장) **수렴**.

---

## C. 비율판정 (Ratio Test) — 문제 18–30

> $\rho := \lim |a_{n+1}/a_n|$ 이 존재하면 $\rho<1$ 이면 절대수렴, $\rho>1$ 이면 발산, $\rho=1$ 은 판정 불가.

## 문제 18. $\sum 2^{n}/n^{2}$

$\dfrac{a_{n+1}}{a_{n}} = 2\cdot\!\left(\dfrac{n}{n+1}\right)^{2}\to 2>1.$ **발산**.

## 문제 19. $\sum 3^{n}/2^{2n}$ — 등비

$a_n = (3/4)^{n}$, 비율 $3/4<1$. **수렴**.

## 문제 20. $\sum n!/(2n)!$

$\dfrac{a_{n+1}}{a_{n}} = \dfrac{n+1}{(2n+1)(2n+2)} = \dfrac{1}{2(2n+1)}\to 0<1.$ **수렴**.

## 문제 21. $\sum 5^{n}(n!)^{2}/(2n)!$

$\dfrac{a_{n+1}}{a_{n}} = \dfrac{5(n+1)^{2}}{(2n+1)(2n+2)} = \dfrac{5(n+1)}{2(2n+1)}\to \dfrac{5}{4}>1.$ **발산**.

## 문제 22. $\sum 10^{n}/(n!)^{2}$

$\dfrac{a_{n+1}}{a_{n}} = \dfrac{10}{(n+1)^{2}}\to 0.$ **수렴**.

## 문제 23. $\sum n!/100^{n}$

$\dfrac{a_{n+1}}{a_{n}} = \dfrac{n+1}{100}\to\infty.$ **발산**.

## 문제 24. $\sum 3^{2n}/2^{3n} = \sum (9/8)^{n}$

등비, $r=9/8>1$. **발산**.

## 문제 25. $\sum e^{n}/\sqrt{n!}$

$\dfrac{a_{n+1}}{a_{n}} = \dfrac{e}{\sqrt{n+1}}\to 0.$ **수렴**.

## 문제 26. $\sum (n!)^{3} e^{3n}/(3n)!$

$$
\frac{a_{n+1}}{a_{n}} = \frac{(n+1)^{3}\,e^{3}}{(3n+1)(3n+2)(3n+3)}
\;\xrightarrow[n\to\infty]{}\; \frac{e^{3}}{27}.
$$

$e^{3}\approx 20.09 < 27$ 이므로 비율 $<1$. **수렴**. (비율이 1보다 약간 작은 미묘한 경계.)

## 문제 27. $\sum 100^{n}/n^{200}$

$\dfrac{a_{n+1}}{a_{n}} = 100\!\left(\dfrac{n}{n+1}\right)^{200}\to 100>1.$ **발산**. (다항보다 지수가 결국 압도.)

## 문제 28. $\sum n!(2n)!/(3n)!$

$$
\frac{a_{n+1}}{a_{n}} = \frac{(n+1)(2n+1)(2n+2)}{(3n+1)(3n+2)(3n+3)}
= \frac{2(n+1)(2n+1)}{3(3n+1)(3n+2)}\;\xrightarrow{}\;\frac{4}{27}<1.
$$

**수렴**.

## 문제 29. $\sum \sqrt{(2n)!}/n!$

$$
\frac{a_{n+1}}{a_{n}} = \frac{\sqrt{(2n+1)(2n+2)}}{n+1} = \sqrt{\frac{2(2n+1)}{n+1}}\to\sqrt{4}=2>1.
$$

**발산**.

## 문제 30. 비율판정의 증명

**$\rho<1$ 인 경우**: $\rho<\sigma<1$ 이 되도록 $\sigma$ 를 잡으면, 충분히 큰 $n\ge N$ 에서 $|a_{n+1}/a_{n}|<\sigma$. 따라서 $|a_{N+k}|<\sigma^{k}|a_{N}|$ 이고

$$
\sum_{k=1}^{\infty}|a_{N+k}| < |a_{N}|\sum_{k=1}^{\infty}\sigma^{k} = \frac{\sigma|a_{N}|}{1-\sigma}<\infty,
$$

즉 $\sum |a_{n}|$ 의 꼬리가 등비급수에 의해 끼어 수렴한다. 절대수렴이므로 본 급수도 수렴.

**$\rho>1$ 인 경우**: $1<\sigma<\rho$ 가 되도록 $\sigma$ 를 잡으면 큰 $n$ 에서 $|a_{n+1}|>\sigma|a_{n}|$, 따라서 $|a_{n}|\ge\sigma^{n-N}|a_{N}|\to\infty$. 일반항이 0으로 가지 않으므로 예비판정에 의해 **발산**.

---

## D. 특수 비교판정 (Special Comparison Test) — 문제 31–37

> $a_n/b_n \to L$ ($0<L<\infty$) 이면 $\sum a_n$ 과 $\sum b_n$ 은 같이 수렴하거나 같이 발산.

## 문제 31. $\sum (2n+1)(3n-5)/\sqrt{n^{2}-73}$ — $b_n = n$

$$
\frac{a_n}{b_n} = \frac{(2n+1)(3n-5)}{n\sqrt{n^{2}-73}}\;\xrightarrow[n\to\infty]{}\;\frac{6n^{2}}{n\cdot n}=6.
$$

$\sum n$ 이 발산하므로 **발산**. (사실 일반항이 무한대로 가서 예비판정으로도 발산.)

## 문제 32. $\sum n(n+1)/[(n+2)^{2}(n+3)]$ — $b_n = 1/n$

$\dfrac{a_n}{1/n} = \dfrac{n^{2}(n+1)}{(n+2)^{2}(n+3)}\to 1$. 조화급수와 같은 거동, **발산**.

## 문제 33. $\sum 1/(2^{n}-n^{2})$ — $b_n = 1/2^{n}$

$\dfrac{a_n}{1/2^{n}} = \dfrac{1}{1-n^{2}/2^{n}}\to 1$ ($n^{2}\ll 2^{n}$). 등비급수와 같은 거동, **수렴**.

## 문제 34. $\sum (n^{2}+3n+4)/(n^{4}+7n^{3}+6n-3)$ — $b_n = 1/n^{2}$

$\dfrac{a_n}{1/n^{2}} \to 1$. $p$-급수 $p=2>1$ 와 같은 거동, **수렴**.

## 문제 35. $\sum (n-\ln n)^{2}/(5n^{4}-3n^{2}+1)$ — $b_n = 1/n^{2}$

$n-\ln n \sim n$ 이므로 $(n-\ln n)^{2}\sim n^{2}$, $a_n \sim n^{2}/(5n^{4}) = 1/(5n^{2})$. $a_n/b_n \to 1/5$. **수렴**.

## 문제 36. $\sum \sqrt{n^{3}+5n-1}/(n^{2}-\sin n^{3})$ — $b_n = 1/\sqrt{n}$

분자 $\sim n^{3/2}$, 분모 $\sim n^{2}$ ($\sin n^{3}$ 은 유계). $a_n \sim n^{3/2}/n^{2} = n^{-1/2}$, $a_n/b_n \to 1$. $p=1/2\le 1$ 인 $p$-급수와 같으므로 **발산**.

## 문제 37. 특수 비교판정 (a)의 증명

$a_n/b_n \to L$ 이고 $M>L$ 이라 하자. 극한의 정의에 의해 충분히 큰 $n\ge N$ 에서 $a_n/b_n < M$, 즉 $a_n < M b_n$. $\sum b_n$ 이 수렴하면 $\sum M b_n = M\sum b_n$ 도 수렴. 보통의 비교판정에 의해 $\sum_{n\ge N} a_n \le \sum_{n\ge N} M b_n$ 이 유한하므로 $\sum a_n$ 도 수렴. (앞쪽 유한 개 항은 수렴 여부에 영향이 없다.)
