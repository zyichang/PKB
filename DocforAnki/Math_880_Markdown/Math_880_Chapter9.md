---
quizify:
  format: 1
  deck: Math_880::Chapter_9
  tags: [Math, 880题, 数一, 第九章, 曲线积分与曲面积分]
---

+++

#### 基础选择 (1) 设 $L$ 为圆周 $x^2+y^2=2x$，则 $I=\int_L x\,\mathrm{d}s=$（　）．

;;;
A. $2\pi$
B. $\pi$
C. $1$
D. $0$
;;;A
***
$L$ 的参数方程为 $\begin{cases}x=\cos t+1,\\ y=\sin t,\end{cases}$ 则 $\mathrm{d}s=\sqrt{x'^2(t)+y'^2(t)}\,\mathrm{d}t=\mathrm{d}t$，故

$$I=\int_L x\,\mathrm{d}s=\int_0^{2\pi}(1+\cos t)\,\mathrm{d}t=2\pi.$$

【注】也可利用质心（形心）坐标 $\bar{x}=1$，则

$$\int_L x\,\mathrm{d}s=\bar{x}\cdot\int_L \mathrm{d}s=1\times 2\pi=2\pi$$

（$\int_L \mathrm{d}s$ 表示圆周长）．

+++

#### 基础选择 (2) 设 $S$ 为球面 $(x-a)^2+(y-b)^2+(z-c)^2=1$（$a,b,c$ 均大于零），则 $I=\iint_S (x+y+z)\,\mathrm{d}S=$（　）．

;;;
A. $4\pi$
B. $4\pi(a+b+c)$
C. $0$
D. $\dfrac{4}{3}\pi(a+b+c)$
;;;B
***
注意到 $S$ 分别关于平面 $x=a$，$y=b$，$z=c$ 对称，则

$$I=\iint_S (x+y+z)\,\mathrm{d}S=\iint_S [(x-a)+(y-b)+(z-c)]\,\mathrm{d}S+\iint_S (a+b+c)\,\mathrm{d}S$$

$$=0+(a+b+c)\iint_S \mathrm{d}S=4\pi(a+b+c).$$

【注】$\iint_S \mathrm{d}S$ 表示球面的表面积．

+++

#### 基础选择 (3) 设 $S:x^2+y^2+z^2=R^2\ (z\geqslant 0)$，$S_1$ 为 $S$ 在第一卦限的部分，则（　）．

;;;
A. $\iint_S x\,\mathrm{d}S=4\iint_{S_1} x\,\mathrm{d}S$
B. $\iint_S y\,\mathrm{d}S=4\iint_{S_1} y\,\mathrm{d}S$
C. $\iint_S z\,\mathrm{d}S=4\iint_{S_1} z\,\mathrm{d}S$
D. $\iint_S xyz\,\mathrm{d}S=4\iint_{S_1} xyz\,\mathrm{d}S$
;;;C
***
由 $z=zx^0y^0$，知 $z$ 关于 $x,y$ 均为偶函数，故 $\iint_S z\,\mathrm{d}S=4\iint_{S_1} z\,\mathrm{d}S$．

由 $S$ 关于 $xOz$ 面、$yOz$ 面均对称，知 $\iint_S x\,\mathrm{d}S=0$，$\iint_S y\,\mathrm{d}S=0$，$\iint_S xyz\,\mathrm{d}S=0$，而 $\iint_{S_1} x\,\mathrm{d}S>0$，$\iint_{S_1} y\,\mathrm{d}S>0$，$\iint_{S_1} xyz\,\mathrm{d}S>0$，故排除 A，B，D，所以 **C** 正确．

+++

#### 基础填空 (1) 设 $S$ 为平面 $x+y+z=4$ 被圆柱面 $x^2+y^2=1$ 截出的有限部分，则 $I=\iint_S z\,\mathrm{d}S=$ ________．
***
$4\sqrt{3}\pi$．

由 $S:z=4-x-y$，得 $z'_x=-1$，$z'_y=-1$，则 $\mathrm{d}S=\sqrt{1+z'^2_x+z'^2_y}\,\mathrm{d}x\mathrm{d}y=\sqrt{3}\,\mathrm{d}x\mathrm{d}y$，故

$$\iint_S z\,\mathrm{d}S=\iint_{D_{xy}}(4-x-y)\cdot\sqrt{3}\,\mathrm{d}x\mathrm{d}y$$

$$=\sqrt{3}\int_0^{2\pi}\mathrm{d}\theta\int_0^1 (4-r\cos\theta-r\sin\theta)r\,\mathrm{d}r=4\sqrt{3}\pi\quad (D_{xy}:x^2+y^2\leqslant 1).$$

+++

#### 基础填空 (2) 设 $L$ 为 $x^2+y^2=R^2\ (y\geqslant 0)$ 上由点 $A\left(-\dfrac{R}{\sqrt{2}},\dfrac{R}{\sqrt{2}}\right)$ 到点 $B(R,0)$ 的一段弧，则 $\int_L y\,\mathrm{d}s=$ ________，$\int_L y\,\mathrm{d}x=$ ________．
***
$\dfrac{2+\sqrt{2}}{2}R^2$，$\dfrac{3\pi+2}{8}R^2$．

弧 $\overparen{AB}$ 是上半圆周上从第二象限的点 $A$ 经最高点 $C(0,R)$ 到 $x$ 轴上的点 $B(R,0)$ 的一段弧．取 $x$ 为参数，则弧 $\overparen{AB}$ 的方程为 $\begin{cases}x=x,\\ y=\sqrt{R^2-x^2}\end{cases}\left(-\dfrac{R}{\sqrt{2}}\leqslant x\leqslant R\right)$．

$$\mathrm{d}s=\sqrt{1+y'^2}\,\mathrm{d}x=\frac{R}{\sqrt{R^2-x^2}}\,\mathrm{d}x,$$

故

$$\int_L y\,\mathrm{d}s=\int_{-\frac{R}{\sqrt{2}}}^{R}\sqrt{R^2-x^2}\cdot\frac{R}{\sqrt{R^2-x^2}}\,\mathrm{d}x=\left(1+\frac{1}{\sqrt{2}}\right)R^2=\frac{2+\sqrt{2}}{2}R^2,$$

$$\int_L y\,\mathrm{d}x=\int_{-\frac{R}{\sqrt{2}}}^{R}\sqrt{R^2-x^2}\,\mathrm{d}x\xlongequal{x=R\cos t}-R^2\int_{\frac{3\pi}{4}}^{0}\sin^2 t\,\mathrm{d}t$$

$$=R^2\int_0^{\frac{3\pi}{4}}\frac{1-\cos 2t}{2}\,\mathrm{d}t=\left(\frac{3\pi}{8}+\frac{1}{4}\right)R^2=\frac{3\pi+2}{8}R^2.$$

【注】本题若取 $y$ 为参数，由图知，曲线上的点与 $y$ 不是一一对应的，则应将曲线 $L$ 分为 $\overparen{AC}$ 和 $\overparen{CB}$ 两段分别积分．

+++

#### 基础填空 (3) 设 $L$ 为球面 $x^2+y^2+z^2=R^2$ 与平面 $x+y+z=0$ 的交线，则 $I=\oint_L (z+x^2)\,\mathrm{d}s=$ ________．
***
$\dfrac{2\pi R^3}{3}$．

由于曲线 $L:\begin{cases}x^2+y^2+z^2=R^2,\\ x+y+z=0\end{cases}$ 关于直线 $x=y=z$ 对称，所以

$$\oint_L x^2\,\mathrm{d}s=\frac{1}{3}\oint_L (x^2+y^2+z^2)\,\mathrm{d}s=\frac{1}{3}\oint_L R^2\,\mathrm{d}s,$$

$$\oint_L z\,\mathrm{d}s=\frac{1}{3}\oint_L (x+y+z)\,\mathrm{d}s=\frac{1}{3}\oint_L 0\,\mathrm{d}s=0,$$

故

$$I=\oint_L (z+x^2)\,\mathrm{d}s=0+\frac{1}{3}\oint_L R^2\,\mathrm{d}s=\frac{R^2}{3}\cdot 2\pi R=\frac{2\pi R^3}{3}.$$

+++

#### 基础填空 (4) 设曲线 $L$ 为 $x^2+y^2+z^2=\dfrac{9}{2}$ 与 $x+z=1$ 的交线，则 $I=\oint_L (x^2+y^2+z^2)\,\mathrm{d}s=$ ________．
***
$18\pi$．

将 $x^2+y^2+z^2=\dfrac{9}{2}$ 代入被积函数，得 $I=\oint_L (x^2+y^2+z^2)\,\mathrm{d}s=\dfrac{9}{2}\oint_L \mathrm{d}s$．

交线 $L$ 的弧长不易直接计算，考虑写出 $L$ 的参数式，将 $L:\begin{cases}x^2+y^2+z^2=\dfrac{9}{2},\\ x+z=1\end{cases}$ 变形为

$$\begin{cases}\dfrac{\left(x-\dfrac{1}{2}\right)^2}{2}+\dfrac{y^2}{4}=1,\\ x+z=1.\end{cases}$$

令 $\dfrac{x-\dfrac{1}{2}}{\sqrt{2}}=\cos t$，$\dfrac{y}{2}=\sin t$，则 $z=1-x=\dfrac{1}{2}-\sqrt{2}\cos t$，即

$$x=\frac{1}{2}+\sqrt{2}\cos t,\quad y=2\sin t,\quad z=\frac{1}{2}-\sqrt{2}\cos t\quad(0\leqslant t\leqslant 2\pi).$$

$$\mathrm{d}s=\sqrt{x'^2(t)+y'^2(t)+z'^2(t)}\,\mathrm{d}t=\sqrt{(-\sqrt{2}\sin t)^2+(2\cos t)^2+(\sqrt{2}\sin t)^2}\,\mathrm{d}t=2\,\mathrm{d}t,$$

故 $I=\oint_L (x^2+y^2+z^2)\,\mathrm{d}s=\dfrac{9}{2}\int_0^{2\pi}2\,\mathrm{d}t=18\pi$．

+++

#### 基础填空 (5) 设曲面 $S:|x|+|y|+|z|=1$，则 $I=\iint_S (x+y+|z|)\,\mathrm{d}S=$ ________．（$S$ 为闭曲面）
***
$\dfrac{4\sqrt{3}}{3}$．

由 $S$ 关于 $yOz$ 面、$xOy$ 面对称，$x$ 与 $y$ 是奇函数，故 $\iint_S x\,\mathrm{d}S=\iint_S y\,\mathrm{d}S=0$．

又 $S$ 关于直线 $x=y=z$ 对称，由轮换性，知

$$I=\iint_S (x+y+|z|)\,\mathrm{d}S=0+0+\frac{1}{3}\iint_S (|x|+|y|+|z|)\,\mathrm{d}S=\frac{1}{3}\iint_S \mathrm{d}S.$$

闭曲面 $S$ 由八块等边三角形组成（每个卦限一块，如 $x+y+z=1$），等边三角形边长为 $\sqrt{2}$，故 $S$ 的面积为 $8\cdot\dfrac{1}{2}\cdot(\sqrt{2})^2\cdot\sin\dfrac{\pi}{3}=4\sqrt{3}$，所以 $I=\dfrac{1}{3}\times 4\sqrt{3}=\dfrac{4\sqrt{3}}{3}$．

+++

#### 基础填空 (6) 设 $L$ 为点 $(1,-1,2)$ 到点 $(2,1,3)$ 的直线段，则 $I=\int_L (x^2+y^2+z^2)\,\mathrm{d}s=$ ________．
***
$9\sqrt{6}$．

两点连线 $L$ 的方向向量为 $\boldsymbol{S}=(1,2,1)$，故 $L$ 的方程为

$$\frac{x-1}{1}=\frac{y+1}{2}=\frac{z-2}{1},\quad 1\leqslant x\leqslant 2,$$

其参数方程为 $\begin{cases}x=1+t,\\ y=-1+2t,\\ z=2+t\end{cases}(0\leqslant t\leqslant 1)$，则 $\mathrm{d}s=\sqrt{x'^2(t)+y'^2(t)+z'^2(t)}\,\mathrm{d}t=\sqrt{6}\,\mathrm{d}t$，故

$$I=\int_L (x^2+y^2+z^2)\,\mathrm{d}s=\int_0^1 \sqrt{6}\left[(1+t)^2+(-1+2t)^2+(2+t)^2\right]\mathrm{d}t$$

$$=\sqrt{6}\int_0^1 (6+2t+6t^2)\,\mathrm{d}t=9\sqrt{6}.$$

+++

#### 基础解答 (1) 设 $L$ 为由 $r=a\ (a>0)$，$\theta=0$ 和 $\theta=\dfrac{\pi}{4}$ 所围凸平面区域的边界，$(r,\theta)$ 为极坐标，计算 $I=\int_L \mathrm{e}^{\sqrt{x^2+y^2}}\,\mathrm{d}s$．
***
计算第一类曲线积分时要化为定积分，关键是正确写出积分曲线的参数方程．

$L$ 由三条曲线 $L_1$（$x$ 轴上从 $O$ 到 $(a,0)$ 的线段）、$L_2$（圆弧 $r=a$，$0\leqslant\theta\leqslant\dfrac{\pi}{4}$）、$L_3$（射线 $\theta=\dfrac{\pi}{4}$ 上从 $\left(\dfrac{\sqrt{2}}{2}a,\dfrac{\sqrt{2}}{2}a\right)$ 回到 $O$ 的线段）构成．

$L_1:\begin{cases}y=0,\\ x=x,\end{cases}\mathrm{d}s=\mathrm{d}x$，则 $\displaystyle\int_{L_1}\mathrm{e}^{\sqrt{x^2+y^2}}\,\mathrm{d}s=\int_0^a \mathrm{e}^x\,\mathrm{d}x=\mathrm{e}^a-1$；

$L_2:\begin{cases}x=a\cos t,\\ y=a\sin t,\end{cases}0\leqslant t\leqslant\dfrac{\pi}{4}$，则

$$\int_{L_2}\mathrm{e}^{\sqrt{x^2+y^2}}\,\mathrm{d}s=\int_0^{\frac{\pi}{4}}\mathrm{e}^a\sqrt{a^2\sin^2 t+a^2\cos^2 t}\,\mathrm{d}t=\frac{\pi}{4}a\mathrm{e}^a;$$

$L_3:\begin{cases}y=x,\\ x=x,\end{cases}\mathrm{d}s=\sqrt{1^2+1^2}\,\mathrm{d}x=\sqrt{2}\,\mathrm{d}x$，则

$$\int_{L_3}\mathrm{e}^{\sqrt{x^2+y^2}}\,\mathrm{d}s=\int_0^{\frac{\sqrt{2}}{2}a}\mathrm{e}^{\sqrt{2}x}\cdot\sqrt{2}\,\mathrm{d}x=\mathrm{e}^a-1,$$

故

$$I=\mathrm{e}^a-1+\frac{\pi}{4}a\mathrm{e}^a+\mathrm{e}^a-1=\left(\frac{\pi}{4}a+2\right)\mathrm{e}^a-2.$$

【注】计算第一类曲线积分 $\int_L f(x,y,z)\,\mathrm{d}s$ 应掌握：\
① 计算公式，写出 $L$ 的参数方程，化为定积分计算，即“变量参数化，计算定积分，上限大于下限”；\
② 将 $L$ 的方程代入被积函数化简；\
③ 对称性包括奇偶性和轮换对称性（与二重积分、三重积分对称性类似）．

+++

#### 基础解答 (2) 设 $L$ 为曲线 $y=1-|1-x|$ 从对应于 $x=0$ 的点到 $x=2$ 的点，计算 $I=\int_L (x^2+y^2)\,\mathrm{d}x+(x^2-y^2)\,\mathrm{d}y$．
***
$L$ 由 $L_1:y=x$（$0\leqslant x\leqslant 1$）和 $L_2:y=2-x$（$1\leqslant x\leqslant 2$）构成．

在 $L_1$ 上，$y=x$，则 $\mathrm{d}y=\mathrm{d}x$，故

$$\int_{L_1}(x^2+y^2)\,\mathrm{d}x+(x^2-y^2)\,\mathrm{d}y=\int_{L_1}(x^2+y^2)\,\mathrm{d}x+0=2\int_0^1 x^2\,\mathrm{d}x=\frac{2}{3};$$

在 $L_2$ 上，$y=2-x$，则 $\mathrm{d}x=-\mathrm{d}y$，故

$$\int_{L_2}(x^2+y^2)\,\mathrm{d}x+(x^2-y^2)\,\mathrm{d}y=0-2\int_1^0 y^2\,\mathrm{d}y=\frac{2}{3},$$

故

$$\int_L (x^2+y^2)\,\mathrm{d}x+(x^2-y^2)\,\mathrm{d}y=\frac{2}{3}+\frac{2}{3}=\frac{4}{3}.$$

【注】在 $L_1:y=x$ 上，显然 $\int_{L_1}(x^2-y^2)\,\mathrm{d}y=0$．

+++

#### 基础解答 (3) 设 $L$ 为 $\left(x-\dfrac{1}{2}\right)^2+y^2=\dfrac{1}{4}\ (y\geqslant 0)$ 上从点 $O(0,0)$ 到点 $A(1,0)$ 的一段弧，计算 $I=\int_L [3+(2-\sqrt{2})y+\mathrm{e}^x\sin y]\,\mathrm{d}x+(\sqrt{2}x+\mathrm{e}^x\cos y)\,\mathrm{d}y$．
***
记 $P=3+(2-\sqrt{2})y+\mathrm{e}^x\sin y$，$Q=\sqrt{2}x+\mathrm{e}^x\cos y$，则

$$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=2\sqrt{2}-2.$$

加线段 $\overline{AO}:\begin{cases}y=0,\\ x=x,\end{cases}$ 即 $x$ 轴上从 $A(1,0)$ 到 $O(0,0)$ 的线段，$L$ 与线段 $\overline{AO}$ 构成闭区域 $D$（上半圆盘，半径 $\dfrac{1}{2}$）．利用格林公式，得

$$I=-\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y-\int_{\overline{AO}}[3+(2-\sqrt{2})y+\mathrm{e}^x\sin y]\,\mathrm{d}x+(\sqrt{2}x+\mathrm{e}^x\cos y)\,\mathrm{d}y$$

$$=-\iint_D (2\sqrt{2}-2)\,\mathrm{d}x\mathrm{d}y+\int_0^1 3\,\mathrm{d}x=(2-2\sqrt{2})\times\frac{1}{2}\times\pi\times\left(\frac{1}{2}\right)^2+3=\frac{(1-\sqrt{2})\pi}{4}+3.$$

【注】此题利用格林公式时，由于 $L+\overline{AO}$ 是顺时针方向，所以应取“$-$”号．

+++

#### 基础解答 (4) 计算积分 $I=\oint_L \dfrac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}$，其中

（Ⅰ）$L$ 为 $(x+2)^2+(y-2)^2=1$，取逆时针方向；\
（Ⅱ）$L$ 为 $x^2+y^2=1$，取逆时针方向；\
（Ⅲ）$L$ 为 $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}=1$，取逆时针方向．
***
（Ⅰ）记 $P=\dfrac{-y}{x^2+y^2}$，$Q=\dfrac{x}{x^2+y^2}$，则 $P$ 与 $Q$ 在 $D_1:(x+2)^2+(y-2)^2\leqslant 1$ 上有一阶连续偏导数，且

$$\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}=\frac{y^2-x^2}{(x^2+y^2)^2}.$$

由格林公式，得 $I=\oint_L \dfrac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\iint_{D_1}\left(\dfrac{\partial Q}{\partial x}-\dfrac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=0$．

（Ⅱ）由于 $P$ 与 $Q$ 及 $\dfrac{\partial Q}{\partial x}$ 和 $\dfrac{\partial P}{\partial y}$ 在 $x^2+y^2<1$ 内的点 $(0,0)$ 处没有定义，所以不能直接利用格林公式，直接利用 $L$ 的参数方程 $\begin{cases}x=\cos t,\\ y=\sin t\end{cases}$ 计算，得

$$I=\oint_L \frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\int_0^{2\pi}\frac{\cos^2 t+\sin^2 t}{1}\,\mathrm{d}t=2\pi.$$

（Ⅲ）由于 $P$ 与 $Q$ 及 $\dfrac{\partial Q}{\partial x}$ 和 $\dfrac{\partial P}{\partial y}$ 在椭圆 $\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}<1$ 内的点 $(0,0)$ 处没有定义，故不能直接利用格林公式．考虑在 $L:\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}=1$ 内作一个半径充分小的圆 $L_{r^-}:\begin{cases}x=r\cos t,\\ y=r\sin t,\end{cases}$ 取顺时针方向，$|r|\ll 1\ (0\leqslant t\leqslant 2\pi)$，挖去点 $(0,0)$，在 $L+L_{r^-}$ 所围的区域 $D_2$ 上用格林公式，得

