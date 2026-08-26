---
quizify:
  format: 1
  deck: Math_880::Chapter_17
  tags: [Math, 880题, 数一, 第十七章, 随机变量及其分布]
---

+++

#### 基础选择 (1) 设随机变量 $X_1$ 与 $X_2$ 的分布函数分别为 $F_1(x)$ 与 $F_2(x)$，$F(x)=aF_1(x)-bF_2(x)$ 是某一随机变量的分布函数，则（　）．

;;;
A. $a=\dfrac{3}{5},b=-\dfrac{2}{5}$
B. $a=\dfrac{2}{3},b=\dfrac{2}{3}$
C. $a=-\dfrac{1}{2},b=\dfrac{3}{2}$
D. $a=\dfrac{1}{2},b=-\dfrac{3}{2}$
;;;A
***
要使 $F(x)$ 为某一随机变量的分布函数，必须有 $F(+\infty)=1$．又由已知，$F_1(+\infty)=1$，$F_2(+\infty)=1$，故 $a-b=1$，即只要 $a,b$ 的取值满足 $a-b=1$ 即可．

+++

#### 基础选择 (2) 设随机变量 $X$ 的概率密度为 $f(x)$，且 $f(-x)=f(x)$，$X$ 的分布函数为 $F(x)$，则对任意实数 $k$，有（　）．

;;;
A. $F(-k)=1-\displaystyle\int_{0}^{k}f(x)\mathrm{d}x$
B. $F(-k)=\dfrac{1}{2}-\displaystyle\int_{0}^{k}f(x)\mathrm{d}x$
C. $F(-k)=2F(k)-1$
D. $F(-k)=F(k)$
;;;B
***
考虑到 $f(-x)=f(x)$，知 $f(x)$ 为**偶函数**，故

$$F(-k)=\int_{-\infty}^{-k}f(x)\mathrm{d}x=\int_{k}^{+\infty}f(x)\mathrm{d}x=\frac{1}{2}\left[\int_{-\infty}^{-k}f(x)\mathrm{d}x+\int_{k}^{+\infty}f(x)\mathrm{d}x\right]$$

$$=\frac{1}{2}\left[\int_{-\infty}^{+\infty}f(x)\mathrm{d}x-\int_{-k}^{k}f(x)\mathrm{d}x\right]=\frac{1}{2}\left[1-\int_{-k}^{k}f(x)\mathrm{d}x\right]=\frac{1}{2}-\int_{0}^{k}f(x)\mathrm{d}x.$$

+++

#### 基础选择 (3) 下列函数中，可作为某一随机变量的分布函数的是（　）．

;;;
A. $F(x)=\dfrac{1}{1+x^{2}}$
B. $F(x)=\dfrac{1}{\pi}\arctan x+\dfrac{1}{2}$
C. $F(x)=\begin{cases}\dfrac{1}{2}(1-\mathrm{e}^{-x}),&x>0,\\0,&x\leqslant 0\end{cases}$
D. $F(x)=\displaystyle\int_{-\infty}^{x}f(t)\mathrm{d}t$，且 $\displaystyle\int_{-\infty}^{+\infty}f(t)\mathrm{d}t=1$
;;;B
***
$F(x)$ 要成为某一随机变量的分布函数，必满足以下三个条件：

①$0\leqslant F(x)\leqslant 1$，$F(+\infty)=1$，$F(-\infty)=0$；\
②$F(x)$ 是单调不减函数；\
③$F(x)$ 右连续，即 $\lim\limits_{x\to a^{+}}F(x)=F(a)$．

只有选项 **B** 满足以上三个条件，而 A，C 中 $F(x)$ 不满足 $F(+\infty)=1$，D 中 $F(x)$ 不一定单调不减．

+++

#### 基础选择 (4) 设 $X$ 是随机变量，对任意实数 $x$，$P\{X=x\}=0$ 的充分必要条件是（　）．

;;;
A. $X$ 的概率密度 $f(x)$ 是连续函数
B. $X$ 的分布函数 $F(x)$ 是连续函数
C. $X$ 为离散型随机变量
D. $X$ 是非离散型随机变量
;;;B
***
$F(x)=P\{X\leqslant x\}$，对任意实数 $x$，$F(x+0)=F(x)$（右连续）．又

$$P\{X=x\}=F(x)-F(x-0),$$

故 $P\{X=x\}=0\Leftrightarrow F(x)-F(x-0)=0\Leftrightarrow F(x-0)=F(x)\Leftrightarrow F(x)$ 在 $x$ 处连续．

+++

#### 基础选择 (5) 设 $X\sim N(\mu,4^{2})$，$Y\sim N(\mu,5^{2})$，记 $p_1=P\{X\leqslant\mu-4\}$，$p_2=P\{Y\geqslant\mu+5\}$，则（　）．

