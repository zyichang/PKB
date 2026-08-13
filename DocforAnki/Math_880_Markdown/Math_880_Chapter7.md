---
quizify:
  format: 1
  deck: Math_880::Chapter_7
  tags: [Math, 880题, 数一, 第七章, 微分方程]
---

+++

#### 基础选择 (1) 下列选项中（$C$ 为任意常数），是微分方程 $\dfrac{\mathrm{d}y}{\mathrm{d}x}+\dfrac{x}{y}=0$ 的通解的是（　）。

;;;
A. $x^2+y^2=C^2$
B. $x^2-y^2=C^2$
C. $x^2+y^2=C$
D. $x^2-y^2=C$
;;;A
***
**A.**

**解** $\dfrac{\mathrm{d}y}{\mathrm{d}x}+\dfrac{x}{y}=0$ 为可分离变量方程，故 $y\mathrm{d}y+x\mathrm{d}x=0$，积分得 $x^2+y^2=C_1$，$C_1\geqslant 0$，即 $x^2+y^2=C^2$，故 A 正确.

+++

#### 基础选择 (2) 设 $y'+P(x)y=0$ 的一个特解为 $y=\cos 2x$，则该方程满足 $y(0)=2$ 的特解为（　）。

;;;
A. $2\cos x$
B. $2\cos 2x$
C. $\cos 2x$
D. $\cos 2x+1$
;;;B
***
**B.**

**解** 将 $y=\cos 2x$ 代入 $y'+P(x)y=0$，解得 $P(x)=2\tan 2x$，故
$$y'+(2\tan 2x)y=0,$$
解此一阶线性齐次微分方程，得 $y=C\mathrm{e}^{-\int P(x)\mathrm{d}x}=C\mathrm{e}^{-\int 2\tan 2x\,\mathrm{d}x}=C\cos 2x$.

由 $y(0)=2$，得 $C=2$，故 $y=2\cos 2x$，B 正确.

+++

#### 基础选择 (3) 微分方程 $y''+2y'-3y=\mathrm{e}^{-x}+x$ 的一个特解形式为（　）。

;;;
A. $a\mathrm{e}^{-x}+bx+c$
B. $ax\mathrm{e}^{-x}+x(bx+c)$
C. $ax\mathrm{e}^{-x}+bx+c$
D. $a\mathrm{e}^{x}+x(bx+c)$
;;;A
***
**A.**

**解** $y''+2y'-3y=\mathrm{e}^{-x}+x$ 的特解为两个微分方程 $y''+2y'-3y=\mathrm{e}^{-x}$ 与 $y''+2y'-3y=x\cdot\mathrm{e}^{0\cdot x}$ 的两个特解之和.

特征方程为 $r^2+2r-3=0$，得 $r_1=1$，$r_2=-3$，$\lambda=-1$ 与 $\lambda=0$ 均不是特征根，故 $y''+2y'-3y=\mathrm{e}^{-x}$ 有形如 $a\mathrm{e}^{-x}$ 的特解，$y''+2y'-3y=x$ 有形如 $bx+c$ 的特解，所以原方程的特解形式为 $a\mathrm{e}^{-x}+bx+c$，A 正确.

+++

#### 基础选择 (4) 设 $y_1(x),y_2(x)$ 是 $y'+P(x)y=0$ 的两个不同特解，其中 $P(x)$ 在 $(-\infty,+\infty)$ 内连续，且 $P(x)$ 不恒为 $0$，则下列结论中**错误**的是（　）。

;;;
A. $y_1(x)-y_2(x)=$ 常数
B. $C[y_1(x)-y_2(x)]$ 是方程的通解
C. $y_1(x)-y_2(x)$ 在任一点不为 $0$
D. $\dfrac{y_2(x)}{y_1(x)}\equiv$ 常数（$y_1(x)\neq 0$）
;;;A
***
**A.**

**解** 依题意，$y_1(x)-y_2(x)$ 是 $y'+P(x)y=0$ 的解.

当 $P(x)$ 不恒为 $0$ 时，非零常数不可能是 $y'+P(x)y=0$ 的解，故选 A.

D 选项正确，因为 $y'+P(x)y=0$ 的通解为 $y=C\mathrm{e}^{-\int P(x)\mathrm{d}x}$，所以任意两个解相差一个常数因子.

C 选项正确，因 $y'+P(x)y=0$ 两个不同的解不能满足相同的初始条件.

事实上，假设存在 $x_0$，使得 $y_1(x_0)=y_2(x_0)$，令 $y_0=y_1(x)-y_2(x)$，则 $y_0(x)$ 是该方程的解，且满足初始条件 $y_0(x_0)=0$，根据微分方程解的存在唯一性定理，知 $y_0(x)$ 恒为零，故 $y_1(x)=y_2(x)$，与已知条件矛盾.

+++

#### 基础选择 (5) 设 $y_1(x),y_2(x),y_3(x)$ 是微分方程 $y''+p(x)y'+q(x)y=f(x)$ 的三个线性无关的解，$f(x)\neq 0$，则该方程的通解为（　）。

;;;
A. $C_1y_1(x)+C_2y_2(x)+y_3(x)$
B. $C_1y_1(x)+(1-2C_1)y_2(x)+C_1y_3(x)$
C. $(C_1-C_2)y_1(x)+C_2y_2(x)+y_3(x)$
D. $C_1y_1(x)+C_2y_2(x)+C_3y_3(x)$（$C_1+C_2+C_3=1$）
;;;D
***
**D.**

**解** 由线性微分方程解的性质和结构，知该方程的通解为
$$C_1[y_1(x)-y_3(x)]+C_2[y_2(x)-y_3(x)]+y_3(x),$$
即
$$C_1y_1(x)+C_2y_2(x)+(1-C_1-C_2)y_3(x).$$
令 $C_3=1-C_1-C_2$，则 $C_1+C_2+C_3=1$，故 D 正确.

+++

#### 基础填空 (1) 微分方程 $(y-x\sin x)\mathrm{d}x+x\mathrm{d}y=0$ 的通解为________.
***
$y=\dfrac{1}{x}(\sin x-x\cos x+C)$（$C$ 为任意常数）.

**解** 原方程变形为 $\dfrac{\mathrm{d}y}{\mathrm{d}x}+\dfrac{1}{x}y=\sin x$，为一阶线性微分方程，故通解为
$$y=\mathrm{e}^{-\int P(x)\mathrm{d}x}\left[\int Q(x)\mathrm{e}^{\int P(x)\mathrm{d}x}\mathrm{d}x+C\right]=\mathrm{e}^{-\int\frac{1}{x}\mathrm{d}x}\left(\int \sin x\cdot\mathrm{e}^{\int\frac{1}{x}\mathrm{d}x}\mathrm{d}x+C\right)$$
$$=\mathrm{e}^{-\ln|x|}\left(\int \mathrm{e}^{\ln|x|}\sin x\,\mathrm{d}x+C\right)=\frac{1}{x}\left(\int x\sin x\,\mathrm{d}x+C\right)=\frac{1}{x}(\sin x-x\cos x+C),$$
其中 $C$ 为任意常数.

【注】① 若令 $P=y-x\sin x$，$Q=x$，则 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}=1$，所以该方程为全微分方程，故通解为 $\displaystyle\int_0^x P(x,0)\mathrm{d}x+\int_0^y Q(x,y)\mathrm{d}y=C$，即
$$\int_0^x (0-x\sin x)\mathrm{d}x+\int_0^y x\,\mathrm{d}y=C,$$
故 $x\cos x-\sin x+xy=C$ 为通解.

② $P(x,y)\mathrm{d}x+Q(x,y)\mathrm{d}y=0$，当 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$ 时，该方程为全微分方程，有通解公式 $\displaystyle\int_{x_0}^x P(x,y_0)\mathrm{d}x+\int_{y_0}^y Q(x,y)\mathrm{d}y=C$.

+++

#### 基础填空 (2) 微分方程 $(1+y^2)\mathrm{d}x+(2x-1)y\mathrm{d}y=0$ 的通解为________.
***
$(2x-1)(1+y^2)=C$（$C$ 为任意常数）.

**解** 原方程可化为可分离变量方程 $\dfrac{\mathrm{d}x}{2x-1}+\dfrac{y\mathrm{d}y}{1+y^2}=0$，积分可得
$$\frac{1}{2}\ln|2x-1|+\frac{1}{2}\ln(1+y^2)=\frac{1}{2}\ln C,$$
故通解为 $(2x-1)(1+y^2)=C$（$C$ 为任意常数）.

+++

#### 基础填空 (3) $y'=\dfrac{y}{x}+\tan\dfrac{y}{x}$ 满足 $y(1)=\dfrac{\pi}{6}$ 的特解为________.
***
$\sin\dfrac{y}{x}=\dfrac{1}{2}x$.

**解** 原方程为齐次微分方程，令 $u=\dfrac{y}{x}$，即 $y=ux$，则
$$\frac{\mathrm{d}y}{\mathrm{d}x}=u+x\cdot\frac{\mathrm{d}u}{\mathrm{d}x}=u+\tan u.$$
分离变量得 $\cot u\,\mathrm{d}u=\dfrac{\mathrm{d}x}{x}$，积分得 $\ln|\sin u|=\ln|x|+C_1$，故
$$\sin u=\pm\mathrm{e}^{C_1}\cdot x=Cx\quad(C\neq 0),$$
即 $\sin\dfrac{y}{x}=Cx$（$C\neq 0$）.

又 $y=0$ 也是原方程的解（$y=0$ 在分离变量过程中漏掉了），故上面常数也可以为零，则原方程的通解为 $\sin\dfrac{y}{x}=Cx$（$C$ 为任意常数）.

由 $y(1)=\dfrac{\pi}{6}$，得 $C=\dfrac{1}{2}$，故所求特解为 $\sin\dfrac{y}{x}=\dfrac{1}{2}x$.

+++

#### 基础填空 (4) 微分方程 $y'-6\dfrac{y}{x}+xy^2=0$（$y$ 不为常函数）的通解为________.
***
$\dfrac{1}{y}=\dfrac{C}{x^6}+\dfrac{x^2}{8}$（$C$ 为任意常数）.

**解** 方程变形为 $y'-\dfrac{6}{x}y=-xy^2$，为 $n=2$ 的伯努利方程.

令 $y^{-1}=z$，则 $\dfrac{\mathrm{d}z}{\mathrm{d}x}=-y^{-2}\dfrac{\mathrm{d}y}{\mathrm{d}x}$，代入原方程，得 $\dfrac{\mathrm{d}z}{\mathrm{d}x}+\dfrac{6}{x}z=x$，为一阶线性微分方程，解得 $z=\dfrac{C}{x^6}+\dfrac{x^2}{8}$，即 $\dfrac{1}{y}=\dfrac{C}{x^6}+\dfrac{x^2}{8}$ 为通解，其中 $C$ 为任意常数.

