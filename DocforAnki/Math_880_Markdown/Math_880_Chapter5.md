---
quizify:
  format: 1
  deck: Math_880::Chapter_5
  tags: [Math, 880题, 数一, 第五章, 多元函数微分学]
---

+++

#### 基础选择 (1) 设 $f(x,y)=\arcsin\sqrt{x^2+y^4}$，则下列选项正确的是（　）。

;;;
A. $f'_x(0,0)$ 存在，$f'_y(0,0)$ 存在
B. $f'_x(0,0)$ 不存在，$f'_y(0,0)$ 存在
C. $f'_x(0,0)$ 不存在，$f'_y(0,0)$ 不存在
D. $f'_x(0,0)$ 存在，$f'_y(0,0)$ 不存在
;;;B
***
**B.**

解

$$
f'_x(0,0)=\lim_{x\to0}\frac{f(x,0)-f(0,0)}{x}=\lim_{x\to0}\frac{\arcsin|x|}{x}=\lim_{x\to0}\frac{|x|}{x},
$$

不存在，

$$
f'_y(0,0)=\lim_{y\to0}\frac{f(0,y)-f(0,0)}{y}=\lim_{y\to0}\frac{\arcsin y^2}{y}=\lim_{y\to0}\frac{y^2}{y}=0,
$$

故 B 正确。

+++

#### 基础选择 (2) 设 $f'_x(x_0,y_0)$，$f'_y(x_0,y_0)$ 均存在，则下列选项正确的是（　）。

;;;
A. $\lim\limits_{\substack{x\to x_0\\ y\to y_0}}f(x,y)$ 存在
B. $f(x,y)$ 在 $(x_0,y_0)$ 处连续
C. $\lim\limits_{x\to x_0}f(x,y_0)$ 存在
D. $f(x,y)$ 在 $\mathring{U}(x_0,y_0)$ 内有定义
;;;C
***
**C.**

解　$f(x,y)$ 在某点偏导数存在不一定在该点连续，排除 B。也不能推得 $\lim\limits_{\substack{x\to x_0\\ y\to y_0}}f(x,y)$ 存在，例如：设

$$
f(x,y)=\begin{cases}\dfrac{xy}{x^2+y^2},&(x,y)\neq(0,0),\\[2mm] 0,&(x,y)=(0,0),\end{cases}
$$

可知 $f'_x(0,0)$，$f'_y(0,0)$ 都存在，但 $\lim\limits_{\substack{x\to0\\ y\to0}}f(x,y)$ 不存在，故排除 A。

由 $f'_x(x_0,y_0)=\lim\limits_{x\to x_0}\dfrac{f(x,y_0)-f(x_0,y_0)}{x-x_0}$ 存在，只能推得当固定 $y=y_0$ 时，$f(x,y)$ 在 $x_0$ 的邻域内有定义。而

$$
\mathring{U}(x_0,y_0)=\left\{(x,y)\ \middle|\ 0<\sqrt{(x-x_0)^2+(y-y_0)^2}<\delta\right\}
$$

是圆域，故 D 不正确。

由 $f'_x(x_0,y_0)=\lim\limits_{x\to x_0}\dfrac{f(x,y_0)-f(x_0,y_0)}{x-x_0}$ 存在，知 $\lim\limits_{x\to x_0}f(x,y_0)=f(x_0,y_0)$，C 正确。

+++

#### 基础选择 (3) 设方程 $xy-z\ln y+\mathrm{e}^{xz}=1$，存在点 $(0,1,1)$ 的一个邻域，在此邻域内该方程（　）。

;;;
A. 可确定隐函数 $y=y(x,z)$ 和 $z=z(x,y)$
B. 可确定隐函数 $x=x(y,z)$ 和 $z=z(x,y)$
C. 可确定隐函数 $x=x(y,z)$ 和 $y=y(x,z)$
D. 只能确定隐函数 $z=z(x,y)$
;;;C
***
**C.**

解　令 $F(x,y,z)=xy-z\ln y+\mathrm{e}^{xz}-1$，则 $F(0,1,1)=0$。

$F(x,y,z)$ 对 $x,y,z$ 分别求偏导，得 $F'_x=y+\mathrm{e}^{xz}\cdot z$，$F'_y=x-\dfrac{z}{y}$，$F'_z=-\ln y+\mathrm{e}^{xz}\cdot x$，故

$$
F'_x(0,1,1)=2\neq0,\quad F'_y(0,1,1)=-1\neq0,\quad F'_z(0,1,1)=0,
$$

根据隐函数存在定理，知 $F(x,y,z)=0$ 在点 $(0,1,1)$ 的某个邻域内能确定隐函数 $x=x(y,z)$ 和 $y=y(x,z)$，故 C 正确。

+++

#### 基础选择 (4) 设可微函数 $f(x,y)$ 在点 $P(x_0,y_0)$ 处取得极大值，则（　）。

;;;
A. $f(x_0,y)$ 在 $y=y_0$ 处导数小于零
B. $f(x_0,y)$ 在 $y=y_0$ 处导数大于零
C. $f(x_0,y)$ 在 $y=y_0$ 处导数等于零
D. $f(x_0,y)$ 在 $y=y_0$ 处导数不存在
;;;C
***
**C.**

解　由已知，$f(x,y)$ 在点 $P(x_0,y_0)$ 处取得极大值，由极值的必要条件，知

$$
f'_x(x_0,y_0)=f'_y(x_0,y_0)=0,
$$

故 C 正确。

+++

#### 基础选择 (5) 设 $f(x,y)=\mathrm{e}^{2x}(x+y^2+2y)$，则 $f(x,y)$ 在点 $P\left(\dfrac12,-1\right)$ 处（　）。

;;;
A. 取得极小值 $-\dfrac{\mathrm{e}}{2}$
B. 取得极大值 $-\dfrac{\mathrm{e}}{2}$
C. 取得极大值 $\mathrm{e}$
D. 不取得极值
;;;A
***
**A.**

解　由

$$
\begin{cases}f'_x=\mathrm{e}^{2x}(2x+2y^2+4y+1)=0,\\ f'_y=\mathrm{e}^{2x}(2y+2)=0,\end{cases}
$$

得驻点 $P\left(\dfrac12,-1\right)$。由于 $A=f''_{xx}(P)=2\mathrm{e}$，$B=f''_{xy}(P)=0$，$C=f''_{yy}(P)=2\mathrm{e}$，故

$$
AC-B^2=2\mathrm{e}\cdot2\mathrm{e}-0>0,\quad A=2\mathrm{e}>0,
$$

所以 $f\left(\dfrac12,-1\right)=-\dfrac{\mathrm{e}}{2}$ 为极小值，A 正确。

+++

#### 基础选择 (6) 设 $z=f(x,y)$ 在点 $(0,0)$ 的某邻域内有定义，且 $f'_x(0,0)=1$，$f'_y(0,0)=1$，则（　）。

;;;
A. $\mathrm{d}z\big|_{(0,0)}=\mathrm{d}x+\mathrm{d}y$
B. 曲线 $\begin{cases}z=f(x,y),\\ y=0\end{cases}$ 在点 $(0,0,f(0,0))$ 处的切向量为 $(1,0,1)$
C. 曲面 $z=f(x,y)$ 在点 $(0,0,f(0,0))$ 处的法向量为 $(1,1,1)$
D. $\lim\limits_{\substack{x\to0\\ y\to0}}f(x,y)$ 必存在
;;;B
***
**B.**

解　偏导数存在，不能推得可微，故 A 不正确。

