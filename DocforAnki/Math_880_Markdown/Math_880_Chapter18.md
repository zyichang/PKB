---
quizify:
  format: 1
  deck: Math_880::Chapter_18
  tags: [Math, 880题, 数一, 第十八章, 多维随机变量及其分布]
---

+++

#### 基础选择 (1) 设二维随机变量 $(X,Y)$ 的分布函数为 $F(x,y)$，则 $P\{X>x_0,Y>y_0\}=$（　）．

;;;
A. $1+F(x_0,y_0)-F(x_0,+\infty)-F(+\infty,y_0)$
B. $F(x_0,y_0)-1+F(x_0,+\infty)+F(+\infty,y_0)$
C. $1-F(x_0,+\infty)-F(+\infty,y_0)$
D. $1-F(x_0,y_0)$
;;;A
***
记 $A=\{X\leqslant x_0\}$，$B=\{Y\leqslant y_0\}$，由分布函数的定义，知

$$F(x_0,y_0)=P\{X\leqslant x_0,Y\leqslant y_0\},$$

故

$$P\{X>x_0,Y>y_0\}=P(\overline{A}\,\overline{B})=P(\overline{A\cup B})=1-P(A\cup B)$$

$$=1-P(A)-P(B)+P(AB)$$

$$=1-P\{X\leqslant x_0\}-P\{Y\leqslant y_0\}+P\{X\leqslant x_0,Y\leqslant y_0\}$$

$$=1-F(x_0,+\infty)-F(+\infty,y_0)+F(x_0,y_0).$$

+++

#### 基础选择 (2) 设两个相互独立的随机变量 $X$ 与 $Y$ 分别服从 $N(0,1)$ 与 $N(1,1)$，则（　）．

;;;
A. $P\{X+Y\leqslant 1\}=\dfrac{1}{2}$
B. $P\{X+Y\leqslant 0\}=\dfrac{1}{2}$
C. $P\{X-Y\leqslant 1\}=\dfrac{1}{2}$
D. $P\{X-Y\leqslant 0\}=\dfrac{1}{2}$
;;;A
***
由 $X,Y$ 相互独立，$X\sim N(0,1)$，$Y\sim N(1,1)$，知

$$X+Y\sim N(0+1,1+1)=N(1,2),$$

所以 $X+Y$ 的概率密度曲线关于 $\mu=1$ 对称，故 $P\{X+Y\leqslant 1\}=\dfrac{1}{2}$．

【注】设 $X_1\sim N(\mu_1,\sigma_1^2)$，$X_2\sim N(\mu_2,\sigma_2^2)$，且 $X_1$ 与 $X_2$ 相互独立，则

$$aX_1+bX_2\sim N\left(a\mu_1+b\mu_2,(a\sigma_1)^2+(b\sigma_2)^2\right),$$

其中 $a,b$ 为不全为零的实数．

+++

#### 基础填空 (1) 设二维随机变量 $(X,Y)$ 的分布律为下表，且事件 $\{X=0\}$ 与 $\{X+Y=1\}$ 相互独立，则 $a=$ ________，$b=$ ________．

| $Y\,\backslash\,X$ | $0$ | $1$ |
| --- | --- | --- |
| $0$ | $\dfrac{1}{4}$ | $a$ |
| $1$ | $b$ | $\dfrac{1}{4}$ |
***
$\dfrac{1}{4}$，$\dfrac{1}{4}$．

由已知，得

$$P\{X=0\}=P\{X=0,Y=0\}+P\{X=0,Y=1\}=\frac{1}{4}+b,$$

$$P\{X+Y=1\}=P\{X=1,Y=0\}+P\{X=0,Y=1\}=a+b.$$

又 $a+b+\dfrac{1}{4}+\dfrac{1}{4}=a+b+\dfrac{1}{2}=1$，知 $a+b=\dfrac{1}{2}$，于是

$$P\{X=0,X+Y=1\}=P\{X=0,Y=1\}=b.$$

因为 $\{X=0\}$ 与 $\{X+Y=1\}$ 相互独立，所以

$$P\{X=0,X+Y=1\}=P\{X=0\}\cdot P\{X+Y=1\},$$

即 $b=\left(\dfrac{1}{4}+b\right)\cdot\dfrac{1}{2}$，得 $b=\dfrac{1}{4}$，$a=\dfrac{1}{4}$．

+++

#### 基础填空 (2) 设 $X$ 与 $Y$ 相互独立且均服从参数为 $\lambda$ 的指数分布，则 $Z=\min\{X,Y\}$ 的分布函数 $F_Z(z)=$ ________．
***
$$F_Z(z)=\begin{cases}1-\mathrm{e}^{-2\lambda z},&z>0,\\0,&z\leqslant 0.\end{cases}$$

依题设，$X$ 与 $Y$ 的分布函数均为

$$F(x)=\begin{cases}1-\mathrm{e}^{-\lambda x},&x>0,\\0,&x\leqslant 0.\end{cases}$$

$$F_Z(z)=P\{\min\{X,Y\}\leqslant z\}=1-P\{\min\{X,Y\}>z\}$$

$$=1-P\{X>z,Y>z\}=1-P\{X>z\}\cdot P\{Y>z\}$$

$$=1-\left[1-F(z)\right]^2=\begin{cases}1-\mathrm{e}^{-2\lambda z},&z>0,\\0,&z\leqslant 0,\end{cases}$$

可见 $\min\{X,Y\}$ 服从参数为 $2\lambda$ 的指数分布．

+++

#### 基础填空 (3) 设随机变量 $X,Y$ 均服从区间为 $[0,4]$ 的均匀分布，$P\{\max\{X,Y\}\leqslant 3\}=\dfrac{9}{16}$，则 $P\{\min\{X,Y\}>3\}=$ ________．
***
$\dfrac{1}{16}$．

依题设，$X,Y$ 的概率密度均为

$$f(x)=\begin{cases}\dfrac{1}{4},&0\leqslant x\leqslant 4,\\0,&\text{其他},\end{cases}$$

故 $P\{X>3\}=P\{Y>3\}=\dfrac{1}{4}$．

$$P\{(X>3)\cup(Y>3)\}=1-P\{X\leqslant 3,Y\leqslant 3\}=1-P\{\max\{X,Y\}\leqslant 3\}=1-\frac{9}{16}=\frac{7}{16},$$

所以

$$P\{\min\{X,Y\}>3\}=P\{X>3,Y>3\}$$

$$=P\{X>3\}+P\{Y>3\}-P\{(X>3)\cup(Y>3)\}$$

$$=\frac{1}{4}+\frac{1}{4}-\frac{7}{16}=\frac{1}{16}.$$

+++

#### 基础填空 (4) 设随机变量 $X$ 与 $Y$ 相互独立，$X$ 服从参数为 $\lambda=1$ 的指数分布，$Y$ 服从参数为 $0.6$ 的 $0-1$ 分布，则 $P\{X+Y\geqslant 1.6\}=$ ________．
***
$0.4\mathrm{e}^{-1.6}+0.6\mathrm{e}^{-0.6}$．

应用全概率公式，有

$$P\{X+Y\geqslant 1.6\}$$

$$=P\{Y=0\}\cdot P\{X+Y\geqslant 1.6\mid Y=0\}+P\{Y=1\}\cdot P\{X+Y\geqslant 1.6\mid Y=1\}$$

$$=0.4P\{X\geqslant 1.6\mid Y=0\}+0.6P\{X\geqslant 0.6\mid Y=1\}.$$

由于 $X$ 与 $Y$ 相互独立，故

$$P\{X\geqslant 1.6\mid Y=0\}=P\{X\geqslant 1.6\}=1-P\{X<1.6\}=\mathrm{e}^{-1.6}.$$

同理，可得 $P\{X\geqslant 0.6\mid Y=1\}=\mathrm{e}^{-0.6}$，故

$$P\{X+Y\geqslant 1.6\}=0.4\mathrm{e}^{-1.6}+0.6\mathrm{e}^{-0.6}.$$

+++

#### 基础解答 (1) 设二维随机变量 $(X,Y)$ 的联合分布律为下表．（Ⅰ）求 $2X+Y,\max\{X,Y\},\min\{X,Y\}$ 的分布律；（Ⅱ）求 $P\{\min\{X,Y\}\geqslant 0\}$；（Ⅲ）问 $X$ 与 $Y$ 是否相互独立？说明理由．

