---
quizify:
  format: 1
  deck: Math_880::Chapter_22
  tags: [Math, 880题, 数一, 第二十二章, 参数估计]
---

+++

#### 基础解答 (1) 设总体 $X$ 的概率分布为

$$\begin{array}{c|ccc}X & 1 & 2 & 3\\\hline p & \theta^2 & 2\theta(1-\theta) & (1-\theta)^2\end{array}$$

已知容量为 $3$ 的样本值为 $x_1=1,x_2=2,x_3=1$，求 $\theta$ 的矩估计值和最大似然估计值．
***
由

$$EX=\theta^2+2\cdot 2\theta(1-\theta)+3(1-\theta)^2=-2\theta+3,$$

得 $\theta=\dfrac{3-EX}{2}$，故 $\theta$ 的矩估计值 $\hat{\theta}=\dfrac{3-\bar{x}}{2}$．又

$$\bar{x}=\frac{x_1+x_2+x_3}{3}=\frac{1+2+1}{3}=\frac{4}{3},$$

所以 $\hat{\theta}=\dfrac{5}{6}$．

似然函数为 $L(\theta)=\theta^2\cdot 2\theta(1-\theta)\cdot\theta^2=2\theta^5(1-\theta)$．取对数，得

$$\ln L(\theta)=\ln 2+5\ln\theta+\ln(1-\theta),$$

令 $\dfrac{\mathrm{d}\ln L(\theta)}{\mathrm{d}\theta}=\dfrac{5}{\theta}-\dfrac{1}{1-\theta}=0$，解得 $\theta$ 的最大似然估计值为 $\hat{\theta}=\dfrac{5}{6}$．

+++

#### 基础解答 (2) 设总体 $X$ 的概率密度为 $f(x;\lambda)=\begin{cases}-\lambda^x\ln\lambda,&x\geqslant 0,\\0,&x<0\end{cases}$ $(0<\lambda<1)$，$(X_1,X_2,\cdots,X_n)$ 为总体 $X$ 的简单随机样本，求 $\lambda$ 的矩估计量．
***
$$EX=\int_{-\infty}^{+\infty}x\cdot f(x;\lambda)\mathrm{d}x=-\int_{0}^{+\infty}x\cdot\lambda^x\ln\lambda\,\mathrm{d}x$$

$$=-\int_{0}^{+\infty}x\,\mathrm{d}(\lambda^x)=-x\lambda^x\Big|_{0}^{+\infty}+\int_{0}^{+\infty}\lambda^x\mathrm{d}x$$

$$=\frac{\lambda^x}{\ln\lambda}\Big|_{0}^{+\infty}=-\frac{1}{\ln\lambda},$$

即 $EX=-\dfrac{1}{\ln\lambda}$，解得 $\lambda=\mathrm{e}^{-\frac{1}{EX}}$，故 $\lambda$ 的矩估计量为 $\hat{\lambda}=\mathrm{e}^{-\frac{1}{\bar{X}}}$，其中 $\bar{X}=\dfrac{1}{n}\sum\limits_{i=1}^{n}X_i$．

+++

#### 基础解答 (3) 设总体 $X$ 的概率密度为 $f(x;\theta)=\begin{cases}\sqrt{\theta}\cdot x^{\sqrt{\theta}-1},&0\leqslant x\leqslant 1,\\0,&\text{其他,}\end{cases}$ 其中 $\theta>0$ 为未知参数，$(x_1,x_2,\cdots,x_n)$ 为 $X$ 的简单随机样本值．

（Ⅰ）求 $\theta$ 的矩估计值；\
（Ⅱ）求 $\theta$ 的最大似然估计值．
***
（Ⅰ）由

$$EX=\int_{-\infty}^{+\infty}x\cdot f(x;\theta)\mathrm{d}x=\int_{0}^{1}x\cdot\sqrt{\theta}\cdot x^{\sqrt{\theta}-1}\mathrm{d}x=\int_{0}^{1}\sqrt{\theta}x^{\sqrt{\theta}}\mathrm{d}x=\frac{\sqrt{\theta}}{\sqrt{\theta}+1},$$

解得 $\theta=\left(\dfrac{EX}{1-EX}\right)^2$，故 $\theta$ 的矩估计值为 $\hat{\theta}=\left(\dfrac{\bar{x}}{1-\bar{x}}\right)^2$．

（Ⅱ）似然函数为 $L(\theta)=\prod\limits_{i=1}^{n}\sqrt{\theta}x_i^{\sqrt{\theta}-1}=\theta^{\frac{n}{2}}\left(\prod\limits_{i=1}^{n}x_i\right)^{\sqrt{\theta}-1}$．取对数，得

$$\ln L(\theta)=\frac{n}{2}\ln\theta+(\sqrt{\theta}-1)\sum_{i=1}^{n}\ln x_i.$$

令

$$\frac{\mathrm{d}\ln L(\theta)}{\mathrm{d}\theta}=\frac{n}{2\theta}+\frac{1}{2\sqrt{\theta}}\sum_{i=1}^{n}\ln x_i=0,$$

得 $\theta$ 的最大似然估计值为 $\hat{\theta}=\dfrac{n^2}{\left(\sum\limits_{i=1}^{n}\ln x_i\right)^2}$．

+++

#### 基础解答 (4) 设 $X_1,X_2,\cdots,X_n$ 是来自总体 $X$ 的简单随机样本，$X$ 的概率密度为

$$f(x)=\frac{1}{2\theta}\mathrm{e}^{-\frac{|x|}{\theta}},\quad -\infty<x<+\infty,\ \theta>0.$$

求参数 $\theta$ 的矩估计量 $\hat{\theta}$ 及 $E(\hat{\theta}^2)$．
***
由于

$$EX=\int_{-\infty}^{+\infty}xf(x)\mathrm{d}x=\int_{-\infty}^{+\infty}x\cdot\frac{1}{2\theta}\mathrm{e}^{-\frac{|x|}{\theta}}\mathrm{d}x=0,$$

$$E(X^2)=\int_{-\infty}^{+\infty}x^2f(x)\mathrm{d}x=\int_{-\infty}^{+\infty}x^2\cdot\frac{1}{2\theta}\mathrm{e}^{-\frac{|x|}{\theta}}\mathrm{d}x$$

$$=\int_{0}^{+\infty}\frac{x^2}{\theta}\mathrm{e}^{-\frac{x}{\theta}}\mathrm{d}x\xlongequal{\frac{x}{\theta}=t}\theta^2\int_{0}^{+\infty}t^2\mathrm{e}^{-t}\mathrm{d}t$$

$$=\theta^2\Gamma(3)=\theta^2\cdot 2!=2\theta^2,$$

故 $\theta$ 的矩估计量 $\hat{\theta}=\sqrt{\dfrac{1}{2n}\sum\limits_{i=1}^{n}X_i^2}$．又由 $\hat{\theta}^2=\dfrac{1}{2n}\sum\limits_{i=1}^{n}X_i^2$，得

$$E(\hat{\theta}^2)=\frac{1}{2n}\sum_{i=1}^{n}E(X_i^2)=\frac{1}{2n}\sum_{i=1}^{n}\left[\int_{-\infty}^{+\infty}x^2f(x)\mathrm{d}x\right]=\theta^2.$$

+++

