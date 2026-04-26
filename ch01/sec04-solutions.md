# 1-4. Convergent and Divergent Series

> 모든 문제에서 일반항 $a_n$, 부분합 $S_n$, 그리고 잔차 $R_n = S - S_n$ 의 닫힌 식을 구한 뒤 $n\to\infty$ 일 때의 극한을 살핀다.
> 표기 규약: 합의 시작 인덱스가 어디든 $S_n$ 은 "보이는 모든 항 가운데 인덱스가 $n$ 이하인 것들의 합"으로 둔다(즉 $\sum_{k=1}^{\infty}$ 형태이면 $S_n = a_1+\cdots+a_n$, $\sum_{k=0}^{\infty}$ 형태이면 $S_n = a_0+\cdots+a_n$).

## 문제 1. 공비 $1/2$ 의 단순 등비급수

대상 급수는 $\displaystyle\sum_{n=1}^{\infty}\frac{1}{2^{n}}$ 이다. 등비급수 합 공식 $S_n = a(1-r^n)/(1-r)$ 에 $a=r=1/2$ 를 대입하면

$$
a_n = \frac{1}{2^{n}},\qquad
S_n = 1 - \frac{1}{2^{n}},\qquad
R_n = S - S_n = \frac{1}{2^{n}}.
$$

극한: $a_n\to 0,\; S_n\to 1,\; R_n\to 0$. **수렴, $S=1$.**

## 문제 2. 0부터 시작하는 공비 $1/5$ 등비급수

대상 급수는 $\displaystyle\sum_{n=0}^{\infty}\frac{1}{5^{n}}$ 이다. $S_n = a_0+a_1+\cdots+a_n$ 이 $n+1$ 개의 항을 갖는 점에 유의:

$$
a_n = \frac{1}{5^{n}},\qquad
S_n = \frac{1-(1/5)^{n+1}}{1-1/5} = \frac{5}{4}\left(1-\frac{1}{5^{n+1}}\right),\qquad
R_n = \frac{5}{4}\cdot\frac{1}{5^{n+1}} = \frac{1}{4\cdot 5^{n}}.
$$

극한: $a_n\to 0,\; S_n\to \tfrac{5}{4},\; R_n\to 0$. **수렴, $S=5/4$.**

## 문제 3. 공비 $-1/2$ 의 교대 등비급수

급수 $1 - \tfrac{1}{2} + \tfrac{1}{4} - \tfrac{1}{8} + \tfrac{1}{16} - \cdots$ 는 $a=1,\; r=-\tfrac{1}{2}$ 인 등비급수이므로

$$
a_n = \left(-\frac{1}{2}\right)^{n-1},\qquad
S_n = \frac{1-(-1/2)^{n}}{1-(-1/2)} = \frac{2}{3}\left(1-\left(-\frac{1}{2}\right)^{n}\right),\qquad
R_n = \frac{2}{3}\left(-\frac{1}{2}\right)^{n}.
$$

극한: $a_n\to 0,\; S_n\to \tfrac{2}{3},\; R_n\to 0$. **수렴, $S=2/3$.**

## 문제 4. 지수표기를 풀어 환원되는 등비급수 ($r=1/3$)

힌트대로 $e^{-\ln 3} = 1/3$ 이므로 $e^{-n\ln 3} = (1/3)^{n}$. 따라서 $\displaystyle\sum_{n=1}^{\infty} e^{-n\ln 3}$ 는 $a=r=1/3$ 의 등비급수와 같다.

$$
a_n = \frac{1}{3^{n}},\qquad
S_n = \frac{1}{2}\left(1-\frac{1}{3^{n}}\right),\qquad
R_n = \frac{1}{2\cdot 3^{n}}.
$$

극한: $a_n\to 0,\; S_n\to \tfrac{1}{2},\; R_n\to 0$. **수렴, $S=1/2$.**

## 문제 5. 삼각함수 지수표기를 단순화한 등비급수 ($r=3/4$)

$\sin(\pi/3) = \sqrt{3}/2$ 이므로

$$
e^{2n\ln\sin(\pi/3)} = \bigl(\sin(\pi/3)\bigr)^{2n} = \left(\frac{\sqrt{3}}{2}\right)^{\!2n} = \left(\frac{3}{4}\right)^{\!n}.
$$

따라서 $\displaystyle\sum_{n=0}^{\infty} e^{2n\ln\sin(\pi/3)}$ 는 0부터 시작하는 공비 $3/4$ 등비급수이다.

$$
a_n = \left(\frac{3}{4}\right)^{n},\qquad
S_n = \frac{1-(3/4)^{n+1}}{1-3/4} = 4 - 3\left(\frac{3}{4}\right)^{n},\qquad
R_n = 3\left(\frac{3}{4}\right)^{n}.
$$

극한: $a_n\to 0,\; S_n\to 4,\; R_n\to 0$. **수렴, $S=4$.**

## 문제 6. 부분분수로 분해되는 망원급수 (telescoping)

힌트의 $\dfrac{1}{n(n+1)} = \dfrac{1}{n} - \dfrac{1}{n+1}$ 를 사용하면 부분합이 망원으로 사라진다.

$$
a_n = \frac{1}{n(n+1)} = \frac{1}{n}-\frac{1}{n+1},
$$

$$
S_n = \sum_{k=1}^{n}\!\left(\frac{1}{k}-\frac{1}{k+1}\right)
     = 1-\frac{1}{n+1} = \frac{n}{n+1},\qquad
R_n = 1 - S_n = \frac{1}{n+1}.
$$

극한: $a_n\to 0,\; S_n\to 1,\; R_n\to 0$. **수렴, $S=1$.**

## 문제 7. 교대 망원급수 — $\dfrac{2n+1}{n(n+1)}$ 의 부호 교대 합

급수 $\dfrac{3}{1\cdot 2} - \dfrac{5}{2\cdot 3} + \dfrac{7}{3\cdot 4} - \dfrac{9}{4\cdot 5} + \cdots$ 의 일반항을 살피면

$$
a_n = (-1)^{n+1}\,\frac{2n+1}{n(n+1)}
    = (-1)^{n+1}\!\left(\frac{1}{n}+\frac{1}{n+1}\right),
$$

이때 $\dfrac{2n+1}{n(n+1)} = \dfrac{1}{n}+\dfrac{1}{n+1}$ 임을 사용했다.

부분합을 정리하기 위해 교대조화수 $A_n = \displaystyle\sum_{k=1}^{n}\frac{(-1)^{k+1}}{k}$ 를 도입하면

$$
S_n = \sum_{k=1}^{n}(-1)^{k+1}\!\left(\frac{1}{k}+\frac{1}{k+1}\right)
     = A_n + \bigl(1 - A_{n+1}\bigr) = 1 - (A_{n+1}-A_n)
     = 1 + \frac{(-1)^{n+1}}{n+1}.
$$

검산: $S_1 = 1 + \tfrac{1}{2} = \tfrac{3}{2}$, $S_2 = 1 - \tfrac{1}{3} = \tfrac{2}{3}$, $S_3 = 1 + \tfrac{1}{4} = \tfrac{5}{4}$. 모두 직접 계산과 일치.

따라서 $S = 1$ 이고

$$
R_n = S - S_n = -\frac{(-1)^{n+1}}{n+1} = \frac{(-1)^{n}}{n+1}.
$$

극한: $a_n\to 0,\; S_n\to 1,\; R_n\to 0$. **수렴, $S=1$.** (절댓값이 $\sim 2/n$ 이므로 절대수렴은 아니고 조건수렴.)
