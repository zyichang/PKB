---
quizify:
  format: 1
  deck: Math_880::Chapter_2
  tags: [Math, 880题, 数一, 第二章, 一元函数微分学]
---
+++

#### 基础选择 (1) 设 $f(x)=\begin{cases}\dfrac{1-\cos x}{\sqrt{x}},&x>0,\\[2mm] x^2\cdot\varphi(x),&x\leqslant 0,\end{cases}$ 其中 $\varphi(x)$ 是有界函数，则 $f(x)$ 在 $x=0$ 处（　）。

;;;
A. 可导
B. 连续，但不可导
C. 极限存在，但不连续
D. 极限不存在
;;;A

***

$\lim\limits_{x\to0^+}f(x)=\lim\limits_{x\to0^+}\dfrac{1-\cos x}{\sqrt{x}}=\lim\limits_{x\to0^+}\dfrac{\frac12x^2}{\sqrt{x}}=0$，$\lim\limits_{x\to0^-}f(x)=\lim\limits_{x\to0^-}x^2\varphi(x)=0$，又 $f(0)=0$，故连续。

$f'_+(0)=\lim\limits_{x\to0^+}\dfrac{1-\cos x}{x\sqrt{x}}=\lim\limits_{x\to0^+}\dfrac{\frac12x^2}{x\sqrt{x}}=0$，$f'_-(0)=\lim\limits_{x\to0^-}\dfrac{x^2\varphi(x)}{x}=0$，故 $f'(0)=0$，**A** 正确。

+++

#### 基础选择 (2) 设 $f'(x)$ 存在，$a,b$ 为任意实数，则 $\lim\limits_{\Delta x\to0}\dfrac{f(x+a\Delta x)-f(x-b\Delta x)}{\Delta x}=$（　）。

;;;
A. $(a+b)f'(x)$
B. $(a-b)f'(x)$
C. $af'(x)$
D. $bf'(x)$
;;;A

***

拆项：

$$
\lim\limits_{\Delta x\to0}\left[a\cdot\dfrac{f(x+a\Delta x)-f(x)}{a\Delta x}+b\cdot\dfrac{f(x-b\Delta x)-f(x)}{-b\Delta x}\right]=af'(x)+bf'(x)=(a+b)f'(x).
$$

+++

#### 基础选择 (3) 设 $f(x)=\dfrac{\sqrt{x}}{\sqrt{1+x}+1}$，则 $f(x)$ 在 $x=0$ 处（　）。

;;;
A. 连续且可导
B. 右连续但右导数不存在
C. 右连续且右导数存在
D. 右极限存在且右导数存在
;;;B

***

$\lim\limits_{x\to0^+}f(x)=\lim\limits_{x\to0^+}\dfrac{\sqrt{x}}{\sqrt{1+x}+1}=0=f(0)$，故右连续。

$\lim\limits_{x\to0^+}\dfrac{f(x)-f(0)}{x-0}=\lim\limits_{x\to0^+}\dfrac{\frac{\sqrt{x}}{\sqrt{1+x}+1}}{x}=\infty$，故 $f'_+(0)$ 不存在，选 **B**。

+++

#### 基础选择 (4) $f(x)=(x^2+3x+2)\,|x^3-x|$ 不可导点的个数为（　）。

;;;
A. 1
B. 2
C. 3
D. 4
;;;B

***

$f(x)=(x+2)(x+1)\,|x+1||x||x-1|$。$(x+1)$ 因子被 $(x+1)$ 平方化抵消，故 $f(x)$ 仅在 $x=0,\ x=1$ 两处不可导，共 **2** 个。

+++

#### 基础选择 (5) 下列函数中，在 $x=0$ 处不可导的是（　）。

;;;
A. $f(x)=|x|\sin|x|$
B. $f(x)=|x|\sin\sqrt{|x|}$
C. $f(x)=\cos|x|$
D. $f(x)=\cos\sqrt{|x|}$
;;;D

***

对 D：$f'_+(0)=\lim\limits_{x\to0^+}\dfrac{\cos\sqrt{|x|}-1}{x}=\lim\limits_{x\to0^+}\dfrac{-\frac12|x|}{x}=-\dfrac12$，$f'_-(0)=\lim\limits_{x\to0^-}\dfrac{-\frac12|x|}{x}=\dfrac12$，左右导数不等，故 $\cos\sqrt{|x|}$ 在 $x=0$ 处不可导，选 **D**。

+++

#### 基础选择 (6) 设 $f(x)$ 可导且 $f'(x_0)=\dfrac12$，则当 $\Delta x\to0$ 时，$f(x)$ 在 $x_0$ 处的微分 $\mathrm{d}y$ 是 $\Delta x$ 的（　）无穷小。

;;;
A. 等价
B. 同阶
C. 低阶
D. 高阶
;;;B

***

由微分定义 $\mathrm{d}y=f'(x_0)\Delta x$，故 $\lim\limits_{\Delta x\to0}\dfrac{\mathrm{d}y}{\Delta x}=\lim\limits_{\Delta x\to0}\dfrac{\frac12\Delta x}{\Delta x}=\dfrac12$，为**同阶**（非等价）无穷小，选 **B**。

+++

#### 基础选择 (7) 设 $f(-x)=-f(x)$，且在 $(0,+\infty)$ 内 $f'(x)>0$，$f''(x)>0$，则 $f(x)$ 在 $(-\infty,0)$ 内必有（　）。

;;;
A. $f'(x)<0,\ f''(x)<0$
B. $f'(x)<0,\ f''(x)>0$
C. $f'(x)>0,\ f''(x)<0$
D. $f'(x)>0,\ f''(x)>0$
;;;C

***

$f(x)$ 是奇函数，则 $f'(x)$ 是偶函数、$f''(x)$ 是奇函数。由 $(0,+\infty)$ 上 $f'>0$ 得 $(-\infty,0)$ 上 $f'(x)>0$；由 $(0,+\infty)$ 上 $f''>0$ 得 $(-\infty,0)$ 上 $f''(x)<0$，选 **C**。

+++

#### 基础选择 (8) 设 $f(x)$ 在 $x=0$ 的某邻域内连续，$f(0)=0$，$\lim\limits_{x\to0}\dfrac{f(x)}{1-\cos x}=2$，则 $f(x)$ 在 $x=0$ 处（　）。

;;;
A. 不可导
B. 可导且 $f'(0)\neq0$
C. 有极小值
D. 有极大值
;;;C

***

$f'(0)=\lim\limits_{x\to0}\dfrac{f(x)}{x}=\lim\limits_{x\to0}\dfrac{f(x)}{1-\cos x}\cdot\dfrac{1-\cos x}{x}=2\cdot0=0$，排除 A、B。

再由 $\lim\limits_{x\to0}\dfrac{f(x)}{1-\cos x}=2>0$ 及保号性、$1-\cos x>0$，知在 $x=0$ 邻域内 $f(x)>0=f(0)$，故 $f(0)$ 为**极小值**，选 **C**。

+++

#### 基础选择 (9) $y=(x-1)^2(x-3)^2$ 的拐点个数为（　）。

;;;
A. 0
B. 1
C. 2
D. 3
;;;C

***

$y'=4(x-1)(x-2)(x-3)$，则 $y''$ 是二次函数，最多两个零点。由罗尔定理，$y''$ 在 $(1,2)$ 和 $(2,3)$ 内各有一个零点，且两侧变号，故有 **2** 个拐点，选 **C**。

+++

#### 基础选择 (10) 设 $f'(x_0)=f''(x_0)=0$，$f'''(x_0)>0$，则下列选项正确的是（　）。

;;;
A. $x_0$ 是 $f(x)$ 的极值点
B. $f(x_0)$ 是 $f(x)$ 的极大值
C. $f(x_0)$ 是 $f(x)$ 的极小值
D. $(x_0,f(x_0))$ 是 $y=f(x)$ 的拐点
;;;D

***

$f'''(x_0)=\lim\limits_{x\to x_0}\dfrac{f''(x)}{x-x_0}>0$，由保号性知 $x>x_0$ 时 $f''>0$、$x<x_0$ 时 $f''<0$，即 $f''$ 在 $x_0$ 两侧变号，故 $(x_0,f(x_0))$ 是拐点，选 **D**。

（注：A 错，如 $f(x)=x^3$，$f'(0)=f''(0)=0$、$f'''(0)=6\neq0$，但 $x=0$ 非极值点。）

+++

#### 基础选择 (11) 设 $f(x)$ 有一阶连续导数，$F(x)=f(x)(1+|\sin x|)$，则 $f(0)=0$ 是 $F(x)$ 在 $x=0$ 处可导的（　）。

;;;
A. 必要非充分条件
B. 充分非必要条件
C. 充分必要条件
D. 既非充分又非必要条件
;;;C

***

$F'_+(0)=\lim\limits_{x\to0^+}\dfrac{f(x)(1+\sin x)-f(0)}{x}=f'_+(0)+f(0)$；同理 $F'_-(0)=f'_-(0)-f(0)$。

$F(x)$ 在 $0$ 可导 $\Leftrightarrow F'_+(0)=F'_-(0)\Leftrightarrow f(0)=0$，故是**充分必要条件**，选 **C**。

+++

#### 基础选择 (12) 设 $f(x)$ 有任意阶导数，且 $f'(x)=f^2(x)$，则 $f^{(n)}(x)=$（　）$(n>3)$。

;;;
A. $n!\,f^{n+1}(x)$
B. $n\,f^{n+1}(x)$
C. $f^{2n}(x)$
D. $n!\,f^{2n}(x)$
;;;A

***

$f''=2f\cdot f'=2f^3$，$f'''=2\cdot3f^2f'=3!\,f^4$，归纳得 $f^{(n)}(x)=n!\,f^{n+1}(x)$，选 **A**。

+++

#### 基础选择 (13) 设 $y=\ln(1-2x)$，则 $y^{(10)}=$（　）。

;;;
A. $\dfrac{-9!}{(1-2x)^{10}}$
B. $\dfrac{9!}{(1-2x)^{10}}$
C. $\dfrac{-9!\cdot 2^{10}}{(1-2x)^{10}}$
D. $\dfrac{10!\cdot 2^{9}}{(1-2x)^{10}}$
;;;C

***

$y'=(1-2x)^{-1}(-2)$，$y''=(-1)(1-2x)^{-2}(-2)^2$，……归纳：

$$
y^{(10)}=(-1)(-2)\cdots(-9)(1-2x)^{-10}(-2)^{10}=\dfrac{-9!\cdot2^{10}}{(1-2x)^{10}}.
$$

+++

#### 基础选择 (14) 设 $\delta>0$，$f(x)$ 在 $(-\delta,\delta)$ 内有定义，当 $x\in(-\delta,\delta)$ 时有 $|f(x)|\leqslant x^2$，则 $x=0$ 是 $f(x)$ 的（　）。

;;;
A. 间断点
B. 连续但不可导点
C. 可导点且 $f'(0)=0$
D. 可导点且 $f'(0)\neq0$
;;;C

***

由 $|f(0)|\leqslant0$ 知 $f(0)=0$。又 $0\leqslant\left|\dfrac{f(x)-f(0)}{x-0}\right|=\left|\dfrac{f(x)}{x}\right|\leqslant\dfrac{x^2}{|x|}=|x|$，由夹逼准则 $\lim\limits_{x\to0}\dfrac{f(x)}{x}=0$，即 $f'(0)=0$，选 **C**。

+++

#### 基础选择 (15) 设 $f(x)$ 连续，且 $f'(x_0)>0$，则存在 $\delta>0$，使得（　）。

;;;
A. 对任意 $x\in(x_0-\delta,x_0)$，有 $f(x)>f(x_0)$
B. 对任意 $x\in(x_0,x_0+\delta)$，有 $f(x)>f(x_0)$
C. $f(x)$ 在 $(x_0-\delta,x_0)$ 内单调减少
D. $f(x)$ 在 $(x_0,x_0+\delta)$ 内单调增加
;;;B

***

$f'_+(x_0)=\lim\limits_{x\to x_0^+}\dfrac{f(x)-f(x_0)}{x-x_0}>0$，由保号性，对 $x\in(x_0,x_0+\delta)$ 有 $f(x)>f(x_0)$，选 **B**。（A 反向不成立；C、D 由一点导数正不能推出邻域单调性。）

+++

#### 基础选择 (16) 已知 $y=x^3+ax^2+bx+c$ 在 $x=-2$ 处取得极值，且与直线 $y=-3x+3$ 相切于点 $(1,0)$，则（　）。

;;;
A. $a=1,\ b=-8,\ c=6$
B. $a=-1,\ b=-8,\ c=-6$
C. $a=1,\ b=8,\ c=-6$
D. $a=-1,\ b=8,\ c=-6$
;;;A

***

由 $y'(-2)=0,\ y'(1)=-3,\ y(1)=0$：

$$
\begin{cases}12-4a+b=0,\\ 3+2a+b=-3,\\ 1+a+b+c=0,\end{cases}\Rightarrow a=1,\ b=-8,\ c=6,
$$

选 **A**。

+++

#### 基础选择 (17) 设 $f'(x)=\dfrac{(x^2-1)(x+3)}{\sqrt{1+x^2}}$，则 $f(x)$（　）。

;;;
A. 在 $x=1,x=-3$ 处取得极大值，在 $x=-1$ 处取得极小值
B. 在 $x=-1$ 处取得极大值，在 $x=1,x=-3$ 处取得极小值
C. 在 $x=-1,x=1,x=-3$ 处都取得极小值
D. 在 $x=-1,x=-3,x=1$ 处都取得极大值
;;;B

***

$f'(x)$ 有零点 $x=-3,-1,1$。由左右两侧符号变化：$x=-3$ 处 $f'$ 由负变正（极小），$x=-1$ 处由正变负（极大），$x=1$ 处由负变正（极小），选 **B**。

+++

#### 基础选择 (18) 曲线 $y=\dfrac{1+\mathrm{e}^{-x^2}}{1-\mathrm{e}^{-x^2}}$ 渐近线的条数为（　）。

;;;
A. 0
B. 1
C. 2
D. 3
;;;C

***

$\lim\limits_{x\to\infty}y=1$（水平渐近线 $y=1$），$\lim\limits_{x\to0}y=+\infty$（铅直渐近线 $x=0$），共 **2** 条，选 **C**。