#### 基础解答 (5) 设总体 $X$ 的概率密度为 $f(x;\theta)=\begin{cases}\dfrac{1}{\theta},&0\leqslant x\leqslant\theta,\\0,&\text{其他,}\end{cases}$ 其中 $\theta>0$ 为未知参数，$(X_1,X_2,\cdots,X_n)$ 为 $X$ 的简单随机样本．

（Ⅰ）求 $\theta$ 的最大似然估计量 $\hat{\theta}$；\
（Ⅱ）求 $E(\hat{\theta})$ 和 $D(\hat{\theta})$．
***
（Ⅰ）由已知，似然函数为

$$L(\theta)=\begin{cases}\dfrac{1}{\theta^n},&0\leqslant x_1,x_2,\cdots,x_n\leqslant\theta,\\0,&\text{其他.}\end{cases}$$

要使 $L(\theta)$ 最大，$\theta$ 应尽量小，但 $0\leqslant x_1,x_2,\cdots,x_n\leqslant\theta$，即 $\theta$ 应大于等于 $x_1,x_2,\cdots,x_n$ 中的每一个，故 $\theta$ 的最大似然估计量为 $\hat{\theta}=\max\{X_1,X_2,\cdots,X_n\}$．

（Ⅱ）$\hat{\theta}$ 的概率密度为

$$f(x)=\begin{cases}n\left(\dfrac{x}{\theta}\right)^{n-1}\cdot\dfrac{1}{\theta}=\dfrac{n}{\theta^n}x^{n-1},&0\leqslant x\leqslant\theta,\\0,&\text{其他,}\end{cases}$$

故

$$E(\hat{\theta})=\int_{0}^{\theta}x\cdot\frac{n}{\theta^n}x^{n-1}\mathrm{d}x=\frac{n}{n+1}\theta,$$

$$E(\hat{\theta}^2)=\int_{0}^{\theta}x^2\cdot\frac{n}{\theta^n}x^{n-1}\mathrm{d}x=\frac{n}{n+2}\theta^2,$$

所以

$$D(\hat{\theta})=E(\hat{\theta}^2)-\left[E(\hat{\theta})\right]^2=\frac{n\theta^2}{(n+2)(n+1)^2}.$$

+++

#### 基础解答 (6) 某射手进行独立重复射击，每次击中目标的概率为 $p>0$，设他在第 $X$ 次射击时首次击中目标，以 $X$ 为总体，$(X_1,X_2,\cdots,X_n)$ 为 $X$ 的简单随机样本．

（Ⅰ）求 $X$ 的概率分布；\
（Ⅱ）求参数 $p$ 的矩估计量和最大似然估计量．
***
（Ⅰ）由已知，$X$ 服从几何分布，故其分布律为

$$P\{X=k\}=p(1-p)^{k-1},\quad k=1,2,\cdots.$$

（Ⅱ）

$$EX=\sum_{k=1}^{\infty}kp(1-p)^{k-1}=\frac{1}{p},$$

即 $p=\dfrac{1}{EX}$，故 $\hat{p}=\dfrac{1}{\bar{X}}$ 为矩估计量．

设 $(x_1,x_2,\cdots,x_n)$ 为 $(X_1,X_2,\cdots,X_n)$ 的样本值，则似然函数为

$$L(p)=\prod_{k=1}^{n}p(1-p)^{x_k-1}=p^n(1-p)^{\sum\limits_{k=1}^{n}x_k-n}.$$

取对数，得

$$\ln L(p)=n\ln p+\left(\sum_{k=1}^{n}x_k-n\right)\ln(1-p).$$

由

$$\frac{\mathrm{d}\ln L(p)}{\mathrm{d}p}=\frac{n}{p}-\frac{1}{1-p}\left(\sum_{k=1}^{n}x_k-n\right)=0,$$

解得 $p$ 的最大似然估计量为 $\hat{p}=\dfrac{1}{\bar{X}}$．

【注】几何分布的期望和方差分别为 $EX=\dfrac{1}{p}$，$DX=\dfrac{1-p}{p^2}\ (0<p<1)$，应牢记．

+++

#### 基础解答 (7) 设 $(X_1,X_2,\cdots,X_{10})$ 为总体 $X\sim N(0,\sigma^2)$ 的简单随机样本，$\sigma>0$ 为未知参数．

（Ⅰ）求 $\sigma^2$ 的最大似然估计量 $\hat{\sigma}^2$；\
（Ⅱ）若记 $U=\sum\limits_{i=1}^{6}X_i$，$V=\sum\limits_{i=5}^{10}X_i$，利用最大似然估计量 $\hat{\sigma}^2$，求相关系数 $\rho_{UV}$．
***
（Ⅰ）由已知，$X$ 的概率密度为

$$f(x)=\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{x^2}{2\sigma^2}},\quad -\infty<x<+\infty,$$

似然函数为

$$L(\sigma^2)=\prod_{i=1}^{10}\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{x_i^2}{2\sigma^2}}=(2\pi\sigma^2)^{-\frac{10}{2}}\cdot\mathrm{e}^{-\frac{1}{2\sigma^2}\sum\limits_{i=1}^{10}x_i^2}.$$

取对数，得

$$\ln L(\sigma^2)=-\frac{10}{2}\ln(2\pi\sigma^2)-\frac{1}{2\sigma^2}\sum_{i=1}^{10}x_i^2.$$

令 $\dfrac{\mathrm{d}}{\mathrm{d}(\sigma^2)}\ln L(\sigma^2)=0$，得 $-\dfrac{10}{2\sigma^2}+\dfrac{1}{2\sigma^4}\sum\limits_{i=1}^{10}x_i^2=0$，故 $\sigma^2$ 的最大似然估计量为 $\hat{\sigma}^2=\dfrac{1}{10}\sum\limits_{i=1}^{10}X_i^2$．

（Ⅱ）由（Ⅰ），知 $X\sim N(0,\hat{\sigma}^2)$，则

$$EU=E\left(\sum_{i=1}^{6}X_i\right)=0,\quad EV=E\left(\sum_{i=5}^{10}X_i\right)=0,$$

$$DU=D\left(\sum_{i=1}^{6}X_i\right)=6\hat{\sigma}^2,\quad DV=D\left(\sum_{i=5}^{10}X_i\right)=6\hat{\sigma}^2.$$

又 $\mathrm{Cov}(U,V)=\mathrm{Cov}\left(\sum\limits_{i=1}^{6}X_i,\sum\limits_{j=5}^{10}X_j\right)=\sum\limits_{i=1}^{6}\sum\limits_{j=5}^{10}\mathrm{Cov}(X_i,X_j)=DX_5+DX_6=2\hat{\sigma}^2$，其中，当 $i\neq j$ 时，$\mathrm{Cov}(X_i,X_j)=0$；当 $i=j$ 时，$\mathrm{Cov}(X_i,X_j)=DX_i=\hat{\sigma}^2$，故

$$\rho_{UV}=\frac{\mathrm{Cov}(U,V)}{\sqrt{DU}\sqrt{DV}}=\frac{2\hat{\sigma}^2}{6\hat{\sigma}^2}=\frac{1}{3}.$$

+++

#### 基础解答 (8) 设总体 $X$ 的概率密度为 $f(x)=\begin{cases}\dfrac{1}{\sqrt{2\pi}x}\mathrm{e}^{-\frac{(\ln x-\mu)^2}{2}},&x>0,\\0,&x\leqslant 0,\end{cases}$ $(X_1,X_2,\cdots,X_n)$ 为总体 $X$ 的简单随机样本．

