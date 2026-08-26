---
quizify:
  format: 1
  deck: Math_880::Chapter_19
  tags: [Math, 880题, 数一, 第十九章, 随机变量的数字特征]
---

+++

#### 基础选择 (1) 设随机变量 $X$ 服从参数为 $2$ 的指数分布，则 $Y=2X+\mathrm{e}^{-2X}$ 的期望 $EY=$（　）．

;;;
A. $\dfrac{3}{2}$
B. $\dfrac{2}{3}$
C. $\dfrac{3}{4}$
D. $\dfrac{4}{3}$
;;;A
***
由于 $X$ 服从参数为 $2$ 的指数分布，故 $EX=\dfrac{1}{2}$．又

$$E(\mathrm{e}^{-2X})=\int_{-\infty}^{+\infty}\mathrm{e}^{-2x}f(x)\mathrm{d}x=\int_{0}^{+\infty}\mathrm{e}^{-2x}\cdot 2\mathrm{e}^{-2x}\mathrm{d}x$$

$$=2\int_{0}^{+\infty}\mathrm{e}^{-4x}\mathrm{d}x=\frac{1}{2},$$

所以

$$EY=2EX+E(\mathrm{e}^{-2X})=2\times\frac{1}{2}+\frac{1}{2}=\frac{3}{2}.$$

+++

#### 基础选择 (2) 设随机变量 $X\sim B(n,p)$，且 $EX=2.4$，$DX=1.44$，则（　）．

;;;
A. $n=8$，$p=0.6$
B. $n=6$，$p=0.4$
C. $n=4$，$p=0.5$
D. $n=12$，$p=0.1$
;;;B
***
由 $X\sim B(n,p)$，可知 $EX=np$，$DX=np(1-p)$，故

$$\begin{cases}np=2.4,\\np(1-p)=1.44,\end{cases}$$

解得 $n=6$，$p=0.4$．

+++

#### 基础选择 (3) 设 $EX$ 与 $E(X^2)$ 均存在，则（　）．

;;;
A. $E(X^2)\geqslant(EX)^2$
B. $E(X^2)<(EX)^2$
C. $E(X^2)<EX$
D. $E(X^2)>EX$
;;;A
***
由 $DX=E(X^2)-(EX)^2\geqslant 0$，知 $E(X^2)\geqslant(EX)^2$．

C 与 D 均不一定成立，如 $X\sim N\left(\dfrac{1}{2},\dfrac{1}{4}\right)$，

$$EX=\frac{1}{2},\quad DX=\frac{1}{4},$$

$$E(X^2)=DX+(EX)^2=\frac{1}{4}+\frac{1}{4}=\frac{1}{2},$$

则 $E(X^2)=EX=\dfrac{1}{2}$．

+++

#### 基础选择 (4) 设随机变量 $X$，有 $EX=\mu$，$DX=\sigma^2$（$\mu,\sigma$ 为常数），则对任意常数 $C$，下列选项正确的是（　）．

;;;
A. $E\left[(X-C)^2\right]=E(X^2)-C^2$
B. $E\left[(X-C)^2\right]=E\left[(X-\mu)^2\right]$
C. $E\left[(X-C)^2\right]<E\left[(X-\mu)^2\right]$
D. $E\left[(X-C)^2\right]\geqslant E\left[(X-\mu)^2\right]$
;;;D
***
因为

$$E\left[(X-C)^2\right]=E\left[(X-\mu+\mu-C)^2\right]=E\left[(X-\mu)^2\right]+(\mu-C)^2,$$

其中 $(\mu-C)^2\geqslant 0$，所以 $E\left[(X-C)^2\right]\geqslant E\left[(X-\mu)^2\right]$，故 **D** 正确．

B 当且仅当 $\mu=C$ 时才成立．

+++

#### 基础选择 (5) 设 $(X,Y)$ 服从二维正态分布，则 $U=X+Y$ 与 $V=X-Y$ 不相关的充要条件是（　）．

;;;
A. $EX=EY$
B. $E(X^2)=E(Y^2)$
C. $E(X^2)+(EY)^2=E(Y^2)+(EX)^2$
D. $E(X^2)+(EX)^2=E(Y^2)+(EY)^2$
;;;C
***
因为 $U$ 与 $V$ 不相关 $\Leftrightarrow\mathrm{Cov}(U,V)=0$，由于

$$\mathrm{Cov}(U,V)=\mathrm{Cov}(X+Y,X-Y)$$

$$=\mathrm{Cov}(X,X)-\mathrm{Cov}(X,Y)+\mathrm{Cov}(Y,X)-\mathrm{Cov}(Y,Y)$$

$$=\mathrm{Cov}(X,X)-\mathrm{Cov}(Y,Y)=DX-DY=0,$$

故 $U,V$ 不相关的充要条件是 $DX=DY$．

而

$$DX=E(X^2)-(EX)^2,\quad DY=E(Y^2)-(EY)^2,$$

故 **C** 正确．

+++

#### 基础选择 (6) 设 $X\sim N(0,1)$，$Y\sim N(1,4)$，且 $\rho_{XY}=1$，则（　）．

;;;
A. $P\{Y=2X+1\}=1$
B. $P\{Y=-2X+1\}=1$
C. $P\{Y=-2X-1\}=1$
D. $P\{Y=2X-1\}=1$
;;;A
***
由 $\rho_{XY}=1\Leftrightarrow P\{Y=aX+b\}=1$，且 $a>0$，排除 B，C．又

$$1=EY=E(aX+b)=aEX+b,$$

由于 $EX=0$，故 $b=1$，所以 **A** 正确．

【注】结论：$|\rho_{XY}|=1\Leftrightarrow$ 存在常数 $a\ (a\neq 0)$ 和 $b$，使得 $P\{Y=aX+b\}=1$，且

$$\rho_{XY}=\begin{cases}1,&a>0,\\-1,&a<0.\end{cases}$$

（见《李林考研数学系列概率论与数理统计辅导讲义》第四章）

+++

#### 基础选择 (7) 设随机变量 $X$ 在 $[-1,1]$ 上服从均匀分布，$Y_1=\arcsin X$，$Y_2=\arccos X$，则 $\rho_{Y_1Y_2}=$（　）．

;;;
A. $1$
B. $-1$
C. $\dfrac{1}{2}$
D. $\dfrac{3}{4}$
;;;B
***
由于 $\arcsin X+\arccos X=\dfrac{\pi}{2}$，故 $Y_1+Y_2=\dfrac{\pi}{2}$，即 $Y_1=\dfrac{\pi}{2}-Y_2$，故 $\rho_{Y_1Y_2}=-1$．

+++

#### 基础选择 (8) 设袋中有 $6$ 只红球，$4$ 只白球，任意摸出一只球，记住颜色后放回袋中，共进行 $4$ 次，设 $X$ 表示摸到红球的次数，则 $EX=$（　）．

;;;
A. $\dfrac{2}{5}$
B. $\dfrac{8}{5}$
C. $\dfrac{12}{5}$
D. $\dfrac{48}{5}$
;;;C
***
依题设，可知试验为有放回摸球，故每次摸到红球的概率为 $\dfrac{3}{5}$，所以 $X\sim B\left(4,\dfrac{3}{5}\right)$，故

$$EX=np=4\times\frac{3}{5}=\frac{12}{5}.$$

+++

#### 基础填空 (1) 一袋中有 $N$ 个球，其中白球数目 $X$ 是一个随机变量，且 $EX=n$，从袋中任取一球，则取得的球是白球的概率为 ________．
***
$\dfrac{n}{N}$．

设 $A=\{$取得一球为白球$\}$，依题意，有 $P\{A\mid X=k\}=\dfrac{k}{N}$，$X$ 的取值可能为 $\{0,1,2,\cdots,N\}$，由全概率公式，得

$$P(A)=\sum_{k=0}^{N}P\{X=k\}\cdot P\{A\mid X=k\}=\frac{1}{N}\sum_{k=0}^{N}kP\{X=k\}=\frac{EX}{N}=\frac{n}{N}.$$

+++

#### 基础填空 (2) 设随机变量 $X$ 的概率密度为 $f(x)=\dfrac{1}{\sqrt{\pi}}\mathrm{e}^{-x^2+2x-1}\ (-\infty<x<+\infty)$，则 $E(X^2)=$ ________．
***
$\dfrac{3}{2}$．

由

$$f(x)=\frac{1}{\sqrt{\pi}}\mathrm{e}^{-x^2+2x-1}=\frac{1}{\sqrt{2\pi}\cdot\dfrac{1}{\sqrt{2}}}\mathrm{e}^{-\frac{(x-1)^2}{2\cdot\frac{1}{2}}},$$

知 $X\sim N\left(1,\dfrac{1}{2}\right)$，故 $EX=1$，$DX=\dfrac{1}{2}$，所以

