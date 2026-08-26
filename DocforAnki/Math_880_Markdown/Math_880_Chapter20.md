---
quizify:
  format: 1
  deck: Math_880::Chapter_20
  tags: [Math, 880题, 数一, 第二十章, 大数定律与中心极限定理]
---

+++

#### 基础选择 (1) 设 $X_1,X_2,\cdots,X_n$ 是总体 $X$ 的简单随机样本，且 $E(X^k)=a_k$，$k=1,2,3,4$，根据中心极限定理，当 $n$ 充分大时，$Y_n=\frac{1}{n}\sum_{i=1}^{n}X_i^2$ 近似服从（　）．

;;;
A. $N\left(a_2,\dfrac{a_4-a_2^2}{n}\right)$
B. $N(a_2,a_4-a_2^2)$
C. $N\left(a_1,\dfrac{a_4-a_2^2}{n}\right)$
D. $N(a_2,a_2^2)$
;;;A
***
由已知，$X_1,X_2,\cdots,X_n$ 独立同分布，故 $X_1^2,X_2^2,\cdots,X_n^2$ 也独立同分布，又

$$E(X_i^2)=a_2,\quad D(X_i^2)=E(X_i^4)-\left[E(X_i^2)\right]^2=a_4-a_2^2.$$

根据独立同分布的中心极限定理，可知

$$Z_n\xlongequal{记}\frac{\sum\limits_{i=1}^{n}X_i^2-na_2}{\sqrt{n(a_4-a_2^2)}}=\frac{\frac{1}{n}\sum\limits_{i=1}^{n}X_i^2-a_2}{\sqrt{\frac{1}{n}(a_4-a_2^2)}}=\frac{Y_n-a_2}{\sqrt{\frac{1}{n}(a_4-a_2^2)}}$$

的极限分布为标准正态分布，故当 $n$ 充分大时，$Z_n$ 近似服从标准正态分布，所以 $Y_n$ 服从 $N\left(a_2,\dfrac{a_4-a_2^2}{n}\right)$．

+++

#### 基础选择 (2) 设随机变量 $X_1,X_2,\cdots,X_n$ 相互独立，记 $Y_n=X_1+X_2+\cdots X_n$，根据列维—林德伯格中心极限定理，$Y_n$ 近似服从正态分布（$n$ 充分大），则只要 $X_1,X_2,\cdots,X_n$（　）．

;;;
A. 服从同一离散型分布
B. 服从同一连续型分布
C. 服从同一指数分布
D. 具有相同的期望与方差
;;;C
***
列维—林德伯格中心极限定理的条件是 $X_1,X_2,\cdots,X_n$ **独立同分布，且期望与方差均存在**．

满足选项 A，B 的随机变量的期望或方差不一定存在，故排除 A，B．

对于 D，有相同的期望与方差未必有相同的分布，故排除 D．

只有 **C** 正确，指数分布的期望与方差均存在．

+++

#### 基础选择 (3) 设 $X_1,X_2,\cdots,X_n$ 是独立同分布的随机变量序列，且 $E(X_i^2)<+\infty$，则对任意 $\varepsilon$，有（　）．

;;;
A. $\lim\limits_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i^2\right|<\varepsilon\right\}=0$
B. $\lim\limits_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i^2-E(X_i^2)\right|<\varepsilon\right\}=0$
C. $\lim\limits_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i^2-E(X_i^2)\right|<\varepsilon\right\}=1$
D. $\lim\limits_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i^2\right|\geqslant\varepsilon\right\}=0$
;;;C
***
依题设，可知 $X_1^2,X_2^2,\cdots,X_n^2$ 独立同分布，根据**辛钦大数定律**，

$$\lim_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i^2-E(X_i^2)\right|<\varepsilon\right\}=1,$$

即样本的二阶原点矩依概率收敛于随机变量的二阶原点矩，即 $\frac{1}{n}\sum_{i=1}^{n}X_i^2\xrightarrow{P}E(X_i^2)$．

+++

#### 基础填空 (1) 设随机变量 $X_i$ 服从二项分布 $B(i,0.2)$，$i=1,2,\cdots,10$，且 $X_1,X_2,\cdots,X_{10}$ 相互独立，则根据切比雪夫不等式，有 $P\left\{6<\sum_{i=1}^{10}X_i<16\right\}\geqslant$ ________．
***
$0.648$．

由 $X_1,X_2,\cdots,X_{10}$ 相互独立，及 $X_i\sim B(i,0.2)$，可知 $\sum\limits_{i=1}^{10}X_i\sim B(55,0.2)$，所以