（Ⅰ）求 $\mu$ 的最大似然估计量 $\hat{\mu}$；\
（Ⅱ）记 $Y=\ln X$，求 $Y$ 的分布函数和 $E\hat{\mu}$．
***
（Ⅰ）似然函数为

$$L(\mu)=\begin{cases}\prod\limits_{i=1}^{n}\dfrac{1}{\sqrt{2\pi}x_i}\mathrm{e}^{-\frac{1}{2}(\ln x_i-\mu)^2},&x_i>0,\\0,&\text{其他.}\end{cases}$$

取对数，得

$$\ln L(\mu)=\ln\left(\frac{1}{\sqrt{2\pi}}\right)^n+\ln\frac{1}{\prod\limits_{i=1}^{n}x_i}-\frac{1}{2}\sum_{i=1}^{n}(\ln x_i-\mu)^2.$$

令 $\dfrac{\mathrm{d}}{\mathrm{d}\mu}\ln L(\mu)=\sum\limits_{i=1}^{n}(\ln x_i-\mu)=0$，得 $\mu$ 的最大似然估计量为 $\hat{\mu}=\dfrac{1}{n}\sum\limits_{i=1}^{n}\ln X_i$．

（Ⅱ）

$$F_Y(x)=P\{Y\leqslant x\}=P\{\ln X\leqslant x\}=P\{X\leqslant\mathrm{e}^x\}$$

$$=\int_{0}^{\mathrm{e}^x}\frac{1}{\sqrt{2\pi}t}\mathrm{e}^{-\frac{1}{2}(\ln t-\mu)^2}\mathrm{d}t\xlongequal{\ln t=u}\int_{-\infty}^{x}\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{1}{2}(u-\mu)^2}\mathrm{d}u,$$

故 $Y=\ln X$ 服从正态分布 $N(\mu,1)$，所以 $E(\ln X)=\mu$，故

$$E\hat{\mu}=E\left(\frac{1}{n}\sum_{i=1}^{n}\ln X_i\right)=\frac{1}{n}\sum_{i=1}^{n}E(\ln X_i)=\mu.$$

+++

#### 基础解答 (9) 设 $X_1,X_2,\cdots,X_n$ 为来自总体 $X$ 的简单随机样本，$EX=\mu$，$DX=\sigma^2$，若 $\hat{\theta}=k\sum\limits_{i=1}^{n-1}(X_{i+1}-X_i)^2$ 为 $\sigma^2$ 的无偏估计量，求 $k$ 的值．
***
由已知，$E\hat{\theta}=\sigma^2$，由于

$$E\left[k\sum_{i=1}^{n-1}(X_{i+1}-X_i)^2\right]=k\sum_{i=1}^{n-1}E(X_{i+1}-X_i)^2$$

$$=k\sum_{i=1}^{n-1}\left\{D(X_{i+1}-X_i)+\left[E(X_{i+1}-X_i)\right]^2\right\}$$

$$=k\sum_{i=1}^{n-1}(DX_{i+1}+DX_i)=2(n-1)k\sigma^2=\sigma^2,$$

故 $k=\dfrac{1}{2(n-1)}$．

+++

#### 基础解答 (10) 设总体 $X$ 的概率密度为 $f(x;\theta)=\begin{cases}\dfrac{3x^2}{\theta^3},&0\leqslant x\leqslant\theta,\\0,&\text{其他,}\end{cases}$ 其中 $\theta>0$ 为未知参数，$(X_1,X_2,\cdots,X_n)$ 为 $X$ 的简单随机样本，$\bar{X}=\dfrac{1}{n}\sum\limits_{i=1}^{n}X_i$，$Y_n=\max\{X_1,X_2,\cdots,X_n\}$，证明：$\dfrac{3n+1}{3n}Y_n$ 与 $\dfrac{4}{3}\bar{X}$ 都是 $\theta$ 的无偏估计量．
***
依题意，得

$$EX=\int_{-\infty}^{+\infty}xf(x;\theta)\mathrm{d}x=\int_{0}^{\theta}x\cdot\frac{3x^2}{\theta^3}\mathrm{d}x=\frac{3}{4}\theta,$$

$$E\left(\frac{4}{3}\bar{X}\right)=\frac{4}{3}E\bar{X}=\frac{4}{3}EX=\frac{4}{3}\cdot\frac{3}{4}\theta=\theta,$$

所以 $\dfrac{4}{3}\bar{X}$ 是 $\theta$ 的无偏估计量．

又 $X$ 的分布函数为

$$F(x)=\int_{-\infty}^{x}f(t)\mathrm{d}t=\begin{cases}0,&x\leqslant 0,\\\dfrac{x^3}{\theta^3},&0<x<\theta,\\1,&x\geqslant\theta,\end{cases}$$

$Y_n=\max\{X_1,X_2,\cdots,X_n\}$ 的分布函数 $F_{Y_n}(x)$ 为

$$F_{Y_n}(x)=P\{\max\{X_1,X_2,\cdots,X_n\}\leqslant x\}$$

$$=P\{X_1\leqslant x,X_2\leqslant x,\cdots,X_n\leqslant x\}$$

$$=P\{X_1\leqslant x\}P\{X_2\leqslant x\}\cdots P\{X_n\leqslant x\}$$

$$=\left[F(x)\right]^n,$$

故 $Y_n$ 的概率密度为

$$f_{Y_n}(x)=F'_{Y_n}(x)=\begin{cases}n\left(\dfrac{x^3}{\theta^3}\right)^{n-1}\cdot\dfrac{3}{\theta^3}\cdot x^2=\dfrac{3nx^{3n-1}}{\theta^{3n}},&0\leqslant x\leqslant\theta,\\0,&\text{其他,}\end{cases}$$

所以

$$E(Y_n)=\int_{-\infty}^{+\infty}xf_{Y_n}(x)\mathrm{d}x=\int_{0}^{\theta}x\cdot\frac{3nx^{3n-1}}{\theta^{3n}}\mathrm{d}x=\frac{3n}{3n+1}\theta,$$

故 $E\left(\dfrac{3n+1}{3n}Y_n\right)=\dfrac{3n+1}{3n}\cdot\dfrac{3n}{3n+1}\theta=\theta$，即 $\dfrac{3n+1}{3n}Y_n$ 也是 $\theta$ 的无偏估计量．

+++

#### 基础解答 (11) 设总体 $X\sim B(1,p)$，参数 $p\in\left[\dfrac{1}{4},\dfrac{3}{4}\right]$，样本容量为 $1$，求 $p$ 的最大似然估计值．
***
由已知，$X$ 的分布律为 $P\{X=x\}=p^x\cdot(1-p)^{1-x}$，$x=0,1$．似然函数为

$$L(p)=p^x\cdot(1-p)^{1-x},\quad x=0,1.$$

令 $\dfrac{\mathrm{d}\ln L(p)}{\mathrm{d}p}=\dfrac{x}{p}-\dfrac{1-x}{1-p}=0$，得唯一解 $p=x$，但 $x\notin\left[\dfrac{1}{4},\dfrac{3}{4}\right]$，因此 $\hat{p}=x$ 不能作为 $p$ 的最大似然估计，用定义求．

由

$$L(p)=\begin{cases}p,&x=1,\\1-p,&x=0,\end{cases}$$

当 $x=0$ 时，$L(p)=1-p$ 关于 $p$ 单调减少，故 $\hat{p}=\dfrac{1}{4}$；当 $x=1$ 时，$L(p)=p$ 关于 $p$ 单调增加，故 $\hat{p}=\dfrac{3}{4}$，所以 $p$ 的最大似然估计值为 $\hat{p}=\dfrac{2x+1}{4}$，$x=0,1$．