$$E(X^2)=DX+(EX)^2=\frac{1}{2}+1^2=\frac{3}{2}.$$

+++

#### 基础填空 (3) 从 $1,2,3,4,5$ 中任取一数 $X$，再从 $1,\cdots,X$ 中任取一数 $Y$，则 $EY=$ ________．
***
$2$．

先求 $Y$ 的分布律．$Y$ 的所有可能取值为 $1,2,3,4,5$，由全概率公式得

$$P\{Y=k\}=\sum_{i=1}^{k}P\{X=i\}\cdot P\{Y=k\mid X=i\}=\frac{1}{5}\sum_{i=k}^{5}\frac{1}{i}\ (k=1,2,\cdots 5),$$

故

$$EY=\sum_{k=1}^{5}k\cdot P\{Y=k\}=\sum_{k=1}^{5}\left(k\cdot\frac{1}{5}\sum_{i=k}^{5}\frac{1}{i}\right)=2.$$

+++

#### 基础填空 (4) 设随机变量 $X$ 的分布函数 $F(x)=0.3\Phi\left(\dfrac{x-4}{2}\right)+0.7\Phi\left(\dfrac{x+1}{3}\right)$，其中 $\Phi(x)$ 为标准正态分布的分布函数，则 $EX=$ ________．
***
$0.5$．

先求 $X$ 的概率密度，再求 $EX$．

$$f(x)=F'(x)=0.3\varphi\left(\frac{x-4}{2}\right)\cdot\frac{1}{2}+0.7\varphi\left(\frac{x+1}{3}\right)\cdot\frac{1}{3},$$

其中 $\varphi(x)$ 为 $X\sim N(0,1)$ 的概率密度．

$$EX=\int_{-\infty}^{+\infty}xf(x)\mathrm{d}x=\int_{-\infty}^{+\infty}0.3\cdot\frac{1}{2}\cdot x\varphi\left(\frac{x-4}{2}\right)\mathrm{d}x+\int_{-\infty}^{+\infty}0.7\cdot\frac{1}{3}\cdot x\varphi\left(\frac{x+1}{3}\right)\mathrm{d}x$$

$$=0.3\times\frac{1}{2}\int_{-\infty}^{+\infty}(2t+4)\varphi(t)\cdot 2\mathrm{d}t+0.7\times\frac{1}{3}\int_{-\infty}^{+\infty}(3t-1)\varphi(t)\cdot 3\mathrm{d}t$$

$$=0.3\times 4+0.7\times(-1)=0.5.$$

【注】① $\displaystyle\int_{-\infty}^{+\infty}t\varphi(t)\mathrm{d}t=\mu=0$．

② 设 $X\sim N(\mu,\sigma^2)\ (\sigma>0)$，则分布函数

$$F(x)=P\{X\leqslant x\}=P\left\{\frac{X-\mu}{\sigma}\leqslant\frac{x-\mu}{\sigma}\right\}=\Phi\left(\frac{x-\mu}{\sigma}\right),$$

即分布函数为 $\Phi\left(\dfrac{x-\mu}{\sigma}\right)$，相应随机变量 $X$，有 $EX=\mu$．

③ 一般结论：若 $F(x)=k_1\Phi\left(\dfrac{x-\mu_1}{\sigma_1}\right)+k_2\Phi\left(\dfrac{x-\mu_2}{\sigma_2}\right)$，当 $k_1+k_2=1$ 时，有 $EX=k_1\mu_1+k_2\mu_2$．

+++

#### 基础填空 (5) 设 $(X,Y)\sim N(\mu_1,\mu_2,\sigma^2,\sigma^2;\rho)$，若 $\dfrac{3X+Y}{2}$ 与 $\dfrac{X-2Y}{3}$ 不相关，则相关系数 $\rho=$ ________．
***
$\dfrac{1}{5}$．

由于

$$\mathrm{Cov}\left(\frac{3X+Y}{2},\frac{X-2Y}{3}\right)=\frac{1}{6}\mathrm{Cov}(3X+Y,X-2Y)$$

$$=\frac{1}{6}\left[3\mathrm{Cov}(X,X)+\mathrm{Cov}(Y,X)-6\mathrm{Cov}(X,Y)-2\mathrm{Cov}(Y,Y)\right]$$

$$=\frac{1}{6}\left[3DX-5\mathrm{Cov}(X,Y)-2DY\right]$$

$$=\frac{1}{6}\left(3\sigma^2-5\rho\sigma^2-2\sigma^2\right)=\frac{1}{6}\sigma^2(1-5\rho)=0,$$

故 $\rho=\dfrac{1}{5}$．

+++

#### 基础解答 (1) 设 $X$ 与 $Y$ 的概率分布分别为

| $X$ | $0$ | $1$ |
| --- | --- | --- |
| $p$ | $\dfrac{1}{3}$ | $\dfrac{2}{3}$ |

| $Y$ | $-1$ | $0$ | $1$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{1}{3}$ | $\dfrac{1}{3}$ | $\dfrac{1}{3}$ |

且 $P\{X^2=Y^2\}=1$．\
（Ⅰ）求 $(X,Y)$ 的概率分布；\
（Ⅱ）求 $\rho_{XY}$．
***
（Ⅰ）由 $P\{X^2=Y^2\}=1$，知 $P\{X^2\neq Y^2\}=0$，故

$$P\{X=0,Y=-1\}=P\{X=0,Y=1\}=P\{X=1,Y=0\}=0.$$

又

$$P\{X=1,Y=-1\}=P\{X=0,Y=0\}=P\{X=1,Y=1\}=\frac{1}{3},$$

故 $(X,Y)$ 的联合概率分布为

| $Y\ \backslash\ X$ | $0$ | $1$ |
| --- | --- | --- |
| $-1$ | $0$ | $\dfrac{1}{3}$ |
| $0$ | $\dfrac{1}{3}$ | $0$ |
| $1$ | $0$ | $\dfrac{1}{3}$ |

（Ⅱ）由（Ⅰ），知 $XY$ 的概率分布为

| $XY$ | $-1$ | $0$ | $1$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{1}{3}$ | $\dfrac{1}{3}$ | $\dfrac{1}{3}$ |

故 $E(XY)=0$．

又 $EX=\dfrac{2}{3}$，$EY=0$，故 $\mathrm{Cov}(X,Y)=E(XY)-EX\cdot EY=0$，所以 $\rho_{XY}=0$．

+++

#### 基础解答 (2) 设随机变量 $X,Y,Z$，满足 $EX=EY=1$，$EZ=-1$，$DX=DY=DZ=1$，$\rho_{XY}=0$，$\rho_{XZ}=\dfrac{1}{2}$，$\rho_{YZ}=-\dfrac{1}{2}$，求 $E(X+Y-2Z)$，$D(X+Y+Z)$．
***
$$E(X+Y-2Z)=EX+EY-2EZ=1+1-2\times(-1)=4,$$

$$D(X+Y+Z)=DX+DY+DZ+2\mathrm{Cov}(X,Y)+2\mathrm{Cov}(X,Z)+2\mathrm{Cov}(Y,Z).$$

$$\mathrm{Cov}(X,Y)=\sqrt{DX\cdot DY}\cdot\rho_{XY}=1\times 0=0,$$

$$\mathrm{Cov}(X,Z)=\sqrt{DX\cdot DZ}\cdot\rho_{XZ}=1\times\frac{1}{2}=\frac{1}{2},$$

$$\mathrm{Cov}(Y,Z)=\sqrt{DY\cdot DZ}\cdot\rho_{YZ}=1\times\left(-\frac{1}{2}\right)=-\frac{1}{2},$$

故

$$D(X+Y+Z)=1+1+1+0+2\times\frac{1}{2}+2\times\left(-\frac{1}{2}\right)=3.$$

+++

#### 基础解答 (3) 设 $X$ 与 $Y$ 相互独立，且均服从 $N\left(1,\dfrac{1}{2}\right)$，求 $D(|X-Y|)$．
***
由 $X,Y$ 相互独立，可知

$$Z=X-Y\sim N\left(1-1,\frac{1}{2}+\frac{1}{2}\right),$$

即 $Z\sim N(0,1)$．

$$E(|Z|)=\int_{-\infty}^{+\infty}|z|\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{z^2}{2}}\mathrm{d}z=2\int_{0}^{+\infty}\frac{1}{\sqrt{2\pi}}z\mathrm{e}^{-\frac{z^2}{2}}\mathrm{d}z$$

$$=\frac{\sqrt{2}}{\sqrt{\pi}}\left[2\int_{0}^{+\infty}\left(\frac{z}{\sqrt{2}}\right)^{2-1}\cdot\mathrm{e}^{-\left(\frac{z}{\sqrt{2}}\right)^2}\mathrm{d}\left(\frac{z}{\sqrt{2}}\right)\right]=\frac{\sqrt{2}}{\sqrt{\pi}}\Gamma(1)=\sqrt{\frac{2}{\pi}},$$