+++

#### 基础选择 (19) 曲线 $y=\mathrm{e}^{\frac{1}{x^2}}\arctan\dfrac{x^2+x+1}{(x-1)(x+2)}$ 的渐近线条数为（　）。

;;;
A. 1
B. 2
C. 3
D. 4
;;;B

***

$\lim\limits_{x\to0}y=-\infty$，知 $x=0$ 是铅直渐近线；$\lim\limits_{x\to\infty}y=\dfrac{\pi}{4}$，知 $y=\dfrac{\pi}{4}$ 是水平渐近线，无斜渐近线，共 **2** 条，选 **B**。

+++

#### 基础选择 (20) 曲线 $y=\sqrt{x^2-a^2}$ 的渐近线的条数为（　）。

;;;
A. 0
B. 1
C. 2
D. 3
;;;C

***

$\lim\limits_{x\to+\infty}\dfrac{y}{x}=1$，$\lim\limits_{x\to+\infty}(\sqrt{x^2-a^2}-x)=0$，故 $y=x$ 是斜渐近线；同理 $\lim\limits_{x\to-\infty}\dfrac{y}{x}=-1$，$\lim\limits_{x\to-\infty}(\sqrt{x^2-a^2}+x)=0$，故 $y=-x$ 也是斜渐近线，共 **2** 条，选 **C**。

+++

#### 基础填空 (1) $f(x)=\begin{cases}\arctan\dfrac1x,&x>0,\\ ax+b,&x\leqslant0\end{cases}$ 在 $x=0$ 处可导，则 $a=\underline{\quad}$，$b=\underline{\quad}$。

***

$a=-1,\ b=\dfrac{\pi}{2}$。

由连续性：$\lim\limits_{x\to0^-}(ax+b)=b$，$\lim\limits_{x\to0^+}\arctan\dfrac1x=\dfrac{\pi}{2}$，故 $b=\dfrac{\pi}{2}$。

$f'_-(0)=a$，$f'_+(0)=\lim\limits_{x\to0^+}\dfrac{\arctan\frac1x-\frac{\pi}{2}}{x}\xlongequal{\text{洛}}\lim\limits_{x\to0^+}\dfrac{-1}{1+x^2}=-1$，由 $f'_-(0)=f'_+(0)$ 得 $a=-1$。

+++

#### 基础填空 (2) 设 $f(x)$ 在 $x=0$ 处可导，且 $f'(0)=2$，$f(0)=0$，则 $\lim\limits_{x\to0}\dfrac{f(1-\cos x)}{\ln(1+x^2)}=\underline{\quad}$。

***

$1$。

$\dfrac{f(1-\cos x)}{\ln(1+x^2)}=\dfrac{x^2}{\ln(1+x^2)}\cdot\dfrac{1-\cos x}{x^2}\cdot\dfrac{f(1-\cos x)-f(0)}{1-\cos x}\to1\cdot\dfrac12\cdot f'(0)=\dfrac12\times2=1.$

+++

#### 基础填空 (3) 设 $y=f(x)$ 由方程 $x=\displaystyle\int_1^{\,y-x}\sin^2\!\left(\dfrac{\pi t}{4}\right)\mathrm{d}t$ 确定，则 $\lim\limits_{n\to\infty}n\left[f\!\left(\dfrac1n\right)-1\right]=\underline{\quad}$。

***

$3$。