+++

#### 基础解答 (12) 设总体 $X$ 在 $\left[\theta-\dfrac{1}{2},\theta+\dfrac{1}{2}\right]$ 上服从均匀分布，$\theta$ 为未知参数，$(X_1,X_2,\cdots,X_n)$ 为总体 $X$ 的样本，求 $\theta$ 的矩估计量 $\hat{\theta}_1$ 和最大似然估计量 $\hat{\theta}_2$．
***
（Ⅰ）先写出 $X$ 的概率密度 $f(x;\theta)=\begin{cases}1,&\theta-\dfrac{1}{2}\leqslant x\leqslant\theta+\dfrac{1}{2},\\0,&\text{其他,}\end{cases}$ 则

$$EX=\int_{-\infty}^{+\infty}x\cdot f(x;\theta)\mathrm{d}x=\int_{\theta-\frac{1}{2}}^{\theta+\frac{1}{2}}x\mathrm{d}x=\theta,$$

故 $\hat{\theta}_1=\bar{X}$ 为矩估计量．

（Ⅱ）似然函数

$$L(\theta)=\prod_{i=1}^{n}f(\theta)=\begin{cases}1,&\theta-\dfrac{1}{2}\leqslant x_i\leqslant\theta+\dfrac{1}{2},\\0,&\text{其他,}\end{cases}$$

$L(\theta)$ 是常值函数，仅取 $0,1$，所以只要满足 $\theta-\dfrac{1}{2}\leqslant x_i\leqslant\theta+\dfrac{1}{2}$ 的任何 $\theta$ 都使 $L(\theta)$ 取到最大值 $1$，由此得

$$\theta-\frac{1}{2}\leqslant\min_{1\leqslant i\leqslant n}\{x_i\},\quad \theta+\frac{1}{2}\geqslant\max_{1\leqslant i\leqslant n}\{x_i\},$$

所以 $\max\limits_{1\leqslant i\leqslant n}\{x_i\}-\dfrac{1}{2}\leqslant\theta\leqslant\min\limits_{1\leqslant i\leqslant n}\{x_i\}+\dfrac{1}{2}$，因此满足 $\max\limits_{1\leqslant i\leqslant n}\{x_i\}-\dfrac{1}{2}\leqslant g(x_1,x_2,\cdots,x_n)\leqslant\min\limits_{1\leqslant i\leqslant n}\{x_i\}+\dfrac{1}{2}$ 的任何统计量 $g(X_1,X_2,\cdots,X_n)$ 都是 $\theta$ 的最大似然估计量，如取 $\hat{\theta}_2=\min\limits_{1\leqslant i\leqslant n}\{X_i\}+\dfrac{1}{2}$ 或 $\hat{\theta}_2=\max\limits_{1\leqslant i\leqslant n}\{X_i\}-\dfrac{1}{2}$．

【注】由此题，知最大似然估计并不唯一．

+++

#### 基础解答 (13) 设总体 $X$ 服从参数为 $\lambda$ 的泊松分布，$(X_1,X_2,\cdots,X_n)$ 是总体 $X$ 的样本，$\bar{X}$ 是样本均值，$S^2$ 是样本方差．

（Ⅰ）对任意实数 $C$，证明：统计量 $T=C\bar{X}+(1-C)S^2$ 是参数 $\lambda$ 的无偏估计；\
（Ⅱ）求概率 $P\{X\geqslant 1\}$ 的最大似然估计量．
***
注意到对任何总体 $X$，$\bar{X}$ 和 $S^2$ 是总体 $X$ 的期望和方差的无偏估计量．

（Ⅰ）由 $X$ 服从泊松分布，故 $E\bar{X}=E(S^2)=\lambda$，于是

$$E\left[C\bar{X}+(1-C)S^2\right]=CE\bar{X}+(1-C)E(S^2)=C\lambda+(1-C)\lambda=\lambda,$$

即 $T$ 是 $\lambda$ 的无偏估计量．

（Ⅱ）先求 $\lambda$ 的最大似然估计量．泊松分布的概率密度为

$$P(x;\lambda)=\frac{\lambda^x}{x!}\mathrm{e}^{-\lambda}\quad(x=0,1,2,\cdots),$$

似然函数为

$$L(\lambda)=\prod_{i=1}^{n}\frac{\lambda^{X_i}}{X_i!}\mathrm{e}^{-\lambda}=\left(\prod_{i=1}^{n}\frac{1}{X_i!}\right)\lambda^{n\bar{X}}\cdot\mathrm{e}^{-n\lambda}.$$

取对数，得

$$\ln L(\lambda)=\ln\left(\prod_{i=1}^{n}\frac{1}{X_i!}\right)+n\bar{X}\ln\lambda-n\lambda.$$

对 $\lambda$ 求导，有

$$\frac{\mathrm{d}\ln L(\lambda)}{\mathrm{d}\lambda}=\frac{n\bar{X}}{\lambda}-n=0\Rightarrow\hat{\lambda}=\bar{X}$$

为 $\lambda$ 的最大似然估计量，由于 $P\{X\geqslant 1\}=1-P\{X=0\}=1-\mathrm{e}^{-\lambda}$ 是 $\lambda$ 的单调函数，根据最大似然估计量的不变性，$1-\mathrm{e}^{-\bar{X}}$ 为 $P\{X\geqslant 1\}$ 的最大似然估计量．

+++

#### 基础解答 (14) 设总体 $X\sim U(0,\theta)\ (\theta>0)$，$(X_1,X_2,\cdots,X_n)$ 为 $X$ 的简单随机样本，$X_{(n)}=\max\{X_1,X_2,\cdots,X_n\}$．

（Ⅰ）证明：$\hat{\theta}_1=2\bar{X}$，$\hat{\theta}_2=\dfrac{n+1}{n}X_{(n)}$ 是 $\theta$ 的无偏估计；\
（Ⅱ）当 $n\geqslant 2$ 时，问 $\hat{\theta}_1$ 和 $\hat{\theta}_2$ 哪一个有效．
***
（Ⅰ）由已知，$X$ 的概率密度为 $f_\theta(x)=\begin{cases}\dfrac{1}{\theta},&0<x<\theta,\\0,&\text{其他,}\end{cases}$

$$f_{X_{(n)}}(x)=F'_{X_{(n)}}(x)=\begin{cases}\dfrac{nx^{n-1}}{\theta^n},&0<x<\theta,\\0,&\text{其他,}\end{cases}$$

所以

$$E(2\bar{X})=E\left(\frac{2}{n}\sum_{i=1}^{n}X_i\right)=\frac{2}{n}\cdot n\cdot\frac{\theta}{2}=\theta,$$

$$E\left(\frac{n+1}{n}X_{(n)}\right)=\frac{n+1}{n}\int_{0}^{\theta}\frac{nx^n}{\theta^n}\mathrm{d}x=\frac{n+1}{n}\cdot\frac{n}{n+1}\theta=\theta,$$

故 $\hat{\theta}_1,\hat{\theta}_2$ 是 $\theta$ 的无偏估计．

（Ⅱ）

$$D(\hat{\theta}_1)=D(2\bar{X})=\frac{4}{n}\cdot\frac{\theta^2}{12}=\frac{\theta^2}{3n},$$