$$E(|Z|^2)=E(Z^2)=DZ+(EZ)^2=1+0=1,$$

故

$$D(|X-Y|)=D(|Z|)=E(|Z|^2)-\left[E(|Z|)\right]^2=1-\frac{2}{\pi}.$$

【注】① 计算 $\displaystyle\int_{0}^{+\infty}\frac{1}{\sqrt{2\pi}}z\mathrm{e}^{-\frac{z^2}{2}}\mathrm{d}z$ 可以凑微分，也可用 $\Gamma$ 函数：

$$\Gamma(\alpha)=\int_{0}^{+\infty}x^{\alpha-1}\cdot\mathrm{e}^{-x}\mathrm{d}x\xrightarrow{\ \diamondsuit\ x=y^2\ }2\int_{0}^{+\infty}y^{2\alpha-1}\mathrm{e}^{-y^2}\mathrm{d}y,$$

$$\Gamma(1)=1,\quad\Gamma\left(\frac{1}{2}\right)=\sqrt{\pi},$$

$$\Gamma(\alpha+1)=\alpha\Gamma(\alpha),\quad\Gamma(n+1)=n!\ (n\ \text{为正整数}).$$

② 本题若用二维随机变量函数的期望公式

$$E(|X-Y|)=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}|x-y|f_X(x)f_Y(y)\mathrm{d}x\mathrm{d}y,$$

计算量较大．

+++

#### 基础解答 (4) 设 $X$ 的概率密度为 $f(x)=\dfrac{1}{2}\mathrm{e}^{-|x|}$，$-\infty<x<+\infty$．

（Ⅰ）求 $EX$ 和 $DX$；\
（Ⅱ）求 $\mathrm{Cov}(X,|X|)$，并判别 $X$ 与 $|X|$ 是否不相关；\
（Ⅲ）问 $X$ 与 $|X|$ 是否相互独立？
***
（Ⅰ）

$$EX=\int_{-\infty}^{+\infty}xf(x)\mathrm{d}x=\int_{-\infty}^{+\infty}x\cdot\frac{1}{2}\mathrm{e}^{-|x|}\mathrm{d}x=0\ (\text{奇函数}),$$

$$DX=E(X^2)-(EX)^2=E(X^2)=\int_{-\infty}^{+\infty}x^2f(x)\mathrm{d}x=2\int_{0}^{+\infty}x^2\cdot\frac{1}{2}\mathrm{e}^{-x}\mathrm{d}x=2.$$

（Ⅱ）

$$\mathrm{Cov}(X,|X|)=E(X|X|)-EX\cdot E(|X|)=E(X|X|).$$

而

$$E(X|X|)=\int_{-\infty}^{+\infty}x|x|f(x)\mathrm{d}x=\int_{-\infty}^{+\infty}x|x|\frac{1}{2}\mathrm{e}^{-|x|}\mathrm{d}x=0,$$

故 $\mathrm{Cov}(X,|X|)=0$，即 $X$ 与 $|X|$ **不相关**．

（Ⅲ）对任意给定的 $0<a<+\infty$，显然事件 $\{|X|\leqslant a\}$ 包含于事件 $\{X\leqslant a\}$，且

$$P\{X\leqslant a\}<1,\quad P\{|X|\leqslant a\}>0,$$

故

$$P\{X\leqslant a,|X|\leqslant a\}=P\{|X|\leqslant a\}.$$

但

$$P\{X\leqslant a\}\cdot P\{|X|\leqslant a\}<P\{|X|\leqslant a\},$$

从而

$$P\{X\leqslant a,|X|\leqslant a\}\neq P\{X\leqslant a\}\cdot P\{|X|\leqslant a\},$$

因此，$X$ 与 $|X|$ **不相互独立**．

【注】① 本题验证 $X$ 与 $|X|$ 不相互独立，是用定义证明的，若用两个随机变量 $X$ 与 $Y$ 的联合概率密度 $f(x,y)$ 是否等于 $f_X(x)\cdot f_Y(y)$ 来证明，则会带来烦琐的计算．

② 本题也可看出：$X,Y$ 不相关 $\nRightarrow X,Y$ 相互独立．

+++

#### 基础解答 (5) 设随机变量 $X$ 与 $Y$ 相互独立，$P\{Y=-1\}=\dfrac{1}{4}$，$P\{Y=1\}=\dfrac{3}{4}$，$X\sim N(0,1)$．

（Ⅰ）求 $Z=XY$ 的概率密度；\
（Ⅱ）求 $\mathrm{Cov}(Z,X)$．
***
（Ⅰ）用定义法．

$$F_Z(z)=P\{XY\leqslant z\}=P\{XY\leqslant z,Y=-1\}+P\{XY\leqslant z,Y=1\}$$

$$=P\{-X\leqslant z,Y=-1\}+P\{X\leqslant z,Y=1\}$$

$$=P\{Y=-1\}\cdot P\{X\geqslant-z\}+P\{Y=1\}\cdot P\{X\leqslant z\}$$

$$=\frac{1}{4}\left(1-P\{X<-z\}\right)+\frac{3}{4}P\{X\leqslant z\}$$

$$=\frac{1}{4}\left[1-\Phi(-z)\right]+\frac{3}{4}\Phi(z)=\frac{1}{4}\Phi(z)+\frac{3}{4}\Phi(z)=\Phi(z),$$

故 $Z=XY$ 服从标准正态分布，其概率密度为

$$f_Z(z)=\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{z^2}{2}},\quad-\infty<z<+\infty.$$

（Ⅱ）

$$\mathrm{Cov}(Z,X)=\mathrm{Cov}(XY,X)=E(XY\cdot X)-E(XY)\cdot EX=E(X^2Y)-EX\cdot EY\cdot EX.$$

又 $EX=0$，$E(X^2Y)=E(X^2)\cdot EY$（$X^2$ 与 $Y$ 相互独立），

$$E(X^2)=DX+(EX)^2=1,\quad EY=(-1)\times\frac{1}{4}+1\times\frac{3}{4}=\frac{1}{2},$$

故

$$\mathrm{Cov}(Z,X)=1\times\frac{1}{2}-0=\frac{1}{2}.$$

+++

#### 基础解答 (6) 设 $X\sim N(1,1)$，$Y\sim N(-2,1)$，且 $X$ 与 $Y$ 相互独立．

（Ⅰ）求 $Z=2X+Y$ 的概率密度；\
（Ⅱ）求 $E(|2X+Y|)$，$D(|2X+Y|)$．
***
（Ⅰ）由 $X,Y$ 相互独立，知 $2X+Y\sim N(2\times 1-2,2^2+1^2)$，即 $Z\sim N(0,5)$，故 $Z=2X+Y$ 的概率密度为

$$f_Z(z)=\frac{1}{\sqrt{10\pi}}\mathrm{e}^{-\frac{z^2}{10}},\quad-\infty<z<+\infty.$$

（Ⅱ）

$$E(|2X+Y|)=E(|Z|)=\frac{1}{\sqrt{10\pi}}\int_{-\infty}^{+\infty}\mathrm{e}^{-\frac{z^2}{10}}|z|\mathrm{d}z=\frac{2}{\sqrt{10\pi}}\int_{0}^{+\infty}z\mathrm{e}^{-\frac{z^2}{10}}\mathrm{d}z=\sqrt{\frac{10}{\pi}},$$

$$D(|2X+Y|)=D(|Z|)=E(|Z|^2)-\left[E(|Z|)\right]^2=E(Z^2)-\left[E(|Z|)\right]^2.$$

而 $E(Z^2)=DZ+(EZ)^2=5+0=5$，所以 $D(|2X+Y|)=5-\dfrac{10}{\pi}$．

+++

#### 基础解答 (7) 设二维随机变量 $(X,Y)$ 服从区域 $D=\{(x,y)\mid 0\leqslant x\leqslant 2,0\leqslant y\leqslant 2\}$ 上的均匀分布．

（Ⅰ）求 $Z=X+Y$ 的概率密度；\
（Ⅱ）求 $E(Z^2)$．
***
（Ⅰ）依题设，$(X,Y)$ 的概率密度为

$$f(x,y)=\begin{cases}\dfrac{1}{4},&(x,y)\in D,\\0,&\text{其他},\end{cases}\qquad F_Z(z)=P\{Z\leqslant z\}=P\{X+Y\leqslant z\}.$$

考虑到 $f(x,y)$ 的非零部分取值为常数 $\dfrac{1}{4}$，可用面积来计算 $P\{X+Y\leqslant z\}$，