$$\oint_{L+L_{r^-}}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\iint_{D_2}\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=\iint_{D_2}0\,\mathrm{d}x\mathrm{d}y=0,$$

故

$$I=\oint_L \frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\oint_{L_r}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\int_0^{2\pi}\frac{r^2(\cos^2 t+\sin^2 t)}{r^2}\,\mathrm{d}t=2\pi,$$

其中 $L_r$ 为逆时针方向．

+++

#### 基础解答 (5) 设 $L:x^2+y^2=R^2\ (R>1)$，取逆时针方向，计算 $I=\oint_L \dfrac{x\,\mathrm{d}y-y\,\mathrm{d}x}{4x^2+9y^2}$．
***
记 $P=\dfrac{-y}{4x^2+9y^2}$，$Q=\dfrac{x}{4x^2+9y^2}$，则 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}=\dfrac{9y^2-4x^2}{(4x^2+9y^2)^2}$．

由于 $P$ 与 $Q$ 及 $\dfrac{\partial Q}{\partial x}$ 和 $\dfrac{\partial P}{\partial y}$ 在 $x^2+y^2<R^2$ 内的点 $(0,0)$ 处没有定义，不能直接利用格林公式，考虑到被积表达式的分母为 $4x^2+9y^2$，在 $x^2+y^2=R^2$ 内部作一个小的椭圆

$$L_{r^-}:\begin{cases}x=\dfrac{1}{2}r\cos t,\\[2pt] y=\dfrac{1}{3}r\sin t,\end{cases}$$

$r$ 充分小，取顺时针方向，则在 $L+L_{r^-}$ 所围区域 $D$ 上用格林公式，有

$$\oint_{L+L_{r^-}}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{4x^2+9y^2}=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=0,$$

故

$$I=\oint_L \frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{4x^2+9y^2}=\oint_{L_r}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{4x^2+9y^2}=\frac{1}{r^2}\oint_{L_r}x\,\mathrm{d}y-y\,\mathrm{d}x=\int_0^{2\pi}\frac{1}{6}(\cos^2 t+\sin^2 t)\,\mathrm{d}t=\frac{\pi}{3},$$

其中 $L_r$ 为逆时针方向．

+++

#### 基础解答 (6) 设曲线 $L:x^2+y^2=R^2\ (R>0)$，取逆时针方向，问 $R$ 为何值时，积分 $I(R)=\oint_L y^3\,\mathrm{d}x+(3x-x^3)\,\mathrm{d}y$ 取得最大值，并求最大值．
***
$L$ 为闭曲线，利用格林公式，记 $P=y^3$，$Q=3x-x^3$，

$$I(R)=\oint_L y^3\,\mathrm{d}x+(3x-x^3)\,\mathrm{d}y=\iint_D (3-3x^2-3y^2)\,\mathrm{d}x\mathrm{d}y$$

$$=3\iint_D (1-x^2-y^2)\,\mathrm{d}x\mathrm{d}y=3\int_0^{2\pi}\mathrm{d}\theta\int_0^R (1-r^2)r\,\mathrm{d}r$$

$$=6\pi\left(\frac{r^2}{2}-\frac{r^4}{4}\right)\Big|_0^R=3\pi\left(R^2-\frac{R^4}{2}\right).$$

由 $\dfrac{\mathrm{d}[I(R)]}{\mathrm{d}R}=6\pi(R-R^3)=0$，得 $R=1$，且

$$\frac{\mathrm{d}^2[I(R)]}{\mathrm{d}R^2}\bigg|_{R=1}=6\pi(1-3R^2)\big|_{R=1}=-12\pi<0,$$

故 $R=1$ 是唯一极大值点，也是最大值点，最大值为 $I(1)=\dfrac{3}{2}\pi$．

+++

#### 基础解答 (7) 设 $f(x)$ 有一阶连续导数，曲线积分 $\int_L [f(x)-\mathrm{e}^x]\sin y\,\mathrm{d}x-f(x)\cos y\,\mathrm{d}y$ 与路径无关，且 $f(0)=0$，求 $f(x)$．
***
记 $P=[f(x)-\mathrm{e}^x]\sin y$，$Q=-f(x)\cos y$．依题意，有 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，即

$$-f'(x)\cos y=[f(x)-\mathrm{e}^x]\cos y,$$

又 $\cos y$ 不恒为零，故 $\begin{cases}f'(x)+f(x)=\mathrm{e}^x,\\ f(0)=0.\end{cases}$

一阶线性微分方程的通解为

$$f(x)=\mathrm{e}^{-\int \mathrm{d}x}\left[\int \mathrm{e}^x\cdot \mathrm{e}^{\int \mathrm{d}x}\,\mathrm{d}x+C\right]=\mathrm{e}^{-x}\left(\frac{1}{2}\mathrm{e}^{2x}+C\right).$$

由 $f(0)=0$，得 $C=-\dfrac{1}{2}$，故 $f(x)=\dfrac{1}{2}(\mathrm{e}^x-\mathrm{e}^{-x})$．

+++

#### 基础解答 (8) 设平面力场为 $\boldsymbol{F}=(2xy^3-y^2\cos x)\boldsymbol{i}+(1-2y\sin x+3x^2y^2)\boldsymbol{j}$，求质点在 $\boldsymbol{F}$ 作用下，沿 $L:2x=\pi y^2$ 从点 $O(0,0)$ 到点 $A\left(\dfrac{\pi}{2},1\right)$ 所做的功 $W$．
***
依题意，有

$$W=\int_L \boldsymbol{F}\cdot\mathrm{d}\boldsymbol{S}=\int_L (2xy^3-y^2\cos x)\,\mathrm{d}x+(1-2y\sin x+3x^2y^2)\,\mathrm{d}y.$$

选取 $y$ 为参数，则 $L:\begin{cases}x=\dfrac{\pi}{2}y^2,\\ y=y,\end{cases}$ $y$ 从 $0$ 到 $1$，故

$$W=\int_0^1\left[\left(2\cdot\frac{\pi}{2}\cdot y^2\cdot y^3-y^2\cos\frac{\pi}{2}y^2\right)\pi y+1-2y\sin\frac{\pi}{2}y^2+3\cdot\left(\frac{\pi}{2}\right)^2 y^4\cdot y^2\right]\mathrm{d}y=\frac{\pi^2}{4}.$$

+++

#### 基础解答 (9) 计算 $I=\int_L \dfrac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}$，其中 $L$ 是从点 $A(1,1)$ 沿直线到点 $B(-1,0)$，再沿曲线 $y=x^2-1$ 到点 $C(1,0)$．
***
**解法 1** 因为 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}=\dfrac{y^2-x^2}{(x^2+y^2)^2}$，所以在不含点 $(0,0)$ 的区域内，积分与路径无关．取折线路径 $A(1,1)\to D(-1,1)\to B(-1,0)$，再由 $B$ 沿上半单位圆 $\overparen{BEC}$（经 $E(0,-1)$ 的下半圆弧）到 $C$，即

$$\overline{AD}:\begin{cases}y=1,\\ x=x,\end{cases}\quad \overline{DB}:\begin{cases}x=-1,\\ y=y,\end{cases}\quad \overparen{BEC}:\begin{cases}x=\cos t,\\ y=\sin t,\end{cases}$$

故

$$I=\int_1^{-1}\frac{-\mathrm{d}x}{1+x^2}+\int_1^0\frac{-\mathrm{d}y}{1+y^2}+\int_{\pi}^{2\pi}\frac{\cos^2 t+\sin^2 t}{1}\,\mathrm{d}t$$

$$=-\left(-\frac{\pi}{4}-\frac{\pi}{4}\right)-\left(0-\frac{\pi}{4}\right)+(2\pi-\pi)=\frac{7\pi}{4}.$$

**解法 2** 用格林公式．连接 $\overline{CA}:\begin{cases}x=1,\\ y=y,\end{cases}$ 取小圆 $l:\begin{cases}x=\delta\cos t,\\ y=\delta\sin t\end{cases}$（$\delta$ 充分小）取顺时针方向，则

$$I=\int_L \frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\oint_{\overparen{ABECA}}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}-\int_{\overline{CA}}-\oint_{l_{\text{顺}}},$$

$$\oint_{\overparen{ABECA}}\frac{x\,\mathrm{d}y-y\,\mathrm{d}x}{x^2+y^2}=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=0,$$

故

$$I=\oint_{l_{\text{逆}}}-\int_{\overline{CA}}=\int_0^{2\pi}\frac{\delta^2}{\delta^2}\,\mathrm{d}t-\int_0^1\frac{\mathrm{d}y}{1+y^2}=2\pi-\frac{\pi}{4}=\frac{7\pi}{4}.$$

【注】解法 1 利用积分与路径无关，不能取 $\overline{CA}$ 的原因是闭曲线 $\overparen{ABEC}+\overline{CA}$ 中含 $(0,0)$，而 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}=\dfrac{y^2-x^2}{(x^2+y^2)^2}$ 在点 $(0,0)$ 处没有意义．

+++

#### 基础解答 (10) 设 $P(x,y)=\dfrac{x(\sqrt{x^2+y^2})^k}{y}$，$Q(x,y)=-\dfrac{x^2(\sqrt{x^2+y^2})^k}{y^2}$，$D=\{(x,y)\mid y>0\}$．

（Ⅰ）若积分 $I=\int_L P\,\mathrm{d}x+Q\,\mathrm{d}y$ 在 $D$ 内与路径无关，求 $k$ 的值；\
（Ⅱ）在 $D$ 内求函数 $u(x,y)$，使得 $\mathrm{d}u=P\,\mathrm{d}x+Q\,\mathrm{d}y$，并计算 $I=\int_{(1,1)}^{(2,2)}P\,\mathrm{d}x+Q\,\mathrm{d}y$．
***
（Ⅰ）由于 $D$ 是单连通区域，且 $P(x,y)$，$Q(x,y)$ 在 $D$ 内有连续偏导数，故

$$\int_L P\,\mathrm{d}x+Q\,\mathrm{d}y\ \text{在}\ D\ \text{内与路径无关}\Rightarrow \frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y},$$

即

$$-\frac{2x}{y^2}(\sqrt{x^2+y^2})^k-\frac{x^2}{y^2}k(\sqrt{x^2+y^2})^{k-1}\cdot\frac{x}{\sqrt{x^2+y^2}}$$

$$=-\frac{x}{y^2}(\sqrt{x^2+y^2})^k+\frac{x}{y}k(\sqrt{x^2+y^2})^{k-1}\cdot\frac{y}{\sqrt{x^2+y^2}},$$