$$E(X_{(n)}^2)=\int_{0}^{\theta}\frac{nx^{n+1}}{\theta^n}\mathrm{d}x=\frac{n}{n+2}\theta^2,$$

故

$$D(\hat{\theta}_2)=\left(\frac{n+1}{n}\right)^2\left\{E(X_{(n)}^2)-\left[EX_{(n)}\right]^2\right\}=\frac{\theta^2}{n(n+2)},$$

当 $n\geqslant 2$ 时，$D(\hat{\theta}_2)<D(\hat{\theta}_1)$，故 $\hat{\theta}_2$ 比 $\hat{\theta}_1$ 有效．

【注】$X_{(n)}=\max\{X_1,X_2,\cdots,X_n\}$ 的分布函数 $F_{X_{(n)}}(x)=\begin{cases}\dfrac{x^n}{\theta^n},&0<x<\theta,\\0,&\text{其他.}\end{cases}$

+++

#### 基础解答 (15) 设总体 $X\sim N(\mu,\sigma^2)$，$\mu,\sigma^2$ 为未知参数，$(x_1,x_2,\cdots,x_n)$ 为总体 $X$ 的简单随机样本值，求 $\mu,\sigma^2$ 的最大似然估计量．
***
由 $X\sim N(\mu,\sigma^2)$，知 $X$ 的概率密度为

$$\varphi(x)=\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x-\mu)^2}{2\sigma^2}}\quad(-\infty<x<+\infty),$$

似然函数为

$$L(\mu,\sigma^2)=\prod_{i=1}^{n}\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(x_i-\mu)^2}{2\sigma^2}}=(2\pi\sigma^2)^{-\frac{n}{2}}\cdot\mathrm{e}^{-\sum\limits_{i=1}^{n}\frac{(x_i-\mu)^2}{2\sigma^2}}.$$

取对数，得

$$\ln L(\mu,\sigma^2)=-\frac{n}{2}\ln 2\pi-\frac{n}{2}\ln\sigma^2-\frac{1}{2\sigma^2}\sum_{i=1}^{n}(x_i-\mu)^2.$$

由于

$$\begin{cases}\dfrac{\partial\ln L}{\partial\mu}=\dfrac{1}{\sigma^2}\left(\sum\limits_{i=1}^{n}x_i-n\mu\right)=0,\\[2mm]\dfrac{\partial\ln L}{\partial\sigma^2}=-\dfrac{n}{2\sigma^2}+\dfrac{1}{2\sigma^4}\sum\limits_{i=1}^{n}(x_i-\mu)^2=0,\end{cases}$$

故最大似然估计量为 $\hat{\mu}=\bar{X}$，$\hat{\sigma}^2=\dfrac{1}{n}\sum\limits_{i=1}^{n}(X_i-\bar{X})^2$．

+++

#### 基础解答 (16) 设随机变量 $X$ 的概率密度为 $f(x)=\dfrac{1}{2}\mathrm{e}^{-|x-\mu|}$，$-\infty<x<+\infty$，$\mu$ 为未知参数，由样本值 $1\,028,968,1\,007$，求 $\mu$ 的矩估计值和最大似然估计值．
***
$$EX=\int_{-\infty}^{+\infty}x\cdot\frac{1}{2}\mathrm{e}^{-|x-\mu|}\mathrm{d}x\xlongequal{t=x-\mu}\int_{-\infty}^{+\infty}(t+\mu)\frac{1}{2}\mathrm{e}^{-|t|}\mathrm{d}t$$

$$=\int_{-\infty}^{+\infty}t\cdot\frac{1}{2}\mathrm{e}^{-|t|}\mathrm{d}t+\mu\int_{-\infty}^{+\infty}\frac{1}{2}\mathrm{e}^{-|t|}\mathrm{d}t=\mu\int_{0}^{+\infty}\mathrm{e}^{-t}\mathrm{d}t=\mu,$$

故 $\mu$ 的矩估计值为

$$\hat{\mu}=\bar{x}=\frac{1}{3}(1\,028+968+1\,007)=1\,001.$$

似然函数为 $L(\mu)=\left(\dfrac{1}{2}\right)^3\mathrm{e}^{-\sum\limits_{i=1}^{3}|x_i-\mu|}$．取对数，得 $\ln L(\mu)=-3\ln 2-\sum\limits_{i=1}^{3}|x_i-\mu|$．

要使 $\ln L(\mu)$ 最大，只要 $\sum\limits_{i=1}^{3}|x_i-\mu|$ 最小．

记 $m=\sum\limits_{i=1}^{3}|x_i-\mu|=|1\,028-\mu|+|968-\mu|+|1\,007-\mu|$，

当 $\mu\leqslant 968$ 时，

$$m=(1\,028-\mu)+(968-\mu)+(1\,007-\mu)=3(1\,001-\mu)\geqslant 3(1\,001-968)=99;$$

当 $\mu\geqslant 1\,028$ 时，

$$m=(\mu-1\,028)+(\mu-968)+(\mu-1\,007)=3(\mu-1\,001)\geqslant 3(1\,028-1\,001)=81;$$

当 $968<\mu<1\,028$ 时，$m=(1\,028-\mu)+(\mu-968)+|1\,007-\mu|=60+|1\,007-\mu|$，

故当 $\mu=1\,007$ 时，$m$ 最小，取值为 $60$，所以 $\mu$ 的最大似然估计值为 $\hat{\mu}=1\,007$．

+++

#### 基础解答 (17) 设总体 $X$ 的概率密度为

$$f(x;\lambda_1,\lambda_2)=\frac{1}{\lambda_2}\mathrm{e}^{-\frac{x-\lambda_1}{\lambda_2}},\quad -\infty<\lambda_1<x<+\infty,\ \lambda_2>0,$$

$(X_1,X_2,\cdots,X_n)$ 为 $X$ 的简单随机样本．

（Ⅰ）当 $\lambda_1$ 已知时，求 $\lambda_2$ 的矩估计量和最大似然估计量；\
（Ⅱ）求 $\lambda_1,\lambda_2$ 的矩估计量和最大似然估计量．
***
（Ⅰ）当 $\lambda_1$ 已知时，

$$EX=\int_{-\infty}^{+\infty}x\cdot f(x;\lambda_1,\lambda_2)\mathrm{d}x=\int_{\lambda_1}^{+\infty}x\cdot\frac{1}{\lambda_2}\mathrm{e}^{-\frac{x-\lambda_1}{\lambda_2}}\mathrm{d}x$$

$$\xlongequal{x=\lambda_1+\lambda_2y}\int_{0}^{+\infty}(\lambda_2y+\lambda_1)\mathrm{e}^{-y}\mathrm{d}y=\lambda_1+\lambda_2,$$

用 $\bar{X}$ 替换 $EX$，得 $\lambda_2$ 的矩估计量为 $\hat{\lambda}_2=\bar{X}-\lambda_1$．

关于 $\lambda_2$ 的似然函数为

$$L(\lambda_2)=\prod_{i=1}^{n}\frac{1}{\lambda_2}\mathrm{e}^{-\frac{x_i-\lambda_1}{\lambda_2}}=\frac{1}{\lambda_2^n}\mathrm{e}^{-\sum\limits_{i=1}^{n}\frac{x_i-\lambda_1}{\lambda_2}},\quad \lambda_1\leqslant x_1,x_2,\cdots,x_n.$$

由