两边对 $x$ 求导：$1=(y'-1)\sin^2\!\left[\dfrac{\pi}{4}(y-x)\right]$，即 $y'=\csc^2\!\left[\dfrac{\pi}{4}(y-x)\right]+1$。

当 $x=0$ 时 $y=1$（即 $f(0)=1$），代入得 $y'|_{x=0}=3$。故

$$
\lim\limits_{n\to\infty}n\left[f\!\left(\tfrac1n\right)-1\right]=\lim\limits_{n\to\infty}\dfrac{f(\frac1n)-f(0)}{\frac1n}=f'(0)=3.
$$

+++

#### 基础填空 (4) 设函数 $f(x)$ 有连续导数，且 $\lim\limits_{x\to0}\left[\dfrac{\sin x}{x^2}+\dfrac{f(x)}{x}\right]=2$，则 $f(x)$ 的一阶麦克劳林展开式为 $\underline{\quad}$。

***

$f(x)=-1+2x+o(x)$。

由 $\lim\limits_{x\to0}\dfrac{\sin x+xf(x)}{x^2}=2$，知 $\sin x+xf(x)$ 与 $2x^2$ 等价。又

$$
\sin x+xf(x)=[x+o(x^2)]+x[f(0)+f'(0)x+o(x)]=[1+f(0)]x+f'(0)x^2+o(x^2),
$$

故 $f(0)=-1,\ f'(0)=2$，所以 $f(x)=-1+2x+o(x)$。

+++

#### 基础填空 (5) 设函数 $f(x)$ 在 $(-\infty,+\infty)$ 内连续，$f''(x)$ 的图形如图所示（$f''$ 在 $x_1$ 处左右不变号、在 $x=0$ 与 $x_2$ 处变号，$f''(0)$ 不存在），则曲线 $y=f(x)$ 的拐点个数为 $\underline{\quad}$。

***

$2$。

由 $f''$ 图形知 $f''(x_1)=f''(x_2)=0$、$f''(0)$ 不存在。在 $x=x_1$ 两侧二阶导数不变号，不是拐点；在 $x=0$、$x=x_2$ 两侧变号，故有 **2** 个拐点。

+++

#### 基础填空 (6) 设 $f'(0)$ 存在，$f(0)=0$，且 $\lim\limits_{x\to0}\left[1+\dfrac{1-\cos f(x)}{\sin x}\right]^{\frac1x}=\mathrm{e}$，则 $f'(0)=\underline{\quad}$。

***

$\pm\sqrt2$。

由 $1^\infty$ 型：$\lim\limits_{x\to0}\dfrac{1-\cos f(x)}{x\sin x}=1$。又 $\sin x\sim x$、$1-\cos f(x)\sim\dfrac12 f^2(x)$，且 $f'(0)$ 存在，故

$$
1=\dfrac12\lim\limits_{x\to0}\dfrac{f^2(x)}{x^2}=\dfrac12\left[\lim\limits_{x\to0}\dfrac{f(x)}{x}\right]^2=\dfrac12[f'(0)]^2,
$$

解得 $f'(0)=\pm\sqrt2$。

+++

#### 基础填空 (7) 当 $x\to0$ 时，$x-\sin x\cos x$ 与 $ax^b$ 为等价无穷小，则 $a=\underline{\quad}$，$b=\underline{\quad}$。

***

$a=\dfrac23,\ b=3$。

$x-\sin x\cos x=x-\dfrac12\sin2x=x-\dfrac12\left[2x-\dfrac{(2x)^3}{3!}+o(x^3)\right]=\dfrac23x^3+o(x^3)\sim\dfrac23x^3$，故 $a=\dfrac23,\ b=3$。

+++

#### 基础填空 (8) 当 $x\to0$ 时，$\mathrm{e}^x+\ln(1-x)-1$ 与 $x^n$ 是同阶无穷小，则 $n=\underline{\quad}$。

***

$3$。

$\mathrm{e}^x=1+x+\dfrac12x^2+\dfrac16x^3+o(x^3)$，$\ln(1-x)=-x-\dfrac12x^2-\dfrac13x^3+o(x^3)$，相加减 $1$ 得 $-\dfrac16x^3+o(x^3)$，故 $n=3$。

+++

#### 基础填空 (9) 曲线 $y=\mathrm{e}^{-x^2}$ 的上凸区间是 $\underline{\quad}$。

***

$\left(-\dfrac{\sqrt2}{2},\dfrac{\sqrt2}{2}\right)$。

$y''=2(2x^2-1)\mathrm{e}^{-x^2}$，令 $y''=0$ 得 $x=\pm\dfrac{\sqrt2}{2}$。当 $x\in\left(-\dfrac{\sqrt2}{2},\dfrac{\sqrt2}{2}\right)$ 时 $y''<0$，为上凸（凹向下）区间。

+++

#### 基础填空 (10) 曲线 $y=(2x-1)\mathrm{e}^{\frac1x}$ 的斜渐近线方程为 $\underline{\quad}$。

***

$y=2x+1$。

$k=\lim\limits_{x\to\infty}\dfrac{y}{x}=\lim\limits_{x\to\infty}\dfrac{(2x-1)\mathrm{e}^{1/x}}{x}=2$；
$b=\lim\limits_{x\to\infty}\left[(2x-1)\mathrm{e}^{1/x}-2x\right]=\lim\limits_{x\to\infty}\left[2x(\mathrm{e}^{1/x}-1)-\mathrm{e}^{1/x}\right]=2-1=1$。故 $y=2x+1$。

+++

#### 基础填空 (11) 设 $f(x)=n^2\mathrm{e}^{\frac{x}{n}}-(1+n)x$ 在 $x=x_n$ 处有水平切线，则 $\lim\limits_{n\to\infty}\mathrm{e}^{x_n}=\underline{\quad}$。

***

$\mathrm{e}$。

$f'(x)=n\mathrm{e}^{x/n}-(1+n)=0\Rightarrow x_n=n\ln\!\left(1+\dfrac1n\right)$，故 $\lim\limits_{n\to\infty}\mathrm{e}^{x_n}=\lim\limits_{n\to\infty}\mathrm{e}^{n\ln(1+\frac1n)}=\mathrm{e}$。

+++

#### 基础填空 (12) 设 $y=f(x)$ 由参数方程 $\begin{cases}x=t^2+1,\\ y=4t-t^2\end{cases}(t\geqslant0)$ 确定，则 $\lim\limits_{n\to\infty}n\left[f\!\left(\dfrac{2n+1}{n}\right)-3\right]=\underline{\quad}$。

***

$1$。

当 $x=2$ 时 $t=1,\ y=3$。原式 $=\lim\limits_{n\to\infty}\dfrac{f(2+\frac1n)-f(2)}{\frac1n}=f'(2)$。而 $\dfrac{\mathrm{d}y}{\mathrm{d}x}\Big|_{x=2}=\dfrac{4-2t}{2t}\Big|_{t=1}=1$，故原式 $=1$。

+++

#### 基础填空 (13) 设连续函数 $y=f(x)$ 在点 $(1,0)$ 处满足 $\Delta y=\Delta x+o(\Delta x)$，则 $\lim\limits_{x\to0}\dfrac{\displaystyle\int_1^{\,\mathrm{e}^x}f(t)\,\mathrm{d}t}{x^2+\ln(1+x^3)}=\underline{\quad}$。

***

$\dfrac12$。

由 $\Delta y=\Delta x+o(\Delta x)$ 得 $f'(1)=1$，且 $f(1)=0$；又 $x^2+\ln(1+x^3)\sim x^2\ (x\to0)$。故

$$
\text{原式}=\lim\limits_{x\to0}\dfrac{\int_1^{\mathrm{e}^x}f(t)\mathrm{d}t}{x^2}=\lim\limits_{x\to0}\dfrac{\mathrm{e}^xf(\mathrm{e}^x)}{2x}=\lim\limits_{x\to0}\dfrac{\mathrm{e}^x}{2}\cdot\dfrac{f(\mathrm{e}^x)-f(1)}{\mathrm{e}^x-1}\cdot\dfrac{\mathrm{e}^x-1}{x}=\dfrac12 f'(1)=\dfrac12.
$$

+++

#### 基础填空 (14) 设 $f(x)=x(2x-1)(3x-2)\cdots(100x-99)$，则 $f'(0)=\underline{\quad}$。

***

$-99!$。

记 $u(x)=x$，$v(x)=(2x-1)(3x-2)\cdots(100x-99)$，则 $f=uv$。$u'(0)=1,\ u(0)=0,\ v(0)=(-1)(-2)\cdots(-99)=-99!$，故 $f'(0)=u'(0)v(0)+u(0)v'(0)=-99!$。

+++

#### 基础填空 (15) 设 $\dfrac{\mathrm{d}}{\mathrm{d}x}\left[f(x^3)\right]=\dfrac1x$，则 $f'(x)=\underline{\quad}$。

***

$\dfrac{1}{3x}$。

$\dfrac{\mathrm{d}}{\mathrm{d}x}[f(x^3)]=3x^2 f'(x^3)=\dfrac1x$，得 $f'(x^3)=\dfrac{1}{3x^3}$，所以 $f'(x)=\dfrac{1}{3x}$。

+++

#### 基础填空 (16) 设 $f(x)=\dfrac{x^{10}}{1-x}$，则 $f^{(10)}(x)=\underline{\quad}$。

***

$\dfrac{10!}{(1-x)^{11}}$。

$f(x)=\dfrac{(x^{10}-1)+1}{1-x}=(-x^9-x^8-\cdots-1)+\dfrac{1}{1-x}$，前一部分是 $9$ 次多项式，$10$ 阶导为 $0$，故 $f^{(10)}(x)=\left(\dfrac{1}{1-x}\right)^{(10)}=\dfrac{10!}{(1-x)^{11}}$。

+++

#### 基础填空 (17) 设 $f(x)$ 可导，且 $\lim\limits_{x\to0}\dfrac{f(1)-f(1-x)}{2x}=-1$，则曲线 $y=f(x)$ 在点 $(1,f(1))$ 处的切线斜率为 $\underline{\quad}$。

***

$-2$。

令 $-x=\Delta t$：$\lim\limits_{x\to0}\dfrac{f(1)-f(1-x)}{2x}=\lim\limits_{\Delta t\to0}\dfrac12\cdot\dfrac{f(1+\Delta t)-f(1)}{\Delta t}=\dfrac12 f'(1)=-1$，故 $f'(1)=-2$。

+++

#### 基础填空 (18) 设 $f(x)=\cos|x|+x^2|x|$ 在 $x=0$ 处存在的最高阶导数的阶数为 $\underline{\quad}$。

***

$2$。

在 $x=0$ 邻域内 $\cos|x|=\cos x$（任意阶可导），而 $x^2|x|$ 在 $x=0$ 处二阶可导、三阶不可导，故最高阶数为 $2$。

+++

#### 基础填空 (19) 曲线 $x=a\cos^3 t,\ y=a\sin^3 t\ (a>0)$ 在 $t=\dfrac{\pi}{4}$ 处的曲率 $=\underline{\quad}$。

***

$\dfrac{2}{3a}$。

$y'=\dfrac{\mathrm{d}y}{\mathrm{d}t}\cdot\dfrac{\mathrm{d}t}{\mathrm{d}x}=\dfrac{3a\sin^2 t\cos t}{-3a\cos^2 t\sin t}=-\tan t$；
$y''=\dfrac{\mathrm{d}}{\mathrm{d}x}(-\tan t)=\dfrac{-\sec^2 t}{-3a\cos^2 t\sin t}=\dfrac{1}{3a}\sec^4 t\csc t$。

$$
K=\dfrac{|y''|}{(1+y'^2)^{3/2}}\Big|_{t=\frac{\pi}{4}}=\left|\dfrac{2}{3a\sin 2t}\right|_{t=\frac{\pi}{4}}=\dfrac{2}{3a}.
$$

+++

#### 基础解答 (1) 计算下列函数的导数：(Ⅰ) $y=\dfrac{1}{\sqrt[3]{x\cdot\sqrt[3]{x}}}$；(Ⅱ) $y=x^{a^a}+a^{x^a}+a^{a^x}(a>0)$；(Ⅲ) $y=2^{|\sin x|}$；(Ⅳ) $y=\ln|\tan x+\sec x|$。

***

(Ⅰ) $y=(x\cdot x^{1/3})^{-1/3}=x^{-4/9}$，故 $y'=-\dfrac49 x^{-13/9}$。

(Ⅱ) $y'=a^a x^{a^a-1}+a(\ln a)x^{a-1}\,a^{x^a}+(\ln a)^2\,a^x\,a^{a^x}$。（$x^{a^a}$ 视为幂函数）

(Ⅲ) 由 $|\sin x|=\sqrt{\sin^2 x}$，$y'=2^{|\sin x|}(\ln2)\cdot\sin2x\cdot\dfrac{1}{2|\sin x|}\ (\sin x\neq0)$。

(Ⅳ) $y'=\dfrac{1}{\tan x+\sec x}(\sec^2 x+\sec x\tan x)=\sec x$。

+++

#### 基础解答 (2) 求下列函数的导数：(Ⅰ) $y=(1+x^2)^{\sin x}$；(Ⅱ) $y=\ln\dfrac{1}{\sqrt{x+\sqrt{x^2+1}}}$。

***

(Ⅰ) 取对数 $\ln y=\sin x\ln(1+x^2)$，求导得

$$
y'=(1+x^2)^{\sin x}\left[\ln(1+x^2)\cos x+\dfrac{2x\sin x}{1+x^2}\right].
$$

(Ⅱ) $y=-\dfrac12\ln(x+\sqrt{x^2+1})$，$y'=-\dfrac12\cdot\dfrac{1}{x+\sqrt{x^2+1}}\left(1+\dfrac{x}{\sqrt{x^2+1}}\right)=-\dfrac{1}{2\sqrt{x^2+1}}$。

+++

#### 基础解答 (3) 求下列函数的微分：(Ⅰ) $y=\varphi\!\left(\arctan\dfrac1x\right)$，$\varphi$ 可导，求 $\mathrm{d}y$；(Ⅱ) $y=y(x)$ 由 $\mathrm{e}^{x+y}-y\sin x=0$ 确定，求 $\mathrm{d}y$；(Ⅲ) $y=y(x)$ 由 $\begin{cases}x=2t,\\ y=5t^2+1\end{cases}$ 确定，求 $\mathrm{d}y$。

***

(Ⅰ) $\mathrm{d}y=\varphi'\!\left(\arctan\dfrac1x\right)\cdot\dfrac{1}{1+\frac1{x^2}}\cdot\left(-\dfrac1{x^2}\right)\mathrm{d}x=-\varphi'\!\left(\arctan\dfrac1x\right)\dfrac{1}{1+x^2}\mathrm{d}x$。

(Ⅱ) 微分：$\mathrm{e}^{x+y}(\mathrm{d}x+\mathrm{d}y)-(\sin x\,\mathrm{d}y+y\cos x\,\mathrm{d}x)=0$，解得

$$
\mathrm{d}y=\dfrac{y\cos x-\mathrm{e}^{x+y}}{\mathrm{e}^{x+y}-\sin x}\mathrm{d}x=\dfrac{y(\cos x-\sin x)}{(y-1)\sin x}\mathrm{d}x.
$$

(Ⅲ) $t=\dfrac x2$，$y=\dfrac{5x^2}{4}+1$，故 $\mathrm{d}y=\dfrac52 x\,\mathrm{d}x$。

+++

#### 基础解答 (4) 设 $y=y(x)$ 由方程 $\sqrt{x^2+y^2}=\mathrm{e}^{\arctan\frac yx}$ 确定，求 $\dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}$。

***

两边取对数 $\dfrac12\ln(x^2+y^2)=\arctan\dfrac yx$，求导整理得 $y'=\dfrac{x+y}{x-y}$。

再求导：$y''=\dfrac{2xy'-2y}{(x-y)^2}$，代入 $y'=\dfrac{x+y}{x-y}$ 得

$$
y''=\dfrac{2(x^2+y^2)}{(x-y)^3}.
$$

+++

#### 基础解答 (5) 设 $y=y(x)$ 由参数方程 $\begin{cases}x=t-\sin t,\\ y=1-\cos t\end{cases}$ 确定，求 $\dfrac{\mathrm{d}y}{\mathrm{d}x},\ \dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}$。

***

$\dfrac{\mathrm{d}y}{\mathrm{d}x}=\dfrac{\sin t}{1-\cos t}$。

$\dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}=\dfrac{\mathrm{d}}{\mathrm{d}t}\!\left(\dfrac{\sin t}{1-\cos t}\right)\cdot\dfrac{\mathrm{d}t}{\mathrm{d}x}=\dfrac{-1}{1-\cos t}\cdot\dfrac{1}{1-\cos t}=-\dfrac{1}{(1-\cos t)^2}$。

+++

#### 基础解答 (6) 求心形线 $r=1-\cos\theta$ 在对应于 $\theta=\dfrac{\pi}{2}$ 处的切线方程。

***

化为参数方程 $x=(1-\cos\theta)\cos\theta,\ y=(1-\cos\theta)\sin\theta$。

$\dfrac{\mathrm{d}y}{\mathrm{d}x}\Big|_{\theta=\frac{\pi}{2}}=\dfrac{y'(\theta)}{x'(\theta)}\Big|_{\theta=\frac{\pi}{2}}=-1$，且 $x\!\left(\tfrac{\pi}{2}\right)=0,\ y\!\left(\tfrac{\pi}{2}\right)=1$。

故切线方程 $y-1=-(x-0)$，即 $x+y=1$。

+++

#### 基础解答 (7) 设 $f(x)=\begin{cases}x^k\sin\dfrac1x,&x\neq0,\\ 0,&x=0.\end{cases}$ (Ⅰ) $k$ 为何值时 $f(x)$ 在 $x=0$ 处不可导；(Ⅱ) $k$ 为何值时可导但导函数不连续；(Ⅲ) $k$ 为何值时导函数连续。

***

$\dfrac{f(x)-f(0)}{x}=x^{k-1}\sin\dfrac1x$。

(Ⅰ) 当 $k\leqslant1$ 时，$f'(0)$ 不存在。

(Ⅱ) 当 $k>1$ 时 $f'(0)=0$，且 $x\neq0$ 时 $f'(x)=kx^{k-1}\sin\dfrac1x-x^{k-2}\cos\dfrac1x$。当 $1<k\leqslant2$ 时 $\lim\limits_{x\to0}f'(x)$ 不存在，即可导但导函数不连续。

(Ⅲ) 当 $k>2$ 时 $\lim\limits_{x\to0}f'(x)=0=f'(0)$，导函数连续。

+++

#### 基础解答 (8) 设 $f(x)$ 在 $(0,+\infty)$ 内满足 $f(xy)=f(x)+f(y)$，且 $f'(1)=1$，证明 $f(x)$ 在 $(0,+\infty)$ 内可导，并求 $f(x)$。

***

令 $x=y=1$ 得 $f(1)=0$。由定义

$$
f'(x)=\lim\limits_{\Delta x\to0}\dfrac{f\!\left[x\left(1+\frac{\Delta x}{x}\right)\right]-f(x)}{\Delta x}=\lim\limits_{\Delta x\to0}\dfrac{f\!\left(1+\frac{\Delta x}{x}\right)-f(1)}{\frac{\Delta x}{x}}\cdot\dfrac1x=\dfrac{f'(1)}{x}=\dfrac1x,
$$

故 $f(x)$ 可导。由 $f'(x)=\dfrac1x$ 积分得 $f(x)=\ln x+C$，又 $f(1)=0$ 得 $C=0$，所以 $f(x)=\ln x$。

+++

#### 基础解答 (9) 设 $f(x)=\begin{cases}\mathrm{e}^{-\frac{1}{x^2}},&x\neq0,\\ 0,&x=0,\end{cases}$ 求 $f^{(n)}(0)$。

***

$f'(0)=\lim\limits_{x\to0}\dfrac{\mathrm{e}^{-1/x^2}}{x}=0$。当 $x\neq0$ 时 $f'(x)=\dfrac{2}{x^3}\mathrm{e}^{-1/x^2}$，故 $f''(0)=\lim\limits_{x\to0}\dfrac1x\cdot\dfrac{2}{x^3}\mathrm{e}^{-1/x^2}=0$。同理 $f^{(k)}(0)=0$，所以 $f^{(n)}(0)=0$。

（关键：利用洛必达法则，对任意正整数 $k$，$\lim\limits_{x\to0}\dfrac{\mathrm{e}^{-1/x^2}}{x^k}=0$。）

+++

#### 基础解答 (10) 设气体以 $100\ \mathrm{cm^3/s}$ 的速率注入球状气球，求当半径为 $10\ \mathrm{cm}$ 时，气球半径增加的速率（设气体压力不变）。

***

由 $V=\dfrac43\pi r^3$，两边对 $t$ 求导：$\dfrac{\mathrm{d}V}{\mathrm{d}t}=4\pi r^2\dfrac{\mathrm{d}r}{\mathrm{d}t}$。

代入 $\dfrac{\mathrm{d}V}{\mathrm{d}t}=100,\ r=10$：$100=4\pi\cdot100\cdot\dfrac{\mathrm{d}r}{\mathrm{d}t}$，解得 $\dfrac{\mathrm{d}r}{\mathrm{d}t}=\dfrac{1}{4\pi}\ \mathrm{cm/s}$。

+++

#### 基础解答 (11) 一动点 $P$ 在曲线 $9y=4x^2$ 上运动，已知 $P$ 横坐标变化速率为 $30\ \mathrm{cm/s}$，当 $P$ 经过 $(3,4)$ 时，从原点到 $P$ 的距离 $S$ 变化率为多少？

***

$\dfrac{\mathrm{d}x}{\mathrm{d}t}=30$。由 $9y=4x^2$ 得 $\dfrac{\mathrm{d}y}{\mathrm{d}t}=\dfrac{8x}{9}\dfrac{\mathrm{d}x}{\mathrm{d}t}$，在 $(3,4)$ 处 $\dfrac{\mathrm{d}y}{\mathrm{d}t}=\dfrac{8\cdot3}{9}\cdot30=80$。

$S=\sqrt{x^2+y^2}$，在 $(3,4)$ 处 $S=5$，$\dfrac{\mathrm{d}S}{\mathrm{d}t}=\dfrac{x\frac{\mathrm{d}x}{\mathrm{d}t}+y\frac{\mathrm{d}y}{\mathrm{d}t}}{S}=\dfrac{3\cdot30+4\cdot80}{5}=\dfrac{410}{5}=82\ \mathrm{cm/s}$。

+++

#### 基础解答 (12) 设 $f(x)$ 二阶可导，$f(0)=0$，$f'(0)=1$，$f''(0)=2$，求 $\lim\limits_{x\to0}\dfrac{f(x)-x}{x^2}$。

***

由带皮亚诺余项的泰勒公式 $f(x)=f(0)+f'(0)x+\dfrac{f''(0)}{2}x^2+o(x^2)=x+x^2+o(x^2)$，

故 $\lim\limits_{x\to0}\dfrac{f(x)-x}{x^2}=\lim\limits_{x\to0}\dfrac{x^2+o(x^2)}{x^2}=1$。

+++

#### 基础解答 (13) 证明 $f(x)=\begin{cases}1+x^2,&0\leqslant x\leqslant1,\\ 1-x^2,&-1\leqslant x<0\end{cases}$ 满足拉格朗日中值定理，并求满足定理的 $\xi$ 的值。

***

$f(x)$ 在 $[-1,1]$ 上连续（$x=0$ 处左右极限均为 $1$）；$x\neq0$ 时可导，$x=0$ 处 $f'_+(0)=f'_-(0)=0$，故在 $(-1,1)$ 内可导，满足定理条件。

$f(-1)=0,\ f(1)=2$，$\dfrac{f(1)-f(-1)}{1-(-1)}=1$。令 $f'(\xi)=1$：$\xi>0$ 时 $2\xi=1\Rightarrow\xi=\dfrac12$；$\xi<0$ 时 $-2\xi=1\Rightarrow\xi=-\dfrac12$。故 $\xi=\pm\dfrac12$。

+++

#### 基础解答 (14) 设 $f(x)$ 在 $[a,b]$ 上连续，在 $(a,b)$ 内可导，$0<a<b$，且 $f(a)=f(b)=0$，证明：(Ⅰ) 至少存在一点 $\xi\in(a,b)$，使 $2f(\xi)+\xi f'(\xi)=0$；(Ⅱ) 至少存在一点 $\eta\in(a,b)$，使 $2\eta f(\eta)-f'(\eta)=0$。

***

(Ⅰ) 令 $g(x)=x^2 f(x)$，则 $g(a)=g(b)=0$，由罗尔定理 $\exists\xi$：$g'(\xi)=\xi(2f(\xi)+\xi f'(\xi))=0$，因 $\xi>0$，故 $2f(\xi)+\xi f'(\xi)=0$。

(Ⅱ) 令 $h(x)=\mathrm{e}^{-x^2}f(x)$，则 $h(a)=h(b)=0$，由罗尔定理 $\exists\eta$：$h'(\eta)=\mathrm{e}^{-\eta^2}(f'(\eta)-2\eta f(\eta))=0$，故 $2\eta f(\eta)-f'(\eta)=0$。

+++

#### 基础解答 (15) 设 $f(x)$ 在 $[a,b]$ 上连续，在 $(a,b)$ 内可导，$0<a<b$，且 $f(a)=0$，证明：至少存在一点 $\xi\in(a,b)$，使 $af(\xi)+(\xi-b)f'(\xi)=0$。

***

构造 $g(x)=(x-b)^a f(x)$。则 $g(a)=(a-b)^a f(a)=0$，$g(b)=0\cdot f(b)=0$。

由罗尔定理，$\exists\xi\in(a,b)$：$g'(\xi)=(\xi-b)^{a-1}[af(\xi)+(\xi-b)f'(\xi)]=0$。因 $(\xi-b)^{a-1}\neq0$，故 $af(\xi)+(\xi-b)f'(\xi)=0$。

+++

#### 基础解答 (16) 设 $f(x)$ 在 $[0,+\infty)$ 上连续，在 $(0,+\infty)$ 内可导，且 $f(0)=0$，$\lim\limits_{x\to+\infty}f(x)=0$，证明：至少存在一点 $\xi\in(0,+\infty)$，使 $f'(\xi)=0$。

***

若 $f\equiv0$ 则结论显然。否则存在 $c>0$ 使 $f(c)\neq0$，不妨设 $f(c)>0$。

由 $f(0)=0$ 及 $\lim\limits_{x\to+\infty}f(x)=0$，取充分大 $M>c$ 使 $f(M)<f(c)$，则 $f$ 在 $[0,M]$ 上连续，最大值在内部某点 $\xi\in(0,M)$ 取得（因端点值均小于 $f(c)$），该点为极大值点且 $f$ 可导，故 $f'(\xi)=0$。

+++

#### 基础解答 (17) 设 $f(x)$ 在 $[0,+\infty)$ 上连续，在 $(0,+\infty)$ 内可导，且 $0\leqslant f(x)\leqslant\dfrac{x}{1+x^2}$，证明：至少存在一点 $\xi\in(0,+\infty)$，使 $f'(\xi)=\dfrac{1-\xi^2}{(1+\xi^2)^2}$。

***

令 $g(x)=f(x)-\dfrac{x}{1+x^2}$，注意 $\left(\dfrac{x}{1+x^2}\right)'=\dfrac{1-x^2}{(1+x^2)^2}$。

由条件，$0\leqslant f(0)\leqslant0\Rightarrow f(0)=0$，故 $g(0)=0$；又 $\lim\limits_{x\to+\infty}\dfrac{x}{1+x^2}=0$，由夹逼知 $\lim\limits_{x\to+\infty}f(x)=0$，故 $\lim\limits_{x\to+\infty}g(x)=0$。

对 $g$ 应用上题的推理（$g(0)=0$ 且 $\lim\limits_{x\to+\infty}g(x)=0$），存在 $\xi\in(0,+\infty)$ 使 $g'(\xi)=0$，即 $f'(\xi)=\dfrac{1-\xi^2}{(1+\xi^2)^2}$。

+++

#### 基础解答 (18) 设 $f(x)$ 在 $[0,1]$ 上连续，在 $(0,1)$ 内可导，且 $f''(x)\leqslant0$，$f(0)=0$，证明：对任意 $x_0\in[0,1]$，有 $f(x_0)\leqslant2f\!\left(\dfrac{x_0}{2}\right)$。

***

$f''(x)\leqslant0$ 表明 $f$ 是凹（上凸）函数。由凹性，中点满足

$$
f\!\left(\dfrac{x_0}{2}\right)=f\!\left(\dfrac{x_0+0}{2}\right)\geqslant\dfrac{f(x_0)+f(0)}{2}=\dfrac{f(x_0)}{2},
$$

故 $f(x_0)\leqslant2f\!\left(\dfrac{x_0}{2}\right)$。

+++

#### 基础解答 (19) 设 $f(x)$ 在 $[0,1]$ 上可导，$f(0)=0$，$f(1)=1$，且 $f(x)$ 不恒等于 $x$，证明：存在一点 $\xi\in(0,1)$，使 $f'(\xi)>1$。

***

因 $f(x)$ 不恒等于 $x$，存在 $x_0\in(0,1)$ 使 $f(x_0)\neq x_0$。

若 $f(x_0)>x_0$：在 $[0,x_0]$ 上由拉格朗日定理，$\exists\xi$：$f'(\xi)=\dfrac{f(x_0)-0}{x_0}=\dfrac{f(x_0)}{x_0}>1$。

若 $f(x_0)<x_0$：在 $[x_0,1]$ 上，$\exists\xi$：$f'(\xi)=\dfrac{1-f(x_0)}{1-x_0}>\dfrac{1-x_0}{1-x_0}=1$。

两种情形都存在 $\xi$ 使 $f'(\xi)>1$。

+++

#### 基础解答 (20) 设 $f(x)$ 在 $[0,1]$ 上连续，在 $(0,1)$ 内可导，且 $f(1)-f(0)=\dfrac12$，证明：存在不同的两点 $\xi$ 和 $\eta\in(0,1)$，使 $f'(\xi)+f'(\eta)=1$。

***

在 $\left[0,\dfrac12\right]$ 上由拉格朗日定理，$\exists\xi\in\left(0,\dfrac12\right)$：$f'(\xi)=2\!\left[f\!\left(\tfrac12\right)-f(0)\right]$。

在 $\left[\dfrac12,1\right]$ 上，$\exists\eta\in\left(\dfrac12,1\right)$：$f'(\eta)=2\!\left[f(1)-f\!\left(\tfrac12\right)\right]$。

相加：$f'(\xi)+f'(\eta)=2[f(1)-f(0)]=2\cdot\dfrac12=1$，且 $\xi\neq\eta$。

+++

#### 基础解答 (21) 设 $f(x)$ 在 $[0,1]$ 上二阶可导，$|f''(x)|\leqslant1$，$f(x)$ 在 $(0,1)$ 内取得最小值，证明：$|f'(0)|+|f'(1)|\leqslant1$。

***

设最小值在 $c\in(0,1)$ 取得，则 $f'(c)=0$。由拉格朗日定理：

$$
|f'(0)|=|f'(0)-f'(c)|=|f''(\xi_1)|\cdot c\leqslant c,\quad\xi_1\in(0,c),
$$

$$
|f'(1)|=|f'(1)-f'(c)|=|f''(\xi_2)|\cdot(1-c)\leqslant1-c,\quad\xi_2\in(c,1).
$$

相加得 $|f'(0)|+|f'(1)|\leqslant c+(1-c)=1$。

+++

#### 基础解答 (22) 设 $f(x)$ 在 $[a,b]$ 上连续，在 $(a,b)$ 内可导，$f(a)=f(b)$，且 $f(x)$ 在 $[a,b]$ 上不恒为常数，证明：存在相异的 $\xi,\eta\in(a,b)$，使 $f'(\xi)\cdot f'(\eta)<0$。

***

因不恒为常数，存在 $c\in(a,b)$ 使 $f(c)\neq f(a)$，不妨设 $f(c)>f(a)=f(b)$。

在 $[a,c]$ 上：$f'(\xi)=\dfrac{f(c)-f(a)}{c-a}>0$；在 $[c,b]$ 上：$f'(\eta)=\dfrac{f(b)-f(c)}{b-c}<0$。

故 $f'(\xi)\cdot f'(\eta)<0$，且 $\xi\in(a,c),\eta\in(c,b)$ 相异。

+++

#### 基础解答 (23) 设 $f(x)$ 在 $[0,1]$ 上二阶可导，且 $f(0)=f(1)=2\displaystyle\int_{1/2}^{1}f(x)\,\mathrm{d}x$，证明：(Ⅰ) 至少存在一点 $\xi\in(0,1)$，使 $f''(\xi)=0$；(Ⅱ) 对 $\forall\lambda\in\mathbf{R}$，至少存在一点 $\eta\in(0,1)$，使 $f''(\eta)-\lambda f'(\eta)=0$。

***

由积分中值定理，$2\displaystyle\int_{1/2}^{1}f(x)\mathrm{d}x=2\cdot f(c)\cdot\dfrac12=f(c)$，$c\in\left(\dfrac12,1\right)$。故 $f(0)=f(1)=f(c)$。

(Ⅰ) 在 $[0,c]$ 与 $[c,1]$ 上分别用罗尔定理，得 $x_1\in(0,c),x_2\in(c,1)$ 使 $f'(x_1)=f'(x_2)=0$；再对 $f'$ 在 $[x_1,x_2]$ 用罗尔定理，得 $\xi$ 使 $f''(\xi)=0$。

(Ⅱ) 令 $g(x)=\mathrm{e}^{-\lambda x}f'(x)$，由 $f'(x_1)=f'(x_2)=0$ 得 $g(x_1)=g(x_2)=0$。由罗尔定理 $\exists\eta\in(x_1,x_2)$：$g'(\eta)=\mathrm{e}^{-\lambda\eta}[f''(\eta)-\lambda f'(\eta)]=0$，故 $f''(\eta)-\lambda f'(\eta)=0$。

+++

#### 基础解答 (24) 设 $f(x)$ 在 $[a,b]$ 上连续，在 $(a,b)$ 内可导，$0<a<b$，证明：存在 $\xi,\eta\in(a,b)$，使 $2\eta f'(\xi)=(b+a)f'(\eta)$。

***

由拉格朗日定理，$\exists\xi\in(a,b)$：$f(b)-f(a)=f'(\xi)(b-a)$。

对 $f(x)$ 与 $g(x)=x^2$ 用柯西中值定理，$\exists\eta\in(a,b)$：$\dfrac{f(b)-f(a)}{b^2-a^2}=\dfrac{f'(\eta)}{2\eta}$，即 $f(b)-f(a)=\dfrac{f'(\eta)}{2\eta}(b-a)(b+a)$。

两式相等：$f'(\xi)(b-a)=\dfrac{f'(\eta)}{2\eta}(b+a)(b-a)$，故 $2\eta f'(\xi)=(b+a)f'(\eta)$。

+++

#### 基础解答 (25) 设 $a,b$ 为正数，证明：至少存在一点 $\xi\in(a,b)$，使 $\dfrac{a\mathrm{e}^b-b\mathrm{e}^a}{a-b}=\mathrm{e}^\xi(1-\xi)$。

***

取 $F(x)=\dfrac{\mathrm{e}^x}{x}$，$G(x)=\dfrac1x$。则

$$
\dfrac{F(b)-F(a)}{G(b)-G(a)}=\dfrac{\frac{\mathrm{e}^b}{b}-\frac{\mathrm{e}^a}{a}}{\frac1b-\frac1a}=\dfrac{(a\mathrm{e}^b-b\mathrm{e}^a)/(ab)}{(a-b)/(ab)}=\dfrac{a\mathrm{e}^b-b\mathrm{e}^a}{a-b}.
$$

由柯西中值定理，$\exists\xi\in(a,b)$：上式 $=\dfrac{F'(\xi)}{G'(\xi)}=\dfrac{\mathrm{e}^\xi(\xi-1)/\xi^2}{-1/\xi^2}=\mathrm{e}^\xi(1-\xi)$。

+++

#### 基础解答 (26) 证明下列不等式：(Ⅰ) 当 $0<x<\pi$ 时 $\sin\dfrac x2>\dfrac x\pi$；(Ⅱ) 当 $\mathrm{e}<a<b$ 时 $a^b>b^a$；(Ⅲ) 当 $x>0$ 时 $(x^2-1)\ln x\geqslant(x-1)^2$；(Ⅳ) 若 $\lim\limits_{x\to0}\dfrac{f(x)}{x}=1$ 且 $f''(x)>0$，有 $f(x)\geqslant x$。

***

(Ⅰ) 令 $t=\dfrac x2\in\left(0,\dfrac\pi2\right)$，即证 $\dfrac{\sin t}{t}>\dfrac2\pi$。因 $\dfrac{\sin t}{t}$ 在 $\left(0,\dfrac\pi2\right)$ 上单调减，$\dfrac{\sin t}{t}>\dfrac{\sin(\pi/2)}{\pi/2}=\dfrac2\pi$。

(Ⅱ) 即证 $b\ln a>a\ln b$，即 $\dfrac{\ln a}{a}>\dfrac{\ln b}{b}$。令 $g(x)=\dfrac{\ln x}{x}$，$g'(x)=\dfrac{1-\ln x}{x^2}<0\,(x>\mathrm{e})$，故单调减，$a<b\Rightarrow g(a)>g(b)$。

(Ⅲ) $(x^2-1)\ln x-(x-1)^2=(x-1)[(x+1)\ln x-(x-1)]$。令 $\varphi(x)=(x+1)\ln x-(x-1)$，$\varphi'(x)=\ln x+\dfrac1x$，其最小值在 $x=1$ 处为 $1>0$，故 $\varphi$ 单调增，$\varphi(1)=0$。于是 $x>1$ 时 $\varphi>0$、$x<1$ 时 $\varphi<0$，与 $(x-1)$ 同号，乘积 $\geqslant0$。

(Ⅳ) 由条件 $f(0)=0,f'(0)=1$。$f''>0$ 表明 $f$ 凸，图形在 $x=0$ 处切线之上：$f(x)\geqslant f(0)+f'(0)x=x$。

+++

#### 基础解答 (27) 求函数 $y=(x-1)\mathrm{e}^{\frac\pi2+\arctan x}$ 的单调区间与极值，并求其渐近线。

***

$y'=\mathrm{e}^{\frac\pi2+\arctan x}\left[1+\dfrac{x-1}{1+x^2}\right]=\mathrm{e}^{\frac\pi2+\arctan x}\cdot\dfrac{x(x+1)}{1+x^2}$。

$y'=0$ 于 $x=-1,0$。单调增：$(-\infty,-1)$ 与 $(0,+\infty)$；单调减：$(-1,0)$。

极大值 $y(-1)=-2\mathrm{e}^{\frac\pi4}$，极小值 $y(0)=-\mathrm{e}^{\frac\pi2}$。

渐近线：$x\to+\infty$ 时 $y=\mathrm{e}^\pi(x-2)+o(1)$，斜渐近线 $y=\mathrm{e}^\pi(x-2)$；$x\to-\infty$ 时 $y=(x-2)+o(1)$，斜渐近线 $y=x-2$。

+++

#### 基础解答 (28) 设 $f(x)=\begin{cases}x^{2x},&x>0,\\ x+2,&x\leqslant0,\end{cases}$ 求 $f(x)$ 的单调区间与极值。

***

$x\leqslant0$：$f'=1>0$，单调增。

$x>0$：$f(x)=\mathrm{e}^{2x\ln x}$，$f'(x)=2x^{2x}(\ln x+1)$，$f'=0$ 于 $x=\dfrac1e$。$0<x<\dfrac1e$ 时 $f'<0$；$x>\dfrac1e$ 时 $f'>0$。

单调增区间 $(-\infty,0]$ 与 $\left[\dfrac1e,+\infty\right)$；单调减区间 $\left(0,\dfrac1e\right]$。

极大值 $f(0)=2$（$x\to0^+$ 时 $f\to1<2$，左侧递增至 $2$）；极小值 $f\!\left(\dfrac1e\right)=\mathrm{e}^{-\frac2e}$。

+++

#### 基础解答 (29) 设 $y=y(x)$ 由参数方程 $\begin{cases}x=t\ln t,\\ y=\dfrac1t\ln t\end{cases}(t\geqslant1)$ 确定，求单调区间、凹凸区间、极值和拐点。

***

$\dfrac{\mathrm{d}x}{\mathrm{d}t}=\ln t+1>0$，$\dfrac{\mathrm{d}y}{\mathrm{d}t}=\dfrac{1-\ln t}{t^2}$，故 $\dfrac{\mathrm{d}y}{\mathrm{d}x}=\dfrac{1-\ln t}{t^2(\ln t+1)}$。

**单调 / 极值**：$1\leqslant t<\mathrm{e}$ 时 $y'>0$，$t>\mathrm{e}$ 时 $y'<0$。因 $x$ 随 $t$ 增，单调增区间 $x\in[0,\mathrm{e})$、单调减区间 $x\in(\mathrm{e},+\infty)$。极大值在 $t=\mathrm{e}$：$x=\mathrm{e},\ y=\dfrac1{\mathrm{e}}$。

**凹凸 / 拐点**：$\dfrac{\mathrm{d}^2y}{\mathrm{d}x^2}=\dfrac{2t(\ln^2 t-2)}{t^4(\ln t+1)^3}$，符号同 $\ln^2 t-2$。$1<t<\mathrm{e}^{\sqrt2}$ 时 $<0$（上凸），$t>\mathrm{e}^{\sqrt2}$ 时 $>0$（下凸）。拐点在 $t=\mathrm{e}^{\sqrt2}$：$\left(\sqrt2\,\mathrm{e}^{\sqrt2},\ \sqrt2\,\mathrm{e}^{-\sqrt2}\right)$。

+++

#### 基础解答 (30) 求曲线 $y=\sqrt{4x^2+x}\,\ln\!\left(2+\dfrac1x\right)$ 的全部渐近线。

***

**铅直渐近线**：$x\to-\dfrac12^{-}$ 时 $2+\dfrac1x\to0^+$，$\ln\to-\infty$，而 $\sqrt{4x^2+x}\to\sqrt{\tfrac12}$，故 $y\to-\infty$，得 $x=-\dfrac12$。（$x\to0^+$ 时 $\sqrt{4x^2+x}\sim\sqrt x\to0$、$\ln\!\left(2+\frac1x\right)\sim-\ln x$，乘积 $\to0$，无铅直渐近线。）

**斜渐近线**：$x\to+\infty$，$\sqrt{4x^2+x}=2x+\dfrac14+o(1)$，$\ln\!\left(2+\frac1x\right)=\ln2+\dfrac1{2x}+o$，得 $y=2(\ln2)x+1+\dfrac{\ln2}{4}+o(1)$，即 $y=2(\ln2)x+1+\dfrac{\ln2}{4}$。

$x\to-\infty$，$\sqrt{4x^2+x}=-2x-\dfrac14+o(1)$，得 $y=-2(\ln2)x-1-\dfrac{\ln2}{4}$。

+++

#### 基础解答 (31) 对数曲线 $y=\ln x$ 上哪一点的曲率半径最小？求出该点的曲率半径。

***

$y'=\dfrac1x,\ y''=-\dfrac1{x^2}$，曲率半径 $R=\dfrac{(1+y'^2)^{3/2}}{|y''|}=\dfrac{(x^2+1)^{3/2}}{x}$。