| $Y\,\backslash\,X$ | $0$ | $1$ |
| --- | --- | --- |
| $-1$ | $\dfrac{3}{16}$ | $\dfrac{9}{16}$ |
| $1$ | $\dfrac{1}{16}$ | $\dfrac{3}{16}$ |
***
（Ⅰ）随机变量取值情况如下：

| $(X,Y)$ | $(0,-1)$ | $(0,1)$ | $(1,-1)$ | $(1,1)$ |
| --- | --- | --- | --- | --- |
| $p_{ij}$ | $\dfrac{3}{16}$ | $\dfrac{1}{16}$ | $\dfrac{9}{16}$ | $\dfrac{3}{16}$ |
| $2X+Y$ | $-1$ | $1$ | $1$ | $3$ |
| $\max\{X,Y\}$ | $0$ | $1$ | $1$ | $1$ |
| $\min\{X,Y\}$ | $-1$ | $0$ | $-1$ | $1$ |

故

| $2X+Y$ | $-1$ | $1$ | $3$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{3}{16}$ | $\dfrac{5}{8}$ | $\dfrac{3}{16}$ |

| $\max\{X,Y\}$ | $0$ | $1$ |
| --- | --- | --- |
| $p$ | $\dfrac{3}{16}$ | $\dfrac{13}{16}$ |

| $\min\{X,Y\}$ | $-1$ | $0$ | $1$ |
| --- | --- | --- | --- |
| $p$ | $\dfrac{3}{4}$ | $\dfrac{1}{16}$ | $\dfrac{3}{16}$ |

（Ⅱ）$P\{\min\{X,Y\}\geqslant 0\}=\dfrac{1}{16}+\dfrac{3}{16}=\dfrac{1}{4}$．

（Ⅲ）$X$ 与 $Y$ 的边缘分布律分别为

| $X$ | $0$ | $1$ |
| --- | --- | --- |
| $p$ | $\dfrac{1}{4}$ | $\dfrac{3}{4}$ |

| $Y$ | $-1$ | $1$ |
| --- | --- | --- |
| $p$ | $\dfrac{3}{4}$ | $\dfrac{1}{4}$ |

显然满足 $p_{ij}=p_{i\cdot}\cdot p_{\cdot j}$，故 $X$ 与 $Y$ **相互独立**．

+++

#### 基础解答 (2) 设随机变量 $(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}1,&0<x<1,\ -x<y<x,\\0,&\text{其他}.\end{cases}$（Ⅰ）求边缘概率密度 $f_X(x),f_Y(y)$；（Ⅱ）求条件概率密度 $f_{X\mid Y}(x\mid y),f_{Y\mid X}(y\mid x)$；（Ⅲ）求 $P\left\{X>\dfrac{1}{2}\ \middle|\ Y>0\right\}$．
***
（Ⅰ）

$$f_X(x)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}y=\begin{cases}\displaystyle\int_{-x}^{x}1\mathrm{d}y,&0<x<1,\\0,&\text{其他}\end{cases}=\begin{cases}2x,&0<x<1,\\0,&\text{其他},\end{cases}$$

$$f_Y(y)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}x=\begin{cases}\displaystyle\int_{y}^{1}1\mathrm{d}x,&0<y<1,\\[4pt]\displaystyle\int_{-y}^{1}1\mathrm{d}x,&-1<y<0,\\0,&\text{其他},\end{cases}$$

故

$$f_Y(y)=\begin{cases}1-|y|,&|y|<1,\\0,&\text{其他}.\end{cases}$$

（Ⅱ）

$$f_{X\mid Y}(x\mid y)=\frac{f(x,y)}{f_Y(y)}=\begin{cases}\dfrac{1}{1-|y|},&|y|<x<1,\\0,&\text{其他},\end{cases}$$

$$f_{Y\mid X}(y\mid x)=\frac{f(x,y)}{f_X(x)}=\begin{cases}\dfrac{1}{2x},&|y|<x<1,\\0,&\text{其他}.\end{cases}$$

（Ⅲ）

$$P\left\{X>\frac{1}{2}\ \middle|\ Y>0\right\}=\frac{P\left\{X>\frac{1}{2},Y>0\right\}}{P\{Y>0\}}=\frac{\displaystyle\int_{\frac{1}{2}}^{1}\mathrm{d}x\int_{0}^{x}1\mathrm{d}y}{\displaystyle\int_{0}^{1}(1-y)\mathrm{d}y}=\frac{\frac{3}{8}}{\frac{1}{2}}=\frac{3}{4}.$$

【注】考虑到 $f(x,y)$ 的非零部分为常数 $1$，可用**面积**求 $P\left\{X>\frac{1}{2},Y>0\right\}$ 和 $P\{Y>0\}$，如图 $18\text{-}1$ 所示．$P\left\{X>\frac{1}{2},Y>0\right\}$ 等于图中阴影部分的面积，$P\{Y>0\}$ 等于图 $18\text{-}1$ 中 $\triangle AOB$ 的面积，故

$$\frac{P\left\{X>\frac{1}{2},Y>0\right\}}{P\{Y>0\}}=\frac{\frac{3}{8}}{\frac{1}{2}}=\frac{3}{4}.$$

+++

#### 基础解答 (3) 设二维随机变量 $(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}k\mathrm{e}^{-(4x+3y)},&x>0,y>0,\\0,&\text{其他}.\end{cases}$（Ⅰ）求常数 $k$ 的值，并判别 $X$ 与 $Y$ 是否相互独立，说明理由；（Ⅱ）求 $Z=X+Y$ 的概率密度 $f_Z(z)$．
***
（Ⅰ）由

$$\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}x\mathrm{d}y=k\int_{0}^{+\infty}\mathrm{e}^{-4x}\mathrm{d}x\int_{0}^{+\infty}\mathrm{e}^{-3y}\mathrm{d}y=\frac{k}{12}=1,$$

得 $k=12$，故

$$f(x,y)=\begin{cases}12\mathrm{e}^{-(4x+3y)},&x>0,y>0,\\0,&\text{其他}.\end{cases}$$

又由于

$$f_X(x)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}y=\int_{0}^{+\infty}12\mathrm{e}^{-4x}\cdot\mathrm{e}^{-3y}\mathrm{d}y=4\mathrm{e}^{-4x},\quad x>0,$$

故 $f_X(x)=\begin{cases}4\mathrm{e}^{-4x},&x>0,\\0,&\text{其他}.\end{cases}$ 同理，可得 $f_Y(y)=\begin{cases}3\mathrm{e}^{-3y},&y>0,\\0,&\text{其他}.\end{cases}$

显然，$f(x,y)=f_X(x)\cdot f_Y(y)$，故 $X$ 与 $Y$ **相互独立**．

（Ⅱ）由卷积公式，有 $f_Z(z)=\displaystyle\int_{-\infty}^{+\infty}f_X(x)f_Y(z-x)\mathrm{d}x$．

当 $z<0$ 时，$f_Z(z)=0$；当 $z\geqslant 0$ 时，

$$f_Z(z)=\int_{0}^{z}12\mathrm{e}^{-4x}\cdot\mathrm{e}^{-3(z-x)}\mathrm{d}x=12\int_{0}^{z}\mathrm{e}^{-3z}\mathrm{e}^{-x}\mathrm{d}x=12\mathrm{e}^{-3z}(1-\mathrm{e}^{-z}).$$

+++

#### 基础解答 (4) 设随机变量 $X$ 与 $Y$ 相互独立，其概率密度分别为 $f_X(x)=\begin{cases}\lambda_1\mathrm{e}^{-\lambda_1x},&x>0,\\0,&x\leqslant 0,\end{cases}$ $f_Y(y)=\begin{cases}\lambda_2\mathrm{e}^{-\lambda_2y},&y>0,\\0,&y\leqslant 0,\end{cases}$ 其中 $\lambda_1>0,\lambda_2>0$ 为常数，令 $Z=\begin{cases}1,&X\leqslant Y,\\0,&X>Y,\end{cases}$ 求 $Z$ 的分布律和分布函数．
***
由 $X$ 与 $Y$ 相互独立，有