曲线 $\begin{cases}x=x,\\ y=0,\\ z=f(x,0),\end{cases}$ 视 $x$ 为参数，故切向量为 $(1,0,f'_x(0,0))=(1,0,1)$，B 正确。

曲面 $z=f(x,y)$ 在点 $(0,0,f(0,0))$ 处的法向量为

$$
(f'_x(0,0),f'_y(0,0),-1)=(1,1,-1),
$$

故 C 不正确。

偏导数存在不能推出二重极限必存在，故 D 不正确。

+++

#### 基础选择 (7) 设 $f(x,y)=\dfrac{\mathrm{e}^x}{x-y}$，则（　）。

;;;
A. $f'_x+f'_y=0$
B. $f'_x-f'_y=0$
C. $f'_x-f'_y=f$
D. $f'_x+f'_y=f$
;;;D
***
**D.**

解　由于 $f'_x=\dfrac{\mathrm{e}^x(x-y)-\mathrm{e}^x}{(x-y)^2}$，$f'_y=\dfrac{\mathrm{e}^x}{(x-y)^2}$，故

$$
f'_x+f'_y=\frac{\mathrm{e}^x}{x-y}=f,
$$

D 正确。

+++

#### 基础选择 (8) 设曲面 $S$ 由方程 $F(ax-bz,ay-cz)=0$ 所确定，$F$ 有连续偏导数，$a,b,c$ 是不为零的常数，则曲面 $S$ 上任一点的切平面都平行于直线（　）。

;;;
A. $\dfrac{x}{a}=\dfrac{y}{b}=\dfrac{z}{c}$
B. $\dfrac{x}{b}=\dfrac{y}{c}=\dfrac{z}{a}$
C. $\dfrac{x}{c}=\dfrac{y}{b}=\dfrac{z}{a}$
D. $\dfrac{x}{c}=\dfrac{y}{a}=\dfrac{z}{b}$
;;;B
***
**B.**

解　设方程 $F(ax-bz,ay-cz)=0$ 确定的隐函数为 $z=z(x,y)$，则其切平面的法向量 $\boldsymbol{n}=\left(\dfrac{\partial z}{\partial x},\dfrac{\partial z}{\partial y},-1\right)$。

方程两边同时对 $x,y$ 求偏导，得

$$
\begin{cases}F'_1\left(a-b\dfrac{\partial z}{\partial x}\right)+F'_2\left(0-c\dfrac{\partial z}{\partial x}\right)=0,\\[2mm] F'_1\left(0-b\dfrac{\partial z}{\partial y}\right)+F'_2\left(a-c\dfrac{\partial z}{\partial y}\right)=0,\end{cases}
$$

解得

$$
\frac{\partial z}{\partial x}=\frac{aF'_1}{bF'_1+cF'_2},\quad \frac{\partial z}{\partial y}=\frac{aF'_2}{bF'_1+cF'_2}.
$$

设 $\boldsymbol{l}=(b,c,a)$，由于

$$
\boldsymbol{l}\cdot\boldsymbol{n}=\frac{abF'_1}{bF'_1+cF'_2}+\frac{caF'_2}{bF'_1+cF'_2}+(-a)=\frac{abF'_1+caF'_2-a(bF'_1+cF'_2)}{bF'_1+cF'_2}=0,
$$

故 B 正确。

+++

#### 基础填空 (1) $\lim\limits_{\substack{x\to3\\ y\to0}}\dfrac{\ln(x+\mathrm{e}^y)}{\sqrt{x^2+y^2}}=$________。
***
**$\dfrac23\ln2$.**

解　由于函数在点 $(3,0)$ 处连续，故极限存在，且

$$
\lim_{\substack{x\to3\\ y\to0}}\frac{\ln(x+\mathrm{e}^y)}{\sqrt{x^2+y^2}}=\frac{\ln(3+\mathrm{e}^0)}{\sqrt{3^2+0^2}}=\frac23\ln2.
$$

+++

#### 基础填空 (2) $\lim\limits_{\substack{x\to\infty\\ y\to\infty}}\dfrac{x+y}{x^2-xy+y^2}=$________。
***
**$0$.**

解　利用不等式 $x^2+y^2\geqslant2|xy|$ 求解。

由于当 $x\to\infty$，$y\to\infty$ 时，有

$$
0\leqslant\left|\frac{x+y}{x^2-xy+y^2}\right|\leqslant\frac{|x|+|y|}{|xy|}=\frac{1}{|x|}+\frac{1}{|y|}\to0,
$$

故 $\lim\limits_{\substack{x\to\infty\\ y\to\infty}}\left|\dfrac{x+y}{x^2-xy+y^2}\right|=0$，从而原极限 $=0$。

+++

#### 基础填空 (3) $\lim\limits_{\substack{x\to\infty\\ y\to0}}\left(1-\dfrac{1}{2x}\right)^{\frac{x^2}{x+y}}=$________。
***
**$\mathrm{e}^{-\frac12}$.**

解

$$
\lim_{\substack{x\to\infty\\ y\to0}}\left(1-\frac{1}{2x}\right)^{\frac{x^2}{x+y}}=\lim_{\substack{x\to\infty\\ y\to0}}\left[\left(1-\frac{1}{2x}\right)^{-2x}\right]^{\frac{x}{x+y}\cdot\left(-\frac12\right)}=\mathrm{e}^{-\frac12}.
$$

+++

#### 基础填空 (4) 设 $z=(1+xy)^y$，则 $\mathrm{d}z\big|_{(1,1)}=$________。
***
**$\mathrm{d}x+(1+2\ln2)\mathrm{d}y$.**

解

$$
\frac{\partial z}{\partial x}=y(1+xy)^{y-1}\cdot y,
$$

$$
\frac{\partial z}{\partial y}=(1+xy)^y\cdot\left[\ln(1+xy)+\frac{xy}{1+xy}\right],
$$

故 $\dfrac{\partial z}{\partial x}\bigg|_{(1,1)}=1$，$\dfrac{\partial z}{\partial y}\bigg|_{(1,1)}=1+2\ln2$，于是

$$
\mathrm{d}z\big|_{(1,1)}=\mathrm{d}x+(1+2\ln2)\mathrm{d}y.
$$

+++

#### 基础填空 (5) 设函数 $f(x,y)$ 可微，且 $f(1,2)=2$，$f'_x(1,2)=3$，$f'_y(1,2)=4$，$F(x)=f[x,f(x,2x)]$，则 $F'(1)=$________。
***
**$47$.**

解　$F'(x)=f'_1+f'_2(f'_1+2f'_2)$。由于

$$
f[1,f(1,2)]=f(1,2),\quad f'_1(1,2)=f'_x(1,2)=3,\quad f'_2(1,2)=f'_y(1,2)=4,
$$

故

$$
\begin{aligned}
F'(1)&=f'_1(1,2)+f'_2(1,2)[f'_1(1,2)+2f'_2(1,2)]\\
&=3+4\times(3+8)=47.
\end{aligned}
$$

+++

#### 基础填空 (6) 设 $z=z(x,y)$ 由方程 $x=z\mathrm{e}^{y+z}$ 确定，则 $\mathrm{d}z\big|_{(\mathrm{e},0)}=$________。
***
**$\dfrac{1}{2\mathrm{e}}\mathrm{d}x-\dfrac12\mathrm{d}y$.**

解　由 $x=\mathrm{e}$，$y=0$，知 $z=1$。令 $F(x,y,z)=z\mathrm{e}^{y+z}-x$，则

$$
\frac{\partial z}{\partial x}=-\frac{F'_x}{F'_z}=-\frac{-1}{\mathrm{e}^{y+z}(1+z)}=\frac{1}{\mathrm{e}^{y+z}(1+z)}=\frac{z}{x(1+z)},
$$

$$
\frac{\partial z}{\partial y}=-\frac{F'_y}{F'_z}=-\frac{z\mathrm{e}^{y+z}}{\mathrm{e}^{y+z}(1+z)}=-\frac{z}{1+z},
$$

故 $\dfrac{\partial z}{\partial x}\bigg|_{(\mathrm{e},0)}=\dfrac{1}{2\mathrm{e}}$，$\dfrac{\partial z}{\partial y}\bigg|_{(\mathrm{e},0)}=-\dfrac12$，所以 $\mathrm{d}z\big|_{(\mathrm{e},0)}=\dfrac{1}{2\mathrm{e}}\mathrm{d}x-\dfrac12\mathrm{d}y$。

+++

#### 基础填空 (7) 设 $\begin{cases}y=f(x,t),\\ F(x,y,t)=0,\end{cases}$ $f,F$ 有一阶连续偏导数，则 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=$________。
***
**$\dfrac{f'_xF'_t-f'_tF'_x}{F'_t+f'_tF'_y}$.**

解　由已知条件，视为方程组确定 $y=y(x)$，$t=t(x)$，方程两边同时对 $x$ 求导，得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=f'_x+f'_t\frac{\mathrm{d}t}{\mathrm{d}x},\quad F'_x+F'_y\cdot\frac{\mathrm{d}y}{\mathrm{d}x}+F'_t\frac{\mathrm{d}t}{\mathrm{d}x}=0,
$$

两式消去 $\dfrac{\mathrm{d}t}{\mathrm{d}x}$，得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{f'_xF'_t-f'_tF'_x}{F'_t+f'_tF'_y}.
$$

+++

#### 基础填空 (8) 设 $y=f(x,t)$，$t=t(x,y)$ 由方程 $G(x,y,t)=0$ 确定，$f,G$ 可微，则 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=$________。
***
**$\dfrac{G'_tf'_x-G'_xf'_t}{G'_yf'_t+G'_t}$.**

解　令 $F(x,y,t)=f(x,t)-y=0$，则 $\begin{cases}F(x,y,t)=0,\\ G(x,y,t)=0\end{cases}$ 确定 $y=y(x)$，$t=t(x)$。

方程组两边同时对 $x$ 求导，得

$$
\begin{cases}F'_x+F'_y\dfrac{\mathrm{d}y}{\mathrm{d}x}+F'_t\dfrac{\mathrm{d}t}{\mathrm{d}x}=f'_x+f'_t\dfrac{\mathrm{d}t}{\mathrm{d}x}-\dfrac{\mathrm{d}y}{\mathrm{d}x}=0,\\[2mm] G'_x+G'_y\dfrac{\mathrm{d}y}{\mathrm{d}x}+G'_t\dfrac{\mathrm{d}t}{\mathrm{d}x}=0,\end{cases}
$$

解方程组，得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{G'_tf'_x-G'_xf'_t}{G'_yf'_t+G'_t}.
$$

+++

#### 基础填空 (9) 设 $z=f\left(\dfrac{y}{x}\right)+g(\mathrm{e}^x,\sin y)$，$f$ 有二阶连续导数，$g$ 有二阶连续偏导数，则 $\dfrac{\partial^2z}{\partial x\partial y}=$________。
***
**$-\dfrac{1}{x^2}f'-\dfrac{y}{x^3}f''+\mathrm{e}^xg''_{12}\cos y$.**

解

$$
\frac{\partial z}{\partial x}=-\frac{y}{x^2}f'+\mathrm{e}^xg'_1,\quad \frac{\partial^2z}{\partial x\partial y}=-\frac{1}{x^2}f'-\frac{y}{x^3}f''+\mathrm{e}^xg''_{12}\cos y.
$$

+++

#### 基础填空 (10) 设 $f(u,v)$ 有二阶连续偏导数，$y=f(\mathrm{e}^x,\cos x)$，则 $\dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}\bigg|_{x=0}=$________。
***
**$f''_{11}(1,1)+f'_1(1,1)-f'_2(1,1)$.**

解

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=f'_1\mathrm{e}^x-f'_2\sin x,
$$

$$
\frac{\mathrm{d}^2y}{\mathrm{d}x^2}=(f''_{11}\mathrm{e}^x-f''_{12}\sin x)\mathrm{e}^x+f'_1\mathrm{e}^x-(f''_{21}\mathrm{e}^x-f''_{22}\sin x)\sin x-f'_2\cos x,
$$

故

$$
\frac{\mathrm{d}^2y}{\mathrm{d}x^2}\bigg|_{x=0}=f''_{11}(1,1)+f'_1(1,1)-f'_2(1,1).
$$

+++

#### 基础填空 (11) 设 $z=z(x,y)$ 由方程 $\mathrm{e}^{2yz}+x+y^2+z=\dfrac74$ 确定，则 $\mathrm{d}z\big|_{\left(\frac12,\frac12\right)}=$________。
***
**$-\dfrac12(\mathrm{d}x+\mathrm{d}y)$.**

解　等式两边同时对 $x,y$ 求偏导，得

$$
\begin{cases}\mathrm{e}^{2yz}\cdot2y\dfrac{\partial z}{\partial x}+1+\dfrac{\partial z}{\partial x}=0,\\[2mm] \mathrm{e}^{2yz}\left(2z+2y\dfrac{\partial z}{\partial y}\right)+2y+\dfrac{\partial z}{\partial y}=0.\end{cases}
$$

当 $x=y=\dfrac12$ 时，$z=0$，代入方程组，解得

$$
\frac{\partial z}{\partial x}\bigg|_{\left(\frac12,\frac12\right)}=-\frac12,\quad \frac{\partial z}{\partial y}\bigg|_{\left(\frac12,\frac12\right)}=-\frac12,
$$

故 $\mathrm{d}z\big|_{\left(\frac12,\frac12\right)}=-\dfrac12(\mathrm{d}x+\mathrm{d}y)$。

+++

#### 基础填空 (12) 设 $f(x,y)=\displaystyle\int_0^{xy}\frac{\sin t}{1+t^2}\mathrm{d}t$，则 $\dfrac{\partial^2f}{\partial x^2}\bigg|_{(0,2)}=$________。
***
**$4$.**

解

$$
\frac{\partial f}{\partial x}=\frac{y\sin xy}{1+(xy)^2},
$$

$$
\frac{\partial^2f}{\partial x^2}\bigg|_{(0,2)}=\left(\frac{2\sin2x}{1+4x^2}\right)'\bigg|_{x=0}=\frac{4(1+4x^2)\cos2x-16x\sin2x}{(1+4x^2)^2}\bigg|_{x=0}=4.
$$

**【注】** 这里先将 $y=2$ 代入再对 $x$ 求导。

+++

#### 基础填空 (13) 设 $z(x,y)$ 的全微分 $\mathrm{d}z=(x^2+2xy-y^2)\mathrm{d}x+(x^2-2xy-y^2)\mathrm{d}y$，则 $z(x,y)=$________。
***
**$\dfrac13x^3+x^2y-xy^2-\dfrac13y^3+C$（$C$ 为任意常数）.**

解　由已知，$\dfrac{\partial z}{\partial x}=x^2+2xy-y^2$，$\dfrac{\partial z}{\partial y}=x^2-2xy-y^2$，故

$$
z=\int(x^2+2xy-y^2)\mathrm{d}x+\varphi(y)=\frac13x^3+x^2y-xy^2+\varphi(y).
$$

又

$$
\frac{\partial z}{\partial y}=x^2-2xy+\varphi'(y)=x^2-2xy-y^2,
$$

得 $\varphi'(y)=-y^2$，积分得 $\varphi(y)=-\dfrac13y^3+C$，其中 $C$ 为任意常数，故

$$
z(x,y)=\frac13x^3+x^2y-xy^2-\frac13y^3+C.
$$

+++

#### 基础填空 (14) 设 $z=z(x,y)$ 由方程 $z+\ln z-\displaystyle\int_y^x\mathrm{e}^{-t^2}\mathrm{d}t=0$ 确定，则 $\dfrac{\partial^2z}{\partial x\partial y}=$________。
***
**$\dfrac{-z\mathrm{e}^{-(x^2+y^2)}}{(1+z)^3}$.**

解　已知方程两边同时对 $x,y$ 求偏导，得

$$
\frac{\partial z}{\partial x}+\frac1z\frac{\partial z}{\partial x}-\mathrm{e}^{-x^2}=0,\quad \frac{\partial z}{\partial y}+\frac1z\frac{\partial z}{\partial y}+\mathrm{e}^{-y^2}=0.
$$

上两式解得 $\dfrac{\partial z}{\partial x}=\dfrac{z\mathrm{e}^{-x^2}}{1+z}$，$\dfrac{\partial z}{\partial y}=\dfrac{-z\mathrm{e}^{-y^2}}{1+z}$，故

$$
\begin{aligned}
\frac{\partial^2z}{\partial x\partial y}&=\frac{\mathrm{e}^{-x^2}\cdot\dfrac{\partial z}{\partial y}\cdot(1+z)-z\mathrm{e}^{-x^2}\cdot\dfrac{\partial z}{\partial y}}{(1+z)^2}\\
&=\frac{\mathrm{e}^{-x^2}}{(1+z)^2}\cdot\left(\frac{-z\mathrm{e}^{-y^2}}{1+z}\right)=\frac{-z\mathrm{e}^{-(x^2+y^2)}}{(1+z)^3}.
\end{aligned}
$$

+++

#### 基础填空 (15) 设 $z=f\left(xy,\dfrac{x}{y}\right)+g\left(\dfrac{y}{x}\right)$，$f$ 具有二阶连续偏导数，$g$ 具有二阶连续导数，则 $\dfrac{\partial^2z}{\partial x\partial y}=$________。
***
**$f'_1-\dfrac{1}{y^2}f'_2+xyf''_{11}-\dfrac{x}{y^3}f''_{22}-\dfrac{1}{x^2}g'-\dfrac{y}{x^3}g''$.**

解

$$
\frac{\partial z}{\partial x}=yf'_1+\frac1yf'_2-\frac{y}{x^2}g',
$$

$$
\begin{aligned}
\frac{\partial^2z}{\partial x\partial y}&=f'_1+y\left(xf''_{11}-\frac{x}{y^2}f''_{12}\right)-\frac{1}{y^2}f'_2+\frac1y\left(xf''_{21}-\frac{x}{y^2}f''_{22}\right)-\frac{1}{x^2}g'-\frac{y}{x^3}g''\\
&=f'_1-\frac{1}{y^2}f'_2+xyf''_{11}-\frac{x}{y^3}f''_{22}-\frac{1}{x^2}g'-\frac{y}{x^3}g''.
\end{aligned}
$$

**【注】** 此题 $g'$ 不能写成 $g'_x$。

+++

#### 基础填空 (16) 曲面 $z=x^2+y^2-1$ 在点 $P(2,1,4)$ 处的切平面方程为________，法线方程为________。
***
**$4x+2y-z-6=0$，$\dfrac{x-2}{4}=\dfrac{y-1}{2}=\dfrac{z-4}{-1}$.**

解　令 $F(x,y,z)=z-x^2-y^2+1$，则法向量为

$$
\boldsymbol{n}=(F'_x(P),F'_y(P),F'_z(P))=(-4,-2,1),
$$

故切平面方程为 $4(x-2)+2(y-1)-(z-4)=0$，即 $4x+2y-z-6=0$。

法线方程为

$$
\frac{x-2}{4}=\frac{y-1}{2}=\frac{z-4}{-1}.
$$

+++

#### 基础填空 (17) 曲线 $L:\begin{cases}x^2+y^2=10,\\ x^2+z^2=10\end{cases}$ 在点 $P(3,1,1)$ 处的切线方程为________，法平面方程为________。
***
**$\dfrac{x-3}{1}=\dfrac{y-1}{-3}=\dfrac{z-1}{-3}$，$x-3y-3z+3=0$.**

解　由 $\begin{cases}x^2+y^2=10,\\ x^2+z^2=10\end{cases}$ 确定函数 $y=y(x)$，$z=z(x)$，视 $x$ 为参数，故曲线 $L$ 的切线的方向向量为 $\boldsymbol{T}=(1,y'(x),z'(x))$。

已知方程组两边同时对 $x$ 求导，得

$$
\begin{cases}2x+2y\dfrac{\mathrm{d}y}{\mathrm{d}x}=0,\\[2mm] 2x+2z\dfrac{\mathrm{d}z}{\mathrm{d}x}=0,\end{cases}
$$

将 $x=3$，$y=1$，$z=1$ 代入上方程组，解得 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=-3$，$\dfrac{\mathrm{d}z}{\mathrm{d}x}=-3$，所以 $\boldsymbol{T}=(1,-3,-3)$，故切线方程为

$$
\frac{x-3}{1}=\frac{y-1}{-3}=\frac{z-1}{-3},
$$

法平面方程为 $(x-3)-3(y-1)-3(z-1)=0$，即 $x-3y-3z+3=0$。

**【注】** 求空间曲线的切线的方向向量时，视为参数方程处理。

+++

#### 基础填空 (18) 设 $\dfrac{(x+ky)\mathrm{d}x+y\mathrm{d}y}{(x+y)^2}$ 为某二元函数的全微分，则 $k=$________。
***
**$2$.**

解　令 $P=\dfrac{x+ky}{(x+y)^2}$，$Q=\dfrac{y}{(x+y)^2}$，依题意，有 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，则

$$
\frac{0-y\cdot2(x+y)}{(x+y)^4}=\frac{k(x+y)^2-(x+ky)\cdot2(x+y)}{(x+y)^4},
$$

比较两边分子，得 $-2y=(k-2)x-ky$，解得 $k=2$。

+++

#### 基础填空 (19) 设 $f(x,y)$ 有连续偏导数，在 $P(1,-2)$ 处有 $f'_x(1,-2)=1$，$f'_y(1,-2)=-1$，则 $f(x,y)$ 在 $P(1,-2)$ 处增加最快的方向为________。
***
**$\boldsymbol{i}-\boldsymbol{j}$.**

解　函数 $f(x,y)$ 在 $P(1,-2)$ 处增加最快的方向是梯度方向，由已知，

$$
\mathbf{grad}\,f(1,-2)=(f'_x(1,-2),f'_y(1,-2))=(1,-1),
$$

故所求方向为 $\boldsymbol{i}-\boldsymbol{j}$。

+++

#### 基础填空 (20) 函数 $u=\ln(x^2+y^2+z^2)$ 在点 $P(1,2,-2)$ 处的梯度 $\mathbf{grad}\,u(P)=$________。
***
**$\dfrac29(1,2,-2)$.**

解

$$
\mathbf{grad}\,u=\frac{\partial u}{\partial x}\boldsymbol{i}+\frac{\partial u}{\partial y}\boldsymbol{j}+\frac{\partial u}{\partial z}\boldsymbol{k}=\frac{1}{x^2+y^2+z^2}(2x\boldsymbol{i}+2y\boldsymbol{j}+2z\boldsymbol{k}),
$$

故

$$
\mathbf{grad}\,u(1,2,-2)=\frac29(1,2,-2).
$$

+++

#### 基础解答 (1) 设 $u=f(x,y,z)$ 有连续偏导数，$y=y(x)$，$z=z(x)$ 分别由方程 $\mathrm{e}^{xy}-y=0$ 和 $\mathrm{e}^z-xz=0$ 确定，求 $\dfrac{\mathrm{d}u}{\mathrm{d}x}$。
***
解

$$
\frac{\mathrm{d}u}{\mathrm{d}x}=f'_1+f'_2\frac{\mathrm{d}y}{\mathrm{d}x}+f'_3\frac{\mathrm{d}z}{\mathrm{d}x}.\qquad ①
$$

方程 $\mathrm{e}^{xy}-y=0$ 两边同时对 $x$ 求导，得 $\mathrm{e}^{xy}\left(y+x\dfrac{\mathrm{d}y}{\mathrm{d}x}\right)-\dfrac{\mathrm{d}y}{\mathrm{d}x}=0$，解得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{y^2}{1-xy}.\qquad ②
$$

方程 $\mathrm{e}^z-xz=0$ 两边同时对 $x$ 求导，得 $\mathrm{e}^z\dfrac{\mathrm{d}z}{\mathrm{d}x}-z-x\dfrac{\mathrm{d}z}{\mathrm{d}x}=0$，解得

$$
\frac{\mathrm{d}z}{\mathrm{d}x}=\frac{z}{xz-x}.\qquad ③
$$

将 ②③ 代入 ①，得

$$
\frac{\mathrm{d}u}{\mathrm{d}x}=f'_1+\frac{y^2}{1-xy}f'_2+\frac{z}{xz-x}f'_3.
$$

+++

#### 基础解答 (2) 设 $y=y(x)$，$z=z(x)$ 由方程组 $\begin{cases}x^2+y^2+z^2=3x,\\ 2x-3y+5z=4\end{cases}$ 确定，求 $\dfrac{\mathrm{d}y}{\mathrm{d}x}$，$\dfrac{\mathrm{d}z}{\mathrm{d}x}$。
***
解　方程组两边同时对 $x$ 求导，得

$$
\begin{cases}2x+2y\dfrac{\mathrm{d}y}{\mathrm{d}x}+2z\dfrac{\mathrm{d}z}{\mathrm{d}x}=3,\\[2mm] 2-3\dfrac{\mathrm{d}y}{\mathrm{d}x}+5\dfrac{\mathrm{d}z}{\mathrm{d}x}=0,\end{cases}
$$

解方程组，得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{\begin{vmatrix}3-2x&2z\\-2&5\end{vmatrix}}{\begin{vmatrix}2y&2z\\-3&5\end{vmatrix}}=-\frac{10x-4z-15}{2(5y+3z)},
$$

$$
\frac{\mathrm{d}z}{\mathrm{d}x}=\frac{\begin{vmatrix}2y&3-2x\\-3&-2\end{vmatrix}}{\begin{vmatrix}2y&2z\\-3&5\end{vmatrix}}=-\frac{6x+4y-9}{2(5y+3z)}.
$$

+++

#### 基础解答 (3) 设曲面 $S:(x-y)^2-z^2=1$，求坐标原点到 $S$ 的最短距离。
***
解　设 $S$ 上任一点为 $(x,y,z)$，则 $(0,0,0)$ 到 $(x,y,z)$ 的距离的平方为

$$
d^2=x^2+y^2+z^2.
$$

令 $L=x^2+y^2+z^2+\lambda[(x-y)^2-z^2-1]$，则

$$
\begin{cases}L'_x=2x+2\lambda(x-y)=0,&①\\ L'_y=2y-2\lambda(x-y)=0,&②\\ L'_z=2z-2\lambda z=0,&③\\ L'_\lambda=(x-y)^2-z^2-1=0.&④\end{cases}
$$

由 ① 和 ②，得 $x=-y$，由 ③ 得 $z=0$ 或 $\lambda=1$。

若 $\lambda=1$，由 ①②，知 $x=y=0$，与 ④ 矛盾，舍去，故 $z=0$。由 ④，可得 $x^2=\dfrac14$，解得驻点 $\left(\dfrac12,-\dfrac12,0\right)$，$\left(-\dfrac12,\dfrac12,0\right)$，故所求最短距离为

$$
d=\sqrt{\left(\frac12\right)^2+\left(-\frac12\right)^2+0^2}=\frac{\sqrt2}{2}.
$$

+++

#### 基础解答 (4) 求平面 $\dfrac{x}{3}+\dfrac{y}{4}+\dfrac{z}{5}=1$ 和柱面 $x^2+y^2=1$ 的交线上与 $xOy$ 平面距离最短的点。
***
解　依题意，平面与柱面的交线在 $xOy$ 面的上方，故归纳为求 $z=5\left(1-\dfrac{x}{3}-\dfrac{y}{4}\right)$ 在条件 $x^2+y^2=1$ 下的极值。

利用拉格朗日乘数法，令 $L=5\left(1-\dfrac{x}{3}-\dfrac{y}{4}\right)+\lambda(x^2+y^2-1)$，则

$$
\begin{cases}L'_x=-\dfrac53+2\lambda x=0,\\[2mm] L'_y=-\dfrac54+2\lambda y=0,\\[2mm] L'_\lambda=x^2+y^2-1=0,\end{cases}
$$

解方程组，得 $\left(\dfrac45,\dfrac35\right)$，$\left(-\dfrac45,-\dfrac35\right)$。

根据题设的实际意义，存在最小值，比较 $z\left(\dfrac45,\dfrac35\right)=\dfrac{35}{12}$，$z\left(-\dfrac45,-\dfrac35\right)=\dfrac{85}{12}$，知距离最短的点为 $\left(\dfrac45,\dfrac35,\dfrac{35}{12}\right)$。

+++

#### 基础解答 (5) 求双曲线 $xy=4$ 与直线 $2x+y=1$ 之间的最短距离。
***
解　在 $xy=4$ 上任取一点 $P(x,y)$，则点 $P$ 到直线 $2x+y=1$ 的距离为

$$
d=\frac{|2x+y-1|}{\sqrt5},
$$

只需求 $d^2=\dfrac{(2x+y-1)^2}{5}$ 的最小值。

利用拉格朗日乘数法，令 $L=\dfrac15(2x+y-1)^2+\lambda(xy-4)$，则

$$
\begin{cases}L'_x=\dfrac45(2x+y-1)+\lambda y=0,\\[2mm] L'_y=\dfrac25(2x+y-1)+\lambda x=0,\\[2mm] L'_\lambda=xy-4=0,\end{cases}
$$

解方程组，得驻点 $(\sqrt2,2\sqrt2)$，$(-\sqrt2,-2\sqrt2)$。比较

$$
d(\sqrt2,2\sqrt2)=\frac{1}{\sqrt5}(4\sqrt2-1),\quad d(-\sqrt2,-2\sqrt2)=\frac{1}{\sqrt5}(1+4\sqrt2),
$$

得最短距离为 $\dfrac{1}{\sqrt5}(4\sqrt2-1)$。

+++

#### 基础解答 (6) 求函数 $z=x^3-3x^2-3y^2$ 在闭区域 $D:x^2+y^2\leqslant16$ 上的最大值。
***
解　（Ⅰ）在 $D:x^2+y^2<16$ 内。由 $\begin{cases}z'_x=3x^2-6x=0,\\ z'_y=-6y=0,\end{cases}$ 得驻点 $(0,0)$，$(2,0)$。

（Ⅱ）在 $D:x^2+y^2=16$ 上。利用拉格朗日乘数法，令 $L=x^3-3x^2-3y^2+\lambda(x^2+y^2-16)$，则

$$
\begin{cases}L'_x=3x^2-6x+2\lambda x=0,\\ L'_y=-6y+2\lambda y=0,\\ L'_\lambda=x^2+y^2-16=0,\end{cases}
$$

解得 $(0,\pm4)$，$(\pm4,0)$。

（Ⅲ）比较大小

$$
z(0,0)=0,\ z(2,0)=-4,\ z(0,4)=-48,
$$

$$
z(0,-4)=-48,\ z(4,0)=16,\ z(-4,0)=-112,
$$

得最大值为 $z(4,0)=16$。

**【注】** 在 $D:x^2+y^2=16$ 上，考虑到 $z=x^3-3x^2-3y^2$ 中含 $x^2+y^2$，可以化为一元函数极值问题。

将 $y^2=16-x^2$ 代入 $z=x^3-3x^2-3y^2$，得 $z=x^3-48\ (-4\leqslant x\leqslant4)$。

又由 $\dfrac{\mathrm{d}z}{\mathrm{d}x}=3x^2=0$，解得 $x=0$，则可得 $y=\pm4$。又因为 $x=\pm4$ 时，$y=0$，所以在 $D$ 边界上可能的最值点有 $(0,4)$，$(0,-4)$，$(4,0)$，$(-4,0)$。

+++

#### 基础解答 (7) 设椭圆 $\begin{cases}z=x^2+y^2,\\ x+y+z=4\end{cases}$ 上的点 $(x,y,z)$ 到原点的距离为 $d$，求其最值以及使得 $d$ 取最大和最小的点。
***
解　依题意，知 $d=\sqrt{x^2+y^2+z^2}$，$d^2=x^2+y^2+z^2$。

问题转化为求 $x^2+y^2+z^2$ 在条件 $z=x^2+y^2$ 和 $x+y+z=4$ 下的最值。利用拉格朗日乘数法，令 $L=x^2+y^2+z^2+\lambda_1(z-x^2-y^2)+\lambda_2(x+y+z-4)$，则

$$
\begin{cases}L'_x=2x-2\lambda_1x+\lambda_2=0,&①\\ L'_y=2y-2\lambda_1y+\lambda_2=0,&②\\ L'_z=2z+\lambda_1+\lambda_2=0,&③\\ L'_{\lambda_1}=z-x^2-y^2=0,&④\\ L'_{\lambda_2}=x+y+z-4=0.&⑤\end{cases}
$$

考虑到 $L$ 关于 $x$ 与 $y$ 具有轮换性，方程组有 $x=y$ 解，将 $x=y$ 代入 ④ 与 ⑤，解得 $(-2,-2,8)$，$(1,1,2)$，故最大值为 $\sqrt{(-2)^2+(-2)^2+8^2}=6\sqrt2$，最小值为 $\sqrt{1^2+1^2+2^2}=\sqrt6$。

**【注】** ① 此题有两个约束条件 $\begin{cases}z=x^2+y^2,\\ x+y+z=4,\end{cases}$ 可将 $z$ 消去化为一个约束条件 $x+y+x^2+y^2=4$，问题转化为求 $x^2+y^2+(4-x-y)^2$ 在约束条件 $x+y+x^2+y^2=4$ 下的最值。

② 此题也可利用微分解决。求 $u=x^2+y^2+z^2$ 在 $\begin{cases}z=x^2+y^2,\\ x+y+z=4\end{cases}$ 下的条件极值。可令全微分 $\mathrm{d}u=0$，并将约束条件两边微分整理得

$$
\begin{cases}2x\mathrm{d}x+2y\mathrm{d}y+2z\mathrm{d}z=0,\\ 2x\mathrm{d}x+2y\mathrm{d}y-\mathrm{d}z=0,\\ \mathrm{d}x+\mathrm{d}y+\mathrm{d}z=0.\end{cases}
$$

由于 $\mathrm{d}x,\mathrm{d}y,\mathrm{d}z$ 不全为零，故上面方程组有非零解，于是

$$
\begin{vmatrix}2x&2y&2z\\2x&2y&-1\\1&1&1\end{vmatrix}=0,
$$

将行列式展开并化简，有 $2(x-y)(2z+1)=0$。又由题意可知 $z\geqslant0$，故 $x=y$，将 $x=y$ 代入 $z=x^2+y^2$ 和 $x+y+z=4$，解得两点分别为 $(1,1,2)$ 和 $(-2,-2,8)$。

+++

#### 基础解答 (8) 设 $u(x,y)$ 有二阶连续偏导数，利用变换 $\xi=x+ay$，$\eta=x+by$，将方程 $\dfrac{\partial^2u}{\partial x^2}+4\dfrac{\partial^2u}{\partial x\partial y}+3\dfrac{\partial^2u}{\partial y^2}=0$ 化为 $\dfrac{\partial^2u}{\partial\xi\partial\eta}=0$，求 $a,b$ 的值。
***
解　视 $\xi,\eta$ 为中间变量，$x,y$ 为自变量。

由已知，得

$$
\begin{cases}\dfrac{\partial u}{\partial x}=\dfrac{\partial u}{\partial\xi}\cdot1+\dfrac{\partial u}{\partial\eta}\cdot1,\\[2mm] \dfrac{\partial u}{\partial y}=\dfrac{\partial u}{\partial\xi}\cdot a+\dfrac{\partial u}{\partial\eta}\cdot b,\end{cases}
$$

这里 $\dfrac{\partial u}{\partial\xi},\dfrac{\partial u}{\partial\eta}$ 是以 $\xi,\eta$ 为中间变量、$x,y$ 为自变量的二元函数，故

$$
\frac{\partial^2u}{\partial x^2}=\frac{\partial^2u}{\partial\xi^2}+2\frac{\partial^2u}{\partial\xi\partial\eta}+\frac{\partial^2u}{\partial\eta^2},
$$

$$
\frac{\partial^2u}{\partial y^2}=a^2\frac{\partial^2u}{\partial\xi^2}+2ab\frac{\partial^2u}{\partial\xi\partial\eta}+b^2\frac{\partial^2u}{\partial\eta^2},
$$

$$
\frac{\partial^2u}{\partial x\partial y}=a\frac{\partial^2u}{\partial\xi^2}+(a+b)\frac{\partial^2u}{\partial\xi\partial\eta}+b\frac{\partial^2u}{\partial\eta^2},
$$

代入已知方程，得

$$
\begin{aligned}
&\frac{\partial^2u}{\partial x^2}+4\frac{\partial^2u}{\partial x\partial y}+3\frac{\partial^2u}{\partial y^2}\\
&=(1+4a+3a^2)\frac{\partial^2u}{\partial\xi^2}+[2+4(a+b)+6ab]\frac{\partial^2u}{\partial\xi\partial\eta}+(1+4b+3b^2)\frac{\partial^2u}{\partial\eta^2}.
\end{aligned}
$$

又由已知，得

$$
\begin{cases}1+4a+3a^2=0,&①\\ 1+4b+3b^2=0,&②\\ 2+4(a+b)+6ab\neq0,&③\end{cases}
$$

联立 ① 式和 ② 式，解得

$$
\begin{cases}a=-1,\\ b=-\dfrac13\end{cases}\quad\text{或}\quad\begin{cases}a=-\dfrac13,\\ b=-1,\end{cases}
$$

且都满足 ③ 式，故为所求。

+++

#### 基础解答 (9) 设 $f(u)$ 有二阶连续导数，且 $z=f(\mathrm{e}^x\sin y)$ 满足 $\dfrac{\partial^2z}{\partial x^2}+\dfrac{\partial^2z}{\partial y^2}=z\mathrm{e}^{2x}$，求 $f(u)$。
***
解　令 $\mathrm{e}^x\sin y=u$，则

$$
\frac{\partial z}{\partial x}=f'(u)\mathrm{e}^x\sin y,\quad \frac{\partial z}{\partial y}=f'(u)\mathrm{e}^x\cos y,
$$

$$
\frac{\partial^2z}{\partial x^2}=f'(u)\mathrm{e}^x\sin y+f''(u)\mathrm{e}^{2x}\sin^2y,
$$

$$
\frac{\partial^2z}{\partial y^2}=-f'(u)\mathrm{e}^x\sin y+f''(u)\mathrm{e}^{2x}\cos^2y,
$$

代入原方程，得 $f''(u)-f(u)=0$，此为二阶齐次线性微分方程，解得

$$
f(u)=C_1\mathrm{e}^u+C_2\mathrm{e}^{-u}\quad(C_1,C_2\ \text{为任意常数}).
$$

+++

#### 综合选择 (1) 设 $f(x,y)$ 在点 $(x_0,y_0)$ 处不可微，则下列命题一定**不成立**的是（　）。

;;;
A. $f(x,y)$ 在点 $(x_0,y_0)$ 处不连续
B. $f(x,y)$ 在点 $(x_0,y_0)$ 处两个偏导数均存在且偏导数连续
C. $f(x,y)$ 在点 $(x_0,y_0)$ 处两个偏导数均存在且至少有一个不连续
D. $f(x,y)$ 在点 $(x_0,y_0)$ 处沿任何方向的方向导数均不存在
;;;B
***
**B.**

解　四个选项中，只有 B 是 $f(x,y)$ 在点 $(x_0,y_0)$ 处可微的充分条件，故 B 一定不成立。

+++

#### 综合选择 (2) 设 $f(x,y)$ 在点 $(0,0)$ 处连续，且 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)}{\mathrm{e}^{x^2+y^2}-1}=1$，则（　）。

;;;
A. $f(x,y)$ 在点 $(0,0)$ 处取得极小值
B. $f(x,y)$ 在点 $(0,0)$ 处取得极大值
C. $f(x,y)$ 在点 $(0,0)$ 处不取得极值
D. 不能确定 $f(x,y)$ 在点 $(0,0)$ 处取得极值
;;;A
***
**A.**

解　利用保号性和极值的定义。

由 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)}{\mathrm{e}^{x^2+y^2}-1}=1$，知 $\lim\limits_{\substack{x\to0\\ y\to0}}f(x,y)=0=f(0,0)$。

又由保号性，知在点 $(0,0)$ 的去心邻域内有 $f(x,y)>0=f(0,0)$。由极值的定义，可知 $f(x,y)$ 在点 $(0,0)$ 处取得极小值，故 A 正确。

+++

#### 综合选择 (3) 设 $f(x,y)$ 在点 $(0,0)$ 的某邻域内连续，且 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)-f(0,0)}{|x|+y^4}=-1$，则 $f(x,y)$ 在点 $(0,0)$ 处（　）。

;;;
A. 取得极小值
B. 取得极大值
C. 不取得极值
D. 无法确定是否取得极值
;;;B
***
**B.**

解　在点 $(0,0)$ 的去心邻域内有 $|x|+y^4>0$，则由保号性，可知 $f(x,y)-f(0,0)<0$，再由极值的定义，可知 $f(x,y)$ 在点 $(0,0)$ 处取得极大值，故 B 正确。

+++

#### 综合选择 (4) 设 $f(x,y)=\begin{cases}y\arctan\dfrac{1}{\sqrt{x^2+y^2}},&(x,y)\neq(0,0),\\[2mm] 0,&(x,y)=(0,0),\end{cases}$ 则 $f(x,y)$ 在点 $(0,0)$ 处（　）。

;;;
A. 连续但不可微
B. 偏导数存在但不连续
C. 可微
D. 连续但偏导数不存在
;;;C
***
**C.**

解　由 $\arctan\dfrac{1}{\sqrt{x^2+y^2}}$ 有界，知

$$
\lim_{\substack{x\to0\\ y\to0}}f(x,y)=\lim_{\substack{x\to0\\ y\to0}}y\arctan\frac{1}{\sqrt{x^2+y^2}}=0=f(0,0),
$$

故 $f(x,y)$ 在点 $(0,0)$ 处连续。

$$
f'_x(0,0)=\lim_{x\to0}\frac{f(x,0)-f(0,0)}{x}=\lim_{x\to0}\frac{0}{x}=0,
$$

$$
f'_y(0,0)=\lim_{y\to0}\frac{f(0,y)-f(0,0)}{y}=\lim_{y\to0}\arctan\frac{1}{|y|}=\frac{\pi}{2},
$$

$$
\frac{\Delta f-\mathrm{d}f}{\rho}=\frac{f(x,y)-f(0,0)-[f'_x(0,0)x+f'_y(0,0)y]}{\rho}=\frac{y\arctan\dfrac{1}{\sqrt{x^2+y^2}}-\left[0\cdot x+\dfrac{\pi}{2}\cdot y\right]}{\sqrt{x^2+y^2}},
$$

由于 $\left|\dfrac{y}{\sqrt{x^2+y^2}}\right|\leqslant1$，故

$$
\lim_{\substack{x\to0\\ y\to0}}\frac{\Delta f-\mathrm{d}f}{\rho}=\lim_{\substack{x\to0\\ y\to0}}\frac{y}{\sqrt{x^2+y^2}}\left(\arctan\frac{1}{\sqrt{x^2+y^2}}-\frac{\pi}{2}\right)=0,
$$

所以 $f(x,y)$ 在点 $(0,0)$ 处可微，故 C 正确。

+++

#### 综合选择 (5) 设 $f(x,y)$ 在点 $(0,0)$ 的某邻域内有定义，$f(0,0)=0$，且 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)-\sqrt{x^2+y^2}}{\sqrt{x^2+y^2}}=k$（$k$ 为常数），则当 $k>-1$ 时，（　）。

;;;
A. $f(x,y)$ 在点 $(0,0)$ 处可微
B. $f(x,y)$ 在点 $(0,0)$ 处取得极小值
C. $f(x,y)$ 在点 $(0,0)$ 处取得极大值
D. $f'_x(0,0)$，$f'_y(0,0)$ 都存在
;;;B
***
**B.**

解　由已知条件及极限与无穷小的关系，有

$$
\frac{f(x,y)-\sqrt{x^2+y^2}}{\sqrt{x^2+y^2}}=k+\alpha\quad(\alpha\to0),
$$

即 $f(x,y)=(1+k)\sqrt{x^2+y^2}+o(\rho)$，$\rho=\sqrt{x^2+y^2}$，则在点 $(0,0)$ 处，$f(x,y)$ 沿任何方向 $\boldsymbol{l}=\cos\alpha\boldsymbol{i}+\cos\beta\boldsymbol{j}$ 的方向导数都存在，且

$$
\frac{\partial f(x,y)}{\partial l}\bigg|_{(0,0)}=\lim_{t\to0^+}\frac{f(t\cos\alpha,t\sin\alpha)-f(0,0)}{t}=\lim_{t\to0^+}\frac{(1+k)t+o(t)}{t}=1+k,
$$

故当 $\dfrac{\partial f(x,y)}{\partial l}\bigg|_{(0,0)}=1+k>0$ 时，$f(x,y)$ 在点 $(0,0)$ 处取得极小值，B 正确。

**【注】** ① 由 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)-\sqrt{x^2+y^2}}{\sqrt{x^2+y^2}}=k$ 及 $f(0,0)=0$，得 $\lim\limits_{\substack{x\to0\\ y\to0}}f(x,y)=f(0,0)=0$。

② $\boldsymbol{l}=\cos\alpha\boldsymbol{i}+\cos\beta\boldsymbol{j}=\cos\alpha\boldsymbol{i}+\sin\alpha\boldsymbol{j}$，如图 5-1 所示，$\alpha+\beta=\dfrac{\pi}{2}$。$\boldsymbol{l}$ 所在直线方程的参数式为 $\begin{cases}x=t\cos\alpha,\\ y=t\sin\alpha.\end{cases}$

③

$$
\lim_{x\to0}\frac{f(x,0)-f(0,0)}{x}=\lim_{x\to0}\frac{(1+k)\sqrt{x^2}+o(x)}{x}=\lim_{x\to0}\left[(1+k)\frac{|x|}{x}+\frac{o(x)}{x}\right].
$$

当 $k>-1$ 时，上述极限不存在，故 $f'_x(0,0)$ 不存在，同样 $f'_y(0,0)$ 不存在，所以 $f(x,y)$ 在点 $(0,0)$ 处不可微。可排除 A，D。

④ $f(x,y)$ 在点 $(0,0)$ 处沿任何方向的方向导数都大于零（小于零），则 $f(x,y)$ 在点 $(0,0)$ 处取得极小（大）值。

+++

#### 综合选择 (6) 设 $f(x,y)$ 可微，对任意的 $x,y$，有 $\dfrac{\partial f(x,y)}{\partial x}>0$，$\dfrac{\partial f(x,y)}{\partial y}<0$，则使得 $f(x_1,y_1)<f(x_2,y_2)$ 成立的一个充分条件是（　）。

;;;
A. $x_1<x_2$，$y_1>y_2$
B. $x_1>x_2$，$y_1>y_2$
C. $x_1<x_2$，$y_1<y_2$
D. $x_1>x_2$，$y_1<y_2$
;;;A
***
**A.**

解　由 $\dfrac{\partial f(x,y)}{\partial x}>0$，知 $f(x,y)$ 关于 $x$ 单调增加；由 $\dfrac{\partial f(x,y)}{\partial y}<0$，知 $f(x,y)$ 关于 $y$ 单调减少，故当 $x_1<x_2$，$y_1>y_2$ 时，有

$$
f(x_1,y_1)<f(x_2,y_1),\quad f(x_2,y_1)<f(x_2,y_2),
$$

即 $f(x_1,y_1)<f(x_2,y_1)<f(x_2,y_2)$，故 A 正确。

+++

#### 综合选择 (7) 设 $F(x,y)$ 在点 $(x_0,y_0)$ 的某邻域内有二阶连续偏导数，且 $F(x_0,y_0)=0$，$F'_x(x_0,y_0)=0$，$F'_y(x_0,y_0)>0$，$F''_{xx}(x_0,y_0)<0$，则由方程 $F(x,y)=0$ 确定的隐函数 $y=y(x)$ 在 $x=x_0$ 处（　）。

;;;
A. 取得极小值
B. 取得极大值
C. 不取得极值
D. 不能确定是否取得极值
;;;A
***
**A.**

解　由 $F'_x(x_0,y_0)=0$，得 $\dfrac{\mathrm{d}y}{\mathrm{d}x}\bigg|_{x=x_0}=-\dfrac{F'_x(x_0,y_0)}{F'_y(x_0,y_0)}=0$，故 $x=x_0$ 是 $y=y(x)$ 的驻点。

$F(x,y)=0$ 两边对 $x$ 求导，得 $F'_x(x,y)+F'_y(x,y)\cdot\dfrac{\mathrm{d}y}{\mathrm{d}x}=0$。再对 $x$ 求导，得

$$
F''_{xx}(x,y)+F''_{xy}(x,y)\cdot\frac{\mathrm{d}y}{\mathrm{d}x}+\left[F''_{yx}(x,y)+F''_{yy}(x,y)\frac{\mathrm{d}y}{\mathrm{d}x}\right]\frac{\mathrm{d}y}{\mathrm{d}x}+F'_y(x,y)\frac{\mathrm{d}^2y}{\mathrm{d}x^2}=0.
$$

将 $(x_0,y_0)$ 代入上式，解得 $\dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}\bigg|_{x=x_0}=-\dfrac{F''_{xx}(x_0,y_0)}{F'_y(x_0,y_0)}>0$，故 $y=y(x)$ 在 $x=x_0$ 处取得极小值，A 正确。

+++

#### 综合填空 (1) 设 $z=z(x,y)$ 满足 $\dfrac{\partial^2z}{\partial y^2}=2$，且 $z(x,0)=1$，$z'_y(x,0)=x$，则 $z(x,y)=$________。
***
**$y^2+xy+1$.**

解　$\dfrac{\partial^2z}{\partial y^2}=2$，两边同时对 $y$ 积分，得

$$
\frac{\partial z}{\partial y}=\int2\mathrm{d}y+\varphi(x)=2y+\varphi(x),
$$

由 $z'_y(x,0)=x$，得 $\varphi(x)=x$，故 $\dfrac{\partial z}{\partial y}=2y+x$，两边再同时对 $y$ 积分，得

$$
z=\int(2y+x)\mathrm{d}y+\varphi_1(x)=y^2+xy+\varphi_1(x).
$$

又由 $z(x,0)=1$，得 $\varphi_1(x)=1$，于是 $z(x,y)=y^2+xy+1$。

+++

#### 综合填空 (2) 设 $z=z(x,y)$ 有二阶连续偏导数，满足 $\dfrac{\partial^2z}{\partial y\partial x}=x+y$，且 $z(x,0)=x$，$z(0,y)=y^2$，则 $z(x,y)=$________。
***
**$\dfrac12x^2y+\dfrac12xy^2+x+y^2$.**

解　$\dfrac{\partial^2z}{\partial y\partial x}=x+y$，两边同时对 $x$ 积分，得

$$
\frac{\partial z}{\partial y}=\int(x+y)\mathrm{d}x+\varphi(y)=\frac12x^2+xy+\varphi(y),
$$

由 $z(0,y)=y^2$，有 $\dfrac{\mathrm{d}(y^2)}{\mathrm{d}y}=\varphi(y)$，故 $\varphi(y)=2y$。

又由 $\dfrac{\partial z}{\partial y}=\dfrac12x^2+xy+2y$，两端同时对 $y$ 积分，得 $z=\dfrac12x^2y+\dfrac12xy^2+y^2+\varphi_1(x)$，由于 $z(x,0)=x$，故 $\varphi_1(x)=x$，所以

$$
z(x,y)=\frac12x^2y+\frac12xy^2+x+y^2.
$$

+++

#### 综合填空 (3) 设 $z=\dfrac{2x}{x^2-y^2}$，则 $\dfrac{\partial^nz}{\partial y^n}\bigg|_{(2,1)}=$________。
***
**$n!\left[1+\dfrac{(-1)^n}{3^{n+1}}\right]$.**

解　$z=\dfrac{2x}{x^2-y^2}=\dfrac{1}{x+y}-\dfrac{1}{y-x}$，利用 $\left(\dfrac1x\right)^{(n)}=(-1)^n\dfrac{n!}{x^{n+1}}$，有

$$
\frac{\partial^nz}{\partial y^n}=(-1)^n\frac{n!}{(x+y)^{n+1}}-(-1)^n\frac{n!}{(y-x)^{n+1}},
$$

故

$$
\frac{\partial^nz}{\partial y^n}\bigg|_{(2,1)}=(-1)^n\frac{n!}{3^{n+1}}-(-1)^n\frac{n!}{(-1)^{n+1}}=n!\left[1+\frac{(-1)^n}{3^{n+1}}\right].
$$

+++

#### 综合填空 (4) 设曲面 $x^2+2y^2+3z^2=21$ 的切平面平行于平面 $x+4y+6z=0$，则该切平面方程为________。
***
**$x+4y+6z=21$ 或 $x+4y+6z=-21$.**

解　令 $F(x,y,z)=x^2+2y^2+3z^2-21$，则 $F'_x=2x$，$F'_y=4y$，$F'_z=6z$，法向量为

$$
\boldsymbol{n}=(F'_x,F'_y,F'_z)=(2x,4y,6z).
$$

设切点为 $(x_0,y_0,z_0)$，于是曲面 $F(x,y,z)=0$ 在该点处的切平面方程为

$$
x_0(x-x_0)+2y_0(y-y_0)+3z_0(z-z_0)=0.
$$

由已知，该切平面与 $x+4y+6z=0$ 平行，故有 $\dfrac{x_0}{1}=\dfrac{2y_0}{4}=\dfrac{3z_0}{6}\xlongequal{\text{记}}\lambda$，解得 $x_0=\lambda$，$y_0=2\lambda$，$z_0=2\lambda$。

又切点在曲面上，故 $\lambda^2+2(2\lambda)^2+3(2\lambda)^2=21$，解得 $\lambda=\pm1$。对应于 $\lambda=1$，切点为 $(1,2,2)$；对应于 $\lambda=-1$，切点为 $(-1,-2,-2)$。

所求切平面方程为

$$
(x-1)+4(y-2)+6(z-2)=0,\quad (x+1)+4(y+2)+6(z+2)=0,
$$

即 $x+4y+6z=21$ 或 $x+4y+6z=-21$。

+++

#### 综合填空 (5) 设可微函数 $f(x,y)$ 对任意 $x,y,t$，满足 $f(tx,ty)=t^2f(x,y)$，$P_0(1,-2,2)$ 是曲面 $z=f(x,y)$ 上一点，且 $f'_x(1,-2)=4$，则曲面在 $P_0$ 点处的切平面方程为________。
***
**$4x-z-2=0$.**

解　依题设，只需求法向量 $\boldsymbol{n}=(f'_x,f'_y,-1)$。

$f(tx,ty)=t^2f(x,y)$ 两边同时对 $t$ 求导，得 $xf'_1(tx,ty)+yf'_2(tx,ty)=2tf(x,y)$，令 $t=1$，则上式为

$$
xf'_1(x,y)+yf'_2(x,y)=2f(x,y).
$$

将 $x=1$，$y=-2$，$z=f(1,-2)=2$，$f'_1(1,-2)=4$ 代入上式，得 $f'_2(1,-2)=0$，即 $f'_y(1,-2)=0$，故法向量为 $\boldsymbol{n}=(4,0,-1)$，所求切平面方程为

$$
4(x-1)+0\cdot(y+2)+(-1)(z-2)=0,
$$

即 $4x-z-2=0$。

+++

#### 综合填空 (6) 设 $u(x,y,z)=1+\dfrac{x^2}{6}+\dfrac{y^2}{12}+\dfrac{z^2}{18}$，$\boldsymbol{n}=\dfrac{1}{\sqrt3}(1,1,1)$，则 $\dfrac{\partial u}{\partial n}\bigg|_{(1,2,3)}=$________。
***
**$\dfrac{\sqrt3}{3}$.**

解　$\dfrac{\partial u}{\partial x}=\dfrac{x}{3}$，$\dfrac{\partial u}{\partial y}=\dfrac{y}{6}$，$\dfrac{\partial u}{\partial z}=\dfrac{z}{9}$，$\boldsymbol{n}$ 为单位向量，故

$$
\frac{\partial u}{\partial n}\bigg|_{(1,2,3)}=\frac13\times\frac{1}{\sqrt3}+\frac13\times\frac{1}{\sqrt3}+\frac13\times\frac{1}{\sqrt3}=\frac{\sqrt3}{3}.
$$

+++

#### 综合填空 (7) 设 $u(x,y,z)=xy^2z^3$ 在点 $P(1,2,-1)$ 处沿曲面 $x^2+y^2=5$ 的外法线方向的方向导数为________。
***
**$-\dfrac{12}{5}\sqrt5$.**

解　令 $F=x^2+y^2-5$，外法线方向 $\boldsymbol{n}=(2x,2y,0)$，则曲面在点 $P(1,2,-1)$ 处 $\boldsymbol{n}$ 的方向余弦为

$$
\cos\alpha=\frac{1}{\sqrt5},\quad \cos\beta=\frac{2}{\sqrt5},\quad \cos\gamma=0.
$$

又 $\dfrac{\partial u}{\partial x}\bigg|_P=-4$，$\dfrac{\partial u}{\partial y}\bigg|_P=-4$，$\dfrac{\partial u}{\partial z}\bigg|_P=12$，故

$$
\frac{\partial u}{\partial n}\bigg|_P=(-4)\times\frac{1}{\sqrt5}+(-4)\times\frac{2}{\sqrt5}+12\times0=-\frac{12}{5}\sqrt5.
$$

+++

#### 综合解答 (1) 已知 $x+y-z=\mathrm{e}^z$，$x\mathrm{e}^x=\tan t$，$y=\cos t$，求 $\dfrac{\mathrm{d}^2z}{\mathrm{d}t^2}\bigg|_{t=0}$。
***
解　此题是隐函数与复合函数求导的综合题。

由 $x\mathrm{e}^x=\tan t$，可知 $x$ 是 $t$ 的函数，同理 $y=\cos t$，$y$ 也是 $t$ 的函数，再由 $x+y-z=\mathrm{e}^z$，可知 $z$ 是 $t$ 的一元函数。

方程 $x+y-z=\mathrm{e}^z$ 两边同时对 $t$ 求导，得 $\dfrac{\mathrm{d}x}{\mathrm{d}t}+\dfrac{\mathrm{d}y}{\mathrm{d}t}-\dfrac{\mathrm{d}z}{\mathrm{d}t}=\mathrm{e}^z\cdot\dfrac{\mathrm{d}z}{\mathrm{d}t}$，故

$$
\frac{\mathrm{d}z}{\mathrm{d}t}=\frac{1}{1+\mathrm{e}^z}\left(\frac{\mathrm{d}x}{\mathrm{d}t}+\frac{\mathrm{d}y}{\mathrm{d}t}\right).
$$

再求导，得 $\dfrac{\mathrm{d}^2x}{\mathrm{d}t^2}+\dfrac{\mathrm{d}^2y}{\mathrm{d}t^2}-\dfrac{\mathrm{d}^2z}{\mathrm{d}t^2}=\mathrm{e}^z\left(\dfrac{\mathrm{d}z}{\mathrm{d}t}\right)^2+\mathrm{e}^z\dfrac{\mathrm{d}^2z}{\mathrm{d}t^2}$，故

$$
\begin{aligned}
\frac{\mathrm{d}^2z}{\mathrm{d}t^2}&=\frac{1}{1+\mathrm{e}^z}\left[\frac{\mathrm{d}^2x}{\mathrm{d}t^2}+\frac{\mathrm{d}^2y}{\mathrm{d}t^2}-\mathrm{e}^z\left(\frac{\mathrm{d}z}{\mathrm{d}t}\right)^2\right]\\
&=\frac{1}{1+\mathrm{e}^z}\left[\frac{\mathrm{d}^2x}{\mathrm{d}t^2}+\frac{\mathrm{d}^2y}{\mathrm{d}t^2}-\mathrm{e}^z\cdot\frac{1}{(1+\mathrm{e}^z)^2}\left(\frac{\mathrm{d}x}{\mathrm{d}t}+\frac{\mathrm{d}y}{\mathrm{d}t}\right)^2\right].\qquad ①
\end{aligned}
$$

而 $\dfrac{\mathrm{d}y}{\mathrm{d}t}=-\sin t$，$\dfrac{\mathrm{d}^2y}{\mathrm{d}t^2}=-\cos t$，

又由 $x\mathrm{e}^x=\tan t$，得 $\mathrm{e}^x\dfrac{\mathrm{d}x}{\mathrm{d}t}+x\mathrm{e}^x\dfrac{\mathrm{d}x}{\mathrm{d}t}=\sec^2t$，再对 $t$ 求导，得

$$
\mathrm{e}^x\left(\frac{\mathrm{d}x}{\mathrm{d}t}\right)^2+\mathrm{e}^x\frac{\mathrm{d}^2x}{\mathrm{d}t^2}+\mathrm{e}^x\left(\frac{\mathrm{d}x}{\mathrm{d}t}\right)^2+x\mathrm{e}^x\left(\frac{\mathrm{d}x}{\mathrm{d}t}\right)^2+x\mathrm{e}^x\frac{\mathrm{d}^2x}{\mathrm{d}t^2}=2\sec^2t\cdot\tan t,
$$

故

$$
\frac{\mathrm{d}x}{\mathrm{d}t}=\frac{\sec^2t}{(1+x)\mathrm{e}^x},\quad \frac{\mathrm{d}^2x}{\mathrm{d}t^2}=\frac{\sec^2t[2\mathrm{e}^x(1+x)^2\tan t-(2+x)\sec^2t]}{(1+x)^3\mathrm{e}^{2x}}.
$$

当 $t=0$ 时，由 $x\mathrm{e}^x=0$，得 $x=0$，而 $y=\cos0=1$。将 $x=0$，$y=1$ 代入 $x+y-z=\mathrm{e}^z$，得 $z=0$，故

$$
\frac{\mathrm{d}x}{\mathrm{d}t}\bigg|_{t=0}=1,\ \frac{\mathrm{d}y}{\mathrm{d}t}\bigg|_{t=0}=0,\ \frac{\mathrm{d}^2x}{\mathrm{d}t^2}\bigg|_{t=0}=-2,\ \frac{\mathrm{d}^2y}{\mathrm{d}t^2}\bigg|_{t=0}=-1,
$$

代入 ① 式，可知 $\dfrac{\mathrm{d}^2z}{\mathrm{d}t^2}\bigg|_{t=0}=-\dfrac{13}{8}$。

+++

#### 综合解答 (2) 设 $f$ 有一阶连续导数，证明：$z=f\left(\dfrac{x}{y}\right)$ 的充要条件是 $x\dfrac{\partial z}{\partial x}+y\dfrac{\partial z}{\partial y}=0$。
***
证　（必要性）设 $z=f\left(\dfrac{x}{y}\right)$。令 $\dfrac{x}{y}=u$，则

$$
\begin{cases}\dfrac{\partial z}{\partial x}=f'(u)\cdot\dfrac1y,&①\\[2mm] \dfrac{\partial z}{\partial y}=f'(u)\cdot\left(-\dfrac{x}{y^2}\right),&②\end{cases}
$$

$①\times x+②\times y$，得 $x\dfrac{\partial z}{\partial x}+y\dfrac{\partial z}{\partial y}=0$。

（充分性）设 $x\dfrac{\partial z}{\partial x}+y\dfrac{\partial z}{\partial y}=0$。令 $u=\dfrac{x}{y}$，$v=y$，则 $z=z(x,y)$ 为

$$
z=z(yu,v)=f(u,v).
$$

根据复合函数微分法，有

$$
\begin{cases}\dfrac{\partial z}{\partial x}=f'_u\cdot\dfrac1y+f'_v\cdot0,\\[2mm] \dfrac{\partial z}{\partial y}=f'_u\cdot\left(-\dfrac{x}{y^2}\right)+f'_v\cdot1.\end{cases}
$$

由条件

$$
x\frac{\partial z}{\partial x}+y\frac{\partial z}{\partial y}=\frac{x}{y}f'_u-\frac{x}{y}f'_u+yf'_v=0,
$$

知 $f'_v=0$，故 $f$ 只是 $u$ 的函数，即 $z=f(u)=f\left(\dfrac{x}{y}\right)$。

+++

#### 综合解答 (3) 设 $z=z(x,y)$ 是由方程 $F\left(\dfrac1x-\dfrac1y-\dfrac1z\right)=\dfrac1z$ 确定的隐函数，其中 $F$ 可微，求 $x^2\dfrac{\partial z}{\partial x}+y^2\dfrac{\partial z}{\partial y}$。
***
**解法 1**　方程 $F\left(\dfrac1x-\dfrac1y-\dfrac1z\right)=\dfrac1z$ 两边分别对 $x$，$y$ 求导，得

$$
\begin{cases}F'\cdot\left(-\dfrac{1}{x^2}+\dfrac{1}{z^2}\dfrac{\partial z}{\partial x}\right)=-\dfrac{1}{z^2}\dfrac{\partial z}{\partial x},&①\\[2mm] F'\cdot\left(\dfrac{1}{y^2}+\dfrac{1}{z^2}\dfrac{\partial z}{\partial y}\right)=-\dfrac{1}{z^2}\dfrac{\partial z}{\partial y},&②\end{cases}
$$

解 ①② 式，得

$$
\frac{\partial z}{\partial x}=\frac{z^2F'}{(F'+1)x^2},\quad \frac{\partial z}{\partial y}=-\frac{z^2F'}{(F'+1)y^2},
$$

故 $x^2\dfrac{\partial z}{\partial x}+y^2\dfrac{\partial z}{\partial y}=0$。

**解法 2**　用公式求。令 $G=F\left(\dfrac1x-\dfrac1y-\dfrac1z\right)-\dfrac1z$，则

$$
G'_x=F'\cdot\left(-\frac{1}{x^2}\right),\quad G'_y=F'\cdot\frac{1}{y^2},\quad G'_z=F'\cdot\frac{1}{z^2}+\frac{1}{z^2},
$$

故

$$
\frac{\partial z}{\partial x}=-\frac{G'_x}{G'_z}=\frac{z^2F'}{x^2(F'+1)},\quad \frac{\partial z}{\partial y}=-\frac{G'_y}{G'_z}=-\frac{z^2F'}{y^2(F'+1)},
$$

