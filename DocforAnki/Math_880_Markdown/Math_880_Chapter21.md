---
quizify:
  format: 1
  deck: Math_880::Chapter_21
  tags: [Math, 880题, 数一, 第二十一章, 数理统计的基本概念]
---

+++

#### 基础选择 (1) 设 $(X_1,X_2,X_3)$ 为总体 $X\sim N(0,\sigma^2)$ 的简单随机样本，则统计量 $U=\dfrac{X_1-X_2}{\sqrt{2}\,|X_3|}$ 服从的分布为（　）．

;;;
A. $t(1)$
B. $t(2)$
C. $F(1,1)$
D. $F(2,1)$
;;;A
***
由已知，

$$X_1-X_2\sim N(0,2\sigma^2),\quad \frac{X_1-X_2}{\sqrt{2}\sigma}\sim N(0,1),$$

又 $\dfrac{X_3-0}{\sigma}\sim N(0,1)$，故 $\left(\dfrac{X_3}{\sigma}\right)^2\sim\chi^2(1)$，所以

$$\frac{\dfrac{X_1-X_2}{\sqrt{2}\sigma}}{\sqrt{\dfrac{\left(\dfrac{X_3}{\sigma}\right)^2}{1}}}=\frac{X_1-X_2}{\sqrt{2}\,|X_3|}\sim t(1).$$

+++

#### 基础选择 (2) 设随机变量 $X,Y$ 均服从 $N(0,1)$，则（　）．

;;;
A. $X+Y$ 服从正态分布
B. $X^2+Y^2$ 服从 $\chi^2$ 分布
C. $\dfrac{X^2}{Y^2}$ 服从 $F$ 分布
D. $X^2$ 与 $Y^2$ 均服从 $\chi^2$ 分布
;;;D
***
由已知，$X^2\sim\chi^2(1)$，$Y^2\sim\chi^2(1)$，知 **D** 正确．

由于没有 $X,Y$ 相互独立的条件，所以 A，B，C 未必成立．

+++

#### 基础选择 (3) 设总体 $X\sim N(\mu,\sigma^2)$，$(X_1,X_2,\cdots,X_{16})$ 为总体 $X$ 的简单随机样本，$\bar{X}=\dfrac{1}{16}\sum_{i=1}^{16}X_i$，且 $P\{|X-\mu|<k\}=P\{|\bar{X}-\mu|<4\}$，则 $k=$（　）．

;;;
A. $4$
B. $4\sigma$
C. $16$
D. $16\sigma$
;;;C
***
由 $X\sim N(\mu,\sigma^2)$，则 $\bar{X}\sim N\left(\mu,\dfrac{\sigma^2}{16}\right)$，故

$$\frac{X-\mu}{\sigma}\sim N(0,1),\quad \frac{4(\bar{X}-\mu)}{\sigma}\sim N(0,1),$$

于是

$$P\{|X-\mu|<k\}=P\left\{\left|\frac{X-\mu}{\sigma}\right|<\frac{k}{\sigma}\right\}=2\Phi\left(\frac{k}{\sigma}\right)-1,$$

$$P\{|\bar{X}-\mu|<4\}=P\left\{\left|\frac{4(\bar{X}-\mu)}{\sigma}\right|<\frac{4^2}{\sigma}\right\}=2\Phi\left(\frac{4^2}{\sigma}\right)-1,$$

其中 $\Phi(x)$ 为 $N(0,1)$ 的分布函数，故由已知，$\dfrac{k}{\sigma}=\dfrac{4^2}{\sigma}$，即 $k=4^2=16$．

+++

#### 基础选择 (4) 设 $(X_1,X_2,\cdots,X_{10})$ 是来自总体 $X\sim N(0,1)$ 的简单随机样本，则统计量 $T=\dfrac{1}{4}\left(\sum_{i=1}^{4}X_i\right)^2+\dfrac{1}{6}\left(\sum_{i=5}^{10}X_i\right)^2$ 服从的分布为（　）．

;;;
A. $N(0,2)$
B. $\chi^2(10)$
C. $\chi^2(2)$
D. $N(0,10)$
;;;C
***
依题设，知 $\sum_{i=1}^{4}X_i\sim N(0,4)$，$\sum_{i=5}^{10}X_i\sim N(0,6)$，故