$$F_Z(z)=P\{X+Y\leqslant z\}=\begin{cases}0,&z<0,\\\dfrac{S_{D_1}}{S_D},&0\leqslant z<2,\\\dfrac{S_D-S_{D_2}}{S_D},&2\leqslant z<4,\\1,&z\geqslant 4\end{cases}=\begin{cases}0,&z<0,\\\dfrac{z^2}{8},&0\leqslant z<2,\\1-\dfrac{(4-z)^2}{8},&2\leqslant z<4,\\1,&z\geqslant 4,\end{cases}$$

故

$$f_Z(z)=F_Z'(z)=\begin{cases}\dfrac{z}{4},&0<z\leqslant 2,\\1-\dfrac{z}{4},&2<z\leqslant 4,\\0,&\text{其他}.\end{cases}$$

（Ⅱ）

$$E(Z^2)=\int_{-\infty}^{+\infty}z^2\cdot f_Z(z)\mathrm{d}z=\int_{0}^{2}\frac{z^3}{4}\mathrm{d}z+\int_{2}^{4}\left(z^2-\frac{z^3}{4}\right)\mathrm{d}z=\frac{14}{3}.$$

【注】由题目条件可判别 $(X,Y)$ 的两个分量 $X$ 与 $Y$ 相互独立（见《李林考研数学系列概率论与数理统计辅导讲义》），且均服从 $[0,2]$ 上的均匀分布，故

$$EX=EY=\frac{2+0}{2}=1,$$

$$DX=DY=\frac{1}{3},\quad E(X+Y)=2,$$

$$D(X+Y)=DX+DY=\frac{2}{3},$$

故

$$E(Z^2)=E\left[(X+Y)^2\right]=D(X+Y)+\left[E(X+Y)\right]^2=\frac{2}{3}+4=\frac{14}{3}.$$

+++

#### 综合选择 (1) 设对任意两个随机变量 $X$ 与 $Y$，有 $E(XY)=EX\cdot EY$，则（　）．

;;;
A. $X$ 与 $Y$ 相互独立
B. $X$ 与 $Y$ 不相互独立
C. $D(X+Y)=DX+DY$
D. $D(XY)=DX\cdot DY$
;;;C
***
$E(XY)=EX\cdot EY\Leftrightarrow X,Y$ 不相关，不一定能得 $X,Y$ 相互独立，故排除 A，B．

而 $D(X+Y)=DX+DY\Leftrightarrow X,Y$ 不相关 $\Leftrightarrow E(XY)=EX\cdot EY$，故 **C** 正确．

$$D(XY)=E\left[(XY)^2\right]-\left[E(XY)\right]^2=E\left[(XY)^2\right]-(EX\cdot EY)^2,$$

$$DX\cdot DY=\left[E(X^2)-(EX)^2\right]\left[E(Y^2)-(EY)^2\right]$$

$$=E(X^2)\cdot E(Y^2)-E(X^2)(EY)^2-(EX)^2E(Y^2)+(EX)^2(EY)^2,$$

故 D 不一定成立．

【注】当 $X,Y$ 相互独立时，有结论：

$$D(XY)=DXDY+(EX)^2DY+(EY)^2DX.$$

事实上，由 $X,Y$ 相互独立，知 $X^2$ 与 $Y^2$ 相互独立（反之不一定成立），故

$$D(XY)=E\left[(XY)^2\right]-\left[E(XY)\right]^2=E(X^2)\cdot E(Y^2)-(EX)^2\cdot(EY)^2$$

$$=\left[DX+(EX)^2\right]\left[DY+(EY)^2\right]-(EX)^2\cdot(EY)^2$$

$$=DXDY+(EX)^2DY+(EY)^2DX.$$

+++

#### 综合选择 (2) 设 $X\sim N(0,1)$，$Y=X^2+X+1$，则 $X$ 与 $Y$（　）．

;;;
A. 相关且相互不独立
B. 相关且相互独立
C. 不相关且相互独立
D. 不相关且相互不独立
;;;A
***
判别 $X$ 与 $Y$ 是否相关，需计算 $\mathrm{Cov}(X,Y)$．

由 $X\sim N(0,1)$，知

$$EX=0,\quad DX=1,\quad E(X^2)=DX+(EX)^2=1,\quad E(X^3)=0,$$

$$E(XY)=E\left[X(X^2+X+1)\right]=E(X^3)+E(X^2)+EX=0+1+0=1,$$

所以

$$\mathrm{Cov}(X,Y)=E(XY)-EXEY=1-0=1\neq 0,$$

故 $X$ 与 $Y$ 不是不相关，即 $X$ 与 $Y$ **相关**，由此知 $X$ 与 $Y$ 一定**不独立**．

【注】① 由 $X,Y$ 独立 $\Rightarrow X,Y$ 不相关（反之不一定成立），根据逆否命题，若 $X$ 与 $Y$ 相关，则 $X,Y$ 不独立．

② 若 $(X,Y)$ 服从二维正态分布，则 $X,Y$ 相互独立 $\Leftrightarrow X,Y$ 不相关．

③ 注意到 ① 中的"不一定"，既不相关又不独立的两个随机变量是存在的．

事实上，$X$ 与 $Y$ 不相关，只能说明 $X$ 与 $Y$ 没有线性关系，至于 $X$ 与 $Y$ 是否独立，要视具体情况．

+++

#### 综合选择 (3) 设随机变量 $X$ 与 $Y$ 相关，相关系数为 $\rho_{XY}$，$Z=aX+b$（$a,b$ 为常数），则 $\rho_{YZ}=\rho_{XY}$ 的充分必要条件为（　）．

;;;
A. $a>0$
B. $a<0$
C. $a\neq 0$
D. $a=1$
;;;A
***
$\rho_{YZ}=\dfrac{\mathrm{Cov}(Y,Z)}{\sqrt{DY}\cdot\sqrt{DZ}}$．又

$$\mathrm{Cov}(Y,Z)=\mathrm{Cov}(Y,aX+b)=a\mathrm{Cov}(X,Y),$$

$$DZ=D(aX+b)=a^2DX,$$

故

$$\rho_{YZ}=\frac{a\mathrm{Cov}(X,Y)}{\sqrt{DY}\sqrt{a^2DX}}=\frac{a}{|a|}\rho_{XY}.$$

又 $X,Y$ 相关，知 $\rho_{XY}\neq 0$，所以 $\rho_{YZ}=\rho_{XY}\Leftrightarrow\dfrac{a}{|a|}=1$，即 $a>0$．

+++

#### 综合选择 (4) 设随机变量 $X$ 在 $\left[0,\dfrac{\pi}{2}\right]$ 上服从均匀分布，$U=\sin X$，$V=\cos X$，则 $U$ 与 $V$ 的相关系数 $\rho_{UV}$ 为（　）．

;;;
A. $\rho_{UV}=0$
B. $|\rho_{UV}|=1$
C. $0<\rho_{UV}<1$
D. $-1<\rho_{UV}<0$
;;;D
***
由 $X\sim U\left[0,\dfrac{\pi}{2}\right]$，知 $X$ 的概率密度为

$$f(x)=\begin{cases}\dfrac{2}{\pi},&0\leqslant x\leqslant\dfrac{\pi}{2},\\0,&\text{其他},\end{cases}$$

故

$$EU=\int_{-\infty}^{+\infty}f(x)\sin x\mathrm{d}x=\int_{0}^{\frac{\pi}{2}}\frac{2}{\pi}\sin x\mathrm{d}x=\frac{2}{\pi},$$

$$E(U^2)=\int_{-\infty}^{+\infty}f(x)\sin^2x\mathrm{d}x=\int_{0}^{\frac{\pi}{2}}\frac{2}{\pi}\sin^2x\mathrm{d}x=\frac{1}{2},$$

$$DU=E(U^2)-(EU)^2=\frac{1}{2}-\frac{4}{\pi^2}.$$

同理，可得 $EV=\dfrac{2}{\pi}$，$DV=\dfrac{1}{2}-\dfrac{4}{\pi^2}$．又

$$E(UV)=\int_{0}^{\frac{\pi}{2}}\frac{2}{\pi}\sin x\cos x\mathrm{d}x=\frac{1}{\pi},$$

$$\mathrm{Cov}(U,V)=E(UV)-EU\cdot EV=\frac{1}{\pi}-\frac{4}{\pi^2}<0,$$

故

$$-1<\rho_{UV}=\frac{\mathrm{Cov}(U,V)}{\sqrt{DU}\cdot\sqrt{DV}}<0.$$

+++

#### 综合填空 (1) 设随机变量 $X$ 的概率分布为 $P\{X=k\}=\dfrac{C}{k!}\ (k=0,1,2,\cdots)$，则 $E(X^2)=$ ________．
***
$2$．

根据概率分布的性质，$\displaystyle\sum_{k=0}^{\infty}\frac{C}{k!}=C\mathrm{e}=1$，可得 $C=\mathrm{e}^{-1}$．