;;;
A. 对任意实数 $\mu$，有 $p_1>p_2$
B. 对任意实数 $\mu$，$p_1<p_2$
C. 对任意实数 $\mu$，有 $p_1=p_2$
D. 只对 $\mu=0$，有 $p_1=p_2$
;;;C
***
$$p_1=P\{X\leqslant\mu-4\}=P\left\{\frac{X-\mu}{4}\leqslant-1\right\}=\Phi(-1),$$

$$p_2=P\{Y\geqslant\mu+5\}=P\left\{\frac{Y-\mu}{5}\geqslant 1\right\}=1-\Phi(1)=\Phi(-1),$$

故 $p_1=p_2$，与 $\mu$ 取值无关．

+++

#### 基础选择 (6) 设 $X\sim N(\mu,\sigma^{2})$，则随着 $\sigma$ 的增大，$P\{|X-\mu|<\sigma\}$（　）．

;;;
A. 单调减少
B. 单调增加
C. 保持不变
D. 增减不确定
;;;C
***
由 $X\sim N(\mu,\sigma^{2})$，则 $\dfrac{X-\mu}{\sigma}\sim N(0,1)$，故

$$P\{|X-\mu|<\sigma\}=P\left\{\frac{|X-\mu|}{\sigma}<1\right\}=\Phi(1)-\Phi(-1),$$

与 $\mu,\sigma$ 取值无关，故 **C** 正确．

+++

#### 基础选择 (7) 设 $f(x)$ 为随机变量 $X$ 的概率密度，且 $f(1-x)=f(1+x)$，$\displaystyle\int_{1}^{2}f(x)\mathrm{d}x=0.4$，$X$ 的分布函数为 $F(x)$，则 $F(0)=$（　）．

;;;
A. $0.1$
B. $0.2$
C. $0.3$
D. $0.4$
;;;A
***
由 $f(1-x)=f(1+x)$，知 $f(x)$ 关于 $x=1$ 对称（图略），

$$F(0)=P\{X\leqslant 0\}=\int_{-\infty}^{0}f(x)\mathrm{d}x=0.5-0.4=0.1,$$

故 **A** 正确．

【注】$y=f(x)$ 的图形关于直线 $x=a$ 对称 $\Leftrightarrow f(a-x)=f(a+x)$．

+++

#### 基础填空 (1) 设随机变量 $X$ 服从参数为 $\lambda\ (\lambda>0)$ 的指数分布，则 $P\{X>16\mid X>8\}=$ ________．
***
$\mathrm{e}^{-8\lambda}$．

利用指数分布的**无记忆性**，得 $P\{X>16\mid X>8\}=P\{X>8\}=\mathrm{e}^{-8\lambda}$．

【注】指数分布的分布函数为 $F(x)=\begin{cases}1-\mathrm{e}^{-\lambda x},&x>0,\\0,&x\leqslant 0,\end{cases}$ 无记忆性是指：

$$P\{X>m+n\mid X>m\}=P\{X>n\}\quad(m,n\ \text{均大于}\ 0).$$

+++

#### 基础填空 (2) 设 $X\sim N(2,\sigma^{2})$ 且 $P\{0<X<2\}=0.3$，则 $P\{X>0\}=$ ________．
***
$0.8$．

由 $X\sim N(2,\sigma^{2})$，知 $X$ 的概率密度曲线 $\varphi(x)=\dfrac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x-2)^{2}}{2\sigma^{2}}}$ 关于直线 $x=2$ 对称，因此

$$P\{X<2\}=P\{X\geqslant 2\}=0.5,\quad P\{0<X<2\}=P\{2\leqslant X<4\}=0.3,$$

故

$$P\{X>0\}=1-P\{X\leqslant 0\}=1-\left(P\{X<2\}-P\{0<X<2\}\right)=1-0.5+0.3=0.8.$$

+++

#### 基础填空 (3) 设 $X\sim N(\mu,\sigma^{2})$，$f(x)$ 为 $X$ 的概率密度，当 $x=1$ 时，$f(x)$ 取得最大值 $\dfrac{1}{2\sqrt{2\pi}}$，则 $P\{X<3\}=$ ________（用标准正态分布函数 $\Phi(x)$ 表示）．
***
$\Phi(1)$．

由已知，$f(x)=\dfrac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x-\mu)^{2}}{2\sigma^{2}}}$，在 $x=\mu=1$ 处，$f(x)$ 取得最大值

$$f(\mu)=\frac{1}{\sqrt{2\pi}\sigma}=\frac{1}{2\sqrt{2\pi}},$$

故 $\mu=1$，$\sigma=2$，即 $X\sim N(1,4)$，所以 $P\{X<3\}=P\left\{\dfrac{X-1}{2}<1\right\}=\Phi(1)$．

+++

#### 基础填空 (4) 设自动机床在任何时长为 $t$ 的时间间隔内发生故障的次数 $X$ 服从参数为 $\lambda t$ 的泊松分布，$Y$ 表示相继两次故障之间的时间间隔，则当 $t>0$ 时，$P\{Y>t\}=$ ________．
***
$\mathrm{e}^{-\lambda t}$．

