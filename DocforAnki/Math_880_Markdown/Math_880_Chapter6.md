---
quizify:
  format: 1
  deck: Math_880::Chapter_6
  tags: [Math, 880题, 数一, 第六章, 重积分]
---

+++

#### 基础选择 (1) 设 $D$ 为由直线 $x+y=\frac{1}{2}$，$x+y=1$ 与两坐标轴所围的区域，

$$I_1=\iint_D[\ln(x+y)]^9\,\mathrm{d}x\mathrm{d}y,\quad I_2=\iint_D(x+y)^9\,\mathrm{d}x\mathrm{d}y,\quad I_3=\iint_D[\sin(x+y)]^9\,\mathrm{d}x\mathrm{d}y,$$

则（　）。

;;;
A. $I_1\leqslant I_2\leqslant I_3$
B. $I_1\leqslant I_3\leqslant I_2$
C. $I_3\leqslant I_2\leqslant I_1$
D. $I_3\leqslant I_1\leqslant I_2$
;;;B
***
在 $D$ 上（此时 $\frac{1}{2}\leqslant x+y\leqslant 1$）有

$$[\ln(x+y)]^9\leqslant[\sin(x+y)]^9\leqslant(x+y)^9,$$

故 **B 正确**。

+++

#### 基础选择 (2) 设 $D$ 为由 $y=x^2-4$ 和 $y=0$ 所围区域，$I=\iint_D(kx+y)\,\mathrm{d}x\mathrm{d}y$，则（　）。

;;;
A. $I=0$
B. $I>0$
C. $I<0$
D. $I$ 的正负与 $k$ 有关
;;;C
***
$D$ 关于 $y$ 轴对称，$kx$ 关于 $x$ 为奇函数，故 $\iint_D kx\,\mathrm{d}x\mathrm{d}y=0$。

又在 $D$ 内 $y<0$，故 $I<0$。

+++

#### 基础选择 (3) 设 $D$ 是 $xOy$ 平面上以 $A(1,1)$，$B(-1,1)$，$C(-1,-1)$ 为顶点的三角形区域，$D_1$ 是 $D$ 在第一象限的部分，则 $I=\iint_D(xy+\cos x\sin y)\,\mathrm{d}x\mathrm{d}y=$（　）。

;;;
A. $0$
B. $2\iint_{D_1}xy\,\mathrm{d}x\mathrm{d}y$
C. $2\iint_{D_1}\cos x\sin y\,\mathrm{d}x\mathrm{d}y$
D. $4\iint_{D_1}(xy+\cos x\sin y)\,\mathrm{d}x\mathrm{d}y$
;;;C
***
把 $D$ 分为四块 $D_1,D_2,D_3,D_4$（$D_1,D_2$ 在 $x$ 轴上方，$D_3,D_4$ 在 $x$ 轴下方），则

$$I=\iint_D(xy+\cos x\sin y)\,\mathrm{d}x\mathrm{d}y=\iint_D xy\,\mathrm{d}x\mathrm{d}y+\iint_D\cos x\sin y\,\mathrm{d}x\mathrm{d}y=I_1+I_2.$$

对于 $I_1$：$D_1\cup D_2$ 关于 $y$ 轴对称，$xy$ 关于 $x$ 为奇函数，故 $\iint_{D_1\cup D_2}xy\,\mathrm{d}x\mathrm{d}y=0$；同理 $\iint_{D_3\cup D_4}xy\,\mathrm{d}x\mathrm{d}y=0$，于是 $I_1=0$。

对于 $I_2$：$D_3\cup D_4$ 关于 $x$ 轴对称，$\cos x\sin y$ 关于 $y$ 是奇函数，故 $\iint_{D_3\cup D_4}\cos x\sin y\,\mathrm{d}x\mathrm{d}y=0$；$D_1\cup D_2$ 关于 $y$ 轴对称，$\cos x\sin y$ 关于 $x$ 是偶函数，故

$$\iint_{D_1\cup D_2}\cos x\sin y\,\mathrm{d}x\mathrm{d}y=2\iint_{D_1}\cos x\sin y\,\mathrm{d}x\mathrm{d}y,$$

故 **C 正确**。

+++

#### 基础选择 (4) 积分 $I=\int_0^2\mathrm{d}x\int_0^{\frac{x^2}{2}}f(x,y)\,\mathrm{d}y+\int_2^{2\sqrt{2}}\mathrm{d}x\int_0^{\sqrt{8-x^2}}f(x,y)\,\mathrm{d}y=$（　）。

;;;
A. $\int_0^{\sqrt{2}}\mathrm{d}y\int_{\sqrt{y}}^{\sqrt{8-y^2}}f(x,y)\,\mathrm{d}x$
B. $\int_0^{\sqrt{2}}\mathrm{d}y\int_{\sqrt{2y}}^{\sqrt{8-y^2}}f(x,y)\,\mathrm{d}x$
C. $\int_0^{2}\mathrm{d}y\int_{\sqrt{2y}}^{\sqrt{8-y^2}}f(x,y)\,\mathrm{d}x$
D. $\int_0^{2}\mathrm{d}y\int_{\sqrt{y}}^{\sqrt{8-y^2}}f(x,y)\,\mathrm{d}x$
;;;C
***
原积分的两块积分区域为

$$D_1=\begin{cases}0\leqslant x\leqslant 2,\\ 0\leqslant y\leqslant \dfrac{x^2}{2},\end{cases}\qquad D_2=\begin{cases}2\leqslant x\leqslant 2\sqrt{2},\\ 0\leqslant y\leqslant \sqrt{8-x^2},\end{cases}$$

合并后 $D$ 的左边界为 $x=\sqrt{2y}$，右边界为 $x=\sqrt{8-y^2}$，$0\leqslant y\leqslant 2$，故

$$I=\int_0^2\mathrm{d}y\int_{\sqrt{2y}}^{\sqrt{8-y^2}}f(x,y)\,\mathrm{d}x.$$

**C 正确。**

+++

#### 基础选择 (5) 设 $D:x^2+y^2\leqslant x$，则 $\iint_D f(x,y)\,\mathrm{d}x\mathrm{d}y=$（　）。

;;;
A. $\int_0^{\pi}\mathrm{d}\theta\int_0^{\cos\theta}f(r\cos\theta,r\sin\theta)r\,\mathrm{d}r$
B. $\int_0^{\pi}\mathrm{d}\theta\int_0^{\sin\theta}f(r\cos\theta,r\sin\theta)r\,\mathrm{d}r$
C. $\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{\cos\theta}f(r\cos\theta,r\sin\theta)r\,\mathrm{d}r$
D. $\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{\sin\theta}f(r\cos\theta,r\sin\theta)r\,\mathrm{d}r$
;;;C
***
$x^2+y^2\leqslant x$ 化为极坐标方程为

$$0\leqslant r\leqslant\cos\theta,\quad -\frac{\pi}{2}\leqslant\theta\leqslant\frac{\pi}{2},$$

故 **C 正确**。

+++

#### 基础选择 (6) 将二重积分 $I=\int_{\frac{\pi}{4}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{2\sin\theta}f(r\cos\theta,r\sin\theta)r\,\mathrm{d}r$ 化为直角坐标系下的二次积分，则 $I=$（　）。

;;;
A. $\int_0^1\mathrm{d}x\int_{1-\sqrt{1-x^2}}^{x}f(x,y)\,\mathrm{d}y$
B. $\int_0^1\mathrm{d}x\int_{x}^{\sqrt{1-x^2}}f(x,y)\,\mathrm{d}y$
C. $\int_0^1\mathrm{d}y\int_0^{y}f(x,y)\,\mathrm{d}x+\int_1^2\mathrm{d}y\int_0^{\sqrt{2y-y^2}}f(x,y)\,\mathrm{d}x$
D. $\int_0^1\mathrm{d}y\int_{y}^{\sqrt{2y-y^2}}f(x,y)\,\mathrm{d}x$
;;;C
***
由 $r=2\sin\theta$ 得 $r^2=2r\sin\theta$，即

$$x^2+y^2=2y,$$

即 $x^2+(y-1)^2=1$。结合 $\frac{\pi}{4}\leqslant\theta\leqslant\frac{\pi}{2}$，积分区域 $D$ 是该圆位于 $y=x$ 上方、$x\geqslant0$ 的部分，所以 **C 正确**。

+++

#### 基础选择 (7) 设 $V:x^2+y^2+z^2\leqslant R^2$，$z\geqslant0$，$V_1$ 是 $V$ 位于第一卦限的部分，则（　）。

;;;
A. $\iiint_V z\,\mathrm{d}V=4\iiint_{V_1}z\,\mathrm{d}V$
B. $\iiint_V x\,\mathrm{d}V=4\iiint_{V_1}x\,\mathrm{d}V$
C. $\iiint_V y\,\mathrm{d}V=4\iiint_{V_1}y\,\mathrm{d}V$
D. $\iiint_V xyz\,\mathrm{d}V=4\iiint_{V_1}xyz\,\mathrm{d}V$
;;;A
***
积分区域 $V$ 关于 $yOz$ 面和 $xOz$ 面对称，而 $z=zx^0y^0$ 关于 $x$ 与 $y$ 均为**偶函数**，故 **A 正确**。

+++

#### 基础填空 (1) 二重积分 $I=\int_0^1 x^2\,\mathrm{d}x\int_x^1\mathrm{e}^{-y^2}\,\mathrm{d}y=$ ________.
***
$$I=\frac{1}{6}-\frac{1}{3\mathrm{e}}.$$

**解** 由于 $\mathrm{e}^{-y^2}$ 的原函数不能用初等函数表达，故交换积分顺序才能计算：

$$I=\int_0^1 x^2\,\mathrm{d}x\int_x^1\mathrm{e}^{-y^2}\,\mathrm{d}y=\int_0^1\mathrm{e}^{-y^2}\,\mathrm{d}y\int_0^y x^2\,\mathrm{d}x=\frac{1}{3}\int_0^1\mathrm{e}^{-y^2}y^3\,\mathrm{d}y\xrightarrow{\text{分部积分}}\frac{1}{6}-\frac{1}{3\mathrm{e}}.$$

+++

#### 基础填空 (2) 二重积分 $I=\int_1^2\mathrm{d}x\int_{\sqrt{x}}^{x}\sin\frac{\pi x}{2y}\,\mathrm{d}y+\int_2^4\mathrm{d}x\int_{\sqrt{x}}^{2}\sin\frac{\pi x}{2y}\,\mathrm{d}y=$ ________.
***
$$I=\frac{4}{\pi^3}(2+\pi).$$

**解** 作出积分区域 $D$ 并交换积分顺序，得

$$I=\int_1^2\mathrm{d}y\int_{y}^{y^2}\sin\frac{\pi x}{2y}\,\mathrm{d}x=\int_1^2\frac{2y}{\pi}\left(\cos\frac{\pi}{2}-\cos\frac{\pi}{2}y\right)\mathrm{d}y=-\frac{2}{\pi}\int_1^2 y\cos\frac{\pi}{2}y\,\mathrm{d}y\xrightarrow{\text{分部积分}}\frac{4}{\pi^3}(2+\pi).$$

+++

#### 基础填空 (3) 二重积分 $I=\int_0^1\mathrm{d}x\int_x^1\sin y^2\,\mathrm{d}y=$ ________.
***
$$I=\frac{1-\cos 1}{2}.$$

**解** 交换积分顺序，得

$$I=\int_0^1\mathrm{d}y\int_0^y\sin y^2\,\mathrm{d}x=\int_0^1 y\sin y^2\,\mathrm{d}y=\frac{1}{2}\int_0^1\sin y^2\,\mathrm{d}(y^2)=\left.\frac{1}{2}(-\cos y^2)\right|_0^1=\frac{1-\cos 1}{2}.$$

+++

#### 基础填空 (4) 设 $D:x^2+y^2\leqslant4$，$x\geqslant0$，$y\geqslant0$，$f(x)$ 在 $[0,+\infty)$ 上连续且取正值，则 $I=\iint_D\dfrac{a\sqrt{f(x)}+b\sqrt{f(y)}}{\sqrt{f(x)}+\sqrt{f(y)}}\,\mathrm{d}x\mathrm{d}y=$ ________.
***
$$I=\frac{a+b}{2}\pi.$$

**解** $D$ 关于直线 $y=x$ 对称，故

$$I=\frac{1}{2}\iint_D\left[\frac{a\sqrt{f(x)}+b\sqrt{f(y)}}{\sqrt{f(x)}+\sqrt{f(y)}}+\frac{a\sqrt{f(y)}+b\sqrt{f(x)}}{\sqrt{f(y)}+\sqrt{f(x)}}\right]\mathrm{d}x\mathrm{d}y=\frac{a+b}{2}\iint_D\mathrm{d}x\mathrm{d}y=\frac{a+b}{2}\cdot\frac{1}{4}\pi\cdot2^2=\frac{a+b}{2}\pi.$$

+++

#### 基础填空 (5) 设 $f(x)$ 在 $[0,1]$ 上连续，且 $\int_0^1 f(x)\,\mathrm{d}x=A$，则 $I=\int_0^1\mathrm{d}x\int_x^1 f(x)f(y)\,\mathrm{d}y=$ ________.
***
$$I=\frac{A^2}{2}.$$

**解** 令 $F(x)=\int_x^1 f(y)\,\mathrm{d}y$，则 $F'(x)=-f(x)$，故

$$I=\int_0^1\mathrm{d}x\int_x^1 f(x)f(y)\,\mathrm{d}y=\int_0^1 f(x)\,\mathrm{d}x\int_x^1 f(y)\,\mathrm{d}y=-\int_0^1 F(x)\,\mathrm{d}[F(x)]=\left.-\frac{1}{2}F^2(x)\right|_0^1=\frac{A^2}{2}.$$

**【注】** 也可利用交换积分顺序及积分与积分变量无关求解：

$$\int_0^1\mathrm{d}x\int_x^1 f(x)f(y)\,\mathrm{d}y=\int_0^1\mathrm{d}y\int_0^y f(x)f(y)\,\mathrm{d}x=\int_0^1\mathrm{d}x\int_0^x f(x)f(y)\,\mathrm{d}y,$$