从而 $x^2\dfrac{\partial z}{\partial x}+y^2\dfrac{\partial z}{\partial y}=0$。

+++

#### 综合解答 (4) 设 $y=g(x,z)$ 与 $z=z(x,y)$ 是由方程 $f(x-z,xy)=0$ 确定的函数，求 $\dfrac{\mathrm{d}y}{\mathrm{d}x}$。
***
解　将 $z=z(x,y)$ 代入 $y=g(x,z)$，得 $y=g[x,z(x,y)]$。　①

在方程 ① 两边分别对 $x$ 求导，得 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=g'_1\cdot1+g'_2\cdot\left(\dfrac{\partial z}{\partial x}+\dfrac{\partial z}{\partial y}\cdot\dfrac{\mathrm{d}y}{\mathrm{d}x}\right)$。　②

在方程 $f(x-z,xy)=0$ 两边分别对 $x$，$y$ 求偏导，视 $z$ 是关于 $x,y$ 的函数，得

$$
\begin{cases}f'_1\cdot\left(1-\dfrac{\partial z}{\partial x}\right)+f'_2\cdot y=0,\\[2mm] f'_1\cdot\left(0-\dfrac{\partial z}{\partial y}\right)+f'_2\cdot x=0,\end{cases}
$$

解得 $\dfrac{\partial z}{\partial x}=\dfrac{f'_1+f'_2\cdot y}{f'_1}$，$\dfrac{\partial z}{\partial y}=\dfrac{f'_2\cdot x}{f'_1}$，将其代入 ② 式，解得

$$
\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{f'_1g'_1+g'_2(f'_1+f'_2\cdot y)}{f'_1-xf'_2g'_2}.
$$

+++

#### 综合解答 (5) 求函数 $f(x,y)=(1+y)^2+(1+x)^2$ 在条件 $x^2+y^2+xy=3$ 下的最大值。
***
解　利用拉格朗日乘数法，令

$$
L(x,y,\lambda)=(1+y)^2+(1+x)^2+\lambda(x^2+y^2+xy-3),
$$

则

$$
\begin{cases}L'_x=2(1+x)+\lambda(2x+y)=0,&①\\ L'_y=2(1+y)+\lambda(2y+x)=0,&②\\ L'_\lambda=x^2+y^2+xy-3=0.&③\end{cases}
$$

由 ①② 消去 $\lambda$，得 $(x-y)(x+y-1)=0$，故 $x=y$ 或 $x+y-1=0$。

当 $x=y$ 时，代入 ③ 式，解得 $x=y=\pm1$；

当 $x+y=1$ 时，代入 ③ 式，解得 $x=2$，$y=-1$ 或 $x=-1$，$y=2$。

比较大小：$f(1,1)=8$，$f(-1,-1)=0$，$f(2,-1)=f(-1,2)=9$，故 $f(x,y)$ 的最大值为 $9$。

**【注】** 若 $L(x,y,\lambda)$ 关于 $x,y$ 具有轮换性（即 $x,y$ 互换位置，$L(x,y,\lambda)$ 不变），一般地，方程组 $L'_x=0$，$L'_y=0$，$L'_\lambda=0$ 有解 $x=y$。但应注意，方程组的全部解不一定都满足 $x=y$，此题最大值不是在满足 $x=y$ 的点取得，否则容易漏解。

+++

#### 综合解答 (6) 求椭球面 $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1(a,b,c>0)$ 在第一卦限上的切平面与三个坐标面围成的四面体的最小体积。
***
解　设点 $P(x,y,z)$ 为椭球面在第一卦限上的任一点，则过点 $P$ 的切平面方程为

$$
\frac{2x}{a^2}(X-x)+\frac{2y}{b^2}(Y-y)+\frac{2z}{c^2}(Z-z)=0,
$$

该切平面在三个坐标轴上的截距分别为 $\dfrac{a^2}{x}$，$\dfrac{b^2}{y}$，$\dfrac{c^2}{z}$，故四面体的体积

$$
V=\frac13\cdot\frac12\cdot\frac{a^2}{x}\cdot\frac{b^2}{y}\cdot\frac{c^2}{z}=\frac{a^2b^2c^2}{6xyz}\quad(x>0,y>0,z>0),
$$

问题转化为求 $xyz$ 在条件 $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=1$ 下的最大值。

令 $L=xyz+\lambda\left(\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}-1\right)$，则