令 $t=x^2$，$R^2=\dfrac{(t+1)^3}{t}$，$\dfrac{\mathrm{d}}{\mathrm{d}t}R^2=\dfrac{(t+1)^2(2t-1)}{t^2}=0\Rightarrow t=\dfrac12$，即 $x=\dfrac{\sqrt2}{2}$。

此时点为 $\left(\dfrac{\sqrt2}{2},-\dfrac12\ln2\right)$，最小曲率半径 $R=\dfrac{(3/2)^{3/2}}{\sqrt{1/2}}=\dfrac{3\sqrt3}{2}$。

+++

#### 基础解答 (32) 证明：方程 $2^x-x^2-1=0$ 有且仅有三个不同实根。

***

令 $g(x)=2^x-x^2-1$。显然 $g(0)=0,\ g(1)=0$ 是两个根。又 $g(2)=-1<0,\ g(5)=6>0$，在 $(4,5)$ 内还有一根。

$g''(x)=2^x(\ln2)^2-2$ 只有一个零点，故 $g'$ 先减后增、至多两个零点，从而 $g$ 至多有三个实根。结合上面已找到的三个根，故恰有三个不同实根。

+++

#### 基础解答 (33) 证明：方程 $\ln x=\dfrac x{\mathrm{e}}-\displaystyle\int_0^\pi\sqrt{1-\cos2x}\,\mathrm{d}x$ 在 $(0,+\infty)$ 内有且仅有两个不同实根。