故 $2\int_0^1\mathrm{d}x\int_x^1 f(x)f(y)\,\mathrm{d}y=\int_0^1\mathrm{d}x\int_0^1 f(x)f(y)\,\mathrm{d}y=\left[\int_0^1 f(x)\,\mathrm{d}x\right]\left[\int_0^1 f(y)\,\mathrm{d}y\right]=A^2$，故 $I=\dfrac{A^2}{2}$。

+++

#### 基础填空 (6) 设 $D:x^2+y^2\leqslant1$，$x\geqslant0$，$y\geqslant0$，则 $I=\iint_D\dfrac{1+x-y}{1+x^2+y^2}\,\mathrm{d}x\mathrm{d}y=$ ________.
***
$$I=\frac{\pi}{4}\ln 2.$$

**解** 由于 $D$ 关于直线 $y=x$ 对称，所以

$$I=\frac{1}{2}\iint_D\left(\frac{1+x-y}{1+x^2+y^2}+\frac{1+y-x}{1+y^2+x^2}\right)\mathrm{d}x\mathrm{d}y=\frac{1}{2}\iint_D\frac{2}{1+x^2+y^2}\,\mathrm{d}x\mathrm{d}y$$

$$=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^1\frac{r}{1+r^2}\,\mathrm{d}r=\frac{\pi}{2}\cdot\frac{1}{2}\int_0^1\frac{\mathrm{d}(1+r^2)}{1+r^2}=\left.\frac{\pi}{4}\ln(1+r^2)\right|_0^1=\frac{\pi}{4}\ln 2.$$

+++

#### 基础填空 (7) 设 $D:-1\leqslant x\leqslant0$，$1-\sqrt{1-x^2}\leqslant y\leqslant-x$，则 $I=\iint_D\dfrac{\mathrm{d}x\mathrm{d}y}{\sqrt{x^2+y^2}\,\sqrt{4-x^2-y^2}}=$ ________.
***
$$I=\frac{\pi^2}{32}.$$

**解** 用极坐标有

$$\frac{3\pi}{4}\leqslant\theta\leqslant\pi,\quad 0\leqslant r\leqslant 2\sin\theta,$$

故

$$I=\int_{\frac{3\pi}{4}}^{\pi}\mathrm{d}\theta\int_0^{2\sin\theta}\frac{r}{r\sqrt{4-r^2}}\,\mathrm{d}r=\int_{\frac{3\pi}{4}}^{\pi}\left.\arcsin\frac{r}{2}\right|_0^{2\sin\theta}\mathrm{d}\theta=\int_{\frac{3\pi}{4}}^{\pi}(\pi-\theta)\,\mathrm{d}\theta=\frac{\pi^2}{32}.$$

+++

#### 基础填空 (8) 设 $D:2x\leqslant x^2+y^2$，$0\leqslant y\leqslant x\leqslant2$，则 $I=\iint_D\dfrac{\mathrm{d}x\mathrm{d}y}{\sqrt{x^2+y^2}}=$ ________.
***
$$I=2\ln(1+\sqrt{2})-\sqrt{2}.$$

**解** 采用极坐标：$x^2+y^2=2x$ 的极坐标方程为 $r=2\cos\theta$，$x=2$ 的极坐标方程为 $r=2\sec\theta$，$y=x$ 的极坐标方程为 $\theta=\dfrac{\pi}{4}$，故

$$I=\iint_D\frac{\mathrm{d}x\mathrm{d}y}{\sqrt{x^2+y^2}}=\int_0^{\frac{\pi}{4}}\mathrm{d}\theta\int_{2\cos\theta}^{2\sec\theta}\frac{1}{r}\cdot r\,\mathrm{d}r=2\int_0^{\frac{\pi}{4}}(\sec\theta-\cos\theta)\,\mathrm{d}\theta$$

$$=\left.2(\ln|\sec\theta+\tan\theta|-\sin\theta)\right|_0^{\frac{\pi}{4}}=2\ln(1+\sqrt{2})-\sqrt{2}.$$

+++

#### 基础填空 (9) 设 $D:x^2+y^2\leqslant1$，则 $I=\iint_D\left(\dfrac{x^2}{4}+\dfrac{y^2}{9}\right)\mathrm{d}x\mathrm{d}y=$ ________.
***
$$I=\frac{13\pi}{144}.$$

**解** $D$ 关于直线 $y=x$ 对称，由轮换对称性，有

$$I=\iint_D\left(\frac{x^2}{4}+\frac{y^2}{9}\right)\mathrm{d}x\mathrm{d}y=\frac{1}{2}\iint_D\left(\frac{x^2}{4}+\frac{y^2}{9}+\frac{y^2}{4}+\frac{x^2}{9}\right)\mathrm{d}x\mathrm{d}y$$

$$=\frac{1}{2}\left(\frac{1}{4}+\frac{1}{9}\right)\iint_D(x^2+y^2)\,\mathrm{d}x\mathrm{d}y=\frac{1}{2}\left(\frac{1}{4}+\frac{1}{9}\right)\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r^3\,\mathrm{d}r=\frac{13\pi}{144}.$$

+++

#### 基础填空 (10) 设区域 $D$ 由 $x=-\sqrt{2y-y^2}$，$x=-2$，$y=0$，$y=2$ 所围，则 $I=\iint_D y\,\mathrm{d}x\mathrm{d}y=$ ________.
***
$$I=4-\frac{\pi}{2}.$$

**解** 设

$$D_{\text{大}}=\{(x,y)\mid -2\leqslant x\leqslant0,\ 0\leqslant y\leqslant2\},\qquad D_{\text{小}}=\{(x,y)\mid -\sqrt{2y-y^2}\leqslant x\leqslant0\},$$

则

$$I=\iint_D y\,\mathrm{d}x\mathrm{d}y=\iint_{D_{\text{大}}}y\,\mathrm{d}x\mathrm{d}y-\iint_{D_{\text{小}}}y\,\mathrm{d}x\mathrm{d}y=\int_{-2}^0\mathrm{d}x\int_0^2 y\,\mathrm{d}y-\int_{\frac{\pi}{2}}^{\pi}\mathrm{d}\theta\int_0^{2\sin\theta}r^2\sin\theta\,\mathrm{d}r$$

$$=4-\frac{8}{3}\int_{\frac{\pi}{2}}^{\pi}\sin^4\theta\,\mathrm{d}\theta=4-\frac{8}{3}\int_0^{\frac{\pi}{2}}\cos^4 t\,\mathrm{d}t=4-\frac{8}{3}\times\frac{3}{4}\times\frac{1}{2}\times\frac{\pi}{2}=4-\frac{\pi}{2}.$$

**【注】** 由于 $D$ 关于 $y=1$ 对称，故

$$I=\iint_D y\,\mathrm{d}x\mathrm{d}y=\iint_D[(y-1)+1]\,\mathrm{d}x\mathrm{d}y=\iint_D(y-1)\,\mathrm{d}x\mathrm{d}y+\iint_D\mathrm{d}x\mathrm{d}y=0+2^2-\frac{1}{2}\pi\times1^2=4-\frac{\pi}{2},$$

或利用形心纵坐标 $\bar{y}=1$，有 $I=\iint_D y\,\mathrm{d}x\mathrm{d}y=\bar{y}\cdot\left(4-\dfrac{\pi}{2}\right)=4-\dfrac{\pi}{2}$。

+++

#### 基础填空 (11) 设 $D:x^2+y^2\leqslant2x$，则 $I=\iint_D(2x+3y)\,\mathrm{d}x\mathrm{d}y=$ ________.
***
$$I=2\pi.$$

**解** 利用极坐标，

$$I=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{2\cos\theta}(2r\cos\theta+3r\sin\theta)r\,\mathrm{d}r=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\left(\frac{16}{3}\cos^4\theta+8\cos^3\theta\sin\theta\right)\mathrm{d}\theta$$

$$=\frac{32}{3}\int_0^{\frac{\pi}{2}}\cos^4\theta\,\mathrm{d}\theta+0=\frac{32}{3}\times\frac{3}{4}\times\frac{1}{2}\times\frac{\pi}{2}=2\pi.$$

**【注】** ① 被积函数关于 $x,y$ 都是一次函数，可利用形心坐标 $(\bar{x},\bar{y})=(1,0)$：由 $\iint_D x\,\mathrm{d}x\mathrm{d}y=\bar{x}\cdot\iint_D\mathrm{d}x\mathrm{d}y$，$\iint_D y\,\mathrm{d}x\mathrm{d}y=\bar{y}\cdot\iint_D\mathrm{d}x\mathrm{d}y$，所以 $I=(2\bar{x}+3\bar{y})\pi\cdot1^2=2\pi$。

② $D$ 关于直线 $x=1$ 对称，$2(x-1)$ 为奇函数，故 $\iint_D 2(x-1)\,\mathrm{d}x\mathrm{d}y=0$，于是 $I=2\iint_D\mathrm{d}x\mathrm{d}y+3\iint_D y\,\mathrm{d}x\mathrm{d}y$；又 $D$ 关于 $x$ 轴对称，$\iint_D y\,\mathrm{d}x\mathrm{d}y=0$，故 $I=2\times\pi\times1^2=2\pi$。

+++

#### 基础填空 (12) 设 $V:x^2+y^2+z^2\leqslant2y-2x$，则 $I=\iiint_V(x+y+z)\,\mathrm{d}V=$ ________.
***
$$I=0.$$

**解** $V$ 是以 $(-1,1,0)$ 为球心、$\sqrt{2}$ 为半径的球体，若视其密度为常数，则质心（形心）坐标为 $(-1,1,0)$，而

$$\bar{x}=\frac{\iiint_V x\,\mathrm{d}V}{\iiint_V\mathrm{d}V},\quad \bar{y}=\frac{\iiint_V y\,\mathrm{d}V}{\iiint_V\mathrm{d}V},\quad \bar{z}=\frac{\iiint_V z\,\mathrm{d}V}{\iiint_V\mathrm{d}V}.$$

而 $\iiint_V\mathrm{d}V$ 为球的体积 $\dfrac{8}{3}\sqrt{2}\pi$，故

$$\iiint_V x\,\mathrm{d}V=\frac{8}{3}\sqrt{2}\pi\times(-1)=-\frac{8}{3}\sqrt{2}\pi,\quad \iiint_V y\,\mathrm{d}V=\frac{8}{3}\sqrt{2}\pi\times1=\frac{8}{3}\sqrt{2}\pi,\quad \iiint_V z\,\mathrm{d}V=0,$$

于是 $I=\iiint_V(x+y+z)\,\mathrm{d}V=0$。

+++

#### 基础填空 (13) 球体 $x^2+y^2+z^2=R^2\ (R>0)$ 被圆柱面 $x^2+y^2=Rx$ 所截得的含在圆柱面内的立体的体积为 ________.
***
$$V=\frac{4}{3}\left(\frac{\pi}{2}-\frac{2}{3}\right)R^3.$$

**解** 由对称性，取 $xOy$ 坐标面上方部分并乘以 $2$、圆柱面区域上下对称再乘 $2$，得

$$V=4\iint_D\sqrt{R^2-x^2-y^2}\,\mathrm{d}x\mathrm{d}y=4\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{R\cos\theta}\sqrt{R^2-r^2}\cdot r\,\mathrm{d}r$$

$$=\frac{4}{3}R^3\int_0^{\frac{\pi}{2}}(1-\sin^3\theta)\,\mathrm{d}\theta=\frac{4}{3}\left(\frac{\pi}{2}-\frac{2}{3}\right)R^3.$$

+++

#### 基础填空 (14) $r\leqslant1$ 与 $r\leqslant1+\cos\theta$ 所围平面区域的形心坐标为 ________.
***
$$\left(\frac{15\pi-32}{30\pi-48},\ 0\right).$$

**解** 由对称性知 $\bar{y}=0$。又由于

$$\bar{x}=\frac{\iint_D x\,\mathrm{d}x\mathrm{d}y}{\iint_D\mathrm{d}x\mathrm{d}y}=\frac{2\displaystyle\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^1 r\cos\theta\cdot r\,\mathrm{d}r+2\displaystyle\int_{\frac{\pi}{2}}^{\pi}\mathrm{d}\theta\int_0^{1+\cos\theta}r\cos\theta\cdot r\,\mathrm{d}r}{\dfrac{1}{2}\pi\times1^2+2\displaystyle\int_{\frac{\pi}{2}}^{\pi}\mathrm{d}\theta\int_0^{1+\cos\theta}r\,\mathrm{d}r}$$

$$=\frac{\dfrac{2}{3}\left(\dfrac{15\pi}{16}-2\right)}{\dfrac{5}{4}\pi-2}=\frac{15\pi-32}{30\pi-48},$$

故形心坐标为 $\left(\dfrac{15\pi-32}{30\pi-48},0\right)$。

+++

#### 基础填空 (15) 设平面薄片（密度 $\rho=1$）由 $y^2=x^3$ 与直线 $y=x$ 所围，则 $D$ 对 $x$ 轴和 $y$ 轴的转动惯量分别为 $I_x=$ ________，$I_y=$ ________.
***
$$I_x=\frac{1}{44},\qquad I_y=\frac{1}{36}.$$

**解** 对 $x$ 轴与 $y$ 轴的转动惯量分别为 $I_x=\iint_D y^2\,\mathrm{d}x\mathrm{d}y$ 与 $I_y=\iint_D x^2\,\mathrm{d}x\mathrm{d}y$，故

$$I_x=\iint_D y^2\,\mathrm{d}x\mathrm{d}y=\int_0^1\mathrm{d}x\int_{x^{\frac{3}{2}}}^{x}y^2\,\mathrm{d}y=\int_0^1\left.\frac{1}{3}y^3\right|_{x^{\frac{3}{2}}}^{x}\mathrm{d}x=\frac{1}{44},$$

$$I_y=\iint_D x^2\,\mathrm{d}x\mathrm{d}y=\int_0^1\mathrm{d}x\int_{x^{\frac{3}{2}}}^{x}x^2\,\mathrm{d}y=\frac{1}{36}.$$