$\{Y>t\}$ 表示相继两次故障之间的时间间隔超过 $t$，故在时长为 $t$ 的时间间隔内没有发生故障，所以 $P\{Y>t\}=P\{X=0\}$，而 $X$ 是服从参数 $\lambda t$ 的泊松分布，故

$$P\{Y>t\}=P\{X=0\}=\frac{(\lambda t)^{0}}{0!}\mathrm{e}^{-\lambda t}=\mathrm{e}^{-\lambda t}.$$

+++

#### 基础填空 (5) 设 $X\sim N(0,1)$，则 $Y=|X|$ 的概率密度 $f_Y(y)=$ ________．
***
$$f_Y(y)=\begin{cases}\sqrt{\dfrac{2}{\pi}}\mathrm{e}^{-\frac{y^{2}}{2}},&y>0,\\0,&y\leqslant 0.\end{cases}$$

由 $Y=|X|$ 取值非负，故当 $y\leqslant 0$ 时，$F_Y(y)=0$；当 $y>0$ 时，

$$F_Y(y)=P\{Y\leqslant y\}=P\{|X|\leqslant y\}=P\{-y\leqslant X\leqslant y\}$$

$$=\int_{-y}^{y}\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{t^{2}}{2}}\mathrm{d}t=\int_{0}^{y}\sqrt{\frac{2}{\pi}}\mathrm{e}^{-\frac{t^{2}}{2}}\mathrm{d}t,$$

于是

$$f_Y(y)=F_Y'(y)=\begin{cases}\sqrt{\dfrac{2}{\pi}}\mathrm{e}^{-\frac{y^{2}}{2}},&y>0,\\0,&y\leqslant 0.\end{cases}$$

+++

#### 基础解答 (1) 设离散型随机变量 $X$ 的分布律为

| $X$ | $-1$ | $1$ | $2$ |
| --- | --- | --- | --- |
| $p$ | $0.2$ | $0.3$ | $0.5$ |

（Ⅰ）求 $X$ 的分布函数；（Ⅱ）求 $P\left\{X>\dfrac{1}{2}\right\}$；（Ⅲ）$P\{-1\leqslant X\leqslant 2\}$．
***
（Ⅰ）分布函数的定义：$F(x)=P\{X\leqslant x\}$．

当 $x<-1$ 时，$F(x)=P\{X\leqslant x\}=0$；\
当 $-1\leqslant x<1$ 时，$F(x)=P\{X\leqslant x\}=P\{X=-1\}=0.2$；\
当 $1\leqslant x<2$ 时，$F(x)=P\{X\leqslant x\}=P\{X=-1\}+P\{X=1\}=0.2+0.3=0.5$；\
当 $x\geqslant 2$ 时，$F(x)=P\{X\leqslant x\}=P\{\Omega\}=1$，故

$$F(x)=\begin{cases}0,&x<-1,\\0.2,&-1\leqslant x<1,\\0.5,&1\leqslant x<2,\\1,&x\geqslant 2.\end{cases}$$

（Ⅱ）$P\left\{X>\dfrac{1}{2}\right\}=1-P\left\{X\leqslant\dfrac{1}{2}\right\}=1-F\left(\dfrac{1}{2}\right)=1-0.2=0.8$．

（Ⅲ）

$$P\{-1\leqslant X\leqslant 2\}=P\{X=-1\}+P\{-1<X\leqslant 2\}$$

$$=P\{X=-1\}+F(2)-F(-1)=0.2+1-0.2=1.$$

+++

#### 基础解答 (2) 设连续型随机变量 $X$ 的分布函数为 $F(x)=\begin{cases}0,&x\leqslant-a,\\k_1+k_2\arcsin\dfrac{x}{a},&-a<x\leqslant a,\\1,&x>a,\end{cases}$ 其中 $a>0$．

（Ⅰ）求常数 $k_1,k_2$ 的值；\
（Ⅱ）求 $X$ 的概率密度；\
（Ⅲ）求 $P\left\{|X|<\dfrac{a}{2}\right\}$．
***
（Ⅰ）由分布函数 $F(x)$ 的性质，有

$$F(-a+0)=F(-a),\quad F(a+0)=F(a),$$

得 $k_1=\dfrac{1}{2}$，$k_2=\dfrac{1}{\pi}$．

（Ⅱ）

$$f(x)=F'(x)=\begin{cases}\dfrac{1}{\pi\sqrt{a^{2}-x^{2}}},&|x|<a,\\0,&|x|\geqslant a.\end{cases}$$

（Ⅲ）

$$P\left\{|X|<\frac{a}{2}\right\}=P\left\{-\frac{a}{2}<X<\frac{a}{2}\right\}=F\left(\frac{a}{2}\right)-F\left(-\frac{a}{2}\right)$$

$$=\frac{1}{2}+\frac{1}{\pi}\arcsin\frac{1}{2}-\left[\frac{1}{2}+\frac{1}{\pi}\arcsin\left(-\frac{1}{2}\right)\right]=\frac{1}{3}.$$