$$\frac{1}{\sqrt{4}}\sum_{i=1}^{4}X_i\sim N(0,1),\quad \frac{1}{\sqrt{6}}\sum_{i=5}^{10}X_i\sim N(0,1).$$

由 $\chi^2$ 分布的定义，知

$$\left(\frac{1}{\sqrt{4}}\sum_{i=1}^{4}X_i\right)^2\sim\chi^2(1),\quad \left(\frac{1}{\sqrt{6}}\sum_{i=5}^{10}X_i\right)^2\sim\chi^2(1),$$

根据 $\chi^2$ 分布的可加性，知

$$T=\frac{1}{4}\left(\sum_{i=1}^{4}X_i\right)^2+\frac{1}{6}\left(\sum_{i=5}^{10}X_i\right)^2\sim\chi^2(2).$$

+++

#### 基础填空 (1) 从总体 $X\sim N(3.4,6^2)$ 中抽取样本 $(X_1,X_2,\cdots,X_n)$，$\bar{X}=\dfrac{1}{n}\sum_{i=1}^{n}X_i$，若 $\bar{X}$ 位于 $(1.4,5.4)$ 内的概率不小于 $0.95$，则样本容量 $n$ 至少应取 ________．（已知 $\Phi(1.96)=0.975$）
***
$35$．

由 $X\sim N(3.4,6^2)$，知 $\bar{X}\sim N\left(3.4,\dfrac{6^2}{n}\right)$，故 $\dfrac{\bar{X}-3.4}{6/\sqrt{n}}\sim N(0,1)$，所以

$$P\{1.4<\bar{X}<5.4\}=P\{-2<\bar{X}-3.4<2\}$$

$$=P\{|\bar{X}-3.4|<2\}=P\left\{\frac{|\bar{X}-3.4|}{6/\sqrt{n}}<\frac{2\sqrt{n}}{6}\right\}$$

$$=2\Phi\left(\frac{\sqrt{n}}{3}\right)-1\geqslant 0.95,$$

即 $\Phi\left(\dfrac{\sqrt{n}}{3}\right)\geqslant 0.975=\Phi(1.96)$．

由 $\Phi(x)$ 单调增加，知 $\dfrac{\sqrt{n}}{3}\geqslant 1.96$，即 $n\geqslant(1.96\times 3)^2\approx 34.57$，所以 $n$ 至少应取 $35$．

+++

#### 基础填空 (2) 设总体 $N(\mu,4^2)$ 的简单随机样本为 $(X_1,X_2,\cdots,X_{10})$，样本方差为 $S^2$，已知 $P\{S^2>a\}=0.1$，则 $a\approx$ ________．（已知 $\chi^2_{0.1}(9)=14.684$，上侧分位数）
***
$26.1$．

依题设，$\dfrac{(n-1)S^2}{\sigma^2}\sim\chi^2(n-1)$，$n=10$，$\sigma^2=4^2$，故

$$P\{S^2>a\}=P\left\{\frac{(10-1)S^2}{4^2}>\frac{(10-1)a}{4^2}\right\}$$

$$=P\left\{\frac{9S^2}{4^2}>\frac{9a}{16}\right\}=0.1,$$

故 $\dfrac{9a}{16}=\chi^2_{0.1}(10-1)=\chi^2_{0.1}(9)=14.684$，所以 $a\approx 26.1$．

+++

#### 基础填空 (3) 设随机变量 $X\sim F(n,n)$，且 $P\{X>a\}=0.05$，则 $P\left\{X>\dfrac{1}{a}\right\}=$ ________．
***
$0.95$．

由 $X\sim F(n,n)$ 及 $F$ 分布的定义，知 $X\sim\dfrac{\chi^2(n)/n}{\chi^2(n)/n}$，故 $\dfrac{1}{X}\sim F(n,n)$，即 $X$ 与 $\dfrac{1}{X}$ 都服从 $F(n,n)$，故 $P\{X>a\}=P\left\{\dfrac{1}{X}>a\right\}$，所以

$$P\left\{X>\frac{1}{a}\right\}=P\left\{\frac{1}{X}<a\right\}=1-P\left\{\frac{1}{X}>a\right\}$$