注意到 $X$ 服从泊松分布，

$$P\{X=k\}=\frac{\lambda^k}{k!}\mathrm{e}^{-\lambda}\ (k=0,1,2,\cdots),$$

对比 $P\{X=k\}=\dfrac{\mathrm{e}^{-1}}{k!}\ (k=0,1,2,\cdots)$，知 $\lambda=1$，即 $X\sim P(1)$，故

$$EX=DX=\lambda=1,$$

所以

$$E(X^2)=DX+(EX)^2=1+1^2=2.$$

【注】常用分布的期望、方差公式应记住，利用方差公式 $DX=E(X^2)-(EX)^2$ 求 $E(X^2)$ 是常用方法．

+++

#### 综合填空 (2) 设随机变量 $X$ 在 $(0,a)\ (a\leqslant 12)$ 上服从均匀分布，则 $X$ 位于 $EX$ 与 $DX$ 之间的概率为 ________．
***
$\left|\dfrac{1}{2}-\dfrac{a}{12}\right|$．

由已知，$X\sim U(0,a)$，则 $EX=\dfrac{a}{2}$，$DX=\dfrac{a^2}{12}$．

当 $6<a\leqslant 12$ 时，$P\left\{\dfrac{a}{2}<X<\dfrac{a^2}{12}\right\}=\displaystyle\int_{\frac{a}{2}}^{\frac{a^2}{12}}\frac{1}{a}\mathrm{d}x=\frac{a}{12}-\frac{1}{2}$；

当 $a\leqslant 6$ 时，$P\left\{\dfrac{a^2}{12}<X<\dfrac{a}{2}\right\}=\dfrac{1}{2}-\dfrac{a}{12}$，故所求概率为 $\left|\dfrac{1}{2}-\dfrac{a}{12}\right|$．

+++

#### 综合填空 (3) 设随机变量 $X_1,X_2,\cdots,X_n$ 独立同分布，且有相同的概率密度，则概率 $P\{X_n>\min\{X_1,X_2,\cdots,X_{n-1}\}\}=$ ________．
***
$1-\dfrac{1}{n}$．

由已知，$X_n$ 与 $Y=\min\{X_1,X_2,\cdots,X_{n-1}\}$ 相互独立，且 $X_1,X_2,\cdots,X_n$ 独立同分布，记其分布函数分别为 $F_1(x),F_2(x),\cdots,F_n(x)$，概率密度分别为 $f_1(x),f_2(x),\cdots,f_n(x)$，则

$$F_Y(y)=P\{Y\leqslant y\}=P\{\min\{X_1,X_2,\cdots,X_{n-1}\}\leqslant y\}$$

$$=1-P\{X_1>y\}\cdot P\{X_2>y\}\cdot\cdots\cdot P\{X_{n-1}>y\}$$

$$=1-\left[1-F_1(y)\right]^{n-1},$$

故 $f_Y(y)=F_Y'(y)=(n-1)\left[1-F_1(y)\right]^{n-2}\cdot f_1(y)$，所以

$$P\{X_n>Y\}=\iint\limits_{x>y}f_n(x)(n-1)f_1(y)\left[1-F_1(y)\right]^{n-2}\mathrm{d}x\mathrm{d}y$$

$$=\int_{-\infty}^{+\infty}f_n(x)\mathrm{d}x\int_{-\infty}^{x}(n-1)f_1(y)\left[1-F_1(y)\right]^{n-2}\mathrm{d}y$$

$$=\int_{-\infty}^{+\infty}f_n(x)\left\{-\left[1-F_1(y)\right]^{n-1}\Big|_{-\infty}^{x}\right\}\mathrm{d}x$$

$$=\int_{-\infty}^{+\infty}\left\{1-\left[1-F_1(x)\right]^{n-1}\right\}f_n(x)\mathrm{d}x$$

$$=1+\frac{\left[1-F_1(x)\right]^n}{n}\bigg|_{-\infty}^{+\infty}=1-\frac{1}{n}.$$

+++

#### 综合填空 (4) 设随机变量 $X$ 的概率密度为 $f(x)=\dfrac{1}{\pi(1+x^2)}$，则 $E(\min\{|x|,1\})=$ ________．
***
$\dfrac{1}{\pi}\ln 2+\dfrac{1}{2}$．

用期望的定义计算．

$$E(\min\{|x|,1\})=\int_{-\infty}^{+\infty}\min\{|x|,1\}\cdot f(x)\mathrm{d}x.$$

当 $|x|\leqslant 1$ 时，$\min\{|x|,1\}=|x|$；当 $|x|\geqslant 1$ 时，$\min\{|x|,1\}=1$，所以

$$\int_{-\infty}^{+\infty}\min\{|x|,1\}f(x)\mathrm{d}x=\frac{1}{\pi}\left[\int_{-1}^{1}\frac{|x|}{1+x^2}\mathrm{d}x+\int_{-\infty}^{-1}\frac{\mathrm{d}x}{1+x^2}+\int_{1}^{+\infty}\frac{\mathrm{d}x}{1+x^2}\right]$$

$$=\frac{2}{\pi}\left[\int_{0}^{1}\frac{x}{1+x^2}\mathrm{d}x+\int_{1}^{+\infty}\frac{\mathrm{d}x}{1+x^2}\right]=\frac{1}{\pi}\ln 2+\frac{1}{2}.$$

+++

#### 综合填空 (5) 设 $15\,000$ 件产品中有 $1\,000$ 件次品，从中任取 $150$ 件进行检测，则检测到次品数 $X$ 的期望 $EX=$ ________．
***
$10$．

令 $X_i=\begin{cases}1,&\text{第 }i\text{ 件产品为次品},\\0,&\text{第 }i\text{ 件产品为正品},\end{cases}\ (i=1,2,\cdots,150)$，则

$$X=X_1+X_2+\cdots+X_{150}.$$

又因 $X_i$ 的分布律为

| $X_i$ | $0$ | $1$ |
| --- | --- | --- |
| $p$ | $\dfrac{14}{15}$ | $\dfrac{1}{15}$ |

$(i=1,2,\cdots,150)$，所以 $EX_i=\dfrac{1}{15}$，故

$$EX=\sum_{i=1}^{150}EX_i=150\times\frac{1}{15}=10.$$

+++

#### 综合填空 (6) 设 $(X,Y)\sim N(1,1,2,2;0)$，$U=X+2Y$，$V=X-2Y$，则 $\rho_{UV}=$ ________．
***
$-\dfrac{3}{5}$．

由题意，可知 $X\sim N(1,2)$，$Y\sim N(1,2)$，$\rho_{XY}=0$，于是

$$EX=EY=1,\quad DX=DY=2,$$

且 $X$ 与 $Y$ 相互独立．

由于 $\rho_{UV}=\dfrac{\mathrm{Cov}(U,V)}{\sqrt{DU}\sqrt{DV}}$，其中

$$\mathrm{Cov}(U,V)=\mathrm{Cov}(X+2Y,X-2Y)$$

$$=\mathrm{Cov}(X,X)-2\mathrm{Cov}(X,Y)+2\mathrm{Cov}(Y,X)-4\mathrm{Cov}(Y,Y)$$

$$=\mathrm{Cov}(X,X)-4\mathrm{Cov}(Y,Y)=DX-4DY=2-4\times 2=-6,$$

$$DU=D(X+2Y)=DX+4DY=2+4\times 2=10,$$

$$DV=D(X-2Y)=DX+4DY=2+4\times 2=10,$$

故

$$\rho_{UV}=\frac{-6}{\sqrt{10}\times\sqrt{10}}=-\frac{3}{5}.$$

+++

#### 综合解答 (1) 在区间 $(0,1)$ 内随机取 $n$ 个数 $X_1,X_2,\cdots,X_n$．

（Ⅰ）求最大数与最小数之间距离 $d$ 的数学期望；\
（Ⅱ）若用 $Y$ 表示 $n$ 个数中大于 $\dfrac{2}{3}$ 的个数，求 $EY$ 和 $DY$．
***
（Ⅰ）依题设，$X_i\ (i=1,2,\cdots,n)$ 相互独立，且都在 $(0,1)$ 上服从均匀分布，其概率密度为

$$f(x)=\begin{cases}1,&0<x<1,\\0,&\text{其他},\end{cases}$$

其分布函数为

$$F(x)=\begin{cases}0,&x\leqslant 0,\\x,&0<x<1,\\1,&x\geqslant 1.\end{cases}$$

$$d=\max\{X_1,X_2,\cdots,X_n\}-\min\{X_1,X_2,\cdots,X_n\}\xlongequal{\text{记}}X_{(n)}-X_{(1)},$$

其中 $X_{(n)}$ 的概率密度为