$$\frac{\mathrm{d}\ln L(\lambda_2)}{\mathrm{d}\lambda_2}=-\frac{n}{\lambda_2}+\frac{1}{\lambda_2^2}\sum_{i=1}^{n}(x_i-\lambda_1)=0,$$

解得 $\hat{\lambda}_2=\dfrac{1}{n}\sum\limits_{i=1}^{n}(X_i-\lambda_1)$ 是 $\lambda_2$ 的最大似然估计量．

（Ⅱ）

$$EX=\lambda_1+\lambda_2,$$

$$E(X^2)=\int_{-\infty}^{+\infty}x^2\cdot f(x)\mathrm{d}x=\int_{\lambda_1}^{+\infty}x^2\cdot\frac{1}{\lambda_2}\mathrm{e}^{-\frac{x-\lambda_1}{\lambda_2}}\mathrm{d}x$$

$$\xlongequal{x=\lambda_1+\lambda_2y}\int_{0}^{+\infty}(\lambda_2y+\lambda_1)^2\mathrm{e}^{-y}\mathrm{d}y=2\lambda_2^2+2\lambda_1\lambda_2+\lambda_1^2,$$

则 $DX=E(X^2)-(EX)^2=\lambda_2^2$．

令 $EX=\bar{X}$，$DX=\dfrac{n-1}{n}S^2$（$S^2=\dfrac{1}{n-1}\sum\limits_{i=1}^{n}(X_i-\bar{X})^2$ 为样本方差），故

$$\begin{cases}\lambda_1+\lambda_2=\bar{X},\\\lambda_2^2=\dfrac{n-1}{n}S^2,\end{cases}$$

所以 $\lambda_1,\lambda_2$ 的矩估计量为

$$\hat{\lambda}_1=\bar{X}-\sqrt{\frac{n-1}{n}S^2},\quad \hat{\lambda}_2=\sqrt{\frac{n-1}{n}S^2}.$$

关于 $\lambda_1,\lambda_2$ 的似然函数为

$$L(\lambda_1,\lambda_2)=\frac{1}{\lambda_2^n}\mathrm{e}^{-\frac{1}{\lambda_2}\sum\limits_{i=1}^{n}(x_i-\lambda_1)},\quad \lambda_1\leqslant x_1,x_2,\cdots,x_n,$$

取对数，求偏导数，得

$$\begin{cases}\dfrac{\partial\ln L(\lambda_1,\lambda_2)}{\partial\lambda_1}=\dfrac{n}{\lambda_2}=0,&\text{①}\\[2mm]\dfrac{\partial\ln L(\lambda_1,\lambda_2)}{\partial\lambda_2}=-\dfrac{n}{\lambda_2}+\dfrac{1}{\lambda_2^2}\sum\limits_{i=1}^{n}(x_i-\lambda_1)=0,&\text{②}\end{cases}$$

由 ② 式，得 $\lambda_2=\bar{x}-\lambda_1$．① 式无解，用最大似然估计原理求 $\lambda_1,\lambda_2$ 的最大似然估计量．

由 $L(\lambda_1,\lambda_2)$ 的表达式知，当 $\hat{\lambda}_1$ 使 $L(\lambda_1,\lambda_2)>0$ 且使 $\sum\limits_{i=1}^{n}(x_i-\lambda_1)$ 达到最小时，才能使 $L(\lambda_1,\lambda_2)$ 达到最大．

由 $x_i\geqslant\lambda_1\ (i=1,2,\cdots,n)$，即 $\min\{X_1,X_2,\cdots,X_n\}\geqslant\lambda_1$ 时，有 $L(\lambda_1,\lambda_2)>0$，若使 $\sum\limits_{i=1}^{n}(x_i-\lambda_1)$ 在 $\hat{\lambda}_1$ 处达到最小，应取 $\hat{\lambda}_1=\min\{X_1,X_2,\cdots,X_n\}$，故当 $\hat{\lambda}_1=\min\{X_1,X_2,\cdots,X_n\}$ 时，有 $L(\lambda_1,\lambda_2)\leqslant L(\hat{\lambda}_1,\lambda_2)$．

当 $\lambda_1=\hat{\lambda}_1$ 时，由 ② 式，知 $\hat{\lambda}_2=\bar{x}-\hat{\lambda}_1$，由

$$\begin{cases}\dfrac{\partial\ln L(\hat{\lambda}_1,\lambda_2)}{\partial\lambda_2}=0,\\[2mm]\dfrac{\partial^2\ln L(\hat{\lambda}_1,\lambda_2)}{\partial\lambda_2^2}<0,\end{cases}$$

故 $L(\hat{\lambda}_1,\lambda_2)$ 在 $\lambda_2=\hat{\lambda}_2$ 处达到最大，故有 $L(\hat{\lambda}_1,\lambda_2)\leqslant L(\hat{\lambda}_1,\hat{\lambda}_2)$，从而知 $\lambda_1,\lambda_2$ 的最大似然估计量为

$$\hat{\lambda}_1=\min\{X_1,X_2,\cdots,X_n\},\quad \hat{\lambda}_2=\bar{X}-\min\{X_1,X_2,\cdots,X_n\}.$$

+++

#### 基础解答 (18) 设 $0.50,1.25,0.80,2.00$ 为来自总体 $X$ 的简单随机样本值，$Y=\ln X$ 服从正态分布 $N(\mu,1)$．（已知 $\Phi(1.96)=0.975$）

（Ⅰ）求 $EX$；\
（Ⅱ）求 $\mu$ 的置信度为 $0.95$ 的置信区间；\
（Ⅲ）求 $EX$ 的置信度为 $0.95$ 的置信区间．
***
（Ⅰ）由已知，$Y$ 的概率密度为 $f(y)=\dfrac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{(y-\mu)^2}{2}}\ (-\infty<y<+\infty)$．故

$$EX=E(\mathrm{e}^Y)=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{+\infty}\mathrm{e}^{y}\cdot\mathrm{e}^{-\frac{(y-\mu)^2}{2}}\mathrm{d}y$$

$$\xlongequal{t=y-\mu}\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{+\infty}\mathrm{e}^{t+\mu}\cdot\mathrm{e}^{-\frac{1}{2}t^2}\mathrm{d}t$$

$$=\mathrm{e}^{\mu+\frac{1}{2}}\int_{-\infty}^{+\infty}\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{1}{2}(t-1)^2}\mathrm{d}t=\mathrm{e}^{\mu+\frac{1}{2}}\cdot 1=\mathrm{e}^{\mu+\frac{1}{2}}.$$

（Ⅱ）当置信度 $1-\alpha=0.95$，即 $\alpha=0.05$，标准正态分布的分位数 $\mu_{1-\frac{\alpha}{2}}=\mu_{0.975}=1.96$．由 $\bar{Y}\sim N\left(\mu,\dfrac{1}{4}\right)$，得 $P\left\{\bar{y}-1.96\times\dfrac{1}{\sqrt{4}}<\mu<\bar{y}+1.96\times\dfrac{1}{\sqrt{4}}\right\}=0.95$．又

$$\bar{y}=\frac{1}{4}(\ln 0.5+\ln 1.25+\ln 0.8+\ln 2)=\frac{1}{4}\ln 1=0,$$

故 $\mu$ 的置信度为 $0.95$ 的置信区间为

$$\left(\bar{y}-1.96\times\frac{1}{\sqrt{4}},\ \bar{y}+1.96\times\frac{1}{\sqrt{4}}\right)=(-0.98,0.98).$$