$$=1-P\{X>a\}=1-0.05=0.95.$$

+++

#### 基础填空 (4) 设 $X\sim t(n)$，$Y\sim F(1,n)$，给定 $\alpha\,(0<\alpha<0.5)$，常数 $k$ 满足 $P\{X>k\}=\alpha$，则 $P\{Y>k^2\}=$ ________．
***
$2\alpha$．

由 $X\sim t(n)$，则 $X^2\sim F(1,n)$，所以

$$P\{Y>k^2\}=P\{X^2>k^2\}=P\{X>k\}+P\{X<-k\}=2\alpha.$$

【注】设 $t=\dfrac{X}{\sqrt{\dfrac{Y}{n}}}\sim t(n)$，则 $t^2\sim F(1,n)$，$\dfrac{1}{t^2}\sim F(n,1)$，见《李林考研数学系列概率论与数理统计辅导讲义》．

+++

#### 基础解答 (1) 设 $(X_1,X_2,\cdots,X_9)$ 为总体 $X\sim N(0,2^2)$ 的简单随机样本，若 $a,b,c$ 使 $X=a(X_1+X_2)^2+b(X_3+X_4+X_5)^2+c(X_6+X_7+X_8+X_9)^2$ 服从 $\chi^2$ 分布，求 $a,b,c$ 的值及 $\chi^2$ 分布的自由度．
***
由 $X_1,X_2,\cdots,X_9$ 独立同分布，且均服从 $N(0,2^2)$，故有

$$X_1+X_2\sim N(0,2^2+2^2)=N(0,8),$$

$$X_3+X_4+X_5\sim N(0,2^2+2^2+2^2)=N(0,12),$$

$$X_6+X_7+X_8+X_9\sim N(0,2^2+2^2+2^2+2^2)=N(0,16),$$

从而

$$\frac{X_1+X_2}{\sqrt{8}}\sim N(0,1),\quad \left(\frac{X_1+X_2}{\sqrt{8}}\right)^2\sim\chi^2(1),$$

$$\frac{X_3+X_4+X_5}{\sqrt{12}}\sim N(0,1),\quad \left(\frac{X_3+X_4+X_5}{\sqrt{12}}\right)^2\sim\chi^2(1),$$

$$\frac{X_6+X_7+X_8+X_9}{\sqrt{16}}\sim N(0,1),\quad \left(\frac{X_6+X_7+X_8+X_9}{\sqrt{16}}\right)^2\sim\chi^2(1).$$

由独立性及 $\chi^2$ 分布的可加性，知

$$\frac{(X_1+X_2)^2}{8}+\frac{(X_3+X_4+X_5)^2}{12}+\frac{(X_6+X_7+X_8+X_9)^2}{16}\sim\chi^2(3),$$

故 $a=\dfrac{1}{8}$，$b=\dfrac{1}{12}$，$c=\dfrac{1}{16}$，自由度 $n=3$．

+++

#### 基础解答 (2) 设总体 $X\sim N(0,\sigma^2)$，$(X_1,X_2,\cdots,X_{10})$ 为 $X$ 的简单随机样本，求下列统计量的分布．

（Ⅰ）$T_1=\dfrac{7}{3}\cdot\dfrac{(X_1+X_2+X_3)^2}{X_4^2+\cdots+X_{10}^2}$；\
（Ⅱ）$T_2=\sqrt{\dfrac{7}{3}}\cdot\dfrac{X_1+X_2+X_3}{\sqrt{X_4^2+\cdots+X_{10}^2}}$；\
（Ⅲ）$T_3=\dfrac{7}{3}\cdot\dfrac{X_1^2+X_2^2+X_3^2}{X_4^2+\cdots+X_{10}^2}$．
***
由 $X\sim N(0,\sigma^2)$，知 $X_i\sim N(0,\sigma^2)$，$X_1+X_2+X_3\sim N(0,3\sigma^2)$，记

$$U=\frac{X_1+X_2+X_3}{\sqrt{3}\sigma}\sim N(0,1),\quad V=\sum_{i=4}^{10}\left(\frac{X_i}{\sigma}\right)^2=\frac{\sum_{i=4}^{10}X_i^2}{\sigma^2}\sim\chi^2(7),$$