$$
\begin{cases}L'_x=yz+2\lambda\dfrac{x}{a^2}=0,&①\\[2mm] L'_y=xz+2\lambda\dfrac{y}{b^2}=0,&②\\[2mm] L'_z=xy+2\lambda\dfrac{z}{c^2}=0,&③\\[2mm] L'_\lambda=\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}-1=0.&④\end{cases}
$$

由 ①②③ 式，得 $\dfrac{x^2}{a^2}=\dfrac{y^2}{b^2}=\dfrac{z^2}{c^2}$，代入 ④ 式，可解得 $x=\dfrac{a}{\sqrt3}$，$y=\dfrac{b}{\sqrt3}$，$z=\dfrac{c}{\sqrt3}$，故所求最小体积为

$$
V=\frac{a^2b^2c^2}{6\cdot\dfrac{a}{\sqrt3}\cdot\dfrac{b}{\sqrt3}\cdot\dfrac{c}{\sqrt3}}=\frac{\sqrt3}{2}abc.
$$

+++

#### 综合解答 (7) 设函数 $f(x,y)=3x+4y-ax^2-2ay^2-2bxy$，问 $a,b$ 满足什么条件时，$f(x,y)$ 有唯一的极大值和唯一的极小值？
***
解　由极值的必要条件，得