等式两边同时除以 $\dfrac{x}{y^2}(\sqrt{x^2+y^2})^{k-2}$，得 $-2(x^2+y^2)-kx^2=-(x^2+y^2)+ky^2$，即 $(k+1)(x^2+y^2)=0$，解得 $k=-1$．

（Ⅱ）由（Ⅰ）知，当 $k=-1$ 时，存在 $u(x,y)$，使得 $\mathrm{d}u=P\,\mathrm{d}x+Q\,\mathrm{d}y$．用积分求 $u(x,y)$．

由 $\dfrac{\partial u}{\partial x}=P(x,y)=\dfrac{x}{y\sqrt{x^2+y^2}}$，可知

$$u(x,y)=\int\frac{x}{y\sqrt{x^2+y^2}}\,\mathrm{d}x+\varphi_1(y)=\frac{\sqrt{x^2+y^2}}{y}+\varphi(y),$$

其中 $\varphi(y)=\varphi_1(y)+C_1$．又因为

$$\frac{\partial u}{\partial y}=-\frac{1}{y^2}\sqrt{x^2+y^2}+\frac{1}{y}\cdot\frac{y}{\sqrt{x^2+y^2}}+\varphi'(y)=\frac{-(x^2+y^2)+y^2}{y^2\sqrt{x^2+y^2}}+\varphi'(y)=\frac{-x^2}{y^2\sqrt{x^2+y^2}}+\varphi'(y)=Q(x,y),$$

所以 $\varphi'(y)=0$，即 $\varphi(y)=C$，从而有

$$u(x,y)=\frac{\sqrt{x^2+y^2}}{y}+C\quad(C\ \text{为任意常数}).$$

$$I=\int_{(1,1)}^{(2,2)}P\,\mathrm{d}x+Q\,\mathrm{d}y=u(x,y)\Big|_{(1,1)}^{(2,2)}=\left(\frac{\sqrt{x^2+y^2}}{y}+C\right)\Big|_{(1,1)}^{(2,2)}=0.$$

+++

#### 基础解答 (11) 设曲线 $L$ 为 $z=4-x^2-y^2$ 与 $z=3$ 的交线，从 $z$ 轴正向看是逆时针方向，计算 $I=\oint_L x^2y^3\,\mathrm{d}x+z\,\mathrm{d}y+y\,\mathrm{d}z$．
***
**解法 1** 曲线 $L:\begin{cases}z=4-x^2-y^2,\\ z=3,\end{cases}$ 消去 $z$，得 $\begin{cases}x^2+y^2=1,\\ z=3,\end{cases}$ 故其参数方程为 $\begin{cases}x=\cos t,\\ y=\sin t,\\ z=3\end{cases}(0\leqslant t\leqslant 2\pi)$．

$$I=\oint_L x^2y^3\,\mathrm{d}x+z\,\mathrm{d}y+y\,\mathrm{d}z=\int_0^{2\pi}\left[\cos^2 t\sin^3 t(-\sin t)+3\cos t+0\right]\mathrm{d}t=-\frac{\pi}{8}.$$

**解法 2** 利用斯托克斯公式，考虑 $L$ 在平面 $z=3$ 上，则

$$I=\oint_L x^2y^3\,\mathrm{d}x+z\,\mathrm{d}y+y\,\mathrm{d}z=\iint_S\begin{vmatrix}\cos\alpha&\cos\beta&\cos\gamma\\ \dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\ x^2y^3&z&y\end{vmatrix}\mathrm{d}S.$$

由 $z=3$，知单位法向量为 $(\cos\alpha,\cos\beta,\cos\gamma)=(0,0,1)$，故

$$I=\iint_S\begin{vmatrix}0&0&1\\ \dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\ x^2y^3&z&y\end{vmatrix}\mathrm{d}S=-\iint_S 3x^2y^2\,\mathrm{d}S.$$

对 $S:z=3$，有 $\mathrm{d}S=\sqrt{1+z'^2_x+z'^2_y}\,\mathrm{d}x\mathrm{d}y=\mathrm{d}x\mathrm{d}y$，故

$$I=-\iint_{D_{xy}}3x^2y^2\,\mathrm{d}x\mathrm{d}y=-3\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r^2\cos^2\theta\cdot r^2\sin^2\theta\cdot r\,\mathrm{d}r$$

$$=-3\int_0^{2\pi}\cos^2\theta\sin^2\theta\,\mathrm{d}\theta\int_0^1 r^5\,\mathrm{d}r=-\frac{1}{2}\int_0^{2\pi}(1-\sin^2\theta)\sin^2\theta\,\mathrm{d}\theta$$

$$=-\frac{1}{2}\left(\int_0^{2\pi}\sin^2\theta\,\mathrm{d}\theta-\int_0^{2\pi}\sin^4\theta\,\mathrm{d}\theta\right)=-\frac{\pi}{8},$$

其中 $D_{xy}:x^2+y^2\leqslant 1$．

【注】① 计算空间曲线积分常有两种方法：\
（i）利用参数方程化为定积分计算；\
（ii）对于空间闭曲线 $L$，可利用斯托克斯公式．\
② 结论：$\int_0^{2\pi}\sin^n\theta\,\mathrm{d}\theta=4\int_0^{\frac{\pi}{2}}\sin^n\theta\,\mathrm{d}\theta$，如 $\int_0^{2\pi}\sin^2\theta\,\mathrm{d}\theta=4\int_0^{\frac{\pi}{2}}\sin^2\theta\,\mathrm{d}\theta$，$\int_0^{2\pi}\sin^4\theta\,\mathrm{d}\theta=4\int_0^{\frac{\pi}{2}}\sin^4\theta\,\mathrm{d}\theta$（见《李林考研数学系列高等数学辅导讲义》）．\
③ 此题也可将 $z=3$ 代入被积表达式，消去 $\mathrm{d}z$，化为平面曲线积分：$I=\oint_L x^2y^3\,\mathrm{d}x+z\,\mathrm{d}y+y\,\mathrm{d}z=\oint_{L_1}x^2y^3\,\mathrm{d}x+3\,\mathrm{d}y\ (L_1:x^2+y^2=1)$．由格林公式，知 $I=\oint_{L_1}x^2y^3\,\mathrm{d}x+3\,\mathrm{d}y=-\iint_{D_{xy}}3x^2y^2\,\mathrm{d}x\mathrm{d}y=-\dfrac{\pi}{8}$．

+++

#### 基础解答 (12) 计算 $I=\iint_S f(x,y,z)\,\mathrm{d}S$，其中 $S:x^2+y^2+z^2=1$，

$$f(x,y,z)=\begin{cases}x^2+y^2, & z\geqslant\sqrt{x^2+y^2},\\ 0, & z<\sqrt{x^2+y^2}.\end{cases}$$
***
被积函数只在锥面 $z=\sqrt{x^2+y^2}$ 以上的球冠部分不为零，该球冠在 $xOy$ 面上的投影为 $D_{xy}:x^2+y^2\leqslant\dfrac{1}{2}$（即 $r\leqslant\dfrac{1}{\sqrt{2}}$），此时 $z=\sqrt{1-x^2-y^2}$，故

$$I=\iint_{D_{xy}}(x^2+y^2)\sqrt{1+z'^2_x+z'^2_y}\,\mathrm{d}x\mathrm{d}y=\iint_{D_{xy}}(x^2+y^2)\cdot\frac{1}{\sqrt{1-x^2-y^2}}\,\mathrm{d}x\mathrm{d}y$$

$$\xlongequal{\text{极坐标}}\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{1}{\sqrt{2}}}\frac{r^3}{\sqrt{1-r^2}}\,\mathrm{d}r=2\pi\int_0^{\frac{1}{\sqrt{2}}}\frac{r^3}{\sqrt{1-r^2}}\,\mathrm{d}r$$

$$\xlongequal{r=\sin t}2\pi\int_0^{\frac{\pi}{4}}\frac{\sin^3 t}{\cos t}\cdot\cos t\,\mathrm{d}t=2\pi\int_0^{\frac{\pi}{4}}\sin^3 t\,\mathrm{d}t$$

$$=2\pi\int_0^{\frac{\pi}{4}}\sin^2 t\cdot\mathrm{d}(-\cos t)=\frac{8-5\sqrt{2}}{6}\pi.$$

+++

#### 基础解答 (13) 设曲面 $S$ 为上半圆锥 $z=\sqrt{x^2+y^2}$ 被圆柱面 $x^2+y^2=2ax\ (a>0)$ 所截出的有限部分，计算 $I=\iint_S (x^2y+yz^2+z^2x)\,\mathrm{d}S$．
***
曲面 $S$ 关于 $xOz$ 面对称，$x^2y$ 和 $yz^2$ 关于 $y$ 是奇函数，故 $\iint_S x^2y\,\mathrm{d}S=\iint_S yz^2\,\mathrm{d}S=0$．

由 $z=\sqrt{x^2+y^2}$，得 $\mathrm{d}S=\sqrt{1+z'^2_x+z'^2_y}\,\mathrm{d}x\mathrm{d}y=\sqrt{2}\,\mathrm{d}x\mathrm{d}y$，故（投影区域 $D_{xy}:x^2+y^2\leqslant 2ax$，极坐标下 $-\dfrac{\pi}{2}\leqslant\theta\leqslant\dfrac{\pi}{2}$，$0\leqslant r\leqslant 2a\cos\theta$）

$$I=\iint_S (x^2y+yz^2+z^2x)\,\mathrm{d}S=0+0+\iint_S z^2x\,\mathrm{d}S=\sqrt{2}\iint_{D_{xy}}x(x^2+y^2)\,\mathrm{d}x\mathrm{d}y$$

$$=\sqrt{2}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{2a\cos\theta}r\cos\theta\cdot r^2\cdot r\,\mathrm{d}r=\sqrt{2}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\cos\theta\,\mathrm{d}\theta\int_0^{2a\cos\theta}r^4\,\mathrm{d}r$$

$$=\frac{\sqrt{2}}{5}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\cos\theta\cdot(2a)^5\cdot\cos^5\theta\,\mathrm{d}\theta=\frac{\sqrt{2}\cdot(2a)^5}{5}\cdot 2\int_0^{\frac{\pi}{2}}\cos^6\theta\,\mathrm{d}\theta$$

$$=\frac{\sqrt{2}(2a)^5}{5}\cdot 2\cdot\frac{5}{6}\cdot\frac{3}{4}\cdot\frac{1}{2}\cdot\frac{\pi}{2}=2\sqrt{2}a^5\pi.$$

+++

#### 基础解答 (14) 设 $S$ 为 $z=x^2+y^2$ 介于 $z=0$ 与 $z=1$ 之间部分的下侧，计算 $I=\iint_S x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y$．
***
**解法 1** 利用高斯公式．添加曲面 $S_1:z=1\ (x^2+y^2\leqslant 1)$，取上侧，有

$$I=\iint_{S+S_1}x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y-\iint_{S_1}x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y\quad(S+S_1\ \text{为闭曲面，取外侧}).$$

由于

$$\iint_{S+S_1}x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=\iiint_V (2x+1)\,\mathrm{d}V\xlongequal{\text{柱面坐标}}\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\,\mathrm{d}r\int_{r^2}^1(2r\cos\theta+1)\,\mathrm{d}z=\frac{\pi}{2},$$

$$\iint_{S_1}x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=\iint_{D_{xy}}1\,\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\,\mathrm{d}r=\pi,$$

其中 $D_{xy}=\{(x,y)\mid x^2+y^2\leqslant 1\}$，故 $I=\dfrac{\pi}{2}-\pi=-\dfrac{\pi}{2}$．

**解法 2** 投影法．$S:z=x^2+y^2$ 下侧的法向量为 $\boldsymbol{n}=(2x,2y,-1)$，方向余弦为

$$\cos\alpha=\frac{2x}{\sqrt{(2x)^2+(2y)^2+(-1)^2}},\quad \cos\gamma=\frac{-1}{\sqrt{(2x)^2+(2y)^2+(-1)^2}}.$$

由 $\dfrac{\mathrm{d}y\mathrm{d}z}{\cos\alpha}=\dfrac{\mathrm{d}z\mathrm{d}x}{\cos\beta}=\dfrac{\mathrm{d}x\mathrm{d}y}{\cos\gamma}=\mathrm{d}S$（转换公式），可知 $\mathrm{d}y\mathrm{d}z=\dfrac{\cos\alpha}{\cos\gamma}\mathrm{d}x\mathrm{d}y=(-2x)\,\mathrm{d}x\mathrm{d}y$，故

$$I=\iint_S x^2\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=\iint_S [x^2\cdot(-2x)+z]\,\mathrm{d}x\mathrm{d}y=-\iint_{D_{xy}}(-2x^3+x^2+y^2)\,\mathrm{d}x\mathrm{d}y,$$

其中 $D_{xy}=\{(x,y)\mid x^2+y^2\leqslant 1\}$，$x^3$ 为奇函数，从而

$$I=2\iint_{D_{xy}}x^3\,\mathrm{d}x\mathrm{d}y-\iint_{D_{xy}}(x^2+y^2)\,\mathrm{d}x\mathrm{d}y=0-\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r^2\cdot r\,\mathrm{d}r=-\frac{\pi}{2}.$$

【注】此题若取 $S:z=x^2+y^2$ 上侧，则法向量取 $\boldsymbol{n}=(-2x,-2y,1)$．

+++

#### 基础解答 (15) 设曲面 $S:z=x^2+y^2\ (0\leqslant z\leqslant 1)$，取上侧，计算 $I=\iint_S (x+1)\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y$．
***
**解法 1**（投影法）记 $I=\iint_S (x+1)\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=I_1+I_2$．

将 $S$ 分为前、后两片（$x=\pm\sqrt{z-y^2}$），在 $yOz$ 面上的投影区域为 $D_{yz}$，则

$$I_1=\iint_S (x+1)\,\mathrm{d}y\mathrm{d}z=\iint_{S_{\text{前}}}(x+1)\,\mathrm{d}y\mathrm{d}z+\iint_{S_{\text{后}}}(x+1)\,\mathrm{d}y\mathrm{d}z$$

$$=-\iint_{D_{yz}}\sqrt{z-y^2}\,\mathrm{d}y\mathrm{d}z+\iint_{D_{yz}}(-\sqrt{z-y^2})\,\mathrm{d}y\mathrm{d}z=-2\iint_{D_{yz}}\sqrt{z-y^2}\,\mathrm{d}y\mathrm{d}z$$

$$=-2\int_{-1}^1\mathrm{d}y\int_{y^2}^1\sqrt{z-y^2}\,\mathrm{d}z=-2\int_{-1}^1\frac{2}{3}(z-y^2)^{\frac{3}{2}}\Big|_{y^2}^1\mathrm{d}y=-2\int_{-1}^1\frac{2}{3}(1-y^2)^{\frac{3}{2}}\,\mathrm{d}y$$

$$=-\frac{4}{3}\cdot 2\int_0^1(1-y^2)^{\frac{3}{2}}\,\mathrm{d}y\xlongequal{y=\sin t}-\frac{4}{3}\cdot 2\int_0^{\frac{\pi}{2}}\cos^4 t\,\mathrm{d}t=-\frac{4}{3}\times 2\times\frac{3}{4}\times\frac{1}{2}\times\frac{\pi}{2}=-\frac{\pi}{2},$$

$$I_2=\iint_S z\,\mathrm{d}x\mathrm{d}y=\iint_{D_{xy}}(x^2+y^2)\,\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r^2\cdot r\,\mathrm{d}r=2\pi\times\frac{1}{4}=\frac{\pi}{2},$$

故 $I=I_1+I_2=-\dfrac{\pi}{2}+\dfrac{\pi}{2}=0$．