$$f(x,y)=f_X(x)\cdot f_Y(y)=\begin{cases}\lambda_1\lambda_2\mathrm{e}^{-\lambda_1x-\lambda_2y},&x>0,y>0,\\0,&\text{其他},\end{cases}$$

$$P\{Z=1\}=P(X\leqslant Y)=\iint\limits_{x\leqslant y}\lambda_1\lambda_2\mathrm{e}^{-\lambda_1x-\lambda_2y}\mathrm{d}x\mathrm{d}y$$

$$=\lambda_1\lambda_2\int_{0}^{+\infty}\mathrm{e}^{-\lambda_1x}\mathrm{d}x\int_{x}^{+\infty}\mathrm{e}^{-\lambda_2y}\mathrm{d}y=\frac{\lambda_1}{\lambda_1+\lambda_2},$$

$$P\{Z=0\}=1-P\{Z=1\}=\frac{\lambda_2}{\lambda_1+\lambda_2},$$

分布函数为

$$F_Z(z)=\begin{cases}0,&z<0,\\[4pt]\dfrac{\lambda_2}{\lambda_1+\lambda_2},&0\leqslant z<1,\\[4pt]1,&z\geqslant 1.\end{cases}$$

+++

#### 基础解答 (5) 设二维随机变量 $(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}x\mathrm{e}^{-y},&0<x<y<+\infty,\\0,&\text{其他}.\end{cases}$（Ⅰ）求 $X$ 与 $Y$ 的边缘概率密度，并判别 $X$ 与 $Y$ 是否相互独立；（Ⅱ）求 $(X,Y)$ 的分布函数 $F(x,y)$；（Ⅲ）求 $Z=X+Y$ 的概率密度 $f_Z(z)$．
***
（Ⅰ）

$$f_X(x)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}y=\begin{cases}\displaystyle\int_{x}^{+\infty}x\mathrm{e}^{-y}\mathrm{d}y,&x>0,\\0,&x\leqslant 0\end{cases}=\begin{cases}x\mathrm{e}^{-x},&x>0,\\0,&x\leqslant 0,\end{cases}$$

$$f_Y(y)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}x=\begin{cases}\displaystyle\int_{0}^{y}x\mathrm{e}^{-y}\mathrm{d}x,&y>0,\\0,&y\leqslant 0\end{cases}=\begin{cases}\dfrac{1}{2}y^2\mathrm{e}^{-y},&y>0,\\0,&y\leqslant 0,\end{cases}$$

由于 $f(x,y)\neq f_X(x)\cdot f_Y(y)$，故 $X$ 与 $Y$ **不相互独立**．

（Ⅱ）$F(x,y)=P\{X\leqslant x,Y\leqslant y\}$，考虑一点 $(x,y)$ 的分布函数．

当 $x<0$ 或 $y<0$ 时，$F(x,y)=0$；当 $0\leqslant y<x<+\infty$ 时，如图 $18\text{-}2(\mathrm{a})$ 所示，

$$F(x,y)=P\{X\leqslant x,Y\leqslant y\}=\int_{0}^{y}\mathrm{d}y\int_{0}^{y}x\mathrm{e}^{-y}\mathrm{d}x=1-\left(\frac{1}{2}y^2+y+1\right)\mathrm{e}^{-y};$$

当 $0\leqslant x<y<+\infty$ 时，如图 $18\text{-}2(\mathrm{b})$ 所示，

$$F(x,y)=P\{X\leqslant x,Y\leqslant y\}=\int_{0}^{x}\mathrm{d}x\int_{x}^{y}x\mathrm{e}^{-y}\mathrm{d}y=1-(x+1)\mathrm{e}^{-x}-\frac{1}{2}x^2\mathrm{e}^{-y}.$$

（Ⅲ）求 $f_Z(z)$ 用卷积公式

$$f_Z(z)=\int_{-\infty}^{+\infty}f(x,z-x)\mathrm{d}x.$$

当 $z<0$ 时，$f_Z(z)=0$；当 $0<x<z-x$ 时，$f(x,z-x)$ 不为 $0$，即 $0<x<\dfrac{z}{2}$，故当 $z\geqslant 0$ 时，如图 $18\text{-}3$ 所示，

$$f_Z(z)=\int_{0}^{\frac{z}{2}}x\mathrm{e}^{-(z-x)}\mathrm{d}x=\int_{0}^{\frac{z}{2}}\mathrm{e}^{-z}x\mathrm{e}^{x}\mathrm{d}x=\mathrm{e}^{-z}+\left(\frac{z}{2}-1\right)\mathrm{e}^{-\frac{z}{2}}.$$

+++

#### 基础解答 (6) 设随机变量 $X$ 与 $Y$ 相互独立，且服从同一分布，其概率密度为 $f(x)=\begin{cases}\dfrac{2}{x^2},&x>2,\\0,&\text{其他},\end{cases}$ 求 $Z=\dfrac{X}{Y}$ 的分布函数和概率密度．
***
由 $X$ 与 $Y$ 相互独立，知 $(X,Y)$ 的概率密度为

$$f(x,y)=\begin{cases}\dfrac{4}{x^2y^2},&x>2,y>2,\\0,&\text{其他}.\end{cases}$$

用定义法，$F_Z(z)=P\{Z\leqslant z\}=P\left\{\dfrac{X}{Y}\leqslant z\right\}$．

当 $z<0$ 时，$F_Z(z)=P(\varnothing)=0$；

当 $0\leqslant z<1$ 时，如图 $18\text{-}4$ 所示，

$$F_Z(z)=P\left\{\frac{X}{Y}\leqslant z\right\}=P\{(X,Y)\in G\}=\int_{\frac{2}{z}}^{+\infty}\mathrm{d}y\int_{2}^{zy}\frac{4}{x^2y^2}\mathrm{d}x=\int_{\frac{2}{z}}^{+\infty}\left(\frac{2}{y^2}-\frac{4}{zy^3}\right)\mathrm{d}y$$

$$=\left(-\frac{2}{y}+\frac{4}{2zy^2}\right)\Bigg|_{\frac{2}{z}}^{+\infty}=z-\frac{z}{2}=\frac{z}{2};$$

当 $z\geqslant 1$ 时，

$$F_Z(z)=P\left\{\frac{X}{Y}\leqslant z\right\}=1-P\{(X,Y)\in D\}=1-\int_{2}^{+\infty}\mathrm{d}y\int_{zy}^{+\infty}\frac{4}{x^2y^2}\mathrm{d}x$$

$$=1-\int_{2}^{+\infty}\frac{4}{y^3z}\mathrm{d}y=1+\frac{4}{2y^2z}\Bigg|_{2}^{+\infty}=1-\frac{1}{2z},$$

故分布函数为

$$F_Z(z)=\begin{cases}0,&z<0,\\[4pt]\dfrac{z}{2},&0\leqslant z<1,\\[4pt]1-\dfrac{1}{2z},&z\geqslant 1,\end{cases}$$

概率密度为

$$f_Z(z)=F_Z'(z)=\begin{cases}0,&z<0,\\[4pt]\dfrac{1}{2},&0\leqslant z<1,\\[4pt]\dfrac{1}{2z^2},&z\geqslant 1.\end{cases}$$

+++

#### 基础解答 (7) 设随机变量 $X$ 和 $Y$ 相互独立，$X$ 在区间 $(0,1)$ 内服从均匀分布，$Y$ 的概率密度为 $f_Y(y)=\begin{cases}\dfrac{1}{2}\mathrm{e}^{-\frac{y}{2}},&y>0,\\0,&y\leqslant 0.\end{cases}$（Ⅰ）求 $(X,Y)$ 的联合概率密度；（Ⅱ）设 $X$ 和 $Y$ 满足关于 $k$ 的二次方程 $k^2+2Xk+Y=0$，求 $k$ 有实根的概率．
***
（Ⅰ）依题设，可知 $X$ 的概率密度为 $f_X(x)=\begin{cases}1,&0<x<1,\\0,&\text{其他}.\end{cases}$

由 $X$ 与 $Y$ 相互独立，得

$$f(x,y)=f_X(x)f_Y(y)=\begin{cases}\dfrac{1}{2}\mathrm{e}^{-\frac{y}{2}},&0<x<1,y>0,\\0,&\text{其他}.\end{cases}$$

（Ⅱ）$k$ 有实根，则 $\Delta=(2X)^2-4Y\geqslant 0$，即 $X^2\geqslant Y$，令 $A=\{(x,y)\mid x^2\geqslant y\}$，则

