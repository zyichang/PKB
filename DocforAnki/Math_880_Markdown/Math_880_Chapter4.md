---
quizify:
  format: 1
  deck: Math_880::Chapter_4
  tags: [Math, 880题, 数一, 第四章, 空间解析几何]
---

+++

#### 基础选择 (1) 设向量 $\boldsymbol{a}=(1,2,1)$，$\boldsymbol{b}=(-1,0,2)$，$\boldsymbol{c}=(0,k,-3)$ 共面，则 $k=$（　）。

;;;
A. $1$
B. $2$
C. $-1$
D. $-2$
;;;D
***
**D.**

解　向量 $\boldsymbol{a},\boldsymbol{b},\boldsymbol{c}$ 共面 $\Leftrightarrow[\boldsymbol{a}\ \boldsymbol{b}\ \boldsymbol{c}]=0$，即

$$
\begin{vmatrix}1&2&1\\-1&0&2\\0&k&-3\end{vmatrix}=0,
$$

解得 $k=-2$。

+++

#### 基础选择 (2) 设直线 $L_1:\dfrac{x-1}{1}=\dfrac{y-5}{-2}=\dfrac{z+8}{1}$ 与 $L_2:\begin{cases}x-y=6,\\ 2y+z=3,\end{cases}$ 则 $L_1$ 与 $L_2$ 的夹角为（　）。

;;;
A. $\dfrac{\pi}{6}$
B. $\dfrac{\pi}{4}$
C. $\dfrac{\pi}{3}$
D. $\dfrac{\pi}{2}$
;;;C
***
**C.**

解　$L_1$ 的方向向量为 $\boldsymbol{s}_1=(1,-2,1)$，$L_2$ 的方向向量为

$$
\boldsymbol{s}_2=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\1&-1&0\\0&2&1\end{vmatrix}=-\boldsymbol{i}-\boldsymbol{j}+2\boldsymbol{k}.
$$

设两直线夹角为 $\varphi$，则

$$
\cos\varphi=\frac{\boldsymbol{s}_1\cdot\boldsymbol{s}_2}{|\boldsymbol{s}_1||\boldsymbol{s}_2|}=\frac{3}{\sqrt6\times\sqrt6}=\frac12,
$$

故 $\varphi=\dfrac{\pi}{3}$。

+++

#### 基础选择 (3) 设直线 $L:\begin{cases}x+3y+2z+2=0,\\ 2x-y-10z-1=0,\end{cases}$ 平面 $\pi:4x-2y+z-2=0$，则直线 $L$（　）。

;;;
A. 平行于平面 $\pi$
B. 在平面 $\pi$ 上
C. 垂直于平面 $\pi$
D. 与平面 $\pi$ 斜交
;;;C
***
**C.**

解　直线 $L$ 的方向向量为

$$
\boldsymbol{s}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\1&3&2\\2&-1&-10\end{vmatrix}=(-28,14,-7),
$$

显然 $\boldsymbol{s}$ 与平面 $\pi$ 的法向量 $\boldsymbol{n}=(4,-2,1)$ 平行，故直线 $L$ **垂直于平面** $\pi$，C 正确。

+++

#### 基础选择 (4) 方程 $x^2-\dfrac{y^2}{4}+z^2=1$ 表示（　）。

;;;
A. 旋转双曲面
B. 双叶双曲面
C. 双曲柱面
D. 锥面
;;;A
***
**A.**

解　方程 $x^2-\dfrac{y^2}{4}+z^2=1$ 所表示的曲面，可视为在 $xOy$ 面上的双曲线 $x^2-\dfrac{y^2}{4}=1$ 绕 $y$ 轴旋转一周所得的**旋转单叶双曲面**。

**【注】** 考研大纲要求能识别常用的二次曲面，如：

① 单叶双曲面：$\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}-\dfrac{z^2}{c^2}=1$。\
② 双叶双曲面：$\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}-\dfrac{z^2}{c^2}=-1$。\
③ 椭圆抛物面：$\dfrac{x^2}{a^2}+\dfrac{y^2}{b^2}=cz$。\
④ 双曲抛物面（马鞍面）：$\dfrac{x^2}{a^2}-\dfrac{y^2}{b^2}=cz$。

+++

#### 基础选择 (5) 设非零向量 $\boldsymbol{\alpha}$ 与 $\boldsymbol{\beta}$ 满足 $|\boldsymbol{\alpha}-\boldsymbol{\beta}|=|\boldsymbol{\alpha}+\boldsymbol{\beta}|$，则必有（　）。