***

先算积分：$\displaystyle\int_0^\pi\sqrt{1-\cos2x}\,\mathrm{d}x=\int_0^\pi\sqrt2\,|\sin x|\,\mathrm{d}x=2\sqrt2$。

令 $g(x)=\dfrac x{\mathrm{e}}-\ln x-2\sqrt2$。$g'(x)=\dfrac1{\mathrm{e}}-\dfrac1x=0\Rightarrow x=\mathrm{e}$，$g''(x)=\dfrac1{x^2}>0$，故 $x=\mathrm{e}$ 为全局最小值点，$g(\mathrm{e})=1-1-2\sqrt2=-2\sqrt2<0$。

又 $x\to0^+$ 与 $x\to+\infty$ 时 $g\to+\infty$，故 $g$ 恰有两个零点，即原方程有且仅有两个实根。

+++

#### 基础解答 (34) 讨论曲线 $y=4\ln x+k$ 与 $y=4x+\ln^4 x$ 交点的个数。

***

交点满足 $4\ln x+k=4x+\ln^4 x$，即 $k=\varphi(x)=4x+\ln^4 x-4\ln x\ (x>0)$。

$\varphi'(x)=4+\dfrac{4\ln^3 x-4}{x}=4+\dfrac{4(\ln^3 x-1)}{x}$。令 $\varphi'(x)=0$ 得唯一驻点 $x=1$，且 $\varphi(1)=4$ 为全局最小值（$x\to0^+$ 及 $x\to+\infty$ 时 $\varphi\to+\infty$）。

故：$k<4$ 时无交点；$k=4$ 时有 $1$ 个交点；$k>4$ 时有 $2$ 个交点。

+++

#### 综合选择 (1) 设 $f(x)$ 在 $(1-\delta,1+\delta)\,(\delta>0)$ 内存在导数，$f'(x)$ 严格单调减少，且 $f(1)=f'(1)=1$，则（　）。

;;;
A. 在 $(1-\delta,1)$ 和 $(1,1+\delta)$ 内，均有 $f(x)<x$
B. 在 $(1-\delta,1)$ 和 $(1,1+\delta)$ 内，均有 $f(x)>x$
C. 在 $(1-\delta,1)$ 内 $f(x)<x$；在 $(1,1+\delta)$ 内 $f(x)>x$
D. 在 $(1-\delta,1)$ 内 $f(x)>x$；在 $(1,1+\delta)$ 内 $f(x)<x$
;;;A

***

在 $x=1$ 处的切线为 $y=f(1)+f'(1)(x-1)=x$。因 $f'(x)$ 严格单调减少，$f(x)$ 为凹函数（上凸），曲线在切线**下方**，故 $x\neq1$ 附近均有 $f(x)<x$，选 **A**。

+++

#### 综合选择 (2) 设 $f(x)$ 在 $[0,+\infty)$ 上二阶可导，$f(0)=0$，$f''(x)<0$，当 $0<a<x<b$ 时，有（　）。

;;;
A. $af(x)>xf(a)$
B. $bf(x)>xf(b)$
C. $xf(x)>bf(b)$
D. $xf(x)>af(a)$
;;;B

***

令 $g(x)=\dfrac{f(x)}{x}$，$g'(x)=\dfrac{xf'(x)-f(x)}{x^2}$。记 $h(x)=xf'(x)-f(x)$，$h'(x)=xf''(x)<0$，$h(0)=0$，故 $h(x)<0$，$g'(x)<0$，即 $\dfrac{f(x)}{x}$ 单调减。由 $x<b$ 得 $\dfrac{f(x)}{x}>\dfrac{f(b)}{b}$，即 $bf(x)>xf(b)$，选 **B**。

+++

#### 综合选择 (3) 设 $f(x)$ 在 $[a,b]$ 上可导，$f(x)$ 在 $x=a$ 处取得最小值，在 $x=b$ 处取得最大值，则（　）。

;;;
A. $f'_+(a)<0$ 且 $f'_-(b)<0$
B. $f'_+(a)>0$ 且 $f'_-(b)<0$
C. $f'_+(a)\geqslant0$ 且 $f'_-(b)\geqslant0$
D. $f'_+(a)<0$ 且 $f'_-(b)>0$
;;;C

***

$a$ 为左端点最小值，故 $f'_+(a)=\lim\limits_{x\to a^+}\dfrac{f(x)-f(a)}{x-a}\geqslant0$；$b$ 为右端点最大值，故 $f'_-(b)=\lim\limits_{x\to b^-}\dfrac{f(x)-f(b)}{x-b}\geqslant0$，选 **C**。

+++

#### 综合选择 (4) 设 $f(x)$ 在 $[0,1]$ 上有二阶导数，且 $f(0)=f(1)$，$f''(x)\neq0$，则下列选项正确的是（　）。

;;;
A. 至少存在一点 $\xi\in(0,1)$，使得 $f(\xi)=0$
B. 在 $(0,1)$ 内，$f'(x)\neq0$
C. 存在唯一一点 $\xi\in(0,1)$，使得 $f'(\xi)=0$
D. 至少存在不同两点 $\xi_1,\xi_2\in(0,1)$，使得 $f'(\xi_1)=f'(\xi_2)=0$
;;;C

***

由 $f(0)=f(1)$ 及罗尔定理，$\exists\xi$ 使 $f'(\xi)=0$。又 $f''(x)\neq0$（保号）表明 $f'(x)$ 严格单调，故零点唯一，选 **C**。

+++

#### 综合选择 (5) 设 $f(x)$ 在 $x=0$ 的某邻域内有定义，则 $F(x)=f(x)|\sin x|$ 在 $x=0$ 处可导的充要条件是（　）。

;;;
A. $\lim\limits_{x\to0}f(x)$ 存在
B. $\lim\limits_{x\to0}f(x)=f(0)$
C. $f(x)$ 在 $x=0$ 处可导
D. $\lim\limits_{x\to0^-}f(x)$ 与 $\lim\limits_{x\to0^+}f(x)$ 均存在，且 $\lim\limits_{x\to0^-}f(x)=-\lim\limits_{x\to0^+}f(x)$
;;;D

***

$F(0)=0$。$F'_+(0)=\lim\limits_{x\to0^+}f(x)\dfrac{|\sin x|}{x}=\lim\limits_{x\to0^+}f(x)$；$F'_-(0)=\lim\limits_{x\to0^-}f(x)\dfrac{|\sin x|}{x}=-\lim\limits_{x\to0^-}f(x)$。

可导 $\Leftrightarrow F'_+(0)=F'_-(0)\Leftrightarrow\lim\limits_{x\to0^+}f(x)=-\lim\limits_{x\to0^-}f(x)$（均存在），选 **D**。

+++

#### 综合选择 (6) 设 $y=f(x)$ 在 $x_0$ 的某邻域内有四阶连续导数，且 $f'(x_0)=f''(x_0)=f'''(x_0)=0$，且 $f^{(4)}(x_0)<0$，则（　）。

;;;
A. $f(x)$ 在 $x_0$ 处取得极小值
B. $f(x)$ 在 $x_0$ 处取得极大值
C. $(x_0,f(x_0))$ 是 $y=f(x)$ 的拐点
D. $f(x)$ 在 $x_0$ 的某邻域内单调减少
;;;B

***

第一个非零导数为偶数阶（$4$ 阶）且 $f^{(4)}(x_0)<0$，故 $x_0$ 为极大值点，选 **B**。

+++

#### 综合选择 (7) 设 $f(x)$ 在 $x_0$ 的某邻域内连续，且 $\lim\limits_{x\to x_0}\dfrac{f(x)-f(x_0)}{(x-x_0)^n}=1$，则（　）。

;;;
A. 当 $n$ 为奇数时，$x_0$ 是 $f(x)$ 的极大值点
B. 当 $n$ 为奇数时，$x_0$ 是 $f(x)$ 的极小值点
C. 当 $n$ 为偶数时，$x_0$ 是 $f(x)$ 的极小值点
D. 当 $n$ 为偶数时，$x_0$ 是 $f(x)$ 的极大值点
;;;C

***

极限为 $1>0$，故 $x_0$ 附近 $f(x)-f(x_0)$ 与 $(x-x_0)^n$ 同号。$n$ 为偶数时 $(x-x_0)^n>0$，故 $f(x)>f(x_0)$，$x_0$ 为极小值点，选 **C**。（$n$ 奇数时两侧变号，非极值。）