+++

#### 基础填空 (5) 微分方程 $\left(1+\mathrm{e}^{\frac{x}{y}}\right)\mathrm{d}x+\mathrm{e}^{\frac{x}{y}}\left(1-\dfrac{x}{y}\right)\mathrm{d}y=0$（$y>0$）的通解为________.
***
$x+y\mathrm{e}^{\frac{x}{y}}=C$（$C$ 为任意常数）.

**解** 令 $P=1+\mathrm{e}^{\frac{x}{y}}$，$Q=\mathrm{e}^{\frac{x}{y}}\left(1-\dfrac{x}{y}\right)$，则 $\dfrac{\partial P}{\partial y}=\mathrm{e}^{\frac{x}{y}}\cdot\left(-\dfrac{x}{y^2}\right)$，$\dfrac{\partial Q}{\partial x}=\mathrm{e}^{\frac{x}{y}}\left(-\dfrac{x}{y^2}\right)$，故 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，原方程为全微分方程. 通过凑微分法，求通解.

原方程变形为 $\mathrm{d}x+\mathrm{e}^{\frac{x}{y}}\mathrm{d}y+\mathrm{e}^{\frac{x}{y}}\left(\dfrac{y\mathrm{d}x-x\mathrm{d}y}{y}\right)=0$，即 $\mathrm{d}x+\mathrm{e}^{\frac{x}{y}}\mathrm{d}y+y\mathrm{e}^{\frac{x}{y}}\left(\dfrac{y\mathrm{d}x-x\mathrm{d}y}{y^2}\right)=0$，故 $\mathrm{d}x+\mathrm{e}^{\frac{x}{y}}\mathrm{d}y+y\mathrm{e}^{\frac{x}{y}}\mathrm{d}\left(\dfrac{x}{y}\right)=0$，也即 $\mathrm{d}x+\mathrm{e}^{\frac{x}{y}}\mathrm{d}y+y\mathrm{d}\left(\mathrm{e}^{\frac{x}{y}}\right)=0$，故 $\mathrm{d}\left(x+y\mathrm{e}^{\frac{x}{y}}\right)=0$，所以原方程的通解为 $x+y\mathrm{e}^{\frac{x}{y}}=C$（$C$ 为任意常数）.

【注】求全微分方程 $P(x,y)\mathrm{d}x+Q(x,y)\mathrm{d}y=0$ 共有三种方法：

① 利用公式，$u(x,y)=\displaystyle\int_{x_0}^x P(x,y_0)\mathrm{d}x+\int_{y_0}^y Q(x,y)\mathrm{d}y=C$.

② 凑微分.

③ 利用积分，由 $\mathrm{d}u(x,y)=P(x,y)\mathrm{d}x+Q(x,y)\mathrm{d}y$，知 $\dfrac{\partial u}{\partial x}=P(x,y)$，$\dfrac{\partial u}{\partial y}=Q(x,y)$，通过积分求出 $u(x,y)$，则通解为 $u(x,y)=C$.

如本题，由 $\dfrac{\partial u}{\partial x}=1+\mathrm{e}^{\frac{x}{y}}$，$\dfrac{\partial u}{\partial y}=\mathrm{e}^{\frac{x}{y}}\left(1-\dfrac{x}{y}\right)$，积分得
$$u=\int\left(1+\mathrm{e}^{\frac{x}{y}}\right)\mathrm{d}x+\varphi(y)=x+y\mathrm{e}^{\frac{x}{y}}+\varphi(y).$$
又
$$\frac{\partial u}{\partial y}=\mathrm{e}^{\frac{x}{y}}-\frac{x}{y}\mathrm{e}^{\frac{x}{y}}+\varphi'(y)=\mathrm{e}^{\frac{x}{y}}\left(1-\frac{x}{y}\right),$$
故 $\varphi'(y)=0$，所以 $\varphi(y)=C_1$，于是 $u(x,y)=x+y\mathrm{e}^{\frac{x}{y}}+C_1$，所以通解为
$$u(x,y)=x+y\mathrm{e}^{\frac{x}{y}}=C\ (C\text{ 为任意常数}).$$

+++

#### 基础填空 (6) 微分方程 $xy'=\sqrt{x^2+y^2}+y$ 的通解为________.
***
$y+\sqrt{x^2+y^2}=Cx^2$（$x>0$）和 $-y+\sqrt{x^2+y^2}=C$（$x<0$），其中 $C$ 为大于 $0$ 的常数.

**解** 方程变形为 $y'=\dfrac{\sqrt{x^2+y^2}}{x}+\dfrac{y}{x}$.

当 $x>0$ 时，方程化为 $y'=\sqrt{1+\left(\dfrac{y}{x}\right)^2}+\dfrac{y}{x}$；

当 $x<0$ 时，方程化为 $y'=-\sqrt{1+\left(\dfrac{y}{x}\right)^2}+\dfrac{y}{x}$.

令 $\dfrac{y}{x}=u$，则 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=u+x\dfrac{\mathrm{d}u}{\mathrm{d}x}$，方程变为 $\dfrac{\mathrm{d}u}{\sqrt{1+u^2}}=\pm\dfrac{\mathrm{d}x}{x}$ 两种情形，积分可得 $y+\sqrt{x^2+y^2}=Cx^2$（$x>0$）和 $-y+\sqrt{x^2+y^2}=C$（$x<0$），为原方程通解，其中 $C$ 为大于 $0$ 的常数.

+++

#### 基础填空 (7) 方程 $y''+2y'+y=x\mathrm{e}^x$ 满足 $y(0)=0$，$y'(0)=0$ 的特解为________.
***
$y=\dfrac{1}{4}\left[(x+1)\mathrm{e}^{-x}+(x-1)\mathrm{e}^{x}\right]$.

**解** 特征方程为 $r^2+2r+1=0$，$r_1=r_2=-1$，故对应齐次微分方程的通解为
$$y=C_1\mathrm{e}^{-x}+C_2x\mathrm{e}^{-x}.$$
由非齐次项 $x\mathrm{e}^x$，知 $\lambda=1$ 不是特征根，故令特解为 $y^*=(ax+b)\mathrm{e}^x$，将 $y^*$ 代入原方程，比较系数得 $a=\dfrac{1}{4}$，$b=-\dfrac{1}{4}$，故通解为 $y=C_1\mathrm{e}^{-x}+C_2x\mathrm{e}^{-x}+\dfrac{1}{4}(x-1)\mathrm{e}^x$.

由 $y(0)=0$，$y'(0)=0$，得 $C_1=\dfrac{1}{4}$，$C_2=\dfrac{1}{4}$，故所求特解为
$$y=\frac{1}{4}\left[(x+1)\mathrm{e}^{-x}+(x-1)\mathrm{e}^{x}\right].$$

+++

#### 基础填空 (8) 方程 $y''-3y'+2y=10\mathrm{e}^{-x}\sin x$ 满足当 $x\to+\infty$ 时，$y(x)\to 0$ 的特解为________.
***
$y=\mathrm{e}^{-x}(\sin x+\cos x)$.

**解** 特征方程 $r^2-3r+2=0$ 的特征根为 $r_1=1$，$r_2=2$，故对应的齐次微分方程的通解为 $y=C_1\mathrm{e}^x+C_2\mathrm{e}^{2x}$.

由非齐次项 $10\mathrm{e}^{-x}\sin x$，知 $-1\pm\mathrm{i}$ 不是特征根，故令原方程的特解为 $y^*=\mathrm{e}^{-x}(A\sin x+B\cos x)$，将其代入原方程，可解得 $A=B=1$，所以原方程的通解为
$$y=C_1\mathrm{e}^x+C_2\mathrm{e}^{2x}+\mathrm{e}^{-x}(\sin x+\cos x).$$
当 $x\to+\infty$ 时，$y(x)\to 0$，而 $\mathrm{e}^x\to+\infty$，$\mathrm{e}^{2x}\to+\infty$，因此有 $C_1=C_2=0$，故所求特解为 $y=\mathrm{e}^{-x}(\sin x+\cos x)$.

+++

#### 基础填空 (9) 方程 $(1-x^2)y''-xy'=0$ 满足 $y(0)=0$，$y'(0)=1$ 的特解为________.
***
$y=\arcsin x$（$-1<x<1$）.

**解** 已知方程为不显含 $y$ 的可降阶方程，令 $y'=p$，则 $y''=p'$，原方程变为 $(1-x^2)p'-xp=0$，即 $p'-\dfrac{x}{1-x^2}p=0$（$x\neq\pm 1$），为一阶线性微分方程，有 $p=C_1\mathrm{e}^{\int\frac{x}{1-x^2}\mathrm{d}x}$，即 $p=C_1\mathrm{e}^{-\frac{1}{2}\ln(1-x^2)}=\dfrac{C_1}{\sqrt{1-x^2}}$.

由 $p(0)=y'(0)=1$，得 $C_1=1$，故 $y=\displaystyle\int p(x)\mathrm{d}x=\int\frac{\mathrm{d}x}{\sqrt{1-x^2}}=\arcsin x+C_2$.

又由 $y(0)=0$，得 $C_2=0$，所以 $y=\arcsin x$（$-1<x<1$）.

【注】$\displaystyle\int\frac{x}{1-x^2}\mathrm{d}x=-\frac{1}{2}\ln|1-x^2|+C$，由已知 $y(0)=0$，$y'(0)=1$，意味着在 $(-1,1)$ 内求解，故 $\displaystyle\int\frac{x}{1-x^2}\mathrm{d}x=-\frac{1}{2}\ln(1-x^2)+C$.

+++

#### 基础填空 (10) 设二阶线性非齐次微分方程 $y''+p(x)y'+q(x)y=f(x)$ 有三个特解为 $x,\mathrm{e}^x,\mathrm{e}^{-x}$，则该方程的通解为________.
***
$y=C_1(\mathrm{e}^x-x)+C_2(\mathrm{e}^{-x}-x)+x$（$C_1,C_2$ 为任意常数）.

**解** 由线性微分方程解的性质及通解结构，知 $y_1=\mathrm{e}^x-x$，$y_2=\mathrm{e}^{-x}-x$ 是对应齐次微分方程的两个线性无关的解，故通解为 $y=C_1(\mathrm{e}^x-x)+C_2(\mathrm{e}^{-x}-x)+x$（$C_1,C_2$ 为任意常数）.

+++