**【注】** 质点（质量为 $m$）对轴 $l$ 的转动惯量为 $I_l=m\cdot r_l^2$，其中 $r_l$ 表示质点到轴 $l$ 的距离。平面区域 $D$ 对 $x$ 轴的转动惯量可采用微元法：任取一个小区域 $\mathrm{d}\sigma$，看成质量集中为一点 $(x,y)$，则微元 $\mathrm{d}I_x=\rho\cdot y^2\mathrm{d}\sigma$（$\rho$ 表示 $D$ 的面密度），故 $I_x=\iint_D y^2\cdot\rho\,\mathrm{d}\sigma$。

+++

#### 基础解答 (1) 计算下列二重积分：

（Ⅰ）设 $D$ 由 $x-y=0$，$x+y=0$ 及 $x=1$ 所围，求 $I=\iint_D xy(x-y)\,\mathrm{d}x\mathrm{d}y$；\
（Ⅱ）设 $D$ 由 $y=\sqrt{x}$，$y=x$ 所围，求 $I=\iint_D\dfrac{\sin y}{y}\,\mathrm{d}x\mathrm{d}y$；\
（Ⅲ）设 $D$ 由 $y=x^2\ (x\geqslant0)$，$y=1$，$x=0$ 所围，求 $I=\iint_D\dfrac{xy}{\sqrt{1+y^3}}\,\mathrm{d}x\mathrm{d}y$；\
（Ⅳ）设 $D:-1\leqslant x\leqslant\sin y$，$|y|\leqslant\dfrac{\pi}{2}$，求 $I=\iint_D x(\mathrm{e}^{x^2+\cos y}\sin y-1)\,\mathrm{d}x\mathrm{d}y$.
***
**（Ⅰ）** 先对 $y$ 积分较简便：

$$I=\iint_D xy(x-y)\,\mathrm{d}x\mathrm{d}y=\int_0^1\mathrm{d}x\int_{-x}^{x}xy(x-y)\,\mathrm{d}y=\int_0^1\left.\left(\frac{x^2y^2}{2}-\frac{xy^3}{3}\right)\right|_{-x}^{x}\mathrm{d}x=-\frac{2}{3}\int_0^1 x^4\,\mathrm{d}x=-\frac{2}{15}.$$

**（Ⅱ）** 若先对 $y$ 积分，则 $\int\dfrac{\sin y}{y}\mathrm{d}y$ 不能表示为初等函数，故只能先对 $x$ 积分：

$$I=\iint_D\frac{\sin y}{y}\,\mathrm{d}x\mathrm{d}y=\int_0^1\mathrm{d}y\int_{y^2}^{y}\frac{\sin y}{y}\,\mathrm{d}x=\int_0^1\frac{\sin y}{y}(y-y^2)\,\mathrm{d}y=\int_0^1(1-y)\sin y\,\mathrm{d}y$$

$$=\left.[-(1-y)\cos y-\sin y]\right|_0^1=1-\sin 1.$$

**（Ⅲ）** 先对 $x$ 积分，则

$$I=\iint_D\frac{xy}{\sqrt{1+y^3}}\,\mathrm{d}x\mathrm{d}y=\int_0^1\frac{y}{\sqrt{1+y^3}}\,\mathrm{d}y\int_0^{\sqrt{y}}x\,\mathrm{d}x=\frac{1}{2}\int_0^1\frac{y^2}{\sqrt{1+y^3}}\,\mathrm{d}y=\left.\frac{1}{2}\cdot\frac{2}{3}(1+y^3)^{\frac{1}{2}}\right|_0^1=\frac{1}{3}(\sqrt{2}-1).$$

**（Ⅳ）** 作辅助线 $y=-\arcsin x\ (-1\leqslant x\leqslant0)$，将 $D$ 划分为 $D_1$ 与 $D_2$，则

$$I=\iint_D x(\mathrm{e}^{x^2+\cos y}\sin y-1)\,\mathrm{d}x\mathrm{d}y=\iint_D x\mathrm{e}^{x^2+\cos y}\sin y\,\mathrm{d}x\mathrm{d}y-\iint_D x\,\mathrm{d}x\mathrm{d}y\xlongequal{\text{记}}I_1-I_2.$$

由 $D_1$ 关于 $y$ 轴对称，$x\mathrm{e}^{x^2+\cos y}\sin y$ 关于 $x$ 是奇函数，故 $\iint_{D_1}x\mathrm{e}^{x^2+\cos y}\sin y\,\mathrm{d}x\mathrm{d}y=0$；同理 $\iint_{D_2}x\mathrm{e}^{x^2+\cos y}\sin y\,\mathrm{d}x\mathrm{d}y=0$，故 $I_1=0$。

对 $I_2$：根据对称性 $\iint_{D_1}x\,\mathrm{d}x\mathrm{d}y=0$，又

$$\iint_{D_2}x\,\mathrm{d}x\mathrm{d}y=2\int_0^{\frac{\pi}{2}}\mathrm{d}y\int_{-1}^{-\sin y}x\,\mathrm{d}x=-\frac{\pi}{4},$$

故 $I=0-\left(-\dfrac{\pi}{4}\right)=\dfrac{\pi}{4}$。

+++

#### 基础解答 (2) 设 $D=\{(x,y)\mid x^2+y^2\leqslant1,\ x^2+y^2\leqslant2x,\ y\geqslant0\}$，计算 $I=\iint_D xy\,\mathrm{d}x\mathrm{d}y$.
***
由 $\begin{cases}x^2+y^2=1,\\ x^2+y^2=2x,\end{cases}$ 解得交点 $A\left(\dfrac{1}{2},\dfrac{\sqrt{3}}{2}\right)$，故

$$I=\iint_D xy\,\mathrm{d}x\mathrm{d}y=\int_0^{\frac{\sqrt{3}}{2}}\mathrm{d}y\int_{1-\sqrt{1-y^2}}^{\sqrt{1-y^2}}xy\,\mathrm{d}x=\frac{1}{2}\int_0^{\frac{\sqrt{3}}{2}}\left.yx^2\right|_{1-\sqrt{1-y^2}}^{\sqrt{1-y^2}}\mathrm{d}y$$

$$=\frac{1}{2}\int_0^{\frac{\sqrt{3}}{2}}y\left[1-y^2-\left(1-\sqrt{1-y^2}\right)^2\right]\mathrm{d}y=\int_0^{\frac{\sqrt{3}}{2}}\left(y\sqrt{1-y^2}-\frac{1}{2}y\right)\mathrm{d}y$$

$$=\left.\left[-\frac{1}{3}(1-y^2)^{\frac{3}{2}}-\frac{1}{4}y^2\right]\right|_0^{\frac{\sqrt{3}}{2}}=\frac{5}{48}.$$

+++

#### 基础解答 (3) 设 $D:x^2+y^2\leqslant\sqrt{2}x$，$0\leqslant y\leqslant x$，计算 $I=\iint_D\left|\sqrt{x^2+y^2}-1\right|\mathrm{d}x\mathrm{d}y$.
***
用 $x^2+y^2=1$，即 $r=1$ 将 $D$ 划分为 $D_1$ 与 $D_2$（$D_1$ 为 $r\leqslant1$ 的部分），则

$$I=\iint_{D_1}(1-r)r\,\mathrm{d}r\mathrm{d}\theta+\iint_{D_2}(r-1)r\,\mathrm{d}r\mathrm{d}\theta=\iint_{D_1}(1-r)r\,\mathrm{d}r\mathrm{d}\theta-\iint_{D_2}(1-r)r\,\mathrm{d}r\mathrm{d}\theta$$

$$=2\iint_{D_1}(1-r)r\,\mathrm{d}r\mathrm{d}\theta-\iint_{D}(1-r)r\,\mathrm{d}r\mathrm{d}\theta=2\int_0^{\frac{\pi}{4}}\mathrm{d}\theta\int_0^1(1-r)r\,\mathrm{d}r-\int_0^{\frac{\pi}{4}}\mathrm{d}\theta\int_0^{\sqrt{2}\cos\theta}(1-r)r\,\mathrm{d}r$$

$$=\frac{\pi}{12}-\int_0^{\frac{\pi}{4}}\left(\cos^2\theta-\frac{2\sqrt{2}}{3}\cos^3\theta\right)\mathrm{d}\theta=\frac{\pi}{12}+\frac{5}{9}-\frac{1}{4}-\frac{\pi}{8}=\frac{11}{36}-\frac{\pi}{24}.$$

+++

#### 基础解答 (4) 设 $D:x^2+y^2\leqslant9$，计算 $I=\iint_D|x^2+y^2-4|\,\mathrm{d}x\mathrm{d}y$.
***
用 $x^2+y^2=4$ 将 $D$ 划分为 $D_1$（内部圆盘）与 $D_2$，则

$$I=\iint_D|x^2+y^2-4|\,\mathrm{d}x\mathrm{d}y=-\iint_{D_1}(x^2+y^2-4)\,\mathrm{d}x\mathrm{d}y+\iint_{D_2}(x^2+y^2-4)\,\mathrm{d}x\mathrm{d}y$$

$$=\iint_D(x^2+y^2-4)\,\mathrm{d}x\mathrm{d}y-2\iint_{D_1}(x^2+y^2-4)\,\mathrm{d}x\mathrm{d}y$$

$$=\int_0^{2\pi}\mathrm{d}\theta\int_0^3(r^2-4)r\,\mathrm{d}r-2\int_0^{2\pi}\mathrm{d}\theta\int_0^2(r^2-4)r\,\mathrm{d}r$$

$$=\left.2\pi\left(\frac{r^4}{4}-2r^2\right)\right|_0^3-\left.4\pi\left(\frac{r^4}{4}-2r^2\right)\right|_0^2=\frac{9}{2}\pi+16\pi=\frac{41}{2}\pi.$$

+++

#### 基础解答 (5) 设 $D:1\leqslant x^2+y^2\leqslant2x$，$y\geqslant0$，计算 $I=\iint_D\dfrac{y}{(1+x^2+y^2)\sqrt{x^2+y^2}}\,\mathrm{d}x\mathrm{d}y$.
***
由 $\begin{cases}x^2+y^2=1,\\ x^2+y^2=2x,\end{cases}$ 解得交点 $A\left(\dfrac{1}{2},\dfrac{\sqrt{3}}{2}\right)$，故

$$I=\int_0^{\frac{\pi}{3}}\mathrm{d}\theta\int_1^{2\cos\theta}\frac{\sin\theta}{1+r^2}\cdot r\,\mathrm{d}r=\frac{1}{2}\int_0^{\frac{\pi}{3}}\sin\theta\left.\left[\ln(1+r^2)\right]\right|_1^{2\cos\theta}\mathrm{d}\theta$$

$$=\frac{1}{2}\int_0^{\frac{\pi}{3}}\left[\ln(1+4\cos^2\theta)-\ln 2\right]\sin\theta\,\mathrm{d}\theta\xlongequal{u=\cos\theta}\frac{1}{2}\int_{\frac{1}{2}}^1\left[\ln(1+4u^2)-\ln 2\right]\mathrm{d}u$$

$$=\left.\frac{1}{2}\left[u\ln(1+4u^2)-2u+\arctan 2u\right]\right|_{\frac{1}{2}}^1-\frac{1}{4}\ln 2=\frac{1}{2}\left(\ln\frac{5}{2}-1+\arctan 2-\frac{\pi}{4}\right).$$

+++

#### 基础解答 (6) 设 $D:0\leqslant x\leqslant2$，$0\leqslant y\leqslant2$，计算 $I=\iint_D[1+x+y]\,\mathrm{d}x\mathrm{d}y$，其中 $[1+x+y]$ 表示不超过 $1+x+y$ 的最大整数.
***
直线 $x+y=i\ (i=1,2,3,4)$ 将 $D$ 分为 $4$ 个区域 $D_k\ (k=1,2,3,4)$，则

$$[1+x+y]=k\quad(k=1,2,3,4),$$

故

$$I=\iint_D[1+x+y]\,\mathrm{d}x\mathrm{d}y=\iint_{D_1}1\,\mathrm{d}x\mathrm{d}y+\iint_{D_2}2\,\mathrm{d}x\mathrm{d}y+\iint_{D_3}3\,\mathrm{d}x\mathrm{d}y+\iint_{D_4}4\,\mathrm{d}x\mathrm{d}y=10.$$

**【注】** $\iint_D\mathrm{d}x\mathrm{d}y$ 表示 $D$ 的面积。

+++

#### 基础解答 (7) 计算 $I=\iint_D\max\{x,y\}\cdot|y-x^2|\,\mathrm{d}x\mathrm{d}y$，其中 $D:0\leqslant x\leqslant1$，$0\leqslant y\leqslant1$.
***
用直线 $y=x$ 将 $D$ 划分为 $D_1$（$y\geqslant x$）与 $D_2$（$y\leqslant x$），故

$$I=\iint_D\max\{x,y\}\cdot|y-x^2|\,\mathrm{d}x\mathrm{d}y=\iint_{D_1}y(y-x^2)\,\mathrm{d}x\mathrm{d}y+\iint_{D_2}x|y-x^2|\,\mathrm{d}x\mathrm{d}y.$$

又 $D_2$ 被 $y=x^2$ 分为上、下两部分，则

$$I=\int_0^1\mathrm{d}x\int_x^1 y(y-x^2)\,\mathrm{d}y+\int_0^1\mathrm{d}x\int_{x^2}^{x}x(y-x^2)\,\mathrm{d}y+\int_0^1\mathrm{d}x\int_0^{x^2}x(x^2-y)\,\mathrm{d}y=\frac{11}{40}.$$

+++

#### 基础解答 (8) 计算 $I=\iint_D\mathrm{sgn}(x^2-y^2+2)\,\mathrm{d}x\mathrm{d}y$，其中 $D:x^2+y^2\leqslant4$.
***
由符号函数的定义，知

$$\mathrm{sgn}(x^2-y^2+2)=\begin{cases}1,& x^2-y^2+2>0,\\ 0,& x^2-y^2+2=0,\\ -1,& x^2-y^2+2<0,\end{cases}$$

故 $x^2-y^2+2=0$，即双曲线 $\dfrac{y^2}{2}-\dfrac{x^2}{2}=1$ 将 $D$ 划分为三个区域 $D_1,D_2,D_3$（$D_1$ 为上方小块，$D_3$ 为下方小块，$D_2$ 为中间部分），