$$f_{(n)}(x)=n\left[F(x)\right]^{n-1}\cdot f(x)=\begin{cases}nx^{n-1},&0<x<1,\\0,&\text{其他},\end{cases}$$

$X_{(1)}$ 的概率密度为

$$f_{(1)}(x)=n\left[1-F(x)\right]^{n-1}\cdot f(x)=\begin{cases}n(1-x)^{n-1},&0<x<1,\\0,&\text{其他},\end{cases}$$

故

$$EX_{(n)}=\int_{-\infty}^{+\infty}x\cdot f_{(n)}(x)\mathrm{d}x=\int_{0}^{1}x\cdot nx^{n-1}\mathrm{d}x=\frac{n}{n+1},$$

$$EX_{(1)}=\int_{-\infty}^{+\infty}x\cdot f_{(1)}(x)\mathrm{d}x=\int_{0}^{1}x\cdot n(1-x)^{n-1}\mathrm{d}x=\frac{1}{n+1},$$

所以

$$Ed=EX_{(n)}-EX_{(1)}=\frac{n}{n+1}-\frac{1}{n+1}=\frac{n-1}{n+1}.$$

（Ⅱ）先求 $Y$ 的分布，用 $X$ 表示在 $(0,1)$ 内任取的数，则 $X$ 在 $(0,1)$ 内服从均匀分布，其概率密度为

$$f(x)=\begin{cases}1,&0<x<1,\\0,&\text{其他}.\end{cases}$$

记 $A=\left\{X>\dfrac{2}{3}\right\}$，则 $P(A)=P\left\{X>\dfrac{2}{3}\right\}=\displaystyle\int_{\frac{2}{3}}^{1}1\mathrm{d}x=\frac{1}{3}$．

由已知，$Y\sim B\left(n,\dfrac{1}{3}\right)$，所以

$$EY=n\cdot p=\frac{n}{3},\quad DY=np(1-p)=\frac{2n}{9}.$$

【注】设 $X_1,X_2,\cdots,X_n$ 独立同分布，其分布函数为 $F(x)$，则\
① $\max\{X_1,X_2,\cdots,X_n\}$ 的分布函数为 $\left[F(x)\right]^n$；\
② $\min\{X_1,X_2,\cdots,X_n\}$ 的分布函数为 $1-\left[1-F(x)\right]^n$．

+++

#### 综合解答 (2) 设 $X_1,X_2,\cdots,X_n\ (n>2)$ 为独立同分布的随机变量，且均服从 $N(0,1)$，$Y_i=X_i-\overline{X}\ (i=1,2,\cdots,n)$，其中 $\overline{X}=\dfrac{1}{n}\displaystyle\sum_{i=1}^{n}X_i$．

（Ⅰ）求 $DY_i\ (i=1,2,\cdots n)$；\
（Ⅱ）求 $\rho_{Y_1Y_n}$．
***
（Ⅰ）

$$DY_i=D(X_i-\overline{X})=D\left(X_i-\frac{1}{n}\sum_{i=1}^{n}X_i\right)=D\left[\left(1-\frac{1}{n}\right)X_i-\frac{1}{n}\sum_{k\neq i}^{n}X_k\right]$$

$$=\left(\frac{n-1}{n}\right)^2DX_i+\frac{1}{n^2}\sum_{k\neq i}^{n}DX_k=\left(\frac{n-1}{n}\right)^2\cdot 1+\frac{1}{n^2}\cdot(n-1)=\frac{n-1}{n},$$

这里利用了 $X_i$ 与 $\displaystyle\sum_{k\neq i}^{n}X_k$ 相互独立．

（Ⅱ）

$$\rho_{Y_1Y_n}=\frac{\mathrm{Cov}(Y_1,Y_n)}{\sqrt{DY_1}\cdot\sqrt{DY_n}}.$$

由（Ⅰ），知 $\sqrt{DY_1}\cdot\sqrt{DY_n}=\dfrac{n-1}{n}$，故

$$\mathrm{Cov}(Y_1,Y_n)=E\left[(Y_1-EY_1)(Y_n-EY_n)\right]$$

$$=E\left[(X_1-\overline{X})(X_n-\overline{X})\right]\quad(EY_1=EY_n=0)$$

$$=E(X_1X_n)+E(\overline{X}^2)-E(X_1\overline{X})-E(X_n\overline{X})$$

$$=EX_1\cdot EX_n+D\overline{X}+(E\overline{X})^2-\frac{1}{n}E(X_1^2)-\frac{1}{n}\sum_{i=2}^{n}E(X_iX_1)-\frac{1}{n}E(X_n^2)-\frac{1}{n}\sum_{i=1}^{n-1}E(X_iX_n),$$

而

$$D\overline{X}=D\left(\frac{1}{n}\sum_{i=1}^{n}X_i\right)=\frac{1}{n^2}\sum_{i=1}^{n}DX_i=\frac{1}{n^2}\cdot n=\frac{1}{n},$$

$$E(X_1^2)=DX_1+(EX_1)^2=1+0=1,$$

$$E(X_n^2)=DX_n+(EX_n)^2=1+0=1,$$

$$\sum_{i=2}^{n}E(X_iX_1)=\sum_{i=2}^{n}(EX_i\cdot EX_1)=0,\quad\sum_{i=1}^{n-1}E(X_iX_n)=\sum_{i=1}^{n-1}(EX_i\cdot EX_n)=0,$$

故

$$\mathrm{Cov}(Y_1,Y_n)=0+\frac{1}{n}+0-\frac{1}{n}-0-\frac{1}{n}-0=-\frac{1}{n},$$

所以

$$\rho_{Y_1Y_n}=\frac{-\dfrac{1}{n}}{\dfrac{n-1}{n}}=-\frac{1}{n-1}.$$

【注】① 设 $\overline{X}=\dfrac{1}{n}\displaystyle\sum_{i=1}^{n}X_i$，$X_1,X_2,\cdots,X_n$ 相互独立，$X_i\sim N(\mu,\sigma^2)\ (i=1,2,\cdots,n)$，则 $E\overline{X}=\mu$，$D\overline{X}=\dfrac{\sigma^2}{n}$．这是统计学中的基本结论．

② $X,Y$ 相互独立 $\Rightarrow E(XY)=EX\cdot EY$，$D(X\pm Y)=DX+DY$．

+++

#### 综合解答 (3) 设随机试验 $E$ 有三种两两不相容的结果 $A_1,A_2,A_3$，且三种结果发生的概率均为 $\dfrac{1}{3}$，将试验 $E$ 独立重复做 $2$ 次，$X$ 表示 $2$ 次试验中结果 $A_1$ 发生的次数，$Y$ 表示 $2$ 次试验中结果 $A_2$ 发生的次数．

（Ⅰ）求 $(X,Y)$ 的联合分布律；\
（Ⅱ）求 $\rho_{XY}$．
***
（Ⅰ）由已知，$P(A_1)=P(A_2)=P(A_3)=\dfrac{1}{3}$，所以

$$X\sim B\left(2,\frac{1}{3}\right),\quad Y\sim B\left(2,\frac{1}{3}\right).$$

依题设，$(X,Y)$ 有 $9$ 个取值

$$(0,0),(0,1),(0,2),(1,0),(1,1),(1,2),(2,0),(2,1),(2,2).$$

由 $X,Y$ 的二项分布计算概率．

$$P\{X=0,Y=0\}=\mathrm{C}_2^0\cdot\frac{1}{3}\cdot\frac{1}{3}=\frac{1}{9},$$

$$P\{X=0,Y=1\}=\mathrm{C}_2^1\cdot\frac{1}{3}\cdot\frac{1}{3}=\frac{2}{9},$$

同理可得

$$P\{X=0,Y=2\}=\frac{1}{9},\quad P\{X=1,Y=0\}=\frac{2}{9},$$

$$P\{X=1,Y=1\}=\frac{2}{9},\quad P\{X=1,Y=2\}=0,\quad P\{X=2,Y=0\}=\frac{1}{9},$$

$$P\{X=2,Y=1\}=0,\quad P\{X=2,Y=2\}=0.$$

故 $(X,Y)$ 的联合分布律为

| $Y\ \backslash\ X$ | $0$ | $1$ | $2$ |
| --- | --- | --- | --- |
| $0$ | $\dfrac{1}{9}$ | $\dfrac{2}{9}$ | $\dfrac{1}{9}$ |
| $1$ | $\dfrac{2}{9}$ | $\dfrac{2}{9}$ | $0$ |
| $2$ | $\dfrac{1}{9}$ | $0$ | $0$ |

（Ⅱ）由（Ⅰ）知，$X,Y$ 的分布律为

| $X$ | $0$ | $1$ | $2$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{4}{9}$ | $\dfrac{4}{9}$ | $\dfrac{1}{9}$ |