**解法 2**（转换公式法）$\dfrac{\mathrm{d}y\mathrm{d}z}{\cos\alpha}=\dfrac{\mathrm{d}z\mathrm{d}x}{\cos\beta}=\dfrac{\mathrm{d}x\mathrm{d}y}{\cos\gamma}=\mathrm{d}S$．曲面 $S:z=x^2+y^2$ 上侧的法向量为 $\boldsymbol{n}=(-2x,-2y,1)$，故

$$\cos\alpha=\frac{-2x}{\sqrt{1+4x^2+4y^2}},\quad \cos\beta=\frac{-2y}{\sqrt{1+4x^2+4y^2}},\quad \cos\gamma=\frac{1}{\sqrt{1+4x^2+4y^2}},$$

所以 $\mathrm{d}y\mathrm{d}z=\dfrac{\cos\alpha}{\cos\gamma}\mathrm{d}x\mathrm{d}y=(-2x)\,\mathrm{d}x\mathrm{d}y$，故

$$I=\iint_S [(x+1)\cdot(-2x)+z]\,\mathrm{d}x\mathrm{d}y=\iint_S (-2x^2+z)\,\mathrm{d}x\mathrm{d}y$$

$$=\iint_{x^2+y^2\leqslant 1}[-2x^2+x^2+y^2]\,\mathrm{d}x\mathrm{d}y=\int_0^{2\pi}\mathrm{d}\theta\int_0^1 (r^2\sin^2\theta-r^2\cos^2\theta)r\,\mathrm{d}r$$

$$=\int_0^{2\pi}(\sin^2\theta-\cos^2\theta)\,\mathrm{d}\theta\int_0^1 r^3\,\mathrm{d}r=-\frac{1}{2}\sin 2\theta\Big|_0^{2\pi}\cdot\frac{1}{4}=0.$$

**解法 3**（高斯公式法）添加辅助面 $S_1:\begin{cases}z=1,\\ x^2+y^2\leqslant 1,\end{cases}$ 取下侧，则 $I=\iint_{S+S_1}-\iint_{S_1}$．又

$$\iint_{S+S_1}(x+1)\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=-\iiint_V (1+0+1)\,\mathrm{d}V\xlongequal{\text{柱坐标}}-2\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\,\mathrm{d}r\int_{r^2}^1\mathrm{d}z=-\pi,$$

$$\iint_{S_1}(x+1)\,\mathrm{d}y\mathrm{d}z+z\,\mathrm{d}x\mathrm{d}y=0+\iint_{S_1}z\,\mathrm{d}x\mathrm{d}y=-\iint_{D_{xy}}1\,\mathrm{d}x\mathrm{d}y=-\int_0^{2\pi}\mathrm{d}\theta\int_0^1 r\,\mathrm{d}r=-\pi,$$

故 $I=-\pi-(-\pi)=0$．

【注】计算第二类曲面积分有三种方法：法 1：投影法；法 2：转换公式法；法 3：高斯公式（见《李林考研数学系列高等数学辅导讲义》）．以上三种解法中，高斯公式法较简单．

+++

#### 基础解答 (16) 设 $S$ 为曲面 $4-y=x^2+z^2$ 上 $y\geqslant 0$ 的部分，取外侧，计算 $I=\iint_S yz\,\mathrm{d}y\mathrm{d}z+(x^2+z^2)y\,\mathrm{d}z\mathrm{d}x+xy\,\mathrm{d}x\mathrm{d}y$．
***
添加辅助面 $S_1:\begin{cases}y=0,\\ x^2+z^2\leqslant 4,\end{cases}$ 取左侧，在 $S_1$ 上，$\iint_{S_1}yz\,\mathrm{d}y\mathrm{d}z+(x^2+z^2)y\,\mathrm{d}z\mathrm{d}x+xy\,\mathrm{d}x\mathrm{d}y=0$．

利用高斯公式，有

$$I=\iint_{S+S_1}yz\,\mathrm{d}y\mathrm{d}z+(x^2+z^2)y\,\mathrm{d}z\mathrm{d}x+xy\,\mathrm{d}x\mathrm{d}y-\iint_{S_1}yz\,\mathrm{d}y\mathrm{d}z+(x^2+z^2)y\,\mathrm{d}z\mathrm{d}x+xy\,\mathrm{d}x\mathrm{d}y$$

$$=\iiint_V (x^2+z^2)\,\mathrm{d}V\xlongequal{\text{先二后一}}\int_0^4\mathrm{d}y\int_0^{2\pi}\mathrm{d}\theta\int_0^{\sqrt{4-y}}r^2\cdot r\,\mathrm{d}r=\frac{\pi}{2}\int_0^4 (4-y)^2\,\mathrm{d}y=\frac{32}{3}\pi.$$

+++

#### 基础解答 (17) 设曲面为 $z=\sqrt{x^2+y^2}$ 介于 $z=1$ 与 $z=2$ 之间的部分，取上侧，计算 $I=\iint_S xz^2\,\mathrm{d}y\mathrm{d}z+y^2\,\mathrm{d}z\mathrm{d}x+zx\,\mathrm{d}x\mathrm{d}y$．
***
为了利用高斯公式，添加辅助面 $S_1:\begin{cases}z=2,\\ x^2+y^2\leqslant 4,\end{cases}$ 取下侧；$S_2:\begin{cases}z=1,\\ x^2+y^2\leqslant 1,\end{cases}$ 取上侧，则

$$I=\iint_{S+S_1+S_2}-\iint_{S_1}-\iint_{S_2}.$$

而

$$\iint_{S+S_1+S_2}xz^2\,\mathrm{d}y\mathrm{d}z+y^2\,\mathrm{d}z\mathrm{d}x+zx\,\mathrm{d}x\mathrm{d}y=-\iiint_V (z^2+2y+x)\,\mathrm{d}x\mathrm{d}y\mathrm{d}z=-\int_1^2 z^2\,\mathrm{d}z\iint_{D_z}\mathrm{d}x\mathrm{d}y$$

$$=-\int_1^2 z^2\cdot\pi z^2\,\mathrm{d}z=-\frac{31\pi}{5}\quad(\text{这里利用了}\ 2y\ \text{与}\ x\ \text{是奇函数}).$$

又

$$\iint_{S_1}xz^2\,\mathrm{d}y\mathrm{d}z+y^2\,\mathrm{d}z\mathrm{d}x+zx\,\mathrm{d}x\mathrm{d}y=0+0+\iint_{x^2+y^2\leqslant 4}2x\,\mathrm{d}x\mathrm{d}y=0+0+0=0,$$

$$\iint_{S_2}xz^2\,\mathrm{d}y\mathrm{d}z+y^2\,\mathrm{d}z\mathrm{d}x+zx\,\mathrm{d}x\mathrm{d}y=0+0+\iint_{x^2+y^2\leqslant 1}x\,\mathrm{d}x\mathrm{d}y=0+0+0=0,$$

故 $I=-\dfrac{31\pi}{5}$．

【注】$\iint_{S_1}xz^2\,\mathrm{d}y\mathrm{d}z+y^2\,\mathrm{d}z\mathrm{d}x+zx\,\mathrm{d}x\mathrm{d}y=\iint_{S_1}xz^2\,\mathrm{d}y\mathrm{d}z+\iint_{S_1}y^2\,\mathrm{d}z\mathrm{d}x+\iint_{S_1}zx\,\mathrm{d}x\mathrm{d}y\xlongequal{\text{记}}I_1+I_2+I_3$．计算 $I_1$，$I_1=\iint_{S_1}xz^2\,\mathrm{d}y\mathrm{d}z=\iint_{D_{yz}}x\cdot z^2\,\mathrm{d}y\mathrm{d}z$，由于 $S_1$ 投影到 $yOz$ 面是一条线段，故 $I_1=0$，同理 $I_2=\iint_{S_1}y^2\,\mathrm{d}z\mathrm{d}x=0$．

+++

#### 基础解答 (18) 设 $S$ 是 $x^2+y^2=1$，$z=-1$，$z=1$ 所围成的圆柱体的全表面，计算 $I=\iint_{S_{\text{外}}}\dfrac{x\,\mathrm{d}y\mathrm{d}z+z^2\,\mathrm{d}x\mathrm{d}y}{x^2+y^2+z^2}$（$S_{\text{外}}$ 表示闭曲面取外侧）．
***
因为原点包含在 $S$ 的内部，所以不能直接用高斯公式，用投影法（公式）．由于 $S_{\text{外}}=S_1+S_2+S_3$（$S_1$ 为上底 $z=1$ 取上侧，$S_2$ 为下底 $z=-1$ 取下侧，$S_3$ 为侧面 $x^2+y^2=1$ 取外侧），则

$$I=\iint_{S_{\text{外}}}=\iint_{S_1}+\iint_{S_2}+\iint_{S_3}.$$

分别计算如下：

（Ⅰ）$\displaystyle\iint_{S_1}\frac{x\,\mathrm{d}y\mathrm{d}z}{x^2+y^2+z^2}=\iint_{S_2}\frac{x\,\mathrm{d}y\mathrm{d}z}{x^2+y^2+z^2}=0$；

（Ⅱ）

$$\iint_{S_1}\frac{z^2\,\mathrm{d}x\mathrm{d}y}{x^2+y^2+z^2}+\iint_{S_2}\frac{z^2\,\mathrm{d}x\mathrm{d}y}{x^2+y^2+z^2}=\iint_{D_{xy}}\frac{\mathrm{d}x\mathrm{d}y}{x^2+y^2+1}+\left(-\iint_{D_{xy}}\frac{\mathrm{d}x\mathrm{d}y}{x^2+y^2+1}\right)=0,$$

其中 $D_{xy}:x^2+y^2\leqslant 1$；

（Ⅲ）$\displaystyle\iint_{S_3}\frac{z^2\,\mathrm{d}x\mathrm{d}y}{x^2+y^2+z^2}=0$；

（Ⅳ）将侧面分为前、后两片（$x=\pm\sqrt{1-y^2}$），在 $yOz$ 面上的投影为 $D_3:-1\leqslant y\leqslant 1$，$-1\leqslant z\leqslant 1$，则

$$\iint_{S_3}\frac{x\,\mathrm{d}y\mathrm{d}z}{x^2+y^2+z^2}=\iint_{S_{3\text{前}}}\frac{x\,\mathrm{d}y\mathrm{d}z}{x^2+y^2+z^2}+\iint_{S_{3\text{后}}}\frac{x\,\mathrm{d}y\mathrm{d}z}{x^2+y^2+z^2}$$

$$=\iint_{D_3}\frac{\sqrt{1-y^2}}{1+z^2}\,\mathrm{d}y\mathrm{d}z-\iint_{D_3}\left(-\frac{\sqrt{1-y^2}}{1+z^2}\right)\mathrm{d}y\mathrm{d}z=2\iint_{D_3}\frac{\sqrt{1-y^2}}{1+z^2}\,\mathrm{d}y\mathrm{d}z$$

$$=2\int_{-1}^1\sqrt{1-y^2}\,\mathrm{d}y\int_{-1}^1\frac{\mathrm{d}z}{1+z^2}=\frac{\pi^2}{2}.$$

综上所述，$I=\dfrac{\pi^2}{2}$．

+++

#### 基础解答 (19) 一个体积为 $V$，表面积为 $S$（不含底面）的雪堆，融化速度为 $\dfrac{\mathrm{d}V}{\mathrm{d}t}=-aS$，其中 $a>0$ 为常数，设在融化期间雪堆的形状保持为 $z=h-\dfrac{x^2+y^2}{h}\ (z>0)$，其中 $h=h(t)$，问一个高度为 $h_0\ (h_0>0)$ 的雪堆全部融化需要多长时间？
***
当雪堆的高度为 $h$ 时，其体积为

$$V=\int_0^h \pi(h^2-hz)\,\mathrm{d}z=\frac{\pi h^3}{2}.$$

其表面积为

$$S=\iint_{x^2+y^2\leqslant h^2}\sqrt{1+z'^2_x+z'^2_y}\,\mathrm{d}x\mathrm{d}y=\iint_{x^2+y^2\leqslant h^2}\sqrt{1+\frac{4x^2}{h^2}+\frac{4y^2}{h^2}}\,\mathrm{d}x\mathrm{d}y$$

$$=\iint_{x^2+y^2\leqslant h^2}\frac{\sqrt{h^2+4x^2+4y^2}}{h}\,\mathrm{d}x\mathrm{d}y=\frac{1}{h}\int_0^{2\pi}\mathrm{d}\theta\int_0^h\sqrt{h^2+4r^2}\,r\,\mathrm{d}r=\frac{\pi h^2}{6}(5\sqrt{5}-1).$$

将 $V$ 和 $S$ 的表达式代入 $\dfrac{\mathrm{d}V}{\mathrm{d}t}=-aS$，得 $\dfrac{\mathrm{d}h}{\mathrm{d}t}=-\dfrac{a}{9}(5\sqrt{5}-1)$，积分得

$$h=-\frac{a}{9}(5\sqrt{5}-1)t+C.$$

由 $h\big|_{t=0}=h_0$，得 $C=h_0$，故 $h=-\dfrac{a}{9}(5\sqrt{5}-1)t+h_0$．

雪堆全部融化，即 $h=0$，所需时间为

$$t=\frac{9h_0}{a(5\sqrt{5}-1)}=\frac{9h_0(5\sqrt{5}+1)}{124a}.$$

+++

#### 综合选择 (1) 设曲线 $L$ 为 $x^2+y^2=1$，取逆时针方向，$f(x,y)>0$，$f(x,-y)=f(x,y)$. $L_1,L_2,L_3$ 如图 9-1 所示，记 $I_1=\int_{L_1}f(x,y)\mathrm{d}x$，$I_2=\int_{L_2}f(x,y)\mathrm{d}s$，$I_3=\int_{L_3}f(x,y)\mathrm{d}x$，则（　）.

（图 9-1 说明：$L$ 为单位圆周 $x^2+y^2=1$；$L_1$ 为第一象限内的弧，由 $(1,0)$ 指向 $(0,1)$，沿 $L_1$ 有 $x$ 减小；$L_2$ 为第二象限内的弧，由 $(0,1)$ 指向 $(-1,0)$；$L_3$ 为第三象限内的弧，由 $(-1,0)$ 指向 $(0,-1)$，沿 $L_3$ 有 $x$ 增大.）

;;;
A. $I_1>I_2>I_3$
B. $I_2>I_3>I_1$
C. $I_3>I_2>I_1$
D. $I_2>I_1>I_3$
;;;B
***
**B.**

由曲线积分的定义，知
$$I_1=\int_{L_1}f(x,y)\mathrm{d}x=\lim_{\lambda\to0}\sum_{i=1}^{n}f(\xi_i,\eta_i)\Delta x_i<0\quad(\text{因 }f(\xi_i,\eta_i)>0,\ \Delta x_i<0),$$
$$I_3=\int_{L_3}f(x,y)\mathrm{d}x=\lim_{\lambda\to0}\sum_{i=1}^{n}f(\xi_i,\eta_i)\Delta x_i>0\quad(\text{因 }f(\xi_i,\eta_i)>0,\ \Delta x_i>0),$$
$$I_2=\int_{L_2}f(x,y)\mathrm{d}s=\lim_{\lambda\to0}\sum_{i=1}^{n}f(\xi_i,\eta_i)\Delta s_i>I_3\quad\left(\text{因 }\Delta s_i=\sqrt{(\Delta x_i)^2+(\Delta y_i)^2}\geqslant|\Delta x_i|\right),$$
故 $I_2>I_3>I_1$.

+++

#### 综合选择 (2) 设 $L$ 为闭曲线 $|x|+|y|=1$，取逆时针方向，则 $I=\oint_L\dfrac{ax\mathrm{d}y-by\mathrm{d}x}{|x|+|y|}=$（　）.

;;;
A. $8(a+b)$
B. $2(a+b)$
C. $8(a-b)$
D. $2(a-b)$
;;;B
***
**B.**