$$P(A)=\int_{0}^{1}\mathrm{d}x\int_{0}^{x^2}\frac{1}{2}\mathrm{e}^{-\frac{y}{2}}\mathrm{d}y=\int_{0}^{1}\left(1-\mathrm{e}^{-\frac{x^2}{2}}\right)\mathrm{d}x$$

$$=1-\sqrt{2\pi}\int_{0}^{1}\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{x^2}{2}}\mathrm{d}x=1-\sqrt{2\pi}\left[\Phi(1)-\Phi(0)\right]\approx 0.144\,5,$$

其中 $\Phi(x)$ 为标准正态分布函数．

+++

#### 基础解答 (8) 设 $X$ 与 $Y$ 相互独立，$X$ 服从参数为 $\dfrac{1}{2}$ 的指数分布，$Y$ 服从参数为 $\dfrac{1}{3}$ 的指数分布，求 $Z=X+Y$ 的概率密度．
***
**解法 1** 依题设，$X$ 和 $Y$ 的概率密度分别为

$$f_X(x)=\begin{cases}\dfrac{1}{2}\mathrm{e}^{-\frac{x}{2}},&x>0,\\0,&x\leqslant 0,\end{cases}\qquad f_Y(y)=\begin{cases}\dfrac{1}{3}\mathrm{e}^{-\frac{y}{3}},&y>0,\\0,&y\leqslant 0.\end{cases}$$

用卷积公式 $f_Z(z)=\displaystyle\int_{-\infty}^{+\infty}f_X(x)f_Y(z-x)\mathrm{d}x$．

确定积分限，只需确定 $f_X(x)f_Y(z-x)$ 的非零取值区域，即 $x>0$ 且 $z-x>0$，如图 $18\text{-}5$ 所示．

当 $z<0$ 时，即 $x<z<0$，有 $f_X(x)=0$，$f_Z(z)=0$；当 $z>0$ 时，即 $x>0$ 且 $x<z$，而

$$f_Z(z)=\int_{0}^{z}\frac{1}{2}\mathrm{e}^{-\frac{x}{2}}\cdot\frac{1}{3}\mathrm{e}^{-\frac{z-x}{3}}\mathrm{d}x=\frac{1}{6}\mathrm{e}^{-\frac{z}{3}}\int_{0}^{z}\mathrm{e}^{-\frac{x}{6}}\mathrm{d}x=\mathrm{e}^{-\frac{z}{3}}\left(1-\mathrm{e}^{-\frac{z}{6}}\right),$$

故 $f_Z(z)=\begin{cases}\mathrm{e}^{-\frac{z}{3}}\left(1-\mathrm{e}^{-\frac{z}{6}}\right),&z>0,\\0,&z\leqslant 0.\end{cases}$

**解法 2** 用定义法．

由 $X$ 与 $Y$ 相互独立，故 $(X,Y)$ 的概率密度为

$$f(x,y)=f_X(x)f_Y(y)=\begin{cases}\dfrac{1}{6}\mathrm{e}^{-\left(\frac{x}{2}+\frac{y}{3}\right)},&x>0,y>0,\\0,&\text{其他},\end{cases}$$

$$F_Z(z)=P\{Z\leqslant z\}=P\{X+Y\leqslant z\}.$$

当 $z<0$ 时，$x+y\leqslant z$ 与区域 $x>0,y>0$ 无公共部分，故 $F_Z(z)=P\{X+Y\leqslant z\}=P(\varnothing)=0$．

当 $z>0$ 时，$F_Z(z)=P\{X+Y\leqslant z\}=\displaystyle\iint\limits_{D}f(x,y)\mathrm{d}x\mathrm{d}y$，其中 $D:x+y\leqslant z,x>0,y>0$，如图 $18\text{-}6$ 所示，故

$$F_Z(z)=\int_{0}^{z}\mathrm{d}x\int_{0}^{z-x}\frac{1}{6}\mathrm{e}^{-\left(\frac{x}{2}+\frac{y}{3}\right)}\mathrm{d}y=\frac{1}{2}\int_{0}^{z}\left(\mathrm{e}^{-\frac{x}{2}}-\mathrm{e}^{-\frac{z}{3}}\cdot\mathrm{e}^{-\frac{x}{6}}\right)\mathrm{d}x=1+2\mathrm{e}^{-\frac{z}{2}}-3\mathrm{e}^{-\frac{z}{3}},$$

所以

$$F_Z(z)=\begin{cases}1+2\mathrm{e}^{-\frac{z}{2}}-3\mathrm{e}^{-\frac{z}{3}},&z>0,\\0,&z\leqslant 0,\end{cases}\qquad f_Z(z)=F_Z'(z)=\begin{cases}\mathrm{e}^{-\frac{z}{3}}\left(1-\mathrm{e}^{-\frac{z}{6}}\right),&z>0,\\0,&z\leqslant 0.\end{cases}$$

【注】卷积公式画图是在 $xOz$（或 $yOz$）坐标中，定义法画图是在 $xOy$ 坐标中．

+++

#### 基础解答 (9) 设 $(X,Y)$ 服从区域 $G=\{(x,y)\mid 0\leqslant x\leqslant 2,0\leqslant y\leqslant 1\}$ 上的均匀分布，求 $Z=XY$ 的分布函数与概率密度．
***
用定义法．

由已知，$(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}\dfrac{1}{2},&(x,y)\in G,\\0,&\text{其他},\end{cases}$ 故

$$F_Z(z)=P\{Z\leqslant z\}=P\{XY\leqslant z\}=\iint\limits_{xy\leqslant z}f(x,y)\mathrm{d}x\mathrm{d}y.$$

当 $z<0$ 时，$F_Z(z)=P(\varnothing)=0$；当 $0\leqslant z<2$ 时，积分区域为区域 $G$ 与 $xy\leqslant z$ 的公共部分，如图 $18\text{-}7$ 所示的阴影部分，故

$$F_Z(z)=\int_{0}^{z}\mathrm{d}x\int_{0}^{1}\frac{1}{2}\mathrm{d}y+\int_{z}^{2}\mathrm{d}x\int_{0}^{\frac{z}{x}}\frac{1}{2}\mathrm{d}y=\int_{0}^{z}\frac{1}{2}\mathrm{d}x+\int_{z}^{2}\frac{z}{2x}\mathrm{d}x=\frac{z}{2}(1+\ln 2-\ln z);$$

当 $z\geqslant 2$ 时，$F_Z(z)=1$，所以

$$F_Z(z)=\begin{cases}0,&z\leqslant 0,\\[4pt]\dfrac{z}{2}(1+\ln 2-\ln z),&0<z<2,\\[4pt]1,&z\geqslant 2,\end{cases}$$

$$f_Z(z)=F_Z'(z)=\begin{cases}\dfrac{1}{2}(\ln 2-\ln z),&0<z<2,\\0,&\text{其他}.\end{cases}$$

+++

#### 基础解答 (10) 设随机变量 $X$ 与 $Y$ 相互独立，$X\sim N(0,\sigma^2)$，$Y$ 服从 $[-a,a]\ (a>0)$ 上的均匀分布，求 $Z=X+Y$ 的概率密度（可用 $\Phi(x)$ 表示）．
***
依题意，$Y$ 的概率密度为

$$f_Y(y)=\begin{cases}\dfrac{1}{2a},&-a\leqslant y\leqslant a,\\0,&\text{其他},\end{cases}$$

$X$ 的概率密度为 $f_X(x)=\dfrac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{x^2}{2\sigma^2}}$，$-\infty<x<+\infty$．

由于 $X$ 与 $Y$ 相互独立，由卷积公式，得

$$f_Z(z)=\int_{-\infty}^{+\infty}f_X(z-y)f_Y(y)\mathrm{d}y=\int_{-a}^{a}\frac{1}{\sqrt{2\pi}\sigma}\mathrm{e}^{-\frac{(z-y)^2}{2\sigma^2}}\cdot\frac{1}{2a}\mathrm{d}y,$$

为将其化为标准正态分布的分布函数 $\Phi(x)$，令 $\dfrac{z-y}{\sigma}=-t$，则 $\mathrm{d}y=\sigma\mathrm{d}t$，故