| $Y$ | $0$ | $1$ | $2$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{4}{9}$ | $\dfrac{4}{9}$ | $\dfrac{1}{9}$ |

由公式 $\rho_{XY}=\dfrac{\mathrm{Cov}(X,Y)}{\sqrt{DX}\sqrt{DY}}$，需计算 $DX,DY,\mathrm{Cov}(X,Y)$．

$$EX=1\times\frac{4}{9}+2\times\frac{1}{9}=\frac{2}{3},\quad E(X^2)=1^2\times\frac{4}{9}+2^2\times\frac{1}{9}=\frac{8}{9},$$

$$DX=E(X^2)-(EX)^2=\frac{4}{9}.$$

同理

$$EY=\frac{2}{3},\quad DY=\frac{4}{9},\quad E(XY)=\frac{2}{9},$$

$$\mathrm{Cov}(X,Y)=E(XY)-EX\cdot EY=\frac{2}{9}-\frac{2}{3}\times\frac{2}{3}=-\frac{2}{9},$$

所以

$$\rho_{XY}=\frac{-\dfrac{2}{9}}{\dfrac{4}{9}}=-\frac{1}{2}.$$

+++

#### 综合解答 (4) 设随机变量 $X_1,X_2,X_3$ 相互独立，且均服从参数为 $\lambda$ 的指数分布，记 $Y=\min\{X_1,X_2\}$，$T=\max\{Y,X_3\}$．

（Ⅰ）求 $Y$ 的概率密度 $f_Y(y)$；\
（Ⅱ）求期望 $ET$．
***
（Ⅰ）由已知，$X_1$ 与 $X_2$ 相互独立，故 $(X_1,X_2)$ 的概率密度为

$$f(x_1,x_2)=\begin{cases}\lambda^2\mathrm{e}^{-\lambda(x_1+x_2)},&x_1>0,x_2>0,\\0,&\text{其他}.\end{cases}$$

设 $Y$ 的分布函数为 $F_Y(y)$，则当 $y\leqslant 0$ 时，$F_Y(y)=0$；当 $y>0$ 时，有

$$F_Y(y)=P\{\min\{X_1,X_2\}\leqslant y\}=1-P\{X_1>y,X_2>y\}$$

$$=1-P\{X_1>y\}\cdot P\{X_2>y\}=1-\mathrm{e}^{-\lambda y}\cdot\mathrm{e}^{-\lambda y}=1-\mathrm{e}^{-2\lambda y},$$

故

$$f_Y(y)=F_Y'(y)=\begin{cases}2\lambda\mathrm{e}^{-2\lambda y},&y>0,\\0,&y\leqslant 0.\end{cases}$$

（Ⅱ）先求 $T$ 的分布函数与概率密度．

当 $t\leqslant 0$ 时，$F_T(t)=0$；当 $t>0$ 时，有

$$F_T(t)=P\{T\leqslant t\}=P\{\max\{Y,X_3\}\leqslant t\}=P\{Y\leqslant t,X_3\leqslant t\}.$$

而 $Y=\min\{X_1,X_2\}$ 与 $X_3$ 相互独立，故

$$F_T(t)=P\{Y\leqslant t\}\cdot P\{X_3\leqslant t\}=(1-\mathrm{e}^{-2\lambda t})(1-\mathrm{e}^{-\lambda t}),$$

所以

$$f_T(t)=F_T'(t)=\begin{cases}\lambda\mathrm{e}^{-\lambda t}+2\lambda\mathrm{e}^{-2\lambda t}-3\lambda\mathrm{e}^{-3\lambda t},&t>0,\\0,&t\leqslant 0,\end{cases}$$

于是

$$ET=\int_{0}^{+\infty}t\cdot(\lambda\mathrm{e}^{-\lambda t}+2\lambda\mathrm{e}^{-2\lambda t}-3\lambda\mathrm{e}^{-3\lambda t})\mathrm{d}t=\frac{1}{\lambda}+\frac{1}{2\lambda}-\frac{1}{3\lambda}=\frac{7}{6\lambda}.$$

+++

#### 综合解答 (5) 设 $X_1,X_2,\cdots,X_n$ 相互独立同分布，其相同的概率密度为

$$f(x)=\begin{cases}2\mathrm{e}^{-2(x-\theta)},&x>\theta,\\0,&x\leqslant\theta,\end{cases}\quad\theta\ \text{为常数},$$

求 $Z=\min\limits_{1\leqslant i\leqslant n}\{X_i\}$ 的数学期望．
***
$n$ 个随机变量的函数的期望计算，先求 $Z$ 的分布函数，从而得 $Z$ 的概率密度，再用期望定义计算．

由已知，$X_1,X_2,\cdots,X_n$ 共同的分布函数为

$$F(x)=\int_{-\infty}^{x}f(t)\mathrm{d}t=\begin{cases}1-\mathrm{e}^{-2(x-\theta)},&x>\theta,\\0,&x\leqslant\theta.\end{cases}$$

$Z$ 的分布函数为

$$F_Z(z)=P\{Z\leqslant z\}=P\left\{\min_{1\leqslant i\leqslant n}\{X_i\}\leqslant z\right\}=1-P\left\{\min_{1\leqslant i\leqslant n}\{X_i\}>z\right\}$$

$$=1-P\{X_1>z,X_2>z,\cdots,X_n>z\}=1-P\{X_1>z\}P\{X_2>z\}\cdots P\{X_n>z\}$$

$$=1-\left[1-F(z)\right]^n=\begin{cases}1-\mathrm{e}^{-2n(z-\theta)},&z>\theta,\\0,&z\leqslant\theta,\end{cases}$$

于是 $Z$ 的概率密度为

$$f_Z(z)=F_Z'(z)=\begin{cases}2n\mathrm{e}^{-2n(z-\theta)},&z>\theta,\\0,&z\leqslant\theta,\end{cases}$$

故

$$EZ=\int_{-\infty}^{+\infty}zf_Z(z)\mathrm{d}z=\int_{\theta}^{+\infty}2nz\mathrm{e}^{-2n(z-\theta)}\mathrm{d}z=\theta+\frac{1}{2n}.$$

+++

#### 综合解答 (6) 设 $X_1$ 与 $X_2$ 相互独立，$X_i\sim B(i,p)\ (i=1,2,\ 0<p<1)$．令

$$Y_1=\begin{cases}0,&X_1+X_2=1,\\1,&X_1+X_2\neq 1,\end{cases}\qquad Y_2=\begin{cases}0,&X_2-X_1=2,\\1,&X_2-X_1\neq 2.\end{cases}$$

（Ⅰ）求 $\mathrm{Cov}(Y_1,Y_2)$；\
（Ⅱ）确定 $p$ 的值，使 $\mathrm{Cov}(Y_1,Y_2)$ 取值最小．
***
（Ⅰ）依题设，$Y_1$ 与 $Y_2$ 均服从 $0-1$ 分布，故

$$E(Y_1)=P\{Y_1=1\}=1-P\{Y_1=0\}=1-P\{X_1+X_2=1\}=1-3p(1-p)^2,$$

$$E(Y_2)=P\{Y_2=1\}=1-P\{Y_2=0\}=1-P\{X_2-X_1=2\}=1-P\{X_1=0,X_2=2\}=1-p^2(1-p).$$

$Y_1Y_2$ 也服从 $0-1$ 分布，故

$$P\{Y_1Y_2=0\}=P\{(Y_1=0)\cup(Y_2=0)\}$$

$$=P\{Y_1=0\}+P\{Y_2=0\}-P\{Y_1=0,Y_2=0\}=3p(1-p)^2+p^2(1-p),$$

这里 $P\{Y_1=0,Y_2=0\}=P\{X_2+X_1=1,X_2-X_1=2\}=P\{\varnothing\}=0$，故

$$P\{Y_1Y_2=1\}=1-P\{Y_1Y_2=0\}=1-3p(1-p)^2-p^2(1-p),$$

所以

$$\mathrm{Cov}(Y_1,Y_2)=E(Y_1Y_2)-E(Y_1)E(Y_2)$$

$$=0\cdot P\{Y_1Y_2=0\}+1\cdot P\{Y_1Y_2=1\}-\left[1-3p(1-p)^2\right]\cdot\left[1-p^2(1-p)\right]$$

$$=-3p^3(1-p)^3\xlongequal{\text{记}}f(p).$$

（Ⅱ）由（Ⅰ），知 $f(p)=-3p^3(1-p)^3$．令

$$f'(p)=-9p^2(1-p)^2\cdot(1-2p)=0,$$

得 $p=0$（舍去），$p=1$（舍去），$p=\dfrac{1}{2}$．