由 $L:|x|+|y|=1$，知
$$I=\oint_L\frac{ax\mathrm{d}y-by\mathrm{d}x}{|x|+|y|}=\oint_L ax\mathrm{d}y-by\mathrm{d}x,$$
则问题转化为求 $I=\oint_L ax\mathrm{d}y-by\mathrm{d}x$.

记 $D$ 为 $|x|+|y|\leqslant1$，应用格林公式，得
$$I=\oint_L ax\mathrm{d}y-by\mathrm{d}x=\iint_D(a+b)\mathrm{d}x\mathrm{d}y=(a+b)\cdot(\sqrt{2})^2=2(a+b).$$

【注】这里将 $L:|x|+|y|=1$ 代入被积表达式是曲线积分计算中常用技巧.

+++

#### 综合选择 (3) 设 $L$ 为平面光滑简单闭曲线，取逆时针方向，$L$ 所围区域的面积为 $S$，则（　）.

;;;
A. $S=\oint_L y\mathrm{d}y-x\mathrm{d}x$
B. $S=\dfrac{1}{2}\oint_L x\mathrm{d}y-y\mathrm{d}x$
C. $S=\oint_L x\mathrm{d}y-y\mathrm{d}x$
D. $S=\dfrac{1}{2}\oint_L y\mathrm{d}y-x\mathrm{d}x$
;;;B
***
**B.**

由格林公式，知 $\iint_D\left(\dfrac{\partial Q}{\partial x}-\dfrac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=\oint_L P\mathrm{d}x+Q\mathrm{d}y$.

取 $P=-y,Q=x$，则 $2\iint_D\mathrm{d}x\mathrm{d}y=\oint_L x\mathrm{d}y-y\mathrm{d}x$，即面积为
$$S=\iint_D\mathrm{d}x\mathrm{d}y=\frac{1}{2}\oint_L x\mathrm{d}y-y\mathrm{d}x.$$

【注】简单闭曲线表示无重点的闭曲线：一个圆周是简单闭曲线，而"8"字形（自身相交一次）的闭曲线不是简单闭曲线（原书配图略）.

+++

#### 综合填空 (1) 设 $L:x^2+y^2=R^2$，取顺时针方向，则 $I=\oint_L\dfrac{\mathrm{e}^{x^2}-x^2y}{x^2+y^2}\mathrm{d}x+\dfrac{xy^2-\mathrm{e}^{y^2}}{x^2+y^2}\mathrm{d}y=$ ________.
***
$-\dfrac{\pi R^2}{2}$.

沿闭曲线 $L$ 的积分，考虑利用格林公式. 先将 $L:x^2+y^2=R^2$ 代入被积函数，去掉被积函数中无定义的点 $(0,0)$，则
$$I=\frac{1}{R^2}\oint_L(\mathrm{e}^{x^2}-x^2y)\mathrm{d}x+(xy^2-\mathrm{e}^{y^2})\mathrm{d}y$$
$$\xlongequal{\text{格林公式}}-\frac{1}{R^2}\iint_D(x^2+y^2)\mathrm{d}x\mathrm{d}y=-\frac{1}{R^2}\int_0^{2\pi}\mathrm{d}\theta\int_0^R r^2\cdot r\mathrm{d}r=-\frac{\pi R^2}{2}.$$

【注】$L$ 为顺时针方向，用格林公式需加一个负号.

+++

#### 综合填空 (2) 设积分 $I=\int_L F(x,y)(y\mathrm{d}x+x\mathrm{d}y)$ 与路径无关，且 $F(x,y)=0$ 确定的隐函数的图形过点 $(1,2)$ 且与坐标轴无交点，其中 $F(x,y)$ 可微，则 $F(x,y)=0$ 确定的隐函数为 ________.
***
$xy=2$.

依题设，记 $P(x,y)=F(x,y)y$，$Q(x,y)=F(x,y)x$，则 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，即
$$F(x,y)+xF'_x(x,y)=F(x,y)+yF'_y(x,y),$$
整理得
$$-\frac{F'_x(x,y)}{F'_y(x,y)}=-\frac{y}{x}=\frac{\mathrm{d}y}{\mathrm{d}x},$$
故 $\displaystyle\int\frac{\mathrm{d}y}{y}=-\int\frac{\mathrm{d}x}{x}$，得 $\ln|y|=-\ln|x|+\ln\mathrm{e}^{C_1}$，所以 $xy=C\ (C=\pm\mathrm{e}^{C_1})$，又过 $(1,2)$ 点，得 $C=2$.

综上可知，所求函数为 $xy=2$.

【注】设 $F(x,y)=0$ 确定的隐函数为 $y=y(x)$，则 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=-\dfrac{F'_x(x,y)}{F'_y(x,y)}$.

+++

#### 综合填空 (3) 设曲面 $S:x^2+y^2+z^2=2x$，其密度为 $\rho=x^2+y^2+z^2$，则曲面 $S$ 的质量 $m=$ ________.
***
$8\pi$.

$$m=\iint_S(x^2+y^2+z^2)\mathrm{d}S=\iint_S 2x\mathrm{d}S$$
$$=\iint_S 2(x-1)\mathrm{d}S+\iint_S 2\mathrm{d}S=0+2\times4\pi\times1^2=8\pi\quad(\text{利用球面面积}).$$

【注】① $S:x^2+y^2+z^2=2x$，即 $(x-1)^2+y^2+z^2=1$ 关于平面 $x=1$ 对称，$2(x-1)$ 关于 $(x-1)$ 是奇函数，故 $\iint_S 2(x-1)\mathrm{d}S=0$.

② 计算 $\iint_S x\mathrm{d}S$（被积函数为一次函数）应注意利用奇偶性（包括"平移"，如上例），有时还可利用质心（形心）坐标：
$$\bar{x}=\frac{\iint_S x\rho\mathrm{d}S}{\iint_S\rho\mathrm{d}S}=\frac{\iint_S x\mathrm{d}S}{\iint_S\mathrm{d}S},$$
则 $\iint_S x\mathrm{d}S=\bar{x}\cdot\iint_S\mathrm{d}S$. 对二重积分、三重积分、第一型曲线积分、第一型曲面积分都有类似解决方法.

+++

#### 综合填空 (4) 设光滑有向曲面 $S$ 的边界曲线为光滑有向闭曲线 $L$，方向符合右手法则，则 $I=\oint_L\mathbf{grad}\,\sin(x+y+z)\cdot\mathrm{d}\boldsymbol{s}=$ ________.
***
$0$.

$\mathbf{grad}\,\sin(x+y+z)=(\cos(x+y+z),\cos(x+y+z),\cos(x+y+z))$.

由斯托克斯公式，有
$$I=\oint_L\cos(x+y+z)\mathrm{d}x+\cos(x+y+z)\mathrm{d}y+\cos(x+y+z)\mathrm{d}z$$
$$=\iint_S\begin{vmatrix}\mathrm{d}y\mathrm{d}z&\mathrm{d}z\mathrm{d}x&\mathrm{d}x\mathrm{d}y\\[2pt]\dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\[4pt]\cos(x+y+z)&\cos(x+y+z)&\cos(x+y+z)\end{vmatrix}=0.$$

+++

#### 综合填空 (5) 向量场 $\boldsymbol{A}(x,y,z)=(x+y+z)\boldsymbol{i}+xy\boldsymbol{j}+z\boldsymbol{k}$ 在点 $P(1,1,1)$ 处的旋度 $\mathbf{rot}\,\boldsymbol{A}=$ ________，$\mathrm{div}\,\boldsymbol{A}=$ ________.
***
$\boldsymbol{j}$，$3$.

$$\mathbf{rot}\,\boldsymbol{A}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\[2pt]\dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\[4pt]P&Q&R\end{vmatrix}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\[2pt]\dfrac{\partial}{\partial x}&\dfrac{\partial}{\partial y}&\dfrac{\partial}{\partial z}\\[4pt]x+y+z&xy&z\end{vmatrix}=\boldsymbol{j}+(y-1)\boldsymbol{k},$$
在点 $P(1,1,1)$ 处，有 $\mathbf{rot}\,\boldsymbol{A}=\boldsymbol{j}$.

$$\mathrm{div}\,\boldsymbol{A}=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}=1+x+1=2+x,$$
故在点 $P(1,1,1)$ 处，$\mathrm{div}\,\boldsymbol{A}=2+1=3$.

+++

#### 综合填空 (6) 设 $\boldsymbol{\gamma}=x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k}$，$\boldsymbol{n}$ 为球面 $S:x^2+y^2+z^2=1$ 的外单位法向量，则 $\iint_S\boldsymbol{\gamma}\cdot\boldsymbol{n}\mathrm{d}S=$ ________.
***
$4\pi$.

令 $F(x,y,z)=x^2+y^2+z^2-1$，则外法向量为 $(F'_x,F'_y,F'_z)=(2x,2y,2z)$，故外单位法向量为
$$\boldsymbol{n}=\left(\frac{2x}{\sqrt{(2x)^2+(2y)^2+(2z)^2}},\frac{2y}{\sqrt{(2x)^2+(2y)^2+(2z)^2}},\frac{2z}{\sqrt{(2x)^2+(2y)^2+(2z)^2}}\right)=(x,y,z)=x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k},$$
从而
$$\iint_S\boldsymbol{\gamma}\cdot\boldsymbol{n}\mathrm{d}S=\iint_S(x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k})\cdot(x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k})\mathrm{d}S=\iint_S(x^2+y^2+z^2)\mathrm{d}S=\iint_S 1\mathrm{d}S=4\pi\times1^2=4\pi,$$
这里 $x^2+y^2+z^2=1$，$\iint_S\mathrm{d}S$ 表示球面 $S$ 的表面积.

+++

#### 综合解答 (1) 设 $f(x)$ 有二阶连续导数，$f(0)=0$，$f'(0)=1$，曲线积分 $I=\int_L\left[x\mathrm{e}^{2x}-6f(x)\right]\sin y\mathrm{d}x-\left[5f(x)-f'(x)\right]\cos y\mathrm{d}y$ 与路径无关，求 $f(x)$ 表达式.
***
记 $P=\left[x\mathrm{e}^{2x}-6f(x)\right]\sin y$，$Q=-\left[5f(x)-f'(x)\right]\cdot\cos y$，依题意，有 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，且 $\cos y\not\equiv0$，故
$$f''(x)-5f'(x)+6f(x)=x\mathrm{e}^{2x}.\qquad ①$$

① 式对应齐次微分方程的特征方程为 $r^2-5r+6=0$，解得 $r_1=2,r_2=3$. 令非齐次微分方程的特解为
$$f^*=x(a_0x+a_1)\mathrm{e}^{2x},$$
代入 ① 式可解得 $a_0=-\dfrac{1}{2},a_1=-1$，故方程 ① 的通解为
$$f(x)=C_1\mathrm{e}^{2x}+C_2\mathrm{e}^{3x}-\frac{1}{2}x(x+2)\mathrm{e}^{2x}.$$

又由 $f(0)=0,f'(0)=1$，得 $C_1=-2,C_2=2$，故
$$f(x)=-2\mathrm{e}^{2x}+2\mathrm{e}^{3x}-\frac{x}{2}(x+2)\mathrm{e}^{2x}.$$

+++

#### 综合解答 (2) 设 $D:x^2+y^2\leqslant1,x\geqslant0,y\geqslant0$，$L$ 为 $D$ 的正向边界，证明：$\oint_L x\mathrm{e}^{y^2}\mathrm{d}y-y\mathrm{e}^{-x^2}\mathrm{d}x\geqslant\dfrac{\pi}{2}$.
***
由格林公式，有
$$\oint_L x\mathrm{e}^{y^2}\mathrm{d}y-y\mathrm{e}^{-x^2}\mathrm{d}x=\iint_D(\mathrm{e}^{y^2}+\mathrm{e}^{-x^2})\mathrm{d}x\mathrm{d}y.$$

又 $D$（第一象限内的四分之一单位圆盘）关于直线 $y=x$ 对称，则
$$\iint_D(\mathrm{e}^{y^2}+\mathrm{e}^{-x^2})\mathrm{d}x\mathrm{d}y=\iint_D\mathrm{e}^{y^2}\mathrm{d}x\mathrm{d}y+\iint_D\mathrm{e}^{-x^2}\mathrm{d}x\mathrm{d}y=\iint_D\mathrm{e}^{x^2}\mathrm{d}x\mathrm{d}y+\iint_D\mathrm{e}^{-x^2}\mathrm{d}x\mathrm{d}y$$
$$=\iint_D(\mathrm{e}^{x^2}+\mathrm{e}^{-x^2})\mathrm{d}x\mathrm{d}y\geqslant\iint_D 2\sqrt{\mathrm{e}^{x^2}\cdot\mathrm{e}^{-x^2}}\mathrm{d}x\mathrm{d}y=2\iint_D\mathrm{d}x\mathrm{d}y=2\times\frac{1}{4}\pi\times1^2=\frac{\pi}{2}.$$

【注】这里分开利用轮换对称性.

+++

#### 综合解答 (3) 设 $f(x,y)$ 在 $\dfrac{x^2}{4}+y^2\leqslant1$ 上有二阶偏导数，$L$ 为 $\dfrac{x^2}{4}+y^2=1$，取顺时针方向，计算 $I=\oint_L\left[-3y+f'_x(x,y)\right]\mathrm{d}x+f'_y(x,y)\mathrm{d}y$.
***
设 $L$ 的参数方程为 $\begin{cases}x=2\cos t,\\ y=\sin t,\end{cases}$ 则
$$I=\oint_L-3y\mathrm{d}x+\oint_L f'_x(x,y)\mathrm{d}x+f'_y(x,y)\mathrm{d}y$$
$$=-\int_0^{2\pi}(-3\sin t)\mathrm{d}(2\cos t)+\oint_L\mathrm{d}\left[f(x,y)\right]$$
$$=-6\pi+0=-6\pi.$$

【注】$\oint_L\mathrm{d}\left[f(x,y)\right]=0$ 是利用了积分与路径无关的等价命题.

+++

#### 综合解答 (4) 设 $L$ 为 $y=\pi\cos x$ 从 $A(\pi,-\pi)$ 到 $B(-\pi,-\pi)$ 的曲线，计算 $I=\int_L\dfrac{(x+y)\mathrm{d}x-(x-y)\mathrm{d}y}{x^2+y^2}$.
***
**解法 1** 记 $P=\dfrac{x+y}{x^2+y^2}$，$Q=-\dfrac{x-y}{x^2+y^2}$，则
$$\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}=\frac{x^2-y^2-2xy}{(x^2+y^2)^2},$$
故在不含 $(0,0)$ 在内的单连通区域积分与路径无关.

选择折线 $ACDB$（$C(\pi,\pi)$，$D(-\pi,\pi)$），其中
$$\overline{AC}:\begin{cases}x=\pi,\\ y=y,\end{cases}\quad\overline{CD}:\begin{cases}y=\pi,\\ x=x,\end{cases}\quad\overline{DB}:\begin{cases}x=-\pi,\\ y=y,\end{cases}$$
故
$$I=\int_{\overline{AC}}+\int_{\overline{CD}}+\int_{\overline{DB}}=\int_{-\pi}^{\pi}\frac{-(\pi-y)\mathrm{d}y}{\pi^2+y^2}+\int_{\pi}^{-\pi}\frac{(\pi+x)\mathrm{d}x}{\pi^2+x^2}+\int_{\pi}^{-\pi}\frac{-(-\pi-y)}{\pi^2+y^2}\mathrm{d}y=-\frac{3}{2}\pi.$$