;;;
A. $\boldsymbol{\alpha}-\boldsymbol{\beta}=\boldsymbol{\alpha}+\boldsymbol{\beta}$
B. $\boldsymbol{\alpha}=\boldsymbol{\beta}$
C. $\boldsymbol{\alpha}\times\boldsymbol{\beta}=\boldsymbol{0}$
D. $\boldsymbol{\alpha}\cdot\boldsymbol{\beta}=0$
;;;D
***
**D.**

解　由题意及非零向量的加、减法，可知四边形的对角线相等（如图 4-1），故 $\boldsymbol{\alpha}\perp\boldsymbol{\beta}$，即 $\boldsymbol{\alpha}\cdot\boldsymbol{\beta}=0$，D 正确。

+++

#### 基础填空 (1) 设向量 $\boldsymbol{a}=(-1,3,0)$，$\boldsymbol{b}=(3,1,0)$，$|\boldsymbol{c}|=r$（常数）。当 $\boldsymbol{c}$ 满足 $\boldsymbol{a}=\boldsymbol{b}\times\boldsymbol{c}$ 时，$r$ 的最小值为________。
***
**$1$.**

解　设 $\boldsymbol{c}=x\boldsymbol{i}+y\boldsymbol{j}+z\boldsymbol{k}$，由 $\boldsymbol{a}=\boldsymbol{b}\times\boldsymbol{c}$，得

$$
-\boldsymbol{i}+3\boldsymbol{j}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\3&1&0\\x&y&z\end{vmatrix}=z\boldsymbol{i}+(-3z)\boldsymbol{j}+(3y-x)\boldsymbol{k},
$$

则有 $z=-1$，$3y-x=0$，于是 $\boldsymbol{c}=x\boldsymbol{i}+3x\boldsymbol{j}-\boldsymbol{k}$。又

$$
r=|\boldsymbol{c}|=\sqrt{x^2+(3x)^2+1}=\sqrt{1+10x^2},
$$

可知当 $x=0$ 时，$r$ 取得最小值 $1$。

+++

#### 基础填空 (2) 设向量 $\boldsymbol{a}=(2,-3,1)$，$\boldsymbol{b}=(1,-2,3)$，$\boldsymbol{c}=(2,1,2)$，向量 $\boldsymbol{r}$ 满足 $\boldsymbol{r}\perp\boldsymbol{a}$，$\boldsymbol{r}\perp\boldsymbol{b}$，$\mathrm{Prj}_{\boldsymbol{c}}\boldsymbol{r}=14$，则 $\boldsymbol{r}=$________。
***
**$(14,10,2)$.**

解　由 $\boldsymbol{r}\perp\boldsymbol{a}$，$\boldsymbol{r}\perp\boldsymbol{b}$，知 $\boldsymbol{r}\ /\!/\ \boldsymbol{a}\times\boldsymbol{b}$。令

$$
\boldsymbol{r}=k(\boldsymbol{a}\times\boldsymbol{b})=k\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\2&-3&1\\1&-2&3\end{vmatrix}=(-7k,-5k,-k).
$$

由于 $\mathrm{Prj}_{\boldsymbol{c}}\boldsymbol{r}=\dfrac{\boldsymbol{r}\cdot\boldsymbol{c}}{|\boldsymbol{c}|}=\dfrac{-21k}{3}=-7k=14$，故 $k=-2$，从而 $\boldsymbol{r}=(14,10,2)$。

+++

#### 基础填空 (3) 过点 $(2,0,-3)$ 且与直线 $\begin{cases}x-2y+4z-7=0,\\ 3x+5y-2z+1=0\end{cases}$ 垂直的平面方程为________。
***
**$16x-14y-11z-65=0$.**

解　直线的方向向量

$$
\boldsymbol{s}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\1&-2&4\\3&5&-2\end{vmatrix}=-16\boldsymbol{i}+14\boldsymbol{j}+11\boldsymbol{k},
$$

故所求平面的法向量 $\boldsymbol{n}=(-16,14,11)$，因此平面方程为

$$
-16(x-2)+14(y-0)+11(z+3)=0,
$$

即 $16x-14y-11z-65=0$。

+++

#### 基础填空 (4) 点 $P(1,-1,2)$ 到平面 $\pi:2x-y+5z-12=0$ 的距离 $d=$________。
***
**$\dfrac{\sqrt{30}}{30}$.**

解