$$\mathrm{sgn}(x^2-y^2+2)=\begin{cases}1,& (x,y)\in D_2,\\ -1,& (x,y)\in D_1\cup D_3,\end{cases}$$

故

$$I=\iint_{D_2}1\,\mathrm{d}x\mathrm{d}y-\iint_{D_1}1\,\mathrm{d}x\mathrm{d}y-\iint_{D_3}1\,\mathrm{d}x\mathrm{d}y=\iint_{D_2}\mathrm{d}x\mathrm{d}y-2\iint_{D_1}\mathrm{d}x\mathrm{d}y.$$

而 $\iint_{D_2}\mathrm{d}x\mathrm{d}y=\iint_D\mathrm{d}x\mathrm{d}y-\iint_{D_1\cup D_3}\mathrm{d}x\mathrm{d}y=\iint_D\mathrm{d}x\mathrm{d}y-2\iint_{D_1}\mathrm{d}x\mathrm{d}y$，故

$$I=\iint_D\mathrm{d}x\mathrm{d}y-4\iint_{D_1}\mathrm{d}x\mathrm{d}y=\pi\times2^2-4\int_{-1}^1\mathrm{d}x\int_{\sqrt{2+x^2}}^{\sqrt{4-x^2}}\mathrm{d}y$$

$$=4\pi-\left.4\left[\frac{x}{2}\sqrt{4-x^2}+2\arcsin\frac{x}{2}-\frac{x}{2}\sqrt{2+x^2}-\ln(x+\sqrt{2+x^2})\right]\right|_{-1}^1$$

$$=4\pi-4\left[\frac{2\pi}{3}-\ln(2+\sqrt{3})\right]=\frac{4\pi}{3}+4\ln(2+\sqrt{3}).$$

+++

#### 基础解答 (9) 设 $f(x,y)=\begin{cases}\dfrac{1}{(x^2+y^2)^2},&1\leqslant x\leqslant3,\ \dfrac{\sqrt{3}}{3}x\leqslant y\leqslant x,\\ 0,&\text{其他},\end{cases}$ $D$ 由 $x=3$，$x=1$，$y=0$，$y=3$ 所围，计算 $I=\iint_D f(x,y)\,\mathrm{d}x\mathrm{d}y$.
***
将 $D$ 分成 $D=D_1+D_2+D_3$（$D_2$ 为 $\dfrac{\sqrt{3}}{3}x\leqslant y\leqslant x$ 的部分），则

$$I=\iint_D f(x,y)\,\mathrm{d}x\mathrm{d}y=\iint_{D_1}0\,\mathrm{d}x\mathrm{d}y+\iint_{D_2}\frac{\mathrm{d}x\mathrm{d}y}{(x^2+y^2)^2}+\iint_{D_3}0\,\mathrm{d}x\mathrm{d}y$$

$$=\int_{\frac{\pi}{6}}^{\frac{\pi}{4}}\mathrm{d}\theta\int_{\sec\theta}^{3\sec\theta}\frac{r}{r^4}\,\mathrm{d}r=\frac{4}{9}\int_{\frac{\pi}{6}}^{\frac{\pi}{4}}\cos^2\theta\,\mathrm{d}\theta=\frac{2}{9}\int_{\frac{\pi}{6}}^{\frac{\pi}{4}}(1+\cos 2\theta)\,\mathrm{d}\theta$$

$$=\frac{2}{9}\left(\frac{\pi}{12}+\frac{1}{2}-\frac{\sqrt{3}}{4}\right)=\frac{\pi+6-3\sqrt{3}}{54}.$$

+++

#### 基础解答 (10) 计算 $I=\iint_D xy\,\mathrm{d}x\mathrm{d}y$，其中 $D$ 由下列双纽线所围.

（Ⅰ）$(x^2+y^2)^2=2(x^2-y^2)$；\
（Ⅱ）$(x^2+y^2)^2=2xy$.
***
**（Ⅰ）** 双纽线 $(x^2+y^2)^2=2(x^2-y^2)$ 所围区域 $D$ 关于 $x$ 轴对称，$xy$ 关于 $y$ 是奇函数，故

$$I=\iint_D xy\,\mathrm{d}x\mathrm{d}y=0.$$

**（Ⅱ）** 双纽线 $(x^2+y^2)^2=2xy$ 所围区域 $D$ 关于原点对称，而 $xy=(-x)(-y)$，故（$D_1$ 是 $D$ 在第一象限的部分）

$$I=\iint_D xy\,\mathrm{d}x\mathrm{d}y=2\iint_{D_1}xy\,\mathrm{d}x\mathrm{d}y=2\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{\sqrt{\sin 2\theta}}r^3\cos\theta\sin\theta\,\mathrm{d}r=\frac{1}{6}.$$

**【注】** 设 $D$ 关于原点对称，则

$$\iint_D f(x,y)\,\mathrm{d}x\mathrm{d}y=\begin{cases}2\displaystyle\iint_{D_1}f(x,y)\,\mathrm{d}x\mathrm{d}y,& f(x,y)\ \text{关于}\ x,y\ \text{是偶函数},\\ 0,& f(x,y)\ \text{关于}\ x,y\ \text{是奇函数},\end{cases}$$

其中 $D_1=D\cap\{(x,y)\mid x\geqslant0\}$。

+++

#### 基础解答 (11) 设 $V$ 由曲面 $z=\sqrt{R^2-x^2-y^2}$ 与 $z=\sqrt{x^2+y^2}$ 所围，求 $I=\iiint_V z\,\mathrm{d}V$.
***
用球坐标 $x=r\sin\varphi\cos\theta$，$y=r\sin\varphi\sin\theta$，$z=r\cos\varphi$，则 $V$ 为

$$0\leqslant r\leqslant R,\quad 0\leqslant\varphi\leqslant\frac{\pi}{4},\quad 0\leqslant\theta\leqslant2\pi,$$

故

$$I=\iiint_V z\,\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{4}}\mathrm{d}\varphi\int_0^R r^2\sin\varphi\cdot r\cos\varphi\,\mathrm{d}r=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{4}}\sin\varphi\cos\varphi\,\mathrm{d}\varphi\int_0^R r^3\,\mathrm{d}r$$

$$=2\pi\cdot\left.\left(\frac{1}{2}\sin^2\varphi\right)\right|_0^{\frac{\pi}{4}}\cdot\left.\left(\frac{1}{4}r^4\right)\right|_0^R=\frac{\pi R^4}{8}.$$

+++

#### 基础解答 (12) 设 $V$ 是由曲面 $z=\sqrt{1-x^2-y^2}$ 与 $z+1=\sqrt{x^2+y^2}$ 所围的区域，计算 $I=\iiint_V z^2\,\mathrm{d}V$.
***
用柱面坐标，积分区域 $V$ 为

$$0\leqslant\theta\leqslant2\pi,\quad 0\leqslant r\leqslant1,\quad r-1\leqslant z\leqslant\sqrt{1-r^2},$$

故

$$I=\iiint_V z^2\,\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\,\mathrm{d}r\int_{r-1}^{\sqrt{1-r^2}}z^2\,\mathrm{d}z=\frac{2\pi}{3}\int_0^1\left[r(1-r^2)^{\frac{3}{2}}-r(r-1)^3\right]\mathrm{d}r=\frac{\pi}{6}.$$

**【注】** 此题若采用球面坐标需分两个区域积分：

$$I=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{2}}\mathrm{d}\varphi\int_0^1 r^2\cos^2\varphi\cdot r^2\sin\varphi\,\mathrm{d}r+\int_0^{2\pi}\mathrm{d}\theta\int_{\frac{\pi}{2}}^{\pi}\mathrm{d}\varphi\int_0^{\frac{1}{\sin\varphi-\cos\varphi}}r^2\cos^2\varphi\cdot r^2\sin\varphi\,\mathrm{d}r,$$

显然计算量较大。

+++

#### 基础解答 (13) 求曲面 $z=\sqrt{5-x^2-y^2}$ 与 $x^2+y^2=4z$ 所围立体体积.
***
立体体积 $V$ 可视为以 $z=\sqrt{5-x^2-y^2}$ 为曲顶的柱体体积与以 $x^2+y^2=4z$ 为曲顶的柱体体积之差。两曲面的交线由 $\begin{cases}z=\sqrt{5-x^2-y^2},\\ x^2+y^2=4z\end{cases}$ 消去 $z$ 得 $D:x^2+y^2=4$，故

$$V=\iint_D\left[\sqrt{5-x^2-y^2}-\frac{1}{4}(x^2+y^2)\right]\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}\theta\int_0^2\left(\sqrt{5-r^2}-\frac{1}{4}r^2\right)r\,\mathrm{d}r$$

$$=2\pi\int_0^2\left(\sqrt{5-r^2}-\frac{1}{4}r^2\right)r\,\mathrm{d}r=2\pi\int_0^2 r\sqrt{5-r^2}\,\mathrm{d}r-\frac{\pi}{2}\int_0^2 r^3\,\mathrm{d}r=\frac{2\pi}{3}(5\sqrt{5}-4).$$

**【注】** 此题也可采用三重积分计算：$V=\iiint_V\mathrm{d}V$，用柱面坐标，有

$$V=\iiint_V\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^2 r\,\mathrm{d}r\int_{\frac{1}{4}r^2}^{\sqrt{5-r^2}}\mathrm{d}z=2\pi\int_0^2\left(\sqrt{5-r^2}-\frac{1}{4}r^2\right)r\,\mathrm{d}r=\frac{2\pi}{3}(5\sqrt{5}-4).$$

+++

#### 基础解答 (14) 设 $V$ 是由 $x^2+y^2+z^2=R^2$ 与 $x^2+y^2+(z-R)^2=R^2$ 所围的区域，计算 $I=\iiint_V z^2\,\mathrm{d}V$.
***
$V$ 由两个球面所围。由 $\begin{cases}x^2+y^2+z^2=R^2,\\ x^2+y^2+(z-R)^2=R^2,\end{cases}$ 解得 $z=\dfrac{R}{2}$，于是积分区域 $V$ 在 $xOy$ 面上的投影曲线为

$$\begin{cases}x^2+y^2=\left(\dfrac{\sqrt{3}}{2}R\right)^2,\\ z=0.\end{cases}$$

考虑到被积函数仅含 $z$，采用直角坐标的"先二后一"，有

$$I=\iiint_V z^2\,\mathrm{d}V=\int_0^{\frac{R}{2}}z^2\,\mathrm{d}z\iint_{x^2+y^2\leqslant 2Rz-z^2}\mathrm{d}x\mathrm{d}y+\int_{\frac{R}{2}}^{R}z^2\,\mathrm{d}z\iint_{x^2+y^2\leqslant R^2-z^2}\mathrm{d}x\mathrm{d}y$$

$$=\pi\int_0^{\frac{R}{2}}z^2(2Rz-z^2)\,\mathrm{d}z+\pi\int_{\frac{R}{2}}^{R}z^2(R^2-z^2)\,\mathrm{d}z$$

$$=\left.\pi\left[\frac{R}{2}z^4-\frac{1}{5}z^5\right]\right|_0^{\frac{R}{2}}+\left.\pi\left[\frac{R^2}{3}z^3-\frac{1}{5}z^5\right]\right|_{\frac{R}{2}}^{R}=\frac{59}{480}\pi R^5.$$

**【注】** 此题也可采用下列方法：

① "先一后二"：$I=\iint_{x^2+y^2\leqslant\frac{3}{4}R^2}\mathrm{d}x\mathrm{d}y\int_{R-\sqrt{R^2-x^2-y^2}}^{\sqrt{R^2-x^2-y^2}}z^2\,\mathrm{d}z$，显然积分较烦琐。

② 柱面坐标：$I=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\sqrt{3}}{2}R}r\,\mathrm{d}r\int_{R-\sqrt{R^2-r^2}}^{\sqrt{R^2-r^2}}z^2\,\mathrm{d}z$。

③ 球面坐标：由 $\begin{cases}z=\dfrac{R}{2},\\ x^2+y^2=\left(\dfrac{\sqrt{3}}{2}R\right)^2\end{cases}$ 化为球坐标，得 $\begin{cases}r\cos\varphi=\dfrac{R}{2},\\ r\sin\varphi=\dfrac{\sqrt{3}}{2}R,\end{cases}$ 解得 $\varphi=\dfrac{\pi}{3}$，故分区域积分有

$$I=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{3}}\sin\varphi\cos^2\varphi\,\mathrm{d}\varphi\int_0^R r^4\,\mathrm{d}r+\int_0^{2\pi}\mathrm{d}\theta\int_{\frac{\pi}{3}}^{\frac{\pi}{2}}\sin\varphi\cos^2\varphi\,\mathrm{d}\varphi\int_0^{2R\cos\varphi}r^4\,\mathrm{d}r.$$

比较以上情形，知选择"先二后一"较为方便。

+++

#### 综合选择 (1) 设 $I_1=\iint_{D}\cos\sqrt{x^2+y^2}\,\mathrm{d}x\mathrm{d}y$，$I_2=\iint_{D}\cos(x^2+y^2)\mathrm{d}x\mathrm{d}y$，$I_3=\iint_{D}\cos(x^2+y^2)^2\,\mathrm{d}x\mathrm{d}y$，其中 $D:x^2+y^2\leqslant1$，则（　）。

;;;
A. $I_1>I_2>I_3$
B. $I_1<I_2<I_3$
C. $I_2>I_1>I_3$
D. $I_3>I_1>I_2$
;;;B
***
在 $D:0\leqslant x^2+y^2\leqslant1$ 上有

$$\frac{\pi}{2}>1\geqslant\sqrt{x^2+y^2}\geqslant x^2+y^2\geqslant(x^2+y^2)^2\geqslant0,$$

且 $\cos x$ 在 $\left[0,\frac{\pi}{2}\right)$ 上为**单调减少**函数，故

$$0\leqslant\cos\sqrt{x^2+y^2}\leqslant\cos(x^2+y^2)\leqslant\cos(x^2+y^2)^2,$$

由二重积分的保序性，所以 $I_1<I_2<I_3$，**B 正确**。

+++

#### 综合选择 (2) $\lim\limits_{n\to\infty}\sum\limits_{i=1}^{n}\sum\limits_{j=1}^{n}\dfrac{1}{\left(1+\frac{i}{n}\right)(n^2+j^2)}=$（　）。