$$f_Z(z)=\int_{\frac{-a-z}{\sigma}}^{\frac{a-z}{\sigma}}\frac{1}{\sqrt{2\pi}}\mathrm{e}^{-\frac{t^2}{2}}\cdot\frac{1}{2a}\mathrm{d}t=\frac{1}{2a}\left[\Phi\left(\frac{a-z}{\sigma}\right)-\Phi\left(\frac{-a-z}{\sigma}\right)\right].$$

+++

#### 基础解答 (11) 设随机变量 $X$ 与 $Y$ 相互独立，$X$ 服从 $p=0.6$ 的 $0-1$ 分布，$Y$ 的分布函数为 $F_Y(y)=\begin{cases}1-\mathrm{e}^{-y},&y\geqslant 0,\\0,&y<0,\end{cases}$ 记 $Z=X-Y$．（Ⅰ）求 $P\left\{Z\leqslant-\dfrac{1}{2}\ \middle|\ X=0\right\}$；（Ⅱ）求 $Z$ 的分布函数．
***
（Ⅰ）由已知，$Y$ 的概率密度为

$$f_Y(y)=F_Y'(y)=\begin{cases}\mathrm{e}^{-y},&y\geqslant 0,\\0,&y<0,\end{cases}$$

$$P\left\{Z\leqslant-\frac{1}{2}\ \middle|\ X=0\right\}=\frac{P\left\{X=0,Z\leqslant-\frac{1}{2}\right\}}{P\{X=0\}}=\frac{P\left\{X=0,Y\geqslant\frac{1}{2}\right\}}{P\{X=0\}}$$

$$=\frac{P\{X=0\}\cdot P\left\{Y\geqslant\frac{1}{2}\right\}}{P\{X=0\}}=P\left\{Y\geqslant\frac{1}{2}\right\}=1-\int_{0}^{\frac{1}{2}}\mathrm{e}^{-y}\mathrm{d}y=\mathrm{e}^{-\frac{1}{2}}.$$

（Ⅱ）

$$F_Z(z)=P\{Z\leqslant z\}=P\{X-Y\leqslant z\}$$

$$=P\{X=0\}\cdot P\{X-Y\leqslant z\mid X=0\}+P\{X=1\}\cdot P\{X-Y\leqslant z\mid X=1\}$$

$$=P\{X=0\}\cdot P\{Y\geqslant-z\mid X=0\}+P\{X=1\}\cdot P\{Y\geqslant 1-z\mid X=1\}.$$

由 $X$ 与 $Y$ 相互独立，知

$$P\{Y\geqslant-z\mid X=0\}=P\{Y\geqslant-z\}=\begin{cases}\mathrm{e}^{z},&z<0,\\1,&z\geqslant 0,\end{cases}$$

$$P\{Y\geqslant 1-z\mid X=1\}=P\{Y\geqslant 1-z\}=\begin{cases}\mathrm{e}^{z-1},&z<1,\\1,&z\geqslant 1,\end{cases}$$

故 $Z$ 的分布函数为

$$F_Z(z)=\begin{cases}0.4\mathrm{e}^{z}+0.6\mathrm{e}^{z-1},&z<0,\\0.4+0.6\mathrm{e}^{z-1},&0\leqslant z<1,\\1,&z\geqslant 1.\end{cases}$$

+++

#### 综合选择 (1) 设随机变量 $X$ 与 $Y$ 独立同分布，均服从 $P\{X=k\}=p(1-p)^{k-1}$，$k=1,2,\cdots$，$0<p<1$，则 $P\{X=Y\}=$（　）．

;;;
A. $\dfrac{p}{1-p}$
B. $\dfrac{1-p}{2-p}$
C. $\dfrac{2p}{1-p}$
D. $\dfrac{p}{2-p}$
;;;D
***
$$P\{X=Y\}=\sum_{k=1}^{\infty}P\{X=Y=k\}=\sum_{k=1}^{\infty}P\{X=k,Y=k\}$$

$$=\sum_{k=1}^{\infty}P\{X=k\}P\{Y=k\}=\sum_{k=1}^{\infty}p^2\cdot(1-p)^{2(k-1)}$$

$$=p^2\sum_{k=1}^{\infty}\left[(1-p)^2\right]^{k-1}=p^2\cdot\frac{1}{1-(1-p)^2}=\frac{p}{2-p}.$$

+++

#### 综合选择 (2) 设二维随机变量 $(X_1,X_2)$ 的概率密度为 $f_1(x_1,x_2)$，$Y_1=2X_1$，$Y_2=3X_2$，则 $(Y_1,Y_2)$ 的概率密度 $f_2(y_1,y_2)=$（　）．

;;;
A. $f_1(2y_1,3y_2)$
B. $f_1\left(\dfrac{1}{2}y_1,\dfrac{1}{3}y_2\right)$
C. $\dfrac{1}{2}f_1(2y_1,3y_2)$
D. $\dfrac{1}{6}f_1\left(\dfrac{1}{2}y_1,\dfrac{1}{3}y_2\right)$
;;;D
***
记 $(X_1,X_2)$ 的分布函数为 $F_1(x_1,x_2)$，$(Y_1,Y_2)$ 的分布函数为 $F_2(y_1,y_2)$，则

$$F_2(y_1,y_2)=P\{Y_1\leqslant y_1,Y_2\leqslant y_2\}=P\{2X_1\leqslant y_1,3X_2\leqslant y_2\}$$

$$=P\left\{X_1\leqslant\frac{1}{2}y_1,X_2\leqslant\frac{1}{3}y_2\right\}=F_1\left(\frac{1}{2}y_1,\frac{1}{3}y_2\right),$$

故

$$f_2(y_1,y_2)=\frac{\partial F_2(y_1,y_2)}{\partial y_1\partial y_2}=\frac{\partial F_1\left(\frac{1}{2}y_1,\frac{1}{3}y_2\right)}{\partial y_1\partial y_2}=\frac{1}{2}\cdot\frac{1}{3}f_1\left(\frac{1}{2}y_1,\frac{1}{3}y_2\right)=\frac{1}{6}f_1\left(\frac{1}{2}y_1,\frac{1}{3}y_2\right).$$

+++

#### 综合选择 (3) 设随机变量 $X,Y$ 均服从 $N(0,1)$，且 $X$ 与 $Y$ 相互独立，则（　）．

;;;
A. $P\{X-Y\geqslant 0\}=\dfrac{1}{4}$
B. $P\{X+Y\geqslant 0\}=\dfrac{1}{4}$
C. $P\{\min\{X,Y\}\geqslant 0\}=\dfrac{1}{4}$
D. $P\{\max\{X,Y\}\geqslant 0\}=\dfrac{1}{4}$
;;;C
***
令 $A_1=\{X\geqslant 0\}$，$A_2=\{Y\geqslant 0\}$，则 $A_1$ 与 $A_2$ 相互独立，且

$$P(A_1)=P(A_2)=\int_{0}^{+\infty}\varphi(x)\mathrm{d}x=\frac{1}{2},$$

其中 $\varphi(x)$ 为 $N(0,1)$ 的概率密度，故

$$P\{\min\{X,Y\}\geqslant 0\}=P\{X\geqslant 0,Y\geqslant 0\}=P(A_1A_2)=P(A_1)P(A_2)=\frac{1}{4},$$

**C** 正确．

由 $X,Y$ 相互独立且均服从 $N(0,1)$，知 $X+Y,X-Y$ 服从 $N(0,2)$，故

$$P\{X+Y\geqslant 0\}=P\{X-Y\geqslant 0\}=\frac{1}{2},$$

$$P\{\max\{X,Y\}\geqslant 0\}=P(A_1\cup A_2)=1-P(\overline{A_1\cup A_2})=1-P(\overline{A_1})P(\overline{A_2})=\frac{3}{4},$$

选项 A，B，D 错误．

+++

#### 综合填空 (1) 设随机变量 $X$ 与 $Y$ 相互独立，$X$ 服从二项分布 $B\left(4,\dfrac{1}{2}\right)$，$Y$ 服从 $\lambda=1$ 的泊松分布，则概率 $P\{1<\max\{X,Y\}\leqslant 3\}=$ ________．
***
$\dfrac{15}{8\mathrm{e}}$．

记 $U=\max\{X,Y\}$，依题设，有