$$
\begin{cases}\dfrac{\partial f}{\partial x}=3-2ax-2by=0,\\[2mm] \dfrac{\partial f}{\partial y}=4-4ay-2bx=0,\end{cases}
$$

即 $\begin{cases}2ax+2by=3,\\ 2bx+4ay=4,\end{cases}$ 当 $\begin{vmatrix}2a&2b\\ 2b&4a\end{vmatrix}=8a^2-4b^2\neq0$ 时，$f(x,y)$ 有唯一驻点，且

$$
x=\frac{3a-2b}{2a^2-b^2},\quad y=\frac{4a-3b}{2(2a^2-b^2)}.
$$

$$
A=\frac{\partial^2f}{\partial x^2}=-2a,\quad B=\frac{\partial^2f}{\partial x\partial y}=-2b,\quad C=\frac{\partial^2f}{\partial y^2}=-4a.
$$

当 $AC-B^2=8a^2-4b^2>0$，即 $2a^2-b^2>0$ 时，$f(x,y)$ 有极值。

当 $A=-2a>0$，即 $a<0$ 时，有极小值；当 $A=-2a<0$，即 $a>0$ 时，有极大值。

综上所述，当 $2a^2-b^2>0$ 且 $a<0$ 时，$f(x,y)$ 有唯一的极小值；当 $2a^2-b^2>0$ 且 $a>0$ 时，有唯一的极大值。