故 $U^2=\dfrac{(X_1+X_2+X_3)^2}{3\sigma^2}\sim\chi^2(1)$．

记 $W=\dfrac{X_1^2+X_2^2+X_3^2}{\sigma^2}\sim\chi^2(3)$，又 $U$ 与 $V$ 相互独立，则：

（Ⅰ）$T_1=\dfrac{U^2/1}{V/7}=\dfrac{7}{3}\cdot\dfrac{(X_1+X_2+X_3)^2}{X_4^2+\cdots+X_{10}^2}\sim F(1,7)$；

（Ⅱ）$T_2=\dfrac{U}{\sqrt{V/7}}=\sqrt{\dfrac{7}{3}}\cdot\dfrac{X_1+X_2+X_3}{\sqrt{X_4^2+\cdots+X_{10}^2}}\sim t(7)$；

（Ⅲ）$T_3=\dfrac{W/3}{V/7}=\dfrac{7}{3}\cdot\dfrac{X_1^2+X_2^2+X_3^2}{X_4^2+\cdots+X_{10}^2}\sim F(3,7)$．（由已知，$W$ 与 $V$ 相互独立）

+++

#### 综合选择 (1) 设 $(X_1,X_2,\cdots,X_n)$ 为总体 $X\sim N(0,\sigma^2)$ 的简单随机样本，$S_1^2=\sum_{i=1}^{n}(X_i-\bar{X})^2$，$\bar{X}=\dfrac{1}{n}\sum_{i=1}^{n}X_i$，则下列选项服从 $t(n-1)$ 分布的统计量为（　）．

;;;
A. $\dfrac{\sqrt{n}\,\bar{X}}{\sqrt{n-1}S_1}$
B. $\dfrac{\sqrt{n-1}\,\bar{X}}{\sqrt{n}S_1}$
C. $\dfrac{\sqrt{n(n-1)}\,\bar{X}}{S_1}$
D. $\dfrac{\bar{X}}{\sqrt{n(n-1)}S_1}$
;;;C
***
记 $S^2=\dfrac{1}{n-1}\sum_{i=1}^{n}(X_i-\bar{X})^2$，则 $S^2$ 为样本方差，由于 $\dfrac{\bar{X}-\mu}{S/\sqrt{n}}\sim t(n-1)$，故

$$T=\frac{\bar{X}-0}{\dfrac{S}{\sqrt{n}}}=\frac{\bar{X}}{\dfrac{S_1}{\sqrt{n-1}}\cdot\dfrac{1}{\sqrt{n}}}=\frac{\sqrt{n(n-1)}\,\bar{X}}{S_1}\sim t(n-1).$$

+++

#### 综合选择 (2) 设 $(X_1,X_2,\cdots,X_n)$ 为总体 $X$ 的简单随机样本，$\bar{X}=\dfrac{1}{n}\sum_{i=1}^{n}X_i$，则 $E(X^2)$ 的矩估计量为（　）．

;;;
A. $\bar{X}^2+\dfrac{1}{n}\sum_{i=1}^{n}(X_i-\bar{X})^2$
B. $\bar{X}^2+\dfrac{1}{n-1}\sum_{i=1}^{n}(X_i-\bar{X})^2$
C. $\dfrac{1}{n-1}\sum_{i=1}^{n}(X_i-\bar{X})^2$
D. $\dfrac{1}{n}\sum_{i=1}^{n}(X_i-\bar{X})^2$
;;;A
***
由于 $E(X^2)=DX+(EX)^2$，而 $DX$ 与 $EX$ 的矩估计量分别为 $\dfrac{1}{n}\sum_{i=1}^{n}(X_i-\bar{X})^2$ 与 $\bar{X}$，故 $E(X^2)$ 的矩估计量为

$$\bar{X}^2+\frac{1}{n}\sum_{i=1}^{n}(X_i-\bar{X})^2.$$

+++

#### 综合选择 (3) 设总体 $X$ 与总体 $Y$ 相互独立，且都服从 $N(\mu,\sigma^2)$，$\bar{X}$ 与 $\bar{Y}$ 分别为来自总体 $X,Y$ 的样本均值，样本容量均为 $n$，则当 $n$ 固定时，$P\{|\bar{X}-\bar{Y}|>\sigma\}$ 的值随着 $\sigma$ 增大（　）．