#### 基础填空 (11) 设二阶常系数线性微分方程 $y''+ay'+by=c\mathrm{e}^x$ 有特解 $y^*=\mathrm{e}^{-x}(1+x\mathrm{e}^{2x})$，则该方程的通解为________.
***
$y=C_1\mathrm{e}^{-x}+C_2\mathrm{e}^{x}+x\mathrm{e}^{x}$（$C_1,C_2$ 为任意常数）.

**解** 由特解 $y^*=\mathrm{e}^{-x}(1+x\mathrm{e}^{2x})=\mathrm{e}^{-x}+x\mathrm{e}^{x}$，知该方程对应的齐次微分方程有特征根 $r_1=-1$，$r_2=1$，且 $x\mathrm{e}^x$ 是其特解，故该方程的通解为 $y=C_1\mathrm{e}^{-x}+C_2\mathrm{e}^{x}+x\mathrm{e}^{x}$（$C_1,C_2$ 为任意常数）.

+++

#### 基础解答 (1) 求 $x^2y''-y'^2=0$ 过点 $P(1,0)$，且在点 $P$ 与 $y=x-1$ 相切的积分曲线.
***
**解** 依题设，有 $y(1)=0$，$y'(1)=1$.

方程 $x^2y''-y'^2=0$ 不显含 $y$，令 $y'=p$，$y''=p'$，代入原方程，得 $x^2p'-p^2=0$，分离变量并积分，得
$$\frac{1}{p}=\frac{1}{x}+C_1.$$
由 $y'(1)=1$，得 $C_1=0$，故 $p=\dfrac{\mathrm{d}y}{\mathrm{d}x}=x$，积分得 $y=\dfrac{1}{2}x^2+C_2$.

又由 $y(1)=0$，得 $C_2=-\dfrac{1}{2}$，故所求积分曲线为 $y=\dfrac{1}{2}(x^2-1)$.

+++

#### 基础解答 (2) 求微分方程 $(x\cos y+\cos x)\dfrac{\mathrm{d}y}{\mathrm{d}x}-y\sin x+\sin y=0$ 的通解.
***
**解** 方程变形为 $(\sin y-y\sin x)\mathrm{d}x+(x\cos y+\cos x)\mathrm{d}y=0$. 记
$$P=\sin y-y\sin x,\quad Q=x\cos y+\cos x,$$
则有 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}=\cos y-\sin x$，故为全微分方程.

由
$$\frac{\partial u}{\partial x}=P(x,y)=\sin y-y\sin x,\quad \frac{\partial u}{\partial y}=Q(x,y)=x\cos y+\cos x,$$
积分得
$$u(x,y)=\int\frac{\partial u}{\partial x}\mathrm{d}x+\varphi(y)=\int(\sin y-y\sin x)\mathrm{d}x+\varphi(y)=x\sin y+y\cos x+\varphi(y).$$
由
$$\frac{\partial u}{\partial y}=x\cos y+\cos x+\varphi'(y)=x\cos y+\cos x,$$
得 $\varphi'(y)=0$，从而 $\varphi(y)=C_1$，所以 $u(x,y)=x\sin y+y\cos x+C_1$，故原方程的通解为 $x\sin y+y\cos x=C$，其中 $C$ 为任意常数.

+++

#### 基础解答 (3) 设 $f(x)$ 是连续函数，且 $f(x)=\cos x-\displaystyle\int_0^x (x-t)f(t)\mathrm{d}t$，求 $f(x)$.
***
**解** 已知等式变形为 $f(x)=\cos x-x\displaystyle\int_0^x f(t)\mathrm{d}t+\int_0^x tf(t)\mathrm{d}t$，两边同时对 $x$ 求导，得
$$f'(x)=-\sin x-\int_0^x f(t)\mathrm{d}t-xf(x)+xf(x)=-\sin x-\int_0^x f(t)\mathrm{d}t,\qquad ①$$
再对 $x$ 求导，得
$$f''(x)+f(x)=-\cos x.\qquad ②$$
对应齐次方程的特征方程为 $r^2+1=0$，得 $r=\pm\mathrm{i}$，故齐次方程的通解为
$$f(x)=C_1\cos x+C_2\sin x.$$
由非齐次项 $-\cos x$，知 $0\pm\mathrm{i}$ 是特征根，故令特解为 $f^*=x(A\cos x+B\sin x)$，将其代入 ② 式，得 $A=0$，$B=-\dfrac{1}{2}$，所以 ② 的通解为 $f(x)=C_1\cos x+C_2\sin x-\dfrac{1}{2}x\sin x$.

又由已知等式及 ① 式，知 $f(0)=1$，$f'(0)=0$，故得 $C_1=1$，$C_2=0$，所以
$$f(x)=\cos x-\frac{1}{2}x\sin x.$$

+++

#### 基础解答 (4) 设 $f(x)$ 可导，对任何实数 $x,y$ 满足 $f(x+y)=\mathrm{e}^x f(y)+\mathrm{e}^y f(x)$，且 $f'(0)=\mathrm{e}$，求 $f(x)$.
***
**解** 由已知条件 $f(0)=0$，由导数定义，有
$$f'(x)=\lim_{\Delta x\to 0}\frac{f(x+\Delta x)-f(x)}{\Delta x}=\lim_{\Delta x\to 0}\frac{\mathrm{e}^x f(\Delta x)+f(x)(\mathrm{e}^{\Delta x}-1)}{\Delta x}$$
$$=\lim_{\Delta x\to 0}\mathrm{e}^x\cdot\frac{f(\Delta x)-f(0)}{\Delta x}+\lim_{\Delta x\to 0}f(x)\cdot\frac{\mathrm{e}^{\Delta x}-1}{\Delta x}$$
$$=\mathrm{e}^x f'(0)+f(x)=\mathrm{e}^{x+1}+f(x),$$
即 $f'(x)-f(x)=\mathrm{e}^{x+1}$，为一阶线性微分方程，故 $f(x)=\mathrm{e}^{\int\mathrm{d}x}\left[\int \mathrm{e}^{x+1}\mathrm{e}^{-\int\mathrm{d}x}\mathrm{d}x+C\right]=x\mathrm{e}^{x+1}+C\mathrm{e}^x$.

又由 $f(0)=0$，得 $C=0$，所以 $f(x)=x\mathrm{e}^{x+1}$.

+++

#### 基础解答 (5) 求微分方程 $y''+\dfrac{1}{2}y'^2=2y$ 满足 $y(0)=y'(0)=2$ 的特解.
***
**解** 已知方程为不显含 $x$ 的可降阶的二阶方程.

令 $y'=p$，则 $y''=\dfrac{\mathrm{d}p}{\mathrm{d}y}\cdot\dfrac{\mathrm{d}y}{\mathrm{d}x}=p\dfrac{\mathrm{d}p}{\mathrm{d}y}$，代入原方程，得 $p\dfrac{\mathrm{d}p}{\mathrm{d}y}+\dfrac{1}{2}p^2=2y$，即 $\dfrac{\mathrm{d}(p^2)}{\mathrm{d}y}+p^2=4y$，是关于 $p^2$ 的一阶线性微分方程，其通解为
$$p^2=\mathrm{e}^{-\int\mathrm{d}y}\left(\int 4y\mathrm{e}^{\int\mathrm{d}y}\mathrm{d}y+C_1\right)=\mathrm{e}^{-y}\left(\int 4y\mathrm{e}^{y}\mathrm{d}y+C_1\right)$$
$$=\mathrm{e}^{-y}(4y\mathrm{e}^y-4\mathrm{e}^y+C_1)=4(y-1)+C_1\mathrm{e}^{-y}.$$
由 $y(0)=2$，$y'(0)=2$，得 $C_1=0$，故 $p^2=4(y-1)$，$p=\pm 2\sqrt{y-1}$，取 $p=2\sqrt{y-1}$（因 $y'(0)=2>0$），故 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=2\sqrt{y-1}$，分离变量，得 $\dfrac{\mathrm{d}y}{\sqrt{y-1}}=2\mathrm{d}x$，积分得
$$\sqrt{y-1}=x+C_2,$$
即 $y=(x+C_2)^2+1$，又由 $y'(0)=2$，得 $C_2=1$，所求特解为 $y=(x+1)^2+1$.

+++

#### 基础解答 (6) 求微分方程 $y'''-y'=0$ 的一条积分曲线，使此积分曲线在原点处有拐点，且以直线 $y=2x$ 为切线.
***
**解** 依题意，$y(0)=0$，$y'(0)=2$，$y''(0)=0$.

