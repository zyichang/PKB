---
quizify:
  format: 1
  deck: Math_880::Chapter_3
  tags: [Math, 880题, 数一, 第三章, 一元函数积分学]
---
+++

#### 基础选择 (1) 设 $f(x)$ 是连续函数，且 $f(x)\neq0$，若 $\int xf(x)\mathrm{d}x=\arcsin x+C$，则 $\int\dfrac{\mathrm{d}x}{f(x)}=$（　）。

;;;
A. $\dfrac13(1-x^2)^{\frac32}+C$
B. $\dfrac23(1-x^2)^{\frac32}+C$
C. $-\dfrac13(1-x^2)^{\frac32}+C$
D. $-\dfrac23(1-x^2)^{\frac32}+C$
;;;C

***

**C.**

解　已知等式 $\int xf(x)\mathrm{d}x=\arcsin x+C$ 两边同时对 $x$ 求导，得

$$
xf(x)=\frac{1}{\sqrt{1-x^2}},
$$

故 $\dfrac{1}{f(x)}=x\sqrt{1-x^2}$，所以

$$
\int\frac{\mathrm{d}x}{f(x)}=\int x\sqrt{1-x^2}\,\mathrm{d}x=-\frac12\int\sqrt{1-x^2}\,\mathrm{d}(1-x^2)=-\frac13(1-x^2)^{\frac32}+C.
$$

+++

#### 基础选择 (2) 设  是连续函数， 是  的原函数，则（　）。

;;;
A. 当 $f(x)$ 为奇函数时，$F(x)$ 必为偶函数
B. 当 $f(x)$ 为偶函数时，$F(x)$ 必为奇函数
C. 当 $f(x)$ 为周期函数时，$F(x)$ 必为周期函数
D. 当 $f(x)$ 为单调函数时，$F(x)$ 必为单调函数
;;;A

***

**A.**

解　令 $F(x)=\int_a^x f(t)\,\mathrm{d}t$，当 $f(t)$ 是连续的奇函数时，$F(x)$ 是偶函数。

+++

#### 基础选择 (3) 设 $F(x)$ 是 $\sin x^2$ 的一个原函数，则 $\mathrm{d}\big[F(x^2)\big]=$（　）。

;;;
A. $\sin x^4\mathrm{d}x$
B. $\sin x^2\mathrm{d}(x^2)$
C. $2x\sin x^2\mathrm{d}x$
D. $2x\sin x^4\mathrm{d}x$
;;;D

***

**D.**

解　由原函数的定义，知 $F'(t)=\sin t^2$，$\mathrm{d}\big[F(t)\big]=F'(t)\mathrm{d}t=\sin t^2\mathrm{d}t$。

令 $t=x^2$，得 $\mathrm{d}\big[F(x^2)\big]=\sin x^4\mathrm{d}(x^2)=2x\sin x^4\mathrm{d}x$。

+++

#### 基础选择 (4) 设 $f(x)=\begin{cases}\sin x,&0\leqslant x<\pi,\\[1mm] 2,&\pi\leqslant x\leqslant2\pi,\end{cases}$ $F(x)=\int_0^x f(t)\,\mathrm{d}t$，则（　）。

;;;
A. $x=\pi$ 是 $F(x)$ 的跳跃间断点
B. $x=\pi$ 是 $F(x)$ 的可去间断点
C. $F(x)$ 在 $x=\pi$ 处连续但不可导
D. $F(x)$ 在 $x=\pi$ 处可导
;;;C

***

**C.**

解　$x=\pi$ 是 $f(x)$ 的跳跃间断点，故 $f(x)$ 可积，则 $F(x)=\int_0^x f(t)\,\mathrm{d}t$ 在 $x=\pi$ 处连续，但不可导，C 正确。

**【注】**　① 此题利用了结论：设 $F(x)=\int_0^x f(t)\,\mathrm{d}t$，$x\in[a,b]$，则
（ⅰ）$f(x)$ 在 $[a,b]$ 上可积 $\Rightarrow F(x)$ 在 $[a,b]$ 上连续；
（ⅱ）$f(x)$ 在 $[a,b]$ 上连续 $\Rightarrow F(x)$ 在 $[a,b]$ 上可导。
② 若 $f(x)$ 在 $[a,b]$ 上只有有限个第一类间断点，则 $f(x)$ 在 $[a,b]$ 上可积。
③ 若 $f(x)$ 在 $[a,b]$ 上存在第一类间断点，则 $f(x)$ 没有原函数。

+++

#### 基础选择 (5) 设 $f(x)$ 在 $[0,1]$ 上连续，$f(x)>0$，$f'(x)<0$，$f''(x)>0$，记 $M=\int_0^1 f(x)\,\mathrm{d}x$，$N=f(1)$，$P=\dfrac12\big[f(0)+f(1)\big]$，则（　）。

;;;
A. $M<N<P$
B. $N<M<P$
C. $P<M<N$
D. $P<N<M$
;;;B

***

**B.**

解　由已知条件，画出示意图，如图 3-1 所示。由 $f'(x)<0$，知当 $x\in[0,1)$ 时，$f(x)>f(1)$，故 $N=(1-0)f(1)<M=\int_0^1 f(x)\,\mathrm{d}x$。

由 $f''(x)>0$，知

$$
P=\frac12(1-0)\big[f(0)+f(1)\big]>\int_0^1 f(x)\,\mathrm{d}x=M,
$$

故 B 正确。

+++

#### 基础选择 (6) 设 $\lim\limits_{x\to0}\dfrac{1}{\sin x-ax}\displaystyle\int_b^x\dfrac{t^2}{\sqrt{1+t^2}}\,\mathrm{d}t=c$，且 $c\neq0$，则（　）。

;;;
A. $a=1$，$b=0$，$c=-2$
B. $a=1$，$b=-2$，$c=-2$
C. $a=0$，$b=1$，$c=-2$
D. $a=1$，$b=1$，$c=1$
;;;A

***

**A.**

解　当 $x\to0$ 时，$\sin x-ax\to0$，故 $\int_b^x\dfrac{t^2}{\sqrt{1+t^2}}\,\mathrm{d}t\to0$，于是必有 $b=0$。

若 $a\neq1$，则当 $x\to0$ 时，$\sin x-ax$ 与 $x$ 是同阶无穷小，$\int_b^x\dfrac{t^2}{\sqrt{1+t^2}}\,\mathrm{d}t$ 是关于 $x$ 的高阶无穷小，故必有 $c=0$，与题设矛盾，所以 $a=1$。由洛必达法则，有

$$
\lim_{x\to0}\frac{\displaystyle\int_0^x\frac{t^2}{\sqrt{1+t^2}}\,\mathrm{d}t}{\sin x-x}=\lim_{x\to0}\frac{\dfrac{x^2}{\sqrt{1+x^2}}}{\cos x-1}=\lim_{x\to0}\frac{\dfrac{x^2}{\sqrt{1+x^2}}}{-\dfrac12x^2}=-2,
$$

故 A 正确。

+++

#### 基础选择 (7) 下列反常积分收敛的是（　）。

;;;
A. $\int_1^{+\infty}\dfrac{\mathrm{d}x}{x^2\sqrt{1+x}}$
B. $\int_0^1\dfrac{\mathrm{d}x}{\ln(1+x)}$
C. $\int_{-1}^1\dfrac{\mathrm{d}x}{\sin x}$
D. $\int_{-\infty}^{+\infty}\dfrac{x}{\sqrt{1+x^2}}\,\mathrm{d}x$
;;;A

***

**A.**

解　对于 A：利用极限审敛法。由

$$
\lim_{x\to+\infty}x^{\frac52}\,\frac{1}{x^2\sqrt{1+x}}=\lim_{x\to+\infty}\frac{1}{\sqrt{1+\dfrac1x}}=1
$$

$\left(\lambda=\dfrac52>1,\ 0<l=1<+\infty\right)$，知积分收敛。

对于 B：$x=0$ 是 $\dfrac{1}{\ln(1+x)}$ 的瑕点。由

$$
\lim_{x\to0^+}(x-0)\frac{1}{\ln(1+x)}=1\quad(\lambda=1,\ 0<l<1<+\infty),
$$

知积分发散。

对于 C：$x=0$ 是 $\dfrac{1}{\sin x}$ 的瑕点。由

$$
\lim_{x\to0^+}(x-0)\frac{1}{\sin x}=1\quad(\lambda=1,\ 0<l=1<+\infty),
$$

知积分发散。

对于 D：$\int_{-\infty}^{+\infty}\dfrac{x}{\sqrt{1+x^2}}\,\mathrm{d}x=\int_{-\infty}^{1}\dfrac{x}{\sqrt{1+x^2}}\,\mathrm{d}x+\int_1^{+\infty}\dfrac{x}{\sqrt{1+x^2}}\,\mathrm{d}x$。

用定义法，有

$$
\begin{aligned}
\lim_{a\to-\infty}\int_a^1\frac{x\,\mathrm{d}x}{\sqrt{1+x^2}}&=\frac12\lim_{a\to-\infty}\int_a^1\frac{\mathrm{d}(1+x^2)}{\sqrt{1+x^2}}=\frac12\cdot2\lim_{a\to-\infty}\sqrt{1+x^2}\,\bigg|_a^1\\
&=\lim_{a\to-\infty}\left(\sqrt2-\sqrt{1+a^2}\right)=-\infty,
\end{aligned}
$$

故原积分发散。

**【注】**　① 判别反常积分敛散性有两种方法：
（ⅰ）定义法，当积分计算较容易时，选择定义法判别；
（ⅱ）反常积分的审敛法。

（a）设 $I=\int_a^{+\infty}f(x)\,\mathrm{d}x$，$f(x)$ 非负连续，则

$$
\lim_{x\to+\infty}x^{\lambda}f(x)=l,\quad
\begin{cases}
0\leqslant l<+\infty\ \text{且}\ \lambda>1,&\text{则收敛},\\[1mm]
0<l\leqslant+\infty\ \text{且}\ \lambda\leqslant1,&\text{则发散}.
\end{cases}
$$

（b）设 $I=\int_a^b f(x)\,\mathrm{d}x$，$x=a$ 是 $f(x)$ 的瑕点，$f(x)$ 非负连续，则

$$
\lim_{x\to a^+}(x-a)^{\lambda}f(x)=l,\quad
\begin{cases}
0\leqslant l<+\infty\ \text{且}\ 0<\lambda<1,&\text{则收敛},\\[1mm]
0<l\leqslant+\infty\ \text{且}\ \lambda\geqslant1,&\text{则发散}.
\end{cases}
$$

② 两个常用结果：
（ⅰ）$\int_1^{+\infty}\dfrac{\mathrm{d}x}{x^p}$：$p>1$ 时收敛，$p\leqslant1$ 时发散；
（ⅱ）$\int_a^b\dfrac{\mathrm{d}x}{(x-a)^p}$：$p<1$ 时收敛，$p\geqslant1$ 时发散。

+++

#### 基础填空 (1) 设 $F(x)$ 是 $f(x)$ 的一个原函数，$F\!\left(\dfrac{\pi}{4}\right)=0$，当 $\dfrac{\pi}{4}<x<\dfrac{\pi}{2}$ 时，$F(x)>0$，$F(x)f(x)=\dfrac{\ln(\tan x)}{\sin x\cos x}$，则 $f(x)=\underline{\quad}$。

***

$\dfrac{1}{\sin x\cos x}$。

由已知，$F'(x)=f(x)$，故 $2F(x)F'(x)=\dfrac{2\ln(\tan x)}{\sin x\cos x}$。两边同时积分，得

$$
\int 2F(x)F'(x)\,\mathrm{d}x=\int\dfrac{2\ln(\tan x)}{\sin x\cos x}\,\mathrm{d}x,
$$

故

$$
F^2(x)=\int\dfrac{2\ln(\tan x)}{\sin x\cos x}\,\mathrm{d}x=[\ln(\tan x)]^2+C.
$$

将 $F\!\left(\dfrac{\pi}{4}\right)=0$ 代入上式，得 $C=0$，故 $F(x)=\sqrt{[\ln(\tan x)]^2}=\ln(\tan x)$，所以

$$
f(x)=F'(x)=[\ln(\tan x)]'=\dfrac{1}{\sin x\cos x}.
$$

+++

#### 基础填空 (2) 设对任意 $x$，有 $f(x+4)=f(x)$，且 $f'(x)=1+|x|$，$x\in[-2,2]$，$f(0)=1$，则 $f(9)=\underline{\quad}$。

***

$\dfrac{5}{2}$。

由 $f(x+4)=f(x)$，知 $f(9)=f(1)$，而

$$
f'(x)=1+|x|=\begin{cases}1-x,&-2<x<0,\\[1mm] 1+x,&0\leqslant x\leqslant 2,\end{cases}
$$

积分，得

$$
f(x)=\begin{cases}-\dfrac{x^2}{2}+x+C_1,&-2<x<0,\\[1mm] 1,&x=0,\\[1mm] \dfrac{x^2}{2}+x+C_2,&0<x<2.\end{cases}
$$

因为 $f(x)$ 可导，所以 $f(x)$ 在 $x=0$ 处连续，可得 $C_1=C_2=1$，故 $f(9)=f(1)=\dfrac{5}{2}$。

+++

#### 基础填空 (3) (Ⅰ) 设 $f(x)=\displaystyle\int_0^x\sin(x-t)^2\,\mathrm{d}t$，则 $f'(x)=\underline{\quad}$；(Ⅱ) 设 $F(x)=\displaystyle\int_0^x tf(x^2-t^2)\,\mathrm{d}t$，$f(x)$ 是连续函数，则 $F'(x)=\underline{\quad}$；(Ⅲ) 设 $F(x)=\displaystyle\int_0^x tf(x^2-t^2)\,\mathrm{d}t$，$f(x)$ 在 $x=0$ 某邻域内可导，且 $f(0)=0$，$f'(0)=1$，则 $\lim\limits_{x\to0}\dfrac{F(x)}{x^4}=\underline{\quad}$；(Ⅳ) 设 $\alpha(x)=\displaystyle\int_0^{5x}\dfrac{\sin t}{t}\,\mathrm{d}t$，$\beta(x)=\displaystyle\int_0^{\sin x}(1+t)^{\frac{1}{t}}\,\mathrm{d}t$，则 $\lim\limits_{x\to0}\dfrac{\alpha(x)}{\beta(x)}=\underline{\quad}$；(Ⅴ) 极限 $\lim\limits_{x\to0}\dfrac{\displaystyle\int_{\cos x}^1 t\ln t\,\mathrm{d}t}{x^4}=\underline{\quad}$；(Ⅵ) 极限 $\lim\limits_{x\to0}\dfrac{\displaystyle\int_0^x\left[\int_0^{u^2}\arctan(1+t)\,\mathrm{d}t\right]\mathrm{d}u}{x(1-\cos x)}=\underline{\quad}$。

***

(Ⅰ) $\sin x^2$；(Ⅱ) $xf(x^2)$；(Ⅲ) $\dfrac{1}{4}$；(Ⅳ) $\dfrac{5}{\mathrm{e}}$；(Ⅴ) $-\dfrac{1}{8}$；(Ⅵ) $\dfrac{\pi}{6}$。

**(Ⅰ)** 令 $x-t=u$，则

$$
\int_0^x\sin(x-t)^2\,\mathrm{d}t=-\int_x^0\sin u^2\,\mathrm{d}u=\int_0^x\sin u^2\,\mathrm{d}u,
$$

故 $f'(x)=\dfrac{\mathrm{d}}{\mathrm{d}x}\displaystyle\int_0^x\sin u^2\,\mathrm{d}u=\sin x^2$。

**(Ⅱ)** $\displaystyle\int_0^x tf(x^2-t^2)\,\mathrm{d}t=-\dfrac{1}{2}\int_0^x f(x^2-t^2)\,\mathrm{d}(x^2-t^2)$，再令 $x^2-t^2=u$，得

$$
-\dfrac{1}{2}\int_{x^2}^0 f(u)\,\mathrm{d}u=\dfrac{1}{2}\int_0^{x^2}f(u)\,\mathrm{d}u,
$$

故 $F'(x)=\dfrac{\mathrm{d}}{\mathrm{d}x}\left[\dfrac{1}{2}\displaystyle\int_0^{x^2}f(u)\,\mathrm{d}u\right]=xf(x^2)$。

**(Ⅲ)** 利用 (Ⅱ)，有

$$
\lim\limits_{x\to0}\dfrac{F(x)}{x^4}=\lim\limits_{x\to0}\dfrac{xf(x^2)}{4x^3}=\lim\limits_{x\to0}\dfrac{f(x^2)}{4x^2}=\dfrac{1}{4}\lim\limits_{x\to0}\dfrac{f(x^2)-f(0)}{x^2-0}=\dfrac{1}{4}f'(0)=\dfrac{1}{4}.
$$