**解法 2** 利用格林公式求解. 作辅助线 $\overline{BA}:\begin{cases}y=-\pi,\\ x=x,\end{cases}$ 及 $L_1:\begin{cases}x=\delta\cos t,\\ y=\delta\sin t,\end{cases}$（$\delta$ 充分小，取顺时针方向），则
$$I=\oint_{L+\overline{BA}+L_1}-\int_{\overline{BA}}-\int_{L_1},$$
$$\oint_{L+\overline{BA}+L_1}\frac{(x+y)\mathrm{d}x-(x-y)\mathrm{d}y}{x^2+y^2}\xlongequal{\text{格林公式}}\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=0,$$
其中 $D$ 为 $L+\overline{BA}+L_1$ 构成的复连通区域. 又
$$\int_{\overline{BA}}\frac{(x+y)\mathrm{d}x-(x-y)\mathrm{d}y}{x^2+y^2}=\int_{-\pi}^{\pi}\frac{(x-\pi)\mathrm{d}x}{x^2+\pi^2}=\frac{1}{2}\int_{-\pi}^{\pi}\frac{\mathrm{d}(x^2+\pi^2)}{x^2+\pi^2}-\pi\int_{-\pi}^{\pi}\frac{\mathrm{d}x}{x^2+\pi^2}$$
$$=\frac{1}{2}\ln(x^2+\pi^2)\Big|_{-\pi}^{\pi}-\pi\cdot\frac{1}{\pi}\arctan\frac{x}{\pi}\Big|_{-\pi}^{\pi}=-\frac{\pi}{2},$$
$$\int_{L_1}\frac{(x+y)\mathrm{d}x-(x-y)\mathrm{d}y}{x^2+y^2}=\int_{2\pi}^{0}\frac{(\delta\cos t+\delta\sin t)(-\delta\sin t)-(\delta\cos t-\delta\sin t)\delta\cos t}{\delta^2\cos^2t+\delta^2\sin^2t}\mathrm{d}t=-\int_{2\pi}^{0}\mathrm{d}t=2\pi,$$
故 $I=0-\left(-\dfrac{\pi}{2}\right)-2\pi=-\dfrac{3\pi}{2}$.

【注】如下解法是错误的：由 $\dfrac{\partial Q}{\partial x}=\dfrac{\partial P}{\partial y}$，连接 $\overline{AB}:\begin{cases}y=-\pi,\\ x=x,\end{cases}$ 则
$$I=\int_L\frac{(x+y)\mathrm{d}x-(x-y)\mathrm{d}y}{x^2+y^2}=\int_{\pi}^{-\pi}\frac{(x-\pi)\mathrm{d}x}{x^2+\pi^2}=\frac{\pi}{2}.$$
因为 $\overline{AB}$ 与 $y=\pi\cos x$ 所围区域 $D$ 内含奇点 $(0,0)$，所以 $D$ 不是单连通区域，不能说明积分与路径无关.

+++

#### 综合解答 (5) 设 $f(x)$ 有连续导数，$L$ 为从点 $A(2,2\pi)$ 沿 $(x-1)^2+(y-\pi)^2=1+\pi^2$ 的上半圆周到点 $O(0,0)$ 的一段弧，计算 $I=\int_L f'(x)\sin y\mathrm{d}x+\left[f(x)\cos y-\pi x\right]\mathrm{d}y$.
***
利用格林公式求解.

记 $P=f'(x)\sin y$，$Q=f(x)\cos y-\pi x$，则 $\dfrac{\partial Q}{\partial x}-\dfrac{\partial P}{\partial y}=-\pi$.

添加线段 $\overline{OA}:\begin{cases}y=\pi x,\\ x=x,\end{cases}$ 则
$$I=\oint_{L+\overline{OA}}f'(x)\sin y\mathrm{d}x+\left[f(x)\cos y-\pi x\right]\mathrm{d}y-\int_{\overline{OA}}f'(x)\sin y\mathrm{d}x+\left[f(x)\cos y-\pi x\right]\mathrm{d}y.$$

而
$$\oint_{L+\overline{OA}}f'(x)\sin y\mathrm{d}x+\left[f(x)\cos y-\pi x\right]\mathrm{d}y=\iint_D(-\pi)\mathrm{d}x\mathrm{d}y=-\pi\iint_D\mathrm{d}x\mathrm{d}y=-\pi\cdot\frac{1}{2}\cdot\pi(1+\pi^2)=-\frac{\pi^2}{2}(1+\pi^2),$$
其中 $D$ 为弧 $\overset{\frown}{AO}$ 与 $\overline{OA}$ 所围半圆区域. 又
$$\int_{\overline{OA}}f'(x)\sin y\mathrm{d}x+\left[f(x)\cos y-\pi x\right]\mathrm{d}y=\int_{\overline{OA}}f'(x)\sin y\mathrm{d}x+f(x)\cos y\mathrm{d}y-\int_{\overline{OA}}\pi x\mathrm{d}y$$
$$=\int_{\overline{OA}}\mathrm{d}\left[f(x)\sin y\right]-\int_0^2\pi\cdot x\mathrm{d}(\pi x)=\int_0^2\mathrm{d}\left[f(x)\sin\pi x\right]-2\pi^2=f(x)\sin\pi x\Big|_0^2-2\pi^2=0-2\pi^2=-2\pi^2,$$
故
$$I=-\frac{\pi^2}{2}(1+\pi^2)+2\pi^2=\frac{\pi^2}{2}(3-\pi^2).$$

+++

#### 综合解答 (6) 设 $f(y)$ 有连续导数，$f(0)=0$，曲线 $\overset{\frown}{OA}$ 的极坐标方程为 $r=a(1-\cos\theta)$，$a>0$，$0\leqslant\theta\leqslant\pi$，$O(0,0)$ 与 $A$ 分别对应于 $\theta=0$ 与 $\theta=\pi$，计算 $I=\int_{\overset{\frown}{OA}}\left[f(y)\mathrm{e}^x-\pi y\right]\mathrm{d}x+\left[f'(y)\mathrm{e}^x-\pi\right]\mathrm{d}y$.
***
记 $P=f(y)\mathrm{e}^x-\pi y$，$Q=f'(y)\mathrm{e}^x-\pi$，则 $\dfrac{\partial Q}{\partial x}-\dfrac{\partial P}{\partial y}=\pi$.

设曲线 $\overset{\frown}{OA}$ 与线段 $\overline{AO}$ 所围区域为 $D$（$A$ 在 $x$ 轴负半轴上，$A(-2a,0)$），
$$\overline{AO}:\begin{cases}y=0,\\ x=x,\end{cases}\quad(-2a\leqslant x\leqslant0).$$

利用格林公式，得
$$\oint_{\overset{\frown}{OA}+\overline{AO}}P\mathrm{d}x+Q\mathrm{d}y=\iint_D\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)\mathrm{d}x\mathrm{d}y=\pi\iint_D\mathrm{d}x\mathrm{d}y$$
$$=\frac{\pi}{2}\int_0^{\pi}r^2\mathrm{d}\theta=\frac{a^2\pi}{2}\int_0^{\pi}(1-\cos\theta)^2\mathrm{d}\theta=\frac{a^2\pi}{2}\int_0^{\pi}\left(\frac{3}{2}-2\cos\theta+\frac{1}{2}\cos2\theta\right)\mathrm{d}\theta=\frac{3\pi^2a^2}{4}.$$

又
$$\int_{\overline{AO}}P\mathrm{d}x+Q\mathrm{d}y=\int_{-2a}^{0}P(x,0)\mathrm{d}x=\int_{-2a}^{0}f(0)\mathrm{e}^x\mathrm{d}x=0,$$
故 $I=\dfrac{3}{4}\pi^2a^2$.

+++

#### 综合解答 (7) 设 $f(x)$ 在 $(-\infty,+\infty)$ 内有连续导数，$L$ 为从点 $A\left(3,\dfrac{2}{3}\right)$ 到点 $B(1,2)$ 的直线段，计算 $I=\int_L\dfrac{1+y^2f(xy)}{y}\mathrm{d}x+\dfrac{x}{y^2}\left[y^2f(xy)-1\right]\mathrm{d}y$.
***
**解法 1** 记 $P=\dfrac{1+y^2f(xy)}{y}$，$Q=\dfrac{x}{y^2}\left[y^2f(xy)-1\right]$，则
$$\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}=f(xy)+xyf'(xy)-\frac{1}{y^2}\quad(y\neq0),$$
故当 $y\neq0$ 时，积分与路径无关.

取折线 $\overline{AC}+\overline{CB}$，$A\left(3,\dfrac{2}{3}\right)$，$C\left(1,\dfrac{2}{3}\right)$，$B(1,2)$，
$$\overline{AC}:\begin{cases}y=\dfrac{2}{3},\\ x=x,\end{cases}\quad\overline{CB}:\begin{cases}x=1,\\ y=y,\end{cases}$$
故
$$I=\int_L\frac{1+y^2f(xy)}{y}\mathrm{d}x+\frac{x}{y^2}\left[y^2f(xy)-1\right]\mathrm{d}y$$
$$=\int_3^1\frac{3}{2}\left[1+\frac{4}{9}f\left(\frac{2}{3}x\right)\right]\mathrm{d}x+\int_{\frac{2}{3}}^{2}\left[f(y)-\frac{1}{y^2}\right]\mathrm{d}y$$
$$=\frac{3}{2}\int_3^1\mathrm{d}x+\frac{2}{3}\int_3^1 f\left(\frac{2x}{3}\right)\mathrm{d}x+\int_{\frac{2}{3}}^{2}f(y)\mathrm{d}y-\int_{\frac{2}{3}}^{2}\frac{1}{y^2}\mathrm{d}y$$
$$=\frac{3}{2}(1-3)+\int_2^{\frac{2}{3}}f(t)\mathrm{d}t+\int_{\frac{2}{3}}^{2}f(y)\mathrm{d}y+\frac{1}{2}-\frac{3}{2}=-4,$$
这里 $\dfrac{2}{3}\displaystyle\int_3^1 f\left(\frac{2x}{3}\right)\mathrm{d}x\xlongequal{\frac{2x}{3}=t}\int_2^{\frac{2}{3}}f(t)\mathrm{d}t$.

**解法 2** 取积分路径为 $xy=2$，则
$$I=\int_{\frac{2}{3}}^{2}\left[\frac{1+y^2f(2)}{y}\left(-\frac{2}{y^2}\right)+\frac{2}{y^3}\left[y^2f(2)-1\right]\right]\mathrm{d}y=\int_{\frac{2}{3}}^{2}\frac{-4}{y^3}\mathrm{d}y=-4.$$

【注】第二类曲线积分（平面），当积分与路径无关时，可选简单路径积分，如折线、圆周等.

+++

#### 综合解答 (8) 设 $f(x),g(x)$ 在 $(0,+\infty)$ 内有连续导数，且 $V(x,y)=yf(xy)\mathrm{d}x+xg(xy)\mathrm{d}y$.

（Ⅰ）若存在函数 $u(x,y)$，使得 $\mathrm{d}u=V$，求 $f(xy)-g(xy)$；\
（Ⅱ）若 $f(x)=\varphi'(x)$，求函数 $u(x,y)$，使 $\mathrm{d}u=V$.
***
（Ⅰ）由 $\mathrm{d}u=V$，$f(x),g(x)$ 有连续导数，得
$$\frac{\partial}{\partial y}\left[yf(xy)\right]=\frac{\partial}{\partial x}\left[xg(xy)\right],$$
即
$$f(xy)+yf'(xy)\cdot x=g(xy)+xg'(xy)\cdot y.$$

令 $xy=t>0$，得 $f(t)+t\dfrac{\mathrm{d}\left[f(t)\right]}{\mathrm{d}t}=g(t)+t\dfrac{\mathrm{d}\left[g(t)\right]}{\mathrm{d}t}$，即
$$t\frac{\mathrm{d}\left[f(t)-g(t)\right]}{\mathrm{d}t}=-\left[f(t)-g(t)\right],$$
当 $f(t)\neq g(t)$ 时，变形为 $\dfrac{\mathrm{d}\left[f(t)-g(t)\right]}{f(t)-g(t)}=-\dfrac{\mathrm{d}t}{t}$，积分得 $f(t)-g(t)=\dfrac{C_0}{t}\ (C_0\neq0)$.

当 $f(t)\equiv g(t)$ 时，即 $f(t)-g(t)=\dfrac{0}{t}$ 也成立，故
$$f(xy)-g(xy)=\frac{C}{xy}\quad(C\ \text{为任意常数}).$$

（Ⅱ）当 $f(x)=\varphi'(x)$，由（Ⅰ）有
$$\mathrm{d}u=y\varphi'(xy)\mathrm{d}x+x\left[\varphi'(xy)-\frac{C}{xy}\right]\mathrm{d}y$$
$$=y\varphi'(xy)\mathrm{d}x+x\varphi'(xy)\mathrm{d}y-\frac{C}{y}\mathrm{d}y$$
$$=\mathrm{d}\left[\varphi(xy)\right]-C\mathrm{d}(\ln|y|)=\mathrm{d}\left[\varphi(xy)-C\ln|y|\right],$$
故
$$u(x,y)=\varphi(xy)-C\ln|y|+C_0\quad(C_0,C\ \text{为任意常数}).$$

+++

#### 综合解答 (9) 设曲线 $L$ 为微分方程 $y'=f(x,y)\ (f(x,y)\neq0)$ 确定的一条简单闭曲线，且 $L$ 所围平面区域 $D$ 的面积为 $A$，计算 $I=\oint_L xf(x,y)\mathrm{d}x-\dfrac{y}{f(x,y)}\mathrm{d}y$（$L$ 为 $D$ 的正向边界）.
***
将 $L$ 满足的微分方程 $y'=f(x,y)$ 代入被积表达式，得
$$I=\oint_L xf(x,y)\mathrm{d}x-\frac{y}{f(x,y)}\mathrm{d}y$$
$$=\oint_L x\cdot y'\mathrm{d}x-\frac{y}{f(x,y)}\cdot f(x,y)\mathrm{d}x$$
$$=\oint_L x\mathrm{d}y-y\mathrm{d}x.$$

由格林公式，得
$$\oint_L x\mathrm{d}y-y\mathrm{d}x=\iint_D\left[1-(-1)\right]\mathrm{d}x\mathrm{d}y=2\iint_D\mathrm{d}x\mathrm{d}y=2A.$$

【注】将曲线 $L$ 的方程代入曲线积分 $\int_L P\mathrm{d}x+Q\mathrm{d}y$ 化简积分，是值得重视的技巧.

+++

#### 综合解答 (10) 设在 $D=\{(x,y)\mid y>0\}$ 内，$f(x,y)$ 有一阶连续偏导数，$f(x,y)\neq0$，且对任意 $t>0$，有 $f(tx,ty)=t^2f(x,y)$，证明：对 $D$ 内的任意分段光滑的有向简单闭曲线 $L$，都有 $\oint_L\dfrac{y}{f(x,y)}\mathrm{d}x-\dfrac{x}{f(x,y)}\mathrm{d}y=0$.
***
令 $P=\dfrac{y}{f(x,y)}$，$Q=-\dfrac{x}{f(x,y)}$，依题意，有
$$\oint_L\frac{y}{f(x,y)}\mathrm{d}x-\frac{x}{f(x,y)}\mathrm{d}y=0\Longleftrightarrow\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y},$$
即
$$\frac{\partial}{\partial x}\left[-\frac{x}{f(x,y)}\right]=\frac{\partial}{\partial y}\left[\frac{y}{f(x,y)}\right],$$
则
$$\frac{xf'_x(x,y)+yf'_y(x,y)-2f(x,y)}{\left[f(x,y)\right]^2}=0,$$
从而
$$xf'_x(x,y)+yf'_y(x,y)-2f(x,y)=0,\qquad ①$$
故原问题转化为证 ① 式成立.