;;;
A. 单调增加
B. 单调减少
C. 保持不变
D. 增减性不确定
;;;C
***
先求 $\bar{X}-\bar{Y}$ 的分布．

由已知，$\bar{X}\sim N\left(\mu,\dfrac{\sigma^2}{n}\right)$，$\bar{Y}\sim N\left(\mu,\dfrac{\sigma^2}{n}\right)$，且 $\bar{X}$ 与 $\bar{Y}$ 相互独立，故 $\bar{X}-\bar{Y}\sim N\left(0,\dfrac{2\sigma^2}{n}\right)$，所以 $\dfrac{\bar{X}-\bar{Y}}{\sigma}\sim N\left(0,\dfrac{2}{n}\right)$．

当 $n$ 固定时，

$$P\{|\bar{X}-\bar{Y}|>\sigma\}=1-P\left\{\left|\frac{\bar{X}-\bar{Y}}{\sigma}\right|\leqslant 1\right\}=1-\left[\Phi\left(\sqrt{\frac{n}{2}}\right)-\Phi\left(-\sqrt{\frac{n}{2}}\right)\right]$$

$$=2\left[1-\Phi\left(\sqrt{\frac{n}{2}}\right)\right],$$

其中 $\Phi(x)$ 为 $N(0,1)$ 的概率分布函数，所以 $P\{|\bar{X}-\bar{Y}|>\sigma\}$ 与 $\sigma$ 无关，**C** 正确．

+++

#### 综合解答 (1) 设总体 $X\sim N(0,1)$，$(X_1,X_2,\cdots,X_{2n})$ 为 $X$ 的简单随机样本，求下列统计量的分布．

（Ⅰ）$T_1=\dfrac{1}{2}\sum_{i=1}^{2n}X_i^2+\sum_{i=1}^{n}X_{2i-1}X_{2i}$；\
（Ⅱ）$T_2=\dfrac{\sqrt{2n-1}X_1}{\sqrt{\sum_{i=2}^{2n}X_i^2}}$；\
（Ⅲ）$T_3=\dfrac{(2n-3)\sum_{i=1}^{3}X_i^2}{3\sum_{i=4}^{2n}X_i^2}$．
***
（Ⅰ）

$$T_1=\frac{1}{2}\sum_{i=1}^{2n}X_i^2+\sum_{i=1}^{n}X_{2i-1}X_{2i}$$

$$=\frac{1}{2}(X_1^2+X_2^2+\cdots+X_{2n-1}^2+X_{2n}^2)+X_1X_2+X_3X_4+\cdots+X_{2n-1}X_{2n}$$

$$=\frac{1}{2}(X_1+X_2)^2+\frac{1}{2}(X_3+X_4)^2+\cdots+\frac{1}{2}(X_{2n-1}+X_{2n})^2$$

$$=\sum_{i=1}^{n}\left(\frac{X_{2i-1}+X_{2i}}{\sqrt{2}}\right)^2\xlongequal{\text{记}}\sum_{i=1}^{n}Y_i^2.$$

由 $X_{2i-1}\sim N(0,1)$，$X_{2i}\sim N(0,1)$，知 $X_{2i-1}+X_{2i}\sim N(0,2)$，故

$$Y_i=\frac{X_{2i-1}+X_{2i}}{\sqrt{2}}\sim N(0,1),$$

所以 $T_1=\sum_{i=1}^{n}Y_i^2\sim\chi^2(n)$．

（Ⅱ）

$$T_2=\frac{\sqrt{2n-1}X_1}{\sqrt{\sum_{i=2}^{2n}X_i^2}}=\frac{X_1}{\sqrt{\dfrac{\sum_{i=2}^{2n}X_i^2}{2n-1}}}\sim t(2n-1)$$

（这里 $\sum_{i=2}^{2n}X_i^2\sim\chi^2(2n-1)$）．

（Ⅲ）由 $\sum_{i=1}^{3}X_i^2\sim\chi^2(3)$，$\sum_{i=4}^{2n}X_i^2\sim\chi^2(2n-3)$，且相互独立，故