+++

#### 综合解答 (8) 设 $f(x,y)=\mathrm{e}^{-x}(ax+b-y^2)$ 在点 $(-1,y_0)$ 处取得极大值，求 $a,b$ 满足的条件。
***
解　依题意，有

$$
\begin{cases}f'_x(-1,y_0)=\mathrm{e}^{-x}(-ax-b+y^2+a)\big|_{(-1,y_0)}=\mathrm{e}(2a-b+y_0^2)=0,&①\\[2mm] f'_y(-1,y_0)=-2y\mathrm{e}^{-x}\big|_{(-1,y_0)}=0&②\end{cases}
$$

（此处由 ② 式，知 $y_0=0$，故 $f(x,y)$ 在点 $(-1,0)$ 处取得极大值），解 ① 式，得 $b=2a$。又

$$
\begin{aligned}
A&=f''_{xx}(-1,0)=\mathrm{e}^{-x}(ax+b-y^2-2a)\big|_{(-1,0)}=\mathrm{e}(-3a+b),\\
B&=f''_{xy}(-1,0)=2y\mathrm{e}^{-x}\big|_{(-1,0)}=0,\\
C&=f''_{yy}(-1,0)=-2\mathrm{e}^{-x}\big|_{(-1,0)}=-2\mathrm{e},
\end{aligned}
$$

由已知，$AC-B^2=-2\mathrm{e}^2(-3a+b)>0$，$A<0$，故 $a>0$，$b=2a$。