+++

#### 综合选择 (8) 设 $f(x)$ 在 $(-\infty,+\infty)$ 内可导，则下列命题正确的是（　）。

;;;
A. 若 $\lim\limits_{x\to-\infty}f(x)=-\infty$，则必有 $\lim\limits_{x\to-\infty}f'(x)=-\infty$
B. 若 $\lim\limits_{x\to-\infty}f'(x)=-\infty$，则必有 $\lim\limits_{x\to-\infty}f(x)=-\infty$
C. 若 $\lim\limits_{x\to+\infty}f(x)=+\infty$，则必有 $\lim\limits_{x\to+\infty}f'(x)=+\infty$
D. 若 $\lim\limits_{x\to+\infty}f'(x)=+\infty$，则必有 $\lim\limits_{x\to+\infty}f(x)=+\infty$
;;;D

***

若 $\lim\limits_{x\to+\infty}f'(x)=+\infty$，则存在 $X$，当 $x>X$ 时 $f'(x)>1$，由拉格朗日 $f(x)-f(X)=f'(c)(x-X)>x-X\to+\infty$，故 $f(x)\to+\infty$，选 **D**。（A、C 反例：$f\to\infty$ 不能推出 $f'\to\infty$；B 中 $f'\to-\infty$ 反而使 $f(x)\to+\infty$。）

+++

#### 综合选择 (9) 设 $k>0$，方程 $\ln x-\dfrac x{\mathrm{e}}+k=0$ 在 $(0,+\infty)$ 内不同实根的个数为（　）。

;;;
A. 0
B. 1
C. 2
D. 3
;;;C

***

令 $g(x)=\ln x-\dfrac x{\mathrm{e}}+k$，$g'(x)=\dfrac1x-\dfrac1{\mathrm{e}}=0\Rightarrow x=\mathrm{e}$，$g(\mathrm{e})=k>0$ 为最大值。又两端 $g\to-\infty$，故有 **2** 个根，选 **C**。

+++

#### 综合选择 (10) 设当 $x\neq0$ 时，方程 $kx+\dfrac1{x^2}=1$ 有且只有一个实根，则（　）。

;;;
A. $|k|>\dfrac29\sqrt3$
B. $|k|<\dfrac29\sqrt3$
C. $k=\dfrac29\sqrt3$
D. $k=-\dfrac29\sqrt3$
;;;A

***

即 $k=\dfrac1x-\dfrac1{x^3}=\varphi(x)$（奇函数）。$\varphi'(x)=\dfrac{3-x^2}{x^4}=0\Rightarrow x=\pm\sqrt3$，正半轴极大值 $\varphi(\sqrt3)=\dfrac{2\sqrt3}{9}$。分析 $k=\varphi(x)$ 解的总数，仅当 $|k|>\dfrac{2\sqrt3}{9}$ 时恰有一个实根，选 **A**。

+++

#### 综合选择 (11) 设 $f(x)$ 在 $[0,+\infty)$ 上二阶可导，$f(0)=0$，$f'(0)<0$，$f''(x)\geqslant M>0$，则方程 $f(x)=0$ 在 $(0,+\infty)$ 内不同实根的个数为（　）。

;;;
A. 3
B. 2
C. 1
D. 0
;;;C

***

$f'(x)\geqslant f'(0)+Mx$ 单调增趋于 $+\infty$。$f'(0)<0$ 使 $f$ 先减（由 $0$ 变负），后因 $f''\geqslant M$ 呈二次增长趋于 $+\infty$，故仅回升穿过零点一次，恰 **1** 个实根，选 **C**。

+++

#### 综合选择 (12) 设可导函数 $f(x)$，$x\in[0,1]$ 满足 $f'(x)\geqslant M>0$，且 $f\!\left(\dfrac12\right)\geqslant0$，则在区间（　）上有 $f(x)\geqslant\dfrac14M$。

;;;
A. $\left[0,\dfrac14\right]$
B. $\left[\dfrac14,\dfrac12\right]$
C. $\left[\dfrac12,\dfrac34\right]$
D. $\left[\dfrac34,1\right]$
;;;D

***

由拉格朗日，$x\geqslant\dfrac12$ 时 $f(x)\geqslant f\!\left(\tfrac12\right)+M\!\left(x-\tfrac12\right)\geqslant M\!\left(x-\tfrac12\right)$。当 $x\in\left[\dfrac34,1\right]$ 时 $x-\dfrac12\geqslant\dfrac14$，故 $f(x)\geqslant\dfrac14M$，选 **D**。

+++

#### 综合选择 (13) 设函数 $f_1(x),f_2(x)$ 有二阶连续导数，且 $f_1''(x)>0$，$f_2''(x)>0$，若曲线 $y=f_1(x)$ 与 $y=f_2(x)$ 在点 $(x_0,y_0)$ 处有公切线 $y=g(x)$，且在该点处曲线 $y=f_1(x)$ 的曲率半径小于 $y=f_2(x)$ 的曲率半径，则在点 $x_0$ 的某邻域内有（　）。

;;;
A. $g(x)\geqslant f_2(x)\geqslant f_1(x)$
B. $g(x)\geqslant f_1(x)\geqslant f_2(x)$
C. $f_1(x)\geqslant f_2(x)\geqslant g(x)$
D. $f_1(x)\geqslant g(x)\geqslant f_2(x)$
;;;C

***

公切线处两曲线的 $f'$ 相同，曲率 $=\dfrac{|f''|}{(1+f'^2)^{3/2}}$。曲率半径小 $\Rightarrow$ 曲率大 $\Rightarrow f_1''(x_0)>f_2''(x_0)>0$。两条凸曲线均在公切线 $g$ 上方，$f''$ 越大离切线越高，故 $f_1(x)\geqslant f_2(x)\geqslant g(x)$，选 **C**。

+++

#### 综合填空 (1) 设函数 $f(x)=\left[\tan\!\left(\dfrac\pi4 x\right)-1\right]\left[\tan\!\left(\dfrac\pi4 x^2\right)-2\right]\cdots\left[\tan\!\left(\dfrac\pi4 x^{100}\right)-100\right]$，则 $f'(1)=\underline{\quad}$。

***

$-\dfrac{99!}{2}\pi$。

$x=1$ 时仅第一个因子 $\tan\dfrac\pi4-1=0$，故求导只保留对该因子求导的项：

$$
f'(1)=\left[\tan\!\left(\tfrac\pi4 x\right)-1\right]'\Big|_{x=1}\cdot\prod_{k=2}^{100}(1-k)=\dfrac\pi4\cdot\dfrac{1}{\cos^2\frac\pi4}\cdot(-99!)=\dfrac\pi2\cdot(-99!)=-\dfrac{99!}{2}\pi.
$$

+++

#### 综合填空 (2) 设 $f(x)=3x^2+kx^{-3}$，若对任意 $x\in(0,+\infty)$ 都有 $f(x)\geqslant20$，则 $k$ 至少为 $\underline{\quad}$。

***

$64$。

$f'(x)=6x-3kx^{-4}=0\Rightarrow x=\sqrt[5]{\dfrac k2}$，$f''>0$ 为最小值点，最小值 $f\!\left(\sqrt[5]{\tfrac k2}\right)=5\left(\dfrac k2\right)^{2/5}$。

由 $5\left(\dfrac k2\right)^{2/5}\geqslant20$ 解得 $k\geqslant64$。

+++

#### 综合填空 (3) 函数 $y=\mathrm{e}^{-x}\left(1+x+\dfrac{x^2}{2!}+\cdots+\dfrac{x^n}{n!}\right)$（$n$ 为正奇数）的极大值为 $\underline{\quad}$。

***

$1$。

$y'=\mathrm{e}^{-x}\left[\left(1+\cdots+\dfrac{x^{n-1}}{(n-1)!}\right)-\left(1+\cdots+\dfrac{x^n}{n!}\right)\right]=-\dfrac{x^n}{n!}\mathrm{e}^{-x}$。

$n$ 奇：$x<0$ 时 $y'>0$，$x>0$ 时 $y'<0$，故 $x=0$ 为极大值点，极大值 $y(0)=1$。

+++

#### 综合填空 (4) 已知 $f(x)$ 在 $(-\infty,+\infty)$ 内可导，且 $\lim\limits_{x\to\infty}f'(x)=\mathrm{e}$，$\lim\limits_{x\to\infty}\left(\dfrac{x+k}{x-k}\right)^x=\lim\limits_{x\to\infty}[f(x)-f(x-1)]$，则 $k=\underline{\quad}$。

***

$\dfrac12$。

左边 $\lim\limits_{x\to\infty}\left(\dfrac{x+k}{x-k}\right)^x=\mathrm{e}^{2k}$；右边由拉格朗日 $f(x)-f(x-1)=f'(\xi)\to\mathrm{e}$。故 $\mathrm{e}^{2k}=\mathrm{e}$，$k=\dfrac12$。

+++

#### 综合填空 (5) 设 $y=f(x)$ 在 $(-\infty,\infty)$ 上连续，其导函数 $f'(x)$ 的图形如图 2-2 所示，其中 $x=0$ 和 $x=x_5$ 是 $f'(x)$ 的铅直渐近线，则 $y=f(x)$ 极值点的个数为 $\underline{\quad}$，拐点的个数为 $\underline{\quad}$。

***

极值点 $4$ 个，拐点 $3$ 个。

由图知 $f'(x_1)=f'(x_3)=f'(x_4)=f'(x_6)=0$（驻点），$f'(0)$、$f'(x_5)$ 不存在。可能极值点为 $x_1,x_3,x_4,x_6,0,x_5$；其中在 $x_1,x_3,0,x_4$ 两侧 $f'(x)$ 均变号，故有 **4** 个极值点。

又 $f''(x_2)=f''(x_6)=0$，$f''(0)$、$f''(x_5)$ 不存在；在 $x_2,x_6,x_5$ 两侧 $f''$ 变号，故有 **3** 个拐点。

+++

#### 综合填空 (6) 设 $f(x)$ 在 $x=x_0$ 处可导，且 $f(x_0)\neq0$，则 $\lim\limits_{x\to\infty}\left[\dfrac{f\!\left(x_0+\frac1x\right)}{f(x_0)}\right]^x=\underline{\quad}$。

***