【注】错误做法：用洛必达法则 $\lim\limits_{x\to0}\dfrac{f(x^2)}{4x^2}=\lim\limits_{x\to0}\dfrac{2xf'(x^2)}{8x}=\dfrac{1}{4}$，由于没有 $f'(x)$ 连续的条件，故 $\lim\limits_{x\to0}f'(x)$ 未必存在。

**(Ⅳ)**

$$
\lim\limits_{x\to0}\dfrac{\alpha(x)}{\beta(x)}=\lim\limits_{x\to0}\dfrac{\displaystyle\int_0^{5x}\dfrac{\sin t}{t}\,\mathrm{d}t}{\displaystyle\int_0^{\sin x}(1+t)^{\frac{1}{t}}\,\mathrm{d}t}=\lim\limits_{x\to0}\dfrac{5\cdot\dfrac{\sin 5x}{5x}}{\cos x\cdot(1+\sin x)^{\frac{1}{\sin x}}}=\dfrac{5}{\mathrm{e}}.
$$

**(Ⅴ)**

$$
\lim\limits_{x\to0}\dfrac{\displaystyle\int_{\cos x}^1 t\ln t\,\mathrm{d}t}{x^4}=\lim\limits_{x\to0}\dfrac{-\displaystyle\int_1^{\cos x}t\ln t\,\mathrm{d}t}{x^4}=\lim\limits_{x\to0}\dfrac{-\cos x\cdot\ln(\cos x)\cdot(-\sin x)}{4x^3}
$$

$$
=\dfrac{1}{4}\lim\limits_{x\to0}\cos x\cdot\lim\limits_{x\to0}\dfrac{\sin x}{x}\cdot\lim\limits_{x\to0}\dfrac{\ln(\cos x)}{x^2}=\dfrac{1}{4}\lim\limits_{x\to0}\dfrac{-\sin x}{2x\cdot\cos x}=-\dfrac{1}{8}.
$$

**(Ⅵ)**

$$
\lim\limits_{x\to0}\dfrac{\displaystyle\int_0^x\left[\int_0^{u^2}\arctan(1+t)\,\mathrm{d}t\right]\mathrm{d}u}{x(1-\cos x)}=\lim\limits_{x\to0}\dfrac{\displaystyle\int_0^{x^2}\arctan(1+t)\,\mathrm{d}t}{\dfrac{3}{2}x^2}=\lim\limits_{x\to0}\dfrac{2x\cdot\arctan(1+x^2)}{3x}=\dfrac{\pi}{6}.
$$

+++

#### 基础填空 (4) 函数 $y=\dfrac{x^2}{\sqrt{1-x^2}}$ 在 $\left[\dfrac{1}{2},\dfrac{\sqrt{3}}{2}\right]$ 上的平均值为 $\underline{\quad}$。

***

$\dfrac{(\sqrt{3}+1)\pi}{12}$。

令 $x=\sin t$，则

$$
\int_{\frac{1}{2}}^{\frac{\sqrt{3}}{2}}\dfrac{x^2}{\sqrt{1-x^2}}\,\mathrm{d}x=\int_{\frac{\pi}{6}}^{\frac{\pi}{3}}\sin^2 t\,\mathrm{d}t=\dfrac{1}{2}\int_{\frac{\pi}{6}}^{\frac{\pi}{3}}(1-\cos 2t)\,\mathrm{d}t=\dfrac{\pi}{12},
$$

故平均值为 $\dfrac{\dfrac{\pi}{12}}{\dfrac{\sqrt{3}}{2}-\dfrac{1}{2}}=\dfrac{(\sqrt{3}+1)\pi}{12}$。

+++

#### 基础填空 (5) 曲线 $y=\dfrac{\sqrt{x}}{1+x^2}$ 绕 $x$ 轴旋转一周所得的旋转体，将它在 $x=0$ 与 $x=\xi\ (\xi>0)$ 之间部分的体积记为 $V(\xi)$，且 $V(a)=\dfrac{1}{2}\lim\limits_{\xi\to+\infty}V(\xi)$，则 $a=\underline{\quad}$。

***

$1$。

依题设，

$$
V(\xi)=\pi\int_0^{\xi}y^2\,\mathrm{d}x=\pi\int_0^{\xi}\dfrac{x}{(1+x^2)^2}\,\mathrm{d}x=\dfrac{\pi}{2}\left(-\dfrac{1}{1+x^2}\right)\bigg|_0^{\xi}=\dfrac{\pi}{2}\left(1-\dfrac{1}{1+\xi^2}\right).
$$

又 $\lim\limits_{\xi\to+\infty}V(\xi)=\dfrac{\pi}{2}$，$V(a)=\dfrac{\pi}{2}\left(1-\dfrac{1}{1+a^2}\right)$，由 $V(a)=\dfrac{1}{2}\lim\limits_{\xi\to+\infty}V(\xi)$，得 $\dfrac{\pi}{2}\left(1-\dfrac{1}{1+a^2}\right)=\dfrac{\pi}{4}$，解得 $a=\pm1$，又 $a>0$，故 $a=1$。

+++

#### 基础填空 (6) 曲线 $r=a\sin^3\dfrac{\theta}{3}\ (a>0,\ 0\leqslant\theta\leqslant 3\pi)$ 的弧长 $s=\underline{\quad}$。

***

$\dfrac{3\pi a}{2}$。

$$
s=\int_0^{3\pi}\sqrt{r^2+r'^2}\,\mathrm{d}\theta=\int_0^{3\pi}\sqrt{a^2\sin^6\dfrac{\theta}{3}+a^2\sin^4\dfrac{\theta}{3}\cos^2\dfrac{\theta}{3}}\,\mathrm{d}\theta=a\int_0^{3\pi}\sin^2\dfrac{\theta}{3}\,\mathrm{d}\theta,
$$

令 $t=\dfrac{\theta}{3}$，得 $s=3a\displaystyle\int_0^{\pi}\sin^2 t\,\mathrm{d}t=\dfrac{3\pi a}{2}$。

+++

#### 基础填空 (7) 曲线 $y=\displaystyle\int_{-\frac{\pi}{2}}^{x}\sqrt{\cos t}\,\mathrm{d}t$ 的全长 $s=\underline{\quad}$。

***

$4$。

函数 $y=\displaystyle\int_{-\frac{\pi}{2}}^{x}\sqrt{\cos t}\,\mathrm{d}t$ 的定义域为 $\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$，全长

$$
s=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\sqrt{1+y'^2}\,\mathrm{d}x=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\sqrt{1+\cos x}\,\mathrm{d}x=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\sqrt{2}\cos\dfrac{x}{2}\,\mathrm{d}x=4.
$$

+++

#### 基础填空 (8) 由曲线 $y=\ln x$ 与两直线 $y=(\mathrm{e}+1)-x$ 及 $y=0$ 所围平面图形的面积 $S=\underline{\quad}$。

***

$\dfrac{3}{2}$。

如图 3-2 所示，

$$
S=\int_0^1\left[(\mathrm{e}+1)-y-\mathrm{e}^y\right]\mathrm{d}y=\dfrac{3}{2},
$$

或

$$
S=\int_1^{\mathrm{e}}\ln x\,\mathrm{d}x+\int_{\mathrm{e}}^{\mathrm{e}+1}(\mathrm{e}+1-x)\,\mathrm{d}x=\dfrac{3}{2}.
$$

+++

#### 基础填空 (9) 设 $D$ 是由曲线 $y=\sin x+1$ 与直线 $x=0$，$x=\pi$，$y=0$ 所围平面图形，则 $D$ 绕 $x$ 轴旋转一周所得旋转体的体积 $V=\underline{\quad}$。

***

$\dfrac{3}{2}\pi^2+4\pi$。

如图 3-3 所示，

$$
V=\int_0^{\pi}\pi(\sin x+1)^2\,\mathrm{d}x=\pi\int_0^{\pi}\left(1+2\sin x+\dfrac{1-\cos 2x}{2}\right)\mathrm{d}x
$$

$$
=\pi\left(\dfrac{3}{2}x-2\cos x-\dfrac{1}{4}\sin 2x\right)\bigg|_0^{\pi}=\dfrac{3}{2}\pi^2+4\pi.
$$

+++

#### 基础填空 (10) 设 $n$ 为正数，$\lim\limits_{x\to0}\left(\dfrac{n-x}{n+x}\right)^{\frac{2}{x}}=\displaystyle\int_{\frac{1}{n}}^{+\infty}x\mathrm{e}^{-4x}\,\mathrm{d}x$，则 $n=\underline{\quad}$。

***

$\dfrac{4}{15}$。

$$
\lim\limits_{x\to0}\left(\dfrac{n-x}{n+x}\right)^{\frac{2}{x}}=\lim\limits_{x\to0}\left[\left(1-\dfrac{2x}{n+x}\right)^{-\frac{n+x}{2x}}\right]^{\frac{-4}{n+x}}=\mathrm{e}^{-\frac{4}{n}},
$$

$$
\int_{\frac{1}{n}}^{+\infty}x\mathrm{e}^{-4x}\,\mathrm{d}x=-\dfrac{1}{4}x\mathrm{e}^{-4x}\bigg|_{\frac{1}{n}}^{+\infty}+\dfrac{1}{4}\int_{\frac{1}{n}}^{+\infty}\mathrm{e}^{-4x}\,\mathrm{d}x=\dfrac{1}{4n}\mathrm{e}^{-\frac{4}{n}}-\dfrac{1}{16}\mathrm{e}^{-4x}\bigg|_{\frac{1}{n}}^{+\infty}=\dfrac{1}{4n}\mathrm{e}^{-\frac{4}{n}}+\dfrac{1}{16}\mathrm{e}^{-\frac{4}{n}},
$$

故 $\left(\dfrac{1}{4n}+\dfrac{1}{16}\right)\mathrm{e}^{-\frac{4}{n}}=\mathrm{e}^{-\frac{4}{n}}$，解得 $n=\dfrac{4}{15}$。

+++

#### 基础解答 (1) 求下列积分：

（Ⅰ）$\displaystyle\int\dfrac{2^x\cdot3^x}{9^x-4^x}\mathrm{d}x$；
（Ⅱ）$\displaystyle\int\dfrac{\mathrm{d}x}{x^2(1-x^4)}$；
（Ⅲ）$\displaystyle\int\dfrac{\mathrm{d}x}{x^4(1+x^2)}$；
（Ⅳ）$\displaystyle\int\dfrac{\arctan x}{x^2(1+x^2)}\mathrm{d}x$；
（Ⅴ）$\displaystyle\int\dfrac{x+\ln(1-x)}{x^2}\mathrm{d}x$．

***

（Ⅰ）

$$
\begin{aligned}
\int\frac{2^x\cdot3^x}{9^x-4^x}\mathrm{d}x&=\int\frac{6^x\mathrm{d}x}{4^x\left[\left(\frac94\right)^x-1\right]}=\int\frac{\left(\frac32\right)^x\mathrm{d}x}{\left[\left(\frac32\right)^x\right]^2-1}\\
&=\frac{1}{\ln\frac32}\int\frac{\mathrm{d}\left[\left(\frac32\right)^x\right]}{\left[\left(\frac32\right)^x\right]^2-1}=\frac{1}{2\ln\frac32}\ln\left|\frac{3^x-2^x}{3^x+2^x}\right|+C.
\end{aligned}
$$

【注】$\displaystyle\int\dfrac{\mathrm{d}x}{x^2-1}=\dfrac12\ln\left|\dfrac{x-1}{x+1}\right|+C.$

（Ⅱ）

$$
\begin{aligned}
\int\frac{\mathrm{d}x}{x^2(1-x^4)}&=\int\frac{x^2}{x^4(1-x^4)}\mathrm{d}x=\int x^2\left(\frac{1}{x^4}+\frac{1}{1-x^4}\right)\mathrm{d}x\\
&=\int\frac{1}{x^2}\mathrm{d}x+\int\frac{1+x^2-1}{1-x^4}\mathrm{d}x\\
&=-\frac1x+\int\frac{\mathrm{d}x}{1-x^2}-\int\frac{\mathrm{d}x}{1-x^4}\\
&=-\frac1x+\int\frac{\mathrm{d}x}{1-x^2}-\frac12\int\left(\frac{1}{1-x^2}+\frac{1}{1+x^2}\right)\mathrm{d}x\\
&=-\frac1x+\frac12\int\frac{\mathrm{d}x}{1-x^2}-\frac12\int\frac{\mathrm{d}x}{1+x^2}\\
&=-\frac1x+\frac14\ln\left|\frac{1+x}{1-x}\right|-\frac12\arctan x+C.
\end{aligned}
$$

（Ⅲ）利用倒代换，令 $x=\dfrac1t$，则

$$
\begin{aligned}
\int\frac{\mathrm{d}x}{x^4(1+x^2)}&=-\int\frac{t^4}{1+t^2}\mathrm{d}t=-\int\frac{t^4-1+1}{1+t^2}\mathrm{d}t=-\int(t^2-1)\mathrm{d}t-\int\frac{\mathrm{d}t}{1+t^2}\\
&=-\frac13t^3+t-\arctan t+C=-\frac{1}{3x^3}+\frac1x-\arctan\frac1x+C.
\end{aligned}
$$

（Ⅳ）考虑到 $\dfrac{1}{x^2(1+x^2)}=\dfrac{1}{x^2}-\dfrac{1}{1+x^2}$，故

$$
\begin{aligned}
\int\frac{\arctan x}{x^2(1+x^2)}\mathrm{d}x&=\int\frac{\arctan x}{x^2}\mathrm{d}x-\int\frac{\arctan x}{1+x^2}\mathrm{d}x\\
&=-\int\arctan x\,\mathrm{d}\left(\frac1x\right)-\int\arctan x\,\mathrm{d}(\arctan x)\\
&=-\frac{\arctan x}{x}+\int\frac{\mathrm{d}x}{x(1+x^2)}-\frac12(\arctan x)^2\\
&=-\frac{\arctan x}{x}+\frac12\int\left(\frac{1}{x^2}-\frac{1}{1+x^2}\right)\mathrm{d}(x^2)-\frac12(\arctan x)^2\\
&=-\frac{\arctan x}{x}-\frac12(\arctan x)^2+\frac12\ln\frac{x^2}{1+x^2}+C.
\end{aligned}
$$

（Ⅴ）

$$
\begin{aligned}
\int\frac{x+\ln(1-x)}{x^2}\mathrm{d}x&=\int\frac{\mathrm{d}x}{x}+\int\frac{\ln(1-x)}{x^2}\mathrm{d}x\\
&=\ln|x|-\int\ln(1-x)\mathrm{d}\left(\frac1x\right)\\
&=\ln|x|-\frac{\ln(1-x)}{x}-\int\frac{\mathrm{d}x}{x(1-x)}\\
&=\ln|x|-\frac{\ln(1-x)}{x}-\int\left(\frac1x+\frac{1}{1-x}\right)\mathrm{d}x\\
&=\left(1-\frac1x\right)\ln(1-x)+C.
\end{aligned}
$$

+++

#### 基础解答 (2) 求下列积分：

（Ⅰ）$\displaystyle\int\dfrac{\mathrm{d}x}{x(1+\sqrt{x})}$；
（Ⅱ）$\displaystyle\int\dfrac{x\mathrm{e}^x}{\sqrt{\mathrm{e}^x-1}}\mathrm{d}x$；
（Ⅲ）$\displaystyle\int\dfrac{x^3}{\sqrt{1+x^2}}\mathrm{d}x$；
（Ⅳ）$\displaystyle\int\dfrac{\mathrm{d}x}{(2x^2+1)\sqrt{1+x^2}}$；
（Ⅴ）$\displaystyle\int\dfrac{\arctan\sqrt{x-1}}{x\sqrt{x-1}}\mathrm{d}x$；
（Ⅵ）$\displaystyle\int\sqrt{\dfrac{x}{1-x\sqrt{x}}}\mathrm{d}x$．

***

（Ⅰ）令 $\sqrt{x}=t$，则 $x=t^2$，故

$$
\begin{aligned}
I=\int\frac{\mathrm{d}x}{x(1+\sqrt{x})}&=\int\frac{2t\mathrm{d}t}{t^2(1+t)}=2\int\frac{\mathrm{d}t}{t(1+t)}\\
&=2\int\left(\frac1t-\frac{1}{1+t}\right)\mathrm{d}t=2[\ln t-\ln(1+t)]+C\\
&=2[\ln\sqrt{x}-\ln(1+\sqrt{x})]+C=2\ln\frac{\sqrt{x}}{1+\sqrt{x}}+C.
\end{aligned}
$$

（Ⅱ）

$$
\begin{aligned}
\int\frac{x\mathrm{e}^x}{\sqrt{\mathrm{e}^x-1}}\mathrm{d}x&=2\int x\,\mathrm{d}(\sqrt{\mathrm{e}^x-1})=2\left(x\sqrt{\mathrm{e}^x-1}-\int\sqrt{\mathrm{e}^x-1}\,\mathrm{d}x\right)\\
&=2x\sqrt{\mathrm{e}^x-1}-2\int\sqrt{\mathrm{e}^x-1}\,\mathrm{d}x,
\end{aligned}
$$

令 $\sqrt{\mathrm{e}^x-1}=t$，则 $x=\ln(1+t^2)$，$\mathrm{d}x=\dfrac{2t}{1+t^2}\mathrm{d}t$，故

$$
\begin{aligned}
\int\sqrt{\mathrm{e}^x-1}\,\mathrm{d}x&=\int\frac{2t^2}{1+t^2}\mathrm{d}t=2\int\frac{t^2+1-1}{1+t^2}\mathrm{d}t\\
&=2t-2\int\frac{\mathrm{d}t}{1+t^2}=2t-2\arctan t+C,
\end{aligned}
$$

所以原式 $=2x\sqrt{\mathrm{e}^x-1}-4\sqrt{\mathrm{e}^x-1}+4\arctan\sqrt{\mathrm{e}^x-1}+C.$

（Ⅲ）令 $x=\tan t,\ t\in\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$，则 $\mathrm{d}x=\sec^2t\mathrm{d}t$，故

$$
\begin{aligned}
I=\int\frac{x^3}{\sqrt{1+x^2}}\mathrm{d}x&=\int\frac{\tan^3t\cdot\sec^2t}{\sec t}\mathrm{d}t\\
&=\int\tan^2t\,\mathrm{d}(\sec t)=\int(\sec^2t-1)\mathrm{d}(\sec t)\\
&=\frac13\sec^3t-\sec t+C.
\end{aligned}
$$

如图 3-4 所示，$\sec t=\sqrt{1+x^2}$，于是原式

$$
I=\frac13(1+x^2)^{\frac32}-(1+x^2)^{\frac12}+C.
$$

【注】此题也可凑微分．

$$
\begin{aligned}
\int\frac{x^3}{\sqrt{1+x^2}}\mathrm{d}x&=\int\frac{x^2\cdot\mathrm{d}(1+x^2)}{2\sqrt{1+x^2}}=\int(x^2+1-1)\mathrm{d}(\sqrt{1+x^2})\\
&=\int(\sqrt{x^2+1})^2\mathrm{d}(\sqrt{1+x^2})-\int\mathrm{d}(\sqrt{1+x^2})\\
&=\frac13(1+x^2)^{\frac32}-(1+x^2)^{\frac12}+C.
\end{aligned}
$$

（Ⅳ）令 $\tan t=x$，则 $\mathrm{d}x=\sec^2t\mathrm{d}t$，故

$$
\begin{aligned}
I=\int\frac{\mathrm{d}x}{(2x^2+1)\sqrt{1+x^2}}&=\int\frac{\mathrm{d}t}{(2\tan^2t+1)\cos t}\\
&=\int\frac{\cos t\mathrm{d}t}{2\sin^2t+\cos^2t}=\int\frac{\mathrm{d}(\sin t)}{1+\sin^2t}=\arctan(\sin t)+C.
\end{aligned}
$$

又 $\sin t=\dfrac{x}{\sqrt{1+x^2}}$，故 $I=\arctan\dfrac{x}{\sqrt{1+x^2}}+C.$

（Ⅴ）

$$
\begin{aligned}
\int\frac{\arctan\sqrt{x-1}}{x\sqrt{x-1}}\mathrm{d}x&=2\int\frac{\arctan\sqrt{x-1}}{x}\mathrm{d}(\sqrt{x-1})\\
&=2\int\frac{\arctan\sqrt{x-1}}{1+(\sqrt{x-1})^2}\mathrm{d}(\sqrt{x-1})\\
&=2\int\arctan\sqrt{x-1}\,\mathrm{d}(\arctan\sqrt{x-1})\\
&=(\arctan\sqrt{x-1})^2+C.
\end{aligned}
$$

（Ⅵ）

$$
\begin{aligned}
\int\sqrt{\frac{x}{1-x\sqrt{x}}}\mathrm{d}x&=\int\frac{\sqrt{x}}{\sqrt{1-x\sqrt{x}}}\mathrm{d}x=\frac23\int\frac{\mathrm{d}(x^{\frac32})}{\sqrt{1-x^{\frac32}}}=-\frac23\int\frac{\mathrm{d}(1-x^{\frac32})}{\sqrt{1-x^{\frac32}}}\\
&=-\frac23\cdot2\int\mathrm{d}(\sqrt{1-x^{\frac32}})=-\frac43\sqrt{1-x\sqrt{x}}+C.
\end{aligned}
$$

+++

#### 基础解答 (3) 求下列积分：

（Ⅰ）$\displaystyle\int\dfrac{\mathrm{d}x}{\sin^2x\cos^4x}$；
（Ⅱ）$\displaystyle\int\dfrac{\mathrm{d}x}{1+\sin x}$；
（Ⅲ）$\displaystyle\int\dfrac{\sin x}{\sin x+\cos x}\mathrm{d}x$；
（Ⅳ）$\displaystyle\int\dfrac{3\sin x+\cos x}{\sin x+2\cos x}\mathrm{d}x$；
（Ⅴ）$\displaystyle\int\dfrac{\mathrm{d}x}{\sin 2x+2\sin x}$；
（Ⅵ）$\displaystyle\int\dfrac{\mathrm{d}x}{a^2\sin^2x+b^2\cos^2x}\ (a^2+b^2>0)$．

***

（Ⅰ）

$$
\begin{aligned}
\int\frac{1}{\sin^2x\cos^4x}\mathrm{d}x&=\int\frac{(\sin^2x+\cos^2x)^2}{\sin^2x\cos^4x}\mathrm{d}x\\
&=\int\left(\frac{\sin^2x}{\cos^4x}+\frac{2}{\cos^2x}+\frac{1}{\sin^2x}\right)\mathrm{d}x\\
&=\int\tan^2x\,\mathrm{d}(\tan x)+2\tan x-\cot x\\
&=\frac13\tan^3x+2\tan x-\cot x+C.
\end{aligned}
$$

【注】求解三角有理式积分首先考虑利用恒等变形、三角公式，一般的方法是利用万能代换．

此题也可以分子分母同乘以 $\cos^2x$，得

$$
\begin{aligned}
\int\frac{1}{\sin^2x\cos^4x}\mathrm{d}x&=\int\frac{1}{\tan^2x\cos^6x}\mathrm{d}x=\int\frac{\sec^4x}{\tan^2x}\mathrm{d}(\tan x)\\
&=\int\frac{\tan^4x+2\tan^2x+1}{\tan^2x}\mathrm{d}(\tan x)\\
&=\frac13\tan^3x+2\tan x-\cot x+C.
\end{aligned}
$$

（Ⅱ）分子分母同时乘以 $(1-\sin x)$，再凑微分．

$$
\begin{aligned}
\int\frac{1}{1+\sin x}\mathrm{d}x&=\int\frac{1-\sin x}{\cos^2x}\mathrm{d}x=\int\frac{1}{\cos^2x}\mathrm{d}x+\int\frac{1}{\cos^2x}\mathrm{d}(\cos x)\\
&=\tan x-\frac{1}{\cos x}+C.
\end{aligned}
$$

【注】利用三角公式．

$$
\begin{aligned}
\int\frac{1}{1+\sin x}\mathrm{d}x&=\int\frac{1}{1+2\sin\frac x2\cos\frac x2}\mathrm{d}x=\int\frac{\mathrm{d}x}{\left(\sin\frac x2+\cos\frac x2\right)^2}\\
&=\int\frac{\sec^2\frac x2}{\left(1+\tan\frac x2\right)^2}\mathrm{d}x=2\int\frac{\mathrm{d}\left(\tan\frac x2\right)}{\left(1+\tan\frac x2\right)^2}=-\frac{2}{1+\tan\frac x2}+C.
\end{aligned}
$$

（Ⅲ）

$$
\begin{aligned}
\int\frac{\sin x}{\sin x+\cos x}\mathrm{d}x&=\frac12\int\frac{(\sin x+\cos x)+(\sin x-\cos x)}{\sin x+\cos x}\mathrm{d}x\\
&=\frac12\int\mathrm{d}x-\frac12\int\frac{\mathrm{d}(\sin x+\cos x)}{\sin x+\cos x}\\
&=\frac12x-\frac12\ln|\sin x+\cos x|+C.
\end{aligned}
$$

【注】这里利用了

$$
f(x)=\frac{f(x)+f(-x)}{2}+\frac{f(x)-f(-x)}{2},
$$

即 $f(x)$ 可以表示成一个偶函数与一个奇函数之和．

（Ⅳ）考虑拆项凑微分．令

$$
3\sin x+\cos x=A(\sin x+2\cos x)+B(\cos x-2\sin x),
$$

比较两边系数，可得 $A=1,B=-1$，故

$$
\begin{aligned}
\int\frac{3\sin x+\cos x}{\sin x+2\cos x}\mathrm{d}x&=\int\frac{(\sin x+2\cos x)-(\cos x-2\sin x)}{\sin x+2\cos x}\mathrm{d}x\\
&=\int\mathrm{d}x-\int\frac{\mathrm{d}(\sin x+2\cos x)}{\sin x+2\cos x}\\
&=x-\ln|\sin x+2\cos x|+C.
\end{aligned}
$$

（Ⅴ）用万能代换，令 $\tan\dfrac x2=t$，则

$$
\sin x=\frac{2t}{1+t^2},\quad\cos x=\frac{1-t^2}{1+t^2},\quad\mathrm{d}x=\frac{2\mathrm{d}t}{1+t^2},
$$

故

$$
\begin{aligned}
\int\frac{\mathrm{d}x}{\sin 2x+2\sin x}&=\int\frac{\mathrm{d}x}{2\sin x\cos x+2\sin x}\\
&=\int\frac{\frac{2\mathrm{d}t}{1+t^2}}{2\cdot\frac{2t}{1+t^2}\cdot\frac{1-t^2}{1+t^2}+2\cdot\frac{2t}{1+t^2}}\\
&=\frac14\int\frac{1+t^2}{t}\mathrm{d}t=\frac14\int\frac1t\mathrm{d}t+\frac14\int t\mathrm{d}t\\
&=\frac14\ln|t|+\frac18t^2+C\\
&=\frac14\ln\left|\tan\frac x2\right|+\frac18\tan^2\frac x2+C.
\end{aligned}
$$

（Ⅵ）当 $a=0,b\neq0$ 时，

$$
\int\frac{\mathrm{d}x}{a^2\sin^2x+b^2\cos^2x}=\int\frac{\mathrm{d}x}{b^2\cos^2x}=\frac{1}{b^2}\tan x+C;
$$

当 $a\neq0,b=0$ 时，

$$
\int\frac{\mathrm{d}x}{a^2\sin^2x+b^2\cos^2x}=\int\frac{\mathrm{d}x}{a^2\sin^2x}=-\frac{1}{a^2}\cot x+C;
$$

当 $a\neq0$ 且 $b\neq0$ 时，

$$
\begin{aligned}
\int\frac{\mathrm{d}x}{a^2\sin^2x+b^2\cos^2x}&=\int\frac{\mathrm{d}x}{b^2\cos^2x\left(1+\frac{a^2}{b^2}\tan^2x\right)}\\
&=\int\frac{1}{ab}\cdot\frac{1}{1+\left(\frac ab\tan x\right)^2}\mathrm{d}\left(\frac ab\tan x\right)\\
&=\frac{1}{ab}\arctan\left(\frac ab\tan x\right)+C.
\end{aligned}
$$

+++

#### 基础解答 (4) 求下列积分：

（Ⅰ）$\displaystyle\int\arctan\sqrt{x}\,\mathrm{d}x$；
（Ⅱ）$\displaystyle\int\dfrac{\ln x}{(1-x)^2}\mathrm{d}x$；
（Ⅲ）$\displaystyle\int\dfrac{x^2\mathrm{e}^x}{(x+2)^2}\mathrm{d}x$；
（Ⅳ）$\displaystyle\int\sin(\ln x)\mathrm{d}x$；
（Ⅴ）$\displaystyle\int\dfrac{1}{x^2}\sqrt{\dfrac{1-x}{1+x}}\mathrm{d}x$；
（Ⅵ）$\displaystyle\int\mathrm{e}^{2x}(1+\tan x)^2\mathrm{d}x$．

***

（Ⅰ）用分部积分法．

$$
\begin{aligned}
\int\arctan\sqrt{x}\,\mathrm{d}x&=x\arctan\sqrt{x}-\int x\cdot\frac{1}{1+x}\cdot\frac{1}{2\sqrt{x}}\mathrm{d}x\\
&=x\arctan\sqrt{x}-\frac12\int\frac{x+1-1}{\sqrt{x}(1+x)}\mathrm{d}x\\
&=x\arctan\sqrt{x}-\int\frac{1}{2\sqrt{x}}\mathrm{d}x+\int\frac{\mathrm{d}(\sqrt{x})}{1+(\sqrt{x})^2}\\
&=x\arctan\sqrt{x}-\sqrt{x}+\arctan\sqrt{x}+C.
\end{aligned}
$$

（Ⅱ）

$$
\begin{aligned}
\int\frac{\ln x}{(1-x)^2}\mathrm{d}x&=-\int\ln x\,\mathrm{d}\left(\frac{1}{x-1}\right)=-\frac{\ln x}{x-1}+\int\frac{1}{x-1}\cdot\frac1x\mathrm{d}x\\
&=-\frac{\ln x}{x-1}+\int\left(\frac{1}{x-1}-\frac1x\right)\mathrm{d}x\\
&=-\frac{\ln x}{x-1}+\ln|x-1|-\ln|x|+C.
\end{aligned}
$$

（Ⅲ）

$$
\begin{aligned}
\int\frac{x^2\mathrm{e}^x}{(x+2)^2}\mathrm{d}x&=-\int x^2\mathrm{e}^x\mathrm{d}\left(\frac{1}{x+2}\right)=-x^2\mathrm{e}^x\cdot\frac{1}{x+2}+\int\frac{1}{x+2}\mathrm{d}(x^2\mathrm{e}^x)\\
&=-\frac{x^2\mathrm{e}^x}{x+2}+\int\frac{x^2\mathrm{e}^x+2x\mathrm{e}^x}{x+2}\mathrm{d}x=-\frac{x^2\mathrm{e}^x}{x+2}+\int x\mathrm{e}^x\mathrm{d}x\\
&=-\frac{x^2\mathrm{e}^x}{x+2}+x\mathrm{e}^x-\int\mathrm{e}^x\mathrm{d}x=-\frac{x^2\mathrm{e}^x}{x+2}+x\mathrm{e}^x-\mathrm{e}^x+C.
\end{aligned}
$$

（Ⅳ）令 $\ln x=t$，则 $x=\mathrm{e}^t$，$\mathrm{d}x=\mathrm{e}^t\mathrm{d}t$．

$$
\begin{aligned}
\int\sin(\ln x)\mathrm{d}x&=\int\sin t\cdot\mathrm{e}^t\mathrm{d}t=\int\sin t\,\mathrm{d}(\mathrm{e}^t)\\
&=\mathrm{e}^t\sin t-\int\mathrm{e}^t\cos t\mathrm{d}t=\mathrm{e}^t\sin t-\int\cos t\,\mathrm{d}(\mathrm{e}^t)\\
&=\mathrm{e}^t\sin t-\left(\mathrm{e}^t\cos t+\int\mathrm{e}^t\sin t\mathrm{d}t\right),
\end{aligned}
$$

设 $I=\displaystyle\int\mathrm{e}^t\sin t\mathrm{d}t$，则 $I=\mathrm{e}^t\sin t-\mathrm{e}^t\cos t-I$，即

$$
I=\frac12(\mathrm{e}^t\sin t-\mathrm{e}^t\cos t)+C=\frac12x[\sin(\ln x)-\cos(\ln x)]+C.
$$

（Ⅴ）令 $\sqrt{\dfrac{1-x}{1+x}}=t$，则 $x=\dfrac{1-t^2}{1+t^2}$，$\mathrm{d}x=-\dfrac{4t}{(1+t^2)^2}\mathrm{d}t$，故

$$
\begin{aligned}
I=\int\frac{1}{x^2}\sqrt{\frac{1-x}{1+x}}\mathrm{d}x&=-\int\frac{4t^2}{(1-t^2)^2}\mathrm{d}t\\
&=-2\int\frac{t\,\mathrm{d}(t^2)}{(1-t^2)^2}=-2\int t\,\mathrm{d}\left(\frac{1}{1-t^2}\right)\\
&=-\frac{2t}{1-t^2}+2\int\frac{1}{1-t^2}\mathrm{d}t=-\frac{2t}{1-t^2}+\ln\left|\frac{1+t}{1-t}\right|+C\\
&=-\frac{\sqrt{1-x^2}}{x}+\ln\left|\frac{\sqrt{1+x}+\sqrt{1-x}}{\sqrt{1+x}-\sqrt{1-x}}\right|+C.
\end{aligned}
$$

【注】此题也可利用倒代换，令 $x=\dfrac1t$，则 $\mathrm{d}x=-\dfrac{1}{t^2}\mathrm{d}t$，故

$$
\int\frac{1}{x^2}\sqrt{\frac{1-x}{1+x}}\mathrm{d}x=-\int\sqrt{\frac{t-1}{t+1}}\mathrm{d}t,
$$

再令 $\sqrt{\dfrac{t-1}{t+1}}=u$，去根号继续求解即可．

（Ⅵ）

$$
\begin{aligned}
I=\int\mathrm{e}^{2x}(1+\tan x)^2\mathrm{d}x&=\int\mathrm{e}^{2x}(1+2\tan x+\tan^2x)\mathrm{d}x\\
&=\int\mathrm{e}^{2x}\sec^2x\mathrm{d}x+2\int\mathrm{e}^{2x}\tan x\mathrm{d}x=\int\mathrm{e}^{2x}\mathrm{d}(\tan x)+2\int\mathrm{e}^{2x}\tan x\mathrm{d}x\\
&=\mathrm{e}^{2x}\tan x-2\int\mathrm{e}^{2x}\tan x\mathrm{d}x+2\int\mathrm{e}^{2x}\tan x\mathrm{d}x=\mathrm{e}^{2x}\tan x+C.
\end{aligned}
$$

【注】此题通过分部积分法消去 $2\displaystyle\int\mathrm{e}^{2x}\tan x\mathrm{d}x$，这类问题一般也可凑微分．

$$
\begin{aligned}
\int\mathrm{e}^{2x}\sec^2x\mathrm{d}x+2\int\mathrm{e}^{2x}\tan x\mathrm{d}x&=\int(\mathrm{e}^{2x}\sec^2x+2\mathrm{e}^{2x}\tan x)\mathrm{d}x\\
&=\int\mathrm{d}(\mathrm{e}^{2x}\tan x)=\mathrm{e}^{2x}\tan x+C.
\end{aligned}
$$

+++

#### 基础解答 (5) 求下列积分：

（Ⅰ）$\displaystyle\int_{-\frac{\pi}{4}}^{\frac{\pi}{4}}\left(x^2\ln\dfrac{1+x}{1-x}-\cos x\right)\mathrm{d}x$；
（Ⅱ）$\displaystyle\int_{-1}^{1}(2+\sin x)\sqrt{1-x^2}\,\mathrm{d}x$；
（Ⅲ）$\displaystyle\int_{-2}^{2}(x+|x|)\mathrm{e}^{-|x|}\mathrm{d}x$；
（Ⅳ）$\displaystyle\int_{-1}^{1}\dfrac{2x^2+x(\mathrm{e}^x+\mathrm{e}^{-x})}{1+\sqrt{1-x^2}}\mathrm{d}x$．

***

（Ⅰ）在对称区间上积分，考查被积函数的奇偶性．

$\ln\dfrac{1+x}{1-x}=\ln(1+x)-\ln(1-x)$ 是奇函数，$\cos x$ 是偶函数，故

$$
I=\int_{-\frac{\pi}{4}}^{\frac{\pi}{4}}\left(x^2\ln\frac{1+x}{1-x}-\cos x\right)\mathrm{d}x=0-2\int_0^{\frac{\pi}{4}}\cos x\mathrm{d}x=-\sqrt2.
$$

（Ⅱ）

$$
\int_{-1}^{1}(2+\sin x)\sqrt{1-x^2}\,\mathrm{d}x=4\int_0^1\sqrt{1-x^2}\,\mathrm{d}x+0=4\times\frac14\pi=\pi.
$$

（Ⅲ）

$$
\begin{aligned}
\int_{-2}^{2}(x+|x|)\mathrm{e}^{-|x|}\mathrm{d}x&=0+2\int_0^2|x|\mathrm{e}^{-|x|}\mathrm{d}x=2\int_0^2x\mathrm{e}^{-x}\mathrm{d}x\\
&=-2x\mathrm{e}^{-x}\bigg|_0^2+2\int_0^2\mathrm{e}^{-x}\mathrm{d}x=2-6\mathrm{e}^{-2}.
\end{aligned}
$$

（Ⅳ）由题可知，$\dfrac{2x^2}{1+\sqrt{1-x^2}}$ 是偶函数，$\dfrac{x(\mathrm{e}^x+\mathrm{e}^{-x})}{1+\sqrt{1-x^2}}$ 是奇函数，故

$$
\begin{aligned}
\int_{-1}^{1}\frac{2x^2+x(\mathrm{e}^x+\mathrm{e}^{-x})}{1+\sqrt{1-x^2}}\mathrm{d}x&=4\int_0^1\frac{x^2}{1+\sqrt{1-x^2}}\mathrm{d}x+0\\
&=4\int_0^1\mathrm{d}x-4\int_0^1\sqrt{1-x^2}\,\mathrm{d}x=4-\pi.
\end{aligned}
$$

+++

#### 基础解答 (6) 求下列积分：

（Ⅰ）$\displaystyle\int_0^2(x-1)^2\sqrt{2x-x^2}\,\mathrm{d}x$；
（Ⅱ）$\displaystyle\int_0^{\pi}(\mathrm{e}^{-\cos x}-\mathrm{e}^{\cos x})\mathrm{d}x$．

***

（Ⅰ）

$$
\begin{aligned}
\int_0^2(x-1)^2\sqrt{2x-x^2}\,\mathrm{d}x&=\int_0^2(x-1)^2\sqrt{1-(x-1)^2}\,\mathrm{d}x\\
&\xlongequal{x-1=t}\int_{-1}^{1}t^2\sqrt{1-t^2}\,\mathrm{d}t=2\int_0^1t^2\sqrt{1-t^2}\,\mathrm{d}t\\
&\xlongequal{t=\sin u}2\int_0^{\frac{\pi}{2}}\cos^2u\sin^2u\,\mathrm{d}u=2\int_0^{\frac{\pi}{2}}(1-\sin^2u)\sin^2u\,\mathrm{d}u\\
&=2\times\frac12\times\frac{\pi}{2}-2\int_0^{\frac{\pi}{2}}\sin^4u\,\mathrm{d}u=\frac{\pi}{2}-2\times\frac34\times\frac12\times\frac{\pi}{2}\\
&=\frac{\pi}{8}.
\end{aligned}
$$

（Ⅱ）

$$
\int_0^{\pi}(\mathrm{e}^{-\cos x}-\mathrm{e}^{\cos x})\mathrm{d}x\xlongequal{x=\frac{\pi}{2}+t}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}(\mathrm{e}^{\sin t}-\mathrm{e}^{-\sin t})\mathrm{d}t=0.
$$

【注】$\mathrm{e}^{\sin t}-\mathrm{e}^{-\sin t}$ 是奇函数．

+++

#### 基础解答 (7) 求下列积分：

（Ⅰ）$\displaystyle\int_{-3}^{2}\min\{2,x^2\}\mathrm{d}x$；
（Ⅱ）$\displaystyle\int_{-1}^{x}(1-|t|)\mathrm{d}t\ (x\geqslant-1)$；
（Ⅲ）$\displaystyle\int_{-1}^{1}|x-y|\mathrm{e}^x\mathrm{d}x\ (|y|\leqslant1)$；
（Ⅳ）$\displaystyle\int_0^{\pi}\sqrt{1-\sin x}\,\mathrm{d}x$．

***

（Ⅰ）

$$
\min\{2,x^2\}=\begin{cases}2,&-3\leqslant x\leqslant-\sqrt2,\\ x^2,&-\sqrt2<x<\sqrt2,\\ 2,&\sqrt2\leqslant x\leqslant2,\end{cases}
$$

故

$$
\begin{aligned}
\int_{-3}^{2}\min\{2,x^2\}\mathrm{d}x&=\int_{-3}^{-\sqrt2}\min\{2,x^2\}\mathrm{d}x+\int_{-\sqrt2}^{\sqrt2}\min\{2,x^2\}\mathrm{d}x+\int_{\sqrt2}^{2}\min\{2,x^2\}\mathrm{d}x\\
&=\int_{-3}^{-\sqrt2}2\mathrm{d}x+\int_{-\sqrt2}^{\sqrt2}x^2\mathrm{d}x+\int_{\sqrt2}^{2}2\mathrm{d}x=10-\frac83\sqrt2.
\end{aligned}
$$

（Ⅱ）当 $-1\leqslant x<0$ 时，$\displaystyle\int_{-1}^{x}(1-|t|)\mathrm{d}t=\int_{-1}^{x}(1+t)\mathrm{d}t=\frac{(1+t)^2}{2}\bigg|_{-1}^{x}=\frac{(1+x)^2}{2}$；

当 $x\geqslant0$ 时，$\displaystyle\int_{-1}^{x}(1-|t|)\mathrm{d}t=\int_{-1}^{0}(1+t)\mathrm{d}t+\int_0^x(1-t)\mathrm{d}t=1-\frac12(1-x)^2$．

【注】注意当 $x\geqslant0$ 时，$\displaystyle\int_{-1}^{x}(1-|t|)\mathrm{d}t\neq\int_{-1}^{x}(1-t)\mathrm{d}t$．

（Ⅲ）分段积分，去绝对值符号．

$$
\begin{aligned}
\int_{-1}^{1}|x-y|\mathrm{e}^x\mathrm{d}x&=\int_{-1}^{y}(y-x)\mathrm{e}^x\mathrm{d}x+\int_y^1(x-y)\mathrm{e}^x\mathrm{d}x\\
&=(y-x)\mathrm{e}^x\bigg|_{-1}^{y}+\int_{-1}^{y}\mathrm{e}^x\mathrm{d}x+(x-y)\mathrm{e}^x\bigg|_y^1-\int_y^1\mathrm{e}^x\mathrm{d}x\\
&=2\mathrm{e}^y-(y+2)\mathrm{e}^{-1}-y\mathrm{e}.
\end{aligned}
$$

（Ⅳ）

$$
\begin{aligned}
\int_0^{\pi}\sqrt{1-\sin x}\,\mathrm{d}x&=\int_0^{\pi}\left|\sin\frac x2-\cos\frac x2\right|\mathrm{d}x\\
&=\int_0^{\frac{\pi}{2}}\left(\cos\frac x2-\sin\frac x2\right)\mathrm{d}x+\int_{\frac{\pi}{2}}^{\pi}\left(\sin\frac x2-\cos\frac x2\right)\mathrm{d}x=4(\sqrt2-1).
\end{aligned}
$$

【注】因为 $\sqrt{1-\sin x}$ 在 $[0,\pi]$ 上关于直线 $x=\dfrac{\pi}{2}$ 对称，所以

$$
\begin{aligned}
I=\int_0^{\pi}\sqrt{1-\sin x}\,\mathrm{d}x&=2\int_0^{\frac{\pi}{2}}\sqrt{1-\sin x}\,\mathrm{d}x=2\int_0^{\frac{\pi}{2}}\left(\cos\frac x2-\sin\frac x2\right)\mathrm{d}x\\
&=2\left(2\sin\frac x2\bigg|_0^{\frac{\pi}{2}}+2\cos\frac x2\bigg|_0^{\frac{\pi}{2}}\right)=4(\sqrt2-1).
\end{aligned}
$$

+++

#### 基础解答 (8) 求下列积分：

（Ⅰ）$\displaystyle\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}(x+\sin^2x)\cos^2x\,\mathrm{d}x$；
（Ⅱ）$\displaystyle\int_0^1x(1-x^4)^{\frac32}\mathrm{d}x$；
（Ⅲ）$\displaystyle\int_0^{\pi}t\sin t\,\mathrm{d}t$；
（Ⅳ）$\displaystyle\int_0^1\left[\sqrt{2x-x^2}+\sqrt{(1-x^2)^3}\right]\mathrm{d}x$．

***

（Ⅰ）由题可知，$x\cos^2x$ 是奇函数，$\sin^2x\cos^2x$ 为偶函数，故

$$
\begin{aligned}
I=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}(x+\sin^2x)\cos^2x\,\mathrm{d}x&=0+2\int_0^{\frac{\pi}{2}}\sin^2x\cos^2x\,\mathrm{d}x\\
&=2\int_0^{\frac{\pi}{2}}\sin^2x(1-\sin^2x)\mathrm{d}x=2\int_0^{\frac{\pi}{2}}\sin^2x\,\mathrm{d}x-2\int_0^{\frac{\pi}{2}}\sin^4x\,\mathrm{d}x\\
&=2\times\frac12\times\frac{\pi}{2}-2\times\frac34\times\frac12\times\frac{\pi}{2}=\frac{\pi}{8}.
\end{aligned}
$$