$$P\{1<\max\{X,Y\}\leqslant 3\}=P\{1<U\leqslant 3\}=P\{U\leqslant 3\}-P\{U\leqslant 1\}$$

$$=P\{X\leqslant 3,Y\leqslant 3\}-P\{X\leqslant 1,Y\leqslant 1\}$$

$$=P\{X\leqslant 3\}\cdot P\{Y\leqslant 3\}-P\{X\leqslant 1\}\cdot P\{Y\leqslant 1\}.$$

而

$$P\{X\leqslant 3\}=1-P\{X=4\}=\frac{15}{16},$$

$$P\{X\leqslant 1\}=P\{X=0\}+P\{X=1\}=\left(\frac{1}{2}\right)^4+4\times\left(\frac{1}{2}\right)^4=\frac{5}{16},$$

$$P\{Y\leqslant 3\}=\sum_{k=0}^{3}\frac{\mathrm{e}^{-1}}{k!}=\frac{8}{3}\mathrm{e}^{-1},$$

$$P\{Y\leqslant 1\}=2\mathrm{e}^{-1},$$

故

$$P\{1<U\leqslant 3\}=\frac{15}{16}\cdot\frac{8}{3}\mathrm{e}^{-1}-\frac{5}{16}\cdot 2\mathrm{e}^{-1}=\frac{15}{8\mathrm{e}}.$$

+++

#### 综合解答 (1) 在区间 $[0,1]$ 上随机地掷两点，求这两点间距离的概率密度．
***
设 $X$ 和 $Y$ 分别表示两点的坐标，则 $(X,Y)$ 服从均匀分布，其概率密度为

$$f(x,y)=\begin{cases}1,&0\leqslant x\leqslant 1,0\leqslant y\leqslant 1,\\0,&\text{其他},\end{cases}$$

所求问题归结为求 $Z=|X-Y|$ 的概率密度．

用定义法，$F_Z(z)=P\{Z\leqslant z\}=P\{|X-Y|\leqslant z\}=\displaystyle\iint\limits_{D}f(x,y)\mathrm{d}x\mathrm{d}y$，其中 $D:|x-y|\leqslant z$，如图 $18\text{-}8$ 所示．

当 $z<0$ 时，$F_Z(z)=0$；当 $0\leqslant z\leqslant 1$ 时，

$$F_Z(z)=\iint\limits_{D}f(x,y)\mathrm{d}x\mathrm{d}y=1-2\cdot\frac{1}{2}(1-z)^2=2z-z^2;$$

当 $z>1$ 时，$D$ 为 $0\leqslant x\leqslant 1,0\leqslant y\leqslant 1$，故 $F_Z(z)=1$，即

$$F_Z(z)=\begin{cases}0,&z<0,\\2z-z^2,&0\leqslant z<1,\\1,&z\geqslant 1,\end{cases}$$

所以 $Z=|X-Y|$ 的概率密度为

$$f_Z(z)=F_Z'(z)=\begin{cases}2(1-z),&0\leqslant z<1,\\0,&\text{其他}.\end{cases}$$

+++

#### 综合解答 (2) 设二维随机变量 $(X,Y)$ 在 $D=\{(x,y)\mid 0\leqslant x\leqslant 2,0\leqslant y\leqslant 1\}$ 上服从均匀分布，令 $U=\begin{cases}0,&X\leqslant Y,\\1,&X>Y,\end{cases}$ $V=\begin{cases}0,&X\leqslant 2Y,\\1,&X>2Y,\end{cases}$ 求 $(U,V)$ 的联合分布律，并判别 $U$ 与 $V$ 是否相互独立．
***
$(U,V)$ 可能的值为 $(0,0),(0,1),(1,0),(1,1)$，依题设，$(X,Y)$ 的概率密度为

$$f(x,y)=\begin{cases}\dfrac{1}{2},&0\leqslant x\leqslant 2,0\leqslant y\leqslant 1,\\0,&\text{其他},\end{cases}$$

考虑到 $f(x,y)$ 的非零取值为常数 $\dfrac{1}{2}$，可直接利用面积进行求解，如图 $18\text{-}9$ 所示，将区域 $D$ 划分为三个三角形区域 $D_1,D_2,D_3$，其面积分别为 $S_1,S_2,S_3$，区域 $D$ 的面积为 $S=S_1+S_2+S_3=2$，用面积求法，得

$$P\{X\leqslant Y\}=\frac{1}{2}\times S_1=\frac{1}{2}\times\frac{1}{2}\times 1\times 1=\frac{1}{4}.$$

同理，得 $P\{X>2Y\}=\dfrac{1}{2}$，$P\{Y<X\leqslant 2Y\}=\dfrac{1}{4}$．故

$$P\{U=0,V=0\}=P\{X\leqslant Y,X\leqslant 2Y\}=P\{X\leqslant Y\}=\frac{1}{4},$$

$$P\{U=0,V=1\}=P\{X\leqslant Y,X>2Y\}=0,$$

$$P\{U=1,V=0\}=P\{X>Y,X\leqslant 2Y\}=P\{Y<X\leqslant 2Y\}=\frac{1}{4},$$

$$P\{U=1,V=1\}=1-\frac{1}{4}-0-\frac{1}{4}=\frac{1}{2},$$

故

| $U\,\backslash\,V$ | $0$ | $1$ | $U$ 的边缘 |
| --- | --- | --- | --- |
| $0$ | $\dfrac{1}{4}$ | $0$ | $\dfrac{1}{4}$ |
| $1$ | $\dfrac{1}{4}$ | $\dfrac{1}{2}$ | $\dfrac{3}{4}$ |
| $V$ 的边缘 | $\dfrac{1}{2}$ | $\dfrac{1}{2}$ | $1$ |

显然 $p_{ij}\neq p_{i\cdot}\cdot p_{\cdot j}$，故 $U$ 与 $V$ **不相互独立**．

+++

#### 综合解答 (3) 设随机变量 $X$ 和 $Y$ 都在 $[a,b]$ 上服从均匀分布，且 $X$ 与 $Y$ 相互独立．（Ⅰ）求 $Z_1=\max\{X,Y\}$ 和 $Z_2=\min\{X,Y\}$ 的概率密度；（Ⅱ）求 $(Z_1,Z_2)$ 的联合概率密度．
***
（Ⅰ）依题设，$X$ 与 $Y$ 的分布函数分别为

$$F_X(x)=\int_{-\infty}^{x}f(t)\mathrm{d}t=\begin{cases}0,&x<a,\\[4pt]\dfrac{x-a}{b-a},&a\leqslant x<b,\\[4pt]1,&x\geqslant b,\end{cases}\qquad F_Y(y)=\int_{-\infty}^{y}f(t)\mathrm{d}t=\begin{cases}0,&y<a,\\[4pt]\dfrac{y-a}{b-a},&a\leqslant y<b,\\[4pt]1,&y\geqslant b.\end{cases}$$

$Z_1$ 的分布函数为

$$F_{Z_1}(z)=P\{Z_1\leqslant z\}=P\{\max\{X,Y\}\leqslant z\}=P\{X\leqslant z,Y\leqslant z\}=P\{X\leqslant z\}P\{Y\leqslant z\}.$$

当 $a\leqslant z\leqslant b$ 时，$F_{Z_1}(z)=\dfrac{z-a}{b-a}\cdot\dfrac{z-a}{b-a}=\left(\dfrac{z-a}{b-a}\right)^2$；当 $z<a$ 时，$F_{Z_1}(z)=0$；当 $z>b$ 时，$F_{Z_1}(z)=1$，故

$$F_{Z_1}(z)=\begin{cases}0,&z<a,\\[4pt]\left(\dfrac{z-a}{b-a}\right)^2,&a\leqslant z<b,\\[4pt]1,&z\geqslant b,\end{cases}\qquad f_{Z_1}(z)=F_{Z_1}'(z)=\begin{cases}\dfrac{2(z-a)}{(b-a)^2},&a\leqslant z\leqslant b,\\0,&\text{其他}.\end{cases}$$

$Z_2$ 的分布函数为

$$F_{Z_2}(z)=P\{Z_2\leqslant z\}=1-P\{Z_2>z\}=1-P\{\min\{X,Y\}>z\}$$