+++

#### 基础解答 (3) 设随机变量 $X$ 服从参数为 $\lambda$ 的指数分布，对 $X$ 进行三次独立重复观察，至少有一次观测值大于 $3$ 的概率为 $\dfrac{26}{27}$，求 $\lambda$ 的值．
***
由已知，$X$ 的概率密度为 $f(x)=\begin{cases}\lambda\mathrm{e}^{-\lambda x},&x>0,\\0,&x\leqslant 0\end{cases}(\lambda>0)$，令 $Y$ 为对 $X$ 作三次独立重复观察中，事件 $\{X>3\}$ 发生的次数，则 $Y\sim B(3,p)$，且

$$p=P\{X>3\}=\int_{3}^{+\infty}\lambda\mathrm{e}^{-\lambda x}\mathrm{d}x=\mathrm{e}^{-3\lambda}.$$

依题设，

$$P\{Y\geqslant 1\}=1-P\{Y=0\}=1-(1-p)^{3}=\frac{26}{27},$$

故 $p=\dfrac{2}{3}$，由 $p=\dfrac{2}{3}=\mathrm{e}^{-3\lambda}$，得 $\lambda=-\dfrac{1}{3}\ln\dfrac{2}{3}$．

+++

#### 基础解答 (4) 设随机变量 $X$ 的概率密度为 $f(x)=\begin{cases}3x^{2},&0<x<1,\\0,&\text{其他,}\end{cases}$ 求 $Y=\dfrac{1}{X}$ 的分布函数和概率密度．
***
用定义法求分布函数 $F_Y(y)$，$F_Y(y)=P\{Y\leqslant y\}=P\left\{\dfrac{1}{X}\leqslant y\right\}$．

当 $y<0$ 时，$F_Y(y)=P\left\{\dfrac{1}{X}\leqslant y<0\right\}=P\left\{\dfrac{1}{y}\leqslant X<0\right\}=\displaystyle\int_{\frac{1}{y}}^{0}0\,\mathrm{d}y=0$；

当 $0<\dfrac{1}{y}<1$，即 $y>1$ 时，

$$F_Y(y)=P\left\{\frac{1}{X}\leqslant y\right\}=P\left\{X\geqslant\frac{1}{y}\right\}=1-P\left\{X<\frac{1}{y}\right\}=1-\int_{0}^{\frac{1}{y}}3x^{2}\mathrm{d}x=1-\frac{1}{y^{3}};$$

当 $\dfrac{1}{y}>1$，即 $0<y<1$ 时，

$$F_Y(y)=P\{Y\leqslant y\}=P\{Y\leqslant 0\}+P\{0<Y\leqslant y\}$$

$$=P\left\{0<\frac{1}{X}\leqslant y\right\}=P\left\{X\geqslant\frac{1}{y}\right\}$$

$$=1-P\left\{X<\frac{1}{y}\right\}=1-\left(\int_{0}^{1}3x^{2}\mathrm{d}x+\int_{1}^{\frac{1}{y}}0\,\mathrm{d}x\right)=0,$$

故

$$F_Y(y)=\begin{cases}1-\dfrac{1}{y^{3}},&y>1,\\0,&\text{其他,}\end{cases}\qquad f_Y(y)=F_Y'(y)=\begin{cases}\dfrac{3}{y^{4}},&y>1,\\0,&\text{其他.}\end{cases}$$

+++

#### 基础解答 (5) 设随机变量 $X$ 在 $(0,1)$ 上服从均匀分布，求 $Y=-2\ln X$ 的概率密度．
***
由已知，$f(x)=\begin{cases}1,&0<x<1,\\0,&\text{其他,}\end{cases}$ $y=-2\ln x$ 在 $(0,1)$ 内单调减少，有反函数 $x=\mathrm{e}^{-\frac{y}{2}}$，用公式有

$$f_Y(y)=\begin{cases}f\left(\mathrm{e}^{-\frac{y}{2}}\right)\left|\left(\mathrm{e}^{-\frac{y}{2}}\right)'\right|,&0<\mathrm{e}^{-\frac{y}{2}}<1,\\0,&\text{其他}\end{cases}=\begin{cases}\dfrac{1}{2}\mathrm{e}^{-\frac{y}{2}},&y>0,\\0,&\text{其他.}\end{cases}$$

+++

#### 基础解答 (6) 设随机变量 $X$ 的概率密度为 $f(x)=\dfrac{1}{\pi(1+x^{2})}$，$-\infty<x<+\infty$，求 $Y=1-\sqrt[3]{X}$ 的分布函数和概率密度．
***
用定义法，$Y$ 的分布函数为

$$F_Y(y)=P\{Y\leqslant y\}=P\{1-\sqrt[3]{X}\leqslant y\}$$