（Ⅱ）令 $x^2=\sin t$，则 $2x\mathrm{d}x=\cos t\mathrm{d}t$，故

$$
\int_0^1x(1-x^4)^{\frac32}\mathrm{d}x=\frac12\int_0^{\frac{\pi}{2}}\cos t\cdot\cos^3t\,\mathrm{d}t=\frac12\times\frac34\times\frac12\times\frac{\pi}{2}=\frac{3\pi}{32}.
$$

（Ⅲ）

$$
\int_0^{\pi}t\sin t\,\mathrm{d}t=-\int_0^{\pi}t\,\mathrm{d}(\cos t)=(-t\cos t)\bigg|_0^{\pi}+\int_0^{\pi}\cos t\,\mathrm{d}t=\pi.
$$

（Ⅳ）

$$
\int_0^1\sqrt{2x-x^2}\,\mathrm{d}x=\int_0^1\sqrt{1-(x-1)^2}\,\mathrm{d}x\xlongequal{x-1=t}\int_{-1}^{0}\sqrt{1-t^2}\,\mathrm{d}t=\frac{\pi}{4},
$$

$$
\int_0^1\sqrt{(1-x^2)^3}\,\mathrm{d}x\xlongequal{x=\sin t}\int_0^{\frac{\pi}{2}}\cos^4t\,\mathrm{d}t=\frac34\times\frac12\times\frac{\pi}{2}=\frac{3\pi}{16},
$$

故原积分 $=\dfrac{\pi}{4}+\dfrac{3\pi}{16}=\dfrac{7\pi}{16}.$

【注】利用结论 $\displaystyle\int_0^{\pi}xf(\sin x)\mathrm{d}x=\frac{\pi}{2}\int_0^{\pi}f(\sin x)\mathrm{d}x$，有

$$
\begin{aligned}
\int_0^{\pi}x\sin^nx\,\mathrm{d}x&=\frac{\pi}{2}\int_0^{\pi}\sin^nx\,\mathrm{d}x=\pi\int_0^{\frac{\pi}{2}}\sin^nx\,\mathrm{d}x\\
&=\begin{cases}\dfrac{(n-1)!!}{n!!}\cdot\dfrac{\pi^2}{2},&n\text{ 为正偶数},\\[2mm] \dfrac{(n-1)!!}{n!!}\cdot\pi,&n\text{ 为大于 }1\text{ 的正奇数},\end{cases}
\end{aligned}
$$

故（Ⅲ）可利用结论求解，即 $\displaystyle\int_0^{\pi}t\sin t\,\mathrm{d}t=\frac{\pi}{2}\int_0^{\pi}\sin t\,\mathrm{d}t=\pi.$

+++

#### 基础解答 (9) 求下列积分：

（Ⅰ）$\displaystyle\int_1^{+\infty}\dfrac{\mathrm{d}x}{\mathrm{e}^{x+1}+\mathrm{e}^{3-x}}$；
（Ⅱ）$\displaystyle\int_{\frac12}^{\frac32}\dfrac{\mathrm{d}x}{\sqrt{|x-x^2|}}$．

***

（Ⅰ）令 $x-1=t$，则

$$
\begin{aligned}
\int_1^{+\infty}\frac{\mathrm{d}x}{\mathrm{e}^{x+1}+\mathrm{e}^{3-x}}&=\int_1^{+\infty}\frac{\mathrm{d}x}{\mathrm{e}^2(\mathrm{e}^{x-1}+\mathrm{e}^{1-x})}=\frac{1}{\mathrm{e}^2}\int_0^{+\infty}\frac{\mathrm{d}t}{\mathrm{e}^t+\mathrm{e}^{-t}}\\
&=\frac{1}{\mathrm{e}^2}\int_0^{+\infty}\frac{\mathrm{e}^t}{1+\mathrm{e}^{2t}}\mathrm{d}t=\frac{1}{\mathrm{e}^2}\arctan\mathrm{e}^t\bigg|_0^{+\infty}\\
&=\frac{1}{\mathrm{e}^2}\left(\frac{\pi}{2}-\frac{\pi}{4}\right)=\frac{\pi}{4\mathrm{e}^2}.
\end{aligned}
$$

（Ⅱ）积分区间内 $x=1$ 是瑕点，在区间 $\left[\dfrac12,1\right)$ 和 $\left(1,\dfrac32\right]$ 上分别计算积分．

$$
\begin{aligned}
\int_{\frac12}^{\frac32}\frac{\mathrm{d}x}{\sqrt{|x-x^2|}}&=\int_{\frac12}^{1}\frac{\mathrm{d}x}{\sqrt{x-x^2}}+\int_1^{\frac32}\frac{\mathrm{d}x}{\sqrt{x^2-x}}\\
&=\int_{\frac12}^{1}\frac{\mathrm{d}x}{\sqrt{\frac14-\left(x-\frac12\right)^2}}+\int_1^{\frac32}\frac{\mathrm{d}x}{\sqrt{\left(x-\frac12\right)^2-\frac14}}\\
&=\arcsin(2x-1)\bigg|_{\frac12}^{1}+\ln\left[\left(x-\frac12\right)+\sqrt{\left(x-\frac12\right)^2-\frac14}\right]\bigg|_1^{\frac32}\\
&=\frac{\pi}{2}+\ln(2+\sqrt3).
\end{aligned}
$$

【注】积分公式：

$$
\int\frac{\mathrm{d}x}{\sqrt{a^2-x^2}}=\arcsin\frac xa+C,
$$

$$
\int\frac{\mathrm{d}x}{\sqrt{x^2-a^2}}=\ln|x+\sqrt{x^2-a^2}|+C.
$$

+++

#### 基础解答 (10) 设 $f(x)$ 在 $[0,a]$ 上具有二阶导数 $(a>0)$，且 $f(x)>0$，$f''(x)>0$，证明：$\displaystyle\int_0^af(x)\mathrm{d}x>af\left(\dfrac a2\right)$．

***

证　利用泰勒公式，将 $f(x)$ 在 $x=\dfrac a2$ 处展开为

$$
\begin{aligned}
f(x)&=f\left(\frac a2\right)+f'\left(\frac a2\right)\left(x-\frac a2\right)+\frac{f''(\xi)}{2!}\left(x-\frac a2\right)^2\\
&\geqslant f\left(\frac a2\right)+f'\left(\frac a2\right)\left(x-\frac a2\right)\quad\left(\xi\ \text{介于}\ \frac a2\ \text{与}\ x\ \text{之间}\right),
\end{aligned}
$$

积分，得