$$E\left(\sum_{i=1}^{10}X_i\right)=11,\quad D\left(\sum_{i=1}^{10}X_i\right)=8.8,$$

故

$$P\left\{6<\sum_{i=1}^{10}X_i<16\right\}=P\left\{\left|\sum_{i=1}^{10}X_i-11\right|<5\right\}\geqslant 1-\frac{8.8}{5^2}=0.648.$$

【注】① 在独立的条件下，二项分布具有**可加性**，即：设 $X\sim B(m,p)$，$Y\sim B(n,p)$，且 $X$ 与 $Y$ 相互独立，则 $X+Y\sim B(m+n,p)$．

② 切比雪夫不等式：$P\{|X-EX|<\varepsilon\}\geqslant 1-\dfrac{DX}{\varepsilon^2}$，等价地 $P\{|X-EX|\geqslant\varepsilon\}\leqslant\dfrac{DX}{\varepsilon^2}$．

+++

#### 基础填空 (2) 设 $X$ 与 $Y$ 满足：$EX=-2$，$EY=2$，$DX=1$，$DY=4$，$\rho_{XY}=-\frac{1}{2}$，则根据切比雪夫不等式，有 $P\{|X+Y|\geqslant 6\}\leqslant$ ________．
***
$\dfrac{1}{12}$．

$$E(X+Y)=EX+EY=-2+2=0,$$

$$D(X+Y)=DX+DY+2\rho_{XY}\sqrt{DX\cdot DY}=1+4-2\times\frac{1}{2}\times 2=3,$$

故

$$P\{|X+Y-0|\geqslant 6\}\leqslant\frac{3}{36}=\frac{1}{12}.$$

+++

#### 基础填空 (3) 设 $X$ 在区间 $[-1,b]$ 上服从均匀分布，由切比雪夫不等式，有 $P\{|X-1|<\varepsilon\}\geqslant\frac{2}{3}$，则 $b=$ ________，$\varepsilon=$ ________．
***
$3$，$2$．

由已知，$EX=\dfrac{b-1}{2}$，$DX=\dfrac{(b+1)^2}{12}$．又 $P\{|X-EX|<\varepsilon\}\geqslant 1-\dfrac{DX}{\varepsilon^2}$．

而已知

$$P\{|X-1|<\varepsilon\}\geqslant\frac{2}{3},$$

故 $EX=1=\dfrac{b-1}{2}$，得 $b=3$，$DX=\dfrac{16}{12}=\dfrac{4}{3}$，所以 $1-\dfrac{DX}{\varepsilon^2}=\dfrac{2}{3}$，故 $\varepsilon=2$．

+++

#### 基础填空 (4) 设随机变量 $X_1,X_2,\cdots,X_{200}$ 相互独立且同分布，$P\{X_1=0\}=P\{X_1=1\}=0.5$，则根据棣莫弗—拉普拉斯中心极限定理，可知 $P\left\{\sum_{i=1}^{100}(X_{2i}-X_{2i-1})^2\leqslant 59.8\right\}=$ ________．（$\Phi(1.96)=0.975$）
***
$0.975$．

令 $Y_i=X_{2i}-X_{2i-1}$，$i=1,2,\cdots,100$，则 $Y_i$ 与 $Y_i^2$ 的分布律分别为

$$\begin{array}{c|ccc}Y_i&-1&0&1\\\hline p&0.25&0.5&0.25\end{array}\qquad\begin{array}{c|cc}Y_i^2&0&1\\\hline p&0.5&0.5\end{array}$$

由于 $X_1,X_2,\cdots,X_{200}$ 相互独立且同分布，故 $Y_1^2,Y_2^2,\cdots,Y_{100}^2$ 也相互独立，且服从参数为 $0.5$ 的 $0-1$ 分布，由此可知 $\sum\limits_{i=1}^{100}Y_i^2$ 服从二项分布 $B(100,0.5)$．根据棣莫弗—拉普拉斯中心极限定理，可知 $\sum\limits_{i=1}^{100}Y_i^2$ 近似服从正态分布 $N(\mu,\sigma^2)$，且

$$\mu=np=50,\quad \sigma^2=np(1-p)=25,$$

故

$$P\left\{\sum_{i=1}^{100}(X_{2i}-X_{2i-1})^2\leqslant 59.8\right\}=P\left\{\sum_{i=1}^{100}Y_i^2\leqslant 59.8\right\}\approx\Phi\left(\frac{59.8-50}{\sqrt{25}}\right)=\Phi(1.96)=0.975.$$

+++