当 $p<\dfrac{1}{2}$ 时，$f'(p)<0$；当 $p>\dfrac{1}{2}$ 时，$f'(p)>0$，故 $p=\dfrac{1}{2}$ 是 $f(p)$ 在 $(0,1)$ 内唯一的极小值点，也是最小值点，所以当 $p=\dfrac{1}{2}$ 时，$\mathrm{Cov}(Y_1,Y_2)$ 取值最小．

【注】求 $P\{X_1+X_2=1\}$，利用 $X_1$ 与 $X_2$ 相互独立．

$$X_1\sim B(1,p),\quad X_2\sim B(2,p),$$

且 $X_1$ 与 $X_2$ 相互独立，则 $X_1+X_2\sim B(1+2,p)=B(3,p)$．

+++

#### 综合解答 (7) 设随机变量 $X$ 与 $Y$ 相互独立，$X$ 的概率分布为 $P\{X=0\}=P\{X=1\}=\dfrac{1}{2}$，$Y$ 在 $[0,1]$ 上服从均匀分布．

（Ⅰ）求 $Z=X+Y$ 的分布函数与概率密度；\
（Ⅱ）求相关系数 $\rho_{XZ}$．
***
（Ⅰ）由已知，$Y$ 的概率密度为

$$f(y)=\begin{cases}1,&0\leqslant y\leqslant 1,\\0,&\text{其他},\end{cases}$$

因此 $Y$ 的分布函数为

$$F(y)=\int_{-\infty}^{y}f(t)\mathrm{d}t=\begin{cases}0,&y<0,\\y,&0\leqslant y\leqslant 1,\\1,&y>1.\end{cases}$$

令 $G(z)$ 是 $Z=X+Y$ 的分布函数，则当 $z<0$ 时，$G(z)=0$；当 $z\geqslant 2$ 时，$G(z)=1$；当 $0\leqslant z<2$ 时，

$$G(z)=P\{Z\leqslant z\}=P\{X+Y\leqslant z\}$$

$$=P\{X+Y\leqslant z,X=0\}+P\{X+Y\leqslant z,X=1\}$$

$$=P\{X=0,Y\leqslant z\}+P\{X=1,Y\leqslant z-1\}$$

$$=P\{X=0\}\cdot P\{Y\leqslant z\}+P\{X=1\}\cdot P\{Y\leqslant z-1\}$$

$$=\frac{1}{2}P\{Y\leqslant z\}+\frac{1}{2}P\{Y\leqslant z-1\}$$

$$=\begin{cases}\dfrac{1}{2}z+0,&0\leqslant z<1,\\\dfrac{1}{2}+\dfrac{1}{2}(z-1),&1\leqslant z<2\end{cases}=\frac{1}{2}z.$$

综上可得，$Z$ 的分布函数为

$$G(z)=\begin{cases}0,&z<0,\\\dfrac{z}{2},&0\leqslant z<2,\\1,&z\geqslant 2,\end{cases}$$

$Z$ 的概率密度为

$$f_Z(z)=G'(z)=\begin{cases}\dfrac{1}{2},&0\leqslant z<2,\\0,&\text{其他},\end{cases}$$

即服从 $U[0,2]$．

（Ⅱ）由于

$$\rho_{XZ}=\frac{\mathrm{Cov}(X,Z)}{\sqrt{DX}\sqrt{DZ}}=\frac{E(XZ)-EX\cdot EZ}{\sqrt{DX}\sqrt{DZ}},$$

其中

$$EX=\frac{1}{2},\quad EY=\frac{0+1}{2}=\frac{1}{2},\quad EZ=\frac{0+2}{2}=1,$$

$$DX=p(1-p)=\frac{1}{2}\times\left(1-\frac{1}{2}\right)=\frac{1}{4},$$

$$DZ=\frac{(2-0)^2}{12}=\frac{1}{3},$$

$$E(XZ)=E\left[X(X+Y)\right]=E(X^2)+E(XY)=\frac{1}{2}+EX\cdot EY=\frac{1}{2}+\frac{1}{2}\times\frac{1}{2}=\frac{3}{4},$$

故

$$\rho_{XZ}=\frac{\dfrac{3}{4}-\dfrac{1}{2}\times 1}{\sqrt{\dfrac{1}{4}}\times\sqrt{\dfrac{1}{3}}}=\frac{\sqrt{3}}{2}.$$

+++

#### 拓展解答 (1) 设随机变量 $X_1$ 与 $X_2$ 相互独立，且 $X_1\sim B(1,p)$，$X_2\sim B(2,p)$，其中 $0<p<1$，令 $Y_1=2X_1+X_2$，$Y_2=X_1-X_2$．

（Ⅰ）求相关系数 $\rho_{Y_1Y_2}$；\
（Ⅱ）问 $Y_1$ 与 $Y_2$ 是否相互独立？并说明理由．
***
（Ⅰ）由 $X_1$ 与 $X_2$ 相互独立及 $X_1\sim B(1,p)$，$X_2\sim B(2,p)$，可知

$$\mathrm{Cov}(X_1,X_2)=0,\quad DX_1=p(1-p),\quad DX_2=2p(1-p).$$

由于

$$\mathrm{Cov}(Y_1,Y_2)=\mathrm{Cov}(2X_1+X_2,X_1-X_2)=2DX_1-DX_2-\mathrm{Cov}(X_1,X_2)$$

$$=2p(1-p)-2p(1-p)=0,$$

故

$$\rho_{Y_1Y_2}=\frac{\mathrm{Cov}(Y_1,Y_2)}{\sqrt{DY_1}\sqrt{DY_2}}=0.$$

（Ⅱ）由于

$$\{Y_1=0\}=\{2X_1+X_2=0\}=\{X_1=0,X_2=0\},$$

$$\{Y_2=0\}=\{X_1-X_2=0\}=\{X_1=0,X_2=0\}\cup\{X_1=1,X_2=1\},$$

且 $\{Y_1=0\}\subset\{Y_2=0\}$，$P\{Y_2=0\}<1$，故

$$P\{Y_1=0,Y_2=0\}=P\{Y_1=0\},$$

$$P\{Y_1=0\}\cdot P\{Y_2=0\}<P\{Y_1=0\},$$

从而

$$P\{Y_1=0,Y_2=0\}\neq P\{Y_1=0\}\cdot P\{Y_2=0\},$$

即 $Y_1$ 与 $Y_2$ **不相互独立**．

【注】此题说明两个随机变量不相关是它们相互独立的必要条件而非充分条件．

+++

#### 拓展解答 (2) 设 $X$ 是连续型随机变量，且 $P\{X\leqslant a\}=P\{X>b\}=\dfrac{1}{4}$，令

$$X_1=\begin{cases}-1,&X\leqslant a,\\1,&X>a,\end{cases}\qquad X_2=\begin{cases}-1,&X\leqslant b,\\1,&X>b.\end{cases}$$

（Ⅰ）求 $(X_1,X_2)$ 的联合分布及边缘分布；\
（Ⅱ）求 $\mathrm{Cov}(X_1,X_2)$，$D(X_1-X_2)$．
***
（Ⅰ）由

$$P\{X\leqslant b\}=1-P\{X>b\}=\frac{3}{4},\quad P\{X\leqslant a\}=\frac{1}{4},$$

知 $a<b$，故

$$P\{X_1=-1,X_2=-1\}=P\{X\leqslant a,X\leqslant b\}=P\{X\leqslant a\}=\frac{1}{4};$$

$$P\{X_1=-1,X_2=1\}=P\{X\leqslant a,X>b\}=0;$$

$$P\{X_1=1,X_2=-1\}=P\{X>a,X\leqslant b\}=P\{a<X\leqslant b\}=\frac{1}{2};$$

$$P\{X_1=1,X_2=1\}=1-\frac{1}{4}-0-\frac{1}{2}=\frac{1}{4}.$$

从而 $(X_1,X_2)$ 的联合分布与边缘分布为

| $X_1\ \backslash\ X_2$ | $-1$ | $1$ | $X_1$ 的边缘 |
| --- | --- | --- | --- |
| $-1$ | $\dfrac{1}{4}$ | $0$ | $\dfrac{1}{4}$ |
| $1$ | $\dfrac{1}{2}$ | $\dfrac{1}{4}$ | $\dfrac{3}{4}$ |
| $X_2$ 的边缘 | $\dfrac{3}{4}$ | $\dfrac{1}{4}$ | |

（Ⅱ）由（Ⅰ），知

$$EX_1=\frac{1}{2},\quad E(X_1^2)=1,\quad EX_2=-\frac{1}{2},\quad E(X_2^2)=1,$$

故 $DX_1=DX_2=\dfrac{3}{4}$，$E(X_1X_2)=0$，从而

$$\mathrm{Cov}(X_1,X_2)=E(X_1X_2)-EX_1\cdot EX_2=\frac{1}{4},$$

$$D(X_1-X_2)=DX_1-2\mathrm{Cov}(X_1,X_2)+DX_2=1.$$