$y'''-y'=0$ 的特征方程为 $r^3-r=0$，得特征根为 $r_1=0$，$r_2=1$，$r_3=-1$，故微分方程的通解为 $y=C_1+C_2\mathrm{e}^x+C_3\mathrm{e}^{-x}$，故
$$y'=C_2\mathrm{e}^x-C_3\mathrm{e}^{-x},\quad y''=C_2\mathrm{e}^x+C_3\mathrm{e}^{-x}.$$
代入初始条件 $y(0)=0$，$y'(0)=2$，$y''(0)=0$，得
$$C_1+C_2+C_3=0,\quad C_2-C_3=2,\quad C_2+C_3=0,$$
解得 $C_1=0$，$C_2=1$，$C_3=-1$，故所求积分曲线为 $y=\mathrm{e}^x-\mathrm{e}^{-x}$.

+++

#### 基础解答 (7) 设 $f(u)$ 有二阶连续导数，$z=f(\sqrt{x^2+y^2})$ 满足 $\dfrac{\partial^2 z}{\partial x^2}+\dfrac{\partial^2 z}{\partial y^2}=x^2+y^2$，求 $z$ 的表达式.
***
**解** 令 $\sqrt{x^2+y^2}=u$，则
$$\frac{\partial z}{\partial x}=\frac{x}{u}f'(u),\quad \frac{\partial^2 z}{\partial x^2}=\frac{u-\dfrac{x^2}{u}}{u^2}f'(u)+\frac{x^2}{u^2}f''(u)=\frac{y^2}{u^3}f'(u)+\frac{x^2}{u^2}f''(u).$$
由 $z=f(\sqrt{x^2+y^2})$ 关于 $x,y$ 具有轮换对称性，知 $\dfrac{\partial^2 z}{\partial y^2}=\dfrac{x^2}{u^3}f'(u)+\dfrac{y^2}{u^2}f''(u)$，将其代入 $\dfrac{\partial^2 z}{\partial x^2}+\dfrac{\partial^2 z}{\partial y^2}=x^2+y^2$，得 $f''(u)+\dfrac{1}{u}f'(u)=u^2$，即 $uf''(u)+f'(u)=u^3$，$[uf'(u)]'=u^3$，积分得 $uf'(u)=\dfrac{1}{4}u^4+C_1$，故 $f'(u)=\dfrac{1}{4}u^3+\dfrac{C_1}{u}$，积分得 $f(u)=\dfrac{1}{16}u^4+C_1\ln u+C_2$，故
$$z=\frac{1}{16}(x^2+y^2)^2+C_1\ln\sqrt{x^2+y^2}+C_2\ (C_1,C_2\text{ 为任意常数}).$$

+++

#### 基础解答 (8) 利用变换 $u=\mathrm{e}^x$，求微分方程 $y''-(2\mathrm{e}^x+1)y'+\mathrm{e}^{2x}y=\mathrm{e}^{3x}$ 的通解.
***
**解** 由 $u=\mathrm{e}^x$，知 $x=\ln u$，则
$$\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{\mathrm{d}y}{\mathrm{d}u}\cdot\frac{\mathrm{d}u}{\mathrm{d}x}=u\frac{\mathrm{d}y}{\mathrm{d}u},$$
$$\frac{\mathrm{d}^2y}{\mathrm{d}x^2}=\frac{\mathrm{d}}{\mathrm{d}x}\left(u\frac{\mathrm{d}y}{\mathrm{d}u}\right)=\frac{\mathrm{d}}{\mathrm{d}u}\left(u\frac{\mathrm{d}y}{\mathrm{d}u}\right)\cdot\frac{\mathrm{d}u}{\mathrm{d}x}=u\frac{\mathrm{d}y}{\mathrm{d}u}+u^2\frac{\mathrm{d}^2y}{\mathrm{d}u^2},$$
将其代入原方程，得
$$\frac{\mathrm{d}^2y}{\mathrm{d}u^2}-2\frac{\mathrm{d}y}{\mathrm{d}u}+y=u,\qquad ①$$
其对应齐次微分方程的特征方程为 $r^2-2r+1=0$，得 $r_1=r_2=1$.

令特解 $y^*=au+b$，代入 ① 可解得 $y^*=u+2$，故方程 ① 的通解为 $y=C_1\mathrm{e}^u+C_2u\mathrm{e}^u+u+2$，将 $u=\mathrm{e}^x$ 代入得原微分方程的通解为 $y=(C_1+C_2\mathrm{e}^x)\mathrm{e}^{\mathrm{e}^x}+\mathrm{e}^x+2$（$C_1,C_2$ 为任意常数）.

+++

#### 基础解答 (9) 设 $L$ 是一条平面曲线，其上任意一点 $P(x,y)$（$x>0$）到原点的距离恒等于该点处的切线在 $y$ 轴上的截距，且 $L$ 过点 $\left(\dfrac{1}{2},0\right)$.

（Ⅰ）求曲线 $L$ 的方程；\
（Ⅱ）求 $L$ 位于第一象限部分的一条切线，使该切线与 $L$ 以及两坐标轴所围的面积最小.
***
**解** （Ⅰ）依题设，曲线 $L$ 过点 $P(x,y)$ 的切线为 $Y-y=y'(X-x)$，令 $X=0$，则切线在 $y$ 轴上的截距为 $y-xy'$.

由已知，$\sqrt{x^2+y^2}=y-xy'$，即 $y'=\dfrac{y-\sqrt{x^2+y^2}}{x}$.

由 $x>0$，$y'=\dfrac{y}{x}-\sqrt{1+\left(\dfrac{y}{x}\right)^2}$，为齐次微分方程. 令 $\dfrac{y}{x}=u$，则 $y'=u+xu'$，则 $u+xu'=u-\sqrt{1+u^2}$，为可分离变量的微分方程，$\dfrac{\mathrm{d}u}{\sqrt{1+u^2}}=-\dfrac{\mathrm{d}x}{x}$，积分并代回 $\dfrac{y}{x}=u$，得 $y+\sqrt{x^2+y^2}=C$. 又 $L$ 过 $\left(\dfrac{1}{2},0\right)$，得 $C=\dfrac{1}{2}$，于是曲线 $L$ 的方程为 $y+\sqrt{x^2+y^2}=\dfrac{1}{2}$，即 $y=\dfrac{1}{4}-x^2$.

（Ⅱ）在第一象限内，$y=\dfrac{1}{4}-x^2$ 在点 $P(x,y)$ 处的切线方程为 $Y-\left(\dfrac{1}{4}-x^2\right)=-2x(X-x)$，即 $Y=-2x\cdot X+x^2+\dfrac{1}{4}$（$0<x\leqslant\dfrac{1}{2}$），它与 $x$ 轴、$y$ 轴的交点分别为 $\left(\dfrac{x^2+\dfrac{1}{4}}{2x},\,0\right)$ 与 $\left(0,\,x^2+\dfrac{1}{4}\right)$，故所求面积为
$$A(x)=\frac{1}{2}\cdot\frac{\left(x^2+\dfrac{1}{4}\right)^2}{2x}-\int_0^{\frac{1}{2}}\left(\frac{1}{4}-x^2\right)\mathrm{d}x,$$
则 $A'(x)=\dfrac{1}{4x^2}\left(x^2+\dfrac{1}{4}\right)\left(3x^2-\dfrac{1}{4}\right)=0$，得 $x=\dfrac{\sqrt{3}}{6}$.

当 $0<x<\dfrac{\sqrt{3}}{6}$ 时，$A'(x)<0$；当 $x>\dfrac{\sqrt{3}}{6}$ 时，$A'(x)>0$，故 $x=\dfrac{\sqrt{3}}{6}$ 是 $A(x)$ 在 $\left(0,\dfrac{1}{2}\right]$ 上唯一的极小值点，也是最小值点，所求切线为 $Y=-2\cdot\dfrac{\sqrt{3}}{6}X+\dfrac{3}{36}+\dfrac{1}{4}$，即 $Y=-\dfrac{\sqrt{3}}{3}X+\dfrac{1}{3}$.

+++

#### 基础解答 (10) 设 $\overparen{OA}$ 是连接 $O(0,0)$ 和 $A(1,1)$ 的一段向上凸的曲线弧，$P(x,y)$ 为 $\overparen{OA}$ 上任一点，曲线弧 $\overparen{OP}$ 与有向线段 $\overrightarrow{OP}$ 所围图形的面积为 $x^2$，求曲线弧 $\overparen{OA}$ 的方程.
***
**解** 设曲线弧 $\overparen{OA}$ 的方程为 $y=y(x)$，则 $\overparen{OP}$ 与 $\overrightarrow{OP}$ 所围面积为
$$\int_0^x\left[y(t)-\frac{y}{x}t\right]\mathrm{d}t=\int_0^x y(t)\mathrm{d}t-\frac{1}{2}xy.$$
依题意，$\displaystyle\int_0^x y(t)\mathrm{d}t-\frac{1}{2}xy=x^2$（$x>0$），两边同时对 $x$ 求导，得 $y-\dfrac{1}{2}y-\dfrac{1}{2}xy'=2x$，即 $y'-\dfrac{1}{x}y=-4$，为一阶线性微分方程，其通解为 $y=x(\ln x^{-4}+C)=x(C-4\ln x)$.

又由已知，有 $y(1)=1$，可得 $C=1$，故所求方程为
$$y=\begin{cases}x-4x\ln x, & 0<x\leqslant 1,\\ 0, & x=0.\end{cases}$$

【注】① $y=x-4x\ln x$ 在 $x=0$ 处无定义，但由于当 $x\to 0^+$ 时，$x-4x\ln x\to 0$，故 $x=0$ 是函数的可去间断点，若令 $y(0)=0$，则积分曲线过原点.

② 依题设，曲线过 $O(0,0)$ 和 $A(1,1)$，若将 $y(0)=0$ 作为初始条件，则从通解中不能确定常数 $C$.

+++

#### 综合选择 (1) 下列方程中，以 $y=C_1\mathrm{e}^{x}+C_2\cos x+C_3\sin x$（$C_1,C_2,C_3$ 为任意常数）为通解的是（　）.

;;;
A. $y'''-y''+y'-y=0$
B. $y'''+y''+y'-y=0$
C. $y'''+y''-y'-y=0$
D. $y'''-y''-y'-y=0$
;;;A
***
由通解 $y=C_1\mathrm{e}^{x}+C_2\cos x+C_3\sin x$，知其特征根为 $r_1=1$，$r_2=\mathrm{i}$，$r_3=-\mathrm{i}$，故对应的特征方程为
$$(r-1)(r^2+1)=0,$$
即 $r^3-r^2+r-1=0$，故对应的微分方程为 $y'''-y''+y'-y=0$，**A 正确**.

+++

#### 综合选择 (2) 若二阶常系数线性齐次微分方程 $y''+py'+qy=0$ 的通解为 $y=C_1\mathrm{e}^{x}+C_2x\mathrm{e}^{x}$，则非齐次微分方程 $y''+py'+qy=x$ 满足 $y(0)=2$，$y'(0)=0$ 的特解为 $y=$（　）.

;;;
A. $x\mathrm{e}^{x}-x-2$
B. $x\mathrm{e}^{x}-x+2$
C. $-x\mathrm{e}^{x}+x+2$
D. $-x\mathrm{e}^{x}-x+2$
;;;C
***
由齐次微分方程通解为 $y=C_1\mathrm{e}^{x}+C_2x\mathrm{e}^{x}$，知对应特征方程的根为 $r_1=r_2=1$，其特征方程为 $(r-1)^2=0$，即 $r^2-2r+1=0$，故 $p=-2$，$q=1$，所以非齐次微分方程为
$$y''-2y'+y=x. \qquad ①$$

令特解 $y^{*}=ax+b$，代入上式，得 $-2a+ax+b=x$，解得 $a=1$，$b=2$，故 ① 的通解为
$$y=C_1\mathrm{e}^{x}+C_2x\mathrm{e}^{x}+x+2.$$

由 $y(0)=2$，$y'(0)=0$，得 $C_1=0$，$C_2=-1$，故 $y=-x\mathrm{e}^{x}+x+2$，**C 正确**.

+++

#### 综合选择 (3) 设 $C$ 为任意常数，则以 $y=\mathrm{e}^{Cx+x^{2}}$ 为通解的一阶微分方程为（　）.