（Ⅲ）由 $\mathrm{e}^x$ 严格单调增加，知 $EX=\mathrm{e}^{\mu+\frac{1}{2}}$ 的 $0.95$ 置信区间为

$$\left(\mathrm{e}^{\bar{y}-0.98+\frac{1}{2}},\ \mathrm{e}^{\bar{y}+0.98+\frac{1}{2}}\right)=\left(\mathrm{e}^{-0.48},\ \mathrm{e}^{1.48}\right).$$

【注】将 $x_i$ 的样本值变形为 $y_i=\ln x_i$，利用 $\bar{Y}$ 的分布求出 $EX=E(\mathrm{e}^Y)$ 以及 $\mu$ 的置信区间，而 $EX$ 是 $\mu$ 的单值函数，从而求出 $EX$ 的置信区间．

+++

#### 拓展解答 (1) 设相互独立的随机变量 $X_1,X_2,\cdots,X_n$ 均服从 $N(\mu,\sigma^2)$，

$$Y_i=|X_i-\mu|\ (i=1,2,\cdots,n),\quad Y=\frac{1}{n}\sum_{i=1}^{n}Y_i.$$

（Ⅰ）求 $Y_1$ 的概率密度；\
（Ⅱ）利用一阶矩求 $\sigma$ 的矩估计量；\
（Ⅲ）求 $EY$ 和 $DY$．
***
（Ⅰ）用定义法求 $f_{Y_1}(y)$．

当 $y\geqslant 0$ 时，

$$F_{Y_1}(y)=P\{Y_1\leqslant y\}=P\{|X_1-\mu|\leqslant y\}$$

$$=P\{-y\leqslant X_1-\mu\leqslant y\}=P\left\{-\frac{y}{\sigma}\leqslant\frac{X_1-\mu}{\sigma}\leqslant\frac{y}{\sigma}\right\}$$

$$=\Phi\left(\frac{y}{\sigma}\right)-\Phi\left(-\frac{y}{\sigma}\right)=2\Phi\left(\frac{y}{\sigma}\right)-1;$$

当 $y<0$ 时，$F_{Y_1}(y)=0$，故

$$f_{Y_1}(y)=F'_{Y_1}(y)=\begin{cases}\dfrac{2}{\sigma}\varphi\left(\dfrac{y}{\sigma}\right),&y\geqslant 0,\\0,&y<0,\end{cases}$$

其中 $\Phi(x)$ 为 $N(0,1)$ 的分布函数，$\varphi(x)=\dfrac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{x^2}{2}}$，$-\infty<x<+\infty$．

（Ⅱ）

$$EY_1=\int_{-\infty}^{+\infty}yf_{Y_1}(y)\mathrm{d}y=\int_{0}^{+\infty}\frac{2y}{\sigma}\varphi\left(\frac{y}{\sigma}\right)\mathrm{d}y$$

$$=2\sigma\int_{0}^{+\infty}\frac{y}{\sigma}\varphi\left(\frac{y}{\sigma}\right)\mathrm{d}\left(\frac{y}{\sigma}\right)$$

$$\xlongequal{\frac{y}{\sigma}=t}2\sigma\int_{0}^{+\infty}t\varphi(t)\mathrm{d}t=2\sigma\int_{0}^{+\infty}t\cdot\frac{1}{\sqrt{2\pi}}\cdot\mathrm{e}^{-\frac{t^2}{2}}\mathrm{d}t$$

$$=\frac{2\sigma}{\sqrt{2\pi}}\int_{0}^{+\infty}\mathrm{e}^{-\frac{t^2}{2}}\mathrm{d}\left(\frac{t^2}{2}\right)=\sqrt{\frac{2}{\pi}}\sigma,$$

故 $\sigma=\sqrt{\dfrac{\pi}{2}}\cdot EY_1$，所以 $\sigma$ 的矩估计量为 $\hat{\sigma}=\sqrt{\dfrac{\pi}{2}}\bar{Y}$，其中 $\bar{Y}=\dfrac{1}{n}\sum\limits_{i=1}^{n}Y_i=Y$．

（Ⅲ）记 $Z_i=X_i-\mu\sim N(0,\sigma^2)$，则 $EZ_i=0$，$DZ_i=\sigma^2$，故

$$E(|X_i-\mu|)=E(|Z_i|)=EY_i=\sqrt{\frac{2}{\pi}}\sigma,$$

$$D(|X_i-\mu|)=D(|Z_i|)=E(|Z_i|^2)-(E|Z_i|)^2$$

$$=E(Z_i^2)-\left(\sqrt{\frac{2}{\pi}}\sigma\right)^2=DZ_i+(EZ_i)^2-\left(\sqrt{\frac{2}{\pi}}\sigma\right)^2$$

$$=\sigma^2-\left(\sqrt{\frac{2}{\pi}}\sigma\right)^2=\left(1-\frac{2}{\pi}\right)\sigma^2,$$

所以

$$EY=E\left(\frac{1}{n}\sum_{i=1}^{n}|X_i-\mu|\right)=\frac{1}{n}\sum_{i=1}^{n}E(|Z_i|)=E(|Z_i|)=\sqrt{\frac{2}{\pi}}\sigma.$$

又 $X_1,X_2,\cdots,X_n$ 相互独立，故

$$DY=D\left(\frac{1}{n}\sum_{i=1}^{n}|X_i-\mu|\right)=\frac{1}{n^2}\sum_{i=1}^{n}DY_i=\frac{\sigma^2}{n}\left(1-\frac{2}{\pi}\right).$$

【注】此题（Ⅰ）（Ⅱ）实际上是 $2017$ 年考题，事实上这是一个结论：设 $X_1,X_2,\cdots,X_n$ 相互独立，且均服从 $N(\mu,\sigma^2)$，$Y=\dfrac{1}{n}\sum\limits_{i=1}^{n}|X_i-\mu|$，则

$$EY=\sqrt{\frac{2}{\pi}}\sigma,\quad DY=\frac{\sigma^2}{n}\left(1-\frac{2}{\pi}\right).$$

+++

#### 拓展解答 (2) 设总体 $X$ 的概率密度为

$$f(x;\theta)=\begin{cases}2\mathrm{e}^{-2(x-\theta)},&x>\theta,\\0,&x\leqslant\theta,\end{cases}$$

其中 $\theta\ (\theta>0)$ 为未知参数，$(X_1,X_2,\cdots,X_n)$ 为来自总体 $X$ 的简单随机样本．

（Ⅰ）求 $\theta$ 的矩估计量 $\hat{\theta}_1$ 与最大似然估计量 $\hat{\theta}_2$；\
（Ⅱ）问 $\hat{\theta}_1$ 和 $\hat{\theta}_2$ 是否为 $\theta$ 的无偏估计量？\
（Ⅲ）将 $\hat{\theta}_1,\hat{\theta}_2$ 修正为 $\hat{\theta}_3,\hat{\theta}_4$，使 $\hat{\theta}_3,\hat{\theta}_4$ 为 $\theta$ 的无偏估计，并比较 $\hat{\theta}_3,\hat{\theta}_4$ 的有效性．
***
（Ⅰ）

$$EX=\int_{-\infty}^{+\infty}x\cdot f(x;\theta)\mathrm{d}x=\int_{\theta}^{+\infty}x\cdot 2\mathrm{e}^{-2(x-\theta)}\mathrm{d}x\xlongequal{x-\theta=t}2\int_{0}^{+\infty}(t+\theta)\mathrm{e}^{-2t}\mathrm{d}t$$