$$
\begin{aligned}
\int_0^af(x)\mathrm{d}x&>\int_0^a\left[f\left(\frac a2\right)+f'\left(\frac a2\right)\left(x-\frac a2\right)\right]\mathrm{d}x\\
&=\left[f\left(\frac a2\right)\cdot x+\frac12f'\left(\frac a2\right)\left(x-\frac a2\right)^2\right]\bigg|_0^a=af\left(\frac a2\right).
\end{aligned}
$$

+++

#### 基础解答 (11) 设 $f(x)$ 在 $[a,b]$ 上连续且单调增加，证明：$\displaystyle\int_a^bxf(x)\mathrm{d}x\geqslant\dfrac{a+b}{2}\int_a^bf(x)\mathrm{d}x$．

***

证　利用单调性证明．令

$$
F(x)=\int_a^xtf(t)\mathrm{d}t-\frac{a+x}{2}\int_a^xf(t)\mathrm{d}t,\quad a\leqslant x\leqslant b,
$$

则

$$
\begin{aligned}
F'(x)&=xf(x)-\frac12\int_a^xf(t)\mathrm{d}t-\frac{a+x}{2}f(x)\\
&=\frac{x-a}{2}f(x)-\frac12\int_a^xf(t)\mathrm{d}t\\
&=\frac{x-a}{2}f(x)-\frac12f(\xi)(x-a)\quad(\text{这里利用积分中值定理})\\
&=\frac{x-a}{2}[f(x)-f(\xi)]\geqslant0\quad(\text{因}\ f(x)\ \text{单调增加}),
\end{aligned}
$$

其中 $a\leqslant\xi\leqslant x$，所以 $F(x)$ 单调增加，故 $F(b)\geqslant F(a)=0$，即

$$
\int_a^bxf(x)\mathrm{d}x\geqslant\frac{a+b}{2}\int_a^bf(x)\mathrm{d}x.
$$

+++

#### 基础解答 (12) 设 $f(x)$ 在 $[a,b]$ 上连续，且 $y=f(x)$ 的图形关于直线 $x=\dfrac{a+b}{2}$ 对称，证明：$\displaystyle\int_a^bxf(x)\mathrm{d}x=\dfrac{a+b}{2}\int_a^bf(x)\mathrm{d}x$．

***

证　利用积分换元法．

$$
\begin{aligned}
\int_a^bxf(x)\mathrm{d}x&\xlongequal{x=a+b-t}\int_b^a(a+b-t)f(a+b-t)(-\mathrm{d}t)\\
&=\int_a^b(a+b-t)f(a+b-t)\mathrm{d}t.
\end{aligned}
$$

由题知 $y=f(x)$ 关于 $x=\dfrac{a+b}{2}$ 对称，则有

$$
f(x)=f\left(2\cdot\frac{a+b}{2}-x\right)=f(a+b-x),
$$

故

$$
\begin{aligned}
\int_a^bxf(x)\mathrm{d}x&=\int_a^b(a+b-t)f(a+b-t)\mathrm{d}t\\
&=(a+b)\int_a^bf(t)\mathrm{d}t-\int_a^btf(t)\mathrm{d}t\\
&=(a+b)\int_a^bf(x)\mathrm{d}x-\int_a^bxf(x)\mathrm{d}x,
\end{aligned}
$$

移项，得 $\displaystyle\int_a^bxf(x)\mathrm{d}x=\frac{a+b}{2}\int_a^bf(x)\mathrm{d}x.$

【注】结论：若 $y=f(x)$ 关于直线 $x=a\ (a\neq0)$ 对称，则 $f(x)=f(2a-x)$；若 $y=f(x)$ 关于点 $(a,0)$ 对称 $(a\neq0)$，则 $f(x)=-f(2a-x)$．

+++

#### 基础解答 (13) 设 $f(x)$ 在 $[0,+\infty)$ 上连续，且单调增加，证明：当 $0<a<b$ 时，有 $\displaystyle\int_a^bxf(x)\mathrm{d}x\geqslant\dfrac12\left[b\int_0^bf(x)\mathrm{d}x-a\int_0^af(x)\mathrm{d}x\right]$．

***

证　利用单调性证明．令

$$
F(x)=\int_a^xtf(t)\mathrm{d}t-\frac12\left[x\int_0^xf(t)\mathrm{d}t-a\int_0^af(t)\mathrm{d}t\right],
$$

则

$$
\begin{aligned}
F'(x)&=xf(x)-\frac12xf(x)-\frac12\int_0^xf(t)\mathrm{d}t=\frac12xf(x)-\frac12\int_0^xf(t)\mathrm{d}t\\
&\geqslant\frac12xf(x)-\frac12\int_0^xf(x)\mathrm{d}t=\frac12xf(x)-\frac12xf(x)=0,
\end{aligned}
$$

故 $F(x)$ 单调增加，所以 $F(b)\geqslant F(a)=0$．所证不等式成立．

【注】考虑到 $b\displaystyle\int_0^bf(x)\mathrm{d}x-a\int_0^af(x)\mathrm{d}x$，也可令辅助函数为 $F(x)=x\displaystyle\int_0^xf(t)\mathrm{d}t\ (x\geqslant0)$，则

$$
\begin{aligned}
b\int_0^bf(x)\mathrm{d}x-a\int_0^af(x)\mathrm{d}x&=F(b)-F(a)=\int_a^bF'(x)\mathrm{d}x\\
&=\int_a^b\left[\int_0^xf(t)\mathrm{d}t+xf(x)\right]\mathrm{d}x\leqslant\int_a^b\left[\int_0^xf(x)\mathrm{d}t+xf(x)\right]\mathrm{d}x\\
&=\int_a^b[f(x)x+xf(x)]\mathrm{d}x=2\int_a^bxf(x)\mathrm{d}x,
\end{aligned}
$$

所以 $\displaystyle\int_a^bxf(x)\mathrm{d}x\geqslant\frac12\left[b\int_0^bf(x)\mathrm{d}x-a\int_0^af(x)\mathrm{d}x\right].$

+++

#### 基础解答 (14) 求 $f(x)=\displaystyle\int_0^x\dfrac{2t-1}{t^2-t+1}\mathrm{d}t$ 在 $[-1,1]$ 上的最大值与最小值．

***

解　对 $f(x)$ 求导有 $f'(x)=\dfrac{2x-1}{x^2-x+1}$，令 $f'(x)=0$，解得 $x=\dfrac12$．

当 $-1<x<\dfrac12$ 时，$f'(x)<0$；当 $\dfrac12<x<1$ 时，$f'(x)>0$．又

$$
f(1)=\int_0^1\frac{2t-1}{t^2-t+1}\mathrm{d}t=\ln(t^2-t+1)\bigg|_0^1=0,
$$

$$
f(-1)=\int_0^{-1}\frac{2t-1}{t^2-t+1}\mathrm{d}t=\ln(t^2-t+1)\bigg|_0^{-1}=\ln3,
$$

$$
f\left(\frac12\right)=\int_0^{\frac12}\frac{2t-1}{t^2-t+1}\mathrm{d}t=\ln(t^2-t+1)\bigg|_0^{\frac12}=\ln\frac34,
$$

故最小值为 $\ln\dfrac34$，最大值为 $\ln3$．

+++

#### 基础解答 (15) 设点 $A(a,0)\ (a>0)$，梯形 $OABC$ 的面积为 $S$，曲边梯形 $OABC$ 的面积为 $S_1$，其曲边由 $y=\dfrac12+x^2$ 确定，证明：$\dfrac{S}{S_1}<\dfrac32$．

***

解　依题设，如图 3-5 所示，由 $y=\dfrac12+x^2$，有 $y(0)=\dfrac12$，$y(a)=a^2+\dfrac12$，故梯形 $OABC$ 的面积为

$$
S=\frac12(|OC|+|AB|)\cdot|OA|=\frac12\left(\frac12+a^2+\frac12\right)\cdot a=\frac12a(a^2+1).
$$

曲边梯形 $OABC$ 的面积为

$$
S_1=\int_0^a\left(x^2+\frac12\right)\mathrm{d}x=\left(\frac13x^3+\frac12x\right)\bigg|_0^a=\frac13a\left(a^2+\frac32\right),
$$

故

$$
\frac{S}{S_1}=\frac{\frac12a(a^2+1)}{\frac13a\left(a^2+\frac32\right)}<\frac32.
$$

+++

#### 基础解答 (16) 设曲线 $y=\sin x\left(0\leqslant x\leqslant\dfrac{\pi}{2}\right)$，直线 $y=k\ (0\leqslant k\leqslant1)$ 与 $x=0$ 所围面积为 $S_1$，$y=\sin x\left(0\leqslant x\leqslant\dfrac{\pi}{2}\right)$，$y=k$ 与 $x=\dfrac{\pi}{2}$ 所围面积为 $S_2$，求 $S=S_1+S_2$ 的最小值．

***

解　由已知，如图 3-6 所示．

设 $\sin x=k\left(0\leqslant x\leqslant\dfrac{\pi}{2}\right)$，依题意知，两个函数图形的交点是唯一的，则

$$
S_1=\int_0^x(k-\sin t)\mathrm{d}t=kx+\cos x-1,
$$

$$
S_2=\int_x^{\frac{\pi}{2}}(\sin t-k)\mathrm{d}t=\cos x+kx-\frac12\pi k.
$$

将 $k=\sin x$ 代入上两式，得

$$
S_1=x\sin x+\cos x-1,\quad S_2=\cos x+x\sin x-\frac12\pi\sin x,
$$

故

$$
S=S_1+S_2=2(x\sin x+\cos x)-\left(1+\frac{\pi}{2}\sin x\right),\quad 0<x<\frac{\pi}{2},
$$

则 $S'=2x\cos x-\dfrac{\pi}{2}\cos x=0$，得唯一驻点 $x=\dfrac{\pi}{4}$．又

$$
S(0)=1,\quad S\left(\frac{\pi}{4}\right)=\sqrt2-1,\quad S\left(\frac{\pi}{2}\right)=\frac{\pi}{2}-1,
$$

所以 $S$ 的最小值为 $S\left(\dfrac{\pi}{4}\right)=\sqrt2-1$．

+++

#### 基础解答 (17) 设曲线 $y=\sin x\left(0\leqslant x\leqslant\dfrac{\pi}{2}\right)$，$y=1$ 及 $x=0$ 所围平面图形为 $D_1$，$y=\sin x\ (0\leqslant x\leqslant\pi)$ 及 $y=0$ 所围平面图形为 $D_2$．

（Ⅰ）求 $D_1$ 绕直线 $x=\dfrac{\pi}{2}$ 旋转一周所得体积 $V_1$；
（Ⅱ）求 $D_2$ 绕 $y$ 轴旋转一周所得体积 $V_2$．

***

（Ⅰ）如图 3-7 所示，用微元法．

任取 $[y,y+\mathrm{d}y]\subset[0,1]$，则微元

$$
\begin{aligned}
\mathrm{d}V_1&=\left[\pi\left(\frac{\pi}{2}\right)^2-\pi\left(\frac{\pi}{2}-x\right)^2\right]\mathrm{d}y\\
&=[\pi^2\arcsin y-\pi(\arcsin y)^2]\mathrm{d}y,
\end{aligned}
$$

故

$$
\begin{aligned}
V_1&=\int_0^1\mathrm{d}V_1=\pi^2\int_0^1\arcsin y\,\mathrm{d}y-\pi\int_0^1(\arcsin y)^2\mathrm{d}y\\
&=\pi^2\left(y\arcsin y+\sqrt{1-y^2}\right)\bigg|_0^1-\pi\left[y(\arcsin y)^2+2\sqrt{1-y^2}\arcsin y-2y\right]\bigg|_0^1\\
&=\pi^2\left(\frac{\pi}{2}-1\right)-\pi\left(\frac{\pi^2}{4}-2\right)=\frac{\pi^3}{4}-\pi^2+2\pi.
\end{aligned}
$$

（Ⅱ）任取 $[x,x+\mathrm{d}x]\subset[0,\pi]$，则微元 $\mathrm{d}V_2=2\pi x\cdot\sin x\mathrm{d}x$，故

$$
V_2=\int_0^{\pi}2\pi x\sin x\,\mathrm{d}x=2\pi^2.
$$

+++

#### 基础解答 (18) 设星形线 $\begin{cases}x=a\cos^3t,\\ y=a\sin^3t\end{cases}(0\leqslant t\leqslant2\pi,\ a>0)$．

（Ⅰ）求所围面积 $A$；
（Ⅱ）求弧长 $L$；
（Ⅲ）求绕 $x$ 轴旋转一周所得体积 $V$ 和表面积 $S$．

***

（Ⅰ）星形线如图 3-8 所示．

$$
\begin{aligned}
A&=4\int_0^ay\mathrm{d}x=4\int_{\frac{\pi}{2}}^{0}a\sin^3t\cdot(-3a\cos^2t\cdot\sin t)\mathrm{d}t\\
&=12\int_0^{\frac{\pi}{2}}a^2(\sin^4t-\sin^6t)\mathrm{d}t=\frac{3\pi a^2}{8}.
\end{aligned}
$$

（Ⅱ）$L=4\displaystyle\int_0^{\frac{\pi}{2}}\sqrt{x'^2(t)+y'^2(t)}\,\mathrm{d}t=4\int_0^{\frac{\pi}{2}}3a\sin t\cos t\,\mathrm{d}t=6a.$

（Ⅲ）$V=2\displaystyle\int_0^a\pi y^2\mathrm{d}x=6\pi a^3\int_0^{\frac{\pi}{2}}\sin^7t(1-\sin^2t)\mathrm{d}t=\frac{32}{105}\pi a^3,$

$$
S=2\int_0^{\frac{\pi}{2}}2\pi y\sqrt{x'^2(t)+y'^2(t)}\,\mathrm{d}t=12\pi a^2\int_0^{\frac{\pi}{2}}\sin^4t\cdot\cos t\,\mathrm{d}t=\frac{12}{5}\pi a^2.
$$

【注】参数方程所围区域图形，求其旋转体面积或体积，关键是在直角坐标系中写出面积或体积表达式，再将参数方程代入，相当于定积分的换元．

如参数方程 $x=x(t)$，$y=y(t)$，设 $x=x(t)$ 的反函数为 $t=t(x)$，则面积为

$$
A=\int_a^by(t(x))\mathrm{d}x\xlongequal{x=x(t)}\int_{\alpha}^{\beta}y(t)\mathrm{d}[x(t)],
$$

这里 $\alpha,\beta$ 是 $t$ 的积分限．

+++

#### 基础解答 (19) 设立体图形的底是介于 $y=x^2-1$ 和 $y=0$ 之间的平面区域，而它的垂直于 $x$ 轴的任一截面是等边三角形，求立体体积 $V$．

***

解　依题意，立体如图 3-9 所示，先求垂直于 $x$ 轴截面的面积

$$
A(x)=\frac12(x^2-1)^2\sin\frac{\pi}{3}=\frac{\sqrt3}{4}(x^2-1)^2,
$$

故所求体积为

$$
\begin{aligned}
V&=\int_{-1}^{1}A(x)\mathrm{d}x=\frac{\sqrt3}{4}\int_{-1}^{1}(x^2-1)^2\mathrm{d}x\\
&=\frac{\sqrt3}{2}\int_0^1(x^2-1)^2\mathrm{d}x=\frac{\sqrt3}{2}\left(\frac{x^5}{5}-\frac23x^3+x\right)\bigg|_0^1=\frac{4}{15}\sqrt3.
\end{aligned}
$$

+++

#### 综合选择 (1) 设 $F(x)=\int_x^{x+2\pi}\mathrm{e}^{\sin t}\cdot\sin t\,\mathrm{d}t$，则正确的是（　）。

;;;
A. $F(x)$ 为正的常数
B. $F(x)$ 为负的常数
C. $F(x)$ 不是常数
D. $F(x)$ 恒为零
;;;A

***

**A**。

由于 $\mathrm{e}^{\sin t}\sin t$ 是以 $2\pi$ 为周期的周期函数，所以

$$
F(x)=\int_x^{x+2\pi}\mathrm{e}^{\sin t}\sin t\,\mathrm{d}t=\int_0^{2\pi}\mathrm{e}^{\sin t}\sin t\,\mathrm{d}t=-\int_0^{2\pi}\mathrm{e}^{\sin t}\,\mathrm{d}(\cos t)
$$

$$
=-\mathrm{e}^{\sin t}\cos t\bigg|_0^{2\pi}+\int_0^{2\pi}\cos t\cdot\mathrm{e}^{\sin t}\cdot\cos t\,\mathrm{d}t=\int_0^{2\pi}\cos^2t\,\mathrm{e}^{\sin t}\,\mathrm{d}t,
$$

又因为 $\cos^2t\geqslant0$，$\mathrm{e}^{\sin t}>0$，所以 $\cos^2t\,\mathrm{e}^{\sin t}\geqslant0$，故 $F(x)>0$，**A** 正确。

【注】设 $f(x+T)=f(x)$，且 $f(x)$ 连续，则对任意 $a\in\mathbf{R}$，有

$$
\int_a^{a+T}f(x)\,\mathrm{d}x=\int_0^{T}f(x)\,\mathrm{d}x.
$$

+++

#### 综合选择 (2) 设 $\delta>0$，在 $(-\delta,\delta)$ 内有 $|f(x)|\leqslant x^2$，$f''(x)>0$，$I=\int_{-\delta}^{\delta}f(x)\,\mathrm{d}x$，则（　）。

;;;
A. $I=0$
B. $I>0$
C. $I<0$
D. 不能确定
;;;B

***

**B**。

**解** 确定 $f(x)$ 在 $(-\delta,\delta)$ 内的符号。

由 $|f(x)|\leqslant x^2$，知 $f(0)=0$，且

$$
0\leqslant|f'(0)|=\lim\limits_{x\to0}\left|\dfrac{f(x)}{x}\right|\leqslant\lim\limits_{x\to0}\dfrac{x^2}{|x|}=0,
$$

故 $f'(0)=0$。

由 $f''(x)>0$，知 $f'(x)$ 单调增加，故在区间 $(-\delta,0)$ 和 $(0,\delta)$ 内分别有 $f'(x)<0$ 和 $f'(x)>0$。

因而 $f(x)$ 在 $(-\delta,0)$ 内单调减少，在 $(0,\delta)$ 内单调增加，又 $f(0)=0$，知 $f(x)$ 在 $(-\delta,\delta)$ 内非负，且仅在 $x=0$ 处 $f(x)=0$，所以 $I=\int_{-\delta}^{\delta}f(x)\,\mathrm{d}x>0$，故 **B** 正确。

+++

#### 综合选择 (3) 设 $I_1=\int_0^{\frac{\pi}{2}}\sin(\sin x)\,\mathrm{d}x$，$I_2=\int_0^{\frac{\pi}{2}}\cos(\sin x)\,\mathrm{d}x$，则（　）。

;;;
A. $I_1<1<I_2$
B. $I_2<1<I_1$
C. $1<I_1<I_2$
D. $I_1<I_2<1$
;;;A

***

**A**。

**解** 因为 $x\in\left[0,\dfrac{\pi}{2}\right]$，所以在该区间上 $\sin x$ 单调增加，$\cos x$ 单调减少，而 $\sin x\leqslant x$，故当 $x\in\left(0,\dfrac{\pi}{2}\right)$ 时，有 $\sin(\sin x)<\sin x$，$\cos(\sin x)>\cos x$，故

$$
I_1=\int_0^{\frac{\pi}{2}}\sin(\sin x)\,\mathrm{d}x<\int_0^{\frac{\pi}{2}}\sin x\,\mathrm{d}x=-\cos x\bigg|_0^{\frac{\pi}{2}}=1,
$$

$$
I_2=\int_0^{\frac{\pi}{2}}\cos(\sin x)\,\mathrm{d}x>\int_0^{\frac{\pi}{2}}\cos x\,\mathrm{d}x=\sin x\bigg|_0^{\frac{\pi}{2}}=1.
$$

综上可知，$I_1<1<I_2$，**A** 正确。

+++

#### 综合选择 (4) 设 $f(x)$ 二阶可导，则下列结论正确的是（　）。

① 当 $f'(x)<0$ 时，则 $\int_{-\pi}^{\pi}f(x)\sin x\,\mathrm{d}x<0$；
② 当 $f'(x)<0$ 时，则 $\int_{-\pi}^{\pi}f(x)\sin x\,\mathrm{d}x>0$；
③ 当 $f''(x)>0$ 时，则 $\int_{-\pi}^{\pi}f(x)\cos x\,\mathrm{d}x>0$；
④ 当 $f''(x)>0$ 时，则 $\int_{-\pi}^{\pi}f(x)\cos x\,\mathrm{d}x<0$.

;;;
A. ②③
B. ①②
C. ②④
D. ①④
;;;D

***

**D**。

**解** 依题意，只需判别被积函数的正、负即可，考虑到 $\sin x$ 在 $[0,\pi]$ 与 $[-\pi,0]$ 上分别非负和非正，有 $\int_{-\pi}^{\pi}f(x)\sin x\,\mathrm{d}x=\int_{-\pi}^{0}f(x)\sin x\,\mathrm{d}x+\int_0^{\pi}f(x)\sin x\,\mathrm{d}x$。而

$$
\int_{-\pi}^{0}f(x)\sin x\,\mathrm{d}x\xlongequal{x=-u}\int_{\pi}^{0}f(-u)\sin(-u)(-\mathrm{d}u)
$$

$$
=-\int_0^{\pi}f(-u)\sin u\,\mathrm{d}u=-\int_0^{\pi}f(-x)\sin x\,\mathrm{d}x,
$$

故

$$
\int_{-\pi}^{\pi}f(x)\sin x\,\mathrm{d}x=\int_0^{\pi}[f(x)-f(-x)]\sin x\,\mathrm{d}x.
$$

由 $f'(x)<0$，知 $f(x)$ 单调减少，故当 $x\in[0,\pi]$ 时，有 $f(x)\leqslant f(-x)$，于是

$$
\int_{-\pi}^{\pi}f(x)\sin x\,\mathrm{d}x=\int_0^{\pi}[f(x)-f(-x)]\sin x\,\mathrm{d}x<0,
$$

故 ① 正确。

又

$$
\int_{-\pi}^{\pi}f(x)\cos x\,\mathrm{d}x=\int_{-\pi}^{\pi}f(x)\,\mathrm{d}(\sin x)=f(x)\sin x\bigg|_{-\pi}^{\pi}-\int_{-\pi}^{\pi}f'(x)\sin x\,\mathrm{d}x=-\int_{-\pi}^{\pi}f'(x)\sin x\,\mathrm{d}x,
$$

且由 $f''(x)>0$，知 $f'(x)$ 单调增加，从而 $-f'(x)$ 单调减少。由 ① 正确，知

$$
\int_{-\pi}^{\pi}f(x)\cos x\,\mathrm{d}x=-\int_{-\pi}^{\pi}f'(x)\sin x\,\mathrm{d}x<0,
$$

故 ④ 正确，从而 **D** 正确。

【注】作为选择题，可用取特殊值法，如对 ①② 取 $f(x)=-x$，对 ①④ 取 $f(x)=\mathrm{e}^x$。

+++

#### 综合选择 (5) 设反常积分 $\int_1^{+\infty}x^k\left(\mathrm{e}^{-\cos\frac1x}-\mathrm{e}^{-1}\right)\mathrm{d}x$ 收敛，则正确的是（　）。

;;;
A. $k>-1$
B. $k<-1$
C. $k>1$
D. $k<1$
;;;D

***

**D**。

**解**

$$
\mathrm{e}^{-\cos\frac1x}-\mathrm{e}^{-1}=\mathrm{e}^{-1}\left(\mathrm{e}^{-\cos\frac1x+1}-1\right).
$$

当 $x\to+\infty$ 时，$\mathrm{e}^{-1}\left(\mathrm{e}^{-\cos\frac1x+1}-1\right)$ 与 $\mathrm{e}^{-1}\left(1-\cos\dfrac1x\right)$ 是等价无穷小，又 $1-\cos\dfrac1x$ 与 $\dfrac{1}{2x^2}$ 是等价无穷小，则 $x^k\left(\mathrm{e}^{-\cos\frac1x}-\mathrm{e}^{-1}\right)$ 与 $\dfrac{1}{2\mathrm{e}x^{2-k}}$ 是等价无穷小。

当 $k<1$ 时，$2-k>1$，故 $\int_1^{+\infty}x^k\left(\mathrm{e}^{-\cos\frac1x}-\mathrm{e}^{-1}\right)\mathrm{d}x$ 收敛；

当 $k\geqslant1$ 时，$2-k\leqslant1$，$\dfrac{1}{2\mathrm{e}x^{2-k}}$ 是阶数不高于 $\dfrac1x$ 的无穷小，故 $\int_1^{+\infty}x^k\left(\mathrm{e}^{-\cos\frac1x}-\mathrm{e}^{-1}\right)\mathrm{d}x$ 发散。

【注】结论：$\int_a^{+\infty}\dfrac{1}{x^p}\mathrm{d}x\ (a>0,\ p$ 为任意实数$)$，当 $p\leqslant1$ 时，发散；当 $p>1$ 时，收敛于 $\dfrac{a^{1-p}}{p-1}$。

+++

#### 综合选择 (6) 设连续函数 $f(x)$ 满足 $f(x)=f(2a-x)\ (a\neq0)$，$b$ 为常数，则 $\int_{-b}^{b}f(a-x)\,\mathrm{d}x=$（　）。

;;;
A. $2\int_0^{b}f(2a-x)\,\mathrm{d}x$
B. $2\int_{-b}^{b}f(2a-x)\,\mathrm{d}x$
C. $2\int_0^{b}f(a-x)\,\mathrm{d}x$
D. $0$
;;;C

***

**C**。

**解**

$$
\int_{-b}^{b}f(a-x)\,\mathrm{d}x=\int_{-b}^{0}f(a-x)\,\mathrm{d}x+\int_0^{b}f(a-x)\,\mathrm{d}x.
$$

由 $f(x)=f(2a-x)$，得 $f(a+x)=f(a-x)$，则

$$
\int_{-b}^{0}f(a-x)\,\mathrm{d}x\xlongequal{x=-t}-\int_{b}^{0}f(a+t)\,\mathrm{d}t=\int_0^{b}f(a-t)\,\mathrm{d}t=\int_0^{b}f(a-x)\,\mathrm{d}x,
$$

故 $\int_{-b}^{b}f(a-x)\,\mathrm{d}x=2\int_0^{b}f(a-x)\,\mathrm{d}x$。**C** 正确。

+++

#### 综合选择 (7) 设 $\varphi(x)=\dfrac{x^2}{x-1}\int_1^{x}f(t)\,\mathrm{d}t$，$f(x)$ 为连续函数，则 $\lim\limits_{x\to1}\varphi(x)=$（　）。

;;;
A. $1$
B. $f(1)$
C. $0$
D. 不存在
;;;B

***

**B**。

**解**

$$
\lim\limits_{x\to1}\varphi(x)=\lim\limits_{x\to1}\dfrac{x^2\int_1^{x}f(t)\,\mathrm{d}t}{x-1}=\lim\limits_{x\to1}\dfrac{2x\int_1^{x}f(t)\,\mathrm{d}t+x^2f(x)}{1}=f(1).
$$

**B** 正确。

+++

#### 综合选择 (8) 设 $f(x)$ 有连续导数，$f(0)=0$，$f'(0)=6$，$\alpha(x)=\int_0^{x^3}f(t)\,\mathrm{d}t$，$\beta(x)=\left[\int_0^{x}f(t)\,\mathrm{d}t\right]^3$，则当 $x\to0$ 时，$\alpha(x)$ 与 $\beta(x)$ 是（　）。

;;;
A. 同阶无穷小
B. 等价无穷小
C. 高阶无穷小
D. 低阶无穷小
;;;A

***

**A**。

**解** 令 $g(x)=\int_0^{x}f(t)\,\mathrm{d}t$，则

$$
g(x^3)=\int_0^{x^3}f(t)\,\mathrm{d}t,\quad g'(x)=f(x),\quad g''(x)=f'(x),
$$

故

$$
\lim\limits_{x\to0}\dfrac{g(x)}{x^2}=\lim\limits_{x\to0}\dfrac{g'(x)}{2x}=\lim\limits_{x\to0}\dfrac{g''(x)}{2}=\lim\limits_{x\to0}\dfrac{f'(x)}{2}=\dfrac{f'(0)}{2}=3,
$$

即有 $\lim\limits_{x\to0}\dfrac{g(x)}{3x^2}=1$，所以 $g(x)\sim3x^2$，$g(x^3)\sim3(x^3)^2=3x^6$，故

$$
\lim\limits_{x\to0}\dfrac{\alpha(x)}{\beta(x)}=\lim\limits_{x\to0}\dfrac{3x^6}{(3x^2)^3}=\dfrac19.
$$

+++

#### 综合选择 (9) 设 $I=\dfrac{1}{s}\int_0^{st}f\left(t+\dfrac{x}{s}\right)\mathrm{d}x$，$s>0$，$t>0$，则正确的是（　）。

;;;
A. $I$ 仅依赖于 $s$
B. $I$ 仅依赖于 $t$
C. $I$ 依赖于 $s,t$
D. $I$ 依赖于 $s,t,x$
;;;B

***

**B**。

**解** 令 $t+\dfrac{x}{s}=u$，则 $\mathrm{d}u=\dfrac1s\mathrm{d}x$，故

$$
I=\dfrac1s\int_0^{st}f\left(t+\dfrac{x}{s}\right)\mathrm{d}x=\dfrac1s\int_t^{2t}f(u)s\,\mathrm{d}u=\int_t^{2t}f(u)\,\mathrm{d}u.
$$

**B** 正确。

+++

#### 综合选择 (10) 设积分 $I=\int_1^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}\ (p>0,\ q>0)$ 收敛，则（　）。

;;;
A. $p>1$ 且 $q<1$
B. $p>1$ 且 $q>1$
C. $p<1$ 且 $q<1$
D. $p<1$ 且 $q>1$
;;;A

***

**A**。

**解**

$$
I=\int_1^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}=\int_1^{\mathrm{e}}\dfrac{\mathrm{d}x}{x^p\ln^qx}+\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}.
$$

因为 $\ln x=\ln[1+(x-1)]\sim x-1\ (x\to1)$，所以 $\lim\limits_{x\to1^+}\dfrac{\frac{1}{x^p\ln^qx}}{\frac{1}{(x-1)^q}}=1$，从而 $\int_1^{\mathrm{e}}\dfrac{\mathrm{d}x}{x^p\ln^qx}$ 与 $\int_1^{\mathrm{e}}\dfrac{\mathrm{d}x}{(x-1)^q}$ 敛散性相同，故当 $q<1$ 时，$\int_1^{\mathrm{e}}\dfrac{\mathrm{d}x}{x^p\ln^qx}$ 收敛。

当 $q<1$，$p=1$ 时，$\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x\ln^qx}=\dfrac{1}{1-q}\ln^{1-q}x\bigg|_{\mathrm{e}}^{+\infty}=\infty$，故发散；