;;;
A. $xy'-y\ln y=x^{2}y$
B. $xy'+y\ln y=xy^{2}$
C. $xy'-y\ln y^{2}=xy$
D. $xy'+y\ln y=xy$
;;;A
***
由 $y=\mathrm{e}^{Cx+x^{2}}$，有 $\ln y=x^{2}+Cx$，即 $\dfrac{\ln y}{x}-x=C$，两边同时对 $x$ 求导，得
$$\frac{\dfrac{x}{y}\cdot y'-\ln y}{x^{2}}-1=0,$$
化简得 $xy'-y\ln y=x^{2}y$，**A 正确**.

+++

#### 综合选择 (4) 设 $y_1,y_2$ 是一阶线性非齐次微分方程 $y'+P(x)y=Q(x)$ 的两个解，若常数 $\lambda,\mu$ 使得 $\lambda y_1+\mu y_2$ 是该方程的解，$\lambda y_1-\mu y_2$ 是对应的齐次微分方程的解，则（　）.

;;;
A. $\lambda=-\dfrac{1}{2}$，$\mu=-\dfrac{1}{2}$
B. $\lambda=\dfrac{1}{2}$，$\mu=\dfrac{1}{2}$
C. $\lambda=\dfrac{1}{3}$，$\mu=\dfrac{2}{3}$
D. $\lambda=\dfrac{2}{3}$，$\mu=\dfrac{2}{3}$
;;;B
***
由 $\lambda y_1+\mu y_2$ 是 $y'+P(x)y=Q(x)$ 的解，知
$$(\lambda y_1+\mu y_2)'+P(x)(\lambda y_1+\mu y_2)=Q(x),$$
即
$$\lambda[y_1'+P(x)y_1]+\mu[y_2'+P(x)y_2]=Q(x),$$
即 $(\lambda+\mu)Q(x)=Q(x)$（$Q(x)\neq0$），故 $\lambda+\mu=1$.

由 $\lambda y_1-\mu y_2$ 是 $y'+P(x)y=0$ 的解，知
$$(\lambda y_1-\mu y_2)'+P(x)(\lambda y_1-\mu y_2)=0,$$
即
$$\lambda[y_1'+P(x)y_1]-\mu[y_2'+P(x)y_2]=0,$$
即 $(\lambda-\mu)Q(x)=0$（$Q(x)\neq0$），故 $\lambda-\mu=0$，解得 $\lambda=\dfrac{1}{2}$，$\mu=\dfrac{1}{2}$，故 **B 正确**.

【注】设 $y_1,y_2$ 是 $y'+P(x)y=Q(x)$ 的解，则\
① $k_1y_1+k_2y_2$ 是非齐次微分方程 $y'+P(x)y=Q(x)$ 的解 $\Leftrightarrow k_1+k_2=1$；\
② $k_1y_1+k_2y_2$ 是对应齐次微分方程 $y'+P(x)y=0$ 的解 $\Leftrightarrow k_1+k_2=0$.\
对 $n$ 阶线性微分方程有类似结果.

+++

#### 综合填空 (1) 微分方程 $y'=\dfrac{y}{x+(y+1)^{2}}$（$y$ 不为常函数）的通解为________.
***
$x=y\left(y+2\ln y-\dfrac{1}{y}+C\right)$（$C$ 为任意常数）.

**解** 原方程不是可分离变量方程，不是线性微分方程，也不是齐次微分方程，需要变形为
$$\frac{\mathrm{d}x}{\mathrm{d}y}-\frac{1}{y}x=\frac{(y+1)^{2}}{y},$$
为一阶线性微分方程，通解为
$$x=\mathrm{e}^{-\int-\frac{1}{y}\mathrm{d}y}\left[\int\frac{(y+1)^{2}}{y}\cdot\mathrm{e}^{-\int\frac{1}{y}\mathrm{d}y}\mathrm{d}y+C\right]=y\left(y+2\ln|y|-\frac{1}{y}+C\right)$$
（$C$ 为任意常数）.

+++

#### 综合填空 (2) 微分方程 $y''-y=\sin x$ 满足 $y(0)=0$，$y'(0)=\dfrac{3}{2}$ 的特解为________.
***
$y=\mathrm{e}^{x}-\mathrm{e}^{-x}-\dfrac{1}{2}\sin x$.

**解** 特征方程为 $r^{2}-1=0$，$r=\pm1$. 又 $\sin x=\mathrm{e}^{0x}\cdot\sin x$，$0\pm\mathrm{i}$ 不是特征根，故令原方程的特解为 $y^{*}=a\sin x+b\cos x$，则 $(y^{*})'=a\cos x-b\sin x$，$(y^{*})''=-a\sin x-b\cos x$，代入原方程，得
$$-a\sin x-b\cos x-(a\sin x+b\cos x)=\sin x,$$
即 $-2a\sin x-2b\cos x=\sin x$，比较 $\sin x$ 与 $\cos x$ 两边系数，得 $-2a=1$，$-2b=0$，即 $a=-\dfrac{1}{2}$，$b=0$，所以原方程的通解为
$$y=C_1\mathrm{e}^{x}+C_2\mathrm{e}^{-x}-\frac{1}{2}\sin x.$$

由 $y(0)=0$，$y'(0)=\dfrac{3}{2}$，得 $C_1+C_2=0$，$C_1-C_2=2$，解得 $C_1=1$，$C_2=-1$，所以特解为 $y=\mathrm{e}^{x}-\mathrm{e}^{-x}-\dfrac{1}{2}\sin x$.

+++

#### 综合填空 (3) 微分方程 $y'=\dfrac{y^{2}-x}{2y(x+1)}$ 的通解为________.
***
$y^{2}=C(x+1)-(x+1)\ln|x+1|-1$（$C$ 为任意常数）.

**解** 原方程变形为 $2yy'-\dfrac{1}{1+x}y^{2}=-\dfrac{x}{1+x}$.

由 $2yy'=(y^{2})'$，令 $u=y^{2}$，则方程变为 $u'-\dfrac{1}{1+x}u=-\dfrac{x}{1+x}$，为一阶线性微分方程，其通解为
$$y^{2}=u=\mathrm{e}^{\int\frac{1}{1+x}\mathrm{d}x}\left[\int\left(-\frac{x}{1+x}\right)\cdot\mathrm{e}^{-\int\frac{1}{1+x}\mathrm{d}x}\mathrm{d}x+C\right]=(1+x)\left[-\int\frac{x}{(1+x)^{2}}\mathrm{d}x+C\right]$$
$$=C(x+1)-(x+1)\ln|x+1|-1\quad(C\ \text{为任意常数}).$$

+++

#### 综合填空 (4) 微分方程 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=\dfrac{y-x}{y+x}$ 满足 $y(1)=0$ 的特解为________.
***
$\dfrac{1}{2}\ln\left[\left(\dfrac{y}{x}\right)^{2}+1\right]+\arctan\dfrac{y}{x}+\ln x=0$.

**解** 已知方程变形为 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=\dfrac{\dfrac{y}{x}-1}{\dfrac{y}{x}+1}$，为一阶齐次微分方程.

令 $\dfrac{y}{x}=u$，则 $y=ux$，$\dfrac{\mathrm{d}y}{\mathrm{d}x}=x\dfrac{\mathrm{d}u}{\mathrm{d}x}+u$，故 $u+x\dfrac{\mathrm{d}u}{\mathrm{d}x}=\dfrac{u-1}{u+1}$，分离变量得
$$\frac{u+1}{u^{2}+1}\mathrm{d}u=-\frac{\mathrm{d}x}{x},$$
积分得
$$\frac{1}{2}\ln(u^{2}+1)+\arctan u=-\ln|x|+C.$$

由 $y(1)=0$，得 $C=0$，故所求特解为 $\dfrac{1}{2}\ln\left[\left(\dfrac{y}{x}\right)^{2}+1\right]+\arctan\dfrac{y}{x}+\ln x=0$.

+++

#### 综合填空 (5) 微分方程 $y'\sec^{2}y+\dfrac{x}{1+x^{2}}\tan y=x$ 满足 $y(0)=0$ 的特解为________.
***
$\tan y=\dfrac{1}{3}\left(1+x^{2}-\dfrac{1}{\sqrt{1+x^{2}}}\right)$.

**解** 由 $(\tan y)'=y'\sec^{2}y$，令 $u=\tan y$，则原方程为 $u'+\dfrac{x}{1+x^{2}}u=x$，为一阶线性微分方程，故通解为
$$\tan y=u=\mathrm{e}^{-\int\frac{x}{1+x^{2}}\mathrm{d}x}\left(\int x\mathrm{e}^{\int\frac{x}{1+x^{2}}\mathrm{d}x}\mathrm{d}x+C\right)=\frac{C}{\sqrt{1+x^{2}}}+\frac{1}{3}(1+x^{2}).$$

由 $y(0)=0$，得 $C=-\dfrac{1}{3}$，故所求特解为 $\tan y=\dfrac{1}{3}\left(1+x^{2}-\dfrac{1}{\sqrt{1+x^{2}}}\right)$.

【注】这类利用导数去"找变量替换"的方法，值得注意.

+++

#### 综合填空 (6) 微分方程 $y''+y=x+\cos x$ 的通解为________.
***
$y=C_1\cos x+C_2\sin x+x+\dfrac{1}{2}x\sin x$（$C_1,C_2$ 为任意常数）.

**解** 特征方程为 $r^{2}+1=0$，得 $r=\pm\mathrm{i}$，故对应齐次微分方程的通解为
$$y=C_1\cos x+C_2\sin x.$$

令 $y''+y=x$ 的特解为 $y_1^{*}=Ax$，则 $(y_1^{*})'=A$，$(y_1^{*})''=0$，故
$$0+Ax=x,\quad A=1.$$

令 $y''+y=\cos x$ 的特解为 $y_2^{*}=x(B\cos x+C\sin x)$，代入方程解得 $B=0$，$C=\dfrac{1}{2}$，故其特解为 $y_2^{*}=\dfrac{1}{2}x\sin x$，所以原方程的通解为
$$y=C_1\cos x+C_2\sin x+x+\frac{1}{2}x\sin x\quad(C_1,C_2\ \text{为任意常数}).$$

+++

#### 综合填空 (7) 微分方程 $y''-y=\sin^{2}x$ 的通解为________.
***
$y=C_1\mathrm{e}^{x}+C_2\mathrm{e}^{-x}-\dfrac{1}{2}+\dfrac{\cos 2x}{10}$（$C_1,C_2$ 为任意常数）.

**解** 特征方程为 $r^{2}-1=0$，$r=\pm1$，故对应齐次微分方程的通解为
$$y=C_1\mathrm{e}^{x}+C_2\mathrm{e}^{-x}.$$

又非齐次项为
$$\sin^{2}x=\frac{1-\cos 2x}{2}=\frac{1}{2}+\frac{-\cos 2x}{2},$$
方程 $y''-y=\dfrac{1}{2}$ 和 $y''-y=-\dfrac{\cos 2x}{2}$ 的特解分别令为
$$y_1^{*}=A,\quad y_2^{*}=B\cos 2x+C\sin 2x,$$
将其分别代入上两个方程，可求得 $A=-\dfrac{1}{2}$，$B=\dfrac{1}{10}$，$C=0$，所以 $y_1^{*}=-\dfrac{1}{2}$ 和 $y_2^{*}=\dfrac{\cos 2x}{10}$，故原方程的通解为 $y=C_1\mathrm{e}^{x}+C_2\mathrm{e}^{-x}-\dfrac{1}{2}+\dfrac{\cos 2x}{10}$（$C_1,C_2$ 为任意常数）.

+++

#### 综合填空 (8) 设 $f(x)$ 有连续导数，对任意 $a$ 满足 $f(x+a)=\displaystyle\int_{x}^{x+a}\frac{t(t^{2}+1)}{f(t)}\mathrm{d}t+f(x)$，且 $f(1)=\sqrt{2}$，则 $f(x)=$________.
***
$\dfrac{\sqrt{2}}{2}(x^{2}+1)$.

**解** 将 $x=0$ 代入已知等式，有 $f(a)=\displaystyle\int_{0}^{a}\frac{t(t^{2}+1)}{f(t)}\mathrm{d}t+f(0)$.

上式两边同时对 $a$ 求导，得 $f'(a)=\dfrac{a(a^{2}+1)}{f(a)}$，故 $2f(a)f'(a)=2a+2a^{3}$，积分得
$$\int 2f(a)f'(a)\mathrm{d}a=\int(2a+2a^{3})\mathrm{d}a,$$
故 $[f(a)]^{2}=a^{2}+\dfrac{1}{2}a^{4}+C$.

由 $f(1)=\sqrt{2}$，得 $C=\dfrac{1}{2}$，故 $f(x)=\dfrac{\sqrt{2}}{2}(x^{2}+1)$（由 $f(1)=\sqrt{2}$，知开方取正）.

+++

#### 综合填空 (9) 设 $f(x)$ 有二阶连续导数，且 $f(x)=\displaystyle\int_{0}^{x}f(1-t)\mathrm{d}t+1$，则 $f(x)=$________.
***
$\cos x+\dfrac{\cos 1}{1-\sin 1}\sin x$.

**解** 已知方程两边同时对 $x$ 求导，得
$$f'(x)=f(1-x), \qquad ①$$
两边再同时对 $x$ 求导，得
$$f''(x)=-f'(1-x). \qquad ②$$

由 ① 式，得 $f'(1-x)=f[1-(1-x)]=f(x)$，代入 ② 式，得 $f''(x)=-f(x)$.

由原方程，有 $f(0)=1$，在 ① 式中令 $x=0$，得 $f'(0)=f(1)$.

解初值问题 $\begin{cases}f''(x)+f(x)=0,\\ f(0)=1,\ f'(0)=f(1),\end{cases}$ 可得通解为 $f(x)=C_1\cos x+C_2\sin x$.

由 $f(0)=1$，得 $C_1=1$，即 $f(x)=\cos x+C_2\sin x$，故 $f'(x)=-\sin x+C_2\cos x$.

再由 $f'(0)=f(1)$，得 $C_2=\dfrac{\cos 1}{1-\sin 1}$，故 $f(x)=\cos x+\dfrac{\cos 1}{1-\sin 1}\sin x$.

+++

#### 综合解答 (1) 设 $f(x)$ 满足 $f(x+y)=\dfrac{f(x)+f(y)}{1-f(x)f(y)}$，且 $f'(0)$ 存在，求 $f'(x)$ 及 $f(x)$.
***
已知等式中，令 $x=y=0$，得 $f(0)=0$. 由导数的定义，有
$$f'(x)=\lim_{\Delta x\to0}\frac{f(x+\Delta x)-f(x)}{\Delta x}=\lim_{\Delta x\to0}\frac{\dfrac{f(x)+f(\Delta x)}{1-f(x)f(\Delta x)}-f(x)}{\Delta x}$$
$$=\lim_{\Delta x\to0}\frac{f(\Delta x)[1+f^{2}(x)]}{\Delta x[1-f(x)f(\Delta x)]}=\lim_{\Delta x\to0}\frac{\dfrac{f(\Delta x)[1+f^{2}(x)]}{\Delta x}}{1-f(x)f(\Delta x)}$$
$$=\lim_{\Delta x\to0}[1+f^{2}(x)]\frac{f(\Delta x)-f(0)}{\Delta x}\cdot\lim_{\Delta x\to0}\frac{1}{1-f(x)f(\Delta x)}=[1+f^{2}(x)]f'(0),$$
即
$$f'(x)=[1+f^{2}(x)]f'(0). \qquad ①$$

① 式变形为 $\dfrac{f'(x)}{1+f^{2}(x)}=f'(0)$，两边同时积分，得 $\arctan f(x)=f'(0)x+C$，由 $f(0)=0$，得 $C=0$，故 $\arctan f(x)=f'(0)x$，即 $f(x)=\tan[f'(0)x]$.

+++

#### 综合解答 (2) 利用变量替换 $x=\sin t$，$y=y(t)$ $\left(0<t<\dfrac{\pi}{2}\right)$ 化简方程 $(1-x^{2})\dfrac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}}-x\dfrac{\mathrm{d}y}{\mathrm{d}x}+y=0$，并求该方程的通解.
***
由 $x=\sin t$，$y=y(t)$ 及复合函数求导法则，有
$$\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{\mathrm{d}y}{\mathrm{d}t}\cdot\frac{\mathrm{d}t}{\mathrm{d}x}=\frac{1}{\cos t}\frac{\mathrm{d}y}{\mathrm{d}t},$$
$$\frac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}}=\frac{\mathrm{d}}{\mathrm{d}x}\left(\frac{\mathrm{d}y}{\mathrm{d}x}\right)=\frac{\mathrm{d}}{\mathrm{d}t}\left(\frac{1}{\cos t}\frac{\mathrm{d}y}{\mathrm{d}t}\right)\cdot\frac{\mathrm{d}t}{\mathrm{d}x}=\left(\frac{\sin t}{\cos^{2}t}\cdot\frac{\mathrm{d}y}{\mathrm{d}t}+\frac{1}{\cos t}\frac{\mathrm{d}^{2}y}{\mathrm{d}t^{2}}\right)\frac{1}{\cos t}=\frac{1}{\cos^{2}t}\frac{\mathrm{d}^{2}y}{\mathrm{d}t^{2}}+\frac{\sin t}{\cos^{3}t}\frac{\mathrm{d}y}{\mathrm{d}t}.$$

将 $\dfrac{\mathrm{d}y}{\mathrm{d}x}$，$\dfrac{\mathrm{d}^{2}y}{\mathrm{d}x^{2}}$ 代入原方程化简为
$$\frac{\mathrm{d}^{2}y}{\mathrm{d}t^{2}}+y=0, \qquad ①$$
特征方程为 $r^{2}+1=0$，$r=\pm\mathrm{i}$，故 ① 的通解为 $y=C_1\cos t+C_2\sin t$.

由 $x=\sin t\left(0<t<\dfrac{\pi}{2}\right)$，知 $\cos t=\sqrt{1-x^{2}}$，所以原方程的通解为
$$y=C_1\sqrt{1-x^{2}}+C_2x\quad(C_1,C_2\ \text{为任意常数}).$$

+++

#### 综合解答 (3) 设 $y''+(4x+\mathrm{e}^{2y})y'^{3}=0$.

（Ⅰ）若视 $x$ 为因变量，$y$ 为自变量，化简该方程；\
（Ⅱ）求该方程的通解.
***
（Ⅰ）由互为反函数的导数关系式，有 $y'(x)=\dfrac{1}{x'(y)}$，两边同时对 $x$ 求导，得
$$y''(x)=\left[\frac{1}{x'(y)}\right]'\cdot\frac{1}{x'(y)}=-\frac{x''(y)}{[x'(y)]^{3}}\quad(x'(y)\neq0),$$
故原方程为
$$-\frac{x''(y)}{[x'(y)]^{3}}+(4x+\mathrm{e}^{2y})\frac{1}{[x'(y)]^{3}}=0,$$
即
$$x''(y)-4x(y)=\mathrm{e}^{2y}. \qquad ①$$

（Ⅱ）① 式为二阶常系数非齐次线性微分方程，特征方程为 $r^{2}-4=0$，解得
$$r_1=-2,\quad r_2=2.$$

又由 $\mathrm{e}^{2y}$ 知 $\lambda=2$ 是单特征根，令特解为 $x^{*}=y\cdot A\cdot\mathrm{e}^{2y}$，代入 ① 式，可求得 $A=\dfrac{1}{4}$，故方程 ① 的通解为
$$x(y)=C_1\mathrm{e}^{-2y}+C_2\mathrm{e}^{2y}+\frac{1}{4}y\mathrm{e}^{2y}\quad(C_1,C_2\ \text{为任意常数}).$$

+++

#### 综合解答 (4) 设 $f(x)$ 有二阶连续导数，且 $f(1)=1$，$f'(1)=2$，求 $u(x,y)$，使得 $\mathrm{d}u=-6yf(x)\mathrm{d}x+[x^{2}f'(x)-4xf(x)]\mathrm{d}y$.
***
令 $P=-6yf(x)$，$Q=x^{2}f'(x)-4xf(x)$，依题意，有 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，即
$$x^{2}f''(x)-2xf'(x)+2f(x)=0,$$
为欧拉方程.

令 $x=\mathrm{e}^{t}$，则上面方程化为
$$f''(t)-3f'(t)+2f(t)=0, \qquad ①$$
为二阶常系数线性齐次微分方程，其特征方程为 $r^{2}-3r+2=0$，解得 $r_1=1$，$r_2=2$，故 ① 的通解为 $f(t)=C_1\mathrm{e}^{t}+C_2\mathrm{e}^{2t}$，所以 $f(x)=C_1x+C_2x^{2}$.

由 $f(1)=1$，$f'(1)=2$，得 $C_1=0$，$C_2=1$，故 $f(x)=x^{2}$，$f'(x)=2x$，从而
$$\mathrm{d}u=-6x^{2}y\mathrm{d}x-2x^{3}\mathrm{d}y.$$

利用公式，有
$$u(x,y)=\int_{0}^{x}-6x^{2}y\mathrm{d}x+\int_{0}^{y}0\mathrm{d}y=-2x^{3}y,$$
所求 $u(x,y)=-2x^{3}y+C$（$C$ 为任意常数）.

+++

#### 综合解答 (5) 设 $f(x)$ 在 $[1,+\infty)$ 上有二阶连续导数，$f(1)=0$，$f'(1)=1$，且函数 $z=(x^{2}+y^{2})f(x^{2}+y^{2})$ 满足 $\dfrac{\partial^{2}z}{\partial x^{2}}+\dfrac{\partial^{2}z}{\partial y^{2}}=0$，求 $f(x)$ 及 $f(x)$ 在 $[1,+\infty)$ 上的最大值.
***
令 $x^{2}+y^{2}=u$，则 $z=uf(u)$，$u_x'=2x$，$u_y'=2y$，于是
$$\frac{\partial z}{\partial x}=f(u)u_x'+uf'(u)u_x'=2x[f(u)+uf'(u)],$$
$$\frac{\partial^{2}z}{\partial x^{2}}=2[f(u)+uf'(u)]+2x[f'(u)u_x'+f'(u)u_x'+uf''(u)u_x']=2f(u)+(10x^{2}+2y^{2})f'(u)+4x^{2}uf''(u).$$

由 $z=(x^{2}+y^{2})f(x^{2}+y^{2})$ 关于 $x$ 与 $y$ 具有轮换对称性，知
$$\frac{\partial^{2}z}{\partial y^{2}}=2f(u)+(10y^{2}+2x^{2})f'(u)+4y^{2}uf''(u),$$
将其代入到 $\dfrac{\partial^{2}z}{\partial x^{2}}+\dfrac{\partial^{2}z}{\partial y^{2}}=0$，得
$$u^{2}f''(u)+3uf'(u)+f(u)=0, \qquad ①$$
① 为二阶欧拉方程，令 $\mathrm{e}^{t}=u$，则
$$uf'(u)=\frac{\mathrm{d}[f(t)]}{\mathrm{d}t},\quad u^{2}f''(u)=\frac{\mathrm{d}^{2}[f(t)]}{\mathrm{d}t^{2}}-\frac{\mathrm{d}[f(t)]}{\mathrm{d}t},$$
将其代入 ① 式，得
$$\frac{\mathrm{d}^{2}[f(t)]}{\mathrm{d}t^{2}}+2\frac{\mathrm{d}[f(t)]}{\mathrm{d}t}+f(t)=0, \qquad ②$$
特征方程为 $r^{2}+2r+1=0$，得 $r_1=r_2=-1$，故 ② 的通解为
$$f(u)=f(t)=C_1\mathrm{e}^{-t}+C_2t\mathrm{e}^{-t}=\frac{1}{u}(C_1+C_2\ln u).$$

由 $f(1)=0$，$f'(1)=1$，得 $C_1=0$，$C_2=1$，所以 $f(u)=\dfrac{\ln u}{u}$，即 $f(x)=\dfrac{\ln x}{x}$.

由 $f'(x)=\dfrac{1-\ln x}{x^{2}}=0$，得 $x=\mathrm{e}$，且当 $1\leqslant x<\mathrm{e}$ 时，$f'(x)>0$；当 $x>\mathrm{e}$ 时，$f'(x)<0$，故 $f(\mathrm{e})=\dfrac{1}{\mathrm{e}}$ 为所求最大值.

+++

#### 综合解答 (6) 设二阶常系数非齐次线性微分方程 $y''+ay'+by=(cx+d)\mathrm{e}^{2x}$ 有特解 $y=2\mathrm{e}^{x}+(x^{2}-1)\mathrm{e}^{2x}$，求该方程的通解，并求 $a,b,c,d$ 的值.
***
方程的通解为
$$y=C_1y_1(x)+C_2y_2(x)+y^{*}(x), \qquad ①$$
其中 $y_1(x),y_2(x)$ 是对应齐次微分方程的两个线性无关的解，$y^{*}(x)$ 是非齐次微分方程的特解.

若 $y^{*}(x)=(Ax+B)\mathrm{e}^{2x}$，则 $\lambda=2$ 不是特征根；\
若 $y^{*}(x)=x(Ax+B)\mathrm{e}^{2x}$，则 $\lambda=2$ 是单特征根.

由已知特解 $y=2\mathrm{e}^{x}+(x^{2}-1)\mathrm{e}^{2x}=2\mathrm{e}^{x}-\mathrm{e}^{2x}+x^{2}\mathrm{e}^{2x}$，应为 ① 式中取定常数所得，从而可知
$$y_1(x)=\mathrm{e}^{x},\quad y_2(x)=\mathrm{e}^{2x},\quad y^{*}(x)=x^{2}\mathrm{e}^{2x},$$
因此 $r=1$，$r=2$ 为特征根，由根与系数的关系，知 $a=-(1+2)=-3$，$b=1\times2=2$，所以原方程的通解为 $y=C_1\mathrm{e}^{x}+C_2\mathrm{e}^{2x}+x^{2}\mathrm{e}^{2x}$（$C_1,C_2$ 为任意常数）.

将 $y^{*}=x^{2}\mathrm{e}^{2x}$ 代入原方程，可得
$$\mathrm{e}^{2x}(4x^{2}+8x+2)-3\mathrm{e}^{2x}(2x^{2}+2x)+2x^{2}\mathrm{e}^{2x}=(cx+d)\mathrm{e}^{2x},$$
即 $2x+2=cx+d$，得 $c=2$，$d=2$.

综上可得，$a=-3$，$b=2$，$c=2$，$d=2$.

+++

#### 综合解答 (7) 设 $y(x)$ 在 $[x_0,+\infty)$ 上有一阶连续导数，且 $\lim\limits_{x\to+\infty}[y'(x)+y(x)]=k$，求 $\lim\limits_{x\to+\infty}y(x)$.
***
令 $y'(x)+y(x)=f(x)$，则由一阶线性微分方程的通解公式，得
$$y(x)=\mathrm{e}^{-x}\left[\int_{x_0}^{x}\mathrm{e}^{t}f(t)\mathrm{d}t+C\right],$$
$$\lim_{x\to+\infty}y(x)=\lim_{x\to+\infty}\frac{\displaystyle\int_{x_0}^{x}\mathrm{e}^{t}f(t)\mathrm{d}t+C}{\mathrm{e}^{x}}.$$

当 $x\to+\infty$ 时，若 $\displaystyle\int_{x_0}^{x}\mathrm{e}^{t}f(t)\mathrm{d}t\to\infty$，则由洛必达法则，知
$$\lim_{x\to+\infty}y(x)=\lim_{x\to+\infty}\frac{\mathrm{e}^{x}f(x)}{\mathrm{e}^{x}}=\lim_{x\to+\infty}f(x)=k;$$

当 $x\to+\infty$ 时，若 $\displaystyle\int_{x_0}^{x}\mathrm{e}^{t}f(t)\mathrm{d}t$ 不趋于 $\infty$，则必有 $k=0$，故
$$\lim_{x\to+\infty}y(x)=\lim_{x\to+\infty}\mathrm{e}^{-x}\left[\int_{x_0}^{x}\mathrm{e}^{t}f(t)\mathrm{d}t+C\right]=0=k.$$

+++

#### 综合解答 (8) 设 $f(x),g(x)$ 满足 $f'(x)=g(x)$，$g(x)=\displaystyle\int_{0}^{x}[1-f(t)]\mathrm{d}t+1$，且 $f(0)=1$，求 $I=\displaystyle\int_{0}^{\frac{\pi}{2}}\mathrm{e}^{-x}[g(x)-f(x)]\mathrm{d}x$.
***
由已知，有 $f''(x)=g'(x)=1-f(x)$，$f'(0)=g(0)=1$，故
$$\begin{cases}f''(x)+f(x)=1,\\ f(0)=f'(0)=1,\end{cases}$$
解上述方程，得 $f(x)=C_1\cos x+C_2\sin x+1$.

由 $f(0)=f'(0)=1$，得 $C_1=0$，$C_2=1$，故 $f(x)=\sin x+1$，所以
$$I=\int_{0}^{\frac{\pi}{2}}\mathrm{e}^{-x}[g(x)-f(x)]\mathrm{d}x=\int_{0}^{\frac{\pi}{2}}\mathrm{e}^{-x}[f'(x)-f(x)]\mathrm{d}x$$
$$=\int_{0}^{\frac{\pi}{2}}\mathrm{d}[\mathrm{e}^{-x}f(x)]=\mathrm{e}^{-x}f(x)\bigg|_{0}^{\frac{\pi}{2}}=2\mathrm{e}^{-\frac{\pi}{2}}-1.$$

+++

#### 综合解答 (9) 设 $y=y(x)$ 有一阶连续导数，$y(0)=1$，且满足 $y'(x)+3\displaystyle\int_{0}^{x}y'(t)\mathrm{d}t+2x\displaystyle\int_{0}^{1}y(xu)\mathrm{d}u+\mathrm{e}^{-x}=0$，求 $y=y(x)$.
***
令 $xu=t$，则
$$\int_{0}^{1}y(xu)\mathrm{d}u=\int_{0}^{x}y(t)\frac{1}{x}\mathrm{d}t=\frac{1}{x}\int_{0}^{x}y(t)\mathrm{d}t,$$
故原方程化为
$$y'(x)+3\int_{0}^{x}y'(t)\mathrm{d}t+2\int_{0}^{x}y(t)\mathrm{d}t+\mathrm{e}^{-x}=0, \qquad ①$$
① 式两边同时对 $x$ 求导，得
$$y''(x)+3y'(x)+2y(x)=\mathrm{e}^{-x}, \qquad ②$$
且 $y(0)=1$，$y'(0)=-1$，特征方程为 $r^{2}+3r+2=0$，得 $r_1=-1$，$r_2=-2$，令特解 $y^{*}=Ax\mathrm{e}^{-x}$，代入 ② 式可得 $A=1$，故方程 ② 的通解为 $y=C_1\mathrm{e}^{-x}+C_2\mathrm{e}^{-2x}+x\mathrm{e}^{-x}$.

又由 $y(0)=1$，$y'(0)=-1$，得 $C_1=0$，$C_2=1$，故 $y=y(x)=\mathrm{e}^{-2x}+x\mathrm{e}^{-x}$.

+++

#### 综合解答 (10) 设 $y=y(x)$ 是向上凸的连续曲线，其上任一点 $(x,y)$ 处的曲率为 $\dfrac{1}{\sqrt{1+y'^{2}}}$，且此曲线上点 $(0,1)$ 处的切线方程为 $y=x+1$，求该曲线的方程.
***
由已知，$y''<0$，于是曲率为
$$K=\frac{|y''|}{(1+y'^{2})^{\frac{3}{2}}}=\frac{-y''}{(1+y'^{2})^{\frac{3}{2}}}=\frac{1}{\sqrt{1+y'^{2}}},$$
化简得 $y''=-(1+y'^{2})$.

由已知，$y(0)=1$，$y'(0)=1$，令 $y'=p$，$y''=\dfrac{\mathrm{d}p}{\mathrm{d}x}$，代入上方程，得 $\dfrac{\mathrm{d}p}{1+p^{2}}=-\mathrm{d}x$，积分得 $p=\tan(C_1-x)$，由 $y'(0)=1$，得 $C_1=\dfrac{\pi}{4}$，故
$$\frac{\mathrm{d}y}{\mathrm{d}x}=\tan\left(\frac{\pi}{4}-x\right)\quad\left(-\frac{\pi}{4}<x<\frac{3\pi}{4}\right),$$
积分得 $y=\ln\left|\cos\left(\dfrac{\pi}{4}-x\right)\right|+C_2$，再由 $y(0)=1$，得 $C_2=1+\dfrac{1}{2}\ln 2$，故所求曲线为
$$y=\ln\left[\cos\left(\frac{\pi}{4}-x\right)\right]+1+\frac{1}{2}\ln 2,\quad-\frac{\pi}{4}<x<\frac{3\pi}{4}.$$

+++

#### 综合解答 (11) （Ⅰ）设 $a(t)$ 在 $[0,+\infty)$ 上是非负连续函数，证明：当且仅当 $\displaystyle\int_{0}^{+\infty}a(t)\mathrm{d}t$ 发散时，微分方程 $\dfrac{\mathrm{d}x}{\mathrm{d}t}+a(t)x=0$ 的每一个解 $x(t)$ 满足 $\lim\limits_{t\to+\infty}x(t)=0$；

（Ⅱ）设 $a>0$，$f(t)$ 在 $[0,+\infty)$ 上连续有界，证明：方程 $\dfrac{\mathrm{d}x}{\mathrm{d}t}+ax=f(t)$ $(t\geqslant0)$ 的所有解在 $[0,+\infty)$ 上有界.
***
**证**（Ⅰ）$\dfrac{\mathrm{d}x}{\mathrm{d}t}+a(t)x=0$ 的通解可表示为 $x(t)=C\mathrm{e}^{-\int_{0}^{t}a(s)\mathrm{d}s}$，当且仅当 $\displaystyle\int_{0}^{+\infty}a(t)\mathrm{d}t$ 发散时，
$$-\int_{0}^{t}a(s)\mathrm{d}s\to-\infty\quad(t\to+\infty),$$
故有 $\lim\limits_{t\to+\infty}x(t)=0$.

（Ⅱ）该方程的通解为 $x(t)=\mathrm{e}^{-at}\left[C+\displaystyle\int_{0}^{t}\mathrm{e}^{as}f(s)\mathrm{d}s\right]$ $(t>0)$，满足 $x(0)=x_0$ 的解为
$$x_0(t)=\mathrm{e}^{-at}\left[x_0+\int_{0}^{t}\mathrm{e}^{as}f(s)\mathrm{d}s\right]\quad(t>0).$$

当 $t\in[0,+\infty)$ 时，由已知，设 $|f(t)|\leqslant M$（$M>0$），则可得
$$|x_0(t)|\leqslant|x_0|+\left|\int_{0}^{t}\mathrm{e}^{-a(t-s)}f(s)\mathrm{d}s\right|\leqslant|x_0|+M\left|\int_{0}^{t}\mathrm{e}^{-a(t-s)}\mathrm{d}s\right|\leqslant|x_0|+\frac{M}{a}.$$

+++

#### 综合解答 (12) 设函数 $y(x)$ $(x\geqslant0)$ 二阶可导，且 $y'(x)>0$，$y(0)=1$，过曲线 $y=y(x)$ 上任一点 $P(x,y)$ 作曲线的切线及 $x$ 轴的垂线，上述两条直线与 $x$ 轴所围三角形的面积记为 $S_1$，区间 $[0,x]$ 上以 $y=y(x)$ 为曲边的曲边梯形的面积记为 $S_2$，且 $2S_1-S_2=1$，求曲线 $y=y(x)$.
***
$y=y(x)$ 在点 $P(x,y)$ 处的切线方程为 $Y-y=y'(X-x)$，它与 $x$ 轴的交点为 $\left(x-\dfrac{y}{y'},0\right)$. 由 $y(0)=1$，$y'(x)>0$，知 $y(x)>y(0)=1>0$（$x>0$），于是
$$S_1=\frac{1}{2}|y|\left|x-\left(x-\frac{y}{y'}\right)\right|=\frac{y^{2}}{2y'},\quad S_2=\int_{0}^{x}y(t)\mathrm{d}t,$$
由 $2S_1-S_2=1$，得
$$\frac{y^{2}}{y'}-\int_{0}^{x}y(t)\mathrm{d}t=1.$$

由此知，$y'(0)=1$，上式两边同时对 $x$ 求导并化简，得 $yy''=y'^{2}$. 令 $y'=p$，$y''=p\dfrac{\mathrm{d}p}{\mathrm{d}y}$，则方程为
$$py\frac{\mathrm{d}p}{\mathrm{d}y}=p^{2}.$$

由 $y'>0$，即 $p>0$，故 $\dfrac{\mathrm{d}p}{p}=\dfrac{\mathrm{d}y}{y}$，积分得 $p=C_1y$，由 $y=1$，$p=1$，得 $C_1=1$，即 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=y$，于是 $y=C_2\mathrm{e}^{x}$，再由 $y(0)=1$，得 $C_2=1$，所求曲线为 $y=\mathrm{e}^{x}$.

+++

#### 综合解答 (13) 一架质量为 $4.5$ 吨的歼击机以 $600\ \mathrm{km/h}$ 的航速开始着陆，在减速伞的作用下滑跑 $500\ \mathrm{m}$ 后速度减为 $100\ \mathrm{km/h}$，设减速伞的阻力与飞机的速度成正比，忽略飞机所受的其他外力，求减速伞的阻力系数. 若保障飞机安全着陆，跑道长度至少应为多少？
***
由牛顿第二定律，$F_{阻}=ma$，故由已知条件，有 $-kv=m\dfrac{\mathrm{d}v}{\mathrm{d}t}$. 又
$$\frac{\mathrm{d}v}{\mathrm{d}t}=\frac{\mathrm{d}v}{\mathrm{d}x}\cdot\frac{\mathrm{d}x}{\mathrm{d}t}=v\cdot\frac{\mathrm{d}v}{\mathrm{d}x}\quad(x\ \text{表示位移}),$$
故 $-kv=m\cdot v\dfrac{\mathrm{d}v}{\mathrm{d}x}$，即 $\mathrm{d}v=-\dfrac{k}{m}\mathrm{d}x$，积分得
$$v=v_0-\frac{k}{m}x, \qquad ①$$
故 $k=\dfrac{m(v_0-v)}{x}$.

将 $m=4\,500\ \mathrm{kg}$，$v_0=600\ \mathrm{km/h}$，$v=100\ \mathrm{km/h}$，$x=0.5\ \mathrm{km}$ 代入上式，得 $k=4.5\times10^{6}\ \mathrm{kg/h}$.

由 ① 有 $v=600-\dfrac{4.5\times10^{6}}{4\,500}\cdot x$，令 $v=0$，解得 $x=0.6\ \mathrm{km}$，即跑道至少应为 $600\ \mathrm{m}$.

+++

#### 拓展解答 (1) 设环境保持恒定温度 $20^{\circ}\mathrm{C}$，有一物体的温度在 $10$ 秒内从 $100^{\circ}\mathrm{C}$ 降到 $60^{\circ}\mathrm{C}$，若物体温度下降的速度与该物体与环境温度之差成正比，问此物体从 $100^{\circ}\mathrm{C}$ 降到 $25^{\circ}\mathrm{C}$ 需要多少时间？
***
依题意，设该物体温度为 $T(t)$，则
$$\frac{\mathrm{d}T(t)}{\mathrm{d}t}=-k[T(t)-20]\quad(k>0),$$
即 $\dfrac{\mathrm{d}T(t)}{\mathrm{d}t}+kT(t)=20k$.

解一阶线性微分方程，得通解为 $T(t)=20+C\mathrm{e}^{-kt}$.

由初始条件 $T(0)=100$，得 $C=80$，故 $T(t)=20+80\mathrm{e}^{-kt}$.

又由 $T(10)=20+80\mathrm{e}^{-10k}=60$，解得 $k=\dfrac{1}{10}\ln 2$，故
$$T(t)=20+80\cdot2^{-0.1t}.$$

由 $T(t)=25$，即 $2^{-0.1t}=\dfrac{1}{16}$，解得 $t=40$，故物体从 $100^{\circ}\mathrm{C}$ 降到 $25^{\circ}\mathrm{C}$ 需要 $40$ 秒.

+++

#### 拓展解答 (2) 设全微分方程 $[xy(x+y)-f(x)y]\mathrm{d}x+[x^{2}y+f'(x)]\mathrm{d}y=0$，其中 $f(x)$ 有二阶连续导数，且 $f(0)=0$，$f'(0)=1$，求 $f(x)$ 及全微分方程的通解.
***
已知方程为全微分方程，记
$$P=xy(x+y)-f(x)y,\quad Q=x^{2}y+f'(x),$$
则由 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，得
$$f''(x)+f(x)=x^{2}. \qquad ①$$

由齐次方程 $f''(x)+f(x)=0$，得特征方程为 $r^{2}+1=0$，解得 $r=\pm\mathrm{i}$，故其通解为
$$y=C_1\cos x+C_2\sin x.$$

由于 $x^{2}\mathrm{e}^{0\cdot x}$，且 $\lambda=0$ 不是特征根，故令方程 ① 的特解为
$$y^{*}=x^{0}\cdot(ax^{2}+bx+c),$$
代入 ① 式，可求得 $a=1$，$b=0$，$c=-2$，故 $y^{*}=x^{2}-2$，从而方程 ① 的通解为
$$f(x)=C_1\cos x+C_2\sin x+x^{2}-2.$$

由 $f(0)=0$，$f'(0)=1$，得 $C_1=2$，$C_2=1$，故
$$f(x)=2\cos x+\sin x+x^{2}-2. \qquad ②$$

由 ② 式，可知全微分方程为
$$[xy^{2}-(2\cos x+\sin x)y+2y]\mathrm{d}x+(-2\sin x+\cos x+2x+x^{2}y)\mathrm{d}y=0.$$

由于
$$[xy^{2}-(2\cos x+\sin x)y+2y]\mathrm{d}x+(-2\sin x+\cos x+2x+x^{2}y)\mathrm{d}y$$
$$=\mathrm{d}\left(\frac{x^{2}y^{2}}{2}\right)+\mathrm{d}(2xy)-\mathrm{d}(2y\sin x)+\mathrm{d}(y\cos x)$$
$$=\mathrm{d}\left(\frac{x^{2}y^{2}}{2}+2xy-2y\sin x+y\cos x\right)=0,$$
故全微分方程通解为
$$\frac{x^{2}y^{2}}{2}+2xy-2y\sin x+y\cos x=C\quad(C\ \text{为任意常数}).$$