在已知等式 $f(tx,ty)=t^2f(x,y)$ 两边同时对 $t$ 求导，得
$$xf'_1(tx,ty)+yf'_2(tx,ty)=2tf(x,y),$$
令 $t=1$，得
$$xf'_1(x,y)+yf'_2(x,y)=2f(x,y),$$
即 $xf'_x(x,y)+yf'_y(x,y)-2f(x,y)=0$. 故所证结论成立.

【注】满足 $f(tx,ty)=t^kf(x,y)$ 的函数 $f(x,y)$，称为 $k$ 次齐次函数. 本题若条件为 $f(tx,ty)=t^{-2}f(x,y)$，则有 $\oint_L yf(x,y)\mathrm{d}x-xf(x,y)\mathrm{d}y=0$（本题为数学一真题）.

+++

#### 综合解答 (11) 设曲面 $S$ 为由圆柱面 $x^2+y^2=R^2$、平面 $z=0$ 和 $z-x=R\ (R>0)$ 所围立体的表面，计算 $I=\oiint_S z\mathrm{d}S$.
***
依题设，曲面 $S$ 可分成三个曲面
$$S_1:z-x=R,\quad S_2:z=0,\quad S_3:x^2+y^2=R^2,$$
则
$$I=\oiint_S z\mathrm{d}S=\iint_{S_1}z\mathrm{d}S+\iint_{S_2}z\mathrm{d}S+\iint_{S_3}z\mathrm{d}S.$$

$$\iint_{S_1}z\mathrm{d}S=\iint_{D_{xy}}(R+x)\sqrt{1+z'^2_x+z'^2_y}\mathrm{d}x\mathrm{d}y=\sqrt{2}\iint_{D_{xy}}(R+x)\mathrm{d}x\mathrm{d}y$$
$$=\sqrt{2}\int_0^{2\pi}\mathrm{d}\theta\int_0^R(R+r\cos\theta)r\mathrm{d}r=\sqrt{2}\int_0^{2\pi}\left(\frac{1}{2}R^3+\frac{1}{3}R^3\cos\theta\right)\mathrm{d}\theta=\sqrt{2}\pi R^3\quad(D_{xy}:x^2+y^2\leqslant R^2).$$

对 $S_3$ 分两块，其方程分别为 $y=\sqrt{R^2-x^2}$，$y=-\sqrt{R^2-x^2}$，将其投影到 $xOz$ 面上，$D_{xz}$ 为三角形的区域，又 $\mathrm{d}S=\sqrt{1+y'^2_x+y'^2_z}\mathrm{d}x\mathrm{d}z=\dfrac{R}{\sqrt{R^2-x^2}}\mathrm{d}x\mathrm{d}z$，由对称性，知
$$\iint_{S_3}z\mathrm{d}S=2\iint_{D_{xz}}z\cdot\frac{R}{\sqrt{R^2-x^2}}\mathrm{d}x\mathrm{d}z=2\int_{-R}^{R}\frac{R}{\sqrt{R^2-x^2}}\mathrm{d}x\int_0^{R+x}z\mathrm{d}z$$
$$=\int_{-R}^{R}\frac{R}{\sqrt{R^2-x^2}}(R+x)^2\mathrm{d}x\xlongequal{x=R\sin t}R^3\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}(1+\sin t)^2\mathrm{d}t=\frac{3\pi R^3}{2}.$$

显然在平面 $S_2:z=0$ 上，$\iint_{S_2}z\mathrm{d}S=0$，故
$$I=\sqrt{2}\pi R^3+0+\frac{3\pi R^3}{2}=\pi R^3\left(\sqrt{2}+\frac{3}{2}\right).$$

+++

#### 综合解答 (12) 设球面为 $x^2+y^2+z^2=R^2$，柱面为 $x^2+y^2=Rx\ (R>0)$，球面在柱体内的面积为 $S_1$，柱面在球体内的面积为 $S_2$，求 $\dfrac{S_1}{S_2}$.
***
由对称性，知求 $S_1$ 只需考虑 $z\geqslant0$ 的部分.

由 $z=\sqrt{R^2-x^2-y^2}$，知
$$\mathrm{d}S=\sqrt{1+z'^2_x+z'^2_y}\mathrm{d}x\mathrm{d}y=\sqrt{1+\left(\frac{-x}{\sqrt{R^2-x^2-y^2}}\right)^2+\left(\frac{-y}{\sqrt{R^2-x^2-y^2}}\right)^2}\mathrm{d}x\mathrm{d}y=\frac{R}{\sqrt{R^2-x^2-y^2}}\mathrm{d}x\mathrm{d}y,$$
故
$$S_1=2\iint_{S_1^+}\mathrm{d}S=2\iint_{D_{xy}}\sqrt{1+z'^2_x+z'^2_y}\mathrm{d}x\mathrm{d}y=2\iint_{D_{xy}}\frac{R}{\sqrt{R^2-x^2-y^2}}\mathrm{d}x\mathrm{d}y$$
$$=2R\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{R\cos\theta}\frac{1}{\sqrt{R^2-r^2}}r\mathrm{d}r=2R^2(\pi-2),$$
其中 $S_1^+$ 为球面在柱体内且 $z\geqslant0$ 的曲面.

求 $S_2$ 只需考虑 $y\geqslant0,z\geqslant0$ 的部分，由 $x^2+y^2=Rx$，知 $y=\sqrt{Rx-x^2}$. 又
$$\mathrm{d}S=\sqrt{1+y'^2_x+y'^2_z}\mathrm{d}x\mathrm{d}z=\sqrt{1+\left(\frac{R-2x}{2\sqrt{Rx-x^2}}\right)^2+0^2}\mathrm{d}x\mathrm{d}z=\frac{R}{2\sqrt{Rx-x^2}}\mathrm{d}x\mathrm{d}z,$$
故
$$S_2=4\iint_{S_2^+}\mathrm{d}S=4\iint_{D_{xz}}\frac{R}{2\sqrt{Rx-x^2}}\mathrm{d}x\mathrm{d}z=2\int_0^R\mathrm{d}z\int_0^{\frac{R^2-z^2}{R}}\frac{R}{\sqrt{Rx-x^2}}\mathrm{d}x$$
$$=2R\int_0^R\mathrm{d}z\int_0^{\frac{R^2-z^2}{R}}\frac{\mathrm{d}\left(\frac{2}{R}x-1\right)}{\sqrt{1-\left(\frac{2}{R}x-1\right)^2}}=2R\int_0^R\left[\frac{\pi}{2}+\arcsin\left(1-\frac{2z^2}{R^2}\right)\right]\mathrm{d}z$$
$$=-2R\int_0^R z\cdot\frac{1}{\sqrt{1-\left(1-\frac{2z^2}{R^2}\right)^2}}\cdot\left(\frac{-4z}{R^2}\right)\mathrm{d}z=4R\int_0^R\frac{z}{\sqrt{R^2-z^2}}\mathrm{d}z=4R^2,$$
其中 $S_2^+$ 为柱面在球体内且 $y\geqslant0,z\geqslant0$ 的曲面. 所以
$$\frac{S_1}{S_2}=\frac{2R^2(\pi-2)}{4R^2}=\frac{1}{2}(\pi-2).$$

【注】由交线 $\begin{cases}x^2+y^2+z^2=R^2,\\ x^2+y^2=Rx,\end{cases}$ 得 $Rx+z^2=R^2$，即 $x=\dfrac{R^2-z^2}{R}$.

+++

#### 综合解答 (13) 设薄片型物体 $S$ 为圆锥面 $z=\sqrt{x^2+y^2}$ 被柱面 $z^2=2x$ 割下的有限部分，其上任一点的密度为 $\mu(x,y,z)=9\sqrt{x^2+y^2+z^2}$，记圆锥面与柱面的交线为 $C$.

（Ⅰ）求 $C$ 在 $xOy$ 面上的投影曲线方程；\
（Ⅱ）求 $S$ 的质量.
***
（Ⅰ）由已知，$C$ 的方程为 $\begin{cases}z=\sqrt{x^2+y^2},\\ z^2=2x,\end{cases}$ 消去 $z$，得 $x^2+y^2=2x$，故 $C$ 在 $xOy$ 面上的投影曲线方程为
$$\begin{cases}x^2+y^2=2x,\\ z=0.\end{cases}$$

（Ⅱ）$S$ 的质量为
$$m=\iint_S\mu(x,y,z)\mathrm{d}S=\iint_S 9\sqrt{x^2+y^2+z^2}\mathrm{d}S$$
$$=\iint_D 9\sqrt{2}\sqrt{x^2+y^2}\cdot\sqrt{2}\mathrm{d}x\mathrm{d}y\quad(D:x^2+y^2\leqslant2x)$$
$$=18\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\mathrm{d}\theta\int_0^{2\cos\theta}r\cdot r\mathrm{d}r=64.$$

+++

#### 综合解答 (14) 在半径为 $a$ 的球表面上取一点，以该点为球心作半径为 $R$ 的球，问 $R$ 为何值时，该球位于定球内的表面积最大？
***
设 $S_0:x^2+y^2+z^2=a^2$，在 $S_0$ 上取点 $P(0,0,a)$，则球面方程 $S_1$ 为 $x^2+y^2+(z-a)^2=R^2$.

由 $\begin{cases}x^2+y^2+z^2=a^2,\\ x^2+y^2+(z-a)^2=R^2,\end{cases}$ 可得 $z=a-\dfrac{R^2}{2a}$，故所求内部曲面在 $xOy$ 上的投影区域为 $D:x^2+y^2\leqslant R^2-\dfrac{R^4}{4a^2}$.

内部曲面记为 $S$，则 $S:z=a-\sqrt{R^2-x^2-y^2}$，故
$$\mathrm{d}S=\sqrt{1+z'^2_x+z'^2_y}\mathrm{d}x\mathrm{d}y=\frac{R}{\sqrt{R^2-x^2-y^2}}\mathrm{d}x\mathrm{d}y.$$

所求表面积为
$$A=\iint_D\frac{R}{\sqrt{R^2-x^2-y^2}}\mathrm{d}x\mathrm{d}y=R\int_0^{2\pi}\mathrm{d}\theta\int_0^{\sqrt{R^2-\frac{R^4}{4a^2}}}\frac{r}{\sqrt{R^2-r^2}}\mathrm{d}r=2\pi\left(R^2-\frac{R^3}{2a}\right).$$

令 $\dfrac{\mathrm{d}A}{\mathrm{d}R}=2\pi\left(2R-\dfrac{3R^2}{2a}\right)=0$，得 $R=\dfrac{4a}{3}$，此时表面积最大.

+++

#### 综合解答 (15) 设 $f(u)$ 有连续导数，$S$ 为 $z=\sqrt{x^2+y^2}$ 与两个半球面 $z=\sqrt{1-x^2-y^2}$，$z=\sqrt{4-x^2-y^2}$ 所围立体的全表面的外侧，计算 $I=\oiint_S\left[\dfrac{1}{y+3}f\left(\dfrac{x+4}{y+3}\right)+3xy^2\right]\mathrm{d}y\mathrm{d}z+\left[\dfrac{1}{x+4}f\left(\dfrac{x+4}{y+3}\right)+3x^2y\right]\mathrm{d}z\mathrm{d}x+z^3\mathrm{d}x\mathrm{d}y$.
***
令
$$P=\frac{1}{y+3}f\left(\frac{x+4}{y+3}\right)+3xy^2,\quad Q=\frac{1}{x+4}f\left(\frac{x+4}{y+3}\right)+3x^2y,\quad R=z^3.$$

所求积分满足高斯公式的条件. 利用高斯公式，有
$$I=\iiint_V\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right)\mathrm{d}V=3\iiint_V(x^2+y^2+z^2)\mathrm{d}V$$
$$\xlongequal{\text{球坐标}}3\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{4}}\sin\varphi\mathrm{d}\varphi\int_1^2 r^4\mathrm{d}r=\frac{93}{5}(2-\sqrt{2})\pi.$$

+++

#### 综合解答 (16) 设曲面 $S:x^2+y^2+z^2=R^2$，$z\geqslant0$，$\boldsymbol{n}=(\cos\alpha,\cos\beta,\cos\gamma)$ 是 $S$ 向外的单位法向量，计算 $I=\iint_S\left[(z^n-y^n)\cos\alpha+(x^n-z^n)\cos\beta+(y^n-x^n)\cos\gamma\right]\mathrm{d}S\ (n\geqslant1)$.
***
由两类曲面积分的关系，有
$$I=\iint_S(z^n-y^n)\mathrm{d}y\mathrm{d}z+(x^n-z^n)\mathrm{d}z\mathrm{d}x+(y^n-x^n)\mathrm{d}x\mathrm{d}y.$$

记 $P=z^n-y^n$，$Q=x^n-z^n$，$T=y^n-x^n$，添加辅助面 $S_1:z=0,x^2+y^2\leqslant R^2$，取下侧，由高斯公式，得
$$I=\oiint_{S+S_1}-\iint_{S_1}.$$

而
$$\oiint_{S+S_1}P\mathrm{d}y\mathrm{d}z+Q\mathrm{d}z\mathrm{d}x+T\mathrm{d}x\mathrm{d}y=\iiint_V\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial T}{\partial z}\right)\mathrm{d}V=\iiint_V 0\mathrm{d}V=0.$$

又
$$\iint_{S_1}(z^n-y^n)\mathrm{d}y\mathrm{d}z+(x^n-z^n)\mathrm{d}z\mathrm{d}x+(y^n-x^n)\mathrm{d}x\mathrm{d}y=0+0-\iint_{D_{xy}}(y^n-x^n)\mathrm{d}x\mathrm{d}y$$
$$=-\int_0^{2\pi}\mathrm{d}\theta\int_0^R(r^n\sin^n\theta-r^n\cos^n\theta)r\mathrm{d}r=-\int_0^{2\pi}(\sin^n\theta-\cos^n\theta)\mathrm{d}\theta\int_0^R r^{n+1}\mathrm{d}r$$
$$=\frac{-R^{n+2}}{n+2}\int_0^{2\pi}(\sin^n\theta-\cos^n\theta)\mathrm{d}\theta=\frac{-R^{n+2}}{n+2}\cdot4\int_0^{\frac{\pi}{2}}(\sin^n\theta-\cos^n\theta)\mathrm{d}\theta=0,$$
（因 $\displaystyle\int_0^{\frac{\pi}{2}}\sin^n\theta\mathrm{d}\theta=\int_0^{\frac{\pi}{2}}\cos^n\theta\mathrm{d}\theta$）. 故 $I=0-0=0$.