$$=1-P\{X>z,Y>z\}=1-\left[1-P\{X\leqslant z\}\right]^2=\begin{cases}0,&z<a,\\[4pt]1-\left(1-\dfrac{z-a}{b-a}\right)^2,&a\leqslant z<b,\\[4pt]1,&z\geqslant b,\end{cases}$$

$$f_{Z_2}(z)=F_{Z_2}'(z)=\begin{cases}\dfrac{2(b-z)}{(b-a)^2},&a\leqslant z\leqslant b,\\0,&\text{其他}.\end{cases}$$

（Ⅱ）$(Z_1,Z_2)$ 的联合分布函数为

$$F(z_1,z_2)=P\{Z_1\leqslant z_1,Z_2\leqslant z_2\}=P\{\max\{X,Y\}\leqslant z_1,\ \min\{X,Y\}\leqslant z_2\}.$$

当 $z_1<z_2$ 时，$F(z_1,z_2)=0$；当 $z_1>z_2$ 时，

$$F(z_1,z_2)=P\left\{(\max\{X,Y\}\leqslant z_1)\cap\left[\Omega-(\min\{X,Y\}>z_2)\right]\right\}$$

$$=P\left\{(\max\{X,Y\}\leqslant z_1)-\left[(\max\{X,Y\}\leqslant z_1)\cap(\min\{X,Y\}>z_2)\right]\right\}$$

$$=P\{\max\{X,Y\}\leqslant z_1\}-P\{(\max\{X,Y\}\leqslant z_1)\cap(\min\{X,Y\}>z_2)\}$$

$$=F_{Z_1}(z_1)-P\{(X\leqslant z_1,Y\leqslant z_1)\cap(X>z_2,Y>z_2)\}$$

$$=F_{Z_1}(z_1)-P\{z_2<X\leqslant z_1,z_2<Y\leqslant z_1\}.$$

由（Ⅰ）的结果，可得

$$F(z_1,z_2)=\begin{cases}0,&z_2<a,\\[4pt]\left(\dfrac{z_1-a}{b-a}\right)^2-\left(\dfrac{z_1-z_2}{b-a}\right)^2,&a\leqslant z_2\leqslant z_1<b,\\[4pt]1-\left(\dfrac{b-z_2}{b-a}\right)^2,&a\leqslant z_2<b<z_1,\\[4pt]1,&b\leqslant z_2<z_1,\end{cases}$$

故 $(Z_1,Z_2)$ 的联合概率密度为

$$f(z_1,z_2)=\frac{\partial^2F(z_1,z_2)}{\partial z_1\partial z_2}=\begin{cases}\dfrac{2}{(b-a)^2},&a<z_2\leqslant z_1<b,\\0,&\text{其他}.\end{cases}$$

+++

#### 综合解答 (4) 设二维随机变量 $(X,Y)$ 服从 $D=\{(x,y)\mid y\geqslant 0,x^2+y^2\leqslant 1\}$ 上的均匀分布，令 $U=\begin{cases}0,&X<0,\\1,&0\leqslant X<Y,\\2,&Y\leqslant X,\end{cases}$ $V=\begin{cases}0,&X\geqslant\sqrt{3}Y,\\1,&X<\sqrt{3}Y.\end{cases}$（Ⅰ）求 $(U,V)$ 的联合概率分布；（Ⅱ）求 $P\{UV\neq 0\}$．
***
（Ⅰ）依题设，$(X,Y)$ 的概率密度为

$$f(x,y)=\begin{cases}\dfrac{2}{\pi},&(x,y)\in D,\\0,&\text{其他},\end{cases}$$

二维随机变量 $(U,V)$ 有六个取值分别为 $(0,0),(0,1),(1,0),(1,1),(2,0),(2,1)$，则

$$P\{U=0,V=0\}=P\{X<0,X\geqslant\sqrt{3}Y\}=P(\varnothing)=0,$$

$$P\{U=1,V=0\}=P\{0\leqslant X<Y,X\geqslant\sqrt{3}Y\}=P(\varnothing)=0.$$

考虑到 $f(x,y)$ 的非零取值为常数 $\dfrac{2}{\pi}$，可直接利用面积求解概率，如图 $18\text{-}10$ 所示，$\angle AOD=\dfrac{\pi}{6}$，$\angle BOD=\dfrac{\pi}{4}$，$\angle COD=\dfrac{\pi}{2}$，可得

$$P\{U=1,V=1\}=P\{0\leqslant X<Y\}=\frac{2}{\pi}\times\frac{1}{2}\times\frac{\pi}{4}\times 1^2=\frac{1}{4},$$

$$P\{U=0,V=1\}=P\{X<0\}=\frac{1}{2},$$

$$P\{U=2,V=0\}=P\{X\geqslant\sqrt{3}Y\}=\frac{1}{6},$$

$$P\{U=2,V=1\}=P\{Y\leqslant X<\sqrt{3}Y\}=\frac{1}{4}-\frac{1}{6}=\frac{1}{12},$$

故 $(U,V)$ 的联合概率分布为

| $U\,\backslash\,V$ | $0$ | $1$ |
| --- | --- | --- |
| $0$ | $0$ | $\dfrac{1}{2}$ |
| $1$ | $0$ | $\dfrac{1}{4}$ |
| $2$ | $\dfrac{1}{6}$ | $\dfrac{1}{12}$ |

（Ⅱ）$P\{UV\neq 0\}=P\{U=1,V=1\}+P\{U=2,V=1\}=\dfrac{1}{4}+\dfrac{1}{12}=\dfrac{1}{3}$．

+++

#### 综合解答 (5) 设 $(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}\dfrac{1}{4}(1+xy),&|x|<1,|y|<1,\\0,&\text{其他}.\end{cases}$（Ⅰ）求 $X$ 和 $Y$ 的边缘概率密度，并判别 $X$ 与 $Y$ 是否相互独立；（Ⅱ）记 $Z_1=X^2$，$Z_2=Y^2$，求 $Z_1,Z_2$ 的分布函数及 $(Z_1,Z_2)$ 的联合分布函数．
***
（Ⅰ）当 $|x|<1$ 时，$X$ 的边缘概率密度为

$$f_X(x)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}y=\int_{-1}^{1}\frac{1}{4}(1+xy)\mathrm{d}y=\frac{1}{2};$$

当 $|x|\geqslant 1$ 时，$f_X(x)=0$，故

$$f_X(x)=\begin{cases}\dfrac{1}{2},&|x|<1,\\0,&|x|\geqslant 1.\end{cases}$$

同理，可得 $Y$ 的边缘概率密度为

$$f_Y(y)=\begin{cases}\dfrac{1}{2},&|y|<1,\\0,&|y|\geqslant 1,\end{cases}$$

显然，$f(x,y)\neq f_X(x)\cdot f_Y(y)$，故 $X$ 与 $Y$ **不相互独立**．

（Ⅱ）设 $Z_1=X^2$ 与 $Z_2=Y^2$ 的分布函数分别为 $F_1(x)$ 与 $F_2(y)$，$(Z_1,Z_2)$ 的分布函数为 $F(x,y)$．

当 $x<0$ 时，$F_1(x)=P\{X^2\leqslant x\}=0$；当 $0\leqslant x<1$ 时，

$$F_1(x)=P\{X^2\leqslant x\}=P\{-\sqrt{x}\leqslant X\leqslant\sqrt{x}\}=\int_{-\sqrt{x}}^{\sqrt{x}}\frac{1}{2}\mathrm{d}x=\sqrt{x};$$

当 $x\geqslant 1$ 时，$F_1(x)=1$，所以

$$F_1(x)=\begin{cases}0,&x<0,\\\sqrt{x},&0\leqslant x<1,\\1,&x\geqslant 1.\end{cases}$$

同理，可得 $F_2(y)=\begin{cases}0,&y<0,\\\sqrt{y},&0\leqslant y<1,\\1,&y\geqslant 1.\end{cases}$

下求 $F(x,y)$．

当 $x<0$ 或 $y<0$ 时，$F(x,y)=0$；

当 $0\leqslant x<1,y\geqslant 1$ 时，$F(x,y)=P\{X^2\leqslant x,Y^2\leqslant y\}=P\{X^2\leqslant x\}=\sqrt{x}$；

当 $0\leqslant y<1,x\geqslant 1$ 时，$F(x,y)=P\{X^2\leqslant x,Y^2\leqslant y\}=P\{Y^2\leqslant y\}=\sqrt{y}$；