$$=P\{X\geqslant(1-y)^{3}\}=\int_{(1-y)^{3}}^{+\infty}\frac{\mathrm{d}x}{\pi(1+x^{2})}$$

$$=\frac{1}{\pi}\arctan x\bigg|_{(1-y)^{3}}^{+\infty}=\frac{1}{\pi}\left[\frac{\pi}{2}-\arctan(1-y)^{3}\right],$$

$Y$ 的概率密度为

$$f_Y(y)=F_Y'(y)=\frac{3}{\pi}\cdot\frac{(1-y)^{2}}{1+(1-y)^{6}}.$$

+++

#### 综合选择 (1) 设 $f(x)$ 为随机变量 $X$ 的概率密度，则下列选项可作为某一随机变量的概率密度的是（　）．

;;;
A. $f(1-x)$
B. $f\left(\dfrac{x}{2}\right)$
C. $f(x^{2})$
D. $f^{2}(x)$
;;;A
***
$f(x)$ 作为随机变量的概率密度，必须满足：①$f(x)\geqslant 0$；②$\displaystyle\int_{-\infty}^{+\infty}f(x)\mathrm{d}x=1$．

对于 A，$f(1-x)\geqslant 0$ 且

$$\int_{-\infty}^{+\infty}f(1-x)\mathrm{d}x=-\int_{-\infty}^{+\infty}f(1-x)\mathrm{d}(1-x)=\int_{-\infty}^{+\infty}f(t)\mathrm{d}t=1,$$

故 **A** 正确．

对于 B，$\displaystyle\int_{-\infty}^{+\infty}f\left(\frac{x}{2}\right)\mathrm{d}x=2\int_{-\infty}^{+\infty}f\left(\frac{x}{2}\right)\mathrm{d}\left(\frac{x}{2}\right)=2\neq 1$．

对于 C，D，$\displaystyle\int_{-\infty}^{+\infty}f^{2}(x)\mathrm{d}x$ 与 $\displaystyle\int_{-\infty}^{+\infty}f(x^{2})\mathrm{d}x$ 都不为 $1$．

+++

#### 综合选择 (2) 设 $X_1,X_2,X_3$ 都服从正态分布，且 $X_1\sim N(0,1)$，$X_2\sim N(0,2^{2})$，$X_3\sim N(5,3^{2})$，$p_i=P\{-2\leqslant X_i\leqslant 2\}\ (i=1,2,3)$，则（　）．

;;;
A. $p_3>p_1>p_2$
B. $p_1>p_3>p_2$
C. $p_1>p_2>p_3$
D. $p_2>p_1>p_3$
;;;C
***
依题设，有

$$p_1=P\{-2\leqslant X_1\leqslant 2\}=\Phi(2)-\Phi(-2)=2\Phi(2)-1,$$

$$p_2=P\{-2\leqslant X_2\leqslant 2\}=P\left\{-1\leqslant\frac{X_2-0}{2}\leqslant 1\right\}=\Phi(1)-\Phi(-1)=2\Phi(1)-1,$$

$$p_3=P\{-2\leqslant X_3\leqslant 2\}=P\left\{-\frac{7}{3}\leqslant\frac{X_3-5}{3}\leqslant-1\right\}=\Phi(-1)-\Phi\left(-\frac{7}{3}\right),$$

又 $\Phi(x)$ 单调增加，所以 $p_1=2\Phi(2)-1>2\Phi(1)-1=p_2$．

而 $\Phi(1)-\Phi(-1)>0.68$，故

$$p_2=\Phi(1)-\Phi(-1)>0.68>0.5=\Phi(0)>\Phi(-1)>p_3,$$

所以 **C** 正确．

【注】根据 $3\sigma$ 准则，可知 $\Phi(1)-\Phi(-1)>0.68$．

+++

#### 综合选择 (3) 设随机变量 $X$ 的概率密度为 $f(x)$，若当 $-\infty<x<+\infty$ 时，恒有 $0\leqslant f(x)<1$，则 $X$ 可能服从（　）．

;;;
A. $N(1,\sigma^{2})$
B. $N(\mu,1)$
C. $N(\mu,\sigma^{2})$
D. $N(0,\sigma^{2})$
;;;B
***
若 $X\sim N(\mu,\sigma^{2})$，则 $X$ 的概率密度为

$$f(x)=\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x-\mu)^{2}}{2\sigma^{2}}},\quad-\infty<x<+\infty.$$

当 $X=\mu$ 时，$f(x)$ 取得最大值 $\dfrac{1}{\sqrt{2\pi}\sigma}$，显然，$f(x)$ 的最大值与 $\mu$ 无关，故当 $X\sim N(\mu,\sigma^{2})$ 时，$f(\mu)=\dfrac{1}{\sqrt{2\pi}\sigma}$．

当 $\sigma=1$ 时，$f(\mu)=\dfrac{1}{\sqrt{2\pi}}<1$，从而 $0\leqslant f(x)<1$，故 **B** 正确．