$$T_3=\frac{(2n-3)\sum_{i=1}^{3}X_i^2}{3\sum_{i=4}^{2n}X_i^2}=\frac{\dfrac{\sum_{i=1}^{3}X_i^2}{3}}{\dfrac{\sum_{i=4}^{2n}X_i^2}{2n-3}}\sim F(3,2n-3).$$

+++

#### 综合解答 (2) 设随机变量 $X_1,X_2,X_3$ 相互独立且均服从 $N(0,\sigma^2)$，证明：$T=\sqrt{\dfrac{2}{3}}\dfrac{X_1+X_2+X_3}{|X_2-X_3|}$ 服从 $t(1)$ 分布．
***
利用 $t$ 分布的定义证明，令 $Y_1=X_2+X_3$，$Y_2=X_2-X_3$，则

$$\mathrm{Cov}(Y_1,Y_2)=E(Y_1Y_2)-EY_1EY_2$$

$$=E[(X_2+X_3)(X_2-X_3)]$$

$$=E(X_2^2)-E(X_3^2)$$

$$=\sigma^2-\sigma^2=0,$$

所以 $Y_1,Y_2$ 相互独立且均服从 $N(0,2\sigma^2)$．又由已知，$Y_1,Y_2$ 与 $X_1$ 独立，则

$$X_1+X_2+X_3=X_1+Y_1\sim N(0,3\sigma^2),$$

故 $\dfrac{1}{\sqrt{3}\sigma}(X_1+X_2+X_3)\sim N(0,1)$．

又 $\left(\dfrac{X_2-X_3}{\sqrt{2}\sigma}\right)^2\sim\chi^2(1)$，且 $X_1+X_2+X_3$ 与 $X_2-X_3$ 相互独立，故由 $t$ 分布的定义，知

$$\sqrt{\frac{2}{3}}\frac{X_1+X_2+X_3}{|X_2-X_3|}\sim t(1).$$

+++

#### 综合解答 (3) 设 $(X_1,X_2,\cdots,X_n,X_{n+1})$ 为总体 $X\sim N(\mu,\sigma^2)$ 的简单随机样本，记 $\bar{X}=\dfrac{1}{n}\sum_{i=1}^{n}X_i$，$S^2=\dfrac{1}{n-1}\sum_{i=1}^{n}(X_i-\bar{X})^2$，$Y=\dfrac{n}{(n+1)\sigma^2}\cdot(X_{n+1}-\bar{X})^2$，$T=\dfrac{k(X_{n+1}-\bar{X})^2}{S^2}$．

（Ⅰ）求 $EY$ 和 $DY$；\
（Ⅱ）若 $T$ 服从 $F$ 分布，求 $k$ 的值．
***
（Ⅰ）先确定 $Y$ 服从的分布．依题设，

$$X_{n+1}\sim N(\mu,\sigma^2),\quad \bar{X}\sim N\left(\mu,\frac{\sigma^2}{n}\right),$$

且 $X_{n+1}$ 与 $\bar{X}$ 相互独立，故 $X_{n+1}-\bar{X}\sim N\left(0,\dfrac{n+1}{n}\sigma^2\right)$，所以

$$\left(\frac{X_{n+1}-\bar{X}}{\sqrt{\dfrac{n+1}{n}}\sigma}\right)^2=\frac{n}{(n+1)\sigma^2}(X_{n+1}-\bar{X})^2=Y\sim\chi^2(1).$$

由 $\chi^2$ 分布的性质，$EY=1$，$DY=2$．

（Ⅱ）由已知，样本方差 $S^2$ 与 $\bar{X}$ 独立，$X_{n+1}$ 与 $S^2$ 独立，且 $\bar{X},X_{n+1},S^2$ 相互独立，故 $S^2$ 与 $(X_{n+1}-\bar{X})^2$ 也独立，所以

$$\frac{\dfrac{n}{(n+1)\sigma^2}(X_{n+1}-\bar{X})^2}{\dfrac{(n-1)S^2}{\sigma^2}\Big/(n-1)}=\frac{n}{n+1}\cdot\frac{(X_{n+1}-\bar{X})^2}{S^2}\sim F(1,n-1),$$

即 $k=\dfrac{n}{n+1}$．