;;;
A. $\frac{\pi}{4}\ln 2$
B. $\frac{\pi}{8}\ln 2$
C. $\frac{\pi}{2}\ln 2$
D. $\pi\ln 2$
;;;A
***
利用**二重积分的定义**，有

$$\lim_{n\to\infty}\frac{1}{n^2}\sum_{i=1}^{n}\sum_{j=1}^{n}f\left(\frac{i}{n},\frac{j}{n}\right)=\int_0^1\mathrm{d}x\int_0^1 f(x,y)\mathrm{d}y,$$

原极限
$$=\lim_{n\to\infty}\frac{1}{n^2}\sum_{i=1}^{n}\sum_{j=1}^{n}\frac{1}{\left(1+\frac{i}{n}\right)\left[1+\left(\frac{j}{n}\right)^2\right]}
=\int_0^1\frac{\mathrm{d}x}{1+x}\int_0^1\frac{\mathrm{d}y}{1+y^2}$$

$$=\int_0^1\frac{1}{1+x}\cdot\arctan y\Big|_0^1\mathrm{d}x=\frac{\pi}{4}\int_0^1\frac{\mathrm{d}x}{1+x}=\frac{\pi}{4}\ln(1+x)\Big|_0^1=\frac{\pi}{4}\ln 2.$$

+++

#### 综合选择 (3) 积分 $I=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{\cos\theta}f(r\cos\theta,r\sin\theta)r\mathrm{d}r=$（　）。

;;;
A. $\int_0^1\mathrm{d}y\int_0^{\sqrt{y-y^2}}f(x,y)\mathrm{d}x$
B. $\int_0^1\mathrm{d}y\int_0^{\sqrt{1-y^2}}f(x,y)\mathrm{d}x$
C. $\int_0^1\mathrm{d}y\int_0^1 f(x,y)\mathrm{d}x$
D. $\int_0^1\mathrm{d}x\int_0^{\sqrt{x-x^2}}f(x,y)\mathrm{d}y$
;;;D
***
此题是**极坐标下的二次积分化为直角坐标下的二次积分**，关键是正确画图。

由 $0\leqslant\theta\leqslant\frac{\pi}{2}$，知 $0\leqslant x\leqslant1$。

$$r=\cos\theta\Rightarrow r^2=r\cos\theta\Rightarrow x^2+y^2=x,$$

即 $y=\sqrt{x-x^2}$，故

$$I=\int_0^1\mathrm{d}x\int_0^{\sqrt{x-x^2}}f(x,y)\mathrm{d}y.$$

**【注】** 一般二次积分的极坐标与直角坐标的相互转化，利用 $x=r\cos\theta,\ y=r\sin\theta$，或 $x^2+y^2=r^2,\ \tan\theta=\frac{y}{x}$。

+++

#### 综合填空 (1) 设 $D:0\leqslant x\leqslant y\leqslant2\pi$，则 $I=\iint_{D}|\sin(x-y)|\mathrm{d}x\mathrm{d}y=$ ________.
***
$4\pi$.

为去掉绝对值符号，用 $y=x+\pi$ 将 $D$ 划分为 $D_1$ 与 $D_2$：

$$D_1:-\pi\leqslant x-y\leqslant0,\qquad D_2:-2\pi\leqslant x-y\leqslant-\pi,$$

故
$$I=\iint_{D}|\sin(x-y)|\mathrm{d}x\mathrm{d}y=\iint_{D_1}[-\sin(x-y)]\mathrm{d}x\mathrm{d}y+\iint_{D_2}\sin(x-y)\mathrm{d}x\mathrm{d}y$$

$$=\int_0^{\pi}\mathrm{d}y\int_0^{y}[-\sin(x-y)]\mathrm{d}x+\int_{\pi}^{2\pi}\mathrm{d}y\int_{y-\pi}^{y}[-\sin(x-y)]\mathrm{d}x+\int_{\pi}^{2\pi}\mathrm{d}y\int_0^{y-\pi}\sin(x-y)\mathrm{d}x=4\pi.$$

+++

#### 综合填空 (2) 设 $f(x)$ 为下面的分段函数，$D:-\infty<x<+\infty,\ -\infty<y<+\infty$，则 $I=\iint_{D}f(y)f(x+y)\mathrm{d}x\mathrm{d}y=$ ________.

$$f(x)=\begin{cases}x,&0\leqslant x\leqslant1,\\0,&\text{其他}.\end{cases}$$
***
$\dfrac{1}{4}$.

由已知，有

$$f(y)=\begin{cases}y,&0\leqslant y\leqslant1,\\0,&\text{其他},\end{cases}\qquad
f(x+y)=\begin{cases}x+y,&0\leqslant x+y\leqslant1,\\0,&\text{其他},\end{cases}$$

故 $D_1=\{(x,y)\mid -y\leqslant x\leqslant1-y,\ 0\leqslant y\leqslant1\}$。

在 $D_1$ 上 $f(y)=y,\ f(x+y)=x+y$；在 $D_1$ 以外部分 $f(y)=0$ 或 $f(x+y)=0$，故

$$I=\iint_{D}f(y)f(x+y)\mathrm{d}x\mathrm{d}y=\iint_{D_1}y(x+y)\mathrm{d}x\mathrm{d}y=\int_0^1\mathrm{d}y\int_{-y}^{1-y}y(x+y)\mathrm{d}x$$

$$=\int_0^1 y\cdot\frac{1}{2}(x+y)^2\Big|_{-y}^{1-y}\mathrm{d}y=\int_0^1\frac{1}{2}y\,\mathrm{d}y=\frac{1}{4}.$$

+++

#### 综合填空 (3) 设 $D=\left\{(x,y)\ \middle|\ \dfrac{x}{4}\leqslant x^2+y^2\leqslant\dfrac{x}{2},\ \dfrac{y}{4}\leqslant x^2+y^2\leqslant\dfrac{y}{2}\right\}$，则 $I=\iint_{D}\dfrac{1}{xy}\mathrm{d}x\mathrm{d}y=$ ________.
***
$(\ln 2)^2$.

利用**极坐标**求解。$D$ 关于 $y=x$ 对称，且

$$D:\frac{1}{4}\cos\theta\leqslant r\leqslant\frac{1}{2}\cos\theta,\quad \frac{1}{4}\sin\theta\leqslant r\leqslant\frac{1}{2}\sin\theta,$$

故由 $r=\frac{1}{2}\sin\theta,\ r=\frac{1}{4}\cos\theta$ 解得 $\theta=\arctan\frac{1}{2}$，故

$$I=\iint_{D}\frac{1}{xy}\mathrm{d}x\mathrm{d}y=2\int_{\arctan\frac{1}{2}}^{\frac{\pi}{4}}\mathrm{d}\theta\int_{\frac{1}{4}\cos\theta}^{\frac{1}{2}\sin\theta}\frac{\mathrm{d}r}{r\sin\theta\cos\theta}$$

$$=2\int_{\arctan\frac{1}{2}}^{\frac{\pi}{4}}\frac{1}{\sin\theta\cos\theta}\ln\frac{\frac{1}{2}\sin\theta}{\frac{1}{4}\cos\theta}\mathrm{d}\theta
=2\int_{\arctan\frac{1}{2}}^{\frac{\pi}{4}}\frac{1}{\tan\theta}\ln(2\tan\theta)\mathrm{d}(\tan\theta)=(\ln 2)^2.$$

+++

#### 综合填空 (4) 积分 $I=\int_0^1\mathrm{d}y\int_0^{y^2}y\sin(1-x)^2\mathrm{d}x=$ ________.
***
$\dfrac{1}{4}(1-\cos 1)$.

**交换积分顺序**，得

$$I=\int_0^1\mathrm{d}x\int_{\sqrt{x}}^{1}y\sin(1-x)^2\mathrm{d}y=\int_0^1\frac{y^2}{2}\sin(1-x)^2\Big|_{\sqrt{x}}^{1}\mathrm{d}x$$

$$=\frac{1}{2}\int_0^1(1-x)\sin(1-x)^2\mathrm{d}x=-\frac{1}{4}\int_0^1\sin(1-x)^2\mathrm{d}\left[(1-x)^2\right]$$

$$=\frac{1}{4}\cos(1-x)^2\Big|_0^1=\frac{1}{4}(1-\cos 1).$$

+++

#### 综合填空 (5) 积分 $I=\int_0^{2\pi}\mathrm{d}\theta\int_{\frac{\theta}{2}}^{\pi}\theta^2\mathrm{e}^{r^2}\mathrm{d}r=$ ________.
***
$\dfrac{4}{3}\mathrm{e}^{\pi^2}(\pi^2-1)+\dfrac{4}{3}$.

**交换极坐标顺序**，则

$$I=\int_0^{\pi}\mathrm{d}r\int_0^{2r}\theta^2\mathrm{e}^{r^2}\mathrm{d}\theta=\int_0^{\pi}\mathrm{e}^{r^2}\cdot\frac{1}{3}\theta^3\Big|_0^{2r}\mathrm{d}r=\int_0^{\pi}\mathrm{e}^{r^2}\cdot\frac{8}{3}r^3\mathrm{d}r$$

令 $r^2=t$，
$$=\frac{8}{3}\int_0^{\pi^2}\frac{1}{2}t\mathrm{e}^{t}\mathrm{d}t=\frac{4}{3}\int_0^{\pi^2}t\mathrm{e}^{t}\mathrm{d}t=\frac{4}{3}\mathrm{e}^{t}(t-1)\Big|_0^{\pi^2}=\frac{4}{3}\mathrm{e}^{\pi^2}(\pi^2-1)+\frac{4}{3}.$$

+++

#### 综合填空 (6) 交换积分顺序 $I=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{a\sqrt{\sin 2\theta}}f(r\cos\theta,r\sin\theta)r\mathrm{d}r\ (a>0)$ 为 ________.
***
$$I=\int_0^{a}\mathrm{d}r\int_{\frac{1}{2}\arcsin\frac{r^2}{a^2}}^{\frac{\pi}{2}-\frac{1}{2}\arcsin\frac{r^2}{a^2}}f(r\cos\theta,r\sin\theta)r\mathrm{d}\theta.$$

极坐标下交换积分顺序可**视 $\theta$ 为 $x$ 轴，$r$ 为 $y$ 轴**，用直角坐标处理（包括画图和确定积分限）。

当 $0\leqslant\theta\leqslant\frac{\pi}{4}$ 时，$r=a\sqrt{\sin 2\theta}$ 的反函数为

$$\theta=\frac{1}{2}\arcsin\frac{r^2}{a^2};$$

当 $\frac{\pi}{4}<\theta\leqslant\frac{\pi}{2}$ 时，$r=a\sqrt{\sin 2\theta}$ 的反函数为

$$\theta=\frac{\pi}{2}-\frac{1}{2}\arcsin\frac{r^2}{a^2},$$

故得上述结果。

+++

#### 综合填空 (7) （选做）设 $D:\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}\leqslant1$，则 $I=\iint_{D}y^2\mathrm{d}x\mathrm{d}y=$ ________.
***
$\dfrac{\pi ab^3}{4}$.

由于 $D$ 为椭圆形区域，故用**广义极坐标**进行计算。

令 $x=ar\cos\theta,\ y=br\sin\theta$，则 $D:\frac{x^2}{a^2}+\frac{y^2}{b^2}\leqslant1$ 变为 $D':0\leqslant r\leqslant1,\ 0\leqslant\theta\leqslant2\pi$，其变换雅可比行列式为

$$J=\frac{\partial(x,y)}{\partial(r,\theta)}=\begin{vmatrix}a\cos\theta&-ar\sin\theta\\ b\sin\theta&br\cos\theta\end{vmatrix}=abr,$$

故
$$\iint_{D}y^2\mathrm{d}x\mathrm{d}y=\iint_{D'}(br\sin\theta)^2|J|\mathrm{d}r\mathrm{d}\theta=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 b^2r^2\sin^2\theta\cdot abr\,\mathrm{d}r=\frac{\pi ab^3}{4}.$$

**【注】** 广义极坐标属于了解内容。

+++

#### 综合填空 (8) 设 $V$ 是由 $z=\sqrt{x^2+y^2},z=1,z=2$ 所围成的立体，计算 $I=\iiint_{V}\dfrac{\mathrm{e}^{z}}{\sqrt{x^2+y^2}}\mathrm{d}x\mathrm{d}y\mathrm{d}z=$ ________.
***
$2\pi\mathrm{e}^2$.

考虑到被积函数，可采用直角坐标下的**“先二后一”**，则

$$I=\int_1^2\mathrm{e}^{z}\mathrm{d}z\iint_{D_z}\frac{1}{\sqrt{x^2+y^2}}\mathrm{d}x\mathrm{d}y,$$

其中 $D_z:x^2+y^2\leqslant z^2$，又因为

$$\iint_{D_z}\frac{1}{\sqrt{x^2+y^2}}\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}\theta\int_0^{z}\frac{1}{r}r\mathrm{d}r=2\pi z,$$

所以
$$I=\int_1^2 2\pi z\mathrm{e}^{z}\mathrm{d}z=2\pi\left(z\mathrm{e}^{z}\Big|_1^2-\int_1^2\mathrm{e}^{z}\mathrm{d}z\right)=2\pi\mathrm{e}^2.$$

**【注】** 此题若采用“先一后二”或球面坐标的方法，计算量较大。

+++

#### 综合填空 (9) 积分 $I=\int_0^1\mathrm{d}x\int_0^{1-x}\mathrm{d}z\int_0^{1-x-z}(1-y)\mathrm{e}^{-(1-y-z)^2}\mathrm{d}y=$ ________.
***
$\dfrac{1}{4\mathrm{e}}$.

直接积分比较困难，**交换积分顺序**，先对 $x$ 积分，得

$$I=\iiint_{V}(1-y)\mathrm{e}^{-(1-y-z)^2}\mathrm{d}V=\iint_{D_{yz}}\mathrm{d}y\mathrm{d}z\int_0^{1-y-z}(1-y)\mathrm{e}^{-(1-y-z)^2}\mathrm{d}x$$