当 $\sigma<\dfrac{1}{\sqrt{2\pi}}$ 时，$f(\mu)=\dfrac{1}{\sqrt{2\pi}\sigma}>1$，所以 A，C，D 不正确．

+++

#### 综合填空 (1) 设随机变量 $X\sim N(\mu,\sigma^{2})$，$\sigma>0$，$(x_0,y_0)$ 为其分布函数曲线 $y=F(x)$ 的拐点，则 $x_0=$ ________，$y_0=$ ________．
***
$\mu$，$\dfrac{1}{2}$．

由 $X\sim N(\mu,\sigma^{2})$，则其概率密度为 $f(x)=\dfrac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x-\mu)^{2}}{2\sigma^{2}}}$，则

$$F''(x_0)=f'(x_0)=\frac{1}{\sqrt{2\pi}\sigma}\cdot\mathrm{e}^{-\frac{(x_0-\mu)^{2}}{2\sigma^{2}}}\cdot\frac{-2(x_0-\mu)}{2\sigma^{2}}=0,$$

故 $x_0=\mu$，$F(x_0)=y_0=\dfrac{1}{2}$．

+++

#### 综合填空 (2) 设随机变量 $X\sim N(\mu,\sigma^{2})$，其中 $\sigma>0$，$F(x)$ 为 $X$ 的分布函数，则 $F(\mu-x\sigma)+F(\mu+x\sigma)=$ ________．
***
$1$．

$$F(\mu-x\sigma)+F(\mu+x\sigma)=P\{X\leqslant\mu-x\sigma\}+P\{X\leqslant\mu+x\sigma\}$$

$$=P\left\{\frac{X-\mu}{\sigma}\leqslant-x\right\}+P\left\{\frac{X-\mu}{\sigma}\leqslant x\right\}$$

$$=\Phi(-x)+\Phi(x)=\left[1-\Phi(x)\right]+\Phi(x)=1.$$

+++

#### 综合填空 (3) 设随机变量 $X$ 服从泊松分布，且 $P\{X=1\}=P\{X=2\}$，则 $P\{X>1\}=$ ________．
***
$1-3\mathrm{e}^{-2}$．

由已知，

$$P\{X=k\}=\frac{\lambda^{k}}{k!}\mathrm{e}^{-\lambda},\quad\lambda>0,\ k=0,1,2,\cdots,$$

依题设，$\lambda\mathrm{e}^{-\lambda}=\dfrac{\lambda^{2}\mathrm{e}^{-\lambda}}{2!}$，解得 $\lambda=2$，$\lambda=0$（舍去），所以

$$P\{X>1\}=1-P\{X\leqslant 1\}=1-P\{X=0\}-P\{X=1\}=1-\mathrm{e}^{-2}-2\mathrm{e}^{-2}=1-3\mathrm{e}^{-2}.$$

+++

#### 综合填空 (4) 在伯努利试验中，设事件发生的概率 $p=\dfrac{3}{4}$，$X$ 表示首次发生所需试验次数，$n$ 为正整数，则 $\displaystyle\sum_{n=1}^{\infty}P\{X=2n\}=$ ________．
***
$\dfrac{1}{5}$．

依题设，

$$P\{X=k\}=(1-p)^{k-1}p=pq^{k-1}\quad\left(q=1-p=\frac{1}{4}\right),$$

故

$$\sum_{n=1}^{\infty}P\{X=2n\}=pq+pq^{3}+\cdots+pq^{2n-1}+\cdots=pq\cdot\frac{1}{1-q^{2}}=\frac{q}{1+q}=\frac{1}{5}.$$

+++

#### 综合填空 (5) 设离散型随机变量 $X$ 的分布律为 $P\{X=k\}=\dfrac{a}{k!}\mathrm{e}^{-2}$，$k=0,1,2,\cdots$，则常数 $a=$ ________．
***
$\mathrm{e}$．

由分布律的性质，有 $\displaystyle\sum_{k=0}^{\infty}P\{X=k\}=1$，故

$$\sum_{k=0}^{\infty}\frac{a}{k!}\mathrm{e}^{-2}=a\mathrm{e}^{-2}\sum_{k=0}^{\infty}\frac{1}{k!}=a\mathrm{e}^{-2}\cdot\mathrm{e}=a\mathrm{e}^{-1}=1,$$

所以 $a=\mathrm{e}$．

【注】①$\displaystyle\sum_{k=0}^{\infty}\frac{x^{k}}{k!}=\mathrm{e}^{x}\ (-\infty<x<+\infty)$．

②泊松分布 $P\{X=k\}=\dfrac{\lambda^{k}}{k!}\mathrm{e}^{-\lambda}$，$k=0,1,2,\cdots$，可知，当 $\lambda=1$ 时，有 $P\{X=k\}=\dfrac{1}{k!}\mathrm{e}^{-1}$，对照已知条件，得 $a=\mathrm{e}$．

+++