当 $q<1$，$p<1$ 时，对 $\forall\,p<a<1$，$\lim\limits_{x\to+\infty}\dfrac{\frac{1}{x^p\ln^qx}}{\frac{1}{x^a}}=+\infty$，且 $\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^a}$ 发散，故 $\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}$ 发散；

当 $q<1$，$p>1$ 时，$\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}<\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^p}$，故 $\int_{\mathrm{e}}^{+\infty}\dfrac{\mathrm{d}x}{x^p\ln^qx}$ 收敛。

综上所述，当 $p>1$，$q<1$ 时，积分收敛，**A** 正确。

+++

#### 综合填空 (1) $f(x)=\max\{1,x^2\}$ 在 $(-\infty,+\infty)$ 内满足 $F(0)=1$ 的一个原函数为 $\underline{\quad}$。

***

$$
F(x)=\begin{cases}\dfrac13x^3+\dfrac13,&x<-1,\\[2mm] x+1,&-1\leqslant x\leqslant1,\\[2mm] \dfrac13x^3+\dfrac53,&x>1.\end{cases}
$$

**解**

$$
f(x)=\max\{1,x^2\}=\begin{cases}x^2,&x<-1\ \text{或}\ x>1,\\ 1,&|x|\leqslant1,\end{cases}
$$

积分，得

$$
F(x)=\int f(x)\,\mathrm{d}x=\begin{cases}\dfrac13x^3+C_1,&x<-1,\\[2mm] x+C_2,&-1\leqslant x\leqslant1,\\[2mm] \dfrac13x^3+C_3,&x>1.\end{cases}
$$

令 $x=0$，则由 $F(0)=1$，知 $C_2=1$，故当 $-1\leqslant x\leqslant1$ 时，$F(x)=x+1$。

又因为原函数 $F(x)$ 处处可导，所以 $F(x)$ 连续，从而有

$$
\lim\limits_{x\to(-1)^-}F(x)=\lim\limits_{x\to(-1)^+}F(x)=F(-1),\quad \lim\limits_{x\to1^-}F(x)=\lim\limits_{x\to1^+}F(x)=F(1),
$$

即 $\begin{cases}-\dfrac13+C_1=-1+1=0,\\[2mm] \dfrac13+C_3=1+1,\end{cases}$ 解得 $C_1=\dfrac13$，$C_3=\dfrac53$。

+++

#### 综合填空 (2) 设 $f(x)$ 在 $[a,b]$ 上连续，若 $x_0\in[a,b]$，$x\in[a,b]$，则极限 $\lim\limits_{\Delta x\to0}\dfrac{1}{\Delta x}\int_{x_0}^{x}[f(t+\Delta x)-f(t)]\,\mathrm{d}t=\underline{\quad}$。

***

$f(x)-f(x_0)$。

**解** 由于 $\int_{x_0}^{x}f(t+\Delta x)\,\mathrm{d}t\xlongequal{t+\Delta x=u}\int_{x_0+\Delta x}^{x+\Delta x}f(u)\,\mathrm{d}u$，故

$$
\lim\limits_{\Delta x\to0}\dfrac{1}{\Delta x}\int_{x_0}^{x}[f(t+\Delta x)-f(t)]\,\mathrm{d}t=\lim\limits_{\Delta x\to0}\dfrac{\int_{x_0+\Delta x}^{x+\Delta x}f(u)\,\mathrm{d}u-\int_{x_0}^{x}f(t)\,\mathrm{d}t}{\Delta x}
$$

$$
\xlongequal{\text{洛必达法则}}\lim\limits_{\Delta x\to0}[f(x+\Delta x)-f(x_0+\Delta x)]=f(x)-f(x_0).
$$

【注】① $\int_{x_0}^{x}f(t)\,\mathrm{d}t$ 不含 $\Delta x$，对 $\Delta x\to0$ 的极限而言为常数。

② 以下解法是错误的，一般情况下，积分号与极限号不能任意交换：

$$
\lim\limits_{\Delta x\to0}\dfrac{1}{\Delta x}\int_{x_0}^{x}[f(t+\Delta x)-f(t)]\,\mathrm{d}t=\lim\limits_{\Delta x\to0}\int_{x_0}^{x}\dfrac{f(t+\Delta x)-f(t)}{\Delta x}\,\mathrm{d}t
$$

$$
=\int_{x_0}^{x}\lim\limits_{\Delta x\to0}\dfrac{f(t+\Delta x)-f(t)}{\Delta x}\,\mathrm{d}t=\int_{x_0}^{x}f'(t)\,\mathrm{d}t=f(x)-f(x_0).
$$

+++

#### 综合填空 (3) 由曲线 $y=x(x-1)(2-x)$ 与 $x$ 轴围成的平面图形的面积 $A=\underline{\quad}$。

***

$\dfrac12$。

**解** 曲线与 $x$ 轴的交点为 $(0,0)$，$(1,0)$，$(2,0)$，在区间 $[0,1]$ 上，$y<0$；在区间 $[1,2]$ 上，$y>0$，故所求面积为

$$
A=-\int_0^{1}x(x-1)(2-x)\,\mathrm{d}x+\int_1^{2}x(x-1)(2-x)\,\mathrm{d}x=\dfrac14+\dfrac14=\dfrac12.
$$

+++

#### 综合填空 (4) 双纽线 $(x^2+y^2)^2=x^2-y^2$ 围成的平面图形的面积为 $\underline{\quad}$。

***

$1$。

**解** 双纽线的极坐标方程为

$$
r^2=\cos2\theta\left(-\dfrac{\pi}{4}\leqslant\theta\leqslant\dfrac{\pi}{4},\ \dfrac{3\pi}{4}\leqslant\theta\leqslant\dfrac{5\pi}{4}\right).
$$

如图 3-10 所示，由对称性，知面积 $A$ 为

$$
A=4\cdot\dfrac12\int_0^{\frac{\pi}{4}}r^2\,\mathrm{d}\theta=2\int_0^{\frac{\pi}{4}}\cos2\theta\,\mathrm{d}\theta=1.
$$

+++

#### 综合填空 (5) 已知 $f'(\mathrm{e}^x)=x\mathrm{e}^{-x}$，且 $f(1)=0$，则 $f(x)=\underline{\quad}$。

***

$\dfrac{(\ln x)^2}{2}$。

**解** 令 $\mathrm{e}^x=t$，则 $x=\ln t$，$f'(t)=\dfrac{\ln t}{t}$，故

$$
f(t)=\int f'(t)\,\mathrm{d}t=\int\dfrac{\ln t}{t}\,\mathrm{d}t=\dfrac12(\ln t)^2+C.
$$

由 $f(1)=0$，得 $C=0$，故 $f(x)=\dfrac{(\ln x)^2}{2}$。

+++

#### 综合填空 (6) 已知 $f'(x)=\sqrt{1-\cos2x}$，$x\in\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$，$f(0)=0$，则 $f(x)=\underline{\quad}$。

***

$$
f(x)=\begin{cases}\sqrt2(1-\cos x),&0\leqslant x\leqslant\dfrac{\pi}{2},\\[2mm] \sqrt2(\cos x-1),&-\dfrac{\pi}{2}\leqslant x<0.\end{cases}
$$

**解**

$$
f(x)=\int\sqrt{1-\cos2x}\,\mathrm{d}x=\sqrt2\int|\sin x|\,\mathrm{d}x=\begin{cases}-\sqrt2\cos x+C_1,&0\leqslant x\leqslant\dfrac{\pi}{2},\\[2mm] \sqrt2\cos x+C_2,&-\dfrac{\pi}{2}\leqslant x<0.\end{cases}
$$

由原函数的可导性，可知 $f(x)$ 在 $x=0$ 处必连续，所以

$$
f(0)=0=-\sqrt2+C_1=\sqrt2+C_2,
$$

解得 $C_1=\sqrt2$，$C_2=-\sqrt2$。

+++

#### 综合填空 (7) 设 $f(x)$ 连续，$g(x)=\int_0^{x^2}xf(t)\,\mathrm{d}t$，且 $g(1)=1$，$g'(1)=5$，则 $f(1)=\underline{\quad}$。

***

$2$。

**解**

$$
g(x)=\int_0^{x^2}xf(t)\,\mathrm{d}t=x\int_0^{x^2}f(t)\,\mathrm{d}t,
$$

由 $g(1)=1$，知 $\int_0^{1}f(t)\,\mathrm{d}t=1$。又 $g'(x)=\int_0^{x^2}f(t)\,\mathrm{d}t+2x^2f(x^2)$，由 $g'(1)=5$，知

$$
5=\int_0^{1}f(t)\,\mathrm{d}t+2f(1)=1+2f(1),
$$

故 $f(1)=2$。

+++

#### 综合填空 (8) 设 $f(2)=\dfrac12$，$f'(2)=0$，且 $\int_0^{2}f(x)\,\mathrm{d}x=1$，则 $I=\int_0^{1}x^2f''(2x)\,\mathrm{d}x=\underline{\quad}$。

***

$0$。

**解**