当 $0\leqslant x<1,0\leqslant y<1$ 时，

$$F(x,y)=\int_{-\sqrt{x}}^{\sqrt{x}}\mathrm{d}x\int_{-\sqrt{y}}^{\sqrt{y}}\frac{1}{4}(1+xy)\mathrm{d}y=\sqrt{xy};$$

当 $x\geqslant 1,y\geqslant 1$ 时，$F(x,y)=1$，故

$$F(x,y)=\begin{cases}0,&x<0\ \text{或}\ y<0,\\\sqrt{x},&0\leqslant x<1,y\geqslant 1,\\\sqrt{y},&x\geqslant 1,0\leqslant y<1,\\\sqrt{xy},&0\leqslant x<1,0\leqslant y<1,\\1,&x\geqslant 1,y\geqslant 1.\end{cases}$$

【注】① 可以验证：$F(x,y)=F_1(x)\cdot F_2(y)$，故 $X^2$ 与 $Y^2$ 相互独立．\
② 此例说明：$X^2$ 与 $Y^2$ 独立 $\nRightarrow$ $X$ 与 $Y$ 独立．\
③ 一般地：$X$ 与 $Y$ 独立 $\Rightarrow h(X)$ 与 $g(Y)$ 独立，反之不成立（$h,g$ 为连续函数）．

+++

#### 综合解答 (6) 设随机变量 $X$ 的概率密度为 $f(x)=\dfrac{k}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\ (-\infty<x<+\infty)$，对 $X$ 作两次独立观察，其观测值分别记为 $x_1,x_2$，令 $Y_i=\begin{cases}1,&x_i\leqslant 1,\\0,&x_i>1\end{cases}\ (i=1,2)$．（Ⅰ）求 $k$ 的值及 $P\{X_1<0,X_2<1\}$；（Ⅱ）求 $(Y_1,Y_2)$ 的概率分布．
***
（Ⅰ）由

$$\int_{-\infty}^{+\infty}f(x)\mathrm{d}x=\int_{-\infty}^{+\infty}\frac{k}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\mathrm{d}x=k\int_{-\infty}^{+\infty}\frac{\mathrm{e}^{x}}{\mathrm{e}^{2x}+1}\mathrm{d}x=k\arctan\mathrm{e}^{x}\Big|_{-\infty}^{+\infty}=k\cdot\frac{\pi}{2}=1,$$

得 $k=\dfrac{2}{\pi}$．

由已知，$X_1$ 与 $X_2$ 相互独立且与 $X$ 同分布，故

$$P\{X_1<0,X_2<1\}=P\{X_1<0\}\cdot P\{X_2<1\}$$

$$=\left(\frac{2}{\pi}\int_{-\infty}^{0}\frac{\mathrm{d}x}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\right)\left(\frac{2}{\pi}\int_{-\infty}^{1}\frac{\mathrm{d}x}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\right)=\frac{1}{\pi}\arctan\mathrm{e}.$$

（Ⅱ）$(Y_1,Y_2)$ 的四个取值分别为 $(1,1),(1,0),(0,1),(0,0)$，则

$$P\{Y_1=1,Y_2=1\}=P\{X_1\leqslant 1,X_2\leqslant 1\}=\left(\frac{2}{\pi}\int_{-\infty}^{1}\frac{\mathrm{d}x}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\right)^2=\frac{4}{\pi^2}(\arctan\mathrm{e})^2,$$

$$P\{Y_1=1,Y_2=0\}=P\{X_1\leqslant 1,X_2>1\}=P\{X_1\leqslant 1\}\cdot P\{X_2>1\}$$

$$=\frac{2}{\pi}\int_{-\infty}^{1}\frac{\mathrm{d}x}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\cdot\left(1-\frac{2}{\pi}\int_{-\infty}^{1}\frac{\mathrm{d}x}{\mathrm{e}^{x}+\mathrm{e}^{-x}}\right)=\left(\frac{2}{\pi}\arctan\mathrm{e}\right)\left(1-\frac{2}{\pi}\arctan\mathrm{e}\right),$$

$$P\{Y_1=0,Y_2=1\}=P\{Y_1=1,Y_2=0\}=\left(\frac{2}{\pi}\arctan\mathrm{e}\right)\left(1-\frac{2}{\pi}\arctan\mathrm{e}\right),$$

$$P\{Y_1=0,Y_2=0\}=P\{X_1>1,X_2>1\}=P\{X_1>1\}\cdot P\{X_2>1\}=\left(1-\frac{2}{\pi}\arctan\mathrm{e}\right)^2.$$

+++

#### 拓展解答 (1) 设随机变量 $X$ 与 $Y$ 相互独立，$X$ 的概率密度为 $f_X(x)=\begin{cases}1,&0\leqslant x\leqslant 1,\\0,&\text{其他},\end{cases}$ $Y$ 的分布函数为 $F_Y(y)$，令 $Z=\begin{cases}Y,&X\leqslant\dfrac{1}{2},\\[4pt]X,&X>\dfrac{1}{2},\end{cases}$ 求 $Z$ 的分布函数 $F_Z(z)$．
***
用定义法．

$$F_Z(z)=P\{Z\leqslant z\}=P\left\{Z\leqslant z,X\leqslant\frac{1}{2}\right\}+P\left\{Z\leqslant z,X>\frac{1}{2}\right\}$$

$$=P\left\{Y\leqslant z,X\leqslant\frac{1}{2}\right\}+P\left\{X\leqslant z,X>\frac{1}{2}\right\}$$

$$=P\left\{X\leqslant\frac{1}{2}\right\}\cdot P\{Y\leqslant z\}+P\left\{X\leqslant z,X>\frac{1}{2}\right\}$$

$$=\begin{cases}\dfrac{1}{2}F_Y(z),&z<\dfrac{1}{2},\\[6pt]\dfrac{1}{2}F_Y(z)+P\left\{\dfrac{1}{2}<X\leqslant z\right\},&\dfrac{1}{2}\leqslant z<1,\\[6pt]\dfrac{1}{2}F_Y(z)+P\left\{\dfrac{1}{2}<X\leqslant 1\right\},&z\geqslant 1\end{cases}=\begin{cases}\dfrac{1}{2}F_Y(z),&z<\dfrac{1}{2},\\[6pt]\dfrac{1}{2}F_Y(z)+z-\dfrac{1}{2},&\dfrac{1}{2}\leqslant z<1,\\[6pt]\dfrac{1}{2}F_Y(z)+\dfrac{1}{2},&z\geqslant 1.\end{cases}$$

+++

#### 拓展解答 (2) 设二维随机变量 $(X,Y)$ 的概率密度为 $f(x,y)=\begin{cases}\lambda^2\mathrm{e}^{-\lambda x},&0<y<x,\\0,&\text{其他}\end{cases}(\lambda>0)$．（Ⅰ）证明：$Y$ 服从参数为 $\lambda$ 的指数分布；（Ⅱ）问 $X$ 与 $Y$ 是否相互独立？并说明理由．
***
（Ⅰ）求 $Y$ 的边缘概率密度．

当 $y\leqslant 0$ 时，$f_Y(y)=0$；当 $y>0$ 时，

$$f_Y(y)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}x=\int_{y}^{+\infty}\lambda^2\mathrm{e}^{-\lambda x}\mathrm{d}x=\lambda\mathrm{e}^{-\lambda y},$$

故 $f_Y(y)=\begin{cases}\lambda\mathrm{e}^{-\lambda y},&y>0,\\0,&y\leqslant 0,\end{cases}$ 即 $Y$ 服从参数为 $\lambda$ 的指数分布．

（Ⅱ）$X$ 的边缘概率密度为

$$f_X(x)=\int_{-\infty}^{+\infty}f(x,y)\mathrm{d}y=\begin{cases}\displaystyle\int_{0}^{x}\lambda^2\mathrm{e}^{-\lambda x}\mathrm{d}y,&x>0,\\0,&x\leqslant 0\end{cases}=\begin{cases}\lambda^2x\mathrm{e}^{-\lambda x},&x>0,\\0,&x\leqslant 0,\end{cases}$$

结合（Ⅰ），可得 $f(x,y)\neq f_X(x)\cdot f_Y(y)$，由此可知，$X$ 与 $Y$ **不相互独立**．