#### 综合填空 (6) 设 $X\sim N(0,\sigma^{2})$，$X$ 在区间 $(a,b)$ 内取值的概率最大，其中 $a>0$，则 $\sigma^{2}=$ ________．
***
$\dfrac{a^{2}-b^{2}}{2(\ln a-\ln b)}$．

依题意，有 $\dfrac{X-0}{\sigma}\sim N(0,1)$，故

$$P\{a<X<b\}=P\left\{\frac{a}{\sigma}<\frac{X}{\sigma}<\frac{b}{\sigma}\right\}=\Phi\left(\frac{b}{\sigma}\right)-\Phi\left(\frac{a}{\sigma}\right)$$

$$=\frac{1}{\sqrt{2\pi}}\left[\int_{-\infty}^{\frac{b}{\sigma}}\mathrm{e}^{-\frac{x^{2}}{2}}\mathrm{d}x-\int_{-\infty}^{\frac{a}{\sigma}}\mathrm{e}^{-\frac{x^{2}}{2}}\mathrm{d}x\right]\xlongequal{\text{记}}f(\sigma),$$

所以

$$f'(\sigma)=\frac{1}{\sqrt{2\pi}}\left[\mathrm{e}^{-\frac{b^{2}}{2\sigma^{2}}}\cdot\left(-\frac{b}{\sigma^{2}}\right)-\mathrm{e}^{-\frac{a^{2}}{2\sigma^{2}}}\cdot\left(-\frac{a}{\sigma^{2}}\right)\right].$$

令 $f'(\sigma)=0$，得 $b\mathrm{e}^{-\frac{b^{2}}{2\sigma^{2}}}=a\mathrm{e}^{-\frac{a^{2}}{2\sigma^{2}}}$，取对数，得 $\ln b+\dfrac{-b^{2}}{2\sigma^{2}}=\ln a+\dfrac{-a^{2}}{2\sigma^{2}}$，解得

$$\sigma^{2}=\frac{a^{2}-b^{2}}{2(\ln a-\ln b)}.$$

+++

#### 综合填空 (7) 设随机变量 $X$ 服从参数为 $1$ 的指数分布，$k$ 为大于零的常数，则 $P\{X\leqslant k+1\mid X>k\}=$ ________．
***
$1-\dfrac{1}{\mathrm{e}}$．

**解法 1** 利用指数分布的无记忆性进行计算．

由于 $X\sim E(1)$，且当 $s,t>0$ 时，有 $P\{X>s+t\mid X>t\}=P\{X>s\}$，故

$$P\{X\leqslant k+1\mid X>k\}=1-P\{X>k+1\mid X>k\}=1-P\{X>1\}=1-\mathrm{e}^{-1}=1-\frac{1}{\mathrm{e}}.$$

**解法 2** 直接利用条件概率进行计算．

$$P\{X\leqslant k+1\mid X>k\}=1-P\{X>k+1\mid X>k\}=1-\frac{P\{X>k+1,X>k\}}{P\{X>k\}}$$

$$=1-\frac{P\{X>k+1\}}{P\{X>k\}}=1-\frac{\displaystyle\int_{k+1}^{+\infty}\mathrm{e}^{-t}\mathrm{d}t}{\displaystyle\int_{k}^{+\infty}\mathrm{e}^{-t}\mathrm{d}t}=1-\frac{\mathrm{e}^{-(k+1)}}{\mathrm{e}^{-k}}=1-\frac{1}{\mathrm{e}}.$$

+++

#### 综合解答 (1) 设随机变量 $X$ 服从 $\lambda=2$ 的指数分布，求 $Y=1-\mathrm{e}^{-2X}$ 的分布函数和概率密度．
***
由已知，$X$ 的分布函数为 $F(x)=\begin{cases}1-\mathrm{e}^{-2x},&x>0,\\0,&x\leqslant 0,\end{cases}$ $y=1-\mathrm{e}^{-2x}$ 是单调增加函数，其反函数为 $x=-\dfrac{\ln(1-y)}{2}$．

令 $G(y)$ 是 $Y$ 的分布函数，则

$$G(y)=P\{Y\leqslant y\}=P\{1-\mathrm{e}^{-2X}\leqslant y\}=\begin{cases}0,&y<0,\\P\left\{X\leqslant-\dfrac{\ln(1-y)}{2}\right\},&0\leqslant y<1,\\1,&y\geqslant 1,\end{cases}=\begin{cases}0,&y<0,\\y,&0\leqslant y<1,\\1,&y\geqslant 1,\end{cases}$$

$$g_Y(y)=G'(y)=\begin{cases}1,&0\leqslant y<1,\\0,&\text{其他,}\end{cases}$$

即 $Y$ 在 $[0,1]$ 上服从均匀分布．

【注】结论：设连续型随机变量 $X$ 的分布函数为 $F(x)$，且严格单调增加，则 $Y=F(X)$ 服从均匀分布（见《李林考研数学系列概率论与数理统计辅导讲义》第二章）．

+++