当 $a=0$，$b=0$ 时，$AC-B^2=0$，此时 $f(x,y)=-y^2\mathrm{e}^{-x}\leqslant f(-1,0)=0$，不满足极值的定义，故 $f(-1,0)$ 不是极大值。

综上所述，$a,b$ 满足的条件为 $a>0$，$b=2a$。

+++

#### 综合解答 (9) 设函数 $z=z(x,y)$ 由方程 $x^2-6xy+10y^2-2yz-z^2+18=0$ 确定，求 $z=z(x,y)$ 的极值。
***
解　已知方程两边同时对 $x$，$y$ 求偏导，得

$$
\begin{cases}2x-6y-2y\dfrac{\partial z}{\partial x}-2z\dfrac{\partial z}{\partial x}=0,&①\\[2mm] -6x+20y-2z-2y\dfrac{\partial z}{\partial y}-2z\dfrac{\partial z}{\partial y}=0.&②\end{cases}
$$

令 $\dfrac{\partial z}{\partial x}=0$，$\dfrac{\partial z}{\partial y}=0$，得 $\begin{cases}x-3y=0,\\ -3x+10y-z=0,\end{cases}$ 解得 $x=3y$，$z=y$，代入原方程解得

$$
x=9,\ y=3,\ z=3\quad\text{或}\quad x=-9,\ y=-3,\ z=-3.
$$

①② 式两边同时对 $x$，$y$ 求偏导，得

$$
\begin{cases}2-2y\dfrac{\partial^2z}{\partial x^2}-2\left(\dfrac{\partial z}{\partial x}\right)^2-2z\dfrac{\partial^2z}{\partial x^2}=0,\\[2mm] -6-2\dfrac{\partial z}{\partial x}-2y\dfrac{\partial^2z}{\partial x\partial y}-2\dfrac{\partial z}{\partial y}\cdot\dfrac{\partial z}{\partial x}-2z\dfrac{\partial^2z}{\partial x\partial y}=0,\\[2mm] 20-2\dfrac{\partial z}{\partial y}-2\dfrac{\partial z}{\partial y}-2y\dfrac{\partial^2z}{\partial y^2}-2\left(\dfrac{\partial z}{\partial y}\right)^2-2z\dfrac{\partial^2z}{\partial y^2}=0,\end{cases}
$$

将 $\dfrac{\partial z}{\partial x}=0$，$\dfrac{\partial z}{\partial y}=0$，$x=9$，$y=3$，$z=3$ 代入上方程组，得

$$
A=\frac{\partial^2z}{\partial x^2}\bigg|_{(9,3,3)}=\frac16,\quad B=\frac{\partial^2z}{\partial x\partial y}\bigg|_{(9,3,3)}=-\frac12,\quad C=\frac{\partial^2z}{\partial y^2}\bigg|_{(9,3,3)}=\frac53,
$$

故 $AC-B^2=\dfrac{1}{36}>0$，$A=\dfrac16>0$，所以 $z(9,3)=3$ 为极小值。

同理，得

$$
A=\frac{\partial^2z}{\partial x^2}\bigg|_{(-9,-3,-3)}=-\frac16,\quad B=\frac{\partial^2z}{\partial x\partial y}\bigg|_{(-9,-3,-3)}=\frac12,\quad C=\frac{\partial^2z}{\partial y^2}\bigg|_{(-9,-3,-3)}=-\frac53,
$$

故 $AC-B^2=\dfrac{1}{36}>0$，$A=-\dfrac16<0$，所以 $z(-9,-3)=-3$ 为极大值。

+++

#### 综合解答 (10) 设 $f(x)$ 有二阶连续导数，且 $f(x)>0$，$f'(0)=0$，证明：$z=f(x)\ln f(y)$ 在点 $(0,0)$ 处取得极小值的充分条件是 $f''(0)>0$ 且 $f(0)>1$。
***
证　由 $z=f(x)\ln f(y)$，得 $z'_x=f'(x)\ln f(y)$，$z'_y=f(x)\cdot\dfrac{f'(y)}{f(y)}$。

由已知，$f'(0)=0$，故

$$
z'_x(0,0)=f'(0)\ln f(0)=0,\quad z'_y(0,0)=f(0)\cdot\frac{f'(0)}{f(0)}=0.
$$

又

$$
\begin{aligned}
z''_{xx}(x,y)&=f''(x)\ln f(y),\\
z''_{xy}(x,y)&=f'(x)\frac{f'(y)}{f(y)},\\
z''_{yy}(x,y)&=f(x)\frac{f''(y)f(y)-[f'(y)]^2}{f^2(y)},
\end{aligned}
$$

所以 $A=z''_{xx}(0,0)=f''(0)\ln f(0)$，$B=z''_{xy}(0,0)=0$，$C=z''_{yy}(0,0)=f''(0)$。

又 $f''(0)>0$，$f(0)>1$，故

$$
AC-B^2=f''(0)\ln f(0)\cdot f''(0)-0^2=[f''(0)]^2\ln f(0)>0,\quad A=f''(0)\ln f(0)>0,
$$

所以 $z=f(x)\ln f(y)$ 在点 $(0,0)$ 处取得极小值。

+++

#### 综合解答 (11) 已知 $z=f(x,y)$ 的全微分 $\mathrm{d}z=(y-x^2)\mathrm{d}x+(x-1)\mathrm{d}y$，且 $f(1,1)=-\dfrac13$，求 $f(x,y)$ 在 $D:0\leqslant y\leqslant7-x$，$0\leqslant x\leqslant7$ 上的最大值。
***
解　依题意，$\dfrac{\partial z}{\partial x}=y-x^2$，$\dfrac{\partial z}{\partial y}=x-1$，故

$$
z=\int\frac{\partial z}{\partial x}\mathrm{d}x=\int(y-x^2)\mathrm{d}x+\varphi(y)=xy-\frac13x^3+\varphi(y),
$$

又 $\dfrac{\partial z}{\partial y}=x+\varphi'(y)=x-1$，得 $\varphi'(y)=-1$，积分得 $\varphi(y)=-y+C$，所以

$$
z=xy-\frac13x^3-y+C.
$$

由 $f(1,1)=-\dfrac13$，得 $C=0$，于是 $z=f(x,y)=xy-\dfrac13x^3-y$。

（Ⅰ）在 $D$ 内，由 $\dfrac{\partial z}{\partial x}=y-x^2=0$，$\dfrac{\partial z}{\partial y}=x-1=0$，解得唯一驻点 $(1,1)$。

（Ⅱ）在 $D$ 的边界上，$y=0(0\leqslant x\leqslant7)$，$f(x,0)=-\dfrac13x^3$，显然在 $[0,7]$ 上最大值为 $0$；$x=0(0\leqslant y\leqslant7)$，$f(0,y)=-y$，最大值为 $0$；

$x+y=7$，$f(x,7-x)=-\dfrac{x^3}{3}-x^2+8x-7(0\leqslant x\leqslant7)$，由 $\dfrac{\mathrm{d}}{\mathrm{d}x}[f(x,7-x)]=-x^2-2x+8=0$，得 $x=2$，$x=-4$（舍）。

比较大小：

$$
f(1,1)=-\frac13,\ f(0,0)=0,\ f(2,5)=\frac73,\ f(0,7)=-7,\ f(7,0)=-\frac{7^3}{3},
$$

故 $f(x,y)$ 在 $D$ 上的最大值为 $f(2,5)=\dfrac73$。

**【注】** 此题已知全微分，求 $f(x,y)$ 也可利用凑微分法：

$$
\begin{aligned}
\mathrm{d}z&=(y-x^2)\mathrm{d}x+(x-1)\mathrm{d}y=y\mathrm{d}x+x\mathrm{d}y-x^2\mathrm{d}x-\mathrm{d}y\\
&=\mathrm{d}(xy)-\mathrm{d}\left(\frac{x^3}{3}\right)-\mathrm{d}y=\mathrm{d}\left(xy-\frac{x^3}{3}-y\right),
\end{aligned}
$$

故 $z=xy-\dfrac{x^3}{3}-y+C$。

+++

#### 综合解答 (12) 求曲线 $x^2+xy+y^2=1$ 上的点到坐标原点的最长距离与最短距离。
***
解　曲线 $x^2+xy+y^2=1$ 上任意一点 $(x,y)$ 到坐标原点的距离为 $d=f(x,y)=\sqrt{x^2+y^2}$，则原问题转化为求 $f(x,y)=\sqrt{x^2+y^2}$ 在条件 $x^2+xy+y^2=1$ 下的最大值与最小值的问题。

令 $L=x^2+y^2+\lambda(x^2+xy+y^2-1)$，则

$$
\begin{cases}L'_x=2x+(2x+y)\lambda=0,&①\\ L'_y=2y+(x+2y)\lambda=0,&②\\ L'_\lambda=x^2+xy+y^2-1=0.&③\end{cases}
$$

由 $①\times y-②\times x$，得 $(y^2-x^2)\lambda=0$，解得 $\lambda=0$ 或 $x=\pm y$。

若 $\lambda=0$，则由 ①② 式，得 $x=y=0$ 不满足 ③ 式，故 $\lambda=0$ 舍去。

将 $x=-y$ 代入 ③ 式，解得 $\begin{cases}x=1,\\ y=-1\end{cases}$ 或 $\begin{cases}x=-1,\\ y=1.\end{cases}$

将 $x=y$ 代入 ③ 式，解得 $\begin{cases}x=\dfrac{1}{\sqrt3},\\[2mm] y=\dfrac{1}{\sqrt3}\end{cases}$ 或 $\begin{cases}x=-\dfrac{1}{\sqrt3},\\[2mm] y=-\dfrac{1}{\sqrt3}.\end{cases}$

比较大小：由于 $f(1,-1)=\sqrt2$，$f(-1,1)=\sqrt2$，$f\left(\dfrac{1}{\sqrt3},\dfrac{1}{\sqrt3}\right)=\dfrac{\sqrt6}{3}$，$f\left(-\dfrac{1}{\sqrt3},-\dfrac{1}{\sqrt3}\right)=\dfrac{\sqrt6}{3}$，故最长距离为 $\sqrt2$，最短距离为 $\dfrac{\sqrt6}{3}$。

+++

#### 综合解答 (13) 设中心在原点的椭圆为 $x^2-4xy+5y^2=1$，求该椭圆的长半轴与短半轴。
***
解　依题意，相当于求原点 $(0,0)$ 到椭圆上的点的距离 $d$ 的最大值和最小值。

设 $P(x,y)$ 为椭圆上任一点，则 $d=\sqrt{x^2+y^2}$，$d^2=x^2+y^2$。

利用拉格朗日乘数法，令 $L=x^2+y^2+\lambda(x^2-4xy+5y^2-1)$，则

$$
\begin{cases}L'_x=2x+2\lambda x-4\lambda y=0,&①\\ L'_y=2y-4\lambda x+10\lambda y=0,&②\\ L'_\lambda=x^2-4xy+5y^2-1=0,&③\end{cases}
$$

$①\times\dfrac{x}{2}+②\times\dfrac{y}{2}$，得 $x^2+y^2+\lambda(x^2-4xy+5y^2)=0$，又 $x^2-4xy+5y^2=1$，故 $x^2+y^2=-\lambda$，于是只需求 $\lambda$，可得 $d=\sqrt{-\lambda}$。

① 与 ② 变形为 $\begin{cases}(1+\lambda)x-2\lambda y=0,\\ -2\lambda x+(1+5\lambda)y=0,\end{cases}$ 上式为关于 $x,y$ 的二元一次齐次方程组，有非零解 $x,y$ 的充要条件是

$$
\begin{vmatrix}1+\lambda&-2\lambda\\ -2\lambda&1+5\lambda\end{vmatrix}=\lambda^2+6\lambda+1=0,
$$

解得 $\lambda_1=-3+2\sqrt2$，$\lambda_2=-3-2\sqrt2$，故 $-\lambda=3\pm2\sqrt2=(\sqrt2\pm1)^2$，所以 $d_1=\sqrt2+1$，$d_2=\sqrt2-1$ 分别为长半轴和短半轴。

+++

#### 综合解答 (14) 设 $x=x(y)$，$z=z(y)$ 由方程组 $\begin{cases}F(y-x,y-z)=0,\\[2mm] G\left(xy,\dfrac zy\right)=0\end{cases}$ 确定，求 $\dfrac{\mathrm{d}x}{\mathrm{d}y}$，$\dfrac{\mathrm{d}z}{\mathrm{d}y}$。
***
解　方程组等号两边同时对 $y$ 求导，得

$$
\begin{cases}F'_1\cdot\left(1-\dfrac{\mathrm{d}x}{\mathrm{d}y}\right)+F'_2\cdot\left(1-\dfrac{\mathrm{d}z}{\mathrm{d}y}\right)=0,\\[2mm] G'_1\cdot\left(x+y\dfrac{\mathrm{d}x}{\mathrm{d}y}\right)+G'_2\cdot\left(-\dfrac{z}{y^2}+\dfrac1y\dfrac{\mathrm{d}z}{\mathrm{d}y}\right)=0,\end{cases}
$$

整理，得

$$
\begin{cases}F'_1\dfrac{\mathrm{d}x}{\mathrm{d}y}+F'_2\dfrac{\mathrm{d}z}{\mathrm{d}y}=F'_1+F'_2,\\[2mm] yG'_1\dfrac{\mathrm{d}x}{\mathrm{d}y}+\dfrac1yG'_2\dfrac{\mathrm{d}z}{\mathrm{d}y}=\dfrac{z}{y^2}G'_2-xG'_1,\end{cases}
$$

解此方程组，得

$$
\frac{\mathrm{d}x}{\mathrm{d}y}=\frac{\begin{vmatrix}F'_1+F'_2&F'_2\\[2mm] \dfrac{z}{y^2}G'_2-xG'_1&\dfrac1yG'_2\end{vmatrix}}{\begin{vmatrix}F'_1&F'_2\\[2mm] yG'_1&\dfrac1yG'_2\end{vmatrix}}=\frac{\dfrac1yF'_1G'_2+xF'_2G'_1+\left(\dfrac1y-\dfrac{z}{y^2}\right)F'_2G'_2}{\dfrac1yF'_1G'_2-yF'_2G'_1}.
$$

同理，可得

$$
\frac{\mathrm{d}z}{\mathrm{d}y}=-\frac{(x+y)F'_1G'_1+yF'_2G'_1-\dfrac{z}{y^2}F'_1G'_2}{\dfrac1yF'_1G'_2-yF'_2G'_1}.
$$

+++

#### 综合解答 (15) 已知曲面 $\mathrm{e}^{2x-z}=f(\pi y-\sqrt2z)$，$f$ 可微。证明：该曲面上任一点的切平面都平行于一条定直线。
***
证　依题意，只要证明曲面上任一点的法向量都垂直于定向量。

令 $F(x,y,z)=\mathrm{e}^{2x-z}-f(\pi y-\sqrt2z)$，则 $F'_x=2\mathrm{e}^{2x-z}$，$F'_y=-\pi f'$，$F'_z=-\mathrm{e}^{2x-z}+\sqrt2f'$，故曲面上任一点 $(x,y,z)$ 处的法向量为

$$
\boldsymbol{n}=(2\mathrm{e}^{2x-z},\ -\pi f',\ -\mathrm{e}^{2x-z}+\sqrt2f').
$$

设定向量为 $\boldsymbol{T}=(l,m,n)$，要使 $\boldsymbol{T}\cdot\boldsymbol{n}=0$，即 $2l\mathrm{e}^{2x-z}-m\pi f'-n\mathrm{e}^{2x-z}+\sqrt2nf'=0$，只需使

$$
2l=n,\quad m\pi=\sqrt2n,
$$

所以若取 $l=\pi$，$n=2\pi$，$m=2\sqrt2$，则有 $\boldsymbol{T}\cdot\boldsymbol{n}=0$，故曲面上任一点的切平面都平行于以 $(\pi,2\sqrt2,2\pi)$ 为方向向量的定直线。

**【注】** 此题说明 $\mathrm{e}^{2x-z}=f(\pi y-\sqrt2z)$ 表示一个柱面。

+++

#### 综合解答 (16) 设 $\alpha,\beta$ 为正数，且 $\dfrac{1}{\alpha}+\dfrac{1}{\beta}=1$，求 $f(x,y)=\dfrac{1}{\alpha}x^\alpha+\dfrac{1}{\beta}y^\beta$ 在条件 $xy=1(x>0,y>0)$ 下的最小值。
***
解　利用拉格朗日乘数法，令 $L=\dfrac{1}{\alpha}x^\alpha+\dfrac{1}{\beta}y^\beta+\lambda(xy-1)$，则

$$
\begin{cases}L'_x=x^{\alpha-1}+\lambda y=0,\\ L'_y=y^{\beta-1}+\lambda x=0,\\ L'_\lambda=xy-1=0,\end{cases}
$$

解方程组得 $x=y=1$。由此得到点 $(1,1)$ 是唯一可能的极值点，再应用二元函数极值的充分条件判断，可知点 $(1,1)$ 是唯一极小值点，故点 $(1,1)$ 即为最小值点，最小值为 $f_{\min}=f(1,1)=1$。

+++

#### 综合解答 (17) 求函数 $u=\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}$ 在点 $P(x,y,z)$ 处沿 $\boldsymbol{l}=x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k}$ 的方向导数，并讨论在哪些点该方向导数等于梯度的模。
***
解

$$
\frac{\partial u}{\partial l}=\frac{\partial u}{\partial x}\cos\alpha+\frac{\partial u}{\partial y}\cos\beta+\frac{\partial u}{\partial z}\cos\gamma.
$$

又

$$
\frac{\partial u}{\partial x}=\frac{2x}{a^2},\quad \frac{\partial u}{\partial y}=\frac{2y}{b^2},\quad \frac{\partial u}{\partial z}=\frac{2z}{c^2},
$$

$$
\cos\alpha=\frac{x}{r},\quad \cos\beta=\frac{y}{r},\quad \cos\gamma=\frac{z}{r},
$$

其中 $r=\sqrt{x^2+y^2+z^2}$，故

$$
\frac{\partial u}{\partial l}=\frac{2x}{a^2}\cdot\frac{x}{r}+\frac{2y}{b^2}\cdot\frac{y}{r}+\frac{2z}{c^2}\cdot\frac{z}{r}=\frac{2u}{r},
$$

且梯度为

$$
\mathbf{grad}\,u=\left(\frac{\partial u}{\partial x},\frac{\partial u}{\partial y},\frac{\partial u}{\partial z}\right)=\left(\frac{2x}{a^2},\frac{2y}{b^2},\frac{2z}{c^2}\right).
$$

（Ⅰ）当 $a,b,c$ 两两不相等时，函数 $u$ 的等值面为椭圆 $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}+\dfrac{z^2}{c^2}=k(k>0)$，梯度方向是等值面的外法线方向，在椭球面的六个顶点处的外法线方向与向径 $\boldsymbol{l}$ 的方向相同，故在这些点处有 $\dfrac{\partial u}{\partial l}=|\mathbf{grad}\,u|$。

（Ⅱ）当 $a=b\neq c$ 时，等值面为旋转椭球面 $\dfrac{x^2+y^2}{a^2}+\dfrac{z^2}{c^2}=k(k>0)$，在顶点 $(0,0,\pm c\sqrt k)$ 及圆周 $\begin{cases}x^2+y^2=a^2k,\\ z=0\end{cases}$ 上，梯度方向与向径 $\boldsymbol{l}$ 方向相同，故在这些点处有 $\dfrac{\partial u}{\partial l}=|\mathbf{grad}\,u|$。

（Ⅲ）当 $a=b=c$ 时，等值面为球面 $x^2+y^2+z^2=a^2k(k>0)$，球面上各点的外法线方向与向径 $\boldsymbol{l}$ 方向相同，故在这些点处有 $\dfrac{\partial u}{\partial l}=|\mathbf{grad}\,u|$。

+++

#### 拓展选择 (1) 下列（　）选项条件成立时，能够推出函数 $f(x,y)$ 在点 $(x_0,y_0)$ 处可微，且全微分 $\mathrm{d}f(x,y)\big|_{(x_0,y_0)}=0$。

;;;
A. $f'_x(x_0,y_0)=f'_y(x_0,y_0)=0$
B. $f(x,y)$ 在点 $(x_0,y_0)$ 处的全增量 $\Delta f=\dfrac{\Delta x\Delta y}{\sqrt{(\Delta x)^2+(\Delta y)^2}}$
C. $f(x,y)$ 在点 $(x_0,y_0)$ 处的全增量 $\Delta f=\dfrac{\sin[(\Delta x)^2+(\Delta y)^2]}{\sqrt{(\Delta x)^2+(\Delta y)^2}}$
D. $f(x,y)$ 在点 $(x_0,y_0)$ 处的全增量 $\Delta f=[(\Delta x)^2+(\Delta y)^2]\sin\dfrac{1}{(\Delta x)^2+(\Delta y)^2}$
;;;D
***
**D.**

解　对于 D：当 D 中条件成立时，有

$$
f'_x(x_0,y_0)=\lim_{\Delta x\to0}\frac{\Delta f}{\Delta x}=\lim_{\Delta x\to0}\left[\frac{1}{\Delta x}\cdot(\Delta x)^2\sin\frac{1}{(\Delta x)^2}\right]=0,
$$

$$
f'_y(x_0,y_0)=\lim_{\Delta y\to0}\frac{\Delta f}{\Delta y}=\lim_{\Delta y\to0}\left[\frac{1}{\Delta y}\cdot(\Delta y)^2\sin\frac{1}{(\Delta y)^2}\right]=0,
$$

$$
\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}\frac{\Delta f-\mathrm{d}f}{\rho}=\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}\frac{[(\Delta x)^2+(\Delta y)^2]\sin\dfrac{1}{(\Delta x)^2+(\Delta y)^2}}{\sqrt{(\Delta x)^2+(\Delta y)^2}}=\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}[(\Delta x)^2+(\Delta y)^2]^{\frac12}\cdot\sin\frac{1}{(\Delta x)^2+(\Delta y)^2}=0.
$$