$$=\iint_{D_{yz}}(1-y)(1-y-z)\mathrm{e}^{-(1-y-z)^2}\mathrm{d}y\mathrm{d}z=\int_0^1(1-y)\mathrm{d}y\int_0^{1-y}(1-y-z)\mathrm{e}^{-(1-y-z)^2}\mathrm{d}z$$

$$=\frac{1}{2}\int_0^1(1-y)\left[\mathrm{e}^{-(1-y-z)^2}\right]\Big|_0^{1-y}\mathrm{d}y=\frac{1}{2}\int_0^1(1-y)\left[1-\mathrm{e}^{-(1-y)^2}\right]\mathrm{d}y=\frac{1}{4\mathrm{e}}.$$

+++

#### 综合填空 (10) 设 $V$ 是由曲面 $x^2+y^2-2z^2=1$、平面 $z=1$ 及 $z=2$ 所围成的区域，则 $I=\iiint_{V}z\mathrm{d}V=$ ________.
***
$9\pi$.

由于被积函数仅与 $z$ 有关，所以采用**“先二后一”**。$D_z$ 为 $x^2+y^2\leqslant1+2z^2\ (1\leqslant z\leqslant2)$，$D_z$ 的面积为 $\pi(1+2z^2)$，故

$$I=\iiint_{V}z\mathrm{d}V=\int_1^2 z\mathrm{d}z\iint_{D_z}\mathrm{d}x\mathrm{d}y=\int_1^2\pi(1+2z^2)z\mathrm{d}z=9\pi.$$

+++

#### 综合填空 (11) 设 $V$ 由曲面 $z=\sqrt{x^2+y^2}$ 与 $z=\sqrt{1-x^2-y^2}$ 所围，则 $I=\iiint_{V}(x+z)\mathrm{d}V=$ ________.
***
$\dfrac{\pi}{8}$.

$V$ 由下半圆锥与上半球面所围，$V$ 关于 $yOz$ 面对称，且被积函数 $x$ 是**奇函数**，故 $\iiint_{V}x\mathrm{d}V=0$，则

$$I=\iiint_{V}(x+z)\mathrm{d}V=0+\iiint_{V}z\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{4}}\mathrm{d}\varphi\int_0^1 r\cos\varphi\cdot r^2\sin\varphi\mathrm{d}r=\frac{\pi}{8}.$$

+++

#### 综合解答 (1) 设 $D:|x|\leqslant1,0\leqslant y\leqslant2$，计算 $I=\iint_{D}|y-x^2|\mathrm{d}x\mathrm{d}y$.
***
由 $y=x^2$ 将 $D$ 划分为 $D_1$ 与 $D_2$，则

$$I=\iint_{D}|y-x^2|\mathrm{d}x\mathrm{d}y=\iint_{D_1}(y-x^2)\mathrm{d}x\mathrm{d}y+\iint_{D_2}(x^2-y)\mathrm{d}x\mathrm{d}y$$

$$=\int_{-1}^{1}\mathrm{d}x\int_{x^2}^{2}(y-x^2)\mathrm{d}y+\int_{-1}^{1}\mathrm{d}x\int_0^{x^2}(x^2-y)\mathrm{d}y$$

$$=\int_{-1}^{1}\frac{1}{2}(y-x^2)^2\Big|_{x^2}^{2}\mathrm{d}x-\int_{-1}^{1}\frac{1}{2}(y-x^2)^2\Big|_0^{x^2}\mathrm{d}x$$

$$=\frac{1}{2}\int_{-1}^{1}(4-4x^2+x^4)\mathrm{d}x+\frac{1}{2}\int_{-1}^{1}x^4\mathrm{d}x$$

$$=2\int_0^1(2-2x^2+x^4)\mathrm{d}x=2\times\left(2-\frac{2}{3}+\frac{1}{5}\right)=\frac{46}{15}.$$

+++

#### 综合解答 (2) 计算积分

$$I=\int_0^1\mathrm{d}x\int_{1-x}^{2-x}\mathrm{e}^{(x+y)^2}(\sin^2x+\cos^2y)\mathrm{d}y+\int_1^2\mathrm{d}x\int_0^{2-x}\mathrm{e}^{(x+y)^2}(\sin^2x+\cos^2y)\mathrm{d}y.$$
***
积分区域 $D$ 为 $1\leqslant x+y\leqslant2$ 位于第一象限的部分，显然 $D$ 关于直线 $x=y$ **对称**，则

$$I=\iint_{D}\mathrm{e}^{(x+y)^2}(\sin^2x+\cos^2y)\mathrm{d}x\mathrm{d}y$$

$$=\frac{1}{2}\iint_{D}\left[\mathrm{e}^{(x+y)^2}(\sin^2x+\cos^2y)+\mathrm{e}^{(y+x)^2}(\sin^2y+\cos^2x)\right]\mathrm{d}x\mathrm{d}y$$

$$=\iint_{D}\mathrm{e}^{(x+y)^2}\mathrm{d}x\mathrm{d}y=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_{\frac{1}{\cos\theta+\sin\theta}}^{\frac{2}{\cos\theta+\sin\theta}}\mathrm{e}^{r^2(\cos\theta+\sin\theta)^2}\cdot r\mathrm{d}r$$

$$=\frac{1}{2}\int_0^{\frac{\pi}{2}}\frac{1}{(\cos\theta+\sin\theta)^2}\cdot\mathrm{e}^{r^2(\cos\theta+\sin\theta)^2}\Big|_{\frac{1}{\cos\theta+\sin\theta}}^{\frac{2}{\cos\theta+\sin\theta}}\mathrm{d}\theta$$

$$=\frac{1}{2}(\mathrm{e}^4-\mathrm{e})\int_0^{\frac{\pi}{2}}\frac{\mathrm{d}\theta}{(\cos\theta+\sin\theta)^2}=\frac{1}{2}(\mathrm{e}^4-\mathrm{e})\int_0^{\frac{\pi}{2}}\frac{\mathrm{d}(\tan\theta)}{(1+\tan\theta)^2}$$

$$=\frac{1}{2}(\mathrm{e}^4-\mathrm{e})\left(-\frac{1}{1+\tan\theta}\right)\Big|_0^{\frac{\pi}{2}}=\frac{1}{2}\mathrm{e}(\mathrm{e}^3-1).$$

+++

#### 综合解答 (3) 求极限 $\lim\limits_{t\to0^+}\dfrac{1}{t^6}\int_0^t\mathrm{d}x\int_x^t\sin(xy)^2\mathrm{d}y$.
***
$\frac{0}{0}$ 型，利用洛必达法则，需**交换积分顺序**：

$$\int_0^t\mathrm{d}x\int_x^t\sin(xy)^2\mathrm{d}y=\int_0^t\mathrm{d}y\int_0^{y}\sin(xy)^2\mathrm{d}x,$$

故
$$\text{原式}=\lim_{t\to0^+}\frac{\int_0^t\mathrm{d}y\int_0^{y}\sin(xy)^2\mathrm{d}x}{t^6}=\lim_{t\to0^+}\frac{\int_0^t\sin(tx)^2\mathrm{d}x}{6t^5}$$

令 $tx=u$，即 $x=\frac{1}{t}u$，
$$=\lim_{t\to0^+}\frac{\int_0^{t^2}\sin u^2\cdot\frac{1}{t}\mathrm{d}u}{6t^5}=\lim_{t\to0^+}\frac{\int_0^{t^2}\sin u^2\mathrm{d}u}{6t^6}=\lim_{t\to0^+}\frac{2t\sin t^4}{36t^5}=\frac{1}{18}.$$

+++

#### 综合解答 (4) 计算 $I=\int_{\arctan\frac{1}{4}}^{\frac{\pi}{4}}\mathrm{d}\theta\int_{\frac{1}{\sqrt{\sin\theta\cos\theta}}}^{\frac{2}{\cos\theta}}r^2\cos\theta\mathrm{d}r$.
***
直接计算极坐标下的二次积分较烦琐，将其**化为直角坐标下的二次积分**：

$$\theta=\frac{\pi}{4}\Rightarrow y=x;\qquad r=\frac{2}{\cos\theta}\Rightarrow x=2;$$

$$r=\frac{1}{\sqrt{\sin\theta\cos\theta}}\Rightarrow r=\frac{r}{\sqrt{r^2\sin\theta\cos\theta}}\Rightarrow 1=\frac{1}{\sqrt{yx}}\Rightarrow xy=1.$$

故在直角坐标系下有

$$I=\int_1^2\mathrm{d}x\int_{\frac{1}{x}}^{x}x\mathrm{d}y=\int_1^2 x\left(x-\frac{1}{x}\right)\mathrm{d}x=\int_1^2 x^2\mathrm{d}x-\int_1^2\mathrm{d}x=\frac{4}{3}.$$

+++

#### 综合解答 (5) 设可导函数 $f(x)$ 满足 $\lim\limits_{x\to0}\dfrac{f(x)}{x}=1$，求极限

$$\lim_{t\to0^+}\frac{\int_0^t\mathrm{d}x\int_{-\sqrt{t^2-x^2}}^{\sqrt{t^2-x^2}}\left[f(\sqrt{x^2+y^2})+2y\right]\mathrm{d}y}{t^3}.$$
***
先化内层积分（$2y$ 关于 $y$ 为奇函数，积分为零）：

$$\int_{-\sqrt{t^2-x^2}}^{\sqrt{t^2-x^2}}\left[f(\sqrt{x^2+y^2})+2y\right]\mathrm{d}y=2\int_0^{\sqrt{t^2-x^2}}f(\sqrt{x^2+y^2})\mathrm{d}y,$$

令 $\sqrt{x^2+y^2}=u$，得 $=2\displaystyle\int_x^t\frac{uf(u)}{\sqrt{u^2-x^2}}\mathrm{d}u$，故

$$\text{原式}=\lim_{t\to0^+}\frac{2\int_0^t\mathrm{d}x\int_x^t\frac{uf(u)}{\sqrt{u^2-x^2}}\mathrm{d}u}{t^3}=2\lim_{t\to0^+}\frac{\int_0^t uf(u)\mathrm{d}u\int_0^{u}\frac{1}{\sqrt{u^2-x^2}}\mathrm{d}x}{t^3}$$

$$=\pi\lim_{t\to0^+}\frac{\int_0^t uf(u)\mathrm{d}u}{t^3}=\pi\lim_{t\to0^+}\frac{tf(t)}{3t^2}=\frac{\pi}{3}.$$

+++

#### 综合解答 (6) 设 $F(t)$ 由下式确定，求函数 $F(t)$ 的表达式.

$$F(t)=\begin{cases}\displaystyle\iint_{\substack{x^2+y^2\leqslant t^2\\ x\geqslant0,\ y\geqslant0}}x\left[1-\frac{F(\sqrt{x^2+y^2})}{x^2+y^2}\right]\mathrm{d}x\mathrm{d}y,&t\neq0,\\[2mm] 0,&t=0.\end{cases}$$
***
用**极坐标**。当 $t\neq0$ 时，

$$F(t)=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{t}r\cos\theta\left[1-\frac{F(r)}{r^2}\right]\cdot r\mathrm{d}r=\int_0^{\frac{\pi}{2}}\cos\theta\mathrm{d}\theta\int_0^{t}r^2\left[1-\frac{F(r)}{r^2}\right]\mathrm{d}r$$

$$=\sin\theta\Big|_0^{\frac{\pi}{2}}\cdot\int_0^{t}\left[r^2-F(r)\right]\mathrm{d}r=\int_0^t r^2\mathrm{d}r-\int_0^t F(r)\mathrm{d}r=\frac{1}{3}t^3-\int_0^t F(r)\mathrm{d}r,$$

即 $F(t)=\frac{1}{3}t^3-\int_0^t F(r)\mathrm{d}r$。①

① 式两边同时对 $t$ 求导，得 $F'(t)=t^2-F(t)$，即 $F'(t)+F(t)=t^2$，该式为**一阶线性微分方程**，解得

$$F(t)=\mathrm{e}^{-\int\mathrm{d}t}\left[\int t^2\mathrm{e}^{\int\mathrm{d}t}\mathrm{d}t+C\right]=t^2-2t+2+C\mathrm{e}^{-t}.$$

由已知 $F(0)=0$，得 $C=-2$，故 $F(t)=t^2-2t+2-2\mathrm{e}^{-t}$.

+++

#### 综合解答 (7) 设 $f(t)$ 在 $(-\infty,+\infty)$ 内有连续导数，且 $f(t)=2\iint_{D}(x^2+y^2)f(\sqrt{x^2+y^2})\mathrm{d}x\mathrm{d}y+t^4$，$D:x^2+y^2\leqslant t^2$，求 $f(t)$.
***
由已知，$f(0)=0$，$f(t)$ 是**偶函数**，只需讨论 $t>0$ 的情况。用极坐标，有

$$f(t)=2\int_0^{2\pi}\mathrm{d}\theta\int_0^t r^3f(r)\mathrm{d}r+t^4=4\pi\int_0^t r^3f(r)\mathrm{d}r+t^4,$$

上式两边同时对 $t$ 求导，得 $f'(t)=4\pi t^3f(t)+4t^3$，且 $f(0)=0$，解此一阶线性微分方程，得

$$f(t)=\frac{1}{\pi}(\mathrm{e}^{\pi t^4}-1),\quad t\geqslant0.$$

而 $f(t)$ 是偶函数，故在 $(-\infty,+\infty)$ 内有 $f(t)=\dfrac{1}{\pi}(\mathrm{e}^{\pi t^4}-1)$.

+++

#### 综合解答 (8) 设 $f(x,y)$ 在区域 $0\leqslant x\leqslant1,0\leqslant y\leqslant1$ 上连续，$f(0,0)=0$，且 $f(x,y)$ 在点 $(0,0)$ 处可微，$f_y'(0,0)=1$，求

$$\lim_{x\to0^+}\frac{\int_0^{x^2}\mathrm{d}t\int_x^{\sqrt{t}}f(t,u)\mathrm{d}u}{1-\mathrm{e}^{-\frac{x^4}{4}}}.$$
***
**交换积分顺序**：

$$\int_0^{x^2}\mathrm{d}t\int_x^{\sqrt{t}}f(t,u)\mathrm{d}u=-\int_0^{x}\mathrm{d}u\int_0^{u^2}f(t,u)\mathrm{d}t,$$