$$=\int_{0}^{+\infty}2t\mathrm{e}^{-2t}\mathrm{d}t+\theta\int_{0}^{+\infty}2\mathrm{e}^{-2t}\mathrm{d}t$$

$$=\frac{1}{2}\int_{0}^{+\infty}(2t)^{2-1}\mathrm{e}^{-2t}\mathrm{d}(2t)-\theta\cdot\mathrm{e}^{-2t}\Big|_{0}^{+\infty}$$

$$=\frac{1}{2}\cdot\Gamma(2)+\theta=\frac{1}{2}\times 1+\theta=\frac{1}{2}+\theta,$$

故 $\theta$ 的矩估计量为 $\hat{\theta}_1=\bar{X}-\dfrac{1}{2}$．

似然函数为

$$L(\theta)=\prod_{i=1}^{n}f(x_i;\theta)=\begin{cases}2^n\mathrm{e}^{-2\sum\limits_{i=1}^{n}(x_i-\theta)},&x_i>\theta\ (i=1,2,\cdots,n),\\0,&\text{其他.}\end{cases}$$

当 $x_i>\theta$ 时，$L(\theta)>0$，取对数，得

$$\ln L(\theta)=n\ln 2-2\sum_{i=1}^{n}(x_i-\theta).$$

因为 $\dfrac{\mathrm{d}\ln L(\theta)}{\mathrm{d}\theta}=2n>0$，所以 $L(\theta)$ 单调增加．由于 $\theta$ 满足 $\theta<x_i\ (i=1,2,\cdots,n)$，所以 $\theta$ 取 $x_1,x_2,\cdots,x_n$ 中的最小值，$L(\theta)$ 取得最大值，故 $\theta$ 的最大似然估计量为

$$\hat{\theta}_2=\min\{X_1,X_2,\cdots,X_n\}.$$

（Ⅱ）由（Ⅰ），知 $\hat{\theta}_1=\bar{X}-\dfrac{1}{2}$，则

$$E(\hat{\theta}_1)=E(\bar{X})-\frac{1}{2}=\frac{1}{2}+\theta-\frac{1}{2}=\theta,$$

故 $\hat{\theta}_1$ 是 $\theta$ 的无偏估计量．

可求得 $\hat{\theta}_2=\min\{X_1,X_2,\cdots,X_n\}$ 的概率密度为

$$f(x)=\begin{cases}2n\mathrm{e}^{-2n(x-\theta)},&x>\theta,\\0,&\text{其他,}\end{cases}$$

故

$$E(\hat{\theta}_2)=\int_{-\infty}^{+\infty}x\cdot f(x)\mathrm{d}x=\int_{\theta}^{+\infty}x\cdot 2n\mathrm{e}^{-2n(x-\theta)}\mathrm{d}x$$

$$\xlongequal{x-\theta=u}\int_{0}^{+\infty}(u+\theta)\cdot 2n\mathrm{e}^{-2nu}\mathrm{d}u=\frac{1}{2n}+\theta\neq\theta,$$

所以 $\hat{\theta}_2$ 不是 $\theta$ 的无偏估计量．

（Ⅲ）由（Ⅱ），知 $E(\hat{\theta}_1)=\theta$，故取 $\hat{\theta}_3=\hat{\theta}_1=\bar{X}-\dfrac{1}{2}$．

$E(\hat{\theta}_2)=\dfrac{1}{2n}+\theta$，取 $\hat{\theta}_4=\hat{\theta}_2-\dfrac{1}{2n}$，则

$$E(\hat{\theta}_4)=E(\hat{\theta}_2)-\frac{1}{2n}=\theta,$$

这样选取得到 $\theta$ 的两个无偏估计量 $\hat{\theta}_3$ 和 $\hat{\theta}_4$．

下面比较 $D(\hat{\theta}_3)$ 与 $D(\hat{\theta}_4)$．

$$D(\hat{\theta}_3)=D\left(\bar{X}-\frac{1}{2}\right)=D(\bar{X})=\frac{DX}{n},$$

$$E(X^2)=\int_{-\infty}^{+\infty}x^2\cdot f(x;\theta)\mathrm{d}x=\int_{\theta}^{+\infty}x^2\cdot 2\mathrm{e}^{-2(x-\theta)}\mathrm{d}x$$

$$\xlongequal{x-\theta=t}\int_{0}^{+\infty}(t+\theta)^2\cdot 2\mathrm{e}^{-2t}\mathrm{d}t$$

$$=\int_{0}^{+\infty}t^2\cdot 2\mathrm{e}^{-2t}\mathrm{d}t+2\theta\int_{0}^{+\infty}t\cdot 2\mathrm{e}^{-2t}\mathrm{d}t+\theta^2\int_{0}^{+\infty}2\mathrm{e}^{-2t}\mathrm{d}t$$

$$=\frac{1}{2}+\theta+\theta^2,$$

故

$$DX=E(X^2)-(EX)^2=\frac{1}{2}+\theta+\theta^2-\left(\frac{1}{2}+\theta\right)^2=\frac{1}{4}.$$

所以 $D(\hat{\theta}_3)=\dfrac{1}{4n}$．

$$D(\hat{\theta}_4)=D\left(\hat{\theta}_2-\frac{1}{2n}\right)=D(\hat{\theta}_2),$$

又 $D(\hat{\theta}_2)=E(\hat{\theta}_2^2)-\left[E(\hat{\theta}_2)\right]^2$，而

$$E(\hat{\theta}_2^2)=\int_{-\infty}^{+\infty}x^2\cdot f(x)\mathrm{d}x=\int_{\theta}^{+\infty}x^2\cdot 2n\mathrm{e}^{-2n(x-\theta)}\mathrm{d}x$$

$$\xlongequal{x-\theta=t}\int_{0}^{+\infty}(t+\theta)^2\cdot 2n\mathrm{e}^{-2nt}\mathrm{d}t$$

$$=\int_{0}^{+\infty}t^2\cdot 2n\mathrm{e}^{-2nt}\mathrm{d}t+2\theta\int_{0}^{+\infty}t\cdot 2n\mathrm{e}^{-2nt}\mathrm{d}t+\theta^2\int_{0}^{+\infty}2n\mathrm{e}^{-2nt}\mathrm{d}t$$

$$=\frac{2}{(2n)^2}+\frac{2\theta}{2n}+\theta^2=\frac{1}{2n^2}+\frac{\theta}{n}+\theta^2,$$

故

$$D(\hat{\theta}_2)=\frac{1}{2n^2}+\frac{\theta}{n}+\theta^2-\left(\frac{1}{2n}+\theta\right)^2=\frac{1}{4n^2}.$$

显然 $D(\hat{\theta}_2)=\dfrac{1}{4n^2}<\dfrac{1}{4n}=D(\hat{\theta}_3)\ (n>1)$，所以 $\hat{\theta}_4$ 比 $\hat{\theta}_3$ 有效．

【注】题中计算中用到 $\Gamma(\alpha)=\displaystyle\int_{0}^{+\infty}x^{\alpha-1}\mathrm{e}^{-x}\mathrm{d}x\ (\alpha>0)$．

$\Gamma(\alpha+1)=\alpha\Gamma(\alpha)$，$\Gamma(n+1)=n!$，$\Gamma\left(\dfrac{1}{2}\right)=\sqrt{\pi}$，$\Gamma(1)=1$．

$\Gamma$ 函数在考试中常用到．