$$
d=\frac{|2\times1-1\times(-1)+5\times2-12|}{\sqrt{2^2+(-1)^2+5^2}}=\frac{\sqrt{30}}{30}.
$$

+++

#### 基础填空 (5) 点 $P(1,-1,0)$ 到直线 $L:\dfrac{x}{3}=\dfrac{y}{3}=\dfrac{z+1}{2}$ 的距离 $d=$________。
***
**$\dfrac{\sqrt{341}}{11}$.**

解　直线 $L$ 过点 $P_0(0,0,-1)$，其方向向量 $\boldsymbol{s}=(3,3,2)$。又 $\overrightarrow{P_0P}=(1,-1,1)$，

$$
\overrightarrow{P_0P}\times\boldsymbol{s}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\1&-1&1\\3&3&2\end{vmatrix}=-5\boldsymbol{i}+\boldsymbol{j}+6\boldsymbol{k},
$$

故所求距离 $d=\dfrac{|\overrightarrow{P_0P}\times\boldsymbol{s}|}{|\boldsymbol{s}|}=\dfrac{\sqrt{341}}{11}$。

**【注】** 点 $P_0(x_0,y_0,z_0)$ 到直线 $L:\dfrac{x-x_1}{l}=\dfrac{y-y_1}{m}=\dfrac{z-z_1}{n}$ 的距离为

$$
d=\frac{|\boldsymbol{s}\times\overrightarrow{P_0P_1}|}{|\boldsymbol{s}|}=\frac{\left|\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\x_1-x_0&y_1-y_0&z_1-z_0\\l&m&n\end{vmatrix}\right|}{\sqrt{l^2+m^2+n^2}},
$$

其中 $P_1(x_1,y_1,z_1)\in L$，$\boldsymbol{s}=(l,m,n)$。

+++

#### 基础填空 (6) 直线 $L_1:\begin{cases}x-1=0,\\ y=z\end{cases}$ 与 $L_2:\begin{cases}x+2y=0,\\ z+2=0\end{cases}$ 之间的距离 $d=$________。
***
**$1$.**

解　先求过直线 $L_2$ 的平面 $\pi$，使平面 $\pi$ 平行于直线 $L_1$。设过直线 $L_2$ 的平面束方程 $\pi:(x+2y)+\lambda(z+2)=0$，即 $x+2y+\lambda z+2\lambda=0$。

由平面束 $\pi$ 平行于直线 $L_1$，知 $\boldsymbol{n}\perp\boldsymbol{s}$，其中 $\boldsymbol{n}=(1,2,\lambda)$，$\boldsymbol{s}=(0,1,1)$，故

$$
\boldsymbol{n}\cdot\boldsymbol{s}=(1,2,\lambda)\cdot(0,1,1)=2+\lambda=0,
$$

得 $\lambda=-2$，所求平面 $\pi$ 为 $x+2y-2z-4=0$，故 $L_1$ 上的点 $(1,0,0)$ 到平面 $\pi$ 的距离为

$$
d=\frac{|1+0+0-4|}{\sqrt{1^2+2^2+(-2)^2}}=1.
$$

**【注】** 直线 $L_1:\begin{cases}x-1=0,\\ y=z\end{cases}$ 化为对称式方程为 $\dfrac{x-1}{0}=\dfrac{y}{1}=\dfrac{z}{1}$，故其方向向量为 $\boldsymbol{s}=(0,1,1)$，且过点 $(1,0,0)$。

+++

#### 基础填空 (7) 直线 $L:\begin{cases}x+2y-3z=2,\\ 2x-y+z=3\end{cases}$ 在平面 $z=0$ 上的投影为________，在平面 $z=1$ 上的投影为________。
***
**$\begin{cases}7x-y=11,\\ z=0;\end{cases}$　$\begin{cases}7x-y=11,\\ z=1.\end{cases}$**

解　直线 $L$ 在 $z=0$ 上的投影为直线，由 $L$ 的方程中消去 $z$，得 $7x-y=11$，故 $L$ 在 $z=0$ 上的投影直线方程为

$$
\begin{cases}7x-y=11,\\ z=0.\end{cases}
$$

同理，$L$ 在平面 $z=1$ 上的投影直线方程为

$$
\begin{cases}7x-y=11,\\ z=1.\end{cases}
$$

+++

#### 基础填空 (8) 过点 $A(1,1,-1)$，$B(-2,-2,2)$ 和 $C(1,-1,2)$ 三点的平面方程为________。
***
**$x-3y-2z=0$.**