故
$$\text{原式}=\lim_{x\to0^+}\frac{-\int_0^{x}\mathrm{d}u\int_0^{u^2}f(t,u)\mathrm{d}t}{\frac{1}{4}x^4}\xlongequal{\text{洛必达法则}}\lim_{x\to0^+}\frac{-\int_0^{x^2}f(t,x)\mathrm{d}t}{x^3}.$$

由**积分中值定理**，$\int_0^{x^2}f(t,x)\mathrm{d}t=f(\xi,x)x^2\ (0\leqslant\xi\leqslant x^2)$，故

$$\text{原式}=\lim_{x\to0^+}\frac{-f(\xi,x)x^2}{x^3}.$$

由 $f(x,y)$ 在点 $(0,0)$ 处可微，则由可微的定义，有

$$f(\xi,x)=f(0,0)+f_x'(0,0)\xi+f_y'(0,0)x+o(\sqrt{x^2+\xi^2}),$$

又 $\left|\dfrac{f_x'(0,0)\xi}{x}\right|\leqslant\left|\dfrac{f_x'(0,0)x^2}{x}\right|=|f_x'(0,0)x|$，则

$$\lim_{x\to0^+}\frac{f_x'(0,0)\xi}{x}=0,\qquad \lim_{x\to0^+}\frac{o(\sqrt{x^2+\xi^2})}{x}=\lim_{x\to0^+}\frac{o(x)}{x}=0,$$

故
$$\lim_{x\to0^+}\frac{-f(\xi,x)x^2}{x^3}=\lim_{x\to0^+}\frac{f(0,0)+f_x'(0,0)\xi+f_y'(0,0)x+o(\sqrt{x^2+\xi^2})}{-x}=-f_y'(0,0)=-1.$$

+++

#### 综合解答 (9) 设 $D:x^2+y^2\leqslant4,x\geqslant0,y\geqslant0$，$f(x,y)$ 在 $D$ 上连续，且

$$f(x,y)=(x^2+y^2-x+y-1)+\iint_{D}f(u,v)\mathrm{d}u\mathrm{d}v,$$

求 $f(x,y)$.
***
设 $\iint_{D}f(u,v)\mathrm{d}u\mathrm{d}v=A$（$A$ 为一个数）。在已知等式两边同时取二重积分，得

$$A=\iint_{D}f(x,y)\mathrm{d}x\mathrm{d}y=\iint_{D}(x^2+y^2-x+y-1)\mathrm{d}x\mathrm{d}y+A\iint_{D}\mathrm{d}x\mathrm{d}y.$$

$D$ 关于直线 $x=y$ **对称**，则

$$A=\frac{1}{2}\iint_{D}(x^2+y^2-x+y-1+y^2+x^2-y+x-1)\mathrm{d}x\mathrm{d}y+A\cdot\frac{\pi}{4}\cdot2^2$$

$$=\iint_{D}(x^2+y^2-1)\mathrm{d}x\mathrm{d}y+\pi A=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^2(r^2-1)r\mathrm{d}r+\pi A=\pi+\pi A,$$

故 $A=\dfrac{\pi}{1-\pi}$，所求函数为

$$f(x,y)=x^2+y^2-x+y-1+\frac{\pi}{1-\pi}.$$

+++

#### 综合解答 (10) 设 $f(x)$ 是连续正值函数，且单调减少，证明：

$$\frac{\int_0^1 xf^2(x)\mathrm{d}x}{\int_0^1 xf(x)\mathrm{d}x}\leqslant\frac{\int_0^1 f^2(x)\mathrm{d}x}{\int_0^1 f(x)\mathrm{d}x}.$$
***
**证** 所证不等式变形为

$$I=\int_0^1 xf^2(x)\mathrm{d}x\int_0^1 f(x)\mathrm{d}x-\int_0^1 xf(x)\mathrm{d}x\int_0^1 f^2(x)\mathrm{d}x\leqslant0,$$

由定积分的值与积分变量的字母无关，故

$$I=\frac{1}{2}\int_0^1\mathrm{d}x\int_0^1\left[xf^2(x)f(y)-xf(x)f^2(y)+yf^2(y)f(x)-yf(y)f^2(x)\right]\mathrm{d}y$$

$$=\frac{1}{2}\iint_{D}\left[f(x)f(y)(x-y)\left[f(x)-f(y)\right]\right]\mathrm{d}x\mathrm{d}y,$$

其中 $D:0\leqslant x\leqslant1,0\leqslant y\leqslant1$ 为正方形。

由 $f(x)$ **单调减少**，知 $[f(x)-f(y)]$ 与 $(x-y)$ 异号，而 $f(x)>0,f(y)>0$，根据二重积分的性质，知 $I\leqslant0$，即所证不等式成立。

+++

#### 综合解答 (11) 设 $D$ 为由下述摆线（$0\leqslant t\leqslant2\pi$）及 $x$ 轴所围的平面区域，求 $D$ 的质心坐标.

$$\begin{cases}x=t-\sin t,\\ y=1-\cos t.\end{cases}$$
***
设其密度为常数 $\rho$，考虑 $D$ 的**对称性**，质心在 $x=\pi$ 上，即 $\overline{x}=\pi$，只需求

$$\overline{y}=\frac{\iint_{D}y\rho\mathrm{d}x\mathrm{d}y}{\iint_{D}\rho\mathrm{d}x\mathrm{d}y}=\frac{\iint_{D}y\mathrm{d}x\mathrm{d}y}{\iint_{D}\mathrm{d}x\mathrm{d}y}.$$

而面积

$$\iint_{D}\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}y(x)\mathrm{d}x=\int_0^{2\pi}(1-\cos t)\cdot(1-\cos t)\mathrm{d}t=3\pi,$$

故
$$\overline{y}=\frac{1}{3\pi}\iint_{D}y\mathrm{d}x\mathrm{d}y=\frac{1}{3\pi}\int_0^{2\pi}\mathrm{d}x\int_0^{y(x)}y\mathrm{d}y=\frac{1}{6\pi}\int_0^{2\pi}\left[y(x)\right]^2\mathrm{d}x=\frac{1}{6\pi}\int_0^{2\pi}(1-\cos t)^3\mathrm{d}t=\frac{5}{6},$$

所以质心为 $\left(\pi,\dfrac{5}{6}\right)$.

+++

#### 综合解答 (12) 设 $V:0\leqslant z\leqslant\sqrt{R^2-x^2-y^2}$，求 $I=\iiint_{V}(3x^2+5y^2+7z^2)\mathrm{d}V$.
***
考虑到被积函数 $3x^2+5y^2+7z^2$ 关于 $z$ 是**偶函数**，对 $V$ 补上下半球体得 $V_1:x^2+y^2+z^2\leqslant R^2$，则 $V_1$ 关于直线 $x=y=z$ 对称（**轮换对称性**），故

$$\iiint_{V_1}x^2\mathrm{d}V=\iiint_{V_1}y^2\mathrm{d}V=\iiint_{V_1}z^2\mathrm{d}V=\frac{1}{3}\iiint_{V_1}(x^2+y^2+z^2)\mathrm{d}V,$$

于是
$$I=\iiint_{V}(3x^2+5y^2+7z^2)\mathrm{d}V=\frac{1}{2}\iiint_{V_1}(3x^2+5y^2+7z^2)\mathrm{d}V$$

$$=\frac{1}{2}\left(3\iiint_{V_1}x^2\mathrm{d}V+5\iiint_{V_1}y^2\mathrm{d}V+7\iiint_{V_1}z^2\mathrm{d}V\right)=\frac{15}{2}\iiint_{V_1}x^2\mathrm{d}V$$

$$=\frac{15}{2}\cdot\frac{1}{3}\iiint_{V_1}(x^2+y^2+z^2)\mathrm{d}V=\frac{5}{2}\iiint_{V_1}(x^2+y^2+z^2)\mathrm{d}V$$

用**球坐标**，
$$=\frac{5}{2}\int_0^{2\pi}\mathrm{d}\theta\int_0^{\pi}\mathrm{d}\varphi\int_0^{R}r^4\sin\varphi\mathrm{d}r=\frac{5}{2}\cdot2\pi\int_0^{\pi}\sin\varphi\mathrm{d}\varphi\int_0^R r^4\mathrm{d}r=2\pi R^5.$$

+++

#### 综合解答 (13) 设 $F(t)=\iiint_{V}\left[z^2+f(x^2+y^2)\right]\mathrm{d}V$，$f(u)$ 连续，其中 $V:0\leqslant z\leqslant h,x^2+y^2\leqslant t^2$.

（Ⅰ）求 $\dfrac{\mathrm{d}F}{\mathrm{d}t}$；\
（Ⅱ）求 $\lim\limits_{t\to0}\dfrac{1}{t^2}F(t)$.
***
（Ⅰ）依题意，这是含参数 $t$ 的三重积分，积分区域 $V$ 是由圆柱面 $x^2+y^2=t^2$，平面 $z=0,z=h$ 所围，采用**柱面坐标**，则 $V:0\leqslant\theta\leqslant2\pi,0\leqslant r\leqslant|t|,0\leqslant z\leqslant h$.

$$F(t)=\iiint_{V}\left[z^2+f(x^2+y^2)\right]\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^{|t|}r\mathrm{d}r\int_0^{h}\left[z^2+f(r^2)\right]\mathrm{d}z$$

$$=2\pi\int_0^{|t|}\left[\frac{h^3}{3}+hf(r^2)\right]r\mathrm{d}r=\frac{\pi}{3}h^3t^2+2\pi h\int_0^{|t|}f(r^2)r\mathrm{d}r$$

令 $r^2=u$，$=\dfrac{\pi}{3}h^3t^2+\pi h\displaystyle\int_0^{t^2}f(u)\mathrm{d}u$.

当 $t>0$ 时，$\dfrac{\mathrm{d}F}{\mathrm{d}t}=\dfrac{2}{3}\pi h^3t+2\pi htf(t^2)$；\
当 $t<0$ 时，$\dfrac{\mathrm{d}F}{\mathrm{d}t}=\dfrac{2}{3}\pi h^3t+2\pi htf(t^2)$；\
当 $t=0$ 时，由导数定义有 $F_+'(0)=F_-'(0)=0$，故 $F'(0)=0$.

所以对一切 $t$ 有 $\dfrac{\mathrm{d}F}{\mathrm{d}t}=\dfrac{2}{3}\pi h^3t+2\pi htf(t^2)$.

（Ⅱ）利用**洛必达法则**，有

$$\lim_{t\to0}\frac{F(t)}{t^2}=\lim_{t\to0}\frac{\frac{2}{3}\pi h^3t+2\pi htf(t^2)}{2t}=\frac{\pi}{3}h^3+\pi hf(0).$$

+++

#### 综合解答 (14) 设 $V$ 是由平面 $z=0,z=1$ 及圆柱面 $x^2+y^2=2$ 所围成的图形，计算

$$I=\iiint_{V}\left|z-\sqrt{x^2+y^2}\right|\mathrm{d}x\mathrm{d}y\mathrm{d}z.$$
***
**去绝对值**。$z=\sqrt{x^2+y^2}$ 将 $V$ 分成两部分，利用**柱面坐标**，得

$$V_1:\begin{cases}z^2\geqslant x^2+y^2,\\ z=0,\\ z=1,\end{cases}\qquad V_2:\begin{cases}z^2\leqslant x^2+y^2\leqslant2,\\ z=0,\\ z=1,\end{cases}$$

即 $V_1:0\leqslant\theta\leqslant2\pi,\ 0\leqslant r\leqslant1,\ r\leqslant z\leqslant1$；

$V_2:0\leqslant\theta\leqslant2\pi,\ 0\leqslant r\leqslant1,\ 0\leqslant z\leqslant r$ 及 $0\leqslant\theta\leqslant2\pi,\ 1\leqslant r\leqslant\sqrt{2},\ 0\leqslant z\leqslant1$，

故
$$I=\iiint_{V_1}(z-\sqrt{x^2+y^2})\mathrm{d}x\mathrm{d}y\mathrm{d}z+\iiint_{V_2}(\sqrt{x^2+y^2}-z)\mathrm{d}x\mathrm{d}y\mathrm{d}z$$

$$=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\mathrm{d}r\int_r^1(z-r)\mathrm{d}z+\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\mathrm{d}r\int_0^r(r-z)\mathrm{d}z+\int_0^{2\pi}\mathrm{d}\theta\int_1^{\sqrt{2}}r\mathrm{d}r\int_0^1(r-z)\mathrm{d}z$$

$$=\frac{1}{6}(8\sqrt{2}-5)\pi.$$

+++

#### 综合解答 (15) 某均匀物体由上、下两部分组成，上部分是半径为 $a$ 的半球体，下部分是底面半径为 $a$、高为 $3$ 的直圆锥体，且半球体的底面圆与圆锥的底面重合，问当 $a$ 为何值时，此物体的质心恰好在球心位置？
***
建立直角坐标系，将球心置于原点，球底面放在 $xOy$ 上，则球面方程为 $z=\sqrt{a^2-x^2-y^2}$.

又 $AB$ 直线方程为 $\begin{cases}\frac{y}{a}+\frac{z}{-3}=1,\\ x=0,\end{cases}$ 即 $\begin{cases}z=\frac{3}{a}y-3,\\ x=0,\end{cases}$ 绕 $z$ 轴旋转得到 $z=\dfrac{3}{a}\sqrt{x^2+y^2}-3$，即为**圆锥面方程**。

由已知条件，质心坐标 $(\overline{x},\overline{y},\overline{z})=(0,0,0)$，故

$$\overline{z}=\frac{\iiint_{V}z\rho\mathrm{d}V}{\iiint_{V}\rho\mathrm{d}V}=\frac{\iiint_{V}z\mathrm{d}V}{\iiint_{V}\mathrm{d}V}=0\quad(\text{常数 }\rho\text{ 为物体的密度}),$$

从而有 $\iiint_{V}z\mathrm{d}V=0$.

考虑到上部分为半球体，下部分为圆锥体，故分别采用**球坐标**和**柱坐标**计算，