#### 基础解答 (1) 设一条生产线的合格率为 $0.8$，要使一批产品的合格率在 $76\%$ 与 $84\%$ 之间的概率不小于 $90\%$，问这批产品至少要生产多少件？
***
**解法 1**　设至少要生产 $m$ 件产品，记随机变量 $X$ 为 $m$ 件产品中合格品的件数，则依题设，$X\sim B(m,0.8)$，现要确定 $m$，使之满足 $P\left\{0.76<\dfrac{X}{m}<0.84\right\}\geqslant 0.90$，利用切比雪夫不等式，得

$$P\left\{0.76<\frac{X}{m}<0.84\right\}=P\{|X-0.8m|<0.04m\}$$

$$\geqslant 1-\frac{0.8m\times 0.2}{(0.04m)^2}=1-\frac{100}{m}\geqslant 0.90,$$

故 $m\geqslant 1\,000$，即至少要生产 $1\,000$ 件才能满足要求．

**解法 2**　利用棣莫弗—拉普拉斯定理估计 $m$ 的值，当 $n$ 比较大时，$X$ 近似服从正态分布 $N(0.8m,0.16m)$，故

$$P\left\{0.76<\frac{X}{m}<0.84\right\}=P\left\{\left|\frac{X-0.8m}{0.4\sqrt{m}}\right|<\frac{0.04m}{0.4\sqrt{m}}\right\}$$

$$\approx 2\Phi(0.1\sqrt{m})-1\geqslant 0.90,$$

查正态分布表可得，$0.1\sqrt{m}\geqslant 1.65$，解得 $m\geqslant 272.25$，故 $m$ 至少为 $273$．

【注】比较解法 1 与解法 2，可知**中心极限定理比切比雪夫不等式要精确**．

+++

#### 基础解答 (2) 设随机变量 $X$ 的概率密度为 $f(x)=\begin{cases}\dfrac{x^n\mathrm{e}^{-x}}{n!},&x\geqslant 0,\\0,&\text{其他}\end{cases}$（$n$ 为正整数），利用切比雪夫不等式证明：$P\{0<X<2(n+1)\}\geqslant\dfrac{n}{n+1}$．
***
**证**　先求 $X$ 的期望和方差．

$$EX=\int_{-\infty}^{+\infty}xf(x)\mathrm{d}x=\frac{1}{n!}\int_{0}^{+\infty}x^{n+1}\mathrm{e}^{-x}\mathrm{d}x=\frac{1}{n!}\Gamma(n+2)=\frac{1}{n!}(n+1)!=n+1,$$

$$E(X^2)=\int_{-\infty}^{+\infty}x^2f(x)\mathrm{d}x=\frac{1}{n!}\int_{0}^{+\infty}x^{n+2}\mathrm{e}^{-x}\mathrm{d}x=\frac{1}{n!}\Gamma(n+3)=\frac{1}{n!}(n+2)!=(n+1)(n+2),$$

$$DX=E(X^2)-(EX)^2=(n+1)(n+2)-(n+1)^2=n+1.$$

由切比雪夫不等式，

$$P\{0<X<2(n+1)\}=P\{-(n+1)<X-(n+1)<n+1\}=P\{|X-(n+1)|<n+1\}$$

$$\geqslant 1-\frac{DX}{(n+1)^2}=1-\frac{n+1}{(n+1)^2}=\frac{n}{n+1}.$$

+++

#### 基础解答 (3) 设随机变量序列 $X_1,X_2,\cdots,X_n$ 独立，$X_i$ 的分布律为

$$\begin{array}{c|ccc}X_i&-ia&0&ia\\\hline p&\dfrac{1}{2i^2}&1-\dfrac{1}{i^2}&\dfrac{1}{2i^2}\end{array}$$

其中 $i=1,2,\cdots,n$，利用大数定律，证明：$\lim_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i\right|\geqslant\varepsilon\right\}=0$．
***
**证**　先验证满足大数定律的条件．

由已知

$$EX_i=0,\quad E(X_i^2)=\frac{2i^2a^2\times 1}{2i^2}=a^2,$$

所以

$$E\left(\frac{1}{n}\sum_{i=1}^{n}X_i\right)=\frac{1}{n}\sum_{i=1}^{n}EX_i=0,$$

$$D\left(\frac{1}{n}\sum_{i=1}^{n}X_i\right)=\frac{1}{n^2}\sum_{i=1}^{n}DX_i=\frac{a^2}{n},$$

满足**切比雪夫大数定律**条件，故

$$\lim_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i-0\right|<\varepsilon\right\}=1,$$

即

$$\lim_{n\to\infty}P\left\{\left|\frac{1}{n}\sum_{i=1}^{n}X_i\right|\geqslant\varepsilon\right\}=0.$$