#### 综合解答 (2) 设连续型随机变量 $X$ 的概率密度为 $f(x)$，求 $Y=\sin X$ 的分布函数和概率密度．
***
$Y=\sin X$ 的值域为 $[-1,1]$．

当 $-1\leqslant y<1$ 时，

$$F(y)=P\{Y\leqslant y\}=P\{\sin X\leqslant y\}=P\{X\in D\},$$

其中

$$D=\{x\mid\sin x\leqslant y\}=\bigcup_{k=-\infty}^{\infty}\left[2k\pi-\pi-\arcsin y,\ 2k\pi+\arcsin y\right],$$

故 $F(y)=\displaystyle\sum_{k=-\infty}^{\infty}\int_{2k\pi-\pi-\arcsin y}^{2k\pi+\arcsin y}f(x)\mathrm{d}x$．

当 $y<-1$ 时，$F(y)=0$；当 $y\geqslant 1$ 时，$F(y)=1$．$Y$ 的概率密度为 $f_Y(y)=F'(y)$，即

$$f_Y(y)=\begin{cases}\displaystyle\sum_{k=-\infty}^{\infty}\left[f(2k\pi+\arcsin y)+f(2k\pi-\pi-\arcsin y)\right]\cdot\frac{1}{\sqrt{1-y^{2}}},&-1\leqslant y<1,\\0,&\text{其他.}\end{cases}$$

+++

#### 综合解答 (3) 设随机变量 $X$ 的概率密度为 $f(x)=\begin{cases}\dfrac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{x^{2}}{2}},&x\leqslant 0,\\\mathrm{e}^{-2x},&x>0,\end{cases}$ 求 $Y=X^{2}$ 的分布函数和概率密度（可用 $\varphi(x)$ 和 $\Phi(x)$ 表示）．
***
用定义法，$F_Y(y)=P\{Y\leqslant y\}=P\{X^{2}\leqslant y\}$．

当 $y\leqslant 0$ 时，$F_Y(y)=0$；

当 $y>0$ 时，

$$F_Y(y)=P\{X^{2}\leqslant y\}=P\{-\sqrt{y}\leqslant X\leqslant\sqrt{y}\}=F(\sqrt{y})-F(-\sqrt{y}),$$

$F(x)$ 是 $X$ 的分布函数．

当 $x\leqslant 0$ 时，$F(x)=\Phi(x)$，故 $F(-\sqrt{y})=\Phi(-\sqrt{y})$；

当 $x>0$ 时，

$$F(x)=\frac{1}{2}+\int_{0}^{x}\mathrm{e}^{-2t}\mathrm{d}t=\frac{1}{2}+\frac{1}{2}\left(1-\mathrm{e}^{-2x}\right),$$

故 $F(\sqrt{y})=\dfrac{1}{2}+\dfrac{1}{2}\left(1-\mathrm{e}^{-2\sqrt{y}}\right)$，所以

$$F_Y(y)=\begin{cases}0,&y\leqslant 0,\\\dfrac{1}{2}+\dfrac{1}{2}\left(1-\mathrm{e}^{-2\sqrt{y}}\right)-\Phi(-\sqrt{y}),&y>0,\end{cases}$$

$$f_Y(y)=F_Y'(y)=\begin{cases}0,&y\leqslant 0,\\\dfrac{1}{2\sqrt{y}}\left[\mathrm{e}^{-2\sqrt{y}}+\varphi(-\sqrt{y})\right],&y>0.\end{cases}$$

+++

#### 拓展解答 (1) 设随机变量 $X$ 的概率密度为 $f(x)=\begin{cases}1-|x|,&-1<x<1,\\0,&\text{其他.}\end{cases}$ 求 $Y=X^{2}+1$ 的分布函数与概率密度．
***
$y=x^{2}+1\ (-1<x<1)$ 不是单调函数，用定义法．

$$F_Y(y)=P\{Y\leqslant y\}=P\{X^{2}+1\leqslant y\}=P\{X^{2}\leqslant y-1\}.$$

当 $y<1$ 时，$F_Y(y)=0$；

当 $1\leqslant y<2$ 时，

$$F_Y(y)=P\{-\sqrt{y-1}\leqslant X\leqslant\sqrt{y-1}\}=\int_{-\sqrt{y-1}}^{\sqrt{y-1}}(1-|x|)\mathrm{d}x=2\int_{0}^{\sqrt{y-1}}(1-x)\mathrm{d}x$$

$$=1-\left(1-\sqrt{y-1}\right)^{2};$$

当 $y\geqslant 2$ 时，$F_Y(y)=1$，故

$$F_Y(y)=\begin{cases}0,&y<1,\\1-\left(1-\sqrt{y-1}\right)^{2},&1\leqslant y<2,\\1,&y\geqslant 2,\end{cases}$$

$$f_Y(y)=F_Y'(y)=\begin{cases}\dfrac{1}{\sqrt{y-1}}-1,&1<y<2,\\0,&\text{其他.}\end{cases}$$
