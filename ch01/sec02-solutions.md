# 1-2. Definitions and Notation

## 문제 1. 제곱근을 포함한 유리식 — 최고차항 정규화

대상 수열은 $\dfrac{n^{2}+5n^{3}}{2n^{3}+3\sqrt{4+n^{6}}}$ 이다. 분자·분모를 최고차항 $n^{3}$ 으로 나눈다.

$$
\frac{n^{2}+5n^{3}}{2n^{3}+3\sqrt{4+n^{6}}}
= \frac{5+\dfrac{1}{n}}{2+3\sqrt{\dfrac{4}{n^{6}}+1}}
\;\xrightarrow[n\to\infty]{}\;
\frac{5}{2+3} = \boxed{1}.
$$

## 문제 2. 다항식 / 제곱근 다항식 — 분자·분모를 같은 위계로 정규화

대상 수열은 $\dfrac{(n+1)^{2}}{\sqrt{3+5n^{2}+4n^{4}}}$ 이다. 분자는 $\sim n^{2}$, 분모는 $\sqrt{4n^{4}+\cdots}\sim 2n^{2}$. 모든 항을 $n^{2}$로 나누어 정리하면

$$
\frac{(n+1)^{2}}{\sqrt{3+5n^{2}+4n^{4}}}
= \frac{\bigl(1+\tfrac{1}{n}\bigr)^{2}}{\sqrt{\tfrac{3}{n^{4}}+\tfrac{5}{n^{2}}+4}}
\;\xrightarrow[n\to\infty]{}\;
\frac{1}{\sqrt{4}} = \boxed{\dfrac{1}{2}}.
$$

## 문제 3. 교대 부호 수열의 절댓값 압축

대상 수열은 $\dfrac{(-1)^{n}\sqrt{n+1}}{n}$ 이다. 부호와 무관하게 절댓값이 0으로 가면 수렴한다.

$$
\left|\frac{(-1)^{n}\sqrt{n+1}}{n}\right|
= \frac{\sqrt{n+1}}{n}
= \sqrt{\frac{n+1}{n^{2}}}
\;\xrightarrow[n\to\infty]{}\; 0.
$$

스퀴즈 정리에 의해 $\boxed{0}$.

## 문제 4. 지수함수가 다항함수를 압도

대상 수열은 $\dfrac{2^{n}}{n^{2}}$ 이다. 지수함수가 다항식보다 빨리 커진다. 비율판정으로 확인하면

$$
\frac{a_{n+1}}{a_{n}} = \frac{2^{n+1}}{(n+1)^{2}}\cdot\frac{n^{2}}{2^{n}}
= 2\left(\frac{n}{n+1}\right)^{2}\;\xrightarrow[n\to\infty]{}\;2>1.
$$

따라서 수열은 발산하며 $\boxed{\,2^{n}/n^{2}\to\infty\,}$.

## 문제 5. 계승이 지수함수를 압도

대상 수열은 $\dfrac{10^{n}}{n!}$ 이다. 비율을 보면

$$
\frac{a_{n+1}}{a_{n}} = \frac{10^{n+1}}{(n+1)!}\cdot\frac{n!}{10^{n}} = \frac{10}{n+1}\;\xrightarrow[n\to\infty]{}\;0.
$$

비율이 1보다 작은 값으로 수렴하므로 수열 자체는 0으로 간다. $\boxed{0}$.

(일반적으로 임의의 상수 $c$에 대해 $c^{n}/n!\to 0$.)

## 문제 6. $n^{n}$ 이 계승을 압도 — 비율판정에 $e$ 가 등장

대상 수열은 $\dfrac{n^{n}}{n!}$ 이다.

$$
\frac{a_{n+1}}{a_{n}}
= \frac{(n+1)^{n+1}}{(n+1)!}\cdot\frac{n!}{n^{n}}
= \frac{(n+1)^{n}}{n^{n}}
= \left(1+\frac{1}{n}\right)^{n}\;\xrightarrow[n\to\infty]{}\;e.
$$

$e>1$ 이므로 수열은 발산하여 $\boxed{\,n^{n}/n!\to\infty\,}$.

(스털링 공식 $n!\sim\sqrt{2\pi n}\,(n/e)^{n}$ 으로도 같은 결론: $n^{n}/n!\sim e^{n}/\sqrt{2\pi n}\to\infty$.)

## 문제 7. 로그 변환으로 푸는 거듭제곱 극한

대상 수열은 $(1+n^{2})^{1/\ln n}$ 이다. 로그를 취한다.

$$
\ln\bigl[(1+n^{2})^{1/\ln n}\bigr] = \frac{\ln(1+n^{2})}{\ln n}.
$$

$n\to\infty$ 에서 $\ln(1+n^{2})=\ln n^{2}+\ln(1+n^{-2}) = 2\ln n + o(1)$ 이므로

$$
\frac{\ln(1+n^{2})}{\ln n}\;\xrightarrow[n\to\infty]{}\;2.
$$

따라서 원래 수열은 $\boxed{e^{2}}$ 로 수렴한다.

## 문제 8. 중심 이항계수의 역수 — 비율판정

대상 수열은 $\dfrac{(n!)^{2}}{(2n)!} = \dfrac{1}{\binom{2n}{n}}$ 이다. 비율판정으로 살피면

$$
\frac{a_{n+1}}{a_{n}}
= \frac{((n+1)!)^{2}}{(2n+2)!}\cdot\frac{(2n)!}{(n!)^{2}}
= \frac{(n+1)^{2}}{(2n+1)(2n+2)}
= \frac{n+1}{2(2n+1)}
\;\xrightarrow[n\to\infty]{}\;\frac{1}{4}.
$$

극한 비율이 $1/4<1$ 이므로 $a_n\to 0$. $\boxed{0}$.

## 문제 9. $\sin x / x$ 극한의 변형

대상 수열은 $n\sin(1/n)$ 이다. $x=1/n$ 으로 놓으면 $n\to\infty$ 일 때 $x\to 0^{+}$이고

$$
n\sin\!\frac{1}{n} = \frac{\sin x}{x}\;\xrightarrow[x\to 0]{}\;1.
$$

따라서 $\boxed{1}$.

(테일러 전개로 보면 $n\sin(1/n)=1-\dfrac{1}{6n^{2}}+O(n^{-4})$.)