$$\iiint_{V}z\mathrm{d}V=\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{2}}\mathrm{d}\varphi\int_0^{a}r\cos\varphi\cdot r^2\sin\varphi\mathrm{d}r+\int_0^{2\pi}\mathrm{d}\theta\int_0^{a}r\mathrm{d}r\int_{\frac{3}{a}r-3}^{0}z\mathrm{d}z$$

$$=2\pi\cdot\frac{1}{2}\cdot\frac{a^4}{4}-\pi\left(\frac{9}{4a^2}\cdot a^4-6a^2+\frac{9}{2}a^2\right)=\frac{\pi}{4}a^2(a^2-3)=0,$$

解得 $a=\sqrt{3}$.

+++

#### 综合解答 (16) 设 $f(x)$ 在 $[0,1]$ 上是连续正值函数，且 $f(x)$ 单调减少，$D:0\leqslant x\leqslant1,0\leqslant y\leqslant1$，证明：

$$\iint_{D}xf(x)f(y)\left[f(x)-f(y)\right]\mathrm{d}x\mathrm{d}y\leqslant0.$$
***
**证** 积分区域 $D$ 关于直线 $y=x$ 对称，由**轮换对称性**，得

$$\iint_{D}xf(x)f(y)\left[f(x)-f(y)\right]\mathrm{d}x\mathrm{d}y=\iint_{D}yf(y)f(x)\left[f(y)-f(x)\right]\mathrm{d}x\mathrm{d}y$$

$$=\frac{1}{2}\iint_{D}\Big\{xf(x)f(y)\left[f(x)-f(y)\right]+yf(y)f(x)\left[f(y)-f(x)\right]\Big\}\mathrm{d}x\mathrm{d}y$$

$$=\frac{1}{2}\iint_{D}f(x)f(y)(x-y)\left[f(x)-f(y)\right]\mathrm{d}x\mathrm{d}y,$$

由已知，$f(x)f(y)>0$，考虑到 $f(x)$ 单调减少，故 $(x-y)[f(x)-f(y)]<0$，于是

$$\iint_{D}xf(x)f(y)\left[f(x)-f(y)\right]\mathrm{d}x\mathrm{d}y\leqslant0.$$

+++

#### 综合解答 (17) 设 $f(u)$ 在 $[-1,1]$ 上连续，$D:|x|+|y|\leqslant1$，证明：

$$\iint_{D}f(x+y)\mathrm{d}x\mathrm{d}y=\int_{-1}^{1}f(u)\mathrm{d}u.$$
***
**证** 积分区域为以 $(\pm1,0),(0,\pm1)$ 为顶点的正方形，故

$$\iint_{D}f(x+y)\mathrm{d}x\mathrm{d}y=\int_{-1}^{0}\mathrm{d}x\int_{-1-x}^{x+1}f(x+y)\mathrm{d}y+\int_0^1\mathrm{d}x\int_{x-1}^{1-x}f(x+y)\mathrm{d}y$$

令 $x+y=u$，
$$=\int_{-1}^{0}\mathrm{d}x\int_{-1}^{1+2x}f(u)\mathrm{d}u+\int_0^1\mathrm{d}x\int_{2x-1}^{1}f(u)\mathrm{d}u.$$

在 $xOu$ 坐标下（区域由 $u=2x+1$ 与 $u=2x-1$ 及 $u=\pm1$ 围成），**交换积分顺序**，则

$$\iint_{D}f(x+y)\mathrm{d}x\mathrm{d}y=\int_{-1}^{1}\mathrm{d}u\int_{\frac{u-1}{2}}^{\frac{u+1}{2}}f(u)\mathrm{d}x=\int_{-1}^{1}f(u)\mathrm{d}u.$$

+++

#### 综合解答 (18) 设 $D:x^2+y^2\leqslant2tx,y\geqslant0\ (t>0)$，$f(u)$ 在 $u=0$ 处可导，且 $f(0)=0$，求

$$\lim_{t\to0^+}\frac{1}{t^4}\iint_{D}f(\sqrt{x^2+y^2})y\mathrm{d}x\mathrm{d}y.$$
***
用**极坐标**，有

$$\iint_{D}f(\sqrt{x^2+y^2})y\mathrm{d}x\mathrm{d}y=\int_0^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{2t\cos\theta}f(r)\cdot r\sin\theta\cdot r\mathrm{d}r=\int_0^{\frac{\pi}{2}}\sin\theta\mathrm{d}\theta\int_0^{2t\cos\theta}f(r)r^2\mathrm{d}r.$$

**交换积分顺序**（可视在直角坐标 $\theta Or$ 下处理），则

$$\int_0^{\frac{\pi}{2}}\sin\theta\mathrm{d}\theta\int_0^{2t\cos\theta}f(r)r^2\mathrm{d}r=\int_0^{2t}r^2f(r)\mathrm{d}r\int_0^{\arccos\frac{r}{2t}}\sin\theta\mathrm{d}\theta$$

$$=\int_0^{2t}r^2f(r)(-\cos\theta)\Big|_0^{\arccos\frac{r}{2t}}\mathrm{d}r=\int_0^{2t}r^2f(r)\left(1-\frac{r}{2t}\right)\mathrm{d}r,$$

故
$$\lim_{t\to0^+}\frac{1}{t^4}\iint_{D}f(\sqrt{x^2+y^2})y\mathrm{d}x\mathrm{d}y=\lim_{t\to0^+}\frac{t\int_0^{2t}r^2f(r)\mathrm{d}r-\frac{1}{2}\int_0^{2t}r^3f(r)\mathrm{d}r}{t^5}$$

$$=\lim_{t\to0^+}\frac{\int_0^{2t}r^2f(r)\mathrm{d}r}{5t^4}=\lim_{t\to0^+}\frac{2(2t)^2f(2t)}{20t^3}=\lim_{t\to0^+}\frac{4}{5}\cdot\frac{f(2t)-f(0)}{2t}=\frac{4}{5}f'(0).$$

**【注】** ① 此题考虑极坐标下交换积分顺序，主要是由于 $\int_0^{\frac{\pi}{2}}\sin\theta\mathrm{d}\theta\int_0^{2t\cos\theta}f(r)r^2\mathrm{d}r$ 中对 $r$ 积分的结果会有 $\theta$，故不能先计算 $\int_0^{\frac{\pi}{2}}\sin\theta\mathrm{d}\theta$，即不能将其化为一元积分。
② 极坐标下交换积分顺序，可视 $\theta$ 为 $x$ 轴，$r$ 为 $y$ 轴，在直角坐标 $\theta Or$ 中画出积分区域，按直角坐标确定其积分限。

+++

#### 综合解答 (19) 设 $f(x)$ 在 $[a,b]$ 上非负可导，且单调增加，$(\overline{x},\overline{y})$ 为 $D=\{(x,y)\mid a\leqslant x\leqslant b,0\leqslant y\leqslant f(x)\}$ 的形心，证明：$\overline{x}\geqslant\dfrac{1}{2}(a+b)$.
***
**证** 依题意，只需证明

$$\overline{x}=\frac{\iint_{D}x\rho\mathrm{d}\sigma}{\iint_{D}\rho\mathrm{d}\sigma}=\frac{\int_a^b x\mathrm{d}x\int_0^{f(x)}\mathrm{d}y}{\int_a^b\mathrm{d}x\int_0^{f(x)}\mathrm{d}y}=\frac{\int_a^b xf(x)\mathrm{d}x}{\int_a^b f(x)\mathrm{d}x}\geqslant\frac{1}{2}(a+b)\quad(\rho\text{ 为常数}),$$

即证明 $\displaystyle\int_a^b xf(x)\mathrm{d}x-\frac{1}{2}(a+b)\int_a^b f(x)\mathrm{d}x\geqslant0$.

令 $F(t)=\displaystyle\int_a^t xf(x)\mathrm{d}x-\frac{1}{2}(a+t)\int_a^t f(x)\mathrm{d}x,\ t\in[a,b]$，则

$$F'(t)=tf(t)-\frac{1}{2}(a+t)f(t)-\frac{1}{2}\int_a^t f(x)\mathrm{d}x,$$

$$F''(t)=\frac{1}{2}(t-a)f'(t)\geqslant0,$$

故 $F'(t)$ 单调增加，又 $F'(a)=0$，所以 $F'(t)\geqslant F'(a)=0$，即 $F(t)$ 单调增加。

又 $F(a)=0$，故 $F(t)\geqslant F(a)=0$，即 $\overline{x}\geqslant\dfrac{1}{2}(a+b)$.

+++

#### 拓展解答 (1) 设 $D$ 由 $x$ 轴，曲线 $y=f(x)\ (f(x)\geqslant0)$，$x=0$，$x=a\ (a>0)$ 围成，平面图形 $D$ 的质心（形心）的横坐标为 $\overline{x}=\dfrac{2}{3}a$.

（Ⅰ）记 $F(x)=\displaystyle\int_0^x f(t)\mathrm{d}t$，证明：$F'(x)=\dfrac{2F(x)}{x}$；\
（Ⅱ）求 $f(x)$.
***
（Ⅰ）由形心公式，

$$\overline{x}=\frac{\iint_{D}x\mathrm{d}x\mathrm{d}y}{\iint_{D}\mathrm{d}x\mathrm{d}y}=\frac{\int_0^a x\mathrm{d}x\int_0^{f(x)}\mathrm{d}y}{\int_0^a\mathrm{d}x\int_0^{f(x)}\mathrm{d}y}=\frac{\int_0^a xf(x)\mathrm{d}x}{\int_0^a f(x)\mathrm{d}x}=\frac{2}{3}a,$$

由 $F(x)=\displaystyle\int_0^x f(t)\mathrm{d}t$，得 $\dfrac{2}{3}x\cdot F(x)=\displaystyle\int_0^x tf(t)\mathrm{d}t$，等式两边同时对 $x$ 求导，得

$$\frac{2}{3}x\cdot F'(x)+\frac{2}{3}F(x)=xf(x)=xF'(x),$$

即 $F'(x)=\dfrac{2F(x)}{x}$.

（Ⅱ）由（Ⅰ）知 $F'(x)=\dfrac{2F(x)}{x}$，即 $F'(x)-\dfrac{2}{x}F(x)=0$，解此**一阶线性齐次微分方程**，得通解为

$$F(x)=C_1\cdot\mathrm{e}^{-\int\left(-\frac{2}{x}\right)\mathrm{d}x}=C_1x^2\quad(C_1\text{ 为任意常数}),$$

故 $f(x)=F'(x)=2C_1x=Cx$（$C$ 为任意常数）。

+++

#### 拓展解答 (2) 设 $D$ 是由下述曲线（$0\leqslant t\leqslant2\pi$）与 $y$ 轴所围平面区域，计算 $I=\iint_{D}(2x+y)\mathrm{d}x\mathrm{d}y$.

$$\begin{cases}x=1-\cos t,\\ y=t-\sin t.\end{cases}$$
***
在直角坐标下，$D=\{(x,y)\mid 0\leqslant y\leqslant2\pi,\ 0\leqslant x\leqslant x(y)\}$，这里 $x=x(y)$ 由参数方程确定。

$$I=\iint_{D}(2x+y)\mathrm{d}x\mathrm{d}y=\iint_{D}2x\mathrm{d}x\mathrm{d}y+\iint_{D}y\mathrm{d}x\mathrm{d}y.$$

又
$$\iint_{D}2x\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}y\int_0^{x(y)}2x\mathrm{d}x=\int_0^{2\pi}x^2(y)\mathrm{d}y=\int_0^{2\pi}\left[x(t)\right]^2\cdot y'(t)\mathrm{d}t$$

$$=\int_0^{2\pi}(1-\cos t)^2\cdot(1-\cos t)\mathrm{d}t=\int_0^{2\pi}(1-\cos t)^3\mathrm{d}t=\int_0^{2\pi}\left(2\sin^2\frac{t}{2}\right)^3\mathrm{d}t$$

$$=8\int_0^{2\pi}\sin^6\frac{t}{2}\mathrm{d}t\xlongequal{\frac{t}{2}=u}16\int_0^{\pi}\sin^6u\mathrm{d}u=16\cdot2\int_0^{\frac{\pi}{2}}\sin^6u\mathrm{d}u=32\times\frac{5}{6}\times\frac{3}{4}\times\frac{1}{2}\times\frac{\pi}{2}=5\pi,$$

$$\iint_{D}y\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}y\mathrm{d}y\int_0^{x(y)}\mathrm{d}x=\int_0^{2\pi}y\cdot x(y)\mathrm{d}y=\int_0^{2\pi}y(t)\cdot x(t)\cdot y'(t)\mathrm{d}t$$

$$=\int_0^{2\pi}(t-\sin t)(1-\cos t)^2\mathrm{d}t\xlongequal{t=u+\pi}\int_{-\pi}^{\pi}(u+\pi+\sin u)(1+\cos u)^2\mathrm{d}u$$

$$=\int_{-\pi}^{\pi}(u+\sin u)(1+\cos u)^2\mathrm{d}u+\pi\int_{-\pi}^{\pi}(1+\cos u)^2\mathrm{d}u=0+\pi\int_{-\pi}^{\pi}(1+\cos u)^2\mathrm{d}u$$

（利用奇函数）
$$=2\pi\int_0^{\pi}(1+\cos u)^2\mathrm{d}u=8\pi\int_0^{\pi}\cos^4\frac{u}{2}\mathrm{d}u\xlongequal{u=2s}16\pi\int_0^{\frac{\pi}{2}}\cos^4s\mathrm{d}s=16\pi\times\frac{3}{4}\times\frac{1}{2}\times\frac{\pi}{2}=3\pi^2,$$

故 $I=5\pi+3\pi^2$.

**【注】** 由于 $D$ 关于直线 $y=\pi$ 对称，故区域 $D$ 的形心位于 $y=\pi$ 上，即形心的纵坐标 $\overline{y}=\pi$，由形心公式 $\overline{y}=\dfrac{\iint_{D}y\mathrm{d}x\mathrm{d}y}{\iint_{D}\mathrm{d}x\mathrm{d}y}$ 也可直接得 $\iint_{D}y\mathrm{d}x\mathrm{d}y=\pi\iint_{D}\mathrm{d}x\mathrm{d}y=3\pi^2$.