解　用平面的点法式方程，需求出平面的法向量 $\boldsymbol{n}$。由已知，$\overrightarrow{AB}=(-3,-3,3)$，$\overrightarrow{AC}=(0,-2,3)$，则 $\boldsymbol{n}\perp\overrightarrow{AB}$，$\boldsymbol{n}\perp\overrightarrow{AC}$，故

$$
\boldsymbol{n}=\overrightarrow{AB}\times\overrightarrow{AC}=\begin{vmatrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\-3&-3&3\\0&-2&3\end{vmatrix}=-3\boldsymbol{i}+9\boldsymbol{j}+6\boldsymbol{k},
$$

故所求平面方程为 $-3(x-1)+9(y-1)+6(z+1)=0$，即 $x-3y-2z=0$。

+++

#### 基础填空 (9) 曲线 $\begin{cases}x^2+2z^2=4,\\ y=0\end{cases}$ 绕 $z$ 轴旋转一周所得的旋转曲面方程为________。
***
**$x^2+y^2+2z^2=4$.**

解　设 $M_0(x_0,y_0,z_0)$ 是已知曲线上的一点，点 $M_0(x_0,y_0,z_0)$ 绕 $z$ 轴转到点 $M(x,y,z)$，此时 $z=z_0$。又点 $M$ 到 $z$ 轴的距离与点 $M_0$ 到 $z$ 轴的距离相等，故 $\sqrt{x^2+y^2}=|x_0|$，即

$$
x_0=\pm\sqrt{x^2+y^2},\quad z_0=z,
$$

从而旋转曲面方程为 $x^2+y^2+2z^2=4$。

**【注】** 一般地，曲线 $\begin{cases}f(x,z)=0,\\ y=0\end{cases}$ 绕 $z$ 轴与 $x$ 轴旋转一周所得的曲面方程分别为

$$
f(\pm\sqrt{x^2+y^2},z)=0,\quad f(x,\pm\sqrt{y^2+z^2})=0.
$$

曲线 $\begin{cases}f(x,y)=0,\\ z=0\end{cases}$ 绕 $x$ 轴与 $y$ 轴旋转一周所得的曲面方程分别为

$$
f(x,\pm\sqrt{y^2+z^2})=0,\quad f(\pm\sqrt{x^2+z^2},y)=0.
$$

曲线 $\begin{cases}f(y,z)=0,\\ x=0\end{cases}$ 绕 $y$ 轴与 $z$ 轴旋转一周所得的曲面方程分别为

$$
f(y,\pm\sqrt{x^2+z^2})=0,\quad f(\pm\sqrt{x^2+y^2},z)=0.
$$

+++

#### 基础填空 (10) 曲线 $\begin{cases}z=2x^2+3y^2,\\ z=12-x^2-3y^2\end{cases}$ 在 $xOy$ 面上的投影曲线方程为________。
***
**$\begin{cases}\dfrac{x^2}{4}+\dfrac{y^2}{2}=1,\\ z=0.\end{cases}$**

解　由 $\begin{cases}z=2x^2+3y^2,\\ z=12-x^2-3y^2\end{cases}$ 消去 $z$，可得曲线在 $xOy$ 面上的投影柱面方程为

$$
\frac{x^2}{4}+\frac{y^2}{2}=1,
$$

故它在 $xOy$ 面上的投影曲线方程为

$$
\begin{cases}\dfrac{x^2}{4}+\dfrac{y^2}{2}=1,\\ z=0.\end{cases}
$$

**【注】** 求空间曲线 $L:\begin{cases}F(x,y,z)=0,\\ G(x,y,z)=0\end{cases}$ 在 $xOy$ 面上的投影曲线方程，一般方法是由上面方程组消去 $z$，得 $H(x,y)=0$，则曲线 $L$ 在 $xOy$ 面上的投影曲线是

$$
\begin{cases}H(x,y)=0,\\ z=0.\end{cases}
$$

类似地，可求得空间曲线在 $yOz$ 面、$xOz$ 面上的投影曲线方程。求投影曲线是数学一常考内容。

+++

#### 基础填空 (11) 设 $\boldsymbol{\alpha}$ 与 $\boldsymbol{\beta}$ 均为单位向量，其夹角为 $\dfrac{\pi}{6}$，则以 $\boldsymbol{\alpha}+2\boldsymbol{\beta}$ 与 $3\boldsymbol{\alpha}+\boldsymbol{\beta}$ 为邻边的平行四边形的面积为________。
***
**$\dfrac52$.**

解　所求平行四边形的面积为

$$
\begin{aligned}
A&=|(\boldsymbol{\alpha}+2\boldsymbol{\beta})\times(3\boldsymbol{\alpha}+\boldsymbol{\beta})|=|\boldsymbol{\alpha}\times\boldsymbol{\beta}+6\boldsymbol{\beta}\times\boldsymbol{\alpha}|\\
&=|\boldsymbol{\alpha}\times\boldsymbol{\beta}-6\boldsymbol{\alpha}\times\boldsymbol{\beta}|=|-5\boldsymbol{\alpha}\times\boldsymbol{\beta}|\\
&=5|\boldsymbol{\alpha}\times\boldsymbol{\beta}|=5|\boldsymbol{\alpha}||\boldsymbol{\beta}|\sin\widehat{(\boldsymbol{\alpha},\boldsymbol{\beta})}=\frac52.
\end{aligned}
$$

**【注】** 以 $\boldsymbol{\alpha},\boldsymbol{\beta}$ 为邻边的平行四边形的面积等于 $\boldsymbol{\alpha}$ 与 $\boldsymbol{\beta}$ 的向量积的模。

+++

#### 基础填空 (12) 设 $\boldsymbol{\alpha}$ 与 $\boldsymbol{\beta}$ 是非零常向量，$|\boldsymbol{\beta}|=2$（$|\boldsymbol{\beta}|$ 表示 $\boldsymbol{\beta}$ 的模），$\boldsymbol{\alpha}$ 与 $\boldsymbol{\beta}$ 之间的夹角为 $\dfrac{\pi}{3}$，求 $\lim\limits_{x\to0}\dfrac{|\boldsymbol{\alpha}+x\boldsymbol{\beta}|-|\boldsymbol{\alpha}|}{x}=$________。
***
**$1$.**

解

$$
\begin{aligned}
\lim_{x\to0}\frac{|\boldsymbol{\alpha}+x\boldsymbol{\beta}|-|\boldsymbol{\alpha}|}{x}
&=\lim_{x\to0}\frac{(\boldsymbol{\alpha}+x\boldsymbol{\beta})\cdot(\boldsymbol{\alpha}+x\boldsymbol{\beta})-\boldsymbol{\alpha}\cdot\boldsymbol{\alpha}}{x(|\boldsymbol{\alpha}+x\boldsymbol{\beta}|+|\boldsymbol{\alpha}|)}\\
&=\lim_{x\to0}\frac{2x\boldsymbol{\alpha}\cdot\boldsymbol{\beta}+x^2\boldsymbol{\beta}\cdot\boldsymbol{\beta}}{2|\boldsymbol{\alpha}|x}=\frac{\boldsymbol{\alpha}\cdot\boldsymbol{\beta}}{|\boldsymbol{\alpha}|}+0\\
&=|\boldsymbol{\beta}|\cos\widehat{(\boldsymbol{\alpha},\boldsymbol{\beta})}=2\times\frac12=1.
\end{aligned}
$$

+++

#### 基础解答 (1) 求平行于平面 $x+y+z=9$ 且与球面 $x^2+y^2+z^2=4$ 相切的平面方程。
***
解　由于所求平面与平面 $x+y+z=9$ 平行，故可设其为平面 $\pi:x+y+z+D=0$，又因平面 $\pi$ 与球面 $x^2+y^2+z^2=4$ 相切，所以球心 $O(0,0,0)$ 到平面 $\pi$ 的距离为

$$
\frac{|0+0+0+D|}{\sqrt{1^2+1^2+1^2}}=2,
$$

解得 $D=\pm2\sqrt3$，故所求平面方程为

$$
x+y+z+2\sqrt3=0\ \text{或}\ x+y+z-2\sqrt3=0.
$$

+++

#### 基础解答 (2) 设平面 $\pi$ 与点 $P(1,2,1)$ 的距离为 $1$，且过直线 $L:\begin{cases}3x-2y+2=0,\\ x-2y-z+6=0,\end{cases}$ 求平面 $\pi$ 的方程。
***
解　过直线 $L$ 的平面束方程为

$$
(3x-2y+2)+\lambda(x-2y-z+6)=0,
$$

即

$$
(3+\lambda)x-(2+2\lambda)y-\lambda z+(2+6\lambda)=0.
$$

由已知，

$$
d=\frac{|(3+\lambda)-2(2+2\lambda)-\lambda+(2+6\lambda)|}{\sqrt{(3+\lambda)^2+(2+2\lambda)^2+\lambda^2}}=1,
$$

即 $|2\lambda+1|=\sqrt{6\lambda^2+14\lambda+13}$，化简得

$$
\lambda^2+5\lambda+6=0,
$$

解得 $\lambda=-2$，$\lambda=-3$，故所求平面 $\pi$ 的方程为

$$
x+2y+2z-10=0\ \text{或}\ 4y+3z-16=0.
$$

**【注】** 求过直线的平面方程，常利用平面束方程进行求解。

+++

#### 基础解答 (3) 设平面 $\pi$ 过直线 $L:\begin{cases}x+5y+z=0,\\ x-z+4=0,\end{cases}$ 且与平面 $\pi_1:x-4y-8z+12=0$ 的夹角为 $45^\circ$，求平面 $\pi$ 的方程。
***
解　过直线 $L$ 的平面束方程为

$$
(x-z+4)+\lambda(x+5y+z)=0,
$$

即

$$
(1+\lambda)x+5\lambda y+(\lambda-1)z+4=0.
$$

由于平面 $\pi$ 与平面 $\pi_1$ 夹角为 $45^\circ$，即两平面的法向量夹角为 $45^\circ$，故

$$
\cos45^\circ=\frac{\sqrt2}{2}=\frac{(1+\lambda)+5\lambda\cdot(-4)+(\lambda-1)\cdot(-8)}{\sqrt{1^2+(-4)^2+(-8)^2}\cdot\sqrt{(1+\lambda)^2+(5\lambda)^2+(\lambda-1)^2}}=\frac{9-27\lambda}{9\sqrt{27\lambda^2+2}}=\frac{1-3\lambda}{\sqrt{27\lambda^2+2}},
$$

解得 $\lambda=0$，$\lambda=-\dfrac43$，故平面 $\pi$ 的方程为

$$
x-z+4=0\ \text{或}\ x+20y+7z-12=0.
$$

+++

#### 基础解答 (4) 求直线 $L:\dfrac{x+2}{3}=\dfrac{2-y}{1}=\dfrac{z+1}{2}$ 在平面 $\pi:2x+3y+3z-8=0$ 上的投影直线方程。
***
解　用平面束方程求出经过直线 $L$ 且与平面 $\pi$ 垂直的平面，该平面与平面 $\pi$ 的方程联立，便可得投影直线方程。

将直线 $L$ 变形为一般式：$\begin{cases}x+3y-4=0,\\ 2x-3z+1=0,\end{cases}$ 故过 $L$ 的平面束方程为

$$
x+3y-4+\lambda(2x-3z+1)=0,
$$

即

$$
(1+2\lambda)x+3y-3\lambda z+\lambda-4=0.
$$

此平面与平面 $\pi$ 垂直，故

$$
(1+2\lambda,3,-3\lambda)\cdot(2,3,3)=11-5\lambda=0,
$$

解得 $\lambda=\dfrac{11}{5}$，于是与平面 $\pi:2x+3y+3z-8=0$ 垂直的平面方程为

$$
\left(1+\frac{22}{5}\right)x+3y-\frac{33}{5}z+\frac{11}{5}-4=0,
$$

即 $9x+5y-11z-3=0$，故所求投影直线方程为

$$
\begin{cases}9x+5y-11z-3=0,\\ 2x+3y+3z-8=0.\end{cases}
$$

+++

#### 基础解答 (5) 求过点 $(-1,2,3)$，垂直于直线 $\dfrac{x}{4}=\dfrac{y}{5}=\dfrac{z}{6}$ 且平行于平面 $7x+8y+9z+10=0$ 的直线方程。
***
解　依题设，解题关键是求所求直线的方向向量 $\boldsymbol{s}=(m,n,p)$。由已知，

$$
\begin{cases}(m,n,p)\cdot(4,5,6)=0,\\ (m,n,p)\cdot(7,8,9)=0,\end{cases}
$$

即

$$
\begin{cases}4m+5n+6p=0,\\ 7m+8n+9p=0.\end{cases}
$$

任取其一组非零解均可作为方向向量，不妨取 $\boldsymbol{s}=(1,-2,1)$，故所求直线方程为

$$
\frac{x+1}{1}=\frac{y-2}{-2}=\frac{z-3}{1}.
$$

+++

#### 基础解答 (6) 求与直线 $L_1:x+2=3-y=z+1$ 和 $L_2:\dfrac{x+4}{2}=y=\dfrac{z-4}{3}$ 都垂直相交的直线方程。
***
**解法 1**　依题意，所求直线的方向向量为

$$
\boldsymbol{s}=(1,-1,1)\times(2,1,3)=(-4,-1,3).
$$

由已知，所求直线 $L$ 既在 $L_1$ 与 $L$ 所确定的平面内，又在 $L_2$ 与 $L$ 所确定的平面内，即直线 $L$ 为两平面的交线。

直线 $L_1$ 与 $L$ 所确定的平面的法向量为

$$
(1,-1,1)\times(-4,-1,3)=(-2,-7,-5);
$$

直线 $L_2$ 与 $L$ 所确定的平面的法向量为

$$
(2,1,3)\times(-4,-1,3)=(6,-18,2).
$$

综上可知，所求直线为

$$
\begin{cases}2(x+2)+7(y-3)+5(z+1)=0,\\ 3(x+4)-9y+(z-4)=0,\end{cases}
$$

即

$$
\begin{cases}2x+7y+5z-12=0,\\ 3x-9y+z+8=0.\end{cases}
$$

**解法 2**　分别在直线 $L_1,L_2$ 上任取一点，则使该两点之间的连线，平行于所求直线的方向向量为

$$
\boldsymbol{s}=(1,-1,1)\times(2,1,3)=(-4,-1,3).
$$

将 $L_1$ 与 $L_2$ 写成参数式方程的形式，有

$$
x_1=-2+t,\ y_1=3-t,\ z_1=-1+t,
$$

$$
x_2=-4+2u,\ y_2=u,\ z_2=4+3u,
$$

其中 $t,u$ 为参数。由

$$
\frac{x_1-x_2}{-4}=\frac{y_1-y_2}{-1}=\frac{z_1-z_2}{3},
$$

解得 $t=2$，$u=0$。

所求直线为点 $(0,1,1)$ 与点 $(-4,0,4)$ 的连线，故所求直线为

$$
\frac{x-0}{-4}=\frac{y-1}{-1}=\frac{z-1}{3}.
$$

+++

#### 基础解答 (7) 求直线 $L_1:\dfrac{x-3}{2}=y=\dfrac{z-1}{0}$ 与 $L_2:\dfrac{x+1}{1}=\dfrac{y-2}{0}=z$ 的公垂线方程。
***
解　分别求出公垂线与 $L_1$ 及 $L_2$ 确定的平面，将二者联立即为所求。

如图 4-2 所示，设 $L$ 为所求公垂线，则 $L$ 在由 $L_1$ 与 $L$ 确定的平面 $\pi_1$ 上，$L$ 也在由 $L$ 和 $L_2$ 确定的平面 $\pi_2$ 上，因此 $L$ 的方向向量为

$$
\boldsymbol{s}=(2,1,0)\times(1,0,1)=(1,-2,-1),
$$

故平面 $\pi_1$ 与平面 $\pi_2$ 的法向量分别为

$$
\boldsymbol{n}_1=\boldsymbol{s}\times(2,1,0)=(1,-2,-1)\times(2,1,0)=(1,-2,5),
$$

$$
\boldsymbol{n}_2=\boldsymbol{s}\times(1,0,1)=(1,-2,-1)\times(1,0,1)=(-2,-2,2),
$$

平面 $\pi_1$ 和平面 $\pi_2$ 的方程分别为

$$
(x-3)-2(y-0)+5(z-1)=0
$$

和

$$
-2(x+1)-2(y-2)+2(z-0)=0,
$$

即

$$
\pi_1:x-2y+5z-8=0,\quad \pi_2:x+y-z-1=0,
$$

故公垂线方程为

$$
\begin{cases}x-2y+5z-8=0,\\ x+y-z-1=0.\end{cases}
$$

**【注】** 对于有关直线、平面较复杂的题目，可先根据题中条件作出直线、平面相互位置的草图，结合几何图形找出直线方向向量、平面法向量之间的关系，从而解决问题。

+++

#### 基础解答 (8) 求直线 $\dfrac{x-1}{0}=\dfrac{y}{1}=\dfrac{z-1}{2}$ 绕 $z$ 轴旋转一周所得的旋转曲面方程。
***
解　已知直线的参数方程为

$$
\begin{cases}x=1,\\ y=t,\\ z=2t+1\end{cases}\quad(t\ \text{为参数}),
$$

其上任一点 $M_0(x_0,y_0,z_0)$ 绕 $z$ 轴旋转至某一点 $M(x,y,z)$ 时，有

$$
\begin{cases}x_0^2+y_0^2=x^2+y^2=1+t^2,\\ z=z_0=2t+1,\end{cases}
$$

消去 $t$，得曲面上任一点坐标满足的关系式，即旋转曲面方程为

$$
x^2+y^2-\left(\frac{z-1}{2}\right)^2=1,
$$

它是一个单叶双曲面。

**【注】** 求空间曲线 $L:x=x(t),\ y=y(t),\ z=z(t)$ 绕 $z$ 轴旋转一周所得旋转曲面方程，一般方法为固定一个 $t$，即得 $L$ 上一点 $M(x(t),y(t),z(t))$，点 $M$ 到 $z$ 轴的距离为

$$
d=\sqrt{x^2+y^2}=\sqrt{x^2(t)+y^2(t)}.
$$

点 $M$ 绕 $z$ 轴旋转一周所得圆周为

$$
\begin{cases}x^2+y^2=x^2(t)+y^2(t),\\ z=z(t).\end{cases}
$$

上式即为旋转曲面上任一点满足的关系式，消去 $t$ 便得旋转曲面的直角坐标方程。求旋转曲面方程是数学一的重要考点。

+++

#### 基础解答 (9) 求直线 $L:\dfrac{x-1}{3}=\dfrac{y-2}{4}=\dfrac{z+1}{1}$ 绕直线 $\begin{cases}x=2,\\ y=3\end{cases}$ 旋转一周所得的曲面方程。
***
解　设 $M_0(x_0,y_0,z_0)$ 是 $L$ 上任一点，定直线 $\begin{cases}x=2,\\ y=3\end{cases}$ 平行于 $z$ 轴，所以当点 $M_0$ 转到点 $M(x,y,z)$ 时，有

$$
z=z_0,\qquad\qquad ①
$$

$$
(x-2)^2+(y-3)^2=(x_0-2)^2+(y_0-3)^2.\qquad ②
$$

又 $M_0(x_0,y_0,z_0)$ 在 $L$ 上，故 $x_0=3z_0+4$，$y_0=4z_0+6$，

$$
(x_0-2)^2=(3z_0+2)^2,\qquad ③
$$

$$
(y_0-3)^2=(4z_0+3)^2.\qquad ④
$$

将 ①③④ 式代入 ② 式，得曲面方程

$$
(x-2)^2+(y-3)^2=(3z+2)^2+(4z+3)^2,
$$

即

$$
x^2+y^2-25z^2-4x-6y-36z=0.
$$

+++

#### 拓展解答 (1) 求满足下列条件的动点的轨迹方程，并说明它们分别表示什么曲面。

（Ⅰ）动点到坐标原点的距离等于它到平面 $z=4$ 的距离；\
（Ⅱ）动点到坐标原点的距离等于它到点 $(2,3,4)$ 的距离的一半；\
（Ⅲ）动点到点 $(0,0,5)$ 的距离等于它到 $x$ 轴的距离；\
（Ⅳ）动点到 $x$ 轴的距离等于它到 $yOz$ 面的距离的两倍。
***
解　设动点为 $(x,y,z)$。

（Ⅰ）

$$
\sqrt{x^2+y^2+z^2}=|z-4|,
$$

即 $x^2+y^2+8z=16$，它是以 $z$ 轴为旋转轴的**旋转抛物面**。

（Ⅱ）

$$
\sqrt{x^2+y^2+z^2}=\frac12\sqrt{(x-2)^2+(y-3)^2+(z-4)^2},
$$

即

$$
3(x^2+y^2+z^2)+4x+6y+8z=29,
$$

$$
\left(x+\frac23\right)^2+(y+1)^2+\left(z+\frac43\right)^2=\frac{116}{9},
$$

它是以点 $\left(-\dfrac23,-1,-\dfrac43\right)$ 为球心，$\dfrac{2\sqrt{29}}{3}$ 为半径的**球面**。

（Ⅲ）动点 $(x,y,z)$ 到 $x$ 轴的距离为 $\sqrt{y^2+z^2}$，故

$$
\sqrt{x^2+y^2+(z-5)^2}=\sqrt{y^2+z^2},
$$

即 $25+x^2=10z$，它是母线平行于 $y$ 轴的**抛物柱面**。

（Ⅳ）动点 $(x,y,z)$ 到 $yOz$ 面的距离为 $|x|$，故 $\sqrt{y^2+z^2}=2|x|$，即

$$
4x^2-y^2-z^2=0,
$$

它是以坐标原点为顶点，$x$ 轴为对称轴的**圆锥面**。