$$
I=\int_0^{1}x^2f''(2x)\,\mathrm{d}x=\dfrac12\int_0^{1}x^2\,\mathrm{d}[f'(2x)]
$$

$$
=\dfrac12\left[x^2f'(2x)\bigg|_0^{1}-\int_0^{1}2xf'(2x)\,\mathrm{d}x\right]
$$

$$
=-\dfrac12\int_0^{1}x\,\mathrm{d}[f(2x)]=-\dfrac12\left[xf(2x)\bigg|_0^{1}-\int_0^{1}f(2x)\,\mathrm{d}x\right]
$$

$$
=\dfrac12\int_0^{1}f(2x)\,\mathrm{d}x-\dfrac12f(2)\xlongequal{2x=t}\dfrac14\int_0^{2}f(t)\,\mathrm{d}t-\dfrac14=0.
$$

+++

#### 综合填空 (9) 设 $f(x)=\int_0^{x}\mathrm{e}^{\cos t}\,\mathrm{d}t$，则 $I=\int_0^{\pi}f(x)\cos x\,\mathrm{d}x=\underline{\quad}$。

***

$\mathrm{e}^{-1}-\mathrm{e}$。

**解**

$$
I=\int_0^{\pi}f(x)\cos x\,\mathrm{d}x=\int_0^{\pi}f(x)\,\mathrm{d}(\sin x)=f(x)\sin x\bigg|_0^{\pi}-\int_0^{\pi}f'(x)\sin x\,\mathrm{d}x
$$

$$
=0-\int_0^{\pi}\mathrm{e}^{\cos x}\sin x\,\mathrm{d}x=\int_0^{\pi}\mathrm{e}^{\cos x}\,\mathrm{d}(\cos x)=\mathrm{e}^{\cos x}\bigg|_0^{\pi}=\mathrm{e}^{-1}-\mathrm{e}.
$$

+++

#### 综合填空 (10) 设 $\int_0^{+\infty}\dfrac{\sin x}{x}\,\mathrm{d}x=\dfrac{\pi}{2}$，则 $I=\int_0^{+\infty}\dfrac{\sin^2x}{x^2}\,\mathrm{d}x=\underline{\quad}$。

***

$\dfrac{\pi}{2}$。

**解**

$$
I=\int_0^{+\infty}\dfrac{\sin^2x}{x^2}\,\mathrm{d}x=-\int_0^{+\infty}\sin^2x\,\mathrm{d}\left(\dfrac1x\right)
$$

$$
=-\dfrac{\sin^2x}{x}\bigg|_0^{+\infty}+\int_0^{+\infty}\dfrac{2\sin x\cos x}{x}\,\mathrm{d}x
$$

$$
=\int_0^{+\infty}\dfrac{\sin2x}{x}\,\mathrm{d}x\xlongequal{2x=t}\int_0^{+\infty}\dfrac{\sin t}{t}\,\mathrm{d}t=\dfrac{\pi}{2}.
$$

+++

#### 综合解答 (1) 求下列积分：

（Ⅰ）设 $f(x)=\displaystyle\int_1^x\dfrac{\mathrm{d}t}{\sqrt{1+t^4}}$，求 $I=\displaystyle\int_0^1x^2f(x)\mathrm{d}x$；
（Ⅱ）设 $f(x)=\displaystyle\int_1^{x^2}\mathrm{e}^{-t^2}\mathrm{d}t$，求 $I=\displaystyle\int_0^1xf(x)\mathrm{d}x$。

***

（Ⅰ）

$$
\begin{aligned}
I&=\int_0^1x^2f(x)\mathrm{d}x=\int_0^1f(x)\mathrm{d}\left(\frac{x^3}{3}\right)\\
&=\frac13x^3f(x)\Big|_0^1-\frac13\int_0^1\frac{x^3\mathrm{d}x}{\sqrt{1+x^4}}\\
&=-\frac16(1+x^4)^{\frac12}\Big|_0^1=\frac16(1-\sqrt2).
\end{aligned}
$$

（Ⅱ）

$$
\begin{aligned}
I&=\int_0^1xf(x)\mathrm{d}x=\frac12\int_0^1f(x)\mathrm{d}(x^2)=\frac12x^2f(x)\Big|_0^1-\frac12\int_0^1x^2f'(x)\mathrm{d}x\\
&=-\int_0^1x^3\mathrm{e}^{-x^4}\mathrm{d}x=\frac14\mathrm{e}^{-x^4}\Big|_0^1=\frac14(\mathrm{e}^{-1}-1),
\end{aligned}
$$

这里 $f(1)=0$。

**【注】** 积分 $\displaystyle\int\dfrac{\mathrm{d}x}{\sqrt{1+x^4}}$，$\displaystyle\int\mathrm{e}^{\pm x^2}\mathrm{d}x$，$\displaystyle\int\dfrac{\sin x}{x}\mathrm{d}x$，$\displaystyle\int\dfrac{\cos x}{x}\mathrm{d}x$ 俗称“积不出来”，即原函数不能用初等函数表达。

+++

#### 综合解答 (2) 设 $f(\sin^2x)=\dfrac{x}{\sin x}$，求 $I=\displaystyle\int\dfrac{\sqrt{x}}{\sqrt{1-x}}f(x)\mathrm{d}x$。

***

令 $\sin^2x=t$，则 $\sin x=\pm\sqrt{t}$，由 $\sqrt{x}\geqslant0$，$\sqrt{1-x}\geqslant0$，可知 $x\geqslant0$，$1-x\geqslant0$，故 $0\leqslant x\leqslant1$，所以 $\sin x\geqslant0$。

取 $\sin x=\sqrt{t}$，则 $x=\arcsin\sqrt{t}$，$f(t)=\dfrac{\arcsin\sqrt{t}}{\sqrt{t}}$，故

$$
\begin{aligned}
I&=\int\frac{\sqrt{x}}{\sqrt{1-x}}f(x)\mathrm{d}x=\int\frac{\sqrt{x}}{\sqrt{1-x}}\cdot\frac{\arcsin\sqrt{x}}{\sqrt{x}}\mathrm{d}x\\
&=-\int\frac{\arcsin\sqrt{x}}{\sqrt{1-x}}\mathrm{d}(1-x)=-2\int\arcsin\sqrt{x}\,\mathrm{d}(\sqrt{1-x})\\
&=-2\sqrt{1-x}\arcsin\sqrt{x}+2\int\sqrt{1-x}\,\mathrm{d}(\arcsin\sqrt{x})\\
&=-2\sqrt{1-x}\arcsin\sqrt{x}+2\sqrt{x}+C.
\end{aligned}
$$

+++

#### 综合解答 (3) 计算积分 $I=\displaystyle\int\mathrm{e}^{\sin x}\cdot\dfrac{x\cos^3x-\sin x}{\cos^2x}\mathrm{d}x$。

***

$$
\begin{aligned}
I&=\int\mathrm{e}^{\sin x}\left(x\cos x-\frac{\sin x}{\cos^2x}\right)\mathrm{d}x=\int x\cos x\,\mathrm{e}^{\sin x}\mathrm{d}x-\int\mathrm{e}^{\sin x}\cdot\frac{\sin x}{\cos^2x}\mathrm{d}x\\
&=\int x\,\mathrm{d}(\mathrm{e}^{\sin x})+\int\mathrm{e}^{\sin x}\mathrm{d}\left(-\frac{1}{\cos x}\right)\\
&=x\mathrm{e}^{\sin x}-\int\mathrm{e}^{\sin x}\mathrm{d}x-\frac{\mathrm{e}^{\sin x}}{\cos x}+\int\mathrm{e}^{\sin x}\cos x\cdot\frac{1}{\cos x}\mathrm{d}x\\
&=x\mathrm{e}^{\sin x}-\frac{\mathrm{e}^{\sin x}}{\cos x}+C.
\end{aligned}
$$

+++

#### 综合解答 (4) 计算 $I=\displaystyle\int\dfrac{\mathrm{e}^{-\sin x}\cdot\sin 2x}{\sin^4\left(\dfrac{\pi}{4}-\dfrac{x}{2}\right)}\mathrm{d}x$。

***

$$
\begin{aligned}
I&=\int\frac{\mathrm{e}^{-\sin x}\cdot2\sin x\cos x}{\left[\sin^2\left(\dfrac{\pi}{4}-\dfrac{x}{2}\right)\right]^2}\mathrm{d}x=\int\frac{\mathrm{e}^{-\sin x}\cdot2\sin x\cos x}{\left[\dfrac{1-\cos\left(\dfrac{\pi}{2}-x\right)}{2}\right]^2}\mathrm{d}x\\
&=8\int\frac{\mathrm{e}^{-\sin x}(-\sin x)\mathrm{d}(-\sin x)}{(1-\sin x)^2}\xlongequal{-\sin x=u}8\int\mathrm{e}^{u}\cdot\frac{u}{(1+u)^2}\mathrm{d}u\\
&=8\int\mathrm{e}^{u}\left[\frac{1}{1+u}-\frac{1}{(1+u)^2}\right]\mathrm{d}u=8\left[\int\frac{\mathrm{e}^{u}}{1+u}\mathrm{d}u-\int\frac{\mathrm{e}^{u}}{(1+u)^2}\mathrm{d}u\right]\\
&=8\left(\int\frac{\mathrm{e}^{u}}{1+u}\mathrm{d}u+\frac{\mathrm{e}^{u}}{1+u}-\int\frac{\mathrm{e}^{u}}{1+u}\mathrm{d}u\right)+C\\
&=\frac{8\mathrm{e}^{u}}{1+u}+C=\frac{8\mathrm{e}^{-\sin x}}{1-\sin x}+C.
\end{aligned}
$$

+++

#### 综合解答 (5) 设 $f(\ln x)=\dfrac{\ln(1+x)}{x}$，求 $I=\displaystyle\int f(x)\mathrm{d}x$。

***

令 $\ln x=t$，则 $x=\mathrm{e}^{t}$，故 $f(t)=f(\ln x)=\dfrac{\ln(1+\mathrm{e}^{t})}{\mathrm{e}^{t}}$，

$$
\begin{aligned}
I&=\int f(x)\mathrm{d}x=\int\frac{\ln(1+\mathrm{e}^{x})}{\mathrm{e}^{x}}\mathrm{d}x=-\int\ln(1+\mathrm{e}^{x})\mathrm{d}(\mathrm{e}^{-x})\\
&=-\mathrm{e}^{-x}\ln(1+\mathrm{e}^{x})+\int\left(1-\frac{\mathrm{e}^{x}}{1+\mathrm{e}^{x}}\right)\mathrm{d}x\\
&=x-(1+\mathrm{e}^{-x})\ln(1+\mathrm{e}^{x})+C.
\end{aligned}
$$

+++

#### 综合解答 (6) 设 $f'(x)=\arctan(x-1)^2$，$f(0)=0$，求 $I=\displaystyle\int_0^1f(x)\mathrm{d}x$。

***

$$
\begin{aligned}
I&=\int_0^1f(x)\mathrm{d}x=xf(x)\Big|_0^1-\int_0^1xf'(x)\mathrm{d}x\\
&=f(1)-\int_0^1x\arctan(x-1)^2\mathrm{d}x\\
&=f(1)-\int_0^1(x-1+1)\arctan(x-1)^2\mathrm{d}(x-1)\\
&=f(1)-\int_0^1(x-1)\arctan(x-1)^2\mathrm{d}(x-1)-\int_0^1\arctan(x-1)^2\mathrm{d}x\\
&=f(1)-\int_0^1(x-1)\arctan(x-1)^2\mathrm{d}(x-1)-\int_0^1f'(x)\mathrm{d}x\\
&=f(1)-\frac12\int_0^1\arctan(x-1)^2\mathrm{d}\left[(x-1)^2\right]-\left[f(1)-f(0)\right]\\
&=-\frac12(x-1)^2\arctan(x-1)^2\Big|_0^1+\frac12\int_0^1\frac{(x-1)^2\cdot2(x-1)}{1+(x-1)^4}\mathrm{d}x\\
&=\frac{\pi}{8}+\frac14\int_0^1\frac{1}{1+(x-1)^4}\mathrm{d}\left[(x-1)^4\right]\\
&=\frac{\pi}{8}+\frac14\ln\left[1+(x-1)^4\right]\Big|_0^1=\frac{\pi}{8}-\frac14\ln2.
\end{aligned}
$$

+++

#### 综合解答 (7) 求极限 $\lim\limits_{x\to0}\dfrac{\dfrac12\displaystyle\int_0^2x\sqrt{4-x^2u^2}\,\mathrm{d}u-2x}{\sqrt{1+2x^3}-1}$。

***

当 $x\to0$ 时，$\sqrt{1+2x^3}-1\sim\dfrac12\cdot2x^3=x^3$，又

$$
\frac12\int_0^2x\sqrt{4-x^2u^2}\,\mathrm{d}u\xlongequal{xu=t}\frac12\int_0^{2x}\sqrt{4-t^2}\,\mathrm{d}t,
$$

所以

$$
\begin{aligned}
\text{原式}&=\lim\limits_{x\to0}\frac{\dfrac12\displaystyle\int_0^{2x}\sqrt{4-t^2}\,\mathrm{d}t-2x}{x^3}=\lim\limits_{x\to0}\frac{\dfrac12\sqrt{4-4x^2}\cdot2-2}{3x^2}\\
&=\lim\limits_{x\to0}\frac{2(\sqrt{1-x^2}-1)}{3x^2}=\lim\limits_{x\to0}\frac{2\cdot\dfrac12(-x^2)}{3x^2}=-\frac13.
\end{aligned}
$$

+++

#### 综合解答 (8) 设 $f(x)$ 在 $(-\infty,0]$ 上连续，且满足

$$
\int_0^xtf(t^2-x^2)\mathrm{d}t=\frac{x^2}{1+x^2}-\frac12\ln(1+x^2),
$$

求函数 $f(x)$ 及其极值。

***

$$
\int_0^xtf(t^2-x^2)\mathrm{d}t=\frac12\int_0^xf(t^2-x^2)\mathrm{d}(t^2-x^2)\xlongequal{u=t^2-x^2}\frac12\int_{-x^2}^0f(u)\mathrm{d}u,
$$

即 $-\dfrac12\displaystyle\int_0^{-x^2}f(u)\mathrm{d}u=\dfrac{x^2}{1+x^2}-\dfrac12\ln(1+x^2)$。

令 $t=-x^2$，得 $-\dfrac12\displaystyle\int_0^tf(u)\mathrm{d}u=\dfrac{-t}{1-t}-\dfrac12\ln(1-t)$，两边同时对 $t$ 求导，得

$$
f(t)=\frac{2}{(1-t)^2}-\frac{1}{1-t}=\frac{1+t}{(1-t)^2},\quad t\leqslant0,
$$

即 $f(x)=\dfrac{1+x}{(1-x)^2}$，$x\leqslant0$。

由 $f'(x)=\dfrac{x+3}{(1-x)^3}$，知 $x=-3$ 为 $(-\infty,0]$ 上的唯一驻点，且可判别当 $x=-3$ 时，$f(x)$ 取得极小值 $f(-3)=-\dfrac18$。

+++

#### 综合解答 (9) 设 $f(x)$ 在 $(0,+\infty)$ 内一阶可导，$g(x)$ 为 $f(x)$ 的反函数，且 $g(x)$ 连续，若

$$
\int_1^{f(x)}g(t)\mathrm{d}t=x^2\mathrm{e}^{x}-4\mathrm{e}^2-\int_1^{x-1}f(t+1)\mathrm{d}t,\quad f(2)=1,
$$

求 $f(x)$ 的表达式。

***

在已知等式两端同时对 $x$ 求导，得

$$
g\left[f(x)\right]f'(x)=2x\mathrm{e}^{x}+x^2\mathrm{e}^{x}-f(x),
$$

故 $xf'(x)=2x\mathrm{e}^{x}+x^2\mathrm{e}^{x}-f(x)$，即 $f'(x)+\dfrac1xf(x)=(2+x)\mathrm{e}^{x}$。解一阶线性微分方程，得

$$
f(x)=\mathrm{e}^{-\int\frac1x\mathrm{d}x}\left[\int(2+x)\mathrm{e}^{x}\cdot\mathrm{e}^{\int\frac1x\mathrm{d}x}\mathrm{d}x+C\right]=\frac1x(x^2\mathrm{e}^{x}+C).
$$

又由 $f(2)=1$，知 $\dfrac12(4\mathrm{e}^2+C)=1$，解得 $C=2-4\mathrm{e}^2$，故 $f(x)=x\mathrm{e}^{x}+\dfrac{2-4\mathrm{e}^2}{x}$ $(x>0)$。

+++

#### 综合解答 (10) 设 $f(x)$ 在 $[1,2]$ 上可导，且 $\displaystyle\int_0^xtf(2x-t)\mathrm{d}t=\dfrac12\arctan x^2$，$f(1)=\dfrac12$，证明：至少存在一点 $\xi\in(1,2)$，使得 $f'(\xi)=0$。

***

$$
\begin{aligned}
\int_0^xtf(2x-t)\mathrm{d}t&\xlongequal{2x-t=u}\int_{2x}^x(2x-u)f(u)\mathrm{d}(-u)\\
&=\int_x^{2x}(2x-u)f(u)\mathrm{d}u=2x\int_x^{2x}f(u)\mathrm{d}u-\int_x^{2x}uf(u)\mathrm{d}u,
\end{aligned}
$$

故

$$
2x\int_x^{2x}f(u)\mathrm{d}u-\int_x^{2x}uf(u)\mathrm{d}u=\frac12\arctan x^2.
$$

等式两端同时对 $x$ 求导，得

$$
2\int_x^{2x}f(u)\mathrm{d}u+2x\left[f(2x)\cdot2-f(x)\right]-\left[2xf(2x)\cdot2-xf(x)\right]=\frac{x}{1+x^4},
$$

即 $2\displaystyle\int_x^{2x}f(u)\mathrm{d}u-xf(x)=\dfrac{x}{1+x^4}$。令 $x=1$，得

$$
2\int_1^2f(u)\mathrm{d}u=\frac12+f(1)=\frac12+\frac12=1,
$$

故 $\displaystyle\int_1^2f(u)\mathrm{d}u=\dfrac12$。

由推广的积分中值定理，有 $\displaystyle\int_1^2f(u)\mathrm{d}u=f(\xi_1)(2-1)=\dfrac12$，即 $f(\xi_1)=\dfrac12$ $(1<\xi_1<2)$。

又 $f(1)=\dfrac12$，由罗尔定理，至少存在一点 $\xi\in(1,\xi_1)\subset(1,2)$，使得 $f'(\xi)=0$。

+++

#### 综合解答 (11) 设 $f(x)$ 满足 $\mathrm{e}^{-x}-\dfrac{x^2}{2}=1+\displaystyle\int_0^xf(t-x)\mathrm{d}t$，求 $f(x)$ 在 $(-\infty,+\infty)$ 内的最值。

***

$$
\int_0^xf(t-x)\mathrm{d}t\xlongequal{t-x=u}\int_{-x}^0f(u)\mathrm{d}u.
$$

由已知，有 $\mathrm{e}^{-x}-\dfrac{x^2}{2}=1+\displaystyle\int_{-x}^0f(u)\mathrm{d}u$。两边同时对 $x$ 求导，得 $-\mathrm{e}^{-x}-x=f(-x)$，于是

$$
f(x)=x-\mathrm{e}^{x},\quad x\in(-\infty,+\infty).
$$

由 $f'(x)=1-\mathrm{e}^{x}=0$，解得 $x=0$。当 $x>0$ 时，$f'(x)<0$；当 $x<0$ 时，$f'(x)>0$，$f(0)=-1$ 为极大值。

又 $\lim\limits_{x\to-\infty}f(x)=-\infty$，$\lim\limits_{x\to+\infty}f(x)=-\infty$，故在 $(-\infty,+\infty)$ 内 $f(x)$ 的最大值为 $f(0)=-1$，没有最小值。

+++

#### 综合解答 (12) 求 $f(x)=\displaystyle\int_0^{x^2}(2-t)\mathrm{e}^{-t}\mathrm{d}t$ 的最大值和最小值。

***

因为 $f(x)$ 是偶函数，所以只需求 $f(x)$ 在 $[0,+\infty)$ 上的最值即可。

由 $f'(x)=2x(2-x^2)\mathrm{e}^{-x^2}=0$，得驻点 $x_1=0$，$x_2=\sqrt2$。

当 $0<x<\sqrt2$ 时，$f'(x)>0$；当 $x>\sqrt2$ 时，$f'(x)<0$。又

$$
\lim\limits_{x\to+\infty}f(x)=\int_0^{+\infty}(2-t)\mathrm{e}^{-t}\mathrm{d}t=-2\mathrm{e}^{-t}\Big|_0^{+\infty}+t\mathrm{e}^{-t}\Big|_0^{+\infty}+\mathrm{e}^{-t}\Big|_0^{+\infty}=1,
$$

比较 $f(0)=0$，$f(\sqrt2)=1+\mathrm{e}^{-2}$，得最小值为 $0$，最大值为 $1+\mathrm{e}^{-2}$。

+++

#### 综合解答 (13) 证明：$\lim\limits_{n\to\infty}\displaystyle\int_0^1\dfrac{x^n}{1+x}\mathrm{d}x=0$。

***

**证法 1** 利用夹逼准则，当 $x\in[0,1]$ 时，有 $0\leqslant\dfrac{x^n}{1+x}\leqslant x^n$。

根据定积分的性质，得 $0\leqslant\displaystyle\int_0^1\dfrac{x^n}{1+x}\mathrm{d}x\leqslant\int_0^1x^n\mathrm{d}x=\dfrac{1}{n+1}$，故 $\lim\limits_{n\to\infty}\displaystyle\int_0^1\dfrac{x^n}{1+x}\mathrm{d}x=0$。

**证法 2** 利用推广的积分中值定理，有

$$
\int_0^1\frac{x^n}{1+x}\mathrm{d}x=\frac{1}{1+\xi}\int_0^1x^n\mathrm{d}x=\frac{1}{(1+\xi)(1+n)}\quad(0<\xi<1),
$$

故

$$
\lim\limits_{n\to\infty}\int_0^1\frac{x^n}{1+x}\mathrm{d}x=\lim\limits_{n\to\infty}\frac{1}{(1+\xi)(1+n)}=0.
$$

**【注】** 推广的积分中值定理：设 $f(x)$ 在 $[a,b]$ 上连续，$g(x)$ 在 $[a,b]$ 上可积且不变号，则至少存在一点 $\xi\in(a,b)$，使得

$$
\int_a^bf(x)g(x)\mathrm{d}x=f(\xi)\int_a^bg(x)\mathrm{d}x.
$$

+++

#### 综合解答 (14) 求极限 $\lim\limits_{n\to\infty}\left(\dfrac{2^{\frac1n}}{n+1}+\dfrac{2^{\frac2n}}{n+\dfrac12}+\cdots+\dfrac{2^{\frac{n}{n}}}{n+\dfrac1n}\right)$。

***

令 $x_n=\dfrac{2^{\frac1n}}{n+1}+\dfrac{2^{\frac2n}}{n+\dfrac12}+\cdots+\dfrac{2^{\frac{n}{n}}}{n+\dfrac1n}$，则

$$
\frac{n}{n+1}\left(2^{\frac1n}+2^{\frac2n}+\cdots+2^{\frac{n}{n}}\right)\frac1n\leqslant x_n\leqslant\frac1n\left(2^{\frac1n}+2^{\frac2n}+\cdots+2^{\frac{n}{n}}\right).
$$

由定积分的定义，有 $\lim\limits_{n\to\infty}\left(2^{\frac1n}+2^{\frac2n}+\cdots+2^{\frac{n}{n}}\right)\dfrac1n=\displaystyle\int_0^12^x\mathrm{d}x=\dfrac{2^x}{\ln2}\Big|_0^1=\dfrac{1}{\ln2}$，而 $\lim\limits_{n\to\infty}\dfrac{n}{n+1}=1$，由夹逼准则，知 $\lim\limits_{n\to\infty}x_n=\dfrac{1}{\ln2}$。

+++

#### 综合解答 (15) 求极限 $\lim\limits_{n\to\infty}\dfrac1n\sqrt[n]{n(n+1)(n+2)\cdots(2n-1)}$。

***

令 $x_n=\dfrac1n\sqrt[n]{n(n+1)(n+2)\cdots(2n-1)}$，则

$$
x_n=\sqrt[n]{\frac{n}{n}\cdot\frac{n+1}{n}\cdot\frac{n+2}{n}\cdot\cdots\cdot\frac{n+(n-1)}{n}},
$$

即 $\ln x_n=\dfrac1n\displaystyle\sum_{k=0}^{n-1}\ln\left(1+\dfrac{k}{n}\right)$，故

$$
\lim\limits_{n\to\infty}\ln x_n=\lim\limits_{n\to\infty}\frac1n\sum_{k=0}^{n-1}\ln\left(1+\frac{k}{n}\right)=\int_0^1\ln(1+x)\mathrm{d}x=2\ln2-1=\ln\frac{4}{\mathrm{e}}.
$$

综上可知，原极限 $=\dfrac{4}{\mathrm{e}}$。

+++

#### 综合解答 (16) 设 $\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x$ 收敛，且 $f(x)=\dfrac{1}{1+x^2}-\dfrac{\mathrm{e}^{-x}}{1+\mathrm{e}^{x}}\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x$，求 $\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x$。

***

由于 $\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x$ 收敛，记 $\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x=A$（$A$ 为常数）。

对已知等式两端分别积分，得

$$
A=\int_0^{+\infty}f(x)\mathrm{d}x=\int_0^{+\infty}\frac{1}{1+x^2}\mathrm{d}x-A\int_0^{+\infty}\frac{\mathrm{e}^{-x}}{1+\mathrm{e}^{x}}\mathrm{d}x,
$$

其中 $\displaystyle\int_0^{+\infty}\dfrac{\mathrm{d}x}{1+x^2}=\arctan x\Big|_0^{+\infty}=\dfrac{\pi}{2}$。又

$$
\begin{aligned}
\int_0^{+\infty}\frac{\mathrm{e}^{-x}}{1+\mathrm{e}^{x}}\mathrm{d}x&=\int_0^{+\infty}\frac{\mathrm{d}x}{\mathrm{e}^{x}(1+\mathrm{e}^{x})}=\int_0^{+\infty}\left(\frac{1}{\mathrm{e}^{x}}-\frac{1}{\mathrm{e}^{x}+1}\right)\mathrm{d}x\\
&=-\mathrm{e}^{-x}\Big|_0^{+\infty}-\int_0^{+\infty}\frac{\mathrm{e}^{-x}}{1+\mathrm{e}^{-x}}\mathrm{d}x=1+\ln(1+\mathrm{e}^{-x})\Big|_0^{+\infty}=1-\ln2,
\end{aligned}
$$

故 $A=\dfrac{\pi}{2}-(1-\ln2)A$，解得 $A=\displaystyle\int_0^{+\infty}f(x)\mathrm{d}x=\dfrac{\pi}{2(2-\ln2)}$。

+++

#### 综合解答 (17) 设 $a_n=\displaystyle\int_0^{\frac{\pi}{4}}\tan^nx\,\mathrm{d}x$，证明：$\dfrac{1}{2(n+1)}<a_n<\dfrac{1}{2(n-1)}$ $(n\geqslant2)$。

***

令 $\tan x=t$，则 $x=\arctan t$，故

$$
a_n=\int_0^{\frac{\pi}{4}}\tan^nx\,\mathrm{d}x=\int_0^1\frac{t^n}{1+t^2}\mathrm{d}t<\int_0^1\frac{t^n}{2t}\mathrm{d}t=\frac{t^n}{2n}\Big|_0^1=\frac{1}{2n}<\frac{1}{2n-2}\quad(n\geqslant2).
$$

又

$$
a_n=\int_0^1\frac{t^n}{1+t^2}\mathrm{d}t>\int_0^1\frac{t^n}{1+1^2}\mathrm{d}t=\frac12\cdot\frac{t^{n+1}}{n+1}\Big|_0^1=\frac{1}{2(n+1)},
$$

故 $\dfrac{1}{2(n+1)}<a_n<\dfrac{1}{2n-2}$。证毕。

+++

#### 综合解答 (18) 求积分 $I_n=\displaystyle\int_0^1x\ln^nx\,\mathrm{d}x$（$n\geqslant0$ 且为整数）的递推关系，并计算 $I_n$。

***

利用分部积分法，得

$$
\begin{aligned}
I_n&=\frac12\int_0^1\ln^nx\,\mathrm{d}(x^2)=\frac12x^2\ln^nx\Big|_0^1-\frac12\int_0^1n\ln^{n-1}x\cdot\frac1x\cdot x^2\mathrm{d}x\\
&=-\frac{n}{2}\int_0^1x\ln^{n-1}x\,\mathrm{d}x=-\frac{n}{2}I_{n-1}\quad\left(\text{这里利用了}\lim\limits_{x\to0^+}x^2\ln^nx=0\right).
\end{aligned}
$$

由递推公式，有

$$
\begin{aligned}
I_n&=-\frac{n}{2}\left(-\frac{n-1}{2}\right)I_{n-2}=\left(-\frac{n}{2}\right)\left(-\frac{n-1}{2}\right)\left(-\frac{n-2}{2}\right)I_{n-3}\\
&=\cdots=\left(-\frac{n}{2}\right)\left(-\frac{n-1}{2}\right)\left(-\frac{n-2}{2}\right)\cdots\left(-\frac12\right)I_0,
\end{aligned}
$$

而 $I_0=\displaystyle\int_0^1x\mathrm{d}x=\dfrac12$，故 $I_n=\dfrac{(-1)^n}{2^n}n!\cdot\dfrac12=\dfrac{(-1)^nn!}{2^{n+1}}$。

+++

#### 综合解答 (19) （Ⅰ）求积分 $I_n=\displaystyle\int\dfrac{1}{(x^2+a^2)^n}\mathrm{d}x$ $(n\geqslant1,a>0)$ 的递推关系；\

（Ⅱ）计算 $I=\displaystyle\int\dfrac{3x+4}{(x^2+2x+2)^2}\mathrm{d}x$。

***

（Ⅰ）当 $n\geqslant1$ 时，

$$
\begin{aligned}
I_n&=\int\frac{1}{(x^2+a^2)^n}\mathrm{d}x=\frac{x}{(x^2+a^2)^n}+\int\frac{2nx^2}{(x^2+a^2)^{n+1}}\mathrm{d}x\\
&=\frac{x}{(x^2+a^2)^n}+2n\int\frac{(x^2+a^2)-a^2}{(x^2+a^2)^{n+1}}\mathrm{d}x=\frac{x}{(x^2+a^2)^n}+2nI_n-2na^2I_{n+1},
\end{aligned}
$$

故

$$
I_{n+1}=\frac{1}{2na^2}\left[(2n-1)I_n+\frac{x}{(x^2+a^2)^n}\right],
$$

其中 $I_1=\displaystyle\int\dfrac{1}{x^2+a^2}\mathrm{d}x=\dfrac1a\arctan\dfrac{x}{a}+C$。

（Ⅱ）

$$
\begin{aligned}
I&=\int\frac{3x+4}{(x^2+2x+2)^2}\mathrm{d}x=\int\frac{\dfrac32(2x+2)}{(x^2+2x+2)^2}\mathrm{d}x+\int\frac{1}{(x^2+2x+2)^2}\mathrm{d}x\\
&=-\frac32\frac{1}{x^2+2x+2}+\int\frac{1}{\left[(x+1)^2+1\right]^2}\mathrm{d}(x+1)\\
&=-\frac32\frac{1}{(x+1)^2+1}+\int\left\{\frac{1}{(x+1)^2+1}-\frac{(x+1)^2}{\left[(x+1)^2+1\right]^2}\right\}\mathrm{d}(x+1)\\
&=-\frac32\frac{1}{(x+1)^2+1}+\int\frac{1}{1+(x+1)^2}\mathrm{d}(x+1)+\frac12\int(x+1)\mathrm{d}\left[\frac{1}{(x+1)^2+1}\right]\\
&=-\frac32\frac{1}{(x+1)^2+1}+\arctan(x+1)+\frac{x+1}{2\left[(x+1)^2+1\right]}-\frac12\arctan(x+1)+C\\
&=\frac{x-2}{2(x^2+2x+2)}+\frac12\arctan(x+1)+C.
\end{aligned}
$$

+++

#### 综合解答 (20) 证明：$f(x)=\displaystyle\int_0^x(t-t^2)\sin^{2n}t\,\mathrm{d}t$ $(x>0)$ 的最大值为 $f(1)$，且

$$
f(1)\leqslant\frac{1}{(2n+2)(2n+3)}.
$$

***

由 $f'(x)=(x-x^2)\sin^{2n}x=0$，得驻点 $x_1=1$，$x_2=k\pi$ $(k=1,2,\cdots)$。

在 $x=k\pi$ 两侧，$f'(x)<0$，可知 $x=k\pi$ 不是极值点；

在 $x=1$ 两侧，$f'(x)$ 由正变为负，故 $x=1$ 是唯一极大值点，从而有 $f(x)$ 在 $(0,1]$ 上单调增加，在 $[1,+\infty)$ 上单调减少，即在 $x=1$ 处取最大值，即 $f(1)=\displaystyle\int_0^1(t-t^2)\sin^{2n}t\,\mathrm{d}t$ 是 $f(x)$ 在 $(0,+\infty)$ 内的最大值。

又

$$
\begin{aligned}
f(1)&=\int_0^1(t-t^2)\sin^{2n}t\,\mathrm{d}t\leqslant\int_0^1(t-t^2)t^{2n}\mathrm{d}t\\
&=\frac{1}{2n+2}-\frac{1}{2n+3}=\frac{1}{(2n+2)(2n+3)},
\end{aligned}
$$

即 $f(1)\leqslant\dfrac{1}{(2n+2)(2n+3)}$，故不等式成立。

+++

#### 综合解答 (21) 设 $f(x)$ 在 $[a,b]$ 上有二阶连续导数，且 $f(b)=f'(b)=0$，证明：

$$
\int_a^bf(x)\mathrm{d}x=\frac12\int_a^bf''(x)(x-a)^2\mathrm{d}x.
$$

***

$$
\begin{aligned}
\int_a^bf''(x)(x-a)^2\mathrm{d}x&=\int_a^b(x-a)^2\mathrm{d}\left[f'(x)\right]\\
&=(x-a)^2f'(x)\Big|_a^b-\int_a^b2(x-a)f'(x)\mathrm{d}x=-2\int_a^b(x-a)\mathrm{d}\left[f(x)\right]\\
&=-2\left[(x-a)f(x)\Big|_a^b-\int_a^bf(x)\mathrm{d}x\right]=2\int_a^bf(x)\mathrm{d}x,
\end{aligned}
$$

所以

$$
\int_a^bf(x)\mathrm{d}x=\frac12\int_a^bf''(x)(x-a)^2\mathrm{d}x.
$$

**【注】** 此题也可以有如下证明：

$$
\begin{aligned}
\int_a^bf(x)\mathrm{d}x&=\int_a^bf(x)\mathrm{d}(x-a)=(x-a)f(x)\Big|_a^b-\int_a^b(x-a)f'(x)\mathrm{d}x\\
&=-\int_a^b(x-a)f'(x)\mathrm{d}x=-\frac12\int_a^bf'(x)\mathrm{d}\left[(x-a)^2\right]\\
&=-\frac12\left[(x-a)^2f'(x)\Big|_a^b-\int_a^b(x-a)^2f''(x)\mathrm{d}x\right]\\
&=\frac12\int_a^b(x-a)^2f''(x)\mathrm{d}x.
\end{aligned}
$$

这里将 $\displaystyle\int_a^bf(x)\mathrm{d}x$ 写成 $\displaystyle\int_a^bf(x)\mathrm{d}(x-a)$ 的技巧值得注意。又如下例：

设 $f(x)$ 在 $[0,1]$ 上有连续导数，且 $f(0)=f(1)=0$，证明：$\left|\displaystyle\int_0^1f(x)\mathrm{d}x\right|\leqslant\dfrac{M}{4}$，$M=\max\limits_{0\leqslant x\leqslant1}\{|f'(x)|\}$。

证：

$$
\begin{aligned}
\int_0^1f(x)\mathrm{d}x&=\int_0^1f(x)\mathrm{d}\left(x-\frac12\right)\\
&=f(x)\left(x-\frac12\right)\Big|_0^1-\int_0^1\left(x-\frac12\right)f'(x)\mathrm{d}x\\
&=0-\int_0^1\left(x-\frac12\right)f'(x)\mathrm{d}x,
\end{aligned}
$$

故

$$
\begin{aligned}
\left|\int_0^1f(x)\mathrm{d}x\right|&=\left|\int_0^1\left(x-\frac12\right)f'(x)\mathrm{d}x\right|\leqslant\int_0^1\left|x-\frac12\right||f'(x)|\mathrm{d}x\\
&\leqslant\int_0^1\left|x-\frac12\right|\cdot M\mathrm{d}x=M\int_0^1\left|x-\frac12\right|\mathrm{d}x\\
&=M\left[\int_0^{\frac12}\left(\frac12-x\right)\mathrm{d}x+\int_{\frac12}^1\left(x-\frac12\right)\mathrm{d}x\right]=\frac{M}{4}.
\end{aligned}
$$

+++

#### 综合解答 (22) 设 $f(x)$ 在 $[a,b]$ 上二阶可导，且 $f''(x)>0$，证明：

$$
f\left(\frac{a+b}{2}\right)<\frac{1}{b-a}\int_a^b f(x)\mathrm{d}x<\frac{f(a)+f(b)}{2}.
$$

***

**证** 由已知，$y=f(x)$ 的图形如图 3-11 所示。

在点 $\left(\dfrac{a+b}{2},f\left(\dfrac{a+b}{2}\right)\right)$ 处切线方程为

$$
y=f\left(\frac{a+b}{2}\right)+f'\left(\frac{a+b}{2}\right)\left(x-\frac{a+b}{2}\right),
$$

曲线的切线在曲线的下方，故

$$
f(x)\geqslant f\left(\frac{a+b}{2}\right)+f'\left(\frac{a+b}{2}\right)\left(x-\frac{a+b}{2}\right),
$$

对上式两端分别积分，得

$$
\begin{aligned}
\int_a^b f(x)\mathrm{d}x&>f\left(\frac{a+b}{2}\right)(b-a)+f'\left(\frac{a+b}{2}\right)\cdot\int_a^b\left(x-\frac{a+b}{2}\right)\mathrm{d}x\\
&=f\left(\frac{a+b}{2}\right)(b-a)+0,
\end{aligned}
$$

即 $f\left(\dfrac{a+b}{2}\right)<\dfrac{1}{b-a}\displaystyle\int_a^b f(x)\mathrm{d}x$。

又 $AB$ 直线段在曲线 $y=f(x)$ 上方，故 $f(x)\leqslant f(a)+\dfrac{f(b)-f(a)}{b-a}\cdot(x-a)$，对上式两端分别积分，得

$$
\begin{aligned}
\int_a^b f(x)\mathrm{d}x&<f(a)(b-a)+\frac{f(b)-f(a)}{b-a}\int_a^b(x-a)\mathrm{d}x\\
&=\frac{f(a)+f(b)}{2}\cdot(b-a),
\end{aligned}
$$

即 $\dfrac{1}{b-a}\displaystyle\int_a^b f(x)\mathrm{d}x<\dfrac{f(a)+f(b)}{2}$。

综上所述，所证不等式成立。

+++

#### 综合解答 (23) 设 $f(x)$ 在 $[a,b](a<b)$ 上连续，且 $\int_a^b f(x)\mathrm{d}x=\int_a^b xf(x)\mathrm{d}x=0$。证明：至少存在不同的 $\xi_1,\xi_2\in(a,b)$，使得 $f(\xi_1)=f(\xi_2)=0$。

***

**证** 令 $F(x)=\displaystyle\int_a^x f(t)\mathrm{d}t$，则 $F(a)=0,F(b)=0$。又

$$
\int_a^b xf(x)\mathrm{d}x=\int_a^b x\,\mathrm{d}[F(x)]=xF(x)\Big|_a^b-\int_a^b F(x)\mathrm{d}x=-\int_a^b F(x)\mathrm{d}x=0,
$$

由推广的积分中值定理，得 $-\displaystyle\int_a^b F(x)\mathrm{d}x=-F(\xi)(b-a)=0\ (a<\xi<b)$，故 $F(\xi)=0$。

$F(x)$ 在 $[a,\xi],[\xi,b]$ 上应用罗尔定理，有

$$
F'(\xi_1)=0,\quad F'(\xi_2)=0\ (a<\xi_1<\xi,\ \xi<\xi_2<b),
$$

即 $f(\xi_1)=0,f(\xi_2)=0$。

【注】 此题也可采用反证法。

由已知条件存在 $\xi_1\in(a,b)$，使得 $f(\xi_1)=0$，否则对 $\forall x\in(a,b)$，$f(x)\neq0$，则 $f(x)$ 在 $[a,b]$ 上恒正或恒负，与 $\displaystyle\int_a^b f(x)\mathrm{d}x=0$ 矛盾。

又存在 $\xi_2\in(a,b)$，$\xi_2\neq\xi_1$，使得 $f(\xi_2)=0$，否则 $(x-\xi_1)f(x)$ 在 $[a,\xi_1]$ 和 $[\xi_1,b]$ 上恒正或恒负，则 $\displaystyle\int_a^b(x-\xi_1)f(x)\mathrm{d}x\neq0$ 与 $\displaystyle\int_a^b xf(x)\mathrm{d}x-\xi_1\int_a^b f(x)\mathrm{d}x=0$ 矛盾，故存在不同的 $\xi_1,\xi_2\in(a,b)$，使得 $f(\xi_1)=f(\xi_2)=0$。

+++

#### 综合解答 (24) 设 $f(x)$ 在 $(-a,a)(a>0)$ 内连续，且 $f'(0)=A\neq0$。

（Ⅰ）证明：对 $x\in(0,a)$，存在 $\theta\in(0,1)$，使得

$$
\int_0^x f(t)\mathrm{d}t+\int_0^{-x}f(t)\mathrm{d}t=x[f(\theta x)-f(-\theta x)];
$$

（Ⅱ）证明：$\lim\limits_{x\to0^+}\theta=\dfrac12$。

***

**证** （Ⅰ）令 $F(x)=\displaystyle\int_0^x f(t)\mathrm{d}t+\int_0^{-x}f(t)\mathrm{d}t$，则 $F(x)$ 在 $[0,x]$ 上可导，应用拉格朗日中值定理，并注意到 $F(0)=0$，存在 $\theta\in(0,1)$，使得 $F(x)-F(0)=F'(0+\theta x)x$，即

$$
\int_0^x f(t)\mathrm{d}t+\int_0^{-x}f(t)\mathrm{d}t=x[f(\theta x)-f(-\theta x)].
$$

（Ⅱ）将（Ⅰ）中式子变形为 $\dfrac{\displaystyle\int_0^x f(t)\mathrm{d}t+\int_0^{-x}f(t)\mathrm{d}t}{x^2}=\dfrac{f(\theta x)-f(-\theta x)}{x}$，

两端分别取极限，有 $\lim\limits_{x\to0^+}\dfrac{\displaystyle\int_0^x f(t)\mathrm{d}t+\int_0^{-x}f(t)\mathrm{d}t}{x^2}=\lim\limits_{x\to0^+}\dfrac{f(\theta x)-f(-\theta x)}{x}$，则

$$
\begin{aligned}
\text{左边}&=\lim_{x\to0^+}\frac{f(x)-f(-x)}{2x}\\
&=\frac12\lim_{x\to0^+}\left[\frac{f(x)-f(0)}{x}+\frac{f(-x)-f(0)}{-x}\right]=f'(0)=A,\\
\text{右边}&=\lim_{x\to0^+}\theta\left[\frac{f(\theta x)-f(0)}{\theta x}+\frac{f(-\theta x)-f(0)}{-\theta x}\right]\\
&=2\lim_{x\to0^+}\theta f'(0)=2A\lim_{x\to0^+}\theta,
\end{aligned}
$$

故 $A=2A\lim\limits_{x\to0^+}\theta$，由 $A\neq0$，可得 $\lim\limits_{x\to0^+}\theta=\dfrac12$。

+++

#### 综合解答 (25) 设 $y=f(x)$ 在 $[0,1]$ 上是非负连续函数。

（Ⅰ）证明：存在 $x_0\in(0,1)$，使得在 $[0,x_0]$ 上以 $f(x_0)$ 为高的矩形面积，等于在 $[x_0,1]$ 上以 $y=f(x)$ 为曲边的曲边梯形面积；

（Ⅱ）又设 $f(x)$ 在 $(0,1)$ 内可导，且 $f'(x)>-\dfrac{2f(x)}{x}$，证明：（Ⅰ）中的 $x_0$ 是唯一的。

***

**证** （Ⅰ）依题设，需证存在 $x_0\in(0,1)$，使得 $x_0f(x_0)=\displaystyle\int_{x_0}^1 f(t)\mathrm{d}t$。

注意到

$$
\left[x\int_x^1 f(t)\mathrm{d}t\right]'=\int_x^1 f(t)\mathrm{d}t-xf(x),
$$

令辅助函数 $F(x)=x\displaystyle\int_x^1 f(t)\mathrm{d}t$，则 $F(0)=F(1)=0$。

由罗尔定理，存在一点 $x_0\in(0,1)$，使 $F'(x_0)=0$，即 $x_0f(x_0)=\displaystyle\int_{x_0}^1 f(t)\mathrm{d}t$。

（Ⅱ）令 $\varphi(x)=\displaystyle\int_x^1 f(t)\mathrm{d}t-xf(x)$，$x\in(0,1)$，则

$$
\varphi'(x)=-f(x)-f(x)-xf'(x)=-2f(x)-xf'(x).
$$

由已知条件 $f'(x)>-\dfrac{2f(x)}{x}$，知 $\varphi'(x)<0$，即 $\varphi(x)$ 在 $(0,1)$ 内严格单调减少，故（Ⅰ）中的 $x_0$ 是 $\varphi(x)$ 唯一零点。

+++

#### 综合解答 (26) 设曲线 $y=f(x)$ 上任一点 $(x,f(x))$ 处的切线斜率为 $a^2x^2-4ax+3$，且 $y=f(x)$ 在 $x=1$ 处取得极小值 $0$。

（Ⅰ）求 $f(x)$ 及 $f(x)$ 的其它极值；

（Ⅱ）证明：$0\leqslant\displaystyle\int_0^1\sqrt{f(ut)}\,\mathrm{d}t\leqslant\dfrac{2}{3u},u\in(0,1)$。

***

**解** （Ⅰ）由已知 $f'(1)=0$，即

$$
(a^2x^2-4ax+3)\Big|_{x=1}=a^2-4a+3=0,
$$

解得 $a=3,a=1$。又

$$
f''(x)=2a^2x-4a,\quad f''(1)=2a^2-4a,
$$

当 $a=3$ 时，$f''(1)=6>0$；当 $a=1$ 时，$f''(1)=-2<0$。

由已知 $f(1)=0$ 为极小值，故 $a=3$，所以 $f'(x)=9x^2-12x+3$，于是

$$
f(x)=f(1)+\int_1^x f'(t)\mathrm{d}t=0+\int_1^x(9t^2-12t+3)\mathrm{d}t=3x^3-6x^2+3x.
$$

令 $f'(x)=0$，得 $f(x)$ 的另一个驻点为 $x=\dfrac13$，且 $f''\left(\dfrac13\right)=-6<0$，所以 $f(x)$ 的极大值为 $f\left(\dfrac13\right)=\dfrac49$。

（Ⅱ）令 $ut=x$，$t=\dfrac1u x$，则

$$
\begin{aligned}
\int_0^1\sqrt{f(ut)}\,\mathrm{d}t&=\int_0^u\sqrt{f(x)}\cdot\frac1u\mathrm{d}x=\frac1u\int_0^u\sqrt{f(x)}\,\mathrm{d}x\\
&\leqslant\frac1u\int_0^1\sqrt{f(x)}\,\mathrm{d}x\leqslant\frac1u\int_0^1\sqrt{\frac49}\,\mathrm{d}x=\frac{2}{3u},\quad u\in(0,1),
\end{aligned}
$$

又显然有 $\displaystyle\int_0^1\sqrt{f(ut)}\,\mathrm{d}t\geqslant0$，故原不等式成立。

+++

#### 综合解答 (27) 设 $f(x)$ 在 $(-\infty,+\infty)$ 内连续，且满足 $f(x+T)=f(x),T>0,f(-x)=f(x)$。

（Ⅰ）证明：$\displaystyle\int_0^{nT}xf(x)\mathrm{d}x=\dfrac{n^2T}{2}\int_0^T f(x)\mathrm{d}x$（$n$ 为正整数）；

（Ⅱ）计算 $I=\displaystyle\int_0^{n\pi}x|\cos x|\mathrm{d}x$。

***

**解** （Ⅰ）利用换元法。令 $x=nT-t$，

$$
\int_0^{nT}xf(x)\mathrm{d}x=nT\int_0^{nT}f(t)\mathrm{d}t-\int_0^{nT}tf(t)\mathrm{d}t,
$$

移项得 $\displaystyle\int_0^{nT}xf(x)\mathrm{d}x=\frac{nT}{2}\int_0^{nT}f(x)\mathrm{d}x$。

又 $f(x+T)=f(x)$，故 $\displaystyle\int_0^{nT}f(x)\mathrm{d}x=n\int_0^T f(x)\mathrm{d}x$，所以 $\displaystyle\int_0^{nT}xf(x)\mathrm{d}x=\frac{n^2T}{2}\int_0^T f(x)\mathrm{d}x$。

（Ⅱ）$|\cos x|$ 是以 $\pi$ 为周期的偶函数，由（Ⅰ）知

$$
\begin{aligned}
I&=\int_0^{n\pi}x|\cos x|\mathrm{d}x=\frac{n^2\pi}{2}\int_0^\pi|\cos x|\mathrm{d}x\\
&=\frac{n^2\pi}{2}\left[\int_0^{\frac\pi2}\cos x\,\mathrm{d}x+\int_{\frac\pi2}^\pi(-\cos x)\mathrm{d}x\right]=n^2\pi.
\end{aligned}
$$

【注】 结论：设 $f(x+T)=f(x)$，则 $\displaystyle\int_0^{nT}f(x)\mathrm{d}x=n\int_0^T f(x)\mathrm{d}x$。（证明见《李林考研数学系列高等数学辅导讲义》）

+++

#### 综合解答 (28) 设 $f(x)$ 在 $(-\infty,+\infty)$ 内有连续导数，证明：

$$
\lim\limits_{a\to0^+}\frac{1}{4a^2}\int_{-a}^a[f(t+a)-f(t-a)]\mathrm{d}t=f'(0).
$$

***

**证** 由积分中值定理，有

$$
\lim_{a\to0^+}\frac{1}{4a^2}\int_{-a}^a[f(t+a)-f(t-a)]\mathrm{d}t=\lim_{a\to0^+}\frac{1}{2a}[f(\xi+a)-f(\xi-a)],\quad-a\leqslant\xi\leqslant a.
$$

$f(x)$ 在 $[\xi-a,\xi+a]$ 上使用拉格朗日中值定理，

$$
f(\xi+a)-f(\xi-a)=2af'(\eta),\quad\xi-a<\eta<\xi+a.
$$

而 $f'(x)$ 在 $(-\infty,+\infty)$ 内连续，故

$$
\text{原式}=\lim_{a\to0^+}f'(\eta)=\lim_{a\to0^+}f'(\xi)=f'(0).
$$

【注】 此题也可利用积分换元法及洛必达法则证明，证明如下：令 $t+a=u$，$\displaystyle\int_{-a}^a f(t+a)\mathrm{d}t=\int_0^{2a}f(u)\mathrm{d}u$；令 $t-a=u$，$\displaystyle\int_{-a}^a f(t-a)\mathrm{d}t=\int_0^{-2a}f(u)\mathrm{d}u$，故

$$
\begin{aligned}
\text{原式}&=\lim_{a\to0^+}\frac{\displaystyle\int_0^{2a}f(u)\mathrm{d}u+\int_0^{-2a}f(u)\mathrm{d}u}{4a^2}=\lim_{a\to0^+}\frac{2f(2a)-2f(-2a)}{8a}\\
&=\lim_{a\to0^+}\frac{2f'(2a)+2f'(-2a)}{4}=f'(0).
\end{aligned}
$$

+++

#### 综合解答 (29) 设曲线 $y=a\sqrt{x}(a>0)$ 与 $y=\ln\sqrt{x}$ 在点 $(x_0,y_0)$ 处有公切线。

（Ⅰ）求常数 $a$ 及点 $(x_0,y_0)$；

（Ⅱ）求两曲线与 $x$ 轴所围图形绕 $x$ 轴旋转一周所得旋转体的体积。

***

**解** （Ⅰ）$y=a\sqrt{x}$，$y=\ln\sqrt{x}$ 的导数分别为

$$
y'=\frac{a}{2\sqrt{x}},\quad y'=\frac{1}{\sqrt{x}}\cdot\frac{1}{2\sqrt{x}}=\frac{1}{2x}.
$$

如图 3-12 所示，由于两曲线在 $(x_0,y_0)$ 处有公切线，则

$$
\begin{cases}a\sqrt{x_0}=\ln\sqrt{x_0},\\[2mm]\dfrac{a}{2\sqrt{x_0}}=\dfrac{1}{2x_0},\end{cases}
$$

解得 $x_0=\mathrm{e}^2$，$a=\mathrm{e}^{-1}$，切点为 $(\mathrm{e}^2,1)$。

（Ⅱ）

$$
\begin{aligned}
V&=\int_0^{\mathrm{e}^2}\pi\left(\frac{\sqrt{x}}{\mathrm{e}}\right)^2\mathrm{d}x-\int_1^{\mathrm{e}^2}\pi(\ln\sqrt{x})^2\mathrm{d}x=\frac{\pi}{\mathrm{e}^2}\int_0^{\mathrm{e}^2}x\,\mathrm{d}x-\frac{\pi}{4}\int_1^{\mathrm{e}^2}(\ln x)^2\mathrm{d}x\\
&=\frac{\pi}{2}\mathrm{e}^2-\frac{\pi}{4}\left[x(\ln x)^2-2x\ln x+2x\right]\Big|_1^{\mathrm{e}^2}=\frac{\pi}{2}\mathrm{e}^2-\frac{\pi}{2}(\mathrm{e}^2-1)=\frac{\pi}{2}.
\end{aligned}
$$

+++

#### 综合解答 (30) 设 $f(x)$ 在 $[a,b]$ 上可导，$f(a)>0,f'(x)>0$，$S_1(x)$ 与 $S_2(x)$ 为如图 3-1 所示阴影部分的面积，证明：存在唯一的 $\xi$，使得 $\dfrac{S_1(\xi)}{S_2(\xi)}=k$（$k$ 为正的常数）。

***

**证** 如图 3-13 所示，依题设，需证明存在唯一的 $\xi$，使得 $S_1(\xi)-kS_2(\xi)=0$。

设 $F(x)=S_1(x)-kS_2(x)$，即证明存在唯一的 $\xi$，使 $F(\xi)=0$。又

$$
S_1(x)=(x-a)f(x)-\int_a^x f(t)\mathrm{d}t,\quad S_2(x)=\int_x^b f(t)\mathrm{d}t-(b-x)f(x),
$$

则 $S_1(a)=0,S_2(b)=0$。于是

$$
\begin{aligned}
F(a)&=-kS_2(a)=-k\left[\int_a^b f(t)\mathrm{d}t-(b-a)f(a)\right]=-k\int_a^b[f(t)-f(a)]\mathrm{d}t,\\
F(b)&=f(b)(b-a)-\int_a^b f(t)\mathrm{d}t=\int_a^b[f(b)-f(t)]\mathrm{d}t.
\end{aligned}
$$

又 $f'(x)>0$，可知 $f(a)<f(x)<f(b)$。又由 $k>0$，可知 $F(a)<0,F(b)>0$。由连续函数的零点定理，存在 $\xi\in(a,b)$，使得 $F(\xi)=0$，即 $\dfrac{S_1(\xi)}{S_2(\xi)}=k$。

再证 $\xi$ 的唯一性，由

$$
\begin{aligned}
F'(x)&=S_1'(x)-kS_2'(x)\\
&=f'(x)(x-a)+f(x)-f(x)-k[-f(x)-f'(x)(b-x)+f(x)]\\
&=f'(x)(x-a)+kf'(x)(b-x)>0,
\end{aligned}
$$

可知 $F(x)$ 在 $(a,b)$ 内严格单调增加，故 $\xi$ 是唯一的。

+++

#### 综合解答 (31) 求曲线 $4y=\displaystyle\int_0^2 x\sqrt{12-x^2u^2}\,\mathrm{d}u(x\geqslant0)$ 的全长。

***

**解** 令 $xu=t$，

$$
\int_0^2 x\sqrt{12-x^2u^2}\,\mathrm{d}u=\int_0^{2x}\sqrt{12-t^2}\,\mathrm{d}t,
$$

故 $4y=\displaystyle\int_0^{2x}\sqrt{12-t^2}\,\mathrm{d}t$。两边同时对 $x$ 求导，得

$$
y'=\frac14\sqrt{12-4x^2}\cdot2=\sqrt{3-x^2}.
$$

曲线的全长为

$$
\begin{aligned}
s&=\int_0^{\sqrt3}\sqrt{1+y'^2}\,\mathrm{d}x=\int_0^{\sqrt3}\sqrt{4-x^2}\,\mathrm{d}x\\
&\xlongequal{x=2\sin t}\int_0^{\frac\pi3}\sqrt{4-4\sin^2t}\cdot2\cos t\,\mathrm{d}t\\
&=4\int_0^{\frac\pi3}\cos^2t\,\mathrm{d}t=2\left(t+\frac12\sin2t\right)\Big|_0^{\frac\pi3}\\
&=2\times\left(\frac\pi3+\frac12\times\frac{\sqrt3}{2}\right)=\frac{2\pi}{3}+\frac{\sqrt3}{2}.
\end{aligned}
$$

+++

#### 综合解答 (32) 设平面图形 $D$ 由 $x^2+y^2\leqslant2x$ 与 $y\geqslant x$ 确定，求图形 $D$ 绕直线 $x=2$ 旋转一周所得旋转体的体积。

***

**解** 如图 3-14 所示，$D$ 的边界方程分别为

$$
x=1-\sqrt{1-y^2},\quad x=y\ (0\leqslant y\leqslant1).
$$

任取 $[y,y+\mathrm{d}y]\subset[0,1]$，则

$$
\begin{aligned}
\mathrm{d}V&=\left\{\pi\left[2-\left(1-\sqrt{1-y^2}\right)\right]^2-\pi(2-y)^2\right\}\mathrm{d}y\\
&=2\pi\left[\sqrt{1-y^2}-(1-y)^2\right]\mathrm{d}y,
\end{aligned}
$$

故

$$
\begin{aligned}
V&=\int_0^1 2\pi\left[\sqrt{1-y^2}-(1-y)^2\right]\mathrm{d}y\\
&=2\pi\left[\frac{y}{2}\sqrt{1-y^2}+\frac12\arcsin y+\frac13(1-y)^3\right]\Big|_0^1=2\pi\left(\frac\pi4-\frac13\right).
\end{aligned}
$$

【注】 此题也可以用如下计算：

$$
V=2\pi\int_0^1\sqrt{1-y^2}\,\mathrm{d}y+2\pi\int_0^1(1-y)^2\mathrm{d}(1-y)=2\pi\left(\frac\pi4-\frac13\right).
$$

+++

#### 综合解答 (33) 求曲线 $y=\mathrm{e}^{-x}\sqrt{\sin x}\,(x\geqslant0)$ 绕 $x$ 轴旋转所得旋转体的体积。

***

**解** 先求 $f(x)=\mathrm{e}^{-x}\sqrt{\sin x}\,(x\geqslant0)$ 的定义域。

由 $\sin x\geqslant0$，知 $x\in[2k\pi,(2k+1)\pi]\ (k=0,1,2,\cdots)$，如图 3-15 所示。

则所求体积为

$$
\begin{aligned}
V&=\sum_{k=0}^\infty\pi\int_{2k\pi}^{(2k+1)\pi}\mathrm{e}^{-2x}\sin x\,\mathrm{d}x\xlongequal{x=t+2k\pi}\sum_{k=0}^\infty\pi\int_0^\pi\mathrm{e}^{-2(2k\pi+t)}\sin t\,\mathrm{d}t\\
&=\sum_{k=0}^\infty\pi\mathrm{e}^{-4k\pi}\int_0^\pi\mathrm{e}^{-2t}\sin t\,\mathrm{d}t=\frac{\pi(1+\mathrm{e}^{-2\pi})}{5}\cdot\sum_{k=0}^\infty\mathrm{e}^{-4k\pi}\quad(\text{等比级数求和})\\
&=\frac{\pi(1+\mathrm{e}^{-2\pi})}{5}\cdot\frac{1}{1-\mathrm{e}^{-4\pi}}=\frac{\pi}{5(1-\mathrm{e}^{-2\pi})}.
\end{aligned}
$$

+++

#### 综合解答 (34) 设摆线 $\begin{cases}x=a(t-\sin t),\\ y=a(1-\cos t)\end{cases}(0\leqslant t\leqslant2\pi,a>0)$ 与 $x$ 轴所围平面图形为 $D$。

（Ⅰ）求 $D$ 绕 $x$ 轴，$y$ 轴各旋转一周所得旋转体的体积；

（Ⅱ）求 $D$ 绕直线 $y=2a$ 旋转一周所得旋转体的体积。

***

**解** （Ⅰ）如图 3-16 所示，

$$
\begin{aligned}
V_x&=\pi\int_0^{2\pi a}y^2\mathrm{d}x=\pi\int_0^{2\pi}a^2(1-\cos t)^2\cdot a(1-\cos t)\mathrm{d}t\\
&=\pi a^3\int_0^{2\pi}(1-\cos t)^3\mathrm{d}t=8\pi a^3\int_0^{2\pi}\sin^6\frac{t}{2}\mathrm{d}t\\
&=32\pi a^3\int_0^{\frac\pi2}\sin^6u\,\mathrm{d}u=5\pi^2a^3,\\
V_y&=2\pi\int_0^{2\pi a}xy\,\mathrm{d}x=2\pi\int_0^{2\pi}a^3(t-\sin t)(1-\cos t)^2\mathrm{d}t\\
&=2\pi a^3\int_0^{2\pi}(t-2t\cos t+t\cos^2t-\sin t+2\sin t\cos t-\sin t\cos^2t)\mathrm{d}t=6\pi^3a^3.
\end{aligned}
$$

（Ⅱ）

$$
\begin{aligned}
V_{y=2a}&=\pi(2a)^2\cdot2\pi a-\int_0^{2\pi a}\pi(2a-y)^2\mathrm{d}x\\
&=8\pi^2a^3-\pi\int_0^{2\pi}[2a-a(1-\cos t)]^2\cdot a(1-\cos t)\mathrm{d}t\\
&=8\pi^2a^3-\pi a^3\int_0^{2\pi}(1+\cos t)^2(1-\cos t)\mathrm{d}t\\
&=8\pi^2a^3-\pi a^3\int_0^{2\pi}\sin^2t(1+\cos t)\mathrm{d}t\\
&=8\pi^2a^3-\pi^2a^3=7\pi^2a^3.
\end{aligned}
$$

+++

#### 综合解答 (35) 设 $f(x)=x^n\sqrt{1-x^2},x\in[0,1]$ 与 $y=0$ 所围平面区域的面积为 $S_n$，$g(x)=\sin^{\frac n2}x,x\in\left[0,\dfrac\pi2\right]$ 与 $y=0$ 所围平面区域绕 $x$ 轴旋转一周所得体积为 $V_n(n=1,2,\cdots)$，求极限 $\lim\limits_{n\to\infty}\dfrac{\pi S_n}{V_n}$。

***

**解** 由已知，$V_n=\pi\displaystyle\int_0^{\frac\pi2}\left(\sin^{\frac n2}x\right)^2\mathrm{d}x=\pi\int_0^{\frac\pi2}\sin^nx\,\mathrm{d}x$，

$$
\pi S_n=\pi\int_0^1 x^n\sqrt{1-x^2}\,\mathrm{d}x\xlongequal{x=\sin t}\pi\int_0^{\frac\pi2}\sin^nt\cdot\cos^2t\,\mathrm{d}t=\pi\int_0^{\frac\pi2}\sin^nt\,\mathrm{d}t-\pi\int_0^{\frac\pi2}\sin^{n+2}t\,\mathrm{d}t=V_n-V_{n+2}.
$$

而

$$
\begin{aligned}
V_{n+2}&=\pi\int_0^{\frac\pi2}\sin^{n+2}t\,\mathrm{d}t=-\pi\int_0^{\frac\pi2}\sin^{n+1}t\,\mathrm{d}(\cos t)\\
&=-\pi\left[\cos t\cdot\sin^{n+1}t\Big|_0^{\frac\pi2}-\int_0^{\frac\pi2}\cos t\cdot(n+1)\sin^nt\cdot\cos t\,\mathrm{d}t\right]\\
&=\pi(n+1)\int_0^{\frac\pi2}\sin^nt\cdot(1-\sin^2t)\mathrm{d}t=(n+1)V_n-(n+1)V_{n+2},
\end{aligned}
$$

整理得 $V_{n+2}=\dfrac{n+1}{n+2}V_n$，所以 $\pi S_n=V_n-V_{n+2}=V_n-\dfrac{n+1}{n+2}V_n=\dfrac{1}{n+2}V_n$，故

$$
\lim_{n\to\infty}\frac{\pi S_n}{V_n}=\lim_{n\to\infty}\frac{1}{n+2}=0.
$$

+++

#### 综合解答 (36) 将半径为 $R$ 的球沉入水中，它与水面相切，设球的密度与水的密度相等，现将球从水中取出，问至少需要做功多少？

***

**解** 建立如图 3-17 所示的坐标系，圆的方程为

$$
x^2+(y-R)^2=R^2.
$$

用微元法。任取 $[y,y+\mathrm{d}y]\subset[0,2R]$，将球从水中取出恰好离开水面时，薄片 $[y,y+\mathrm{d}y]$ 行程为 $2R$，其中在水中移动的距离为 $y$，由于球与水的密度相等，所以重力与浮力的合力为零，故球在水中移动所做功为零；在水面以上移动的距离为 $2R-y$，故克服重力做功的微元为

$$
\mathrm{d}W=\rho g(2R-y)\pi x^2\mathrm{d}y=\rho g\pi(2R-y)\left[R^2-(y-R)^2\right]\mathrm{d}y,
$$

则

$$
W=\int_0^{2R}\mathrm{d}W=\rho g\int_0^{2R}\pi(2R-y)\left[R^2-(y-R)^2\right]\mathrm{d}y=\frac43\pi\rho gR^4.
$$

+++

#### 综合解答 (37) 设如图 3-2(a)，3-2(b) 所示为同一等腰三角形薄板，已知其底为 $2b$、高为 $h$，将其垂直放入静水中，图(a) 是其底与水面相齐，图(b) 是其顶点与水面相齐，设图(a) 与图(b) 薄板一侧所受压力分别为 $P_1$ 和 $P_2$，求 $\dfrac{P_2}{P_1}$。

***

**解** 如图 3-18(a) 中直线 $AC$ 的方程为 $y=\dfrac{b(h-x)}{h}$。用微元法，任取 $[x,x+\mathrm{d}x]\subset[0,h]$，则 $\mathrm{d}P_1=2\rho gxy\,\mathrm{d}x=\dfrac{2\rho gb}{h}(h-x)x\,\mathrm{d}x$，故

$$
P_1=\int_0^h\mathrm{d}P_1=\int_0^h\frac{2\rho gb}{h}(h-x)x\,\mathrm{d}x=\frac13\rho gbh^2.
$$

如图 3-18(b) 中直线 $OA$ 方程为 $y=\dfrac{bx}{h}$，则 $\mathrm{d}P_2=2\rho gxy\,\mathrm{d}x=\dfrac{2\rho gb}{h}x^2\mathrm{d}x$，故

$$
P_2=\int_0^h\mathrm{d}P_2=\int_0^h\rho g\frac{2b}{h}x^2\mathrm{d}x=\frac23\rho gbh^2.
$$

所以 $\dfrac{P_2}{P_1}=2$，即 $P_2=2P_1$。

+++

#### 综合解答 (38) 求曲线 $y=3-|x^2-1|$ 与 $x$ 轴围成封闭图形绕直线 $y=3$ 旋转所得旋转体的体积。

***

**解** 曲线的图形如图 3-19 所示。

由已知及对称性，只需考虑 $x\in[0,2]$ 的情况，

$$
y=3-|x^2-1|=\begin{cases}x^2+2,&0\leqslant x\leqslant1,\\4-x^2,&1<x\leqslant2.\end{cases}
$$

用微元法。任取 $[x,x+\mathrm{d}x]\subset[0,1]$，$[0,1]$ 上体积记为 $V_1$，$[1,2]$ 上体积记为 $V_2$，则 $\mathrm{d}V_1=\pi\left\{3^2-\left[3-(x^2+2)\right]^2\right\}\mathrm{d}x$。

同理 $\mathrm{d}V_2=\pi\left\{3^2-\left[3-(4-x^2)\right]^2\right\}\mathrm{d}x$，故

$$
V=2(V_1+V_2)=2\pi\int_0^1(8+2x^2-x^4)\mathrm{d}x+2\pi\int_1^2(8+2x^2-x^4)\mathrm{d}x=\frac{448\pi}{15}.
$$

+++

#### 综合解答 (39) 设心形线 $r=4(1+\cos\theta)$ 与 $\theta=0,\theta=\dfrac\pi2$ 所围图形为 $D$，求 $D$ 绕极轴旋转一周所得旋转体的体积。

***

**解** 心形线 $r=4(1+\cos\theta)$ 的参数方程为

$$
\begin{cases}x=4(1+\cos\theta)\cos\theta,\\ y=4(1+\cos\theta)\sin\theta.\end{cases}
$$

心形线的图形如图 3-20 所示，则

$$
\begin{aligned}
V&=\int_0^8\pi y^2\mathrm{d}x=\int_{\frac\pi2}^0\pi\cdot16(1+\cos\theta)^2\sin^2\theta\cdot4(-\sin\theta-2\sin\theta\cos\theta)\mathrm{d}\theta\\
&=64\pi\int_0^{\frac\pi2}(1+\cos\theta)^2\sin^3\theta(1+2\cos\theta)\mathrm{d}\theta=160\pi.
\end{aligned}
$$

【注】 极坐标下计算旋转体体积：先将极坐标方程化为参数方程，再用直角坐标下公式计算。

+++

#### 综合解答 (40) 设 $D$ 位于曲线 $y=\dfrac{1}{x(\ln x)^{\alpha+1}}(\alpha>0,2\leqslant x<+\infty)$ 下方，$x$ 轴上方的无界区域。

（Ⅰ）求 $D$ 的面积 $S(\alpha)$；

（Ⅱ）求 $S(\alpha)$ 的最小值。

***

**解** （Ⅰ）依题设，

$$
S(\alpha)=\int_2^{+\infty}\frac{\mathrm{d}x}{x(\ln x)^{\alpha+1}}=\int_2^{+\infty}(\ln x)^{-\alpha-1}\mathrm{d}(\ln x)=-\frac1\alpha(\ln x)^{-\alpha}\Big|_2^{+\infty}=\frac{1}{\alpha(\ln2)^\alpha}.
$$

（Ⅱ）令 $f(\alpha)=\alpha(\ln2)^\alpha$，则由

$$
f'(\alpha)=(\ln2)^\alpha+\alpha\cdot(\ln2)^\alpha\cdot\ln(\ln2)=(\ln2)^\alpha[1+\alpha\ln(\ln2)]=0,
$$

得 $\alpha_0=-\dfrac{1}{\ln(\ln2)}$ 是唯一驻点。

当 $\alpha<-\dfrac{1}{\ln(\ln2)}$ 时，$f'(\alpha)>0$；当 $\alpha>-\dfrac{1}{\ln(\ln2)}$ 时，$f'(\alpha)<0$，故

$$
f(\alpha_0)=-\frac{1}{\ln(\ln2)}(\ln2)^{-\frac{1}{\ln(\ln2)}}=-\frac{1}{\ln(\ln2)}\cdot\frac{1}{(\ln2)^{\frac{1}{\ln(\ln2)}}}
$$

为最大值，所以 $S(\alpha)$ 的最小值为 $\dfrac{1}{f(\alpha_0)}=-\ln(\ln2)\cdot(\ln2)^{\frac{1}{\ln(\ln2)}}$。

+++

#### 综合解答 (41) 设 $f(x)$ 在 $[0,+\infty)$ 上连续且单调减少，$f(x)\geqslant0$，$a_n=\displaystyle\sum_{k=1}^n f(k)-\int_1^n f(x)\mathrm{d}x\ (n=1,2,\cdots)$，证明：$\lim\limits_{n\to\infty}a_n$ 存在。

***

**证**

$$
a_n=\sum_{k=1}^n f(k)-\sum_{k=1}^{n-1}\int_k^{k+1}f(x)\mathrm{d}x=\sum_{k=1}^n\left[f(k)-\int_k^{k+1}f(x)\mathrm{d}x\right]+\int_n^{n+1}f(x)\mathrm{d}x.\qquad ①
$$

由于 $f(x)$ 单调减少，所以

$$
f(k+1)=\int_k^{k+1}f(k+1)\mathrm{d}x\leqslant\int_k^{k+1}f(x)\mathrm{d}x\leqslant\int_k^{k+1}f(k)\mathrm{d}x=f(k),
$$

故

$$
\begin{aligned}
a_{n+1}-a_n&=\sum_{k=1}^{n+1}f(k)-\sum_{k=1}^n f(k)-\int_1^{n+1}f(x)\mathrm{d}x+\int_1^n f(x)\mathrm{d}x\\
&=f(n+1)-\int_n^{n+1}f(x)\mathrm{d}x\leqslant0,
\end{aligned}
$$

所以 $\{a_n\}$ 单调减少。又由 ① 式，知

$$
f(k)-\int_k^{k+1}f(x)\mathrm{d}x\geqslant0,\quad\int_n^{n+1}f(x)\mathrm{d}x\geqslant0,
$$

故 $\{a_n\}$ 有下界 $0$。再由单调有界准则，知 $\lim\limits_{n\to\infty}a_n$ 存在。

+++

#### 综合解答 (42) 设 $a_n=\displaystyle\int_0^1 x^n\sqrt{1-x^2}\,\mathrm{d}x$，$b_n=\displaystyle\int_0^{\frac\pi2}\sin^nx\cos^nx\,\mathrm{d}x$，求 $\lim\limits_{n\to\infty}\dfrac{b_n}{a_n}$。

***

**解**

$$
\begin{aligned}
b_n&=\int_0^{\frac\pi2}\sin^nx\cos^nx\,\mathrm{d}x=2^{-n-1}\int_0^{\frac\pi2}\sin^n2x\,\mathrm{d}(2x)=2^{-n-1}\int_0^\pi\sin^nx\,\mathrm{d}x\\
&=2^{-n-1}\cdot2\int_0^{\frac\pi2}\sin^nx\,\mathrm{d}x=2^{-n}\int_0^{\frac\pi2}\sin^nx\,\mathrm{d}x.
\end{aligned}
$$

记 $c_n=\displaystyle\int_0^{\frac\pi2}\sin^nx\,\mathrm{d}x$，则 $b_n=2^{-n}c_n$，

$$
a_n=\int_0^1 x^n\sqrt{1-x^2}\,\mathrm{d}x\xlongequal{x=\sin t}\int_0^{\frac\pi2}\sin^nt\cdot\cos^2t\,\mathrm{d}t=\int_0^{\frac\pi2}\sin^nt(1-\sin^2t)\mathrm{d}t=\int_0^{\frac\pi2}\sin^nt\,\mathrm{d}t-\int_0^{\frac\pi2}\sin^{n+2}t\,\mathrm{d}t=c_n-c_{n+2}.
$$

又

$$
\begin{aligned}
c_{n+2}&=\int_0^{\frac\pi2}\sin^{n+2}t\,\mathrm{d}t=-\int_0^{\frac\pi2}\sin^{n+1}t\,\mathrm{d}(\cos t)\\
&=-\left[\cos t\cdot\sin^{n+1}t\Big|_0^{\frac\pi2}-\int_0^{\frac\pi2}\cos t\cdot(n+1)\sin^nt\cdot\cos t\,\mathrm{d}t\right]\\
&=(n+1)\int_0^{\frac\pi2}\sin^nt(1-\sin^2t)\mathrm{d}t=(n+1)c_n-(n+1)c_{n+2},
\end{aligned}
$$

移项，得 $c_{n+2}=\dfrac{n+1}{n+2}c_n$，故 $a_n=c_n-c_{n+2}=\dfrac{1}{n+2}c_n=\dfrac{1}{n+2}\cdot2^nb_n$，所以

$$
\lim_{n\to\infty}\frac{b_n}{a_n}=\lim_{n\to\infty}\frac{n+2}{2^n}=0.
$$

+++

#### 拓展解答 (1) 已知曲线 $L$ 的极坐标方程为 $r=1+\cos\theta\ \left(0\leqslant\theta\leqslant\dfrac{\pi}{2}\right)$。

（Ⅰ）求曲线 $L$ 在 $\theta=\dfrac{\pi}{4}$ 对应点处的切线 $T$ 的直角坐标方程；
（Ⅱ）求曲线 $L$、切线 $T$ 与 $x$ 轴所围图形的面积。

***

**解**　（Ⅰ）曲线 $L$ 的参数方程为

$$
\begin{cases}x=r\cos\theta=(1+\cos\theta)\cos\theta,\\ y=r\sin\theta=(1+\cos\theta)\sin\theta,\end{cases}
$$

则

$$
\dfrac{\mathrm{d}y}{\mathrm{d}x}=\dfrac{y'(\theta)}{x'(\theta)}=\dfrac{\cos\theta+\cos2\theta}{-\sin\theta-\sin2\theta},\quad \dfrac{\mathrm{d}y}{\mathrm{d}x}\bigg|_{\theta=\frac{\pi}{4}}=1-\sqrt{2}.
$$

当 $\theta=\dfrac{\pi}{4}$ 时，有 $x=\dfrac12(1+\sqrt2)$，$y=\dfrac12(1+\sqrt2)$，故切线 $T$ 的方程为

$$
y-\dfrac12(1+\sqrt2)=(1-\sqrt2)\left[x-\dfrac12(1+\sqrt2)\right],
$$

即 $y=(1-\sqrt2)x+1+\dfrac{\sqrt2}{2}$。

（Ⅱ）所围图形为如图 3-21 所示的阴影部分。曲边三角形 $AOP$ 的面积为

$$
\begin{aligned}
A_1&=\dfrac12\int_0^{\frac{\pi}{4}}r^2(\theta)\,\mathrm{d}\theta=\dfrac12\int_0^{\frac{\pi}{4}}(1+\cos\theta)^2\,\mathrm{d}\theta\\
&=\dfrac12\int_0^{\frac{\pi}{4}}\left(\dfrac32+2\cos\theta+\dfrac12\cos2\theta\right)\mathrm{d}\theta\\
&=\dfrac12\left(\dfrac32\theta+2\sin\theta+\dfrac14\sin2\theta\right)\bigg|_0^{\frac{\pi}{4}}\\
&=\dfrac{3}{16}\pi+\dfrac18+\dfrac{\sqrt2}{2}.
\end{aligned}
$$

由（Ⅰ）知，切线的方程为 $y=(1-\sqrt2)x+1+\dfrac{\sqrt2}{2}$，令 $y=0$，得 $x$ 轴上截距为 $x=2+\dfrac32\sqrt2$，故所求面积为

$$
S=\dfrac12\times\left(2+\dfrac32\sqrt2\right)\times\dfrac{1+\sqrt2}{2}-\left(\dfrac{3\pi}{16}+\dfrac18+\dfrac{\sqrt2}{2}\right)=\dfrac98-\dfrac{3\pi}{16}+\dfrac{3\sqrt2}{8}.
$$

+++

#### 拓展解答 (2) 如图 3-3(a) 所示，在水平放置的椭圆底柱形容器内存放液体（密度为 $\rho\ \mathrm{kg/m^3}$），容器长为 $4\ \mathrm{m}$，椭圆方程为 $\dfrac{x^2}{4}+y^2=1$（单位：$\mathrm{m}$），即如图 3-3(b)。

（Ⅰ）当液面在过点 $(0,y)\ (-1\leqslant y\leqslant1)$ 处的水平线时，问容器内液体的体积是多少？
（Ⅱ）当容器内存满了液体后，平均每分钟从容器顶端抽出 $0.16\ \mathrm{m^3}$ 的液体，当液面降至 $y=0$ 处时，求液体下降的速度；
（Ⅲ）问抽出全部液体需做多少功？

***

**解**　（Ⅰ）

$$
V=4\cdot2\int_{-1}^{y}2\sqrt{1-y^2}\,\mathrm{d}y\xlongequal{y=\sin t}16\int_{-\frac{\pi}{2}}^{\arcsin y}\cos^2t\,\mathrm{d}t=8\arcsin y+8y\sqrt{1-y^2}+4\pi\ (\mathrm{m^3}).
$$

（Ⅱ）由于 $\dfrac{\mathrm{d}V}{\mathrm{d}t}=\dfrac{\mathrm{d}V}{\mathrm{d}y}\cdot\dfrac{\mathrm{d}y}{\mathrm{d}t}=16\sqrt{1-y^2}\cdot\dfrac{\mathrm{d}y}{\mathrm{d}t}$，故

$$
\dfrac{\mathrm{d}y}{\mathrm{d}t}\bigg|_{y=0}=\dfrac{1}{16\sqrt{1-y^2}}\cdot\dfrac{\mathrm{d}V}{\mathrm{d}t}\bigg|_{y=0}=\dfrac{1}{16}\times0.16=0.01\ (\mathrm{m/min}).
$$

（Ⅲ）

$$
\begin{aligned}
W&=4\rho g\int_{-1}^{1}4\sqrt{1-y^2}\cdot(1-y)\,\mathrm{d}y\\
&=4\rho g\left(\int_{-1}^{1}4\sqrt{1-y^2}\,\mathrm{d}y-\int_{-1}^{1}4\sqrt{1-y^2}\cdot y\,\mathrm{d}y\right)\\
&=4\rho g\int_{-1}^{1}4\sqrt{1-y^2}\,\mathrm{d}y-0=8\rho g\pi\ (\mathrm{J}).
\end{aligned}
$$

+++

#### 拓展解答 (3) 已知曲线 $y=\sqrt{x}$ 与 $y=ax\ (a>0)$ 所围图形绕 $x$ 轴旋转一周与绕 $y$ 轴旋转一周所得旋转体的体积相等，求 $a$ 的值。

***

**解**　$y=\sqrt{x}$ 与 $y=ax$ 的交点为 $(0,0)$，$\left(\dfrac{1}{a^2},\dfrac{1}{a}\right)\ (a>0)$。故

$$
V_x=\pi\int_0^{\frac{1}{a^2}}(\sqrt{x})^2\,\mathrm{d}x-\dfrac13\pi\cdot\left(\dfrac1a\right)^2\cdot\dfrac{1}{a^2}=\dfrac{\pi}{6a^4},
$$

$$
V_y=\dfrac{\pi}{3}\left(\dfrac{1}{a^2}\right)^2\cdot\dfrac1a-\pi\int_0^{\frac1a}x^2(y)\,\mathrm{d}y=\dfrac{\pi}{3a^5}-\pi\int_0^{\frac1a}y^4\,\mathrm{d}y=\dfrac{2\pi}{15a^5}.
$$

由已知 $V_x=V_y$，即 $\dfrac{\pi}{6a^4}=\dfrac{2\pi}{15a^5}$，解得 $a=\dfrac45$。