$\mathrm{e}^{\frac{f'(x_0)}{f(x_0)}}$。

$1^\infty$ 型：指数 $\lim\limits_{x\to\infty}x\left[\dfrac{f(x_0+\frac1x)-f(x_0)}{f(x_0)}\right]=\dfrac{1}{f(x_0)}\lim\limits_{x\to\infty}\dfrac{f(x_0+\frac1x)-f(x_0)}{\frac1x}=\dfrac{f'(x_0)}{f(x_0)}$，故原极限 $=\mathrm{e}^{\frac{f'(x_0)}{f(x_0)}}$。

+++

#### 综合填空 (7) 设 $y=f(x)$ 在 $x_0$ 处有三阶连续导数，$f'(x_0)=1$，$f''(x_0)=2$，$f'''(x_0)=3$，$f(x)$ 有反函数 $x=g(y)$，且 $y_0=f(x_0)$，则 $g'''(y_0)=\underline{\quad}$。

***

$9$。

由反函数求导：$g'=\dfrac{1}{f'}$，$g''=-\dfrac{f''}{(f')^3}$，$g'''=-\dfrac{f'''(f')^3-3(f')^2(f'')^2}{(f')^7}$。

代入 $f'=1,f''=2,f'''=3$：$g'''(y_0)=-\dfrac{3\cdot1-3\cdot1\cdot4}{1}=-(3-12)=9$。

+++

#### 综合解答 (1) 设 $f(x)=\begin{cases}ax^2+b\sin x+c,&x\leqslant0,\\ \ln(1+x),&x>0,\end{cases}$ 问 $a,b,c$ 为何值时，$f(x)$ 在 $x=0$ 处一阶导数连续，但二阶导数不存在？

***

**连续**：$\lim\limits_{x\to0^-}f=c$，$\lim\limits_{x\to0^+}f=0$，$f(0)=c$，故 $c=0$。

**一阶导数**：$f'_+(0)=\lim\limits_{x\to0^+}\dfrac{\ln(1+x)}{x}=1$，$f'_-(0)=\lim\limits_{x\to0^-}\dfrac{ax^2+b\sin x}{x}=b$，故 $b=1$。此时

$$
f'(x)=\begin{cases}2ax+\cos x,&x<0,\\ 1,&x=0,\\ \dfrac{1}{1+x},&x>0,\end{cases}
$$

在 $x=0$ 处连续。

**二阶导数**：$f''_+(0)=\lim\limits_{x\to0^+}\dfrac{\frac{1}{1+x}-1}{x}=-1$，$f''_-(0)=\lim\limits_{x\to0^-}\dfrac{2ax+\cos x-1}{x}=2a$。

故当 $b=1,\ c=0$ 且 $a\neq-\dfrac12$ 时，$f'$ 连续而 $f''(0)$ 不存在。

+++

#### 综合解答 (2) 设 $z=f[\varphi(x)+y^2]$，其中 $x,y$ 满足 $y+\mathrm{e}^y=x$，$f,\varphi$ 均具有二阶导数，求 $\dfrac{\mathrm{d}z}{\mathrm{d}x},\ \dfrac{\mathrm{d}^2z}{\mathrm{d}x^2}$。

***

由 $y+\mathrm{e}^y=x$ 求导：$y'=\dfrac{1}{1+\mathrm{e}^y}$，$y''=-\dfrac{\mathrm{e}^y}{(1+\mathrm{e}^y)^3}$。

$$
\dfrac{\mathrm{d}z}{\mathrm{d}x}=f'[\varphi(x)+y^2]\left[\varphi'(x)+\dfrac{2y}{1+\mathrm{e}^y}\right],
$$

$$
\dfrac{\mathrm{d}^2z}{\mathrm{d}x^2}=f''[\varphi+y^2]\left[\varphi'+\dfrac{2y}{1+\mathrm{e}^y}\right]^2+f'[\varphi+y^2]\left[\varphi''+\dfrac{2}{(1+\mathrm{e}^y)^2}-\dfrac{2y\mathrm{e}^y}{(1+\mathrm{e}^y)^3}\right].
$$

+++

#### 综合解答 (3) 已知 $f(x)$ 是周期为 $5$ 的连续函数，在 $x=1$ 的某邻域内满足 $f(1+\sin x)-3f(1-\sin x)=8x+\alpha(x)$，其中 $\alpha(x)$ 是 $x\to0$ 时比 $x$ 高阶的无穷小，且 $f(x)$ 在 $x=1$ 处可导，求曲线 $y=f(x)$ 在点 $(6,f(6))$ 处的切线方程。

***

令 $x\to0$：$f(1)-3f(1)=0\Rightarrow f(1)=0$。

再除以 $\sin x$ 取极限：

$$
\lim\limits_{x\to0}\left[\dfrac{f(1+\sin x)-f(1)}{\sin x}+3\cdot\dfrac{f(1-\sin x)-f(1)}{-\sin x}\right]=8,
$$

即 $f'(1)+3f'(1)=8$，故 $f'(1)=2$。

由周期 $5$：$f(6)=f(1)=0$，$f'(6)=f'(1)=2$。切线方程 $y-0=2(x-6)$，即 $2x-y-12=0$。

+++

#### 综合解答 (4) 设 $f(x)=nx(1-x)^n$（$n$ 为正整数），求 $f(x)$ 在 $[0,1]$ 上的最大值 $M(n)$ 及 $\lim\limits_{n\to\infty}M(n)$。

***

$f'(x)=n(1-x)^{n-1}[1-(n+1)x]$，令 $f'=0$ 得 $x_0=\dfrac{1}{n+1}$。

$0<x<x_0$ 时 $f'>0$，$x_0<x<1$ 时 $f'<0$，故 $x_0$ 为极大值点。又 $f(0)=f(1)=0$，所以

$$
M(n)=f(x_0)=\dfrac{n}{n+1}\left(1-\dfrac{1}{n+1}\right)^n=\left(\dfrac{n}{n+1}\right)^{n+1}.
$$

$$
\lim\limits_{n\to\infty}M(n)=\lim\limits_{n\to\infty}\left(\dfrac{n}{n+1}\right)^{n+1}=\mathrm{e}^{-1}.
$$

+++

#### 综合解答 (5) 设 $f(x)=\begin{cases}|x|^p\sin\dfrac1x,&x\neq0,\\ 0,&x=0.\end{cases}$ (Ⅰ) $p$ 为何值时 $f(x)$ 在 $x=0$ 处连续；(Ⅱ) $p$ 为何值时 $f(x)$ 在 $x=0$ 处可导；(Ⅲ) $p$ 为何值时 $f'(x)$ 在 $x=0$ 处连续。

***

(Ⅰ) $p\leqslant0$ 时 $\lim\limits_{x\to0}|x|^p\sin\dfrac1x$ 不存在，$x=0$ 为间断点；$p>0$ 时极限为 $0=f(0)$，故 **$p>0$ 时连续**。

(Ⅱ) $\dfrac{f(x)-f(0)}{x}=\pm|x|^{p-1}\sin\dfrac1x$，当 $p>1$ 时极限为 $0$，故 **$p>1$ 时可导**且 $f'(0)=0$。

(Ⅲ) $x\neq0$ 时 $f'(x)=p|x|^{p-1}\mathrm{sgn}(x)\sin\dfrac1x-|x|^{p-2}\cos\dfrac1x$。当 $p>2$ 时 $\lim\limits_{x\to0}f'(x)=0=f'(0)$，故 **$p>2$ 时 $f'$ 连续**。

+++

#### 综合解答 (6) 设 $f(x)$ 在 $[0,1]$ 上二阶可导，且 $\lim\limits_{x\to0^+}\dfrac{f(x)}{x}=\lim\limits_{x\to1^-}\dfrac{f(x)}{x-1}=1$，证明：(Ⅰ) 至少存在一点 $\xi\in(0,1)$，使 $f(\xi)=0$；(Ⅱ) 至少存在一点 $\eta\in(0,1)$，使 $f''(\eta)=f(\eta)$。

***

由条件得 $f(0)=0,\ f'_+(0)=1$；$f(1)=0,\ f'_-(1)=1$。

(Ⅰ) 由 $f'_+(0)=1>0$，在 $0$ 右侧有 $f(x)>0$；由 $f'_-(1)=1>0$，在 $1$ 左侧有 $f(x)<0$。由介值定理，$\exists\xi\in(0,1)$ 使 $f(\xi)=0$。

(Ⅱ) 在 $[0,\xi]$ 上 $f$ 有正的最大值，取于内点 $c_1$：$f'(c_1)=0,\ f''(c_1)\leqslant0,\ f(c_1)>0$，故 $f''(c_1)-f(c_1)<0$。
在 $[\xi,1]$ 上 $f$ 有负的最小值，取于内点 $c_2$：$f'(c_2)=0,\ f''(c_2)\geqslant0,\ f(c_2)<0$，故 $f''(c_2)-f(c_2)>0$。

令 $\phi(x)=[f'(x)+f(x)]\mathrm{e}^{-x}$，则 $\phi'(x)=[f''(x)-f(x)]\mathrm{e}^{-x}$，且 $\phi'(c_1)<0<\phi'(c_2)$。由导函数的介值性（达布定理），$\exists\eta$ 介于 $c_1,c_2$ 之间使 $\phi'(\eta)=0$，即 $f''(\eta)=f(\eta)$。

+++

#### 综合解答 (7) 设 $f(x)$ 与 $g(x)$ 在 $[a,b]$ 上连续，在 $(a,b)$ 内可导，且 $f(a)=g(b)=0$，证明：至少存在一点 $\xi\in(a,b)$，使 $f'(\xi)\displaystyle\int_\xi^b g(t)\mathrm{d}t+g'(\xi)\int_a^\xi f(t)\mathrm{d}t=0$。

***

令 $A(x)=\displaystyle\int_a^x f(t)\mathrm{d}t$，$B(x)=\int_x^b g(t)\mathrm{d}t$，构造

$$
\Phi(x)=f(x)B(x)+g(x)A(x).
$$

则 $\Phi'(x)=f'(x)B(x)-f(x)g(x)+g'(x)A(x)+g(x)f(x)=f'(x)B(x)+g'(x)A(x)$。

而 $\Phi(a)=f(a)B(a)+g(a)\cdot0=0$（因 $f(a)=0$），$\Phi(b)=f(b)\cdot0+g(b)A(b)=0$（因 $g(b)=0$）。

由罗尔定理，$\exists\xi\in(a,b)$ 使 $\Phi'(\xi)=0$，即所证等式成立。

+++

#### 综合解答 (8) 在 $x=0$ 的右邻域内，用多项式 $\mathrm{e}+ax+bx^2$ 近似表示函数 $f(x)=(1+x)^{\frac1x}$，使其误差是比 $x^2$ 高阶的无穷小 $(x\to0^+)$，求 $a,b$ 的值。

***

$(1+x)^{1/x}=\mathrm{e}^{\frac{\ln(1+x)}{x}}$，而 $\dfrac{\ln(1+x)}{x}=1-\dfrac x2+\dfrac{x^2}{3}+o(x^2)$，故

$$
f(x)=\mathrm{e}\cdot\mathrm{e}^{-\frac x2+\frac{x^2}{3}+o(x^2)}=\mathrm{e}\left[1+\left(-\dfrac x2+\dfrac{x^2}{3}\right)+\dfrac12\cdot\dfrac{x^2}{4}+o(x^2)\right]=\mathrm{e}-\dfrac{\mathrm{e}}{2}x+\dfrac{11\mathrm{e}}{24}x^2+o(x^2).
$$

故 $a=-\dfrac{\mathrm{e}}{2},\quad b=\dfrac{11\mathrm{e}}{24}$。

+++

#### 综合解答 (9) 设 $f(x)$ 在 $[a,b]$ 上可导，证明：(Ⅰ) 若 $f'_+(a)f'_-(b)<0$，则存在 $\xi\in(a,b)$，使 $f'(\xi)=0$；(Ⅱ) 若 $f'_+(a)\neq f'_-(b)$，则对介于 $f'_+(a)$ 和 $f'_-(b)$ 之间的每个实数 $\mu$，都存在 $\xi\in(a,b)$，使 $f'(\xi)=\mu$。

***

(Ⅰ) 不妨设 $f'_+(a)>0>f'_-(b)$。由 $f'_+(a)>0$，在 $a$ 右侧有 $f(x)>f(a)$；由 $f'_-(b)<0$，在 $b$ 左侧有 $f(x)>f(b)$。故 $f$ 在 $[a,b]$ 上的最大值必在内点 $\xi$ 取得，由费马定理 $f'(\xi)=0$。

(Ⅱ) 令 $g(x)=f(x)-\mu x$，则 $g'_+(a)=f'_+(a)-\mu$ 与 $g'_-(b)=f'_-(b)-\mu$ 异号，由 (Ⅰ) 存在 $\xi$ 使 $g'(\xi)=0$，即 $f'(\xi)=\mu$。（此即导函数的达布介值定理。）

+++

#### 综合解答 (10) 设函数 $f(x)$ 在 $[a,b]$ 上有二阶导数，且 $f(a)=f(b)=0$，$f'_+(a)f'_-(b)>0$，证明：在 $(a,b)$ 内存在两点 $\xi$ 与 $\eta$，使 $f(\xi)=0$，$f''(\eta)=0$。

***

不妨设 $f'_+(a)>0,\ f'_-(b)>0$。

由 $f(a)=0,f'_+(a)>0$，在 $a$ 右侧 $f(x)>0$；由 $f(b)=0,f'_-(b)>0$，在 $b$ 左侧 $f(x)<0$。由介值定理 $\exists\xi\in(a,b)$：$f(\xi)=0$。

于是 $f(a)=f(\xi)=f(b)=0$，两次用罗尔定理得 $c_1\in(a,\xi),c_2\in(\xi,b)$ 使 $f'(c_1)=f'(c_2)=0$；再对 $f'$ 在 $[c_1,c_2]$ 上用罗尔定理，得 $\eta$ 使 $f''(\eta)=0$。

+++

#### 综合解答 (11) 设 $f(x)$ 在 $[0,+\infty)$ 上有二阶导数，$f(0)=0$，$f'_+(0)<0$，$f''(x)\geqslant M>0\ (x>0)$，证明：$f(x)=0$ 在 $(0,+\infty)$ 内有唯一实根。

***

因 $f''\geqslant M>0$，$f'$ 严格单调增且 $f'(x)\geqslant f'_+(0)+Mx\to+\infty$，故存在唯一 $x_0>0$ 使 $f'(x_0)=0$。

于是 $f$ 在 $(0,x_0)$ 上单调减、在 $(x_0,+\infty)$ 上单调增，$x_0$ 为全局最小点，$f(x_0)<f(0)=0$。

在 $(0,x_0]$ 上 $f(x)<0$ 无根；在 $(x_0,+\infty)$ 上 $f$ 严格增且 $f(x)\geqslant f(x_0)+\dfrac M2(x-x_0)^2\to+\infty$，故恰有一个零点。综上，唯一实根。

+++

#### 综合解答 (12) 设 $f(x)$ 在 $[0,1]$ 上连续，在 $(0,1)$ 内可导，$f(x)\neq0$，且 $\lim\limits_{x\to0^-}\dfrac{f(x+1)}{x}$ 存在，证明：(Ⅰ) 存在 $\xi\in(0,1)$，使 $\dfrac{1-\mathrm{e}}{\mathrm{e}\int_0^1 f(t)\mathrm{d}t}=-\dfrac{1}{\mathrm{e}^\xi f(\xi)}$；(Ⅱ) 存在 $\eta\in(0,1)$，使 $\mathrm{e}\displaystyle\int_0^1 f(t)\mathrm{d}t=(\mathrm{e}-1)\mathrm{e}^\xi(\xi-1)f'(\eta)$。

***

由极限存在且分母 $\to0$，得 $f(1)=0$。

(Ⅰ) 对 $F(x)=\displaystyle\int_0^x f(t)\mathrm{d}t$ 与 $G(x)=\mathrm{e}^{-x}$ 用柯西中值定理：

$$
\dfrac{F(1)-F(0)}{G(1)-G(0)}=\dfrac{f(\xi)}{-\mathrm{e}^{-\xi}}\Rightarrow\dfrac{\int_0^1 f}{\mathrm{e}^{-1}-1}=-\mathrm{e}^\xi f(\xi).
$$

整理即 $\dfrac{1-\mathrm{e}}{\mathrm{e}\int_0^1 f(t)\mathrm{d}t}=-\dfrac{1}{\mathrm{e}^\xi f(\xi)}$。

(Ⅱ) 由 (Ⅰ) 得 $\mathrm{e}\displaystyle\int_0^1 f=(\mathrm{e}-1)\mathrm{e}^\xi f(\xi)$。又 $f(1)=0$，在 $[\xi,1]$ 上用拉格朗日定理：$-f(\xi)=f'(\eta)(1-\xi)$，即 $f(\xi)=(\xi-1)f'(\eta)$。代入即得结论。

+++

#### 综合解答 (13) 设 $f(x)$ 在 $[0,1]$ 上具有二阶导数，且 $|f(x)|\leqslant a$，$|f''(x)|\leqslant b$（$a,b$ 为非负常数），$c$ 是 $(0,1)$ 内任一点。(Ⅰ) 写出 $f(x)$ 在 $x=c$ 处带拉格朗日余项的一阶泰勒公式；(Ⅱ) 证明 $|f'(c)|\leqslant2a+\dfrac b2$。

***

(Ⅰ) $f(x)=f(c)+f'(c)(x-c)+\dfrac{f''(\xi)}{2}(x-c)^2$，$\xi$ 介于 $x$ 与 $c$ 之间。

(Ⅱ) 分别取 $x=0$ 与 $x=1$：

$$
f(0)=f(c)-f'(c)c+\dfrac{f''(\xi_1)}{2}c^2,\qquad f(1)=f(c)+f'(c)(1-c)+\dfrac{f''(\xi_2)}{2}(1-c)^2.
$$

相减得 $f(1)-f(0)=f'(c)+\dfrac12\left[f''(\xi_2)(1-c)^2-f''(\xi_1)c^2\right]$，故

$$
|f'(c)|\leqslant|f(1)|+|f(0)|+\dfrac b2\left[(1-c)^2+c^2\right]\leqslant2a+\dfrac b2,
$$

其中用到 $c\in[0,1]$ 时 $(1-c)^2+c^2\leqslant1$。

+++

#### 综合解答 (14) 证明下列结论：(Ⅰ) 设 $f(x)=\displaystyle\int_0^x\dfrac{\mathrm{d}t}{1+t^2}+\int_0^{1/x}\dfrac{\mathrm{d}t}{1+t^2}\ (x>0)$，则 $f(x)=\dfrac\pi2$；(Ⅱ) 当 $x\geqslant1$ 时，$\arctan x-\dfrac12\arccos\dfrac{2x}{1+x^2}=\dfrac\pi4$。

***

(Ⅰ) $f'(x)=\dfrac{1}{1+x^2}+\dfrac{1}{1+\frac1{x^2}}\cdot\left(-\dfrac1{x^2}\right)=\dfrac{1}{1+x^2}-\dfrac{1}{1+x^2}=0$，故 $f$ 为常数。取 $x=1$：$f(1)=2\displaystyle\int_0^1\dfrac{\mathrm{d}t}{1+t^2}=2\cdot\dfrac\pi4=\dfrac\pi2$。

(Ⅱ) 令 $g(x)=\arctan x-\dfrac12\arccos u,\ u=\dfrac{2x}{1+x^2}$。则 $u'=\dfrac{2(1-x^2)}{(1+x^2)^2}$，$\sqrt{1-u^2}=\dfrac{x^2-1}{1+x^2}\ (x\geqslant1)$，故 $(\arccos u)'=-\dfrac{u'}{\sqrt{1-u^2}}=\dfrac{2}{1+x^2}$。

于是 $g'(x)=\dfrac{1}{1+x^2}-\dfrac12\cdot\dfrac{2}{1+x^2}=0$，$g$ 为常数。取 $x=1$：$g(1)=\dfrac\pi4-\dfrac12\arccos1=\dfrac\pi4$。

+++

#### 综合解答 (15) 设函数 $f(x)$ 有二阶连续导数，且 $(x-1)f''(x)=1-\mathrm{e}^{1-x}+2(x-1)f'(x)$，证明：当 $x=x_0$ 是 $f(x)$ 的极值点时，$f(x)$ 在 $x_0$ 处取得极小值。

***

设 $x_0$ 为极值点，则 $f'(x_0)=0$，代入方程得 $(x_0-1)f''(x_0)=1-\mathrm{e}^{1-x_0}$。

注意 $1-\mathrm{e}^{1-x}$ 与 $x-1$ **同号**：$x>1$ 时二者皆正，$x<1$ 时二者皆负。

- 若 $x_0\neq1$：两边同除 $(x_0-1)$ 得 $f''(x_0)=\dfrac{1-\mathrm{e}^{1-x_0}}{x_0-1}>0$。
- 若 $x_0=1$：由 $f''$ 连续及 $\lim\limits_{x\to1}\dfrac{1-\mathrm{e}^{1-x}}{x-1}=1$，得 $f''(1)=1+2f'(1)=1>0$。

两种情形均有 $f''(x_0)>0$，故 $f(x)$ 在 $x_0$ 处取得**极小值**。

+++

#### 综合解答 (16) 求椭圆 $x^2-xy+y^2=3$ 上纵坐标最大和最小的点。

***

两边对 $x$ 求导：$2x-y-xy'+2yy'=0$，得 $y'=\dfrac{y-2x}{2y-x}$。

令 $y'=0$ 得 $y=2x$，代入原方程：$x^2-2x^2+4x^2=3\Rightarrow3x^2=3\Rightarrow x=\pm1$。

故纵坐标最大的点为 $(1,2)$（$y_{\max}=2$），最小的点为 $(-1,-2)$（$y_{\min}=-2$）。

+++

#### 综合解答 (17) 设曲线 $y=\dfrac{1}{\sqrt x}$ 的一条切线与 $x$ 轴和 $y$ 轴围成一个平面图形 $D$。(Ⅰ) 记切点横坐标为 $a$，求切线方程和图形 $D$ 的面积；(Ⅱ) 当切点沿曲线趋于无穷远时，该面积的变化趋势如何？

***

(Ⅰ) $y=x^{-1/2}$，$y'=-\dfrac12x^{-3/2}$。切点 $\left(a,a^{-1/2}\right)$ 处切线：

$$
y=-\dfrac{1}{2}a^{-3/2}x+\dfrac32 a^{-1/2}.
$$

截距：$x$ 轴 $x=3a$，$y$ 轴 $y=\dfrac32a^{-1/2}$。故

$$
S(a)=\dfrac12\cdot3a\cdot\dfrac{3}{2\sqrt a}=\dfrac94\sqrt a.
$$

(Ⅱ) $a\to+\infty$ 时 $S(a)=\dfrac94\sqrt a\to+\infty$，即面积**单调增加且无界**。

+++

#### 综合解答 (18) 设 $f(x)=\arctan x$，求 $f^{(n)}(0)$。

***

$f'(x)=\dfrac{1}{1+x^2}=\sum_{k=0}^{\infty}(-1)^kx^{2k}$，积分得 $\arctan x=\sum_{k=0}^{\infty}\dfrac{(-1)^k}{2k+1}x^{2k+1}$。

比较泰勒系数 $\dfrac{f^{(n)}(0)}{n!}$：

- $n$ 为偶数时，$f^{(n)}(0)=0$；
- $n$ 为奇数时，令 $n=2k+1$，$f^{(n)}(0)=(2k+1)!\cdot\dfrac{(-1)^k}{2k+1}=(-1)^k(2k)!=(-1)^{\frac{n-1}{2}}(n-1)!$。

+++

#### 综合解答 (19) 设 $f(x)=a_1\sin x+a_2\sin2x+\cdots+a_n\sin nx$，$a_i$ 为实数，$n$ 为正整数。(Ⅰ) 求 $f'(0)$；(Ⅱ) 若 $|f(x)|\leqslant|\sin x|$，证明 $|a_1+2a_2+\cdots+na_n|\leqslant1$。

***

(Ⅰ) $f'(x)=\sum_{k=1}^{n}ka_k\cos kx$，故 $f'(0)=a_1+2a_2+\cdots+na_n$。

(Ⅱ) 因 $f(0)=0$，

$$
|f'(0)|=\lim\limits_{x\to0}\left|\dfrac{f(x)-f(0)}{x}\right|=\lim\limits_{x\to0}\dfrac{|f(x)|}{|x|}\leqslant\lim\limits_{x\to0}\dfrac{|\sin x|}{|x|}=1,
$$

即 $|a_1+2a_2+\cdots+na_n|\leqslant1$。

+++

#### 综合解答 (20) 已知 $f(x)$ 可导，证明：曲线 $y=f(x)\ (f(x)>0)$ 与曲线 $y=f(x)\sin x$ 在交点处相切。

***

交点满足 $f(x)=f(x)\sin x$，因 $f(x)>0$，得 $\sin x=1$，即 $x_0=\dfrac\pi2+2k\pi$，此时 $\cos x_0=0$，两曲线纵坐标相同。

斜率：$y_1'=f'(x)$；$y_2'=f'(x)\sin x+f(x)\cos x$。在 $x_0$ 处 $y_2'(x_0)=f'(x_0)\cdot1+f(x_0)\cdot0=f'(x_0)=y_1'(x_0)$。

即交点处纵坐标与切线斜率均相同，故两曲线相切。

+++

#### 综合解答 (21) 确定 $k$ 的取值，使方程 $x^3+2x^2+x=k$ 有 $3$ 个不同实根。

***

令 $\varphi(x)=x^3+2x^2+x$，$\varphi'(x)=3x^2+4x+1=(3x+1)(x+1)$，驻点 $x=-1,\ x=-\dfrac13$。

$\varphi(-1)=0$ 为极大值，$\varphi\!\left(-\dfrac13\right)=-\dfrac{4}{27}$ 为极小值，且 $x\to\pm\infty$ 时 $\varphi\to\pm\infty$。

水平线 $y=k$ 与曲线有 $3$ 个交点的条件为 $-\dfrac{4}{27}<k<0$。

+++

#### 综合解答 (22) 设 $R=R(x)$ 是抛物线 $y=\sqrt x$ 上任一点 $M(x,y)\ (x\geqslant1)$ 处的曲率半径，$s=s(x)$ 是该抛物线上介于点 $A(1,1)$ 与 $M$ 之间的弧长，计算 $3R\dfrac{\mathrm{d}^2R}{\mathrm{d}s^2}-\left(\dfrac{\mathrm{d}R}{\mathrm{d}s}\right)^2$ 的值。

***

$y'=\dfrac{1}{2\sqrt x},\ y''=-\dfrac{1}{4}x^{-3/2}$，$1+y'^2=\dfrac{4x+1}{4x}$，故

$$
R=\dfrac{(1+y'^2)^{3/2}}{|y''|}=\dfrac{(4x+1)^{3/2}}{2}.
$$

$\dfrac{\mathrm{d}s}{\mathrm{d}x}=\sqrt{1+y'^2}=\dfrac{\sqrt{4x+1}}{2\sqrt x}$，$\dfrac{\mathrm{d}R}{\mathrm{d}x}=3\sqrt{4x+1}$，故

$$
\dfrac{\mathrm{d}R}{\mathrm{d}s}=3\sqrt{4x+1}\cdot\dfrac{2\sqrt x}{\sqrt{4x+1}}=6\sqrt x,\qquad \dfrac{\mathrm{d}^2R}{\mathrm{d}s^2}=\dfrac{3/\sqrt x}{\frac{\sqrt{4x+1}}{2\sqrt x}}=\dfrac{6}{\sqrt{4x+1}}.
$$

于是

$$
3R\dfrac{\mathrm{d}^2R}{\mathrm{d}s^2}-\left(\dfrac{\mathrm{d}R}{\mathrm{d}s}\right)^2=3\cdot\dfrac{(4x+1)^{3/2}}{2}\cdot\dfrac{6}{\sqrt{4x+1}}-36x=9(4x+1)-36x=\boxed{9}.
$$

+++

#### 综合解答 (23) 已知 $f(x)$ 在 $[0,+\infty)$ 上有二阶连续导数，$f(0)=f'(0)=0$，且 $x\in[0,+\infty)$ 时 $f''(x)>0$，设 $F(x)$ 是曲线 $y=f(x)$ 上任一点 $(x,f(x))$ 处的切线在 $x$ 轴的截距 $(x>0)$，求 $\lim\limits_{x\to0^+}[F(x)+F'(x)]$。

***

切线 $Y-f(x)=f'(x)(X-x)$，令 $Y=0$ 得 $F(x)=x-\dfrac{f(x)}{f'(x)}$。

当 $x\to0^+$：$f(x)\sim\dfrac{f''(0)}{2}x^2$，$f'(x)\sim f''(0)x$，故 $\dfrac{f(x)}{f'(x)}\sim\dfrac x2$，得 $F(x)\to0$。

$F'(x)=1-\dfrac{f'^2(x)-f(x)f''(x)}{f'^2(x)}=\dfrac{f(x)f''(x)}{f'^2(x)}\to\dfrac{\frac{f''(0)}{2}x^2\cdot f''(0)}{[f''(0)]^2x^2}=\dfrac12$。

故 $\lim\limits_{x\to0^+}[F(x)+F'(x)]=0+\dfrac12=\dfrac12$。

+++

#### 拓展解答 (1) 设 $f(x)$ 有二阶连续导数，$f(0)=f'(0)=0$，$f''(0)>0$，$u=u(x)$ 是曲线 $y=f(x)$ 在点 $(x,f(x))$ 处的切线在 $x$ 轴上的截距，求 $\lim\limits_{x\to0}\dfrac{x}{u(x)}$。

***

$u(x)=x-\dfrac{f(x)}{f'(x)}$。

由泰勒展开 $f(x)=\dfrac{f''(0)}{2}x^2+o(x^2)$，$f'(x)=f''(0)x+o(x)$，故 $\dfrac{f(x)}{f'(x)}=\dfrac x2+o(x)$，从而 $u(x)=\dfrac x2+o(x)$。

$$
\lim\limits_{x\to0}\dfrac{x}{u(x)}=\lim\limits_{x\to0}\dfrac{x}{\frac x2+o(x)}=2.
$$

+++

#### 拓展解答 (2) 设 $f(x)$ 在 $[a,b]$ 上有二阶连续导数，且 $f(a)=f(b)=0$，$M=\max\limits_{a\leqslant x\leqslant b}|f''(x)|$。(Ⅰ) 证明 $\max\limits_{a\leqslant x\leqslant b}|f(x)|\leqslant\dfrac18M(b-a)^2$；(Ⅱ) 证明 $\max\limits_{a\leqslant x\leqslant b}|f'(x)|\leqslant\dfrac12M(b-a)$。

***

(Ⅰ) 由 $f(a)=f(b)=0$ 及拉格朗日插值余项公式，对任意 $x\in[a,b]$ 存在 $\xi$ 使

$$
f(x)=\dfrac{f''(\xi)}{2}(x-a)(x-b)\Rightarrow|f(x)|\leqslant\dfrac M2(x-a)(b-x).
$$

又 $(x-a)(b-x)\leqslant\left(\dfrac{b-a}{2}\right)^2$，故 $|f(x)|\leqslant\dfrac18M(b-a)^2$。

(Ⅱ) 对任意 $x\in[a,b]$，在 $x$ 处作带拉格朗日余项的泰勒公式并取 $a,b$：

$$
0=f(a)=f(x)+f'(x)(a-x)+\dfrac{f''(\xi_1)}{2}(a-x)^2,
$$

$$
0=f(b)=f(x)+f'(x)(b-x)+\dfrac{f''(\xi_2)}{2}(b-x)^2.
$$

相减得 $f'(x)(b-a)=-\dfrac12\left[f''(\xi_2)(b-x)^2-f''(\xi_1)(x-a)^2\right]$，故

$$
|f'(x)|(b-a)\leqslant\dfrac M2\left[(b-x)^2+(x-a)^2\right]\leqslant\dfrac M2(b-a)^2,
$$

即 $|f'(x)|\leqslant\dfrac12M(b-a)$。