【注】① 此题也可利用对称性计算：令 $F=x^2+y^2+z^2-R^2$，则 $(F'_x,F'_y,F'_z)=(2x,2y,2z)$，
$$\cos\alpha=\frac{2x}{\sqrt{(2x)^2+(2y)^2+(2z)^2}}=\frac{x}{\sqrt{x^2+y^2+z^2}}=\frac{x}{R},$$
同理 $\cos\beta=\dfrac{y}{R}$，$\cos\gamma=\dfrac{z}{R}$，故 $\boldsymbol{n}=(\cos\alpha,\cos\beta,\cos\gamma)=\dfrac{1}{R}(x,y,z)$，故
$$I=\iint_S\left[(z^n-y^n)\frac{x}{R}+(x^n-z^n)\frac{y}{R}+(y^n-x^n)\frac{z}{R}\right]\mathrm{d}S.$$
由 $S$ 关于 $xOy$ 面、$yOz$ 面对称，且 $(z^n-y^n)\dfrac{x}{R}$，$(x^n-z^n)\dfrac{y}{R}$ 分别关于 $x,y$ 是奇函数，故
$$\iint_S\left[(z^n-y^n)\frac{x}{R}+(x^n-z^n)\frac{y}{R}\right]\mathrm{d}S=0.$$
又 $S$ 关于平面 $x=y$ 对称，由轮换对称性，知 $\iint_S y^nz\mathrm{d}S=\iint_S x^nz\mathrm{d}S$，即 $\iint_S(y^n-x^n)\dfrac{z}{R}\mathrm{d}S=0$. 综上所述，$I=0$.

② $\iint_S f(x,y,z)\mathrm{d}S$ 与三重积分 $\iiint_V f(x,y,z)\mathrm{d}V$ 一样，利用轮换对称性时，可以三个变量轮换，也可以两个变量轮换.

+++

#### 综合解答 (17) 设曲面 $S:z=\sqrt{R^2-x^2-y^2}\ (R>0)$，取下侧，计算 $I=\iint_S\dfrac{Rx\mathrm{d}y\mathrm{d}z+(R+z)^2\mathrm{d}x\mathrm{d}y}{\sqrt{x^2+y^2+z^2}}$.
***
由于被积表达式在点 $(0,0,0)$ 处没有意义，先将曲面 $S:z=\sqrt{R^2-x^2-y^2}$ 代入化简，得
$$I=\frac{1}{R}\iint_S Rx\mathrm{d}y\mathrm{d}z+(R+z)^2\mathrm{d}x\mathrm{d}y.$$

为了利用高斯公式，添加辅助面 $S_1:\begin{cases}z=0,\\ x^2+y^2\leqslant R^2,\end{cases}$ 取上侧，故
$$\frac{1}{R}\oiint_{S+S_1}Rx\mathrm{d}y\mathrm{d}z+(R+z)^2\mathrm{d}x\mathrm{d}y=-\frac{1}{R}\iiint_V(R+2R+2z)\mathrm{d}V=-\frac{1}{R}\iiint_V(3R+2z)\mathrm{d}V$$
$$=-\frac{1}{R}\cdot3R\cdot\frac{4}{3}\pi R^3\cdot\frac{1}{2}-\frac{2}{R}\iiint_V z\mathrm{d}V$$
$$\xlongequal{\text{球坐标}}-2\pi R^3-\frac{2}{R}\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{2}}\mathrm{d}\varphi\int_0^R r\cos\varphi\cdot r^2\sin\varphi\mathrm{d}r$$
$$=-2\pi R^3-\frac{1}{2}\pi R^3=-\frac{5}{2}\pi R^3.$$

又由于
$$\frac{1}{R}\iint_{S_1}Rx\mathrm{d}y\mathrm{d}z+(R+z)^2\mathrm{d}x\mathrm{d}y=0+\frac{1}{R}\iint_{x^2+y^2\leqslant R^2}R^2\mathrm{d}x\mathrm{d}y=\frac{1}{R}R^2\cdot\pi R^2=\pi R^3,$$
故
$$I=\oiint_{S+S_1}-\iint_{S_1}=-\frac{5}{2}\pi R^3-\pi R^3=-\frac{7}{2}\pi R^3.$$

+++

#### 综合解答 (18) 设 $S$ 为椭球面 $x^2+2y^2+3z^2=1$ 外侧，计算 $I=\oiint_S\dfrac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}$.
***
被积函数较烦琐，又不能代入 $S$ 的方程化简，考虑到 $(x^2+y^2+z^2)^{\frac{3}{2}}$ 在原点 $(0,0,0)$ 处为零，挖去原点，作球面 $S_1:x^2+y^2+z^2=r^2$（$r$ 充分小），取内侧，$V_r$ 表示 $S$ 与 $S_1$ 所围空间区域，应用高斯公式，记
$$P=\frac{x}{(x^2+y^2+z^2)^{\frac{3}{2}}},\quad Q=\frac{y}{(x^2+y^2+z^2)^{\frac{3}{2}}},\quad R=\frac{z}{(x^2+y^2+z^2)^{\frac{3}{2}}},$$
计算可得在 $V_r$ 中，有 $\dfrac{\partial P}{\partial x}+\dfrac{\partial Q}{\partial y}+\dfrac{\partial R}{\partial z}=0$，故
$$\oiint_{S+S_1}\frac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}=\iiint_{V_r}\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}\right)\mathrm{d}V=0.$$

于是
$$I=\oiint_S\frac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}=-\oiint_{S_1}\frac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}$$
$$=\oiint_{S_1^-}\frac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}\xlongequal{(*)}\oiint_{S_1^-}\frac{1}{r^2}\mathrm{d}S=\frac{1}{r^2}\cdot4\pi r^2=4\pi$$
（$S_1^-$ 为 $S_1$ 的外侧）.

【注】① $(*)$ 利用两类积分之间的关系：
$$\iint_S P\mathrm{d}y\mathrm{d}z+Q\mathrm{d}z\mathrm{d}x+R\mathrm{d}x\mathrm{d}y=\iint_S(P\cos\alpha+Q\cos\beta+R\cos\gamma)\mathrm{d}S.$$
因为 $S_1:x^2+y^2+z^2=r^2$ 的法向量为 $\boldsymbol{n}=(2x,2y,2z)$，所以 $\cos\alpha=\dfrac{x}{r}$，$\cos\beta=\dfrac{y}{r}$，$\cos\gamma=\dfrac{z}{r}$，故
$$\oiint_{S_1^-}\frac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}=\oiint_{S_1^-}\frac{1}{r^2}(\cos^2\alpha+\cos^2\beta+\cos^2\gamma)\mathrm{d}S=\oiint_{S_1^-}\frac{1}{r^2}\mathrm{d}S.$$

② 计算 $\oiint_{S_1^-}\dfrac{x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y}{(x^2+y^2+z^2)^{\frac{3}{2}}}$ 时，也可代入 $S_1^-$ 的方程 $x^2+y^2+z^2=r^2$，化简得
$$\oiint_{S_1^-}\frac{x}{r^3}\mathrm{d}y\mathrm{d}z+\frac{y}{r^3}\mathrm{d}z\mathrm{d}x+\frac{z}{r^3}\mathrm{d}x\mathrm{d}y=\frac{1}{r^3}\oiint_{S_1^-}x\mathrm{d}y\mathrm{d}z+y\mathrm{d}z\mathrm{d}x+z\mathrm{d}x\mathrm{d}y$$
$$\xlongequal{\text{高斯公式}}\frac{1}{r^3}\iiint_V(1+1+1)\mathrm{d}V=\frac{1}{r^3}\cdot3\cdot\frac{4}{3}\pi r^3=4\pi.$$

+++

#### 综合解答 (19) 设曲面 $S$ 为球面 $x^2+y^2+z^2=4z$ 与锥面 $z=\dfrac{\sqrt{x^2+y^2}}{\sqrt{3}}$ 所围，且位于锥面上方部分的立体表面，流速场为 $\boldsymbol{A}(x,y,z)=\left(\dfrac{1}{3}x^3+x^2y+x^2z,\ \dfrac{1}{3}y^3+y^2z,\ \dfrac{1}{3}z^3\right)$，求 $\boldsymbol{A}(x,y,z)$ 从曲面 $S$ 内部流向外部的流量 $\Phi$.
***
依题设，流量为
$$\Phi=\oiint_S\left(\frac{1}{3}x^3+x^2y+x^2z\right)\mathrm{d}y\mathrm{d}z+\left(\frac{1}{3}y^3+y^2z\right)\mathrm{d}z\mathrm{d}x+\frac{1}{3}z^3\mathrm{d}x\mathrm{d}y.$$

利用高斯公式，得
$$\Phi=\iiint_V(x^2+2xy+2xz+y^2+2yz+z^2)\mathrm{d}V=\iiint_V(x^2+y^2+z^2)\mathrm{d}V+2\iiint_V(xy+xz+yz)\mathrm{d}V.$$

由 $V$ 关于 $xOz$ 面、$yOz$ 面对称，$xy$ 与 $yz$ 关于 $y$ 是奇函数，$xz$ 关于 $x$ 是奇函数，知
$$2\iiint_V(xy+xz+yz)\mathrm{d}V=0,$$
故
$$\Phi=\iiint_V(x^2+y^2+z^2)\mathrm{d}V\xlongequal{\text{球坐标}}\int_0^{2\pi}\mathrm{d}\theta\int_0^{\frac{\pi}{3}}\mathrm{d}\varphi\int_0^{4\cos\varphi}r^2\cdot r^2\sin\varphi\mathrm{d}r=\frac{336\pi}{5}.$$

【注】$x^2+y^2+z^2=4z$ 化为球面坐标为 $r=4\cos\varphi$；$z=\dfrac{\sqrt{x^2+y^2}}{\sqrt{3}}$，即 $z^2=\dfrac{1}{3}(x^2+y^2)\ (z\geqslant0)$，化为球面坐标为 $r^2\cos^2\varphi=\dfrac{1}{3}r^2\sin^2\varphi$，即 $\tan\varphi=\sqrt{3}$，故 $\varphi=\dfrac{\pi}{3}$.

+++

#### 综合解答 (20) 设 $f(x,y)$ 在 $D=\{(x,y)\mid x^2+y^2\leqslant1\}$ 上有二阶连续偏导数，且 $\dfrac{\partial^2f}{\partial x^2}+\dfrac{\partial^2f}{\partial y^2}=\mathrm{e}^{-(x^2+y^2)}$，计算 $I=\iint_D\left(x\dfrac{\partial f}{\partial x}+y\dfrac{\partial f}{\partial y}\right)\mathrm{d}x\mathrm{d}y$.
***
积分区域 $D$ 为单位圆盘 $x^2+y^2\leqslant1$.

$$I=\iint_D\left(x\frac{\partial f}{\partial x}+y\frac{\partial f}{\partial y}\right)\mathrm{d}x\mathrm{d}y\xlongequal{\text{极坐标}}\int_0^{2\pi}\mathrm{d}\theta\int_0^1(f'_x\cdot r\cos\theta+f'_y\cdot r\sin\theta)r\mathrm{d}r$$
$$=\int_0^1 r\mathrm{d}r\int_0^{2\pi}(f'_x\cdot r\cos\theta+f'_y\cdot r\sin\theta)\mathrm{d}\theta.$$

设 $L_r:x^2+y^2=r^2\ (0\leqslant r\leqslant1)$，取逆时针，$D_r:x^2+y^2\leqslant r^2$，则
$$\int_0^{2\pi}(f'_x\cdot r\cos\theta+f'_y\cdot r\sin\theta)\mathrm{d}\theta=\int_{L_r}-f'_y\mathrm{d}x+f'_x\mathrm{d}y=\iint_{D_r}\left(\frac{\partial^2f}{\partial x^2}+\frac{\partial^2f}{\partial y^2}\right)\mathrm{d}x\mathrm{d}y$$
$$=\iint_{D_r}\mathrm{e}^{-(x^2+y^2)}\mathrm{d}x\mathrm{d}y=\pi(1-\mathrm{e}^{-r^2}),$$
故
$$I=\iint_D\left(x\frac{\partial f}{\partial x}+y\frac{\partial f}{\partial y}\right)\mathrm{d}x\mathrm{d}y=\int_0^1\pi r(1-\mathrm{e}^{-r^2})\mathrm{d}r=\frac{\pi}{2\mathrm{e}}.$$

+++

#### 综合解答 (21) 设 $f(x,y)$ 在 $x^2+y^2\leqslant1$ 上有一阶连续偏导数，且在边界上取值为零，证明：$\lim\limits_{t\to0^+}\dfrac{-1}{2\pi}\iint_D\dfrac{xf'_x(x,y)+yf'_y(x,y)}{x^2+y^2}\mathrm{d}x\mathrm{d}y=f(0,0)$，其中 $D:t^2\leqslant x^2+y^2\leqslant1$，$t>0$.
***
应用极坐标计算，积分区域 $D$ 为圆环域 $t\leqslant r\leqslant1$.

$$\frac{xf'_x(x,y)+yf'_y(x,y)}{x^2+y^2}=\frac{f'_x(r\cos\theta,r\sin\theta)r\cos\theta+f'_y(r\cos\theta,r\sin\theta)r\sin\theta}{r^2},$$
故
$$\iint_D\frac{xf'_x(x,y)+yf'_y(x,y)}{x^2+y^2}\mathrm{d}x\mathrm{d}y=\iint_D\left[f'_x(r\cos\theta,r\sin\theta)\cos\theta+f'_y(r\cos\theta,r\sin\theta)\sin\theta\right]\mathrm{d}r\mathrm{d}\theta$$
$$=\int_0^{2\pi}\mathrm{d}\theta\int_t^1\frac{\partial f}{\partial r}\mathrm{d}r=\int_0^{2\pi}\left[f(r\cos\theta,r\sin\theta)\right]\Big|_t^1\mathrm{d}\theta=\int_0^{2\pi}\left[0-f(t\cos\theta,t\sin\theta)\right]\mathrm{d}\theta$$
$$=-2\pi f(t\cos\xi,t\sin\xi)\quad(\text{积分中值定理},\ 0\leqslant\xi\leqslant2\pi),$$
故
$$\lim_{t\to0^+}\frac{-1}{2\pi}\iint_D\frac{xf'_x(x,y)+yf'_y(x,y)}{x^2+y^2}\mathrm{d}x\mathrm{d}y=\lim_{t\to0^+}\frac{-1}{2\pi}\left[-2\pi f(t\cos\xi,t\sin\xi)\right]=f(0,0).$$

+++

#### 综合解答 (22) 设 $f(r)\ (r>0)$ 有二阶连续导数，$u=f\left(\sqrt{x^2+y^2+z^2}\right)$ 满足 $\mathrm{div}(\mathbf{grad}\,u)=\sqrt{x^2+y^2+z^2}$，求函数 $u$ 的表达式.
***
$$\mathbf{grad}\,u=\left(\frac{\partial u}{\partial x},\frac{\partial u}{\partial y},\frac{\partial u}{\partial z}\right)\xlongequal{\text{记}}(P,Q,R),$$
$$\mathrm{div}(\mathbf{grad}\,u)=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}=\frac{\partial^2u}{\partial x^2}+\frac{\partial^2u}{\partial y^2}+\frac{\partial^2u}{\partial z^2}.$$

而
$$\frac{\partial u}{\partial x}=f'(r)\frac{\partial r}{\partial x}=f'(r)\frac{x}{r}\quad\left(r=\sqrt{x^2+y^2+z^2}\right),$$
$$\frac{\partial^2u}{\partial x^2}=f''(r)\frac{x^2}{r^2}+f'(r)\frac{r^2-x^2}{r^3}.$$

考虑到 $u=f\left(\sqrt{x^2+y^2+z^2}\right)$ 关于 $x,y,z$ 具有轮换性，故
$$\frac{\partial^2u}{\partial y^2}=f''(r)\frac{y^2}{r^2}+f'(r)\frac{r^2-y^2}{r^3},\quad\frac{\partial^2u}{\partial z^2}=f''(r)\frac{z^2}{r^2}+f'(r)\frac{r^2-z^2}{r^3}.$$

将其代入 $\dfrac{\partial^2u}{\partial x^2}+\dfrac{\partial^2u}{\partial y^2}+\dfrac{\partial^2u}{\partial z^2}=\sqrt{x^2+y^2+z^2}$，得
$$f''(r)+\frac{2}{r}f'(r)=r,$$
为可降阶微分方程.

变形为 $\left[r^2f'(r)\right]'=r^3$，积分得 $r^2f'(r)=\dfrac{1}{4}r^4+C_1$，即 $f'(r)=\dfrac{1}{4}r^2+\dfrac{C_1}{r^2}$，再积分得 $f(r)=\dfrac{1}{12}r^3-\dfrac{C_1}{r}+C_2$，即
$$u=\frac{1}{12}(x^2+y^2+z^2)^{\frac{3}{2}}-C_1(x^2+y^2+z^2)^{-\frac{1}{2}}+C_2\quad(C_1,C_2\ \text{为任意常数}).$$