由可微的定义，知 $f(x,y)$ 在点 $(x_0,y_0)$ 处可微，且 $\mathrm{d}f=0$，D 正确。

对于 A：由 $f'_x(x_0,y_0)=f'_y(x_0,y_0)=0$，知偏导数存在，但不能推出 $f(x,y)$ 在点 $(x_0,y_0)$ 处可微。

对于 B：$\Delta f=\dfrac{\Delta x\Delta y}{\sqrt{(\Delta x)^2+(\Delta y)^2}}$，当 $\Delta y=0$ 时，$\Delta f=0$；当 $\Delta x=0$ 时，$\Delta f=0$，故 $f'_x(x_0,y_0)=\lim\limits_{\Delta x\to0}\dfrac{\Delta f}{\Delta x}=0$，$f'_y(x_0,y_0)=\lim\limits_{\Delta y\to0}\dfrac{\Delta f}{\Delta y}=0$，由此可知

$$
\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}\frac{\Delta f-\mathrm{d}f}{\rho}=\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}\frac{\Delta x\Delta y}{\sqrt{(\Delta x)^2+(\Delta y)^2}}\cdot\frac{1}{\sqrt{(\Delta x)^2+(\Delta y)^2}}=\lim_{\substack{\Delta x\to0\\ \Delta y\to0}}\frac{\Delta x\Delta y}{(\Delta x)^2+(\Delta y)^2}
$$

不存在，即 $f(x,y)$ 在点 $(x_0,y_0)$ 处不可微。

对于 C：由于 $\Delta f=\dfrac{\sin[(\Delta x)^2+(\Delta y)^2]}{\sqrt{(\Delta x)^2+(\Delta y)^2}}$，故 $f'_x(x_0,y_0)=\lim\limits_{\Delta x\to0}\dfrac{\sin(\Delta x)^2}{|\Delta x|\cdot\Delta x}=\lim\limits_{\Delta x\to0}\dfrac{\Delta x}{|\Delta x|}$，又因为 $\lim\limits_{\Delta x\to0^+}\dfrac{\Delta x}{|\Delta x|}=1$，$\lim\limits_{\Delta x\to0^-}\dfrac{\Delta x}{|\Delta x|}=-1$，所以 $f'_x(x_0,y_0)$ 不存在。同理 $f'_y(x_0,y_0)$ 不存在，故 $f(x,y)$ 在点 $(x_0,y_0)$ 处不可微。

+++

#### 拓展解答 (1) 设 $f(x,y)$ 在点 $(0,0)$ 的某邻域内有定义，$f(0,0)=0$，且 $\lim\limits_{\substack{x\to0\\ y\to0}}\dfrac{f(x,y)}{\sqrt{x^2+y^2}}=1+k$（$k$ 为常数）。

证明：（Ⅰ）$f(x,y)$ 在点 $(0,0)$ 处连续；\
（Ⅱ）当 $k\neq-1$ 时，$f(x,y)$ 在点 $(0,0)$ 处不可微；\
（Ⅲ）当 $k=-1$ 时，$f(x,y)$ 在点 $(0,0)$ 处可微。
***
证　令 $\rho=\sqrt{x^2+y^2}$，由已知条件及极限与无穷小的关系，有

$$
\frac{f(x,y)}{\sqrt{x^2+y^2}}=(1+k)+\alpha\quad(\alpha\ \text{为无穷小}),
$$

即 $f(x,y)=(1+k)\sqrt{x^2+y^2}+o(\rho)$。　①

（Ⅰ）① 式两边同时取极限，有

$$
\lim_{\substack{x\to0\\ y\to0}}f(x,y)=\lim_{\substack{x\to0\\ y\to0}}(1+k)\sqrt{x^2+y^2}+\lim_{\substack{x\to0\\ y\to0}}o(\rho)=0=f(0,0),
$$

故 $f(x,y)$ 在点 $(0,0)$ 处连续。

（Ⅱ）当 $k\neq-1$ 时，

$$
f'_x(0,0)=\lim_{x\to0}\frac{f(x,0)-f(0,0)}{x}=\lim_{x\to0}\frac{(1+k)\sqrt{x^2}+o(x)}{x}=\lim_{x\to0}\left[(1+k)\frac{|x|}{x}+\frac{o(x)}{x}\right],
$$

$\lim\limits_{x\to0}(1+k)\dfrac{|x|}{x}$ 不存在，故 $f'_x(0,0)$ 不存在，同理 $f'_y(0,0)$ 不存在，因此 $f(x,y)$ 在点 $(0,0)$ 处不可微（偏导数存在是可微的必要条件）。

（Ⅲ）当 $k=-1$ 时，$f(x,y)=o(\rho)$，故

$$
f'_x(0,0)=\lim_{x\to0}\frac{f(x,0)-f(0,0)}{x}=\lim_{x\to0}\frac{o(x)}{x}=0.
$$

同理，$f'_y(0,0)=0$，故 $\mathrm{d}f\big|_{(0,0)}=0\cdot x+0\cdot y$，则

$$
\lim_{\substack{x\to0\\ y\to0}}\frac{\Delta f-\mathrm{d}f}{\rho}=\lim_{\substack{x\to0\\ y\to0}}\frac{f(x,y)-f(0,0)-0}{\sqrt{x^2+y^2}}=\lim_{\substack{x\to0\\ y\to0}}\frac{f(x,y)}{\sqrt{x^2+y^2}}=0,
$$

故 $f(x,y)$ 在点 $(0,0)$ 处可微。
