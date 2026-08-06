+++

#### 选择 (1) 函数 $f(x)=|x\sin x|\,\mathrm{e}^{\cos x}$，$x\in(-\infty,+\infty)$，是（　）。

;;;
A. 单调函数
B. 周期函数
C. 偶函数
D. 有界函数
;;;C
***
$f(-x)=|(-x)\sin(-x)|\,\mathrm{e}^{\cos(-x)}=|x\sin x|\,\mathrm{e}^{\cos x}=f(x)$，故为**偶函数**。

由于 $|x\sin x|$ 随 $x$ 无限增大，$f(x)$ 既非有界、也非单调、更非周期，故选 **C**。

+++

#### 选择 (2) 设函数 $f(x)=\cos(\sin x)$，$g(x)=\sin(\cos x)$，则当 $x\in\left(0,\dfrac{\pi}{2}\right)$ 时，（　）。

;;;
A. $f(x)$ 单调增加，$g(x)$ 单调减少
B. $f(x)$ 单调减少，$g(x)$ 单调增加
C. $f(x)$ 与 $g(x)$ 都单调增加
D. $f(x)$ 与 $g(x)$ 都单调减少
;;;D
***
在 $\left(0,\dfrac{\pi}{2}\right)$ 上：$\sin x$ 由 $0$ 增到 $1$，而 $\cos$ 在 $(0,1)$ 上递减，故 $f(x)=\cos(\sin x)$ **单调减少**。

$\cos x$ 由 $1$ 减到 $0$，而 $\sin$ 在 $(0,1)$ 上递增，复合后 $g(x)=\sin(\cos x)$ 随 $\cos x$ 减小而 **单调减少**。

故两者都单调减少，选 **D**。

+++

#### 选择 (3) 设函数 $f(x)=\sqrt{1+x+x^2}-\sqrt{1-x+x^2}$，则（　）。

;;;
A. $f(x)$ 为偶函数
B. $f(x)$ 为奇函数
C. $f(x)$ 为无界函数
D. $\lim\limits_{x\to\infty}f(x)=1$
;;;B
***
$f(-x)=\sqrt{1-x+x^2}-\sqrt{1+x+x^2}=-f(x)$，故为**奇函数**，选 **B**。

有理化：$f(x)=\dfrac{2x}{\sqrt{1+x+x^2}+\sqrt{1-x+x^2}}$，$|f(x)|<1$ 有界；且 $x\to+\infty$ 时极限为 $1$，$x\to-\infty$ 时为 $-1$，故 $\lim\limits_{x\to\infty}f(x)$ 不存在，D 错。

+++

#### 选择 (4) 设当 $x\to+\infty$ 时，$f(x)$，$g(x)$ 都是无穷大，则当 $x\to+\infty$ 时，下列结论正确的是（　）。

;;;
A. $f(x)-g(x)$ 是无穷小
B. $f(x)+g(x)$ 是无穷大
C. $\dfrac{g(x)}{f(x)}\to 1$
D. $\dfrac{f(x)+g(x)}{f(x)g(x)}$ 是无穷小
;;;D
***
$\dfrac{f(x)+g(x)}{f(x)g(x)}=\dfrac{1}{g(x)}+\dfrac{1}{f(x)}$。因 $f,g$ 均为无穷大，故 $\dfrac{1}{f}\to 0$、$\dfrac{1}{g}\to 0$，其和为**无穷小**，选 **D**。

A、B、C 均可举反例（无穷大相减/相加不一定仍为无穷大或无穷小，比值不一定趋于 $1$）。

+++

#### 选择 (5) 当 $x\to 0$ 时，$\dfrac{1}{x^2}\sin\dfrac{1}{x}$ 是（　）。

;;;
A. 无穷大
B. 无穷小
C. 有界但非无穷小
D. 无界但非无穷大
;;;D
***
取 $x_n=\dfrac{1}{n\pi}\to 0$，此时 $\sin\dfrac{1}{x_n}=0$，函数值为 $0$，故**不是无穷大**（无穷大要求趋近过程中最终恒大）。

取 $x_n=\dfrac{1}{2n\pi+\frac{\pi}{2}}\to 0$，函数值为 $\dfrac{1}{x_n^2}\to+\infty$，故**无界**。

综上为**无界但非无穷大**，选 **D**。

+++

#### 选择 (6) 已知 $\lim\limits_{x\to\infty}\left(\dfrac{x^2}{x+1}-ax-b\right)=0$，则（　）。

;;;
A. $a=1,\ b=1$
B. $a=-1,\ b=1$
C. $a=1,\ b=-1$
D. $a=-1,\ b=-1$
;;;C
***
$\dfrac{x^2}{x+1}=x-1+\dfrac{1}{x+1}$，故
$$\dfrac{x^2}{x+1}-ax-b=(1-a)x-(1+b)+\dfrac{1}{x+1}.$$
令极限为 $0$，需 $1-a=0$ 且 $-(1+b)=0$，即 $a=1,\ b=-1$，选 **C**。

+++

#### 选择 (7) 设当 $x\to 0$ 时，$(x-\sin x)\tan x$ 是比 $\ln(1+x^n)$ 高阶的无穷小，而 $\ln(1+x^n)$ 是比 $x^2$ 高阶的无穷小，则 $n=$（　）。

;;;
A. $4$
B. $3$
C. $2$
D. $1$
;;;B
***
$x-\sin x\sim\dfrac{x^3}{6}$，$\tan x\sim x$，故 $(x-\sin x)\tan x\sim\dfrac{x^4}{6}$，为 $4$ 阶无穷小。

$\ln(1+x^n)\sim x^n$。由题意 $4>n$ 且 $n>2$，故 $2<n<4$，取 $n=3$，选 **B**。

+++

#### 选择 (8) 设 $f(x)=\ln^2 x$，$g(x)=x$，$h(x)=\mathrm{e}^{\frac{x}{2}}$（$x>1$），则当 $x$ 充分大时，（　）。

;;;
A. $f(x)<g(x)<h(x)$
B. $g(x)<h(x)<f(x)$
C. $h(x)<g(x)<f(x)$
D. $g(x)<f(x)<h(x)$
;;;A
***
当 $x\to+\infty$ 时，增长速度：对数 $\ll$ 幂 $\ll$ 指数，即 $\ln^2 x\ll x\ll\mathrm{e}^{x/2}$。

故 $f(x)<g(x)<h(x)$，选 **A**。

+++

#### 选择 (9) 设 $\lim a_n$ 与 $\lim b_n$ 均不存在，则下列选项正确的是（　）。

;;;
A. 若 $\lim\limits_{n\to\infty}(a_n+b_n)$ 不存在，则 $\lim\limits_{n\to\infty}(a_n-b_n)$ 必不存在
B. 若 $\lim\limits_{n\to\infty}(a_n+b_n)$ 不存在，则 $\lim\limits_{n\to\infty}(a_n-b_n)$ 必存在
C. 若 $\lim\limits_{n\to\infty}(a_n+b_n)$ 存在，则 $\lim\limits_{n\to\infty}(a_n-b_n)$ 必不存在
D. 若 $\lim\limits_{n\to\infty}(a_n+b_n)$ 存在，则 $\lim\limits_{n\to\infty}(a_n-b_n)$ 必存在
;;;C
***
若 $\lim(a_n+b_n)$ 存在，且假设 $\lim(a_n-b_n)$ 也存在，则两式相加得 $\lim 2a_n$ 存在，即 $\lim a_n$ 存在，与已知矛盾。

故 $\lim(a_n-b_n)$ 必不存在，选 **C**。

A、B 可举反例（如 $a_n=(-1)^n,\ b_n=(-1)^n$ 使和不存在而差为 $0$）。

+++

#### 选择 (10) 函数 $f(x)=\dfrac{2+\mathrm{e}^{\frac{1}{x}}}{1+\mathrm{e}^{\frac{2}{x}}}+\dfrac{\sin x}{|x|}$ 在 $x=0$ 处为（　）。

;;;
A. 可去间断点
B. 跳跃间断点
C. 无穷间断点
D. 振荡间断点
;;;A
***
**右极限**（$x\to 0^+$）：$\mathrm{e}^{1/x},\mathrm{e}^{2/x}\to+\infty$，$\dfrac{2+\mathrm{e}^{1/x}}{1+\mathrm{e}^{2/x}}\to 0$；$\dfrac{\sin x}{|x|}\to 1$。故右极限 $=0+1=1$。

**左极限**（$x\to 0^-$）：$\mathrm{e}^{1/x},\mathrm{e}^{2/x}\to 0$，$\dfrac{2+0}{1+0}=2$；$\dfrac{\sin x}{|x|}\to -1$。故左极限 $=2-1=1$。

左右极限都等于 $1$ 而 $f(x)$ 在 $x=0$ 无定义，极限存在，为**可去间断点**，选 **A**。

+++

#### 填空 (1) 设 $f(x)=\begin{cases}1,&|x|\leqslant 1,\\[2pt]0,&|x|>1,\end{cases}$ 则 $f\{f[f(x)]\}=$ ______。
***
无论 $x$ 取何值，$f(x)\in\{0,1\}$，均有 $|f(x)|\leqslant 1$，故 $f[f(x)]=1$；再由 $|1|\leqslant 1$ 得 $f\{f[f(x)]\}=f(1)=1$。

$$f\{f[f(x)]\}=1.$$

+++

#### 填空 (2) 当 $x\to 0$ 时，$(1+ax^2)^{\frac{1}{3}}-1$ 与 $\cos x-1$ 是等价无穷小，则 $a=$ ______。
***
$(1+ax^2)^{\frac{1}{3}}-1\sim\dfrac{1}{3}ax^2$，$\cos x-1\sim-\dfrac{x^2}{2}$。

等价要求 $\dfrac{a}{3}=-\dfrac{1}{2}$，故
$$a=-\dfrac{3}{2}.$$

+++

#### 填空 (3) 设函数 $f(x)=\begin{cases}\dfrac{\sin 2x+\mathrm{e}^{2ax}-1}{x},&x\neq 0,\\[6pt]a,&x=0,\end{cases}$ 在 $x=0$ 处连续，则 $a=$ ______。
***
$\lim\limits_{x\to 0}\dfrac{\sin 2x+\mathrm{e}^{2ax}-1}{x}$，由 $\sin 2x\sim 2x$、$\mathrm{e}^{2ax}-1\sim 2ax$ 得分子 $\sim(2+2a)x$，故极限 $=2+2a$。

连续要求 $a=2+2a$，解得
$$a=-2.$$

+++

#### 填空 (4) 设 $a>0$，若 $\lim\limits_{x\to+\infty}x^{P}\left(a^{\frac{1}{x}}-a^{\frac{1}{x+1}}\right)$ 存在，则 $P$ 的取值范围为 ______。
***
$a^{\frac{1}{x}}-a^{\frac{1}{x+1}}=\mathrm{e}^{\frac{\ln a}{x}}-\mathrm{e}^{\frac{\ln a}{x+1}}\sim\ln a\left(\dfrac{1}{x}-\dfrac{1}{x+1}\right)=\dfrac{\ln a}{x(x+1)}\sim\dfrac{\ln a}{x^2}$（$a\neq 1$）。

于是 $x^{P}\cdot\dfrac{\ln a}{x^2}=(\ln a)\,x^{P-2}$，当 $x\to+\infty$ 时极限存在需 $P-2\leqslant 0$，即
$$P\leqslant 2.$$

+++

#### 填空 (5) $\lim\limits_{x\to+\infty}\dfrac{x^3+x^2+1}{\mathrm{e}^x+x^3}(\sin x+\cos x)=$ ______。
***
分母中 $\mathrm{e}^x$ 起主导作用，故 $\dfrac{x^3+x^2+1}{\mathrm{e}^x+x^3}\to 0$（无穷小）；而 $\sin x+\cos x$ 有界。

无穷小乘有界仍为无穷小，故极限
$$=0.$$

+++

#### 填空 (6) $\lim\limits_{x\to 0}\dfrac{\mathrm{e}^{x^2}-\mathrm{e}^{2-2\cos x}}{\mathrm{e}^{x^4}-1}=$ ______。
***
由 $\cos x=1-\dfrac{x^2}{2}+\dfrac{x^4}{24}-\cdots$，得 $2-2\cos x=x^2-\dfrac{x^4}{12}+\cdots$。

分子 $=\mathrm{e}^{x^2}-\mathrm{e}^{x^2-\frac{x^4}{12}}=\mathrm{e}^{x^2}\left(1-\mathrm{e}^{-\frac{x^4}{12}}\right)\sim 1\cdot\dfrac{x^4}{12}$；分母 $\mathrm{e}^{x^4}-1\sim x^4$。

故极限
$$=\dfrac{1}{12}.$$

+++

#### 填空 (7) 设 $f(x)=a+bx+cx^2+dx^3-\tan x$，当 $x\to 0$ 时，$f(x)$ 是比 $x^3$ 高阶的无穷小，则 $a+b+c+d=$ ______。
***
$\tan x=x+\dfrac{x^3}{3}+\cdots$，故
$$f(x)=a+(b-1)x+cx^2+\left(d-\dfrac{1}{3}\right)x^3+\cdots.$$
要 $f(x)=o(x^3)$，需各系数为 $0$：$a=0,\ b=1,\ c=0,\ d=\dfrac{1}{3}$。

故 $a+b+c+d=0+1+0+\dfrac{1}{3}=\dfrac{4}{3}$。

+++

#### （1）设 $f(x)$ 是定义在 $(-a,a)$ 内的函数，证明：$f(x)$ 可以表示为一个偶函数与一个奇函数之和。
***
构造 $g(x)=\dfrac{f(x)+f(-x)}{2}$，$h(x)=\dfrac{f(x)-f(-x)}{2}$。由于 $(-a,a)$ 关于原点对称，$g,h$ 均在 $(-a,a)$ 内有定义。\
$g(-x)=\dfrac{f(-x)+f(x)}{2}=g(x)$，故 $g(x)$ 为偶函数；\
$h(-x)=\dfrac{f(-x)-f(x)}{2}=-h(x)$，故 $h(x)$ 为奇函数。\
又 $g(x)+h(x)=f(x)$，故 $f(x)$ 可表示为偶函数与奇函数之和。$\blacksquare$

+++

#### （2）设函数 $f(x)$ 满足 $af(x)+bf\left(\dfrac{1}{x}\right)=\dfrac{c}{x}$，其中 $a,b,c$ 均为常数，且 $|a|\neq|b|$，求 $f(x)$ 的表达式，并证明 $f(x)$ 是奇函数。
***
在 $af(x)+bf\left(\dfrac1x\right)=\dfrac{c}{x}$ 中以 $\dfrac1x$ 代 $x$，得 $af\left(\dfrac1x\right)+bf(x)=cx$。\
将两式联立消去 $f\left(\dfrac1x\right)$：第一式 $\times a$ 减第二式 $\times b$，得 $(a^2-b^2)f(x)=\dfrac{ac}{x}-bcx$。\
因 $|a|\neq|b|$，即 $a^2\neq b^2$，故 **$f(x)=\dfrac{c}{a^2-b^2}\left(\dfrac{a}{x}-bx\right)$**。\
又 $f(-x)=\dfrac{c}{a^2-b^2}\left(-\dfrac{a}{x}+bx\right)=-f(x)$，故 $f(x)$ 为奇函数。$\blacksquare$

+++

#### （3）设函数 $f(x)$ 在区间 $(-a,a)$ 内有定义，其中 $a>0$，且对任意 $x_1,x_2\in(-a,a)$，有 $|f(x_1)-f(x_2)|\leqslant|x_1-x_2|$，证明：$F(x)=f(x)+x$ 在 $(-a,a)$ 内单调增加。
***
任取 $x_1,x_2\in(-a,a)$ 且 $x_1<x_2$。由条件 $|f(x_1)-f(x_2)|\leqslant|x_1-x_2|=x_2-x_1$，\
故 $f(x_2)-f(x_1)\geqslant-(x_2-x_1)$。\
于是 $F(x_2)-F(x_1)=[f(x_2)-f(x_1)]+(x_2-x_1)\geqslant-(x_2-x_1)+(x_2-x_1)=0$，\
即当 $x_1<x_2$ 时 $F(x_2)\geqslant F(x_1)$，故 $F(x)=f(x)+x$ 在 $(-a,a)$ 内单调增加（不减）。$\blacksquare$

+++

#### （4）设数列 $\{x_n\}$ 满足 $\lim\limits_{k\to\infty}x_{2k}=\lim\limits_{k\to\infty}x_{2k+1}=a$，证明：$\lim\limits_{n\to\infty}x_n=a$。
***
$\forall\varepsilon>0$。由 $\lim\limits_{k\to\infty}x_{2k}=a$，$\exists K_1$，当 $k>K_1$ 时 $|x_{2k}-a|<\varepsilon$；\
由 $\lim\limits_{k\to\infty}x_{2k+1}=a$，$\exists K_2$，当 $k>K_2$ 时 $|x_{2k+1}-a|<\varepsilon$。\
取 $N=\max\{2K_1,\,2K_2+1\}$。当 $n>N$ 时：若 $n$ 为偶数 $n=2k$，则 $k>K_1$；若 $n$ 为奇数 $n=2k+1$，则 $k>K_2$。两种情形均有 $|x_n-a|<\varepsilon$。\
故 $\lim\limits_{n\to\infty}x_n=a$。$\blacksquare$

+++

#### （5）求下列极限：

（Ⅰ）$\lim\limits_{x\to\infty}\dfrac{x^2-x\sin x}{x^2+x\sin\frac{1}{x}}$；\
（Ⅱ）$\lim\limits_{x\to+\infty}\left(\dfrac{a^{\frac{1}{x}}+b^{\frac{1}{x}}+c^{\frac{1}{x}}}{3}\right)^x$（$a,b,c$ 为正数）；\
（Ⅲ）$\lim\limits_{x\to 0}\dfrac{\ln(\sin^2 x+e^x)-x}{\ln(e^{2x}-x^2)-2x}$；\
（Ⅳ）$\lim\limits_{x\to 0}\dfrac{(1+x)^{\frac{3}{x}}-e^3}{x}$；\
（Ⅴ）$\lim\limits_{x\to 0}\dfrac{e^{\tan x}-e^x}{x^3}$；\
（Ⅵ）$\lim\limits_{x\to 0}\cot x\left(\dfrac{1}{\sin x}-\dfrac{1}{x}\right)$；\
（Ⅶ）$\lim\limits_{x\to 0}(1-x^2)^{\frac{1}{1-\sqrt{1-x^2}}}$；\
（Ⅷ）$\lim\limits_{x\to 0^+}x^{\sin x}$。
***
（Ⅰ）分子分母同除 $x^2$：$\dfrac{1-\frac{\sin x}{x}}{1+\frac{\sin(1/x)}{x}}$。当 $x\to\infty$ 时 $\frac{\sin x}{x}\to0$，$\frac{\sin(1/x)}{x}\sim\frac1{x^2}\to0$，故极限为 **$1$**。\
（Ⅱ）$1^\infty$ 型。$x\ln\dfrac{a^{1/x}+b^{1/x}+c^{1/x}}{3}\sim x\cdot\dfrac{(a^{1/x}-1)+(b^{1/x}-1)+(c^{1/x}-1)}{3}$，而 $x(a^{1/x}-1)\to\ln a$（$b,c$ 同理），和为 $\frac13\ln(abc)$，故极限为 **$\sqrt[3]{abc}$**。\
（Ⅲ）分子 $=\ln\dfrac{\sin^2x+e^x}{e^x}=\ln(1+e^{-x}\sin^2x)\sim\sin^2x\sim x^2$；分母 $=\ln\dfrac{e^{2x}-x^2}{e^{2x}}=\ln(1-e^{-2x}x^2)\sim-x^2$。故极限为 **$-1$**。\
（Ⅳ）$(1+x)^{3/x}=e^{\frac3x\ln(1+x)}=e^{3-\frac32x+o(x)}=e^3\left(1-\frac32x+o(x)\right)$，故 $\dfrac{(1+x)^{3/x}-e^3}{x}\to$ **$-\dfrac32e^3$**。\
（Ⅴ）$\dfrac{e^{\tan x}-e^x}{x^3}=e^x\cdot\dfrac{e^{\tan x-x}-1}{x^3}\sim\dfrac{\tan x-x}{x^3}$，而 $\tan x-x\sim\frac13x^3$，故极限为 **$\dfrac13$**。\
（Ⅵ）$\cot x\left(\dfrac1{\sin x}-\dfrac1x\right)=\dfrac{\cos x\,(x-\sin x)}{x\sin^2x}\sim\dfrac{x-\sin x}{x^3}$，而 $x-\sin x\sim\frac16x^3$，故极限为 **$\dfrac16$**。\
（Ⅶ）$1^\infty$ 型。指数极限 $\dfrac{\ln(1-x^2)}{1-\sqrt{1-x^2}}\sim\dfrac{-x^2}{x^2/2}=-2$（因 $1-\sqrt{1-x^2}\sim\frac12x^2$），故极限为 **$e^{-2}$**。\
（Ⅷ）$x^{\sin x}=e^{\sin x\ln x}$，$\sin x\ln x\sim x\ln x\to0$，故极限为 **$1$**。

+++

#### （6）求下列极限：

（Ⅰ）$\lim\limits_{n\to\infty}\left(\dfrac{1}{n^2+n+1}+\dfrac{2}{n^2+n+2}+\cdots+\dfrac{n}{n^2+n+n}\right)$；\
（Ⅱ）$\lim\limits_{n\to\infty}\left[\sqrt{1+2+\cdots+n}-\sqrt{1+2+\cdots+(n-1)}\right]$；\
（Ⅲ）$\lim\limits_{n\to\infty}\sum\limits_{k=1}^{n}\dfrac{1}{4k^2-1}$；\
（Ⅳ）$\lim\limits_{n\to\infty}\sqrt[n]{1+\dfrac{1}{2}+\dfrac{1}{3}+\cdots+\dfrac{1}{n}}$；\
（Ⅴ）$\lim\limits_{n\to\infty}\left(\dfrac{1+\sqrt[n]{3}}{2}\right)^n$。
***
（Ⅰ）夹逼准则：$\dfrac{\frac{n(n+1)}2}{n^2+2n}\leqslant\sum\limits_{k=1}^n\dfrac{k}{n^2+n+k}\leqslant\dfrac{\frac{n(n+1)}2}{n^2+n+1}$，两端当 $n\to\infty$ 均 $\to\frac12$，故极限为 **$\dfrac12$**。\
（Ⅱ）$1+2+\cdots+n=\dfrac{n(n+1)}2$，原式 $=\dfrac{\frac{n(n+1)}2-\frac{n(n-1)}2}{\sqrt{\frac{n(n+1)}2}+\sqrt{\frac{n(n-1)}2}}=\dfrac{n}{\sqrt{\frac{n(n+1)}2}+\sqrt{\frac{n(n-1)}2}}\to\dfrac{n}{2\cdot\frac{n}{\sqrt2}}=$ **$\dfrac{\sqrt2}{2}$**。\
（Ⅲ）$\dfrac1{4k^2-1}=\dfrac12\left(\dfrac1{2k-1}-\dfrac1{2k+1}\right)$，裂项求和得 $\dfrac12\left(1-\dfrac1{2n+1}\right)\to$ **$\dfrac12$**。\
（Ⅳ）由 $1\leqslant1+\frac12+\cdots+\frac1n\leqslant n$，得 $1\leqslant\sqrt[n]{1+\frac12+\cdots+\frac1n}\leqslant\sqrt[n]{n}\to1$，由夹逼准则极限为 **$1$**。\
（Ⅴ）$1^\infty$ 型。$n\ln\dfrac{1+3^{1/n}}2\sim n\cdot\dfrac{3^{1/n}-1}2\to\dfrac{\ln3}2$（因 $3^{1/n}-1\sim\frac{\ln3}n$），故极限为 $e^{\frac12\ln3}=$ **$\sqrt3$**。

+++

#### （7）求 $f(x)=(1+x)^{\frac{x}{\tan\left(x-\frac{\pi}{4}\right)}}$ 在 $(0,2\pi)$ 内的间断点，并指出其类型。
***
底 $1+x>1>0$ 恒成立，间断点由指数 $\dfrac{x}{\tan(x-\frac\pi4)}$ 决定，需考察 $\tan(x-\frac\pi4)=0$ 及其无定义之处。在 $(0,2\pi)$ 内：\
$x=\frac\pi4,\ \frac{5\pi}4$ 处 $\tan(x-\frac\pi4)=0$，指数 $\to\pm\infty$；\
$x=\frac{3\pi}4,\ \frac{7\pi}4$ 处 $\tan(x-\frac\pi4)$ 无定义（$\to\infty$），指数 $\to0$，$f\to(1+x)^0=1$。\
$x=\frac{3\pi}4$：$\lim f=1$ 存在但 $f$ 在该点无定义，为**第一类（可去）间断点**；同理 $x=\frac{7\pi}4$ 为**第一类（可去）间断点**（极限为 $1$）。\
$x=\frac\pi4$：$x\to\frac\pi4^-$ 时指数 $\to-\infty$，$f\to0$；$x\to\frac\pi4^+$ 时指数 $\to+\infty$，$f\to+\infty$，为**第二类（无穷）间断点**；同理 $x=\frac{5\pi}4$ 为**第二类（无穷）间断点**。

+++

#### （8）讨论函数 $f(x)=\lim\limits_{n\to\infty}\dfrac{x^{n+2}-x^{-n}}{x^n+x^{-n}}$ 的连续性。
***
按 $|x|$ 分类求此极限：\
当 $|x|>1$：分子分母同除 $x^n$，$f=\dfrac{x^2-x^{-2n}}{1+x^{-2n}}\to x^2$（$x^{-2n}\to0$）；\
当 $0<|x|<1$：分子分母同除 $x^{-n}$，$f=\dfrac{x^{2n+2}-1}{x^{2n}+1}\to-1$（$x^{2n}\to0$）；\
当 $x=\pm1$：直接代入得 $f=0$；当 $x=0$ 时 $x^{-n}$ 无定义。\
即 $f(x)=\begin{cases}x^2,&|x|>1\\-1,&0<|x|<1\\0,&x=\pm1\end{cases}$，且在 $x=0$ 处无定义。\
连续性：$f(x)$ 在 $(-\infty,-1),\ (-1,0),\ (0,1),\ (1,+\infty)$ 内均连续。\
$x=0$：左右极限均为 $-1$，但 $f(0)$ 无定义，为**可去间断点（第一类）**；\
$x=1$：左极限 $-1$、右极限 $1$、$f(1)=0$，为**第一类（跳跃）间断点**；\
$x=-1$：左极限 $1$、右极限 $-1$、$f(-1)=0$，为**第一类（跳跃）间断点**。

+++

#### （9）设 $f(x)$ 在 $[a,b]$ 上连续，且 $a<c<d<b$，证明：在 $(a,b)$ 内必存在一点 $\xi$，使得 $mf(c)+nf(d)=(m+n)f(\xi)$，其中 $m,n$ 为任意给定的自然数。
***
记 $\mu=\dfrac{mf(c)+nf(d)}{m+n}$。因 $m,n$ 为自然数（正数），$\mu$ 是 $f(c),f(d)$ 的加权平均，故 $\min\{f(c),f(d)\}\leqslant\mu\leqslant\max\{f(c),f(d)\}$。\
$f(x)$ 在 $[c,d]$ 上连续，由介值定理，$\exists\xi\in[c,d]$ 使 $f(\xi)=\mu$，即 $mf(c)+nf(d)=(m+n)f(\xi)$。\
又 $[c,d]\subset(a,b)$，故 $\xi\in(a,b)$。$\blacksquare$

+++

#### （10）设 $x_1=\sqrt{a}\,(a>0)$，$x_{n+1}=\sqrt{a+x_n}$，证明：$\lim\limits_{n\to\infty}x_n$ 存在，并求其值。
***
**单调性**：$x_2=\sqrt{a+\sqrt a}>\sqrt a=x_1$；若 $x_n>x_{n-1}$，则 $x_{n+1}=\sqrt{a+x_n}>\sqrt{a+x_{n-1}}=x_n$，故 $\{x_n\}$ 单调增加。\
**有界**：设 $L=\dfrac{1+\sqrt{1+4a}}2$（满足 $L^2=a+L$，且 $L>\sqrt a$）。$x_1=\sqrt a<L$；若 $x_n<L$，则 $x_{n+1}=\sqrt{a+x_n}<\sqrt{a+L}=\sqrt{L^2}=L$，故 $\{x_n\}$ 有上界 $L$。\
由单调有界准则，极限存在。设 $\lim\limits_{n\to\infty}x_n=t$，对 $x_{n+1}=\sqrt{a+x_n}$ 取极限得 $t^2=a+t$，解得（取正根）**$\lim\limits_{n\to\infty}x_n=\dfrac{1+\sqrt{1+4a}}2$**。

+++

#### （11）设 $x_1=a\geqslant 0$，$y_1=b\geqslant 0$，$a\leqslant b$，$x_{n+1}=\sqrt{x_n y_n}$，$y_{n+1}=\dfrac{x_n+y_n}{2}$（$n=1,2,\cdots$），证明：$\lim\limits_{n\to\infty}x_n=\lim\limits_{n\to\infty}y_n$。
***
由均值不等式，对 $x_n,y_n\geqslant0$ 有 $x_{n+1}=\sqrt{x_ny_n}\leqslant\dfrac{x_n+y_n}2=y_{n+1}$；又 $x_1=a\leqslant b=y_1$，故对一切 $n$ 有 $x_n\leqslant y_n$。\
从而 $x_{n+1}=\sqrt{x_ny_n}\geqslant\sqrt{x_n\cdot x_n}=x_n$，$\{x_n\}$ 单调增加；$y_{n+1}=\dfrac{x_n+y_n}2\leqslant\dfrac{y_n+y_n}2=y_n$，$\{y_n\}$ 单调减少。\
又 $x_1\leqslant x_n\leqslant y_n\leqslant y_1$，故 $\{x_n\}$ 增而有上界、$\{y_n\}$ 减而有下界，二者均收敛。设 $\lim\limits_{n\to\infty}x_n=\alpha$，$\lim\limits_{n\to\infty}y_n=\beta$。\
对 $y_{n+1}=\dfrac{x_n+y_n}2$ 取极限得 $\beta=\dfrac{\alpha+\beta}2$，即 $\alpha=\beta$，故 **$\lim\limits_{n\to\infty}x_n=\lim\limits_{n\to\infty}y_n$**。$\blacksquare$

+++

#### 综合题·选择题 (1). $\lim\limits_{x\to\infty}\dfrac{e^{\sin\frac{1}{x}}-1}{\left(1+\frac{1}{x}\right)^k-\left(1+\frac{1}{x}\right)}=a\neq 0$ 成立的充要条件是（　）。

;;;
A. $k\neq 1$
B. $k>1$
C. $k>0$
D. 与 $k$ 无关
;;;A
***
令 $t=\dfrac{1}{x}\to 0$。分子 $e^{\sin t}-1\sim\sin t\sim t$。

分母 $(1+t)^k-(1+t)=(1+t)\big[(1+t)^{k-1}-1\big]\sim(1+t)\cdot(k-1)t\sim(k-1)t$。

故原式 $\to\dfrac{1}{k-1}$。要使极限为非零常数 $a$，必须 $k-1\neq 0$，即 $k\neq 1$。

+++

#### 综合题·选择题 (2). 已知 $\lim\limits_{x\to 0}\dfrac{2\arctan x-\ln\frac{1+x}{1-x}}{x^{p}}=c\neq 0$，则（　）。

;;;
A. $p=3,\ c=-\dfrac{4}{3}$
B. $p=-3,\ c=\dfrac{4}{3}$
C. $p=\dfrac{4}{3},\ c=3$
D. $p=-\dfrac{4}{3},\ c=-3$
;;;A
***
利用泰勒展开（$x\to 0$）：

$$2\arctan x=2x-\frac{2}{3}x^{3}+\cdots$$

$$\ln\frac{1+x}{1-x}=\ln(1+x)-\ln(1-x)=2x+\frac{2}{3}x^{3}+\cdots$$

所以分子 $=2\arctan x-\ln\dfrac{1+x}{1-x}=-\dfrac{4}{3}x^{3}+o(x^{3})$。

要使极限为非零常数，取 $p=3$，此时 $c=-\dfrac{4}{3}$。

+++

#### 综合题·选择题 (3). 设当 $x\to 0$ 时，$\alpha(x)=\tan x-\sin x$，$\beta(x)=\sqrt{1+x^{2}}-\sqrt{1-x^{2}}$，$\gamma(x)=\int_{0}^{1-\cos x}\sin t\,dt$ 都是无穷小，将它们关于 $x$ 的阶数从低到高排列，正确的顺序为（　）。

;;;
A. $\alpha(x),\beta(x),\gamma(x)$
B. $\alpha(x),\gamma(x),\beta(x)$
C. $\gamma(x),\alpha(x),\beta(x)$
D. $\beta(x),\alpha(x),\gamma(x)$
;;;D
***
分别求阶：

$\alpha(x)=\tan x-\sin x=\sin x\cdot\dfrac{1-\cos x}{\cos x}\sim x\cdot\dfrac{x^{2}}{2}=\dfrac{x^{3}}{2}$，**3 阶**。

$\beta(x)=\dfrac{(1+x^{2})-(1-x^{2})}{\sqrt{1+x^{2}}+\sqrt{1-x^{2}}}=\dfrac{2x^{2}}{\approx 2}\sim x^{2}$，**2 阶**。

$\gamma(x)=1-\cos(1-\cos x)\sim\dfrac{(1-\cos x)^{2}}{2}\sim\dfrac{(x^{2}/2)^{2}}{2}=\dfrac{x^{4}}{8}$，**4 阶**。

从低到高：$\beta(2)<\alpha(3)<\gamma(4)$，即 $\beta(x),\alpha(x),\gamma(x)$。

+++

#### 综合题·选择题 (4). 设 $y=y(x)$ 是方程 $y''+2y'+y=e^{3x}$ 的解，且满足 $y(0)=y'(0)=0$，则当 $x\to 0$ 时，与 $y(x)$ 为等价无穷小的是（　）。

;;;
A. $\sin x^{2}$
B. $\sin x$
C. $\ln(1+x^{2})$
D. $\ln\sqrt{1+x^{2}}$
;;;D
***
由方程在 $x=0$ 处：$y''(0)+2y'(0)+y(0)=e^{0}=1$，故 $y''(0)=1$。

由泰勒展开 $y(x)=y(0)+y'(0)x+\dfrac{y''(0)}{2}x^{2}+\cdots=\dfrac{1}{2}x^{2}+o(x^{2})$，即 $y(x)\sim\dfrac{x^{2}}{2}$。

而 $\ln\sqrt{1+x^{2}}=\dfrac{1}{2}\ln(1+x^{2})\sim\dfrac{1}{2}x^{2}$，与 $y(x)$ 等价。

（$\sin x^{2}\sim x^{2}$、$\ln(1+x^{2})\sim x^{2}$ 均为 $y(x)$ 的 2 倍，非等价。）

+++

#### 综合题·选择题 (5). 设

$$F(x)=\begin{cases}\dfrac{f(x)}{x},&x\neq 0,\\[2mm] f(0),&x=0,\end{cases}$$

其中 $f(x)$ 在 $x=0$ 处可导，且 $f'(0)\neq 0$，$f(0)=0$，则（　）。

;;;
A. $x=0$ 是 $F(x)$ 的连续点
B. $x=0$ 是 $F(x)$ 的第一类间断点
C. $x=0$ 是 $F(x)$ 的第二类间断点
D. 以上说法均错误
;;;B
***
$F(0)=f(0)=0$。

$\lim\limits_{x\to 0}F(x)=\lim\limits_{x\to 0}\dfrac{f(x)}{x}=\lim\limits_{x\to 0}\dfrac{f(x)-f(0)}{x-0}=f'(0)\neq 0$。

极限存在（等于 $f'(0)$）但不等于 $F(0)=0$，故 $x=0$ 是**可去间断点**，属于第一类间断点。

+++

#### 综合题·选择题 (6). 设

$$f(x)=\begin{cases}(x+1)\arctan\dfrac{1}{x^{2}-1},&x\neq\pm 1,\\[2mm] 0,&x=\pm 1,\end{cases}$$

则 $f(x)$（　）。

;;;
A. 在 $x=1,\ x=-1$ 处都连续
B. 在 $x=1,\ x=-1$ 处都间断
C. 在 $x=-1$ 处间断，$x=1$ 处连续
D. 在 $x=-1$ 处连续，$x=1$ 处间断
;;;D
***
**在 $x=1$ 处：** $x+1\to 2$。当 $x\to 1^{+}$，$x^{2}-1\to 0^{+}$，$\dfrac{1}{x^{2}-1}\to+\infty$，$\arctan\to\dfrac{\pi}{2}$，右极限 $=\pi$；当 $x\to 1^{-}$，$\arctan\to-\dfrac{\pi}{2}$，左极限 $=-\pi$。左右极限不等，故**间断**（跳跃间断点）。

**在 $x=-1$ 处：** $x+1\to 0$，而 $\arctan$ 有界，故乘积 $\to 0=f(-1)$，**连续**。

+++

#### 综合题·选择题 (7). 下列结论中错误的是（　）。

;;;
A. 设 $\lim\limits_{n\to\infty}a_{n}=a>1$，则存在 $M>1$，当 $n$ 充分大时，有 $a_{n}>M$
B. 设 $a=\lim\limits_{n\to\infty}a_{n}<\lim\limits_{n\to\infty}b_{n}=b$，则当 $n$ 充分大时，有 $a_{n}<b_{n}$
C. 设 $M\leqslant a_{n}\leqslant N\ (n=1,2,\cdots)$，若 $\lim\limits_{n\to\infty}a_{n}=a$，则 $M\leqslant a\leqslant N$
D. 若 $\lim\limits_{n\to\infty}a_{n}=a\neq 0$，则当 $n$ 充分大时，$a_{n}>a-\dfrac{1}{n}$
;;;D
***
A、B、C 均为极限保号性/保序性的正确结论。

D 错误：反例取 $a_{n}=a-\dfrac{2}{n}$，则 $\lim a_{n}=a$，但

$$a_{n}-\left(a-\frac{1}{n}\right)=-\frac{2}{n}+\frac{1}{n}=-\frac{1}{n}<0,$$

即 $a_{n}<a-\dfrac{1}{n}$，与 D 矛盾。

+++

#### 综合题·选择题 (8). 设 $\{x_{n}\}$ 与 $\{y_{n}\}$ 为两个数列，则下列说法正确的是（　）。

;;;
A. 若 $\{x_{n}\}$ 与 $\{y_{n}\}$ 无界，则 $\{x_{n}+y_{n}\}$ 无界
B. 若 $\{x_{n}\}$ 与 $\{y_{n}\}$ 无界，则 $\{x_{n}y_{n}\}$ 无界
C. 若 $\{x_{n}\}$ 与 $\{y_{n}\}$ 中，一个有界，一个无界，则 $\{x_{n}y_{n}\}$ 无界
D. 若 $\{x_{n}\}$ 与 $\{y_{n}\}$ 均为无穷大，则 $\{x_{n}y_{n}\}$ 一定为无穷大
;;;D
***
A 错：$x_{n}=n,\ y_{n}=-n$，和为 $0$ 有界。

B 错：$x_{n}$ 取奇数项为 $n$、偶数项为 $0$，$y_{n}$ 反之，二者均无界但乘积恒为 $0$。

C 错：有界数列取 $x_{n}=0$，无界数列 $y_{n}=n$，乘积恒为 $0$ 有界。

D 正确：$|x_{n}|\to\infty,\ |y_{n}|\to\infty\Rightarrow|x_{n}y_{n}|\to\infty$，故乘积为无穷大。

+++

#### 综合题·选择题 (9). 下列极限存在的是（　）。

;;;
A. $\lim\limits_{x\to 1}\dfrac{1}{1+2^{\frac{1}{1-x}}}$
B. $\lim\limits_{x\to+\infty}\left(1+\dfrac{\sin x}{x}\right)^{x}$
C. $\lim\limits_{n\to\infty}\big[n+(-1)^{n}(n+1)\big]$
D. $\lim\limits_{n\to\infty}\left(\dfrac{1}{1^{2}}+\dfrac{1}{2^{2}}+\cdots+\dfrac{1}{n^{2}}\right)^{\frac{1}{n}}$
;;;D
***
A 不存在：$x\to 1^{-}$ 时值 $\to 0$，$x\to 1^{+}$ 时值 $\to 1$，左右不等。

B 不存在：取对数 $x\ln\!\left(1+\dfrac{\sin x}{x}\right)\sim\sin x$，随 $x$ 振荡，$e^{\sin x}$ 不收敛。

C 不存在：$n$ 为偶数时 $=2n+1\to+\infty$，$n$ 为奇数时 $=-1$，振荡。

D 存在：记 $S_{n}=\sum_{k=1}^{n}\dfrac{1}{k^{2}}$，有 $1\leqslant S_{n}<\dfrac{\pi^{2}}{6}$，故 $S_{n}^{1/n}=e^{\frac{\ln S_{n}}{n}}\to e^{0}=1$。

+++

#### 综合题·选择题 (10). 设 $f(x)$ 在 $(-\infty,+\infty)$ 内为连续的奇函数，$a$ 为常数，则必为偶函数的是（　）。

;;;
A. $\displaystyle\int_{0}^{x}du\int_{a}^{u}t f(t)\,dt$
B. $\displaystyle\int_{a}^{x}du\int_{0}^{u}f(t)\,dt$
C. $\displaystyle\int_{0}^{x}du\int_{a}^{u}f(t)\,dt$
D. $\displaystyle\int_{a}^{x}du\int_{0}^{u}t f(t)\,dt$
;;;D
***
记 $\varphi(u)=\int_{0}^{u}f(t)\,dt$（$f$ 奇 $\Rightarrow\varphi$ **偶**），$\psi(u)=\int_{0}^{u}t f(t)\,dt$（$t f(t)$ 偶 $\Rightarrow\psi$ **奇**）。

D：$\displaystyle\int_{a}^{x}\psi(u)\,du=\int_{0}^{x}\psi(u)\,du-\int_{0}^{a}\psi(u)\,du$。$\psi$ 奇 $\Rightarrow\int_{0}^{x}\psi$ 为**偶**，再减常数仍为偶函数，故 D 为偶函数。

（A 含 $-\psi(a)x$ 为奇项；B、C 化简后分别含奇函数项，均非偶。）

+++

#### 综合题·选择题 (11). 设 $f(x)=\lim\limits_{t\to+\infty}\dfrac{x+2^{tx}}{1+2^{tx}}$，则 $F(x)=\int_{-1}^{x}f(t)\,dt$ 在 $x=0$ 处（　）。

;;;
A. 可导
B. 间断点
C. 不可导但连续
D. 无法判定
;;;C
***
求极限得

$$f(x)=\begin{cases}x,&x<0,\\ \tfrac{1}{2},&x=0,\\ 1,&x>0.\end{cases}$$

$f$ 在 $x=0$ 处有跳跃间断（左极限 $0$，右极限 $1$），但有界可积，故 $F(x)$ 处处连续。

在 $x=0$：$F'_{-}(0)=f(0^{-})=0$，$F'_{+}(0)=f(0^{+})=1$，左右导数不等，故 $F(x)$ 在 $x=0$ 处**不可导但连续**。

+++

#### 综合题·选择题 (12). 设

$$f(x)=\begin{cases}\dfrac{(x^{3}-1)\sin x}{|x|(1+x^{2})},&x\neq 0,\\[2mm] 0,&x=0,\end{cases}\qquad x\in(-\infty,+\infty),$$

则（　）。

;;;
A. $f(x)$ 在 $(-\infty,+\infty)$ 内有界
B. 存在 $X>0$，当 $|x|<X$ 时 $f(x)$ 有界，当 $|x|>X$ 时 $f(x)$ 无界
C. 存在 $X>0$，当 $|x|<X$ 时 $f(x)$ 无界，当 $|x|>X$ 时 $f(x)$ 有界
D. 对任意 $X>0$，当 $|x|\leqslant X$ 时 $f(x)$ 有界，但在 $(-\infty,+\infty)$ 内无界
;;;A
***
**$x\to 0$ 时：** 分子 $(x^{3}-1)\sin x\sim(-1)\cdot x=-x$，分母 $\sim|x|$，故 $f(x)\sim-\dfrac{x}{|x|}=-\operatorname{sgn}x$，有界。

**$x\to\infty$ 时：** $\dfrac{x^{3}-1}{|x|(1+x^{2})}\to\pm 1$（$x\to+\infty$ 趋于 $1$，$x\to-\infty$ 趋于 $-1$），乘以有界的 $\sin x$ 仍有界。

分母仅在 $x=0$ 为零而该处已补充定义且邻域有界，$1+x^{2}$ 恒不为零，故 $f(x)$ 在整个 $(-\infty,+\infty)$ 上**有界**。

+++

#### 综合题·填空题 (1). 当 $x\to 0$ 时，$f(x)=3x-4\sin x+\sin x\cos x$ 是关于 $x$ 的 ______ 阶无穷小。

***
**答案：$5$ 阶。**

展开（$x\to 0$）：$\sin x=x-\dfrac{x^{3}}{6}+\dfrac{x^{5}}{120}-\cdots$，

$\sin x\cos x=\dfrac{1}{2}\sin 2x=x-\dfrac{2}{3}x^{3}+\dfrac{2}{15}x^{5}-\cdots$。

代入：

$$f(x)=(3-4+1)x+\left(\tfrac{4}{6}-\tfrac{2}{3}\right)x^{3}+\left(-\tfrac{4}{120}+\tfrac{2}{15}\right)x^{5}+\cdots=\frac{x^{5}}{10}+o(x^{5}).$$

故 $f(x)$ 是 $5$ 阶无穷小。

+++

#### 综合题·填空题 (2). $\lim\limits_{x\to 0}\dfrac{(\cos x-e^{x^{2}})\sin x^{2}}{\frac{x^{2}}{2}+1-\sqrt{1+x^{2}}}=$ ______。

***
**答案：$-12$。**

分子：$\cos x-e^{x^{2}}=\left(1-\tfrac{x^{2}}{2}+\cdots\right)-\left(1+x^{2}+\cdots\right)=-\tfrac{3}{2}x^{2}+\cdots$，乘以 $\sin x^{2}\sim x^{2}$，得 $\sim-\dfrac{3}{2}x^{4}$。

分母：$\sqrt{1+x^{2}}=1+\tfrac{x^{2}}{2}-\tfrac{x^{4}}{8}+\cdots$，故 $\dfrac{x^{2}}{2}+1-\sqrt{1+x^{2}}\sim\dfrac{x^{4}}{8}$。

极限 $=\dfrac{-\frac{3}{2}x^{4}}{\frac{1}{8}x^{4}}=-12$。

+++

#### 综合题·填空题 (3). 设 $f(x)$ 是连续函数，$\lim\limits_{x\to 0}\dfrac{f(x)}{1-\cos x}=-1$，当 $x\to 0$ 时，$\int_{0}^{\sin^{2}x}f(t)\,dt$ 是关于 $x$ 的 $n$ 阶无穷小，则 $n=$ ______。

***
**答案：$n=6$。**

由条件 $f(x)\sim-(1-\cos x)\sim-\dfrac{x^{2}}{2}$（且 $f(0)=0$）。

上限 $\sin^{2}x\sim x^{2}$，故

$$\int_{0}^{\sin^{2}x}f(t)\,dt\sim\int_{0}^{\sin^{2}x}\left(-\frac{t^{2}}{2}\right)dt=-\frac{(\sin^{2}x)^{3}}{6}\sim-\frac{x^{6}}{6}.$$

故为 $6$ 阶无穷小。

+++

#### 综合题·填空题 (4). 设 $a_{n}=\dfrac{3}{2}\displaystyle\int_{0}^{\frac{n}{n+1}}x^{n-1}\sqrt{1+x^{n}}\,dx$，则 $\lim\limits_{n\to\infty}n a_{n}=$ ______。

***
**答案：$\left(1+e^{-1}\right)^{3/2}-1$。**

令 $u=x^{n}$，$du=n x^{n-1}dx$：

$$a_{n}=\frac{3}{2}\cdot\frac{1}{n}\int_{0}^{(n/(n+1))^{n}}\sqrt{1+u}\,du=\frac{1}{n}\left[\left(1+\Big(\tfrac{n}{n+1}\Big)^{n}\right)^{3/2}-1\right].$$

故 $n a_{n}=\left(1+\Big(\tfrac{n}{n+1}\Big)^{n}\right)^{3/2}-1$。

又 $\Big(\dfrac{n}{n+1}\Big)^{n}=\dfrac{1}{(1+1/n)^{n}}\to\dfrac{1}{e}$，所以 $\lim\limits_{n\to\infty}n a_{n}=\left(1+e^{-1}\right)^{3/2}-1$。

+++

#### 综合题·填空题 (5). 设 $k\neq\dfrac{1}{2}$，则 $\lim\limits_{n\to\infty}\ln\left[\dfrac{n-2nk+1}{n(1-2k)}\right]^{n}=$ ______。

***
**答案：$\dfrac{1}{1-2k}$。**

括号内 $=\dfrac{n(1-2k)+1}{n(1-2k)}=1+\dfrac{1}{n(1-2k)}$。

故 $\left[\,\cdots\right]^{n}=\left(1+\dfrac{1}{n(1-2k)}\right)^{n}\to e^{\frac{1}{1-2k}}$。

取对数得 $\lim\limits_{n\to\infty}\ln[\,\cdots]^{n}=\ln e^{\frac{1}{1-2k}}=\dfrac{1}{1-2k}$。

+++

#### 综合题·填空题 (6). 设 $0<a_{1}<a_{2}$，则 $\lim\limits_{n\to\infty}\left(a_{1}^{-n}+a_{2}^{-n}\right)^{\frac{1}{n}}=$ ______。

***
**答案：$\dfrac{1}{a_{1}}$。**

由 $0<a_{1}<a_{2}$ 得 $a_{1}^{-1}>a_{2}^{-1}>0$。由「$n$ 次方和开 $n$ 次方取最大值」的结论：

$$\lim\limits_{n\to\infty}\left(a_{1}^{-n}+a_{2}^{-n}\right)^{\frac{1}{n}}=\max\{a_{1}^{-1},a_{2}^{-1}\}=a_{1}^{-1}=\frac{1}{a_{1}}.$$

+++

#### 综合题·填空题 (7). 设 $\lim\limits_{x\to\infty}\left(\sqrt[3]{1-x^{6}}-ax^{2}-b\right)=0$，则 $a=$ ______，$b=$ ______。

***
**答案：$a=-1$，$b=0$。**

$$\sqrt[3]{1-x^{6}}=\sqrt[3]{-x^{6}\left(1-\tfrac{1}{x^{6}}\right)}=-x^{2}\left(1-\tfrac{1}{x^{6}}\right)^{1/3}=-x^{2}+\frac{1}{3x^{4}}+\cdots$$

于是 $\sqrt[3]{1-x^{6}}-ax^{2}-b=-(1+a)x^{2}-b+o(1)$。

要极限为 $0$，须 $1+a=0$ 且 $b=0$，即 $a=-1,\ b=0$。

+++

#### 综合题·填空题 (8). 设 $\lim\limits_{x\to 0}\left\{a[x]+\dfrac{\ln(1+e^{\frac{2}{x}})}{\ln(1+e^{\frac{1}{x}})}\right\}=b$，其中 $[x]$ 表示不超过 $x$ 的最大整数，则 $a=$ ______，$b=$ ______。

***
**答案：$a=-2$，$b=2$。**

**$x\to 0^{+}$：** $[x]=0$，$\dfrac{1}{x}\to+\infty$，$\ln(1+e^{2/x})\sim\dfrac{2}{x}$，$\ln(1+e^{1/x})\sim\dfrac{1}{x}$，比值 $\to 2$，右极限 $=2$。

**$x\to 0^{-}$：** $[x]=-1$，$\dfrac{1}{x}\to-\infty$，$e^{1/x},e^{2/x}\to 0$，比值 $=\dfrac{e^{2/x}}{e^{1/x}}=e^{1/x}\to 0$，左极限 $=-a$。

极限存在需左右相等：$-a=2\Rightarrow a=-2$，$b=2$。

+++

#### 综合题·填空题 (9). 已知连续函数 $y=f(x)$ 关于点 $(a,0)\,(a\neq 0)$ 对称，则对常数 $c$，$I=\displaystyle\int_{-c}^{c}f(a-x)\,dx=$ ______。

***
**答案：$I=0$。**

关于点 $(a,0)$ 对称即 $f(a-x)+f(a+x)=0$。

令 $x\to-x$ 得 $I=\int_{-c}^{c}f(a-x)\,dx=\int_{-c}^{c}f(a+x)\,dx$。

两式相加：

$$2I=\int_{-c}^{c}\big[f(a-x)+f(a+x)\big]\,dx=\int_{-c}^{c}0\,dx=0,$$

故 $I=0$。

+++

#### (1) 设数列 $\{a_n\}$ 满足 $\lim\limits_{n\to\infty}\dfrac{a_{n+1}}{a_n}=q$，且 $|q|<1$，证明：$\lim\limits_{n\to\infty}a_n=0$。
***
证明：取 $r$ 满足 $|q|<r<1$。由 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=|q|<r$，存在 $N$，使 $n\geqslant N$ 时 $\left|\dfrac{a_{n+1}}{a_n}\right|<r$，即 $|a_{n+1}|<r\,|a_n|$。 \
于是 $n>N$ 时 $|a_n|<r^{\,n-N}|a_N|=\dfrac{|a_N|}{r^{N}}\,r^{n}$。 \
因 $0<r<1$，$\lim\limits_{n\to\infty}r^{n}=0$，由夹逼定理 $|a_n|\to0$，故 **$\lim\limits_{n\to\infty}a_n=0$**。

+++

#### (2) 设 $a_k=2^{\frac{1}{2^k}}$，$u_n=a_1a_2\cdots a_n$（$n=1,2,\cdots$），求 $\lim\limits_{n\to\infty}u_n$。
***
解：$u_n=\prod_{k=1}^{n}2^{1/2^{k}}=2^{\sum_{k=1}^{n}1/2^{k}}=2^{\,1-1/2^{n}}$。 \
当 $n\to\infty$ 时指数 $1-\dfrac{1}{2^{n}}\to1$，故 **$\lim\limits_{n\to\infty}u_n=2$**。

+++

#### (3) 设数列 $x_n=(1+a)^n+(1-a)^n$，证明：

$$\lim_{n\to\infty}\frac{x_{n+1}}{x_n}=\begin{cases}1+|a|, & a\neq 0,\\[4pt] 1, & a=0.\end{cases}$$
***
证明：记 $b=1+a,\ c=1-a$。 \
当 $a=0$：$x_n=2$，$\dfrac{x_{n+1}}{x_n}=1$。 \
当 $a\neq0$：注意 $\max\{|b|,|c|\}=1+|a|$，记为 $\beta$，另一个记为 $\gamma$，则 $\left|\dfrac{\gamma}{\beta}\right|<1$。 \
$\dfrac{x_{n+1}}{x_n}=\dfrac{\beta^{n+1}+\gamma^{n+1}}{\beta^{n}+\gamma^{n}}=\beta\cdot\dfrac{1+(\gamma/\beta)^{n+1}}{1+(\gamma/\beta)^{n}}\to\beta=1+|a|$。 \
故 **$\lim\limits_{n\to\infty}\dfrac{x_{n+1}}{x_n}=\begin{cases}1+|a|,&a\neq0\\ 1,&a=0\end{cases}$**。

+++

#### (4) 证明：$\lim\limits_{n\to\infty}\sqrt[n]{a_1^{\,n}+a_2^{\,n}+\cdots+a_k^{\,n}}=\max\{a_1,a_2,\cdots,a_k\}$（$a_i>0$，$i=1,2,\cdots,k$）。
***
证明：记 $M=\max\{a_1,\dots,a_k\}>0$，则 \
$M^{n}\leqslant a_1^{n}+\cdots+a_k^{n}\leqslant kM^{n}$， \
开 $n$ 次方得 $M\leqslant\sqrt[n]{a_1^{n}+\cdots+a_k^{n}}\leqslant M\sqrt[n]{k}$。 \
因 $\sqrt[n]{k}\to1$，由夹逼定理 **$\lim\limits_{n\to\infty}\sqrt[n]{a_1^{n}+\cdots+a_k^{n}}=M=\max\{a_1,\dots,a_k\}$**。

+++

#### (5)（Ⅰ）设 $x_1=1$，$x_2=2$，$x_{n+2}=\dfrac{1}{2}(3x_{n+1}-x_n)$（$n=1,2,\cdots$），求 $\lim\limits_{n\to\infty}x_n$；

（Ⅱ）设 $x_1=1$，$x_2=2$，$x_{n+2}=\dfrac{1}{2}(x_n+x_{n+1})$，求 $\lim\limits_{n\to\infty}x_n$。
***
（Ⅰ）特征方程 $2r^{2}-3r+1=0$，根 $r=1,\tfrac12$，通解 $x_n=A+B\left(\tfrac12\right)^{n}$。 \
由 $x_1=1,x_2=2$ 得 $A+\tfrac{B}{2}=1,\ A+\tfrac{B}{4}=2$，解得 $A=3,B=-4$，即 $x_n=3-4\left(\tfrac12\right)^{n}$，故 **$\lim\limits_{n\to\infty}x_n=3$**。 \
（Ⅱ）特征方程 $2r^{2}-r-1=0$，根 $r=1,-\tfrac12$，通解 $x_n=A+B\left(-\tfrac12\right)^{n}$。 \
由 $x_1=1,x_2=2$ 得 $A-\tfrac{B}{2}=1,\ A+\tfrac{B}{4}=2$，解得 $A=\tfrac53,B=\tfrac43$，故 **$\lim\limits_{n\to\infty}x_n=\dfrac53$**。

+++

#### (6) 设 $f_n(x)=1-(1-\cos x)^n$（$n=1,2,\cdots$）。

（Ⅰ）证明：方程 $f_n(x)=\dfrac{1}{2}$ 在 $\left(0,\dfrac{\pi}{2}\right)$ 内有且仅有一个实根 $x_n$；

（Ⅱ）设 $x_n\in\left(0,\dfrac{\pi}{2}\right)$，满足 $f_n(x_n)=\dfrac{1}{2}$，证明：$\arccos\dfrac{1}{n}<x_n<\dfrac{\pi}{2}$，且 $\lim\limits_{n\to\infty}x_n=\dfrac{\pi}{2}$。
***
（Ⅰ）令 $g(x)=f_n(x)-\tfrac12$，$g$ 连续。$g(0)=\tfrac12>0$，$g\!\left(\tfrac{\pi}{2}\right)=-\tfrac12<0$，由零点定理有根。 \
在 $\left(0,\tfrac{\pi}{2}\right)$ 上 $\cos x$ 递减，$(1-\cos x)^{n}$ 递增，故 $f_n$ 严格递减，根唯一，记为 $x_n$，即 **有且仅有一个实根**。 \
（Ⅱ）由 $f_n(x_n)=\tfrac12$ 得 $(1-\cos x_n)^{n}=\tfrac12$，即 $\cos x_n=1-2^{-1/n}\in(0,1)$，故 $x_n<\tfrac{\pi}{2}$。 \
又 $\left(1-\tfrac1n\right)^{n}<\tfrac1{\mathrm e}<\tfrac12$，故 $2^{-1/n}>1-\tfrac1n$，即 $\cos x_n=1-2^{-1/n}<\tfrac1n$，由 $\cos$ 递减得 $x_n>\arccos\tfrac1n$。 \
于是 **$\arccos\dfrac1n<x_n<\dfrac{\pi}{2}$**；令 $n\to\infty$，$\cos x_n=1-2^{-1/n}\to0$，故 **$\lim\limits_{n\to\infty}x_n=\dfrac{\pi}{2}$**。

+++

#### (7)（Ⅰ）证明：方程 $x=1+2\ln x$ 在 $(\mathrm{e},+\infty)$ 内有唯一实根 $\xi$；

（Ⅱ）取 $x_0\in(\mathrm{e},\xi)$，令 $x_n=1+2\ln x_{n-1}$（$n=1,2,\cdots$），证明：$\lim\limits_{n\to\infty}x_n=\xi$。
***
（Ⅰ）令 $g(x)=x-1-2\ln x$，$g'(x)=1-\tfrac2x>0\ (x>\mathrm e)$，故 $g$ 在 $(\mathrm e,+\infty)$ 严格递增。 \
$g(\mathrm e)=\mathrm e-3<0$，$g(+\infty)=+\infty$，故 **在 $(\mathrm e,+\infty)$ 内有唯一实根 $\xi$**。 \
（Ⅱ）记 $\varphi(x)=1+2\ln x$，$\varphi(\xi)=\xi$。当 $x_{n-1}\in(\mathrm e,\xi)$ 时 $\varphi$ 递增且 $\varphi(\mathrm e)=3>\mathrm e$，故 $x_n\in(\mathrm e,\xi)$。 \
又 $\varphi(x)-x=-g(x)>0\ (\mathrm e<x<\xi)$，故 $\{x_n\}$ 单调递增且以 $\xi$ 为上界，收敛。 \
设极限为 $L$，则 $L=\varphi(L)$，由不动点唯一得 $L=\xi$，故 **$\lim\limits_{n\to\infty}x_n=\xi$**。

+++

#### (8) 设 $f(x)$ 在 $[0,1]$ 上连续，且 $f(0)=f(1)$，证明：

（Ⅰ）至少存在一点 $\xi\in(0,1)$，使得 $f(\xi)=f\left(\xi+\dfrac{1}{2}\right)$；

（Ⅱ）至少存在一点 $\xi\in(0,1)$，使得 $f(\xi)=f\left(\xi+\dfrac{1}{n}\right)$（$n\geqslant 2$ 为自然数）。
***
（Ⅰ）令 $g(x)=f(x)-f\!\left(x+\tfrac12\right)$，$x\in\left[0,\tfrac12\right]$。 \
$g(0)=f(0)-f\!\left(\tfrac12\right)$，$g\!\left(\tfrac12\right)=f\!\left(\tfrac12\right)-f(1)=-g(0)$，故 $g(0)\,g\!\left(\tfrac12\right)=-g(0)^{2}\leqslant0$。 \
由零点定理（或端点直接取得）存在 $\xi\in(0,1)$ 使 $g(\xi)=0$，即 **$f(\xi)=f\!\left(\xi+\tfrac12\right)$**。 \
（Ⅱ）令 $g(x)=f(x)-f\!\left(x+\tfrac1n\right)$。注意 $\sum_{k=0}^{n-1}g\!\left(\tfrac{k}{n}\right)=f(0)-f(1)=0$。 \
若诸 $g\!\left(\tfrac{k}{n}\right)$ 全为 $0$，取 $\xi=\tfrac1n$ 即可；否则其中有正有负，由介值定理存在 $\xi$ 使 $g(\xi)=0$。 \
故 **存在 $\xi\in(0,1)$ 使 $f(\xi)=f\!\left(\xi+\tfrac1n\right)$**。

+++

#### (9) 证明：$\lim\limits_{n\to\infty}\left[\sin\left(\pi\sqrt{n^2+1}\right)\cdot\sin\left(\pi\sqrt{n^2+n}\right)\right]=0$。
***
证明：$\sqrt{n^{2}+1}-n=\dfrac{1}{\sqrt{n^{2}+1}+n}\to0$。 \
$\sin\!\left(\pi\sqrt{n^{2}+1}\right)=\sin\!\left(\pi n+\pi(\sqrt{n^{2}+1}-n)\right)=(-1)^{n}\sin\!\left(\pi(\sqrt{n^{2}+1}-n)\right)\to0$。 \
又 $\left|\sin\!\left(\pi\sqrt{n^{2}+n}\right)\right|\leqslant1$，由「有界量乘无穷小」得 **$\lim\limits_{n\to\infty}\left[\sin\!\left(\pi\sqrt{n^{2}+1}\right)\sin\!\left(\pi\sqrt{n^{2}+n}\right)\right]=0$**。

+++

#### (10) 计算极限 $\lim\limits_{x\to 0}\dfrac{\displaystyle\int_0^x\left[(3+2\tan t)^t-3^t\right]\mathrm{d}t}{\mathrm{e}^{3x^3}-1}$。
***
解：分母 $\mathrm e^{3x^{3}}-1\sim3x^{3}$。由洛必达法则，原式 $=\lim\limits_{x\to0}\dfrac{(3+2\tan x)^{x}-3^{x}}{9x^{2}\mathrm e^{3x^{3}}}$。 \
而 $(3+2\tan x)^{x}-3^{x}=3^{x}\left[\left(1+\tfrac{2\tan x}{3}\right)^{x}-1\right]$，其中指数 $x\ln\!\left(1+\tfrac{2\tan x}{3}\right)\sim x\cdot\tfrac{2x}{3}=\tfrac{2x^{2}}{3}$。 \
故分子 $\sim3^{x}\cdot\tfrac{2x^{2}}{3}\sim\tfrac{2x^{2}}{3}$，于是原式 $=\lim\limits_{x\to0}\dfrac{2x^{2}/3}{9x^{2}}=$ **$\dfrac{2}{27}$**。

+++

#### (11) 设 $0<x_1<\pi$，$x_{n+1}=\sin x_n$。

（Ⅰ）证明：$\lim\limits_{n\to\infty}x_n$ 存在，并求值；

（Ⅱ）求 $\lim\limits_{n\to\infty}\left(\dfrac{x_{n+1}}{x_n}\right)^{\frac{1}{x_n^{2}}}$。
***
（Ⅰ）当 $n\geqslant2$ 时 $x_n=\sin x_{n-1}\in(0,1)$，且 $\sin x<x\ (x>0)$，故 $x_{n+1}=\sin x_n<x_n$，数列递减且有下界 $0$，收敛。 \
设极限为 $L$，由 $L=\sin L$ 得 $L=0$，故 **$\lim\limits_{n\to\infty}x_n=0$**。 \
（Ⅱ）令 $t=x_n\to0$，$\dfrac{x_{n+1}}{x_n}=\dfrac{\sin t}{t}=1-\tfrac{t^{2}}{6}+o(t^{2})$。 \
$\ln\left(\dfrac{\sin t}{t}\right)^{1/t^{2}}=\dfrac{1}{t^{2}}\ln\!\left(1-\tfrac{t^{2}}{6}+o(t^{2})\right)\to-\dfrac16$，故 **$\lim\limits_{n\to\infty}\left(\dfrac{x_{n+1}}{x_n}\right)^{1/x_n^{2}}=\mathrm e^{-1/6}$**。

+++

#### (12) 设 $\dfrac{1}{n+1}<\ln\left(1+\dfrac{1}{n}\right)<\dfrac{1}{n}$，证明：极限 $\lim\limits_{n\to\infty}\left(1+\dfrac{1}{2}+\cdots+\dfrac{1}{n}-\ln n\right)$ 存在。
***
证明：记 $a_n=\sum_{k=1}^{n}\tfrac1k-\ln n$。 \
$a_{n+1}-a_n=\dfrac{1}{n+1}-\ln\!\left(1+\tfrac1n\right)<0$（因 $\ln(1+\tfrac1n)>\tfrac{1}{n+1}$），故 $\{a_n\}$ 单调递减。 \
又 $\ln n=\sum_{k=1}^{n-1}\ln\!\left(1+\tfrac1k\right)<\sum_{k=1}^{n-1}\tfrac1k<\sum_{k=1}^{n}\tfrac1k$，故 $a_n>0$，数列有下界。 \
单调递减且有下界，由单调有界准则知 **极限 $\lim\limits_{n\to\infty}\left(1+\tfrac12+\cdots+\tfrac1n-\ln n\right)$ 存在**（即欧拉常数 $\gamma$）。

+++

#### (13) 设 $x_1>0$，数列 $\{x_n\}$ 满足 $x_{n+1}=\ln(\mathrm{e}^{x_n}-1)-\ln x_n$，证明：$\lim\limits_{n\to\infty}x_n$ 存在，并求值。
***
证明：$x_{n+1}=\ln\dfrac{\mathrm e^{x_n}-1}{x_n}$。因 $x>0$ 时 $\dfrac{\mathrm e^{x}-1}{x}>1$，故 $x_{n+1}>0$，数列恒正。 \
令 $\phi(x)=\mathrm e^{x}(1-x)$，$\phi'(x)=-x\mathrm e^{x}<0\ (x>0)$，故 $\phi(x)<\phi(0)=1$，即 $\mathrm e^{x}-1<x\mathrm e^{x}$。 \
于是 $\dfrac{\mathrm e^{x_n}-1}{x_n}<\mathrm e^{x_n}$，取对数得 $x_{n+1}<x_n$，数列递减且有下界 $0$，收敛。 \
设极限为 $L$：若 $L>0$ 则 $\mathrm e^{L}(1-L)=1$，与 $x>0$ 时 $\phi(x)<1$ 矛盾，故 **$\lim\limits_{n\to\infty}x_n=0$**。

+++

#### (14) 求下列极限：

（Ⅰ）当 $|x|<1$ 时，求 $\lim\limits_{n\to\infty}(1+x)(1+x^2)(1+x^4)\cdots(1+x^{2^n})$；

（Ⅱ）当 $|x|\neq 0$ 时，求 $\lim\limits_{n\to\infty}\cos\dfrac{x}{2}\cos\dfrac{x}{4}\cdots\cos\dfrac{x}{2^n}$；

（Ⅲ）$\lim\limits_{x\to\frac{\pi}{2}}\dfrac{(1-\sqrt{\sin x})(1-\sqrt[3]{\sin x})\cdots(1-\sqrt[n]{\sin x})}{(1-\sin x)^{n-1}}$。
***
（Ⅰ）乘以 $(1-x)$：$(1-x)\prod_{k=0}^{n}(1+x^{2^{k}})=1-x^{2^{n+1}}$，故乘积 $=\dfrac{1-x^{2^{n+1}}}{1-x}$。 \
$|x|<1$ 时 $x^{2^{n+1}}\to0$，故 **原极限 $=\dfrac{1}{1-x}$**。 \
（Ⅱ）反复用 $\sin2\theta=2\sin\theta\cos\theta$，得 $\prod_{k=1}^{n}\cos\dfrac{x}{2^{k}}=\dfrac{\sin x}{2^{n}\sin(x/2^{n})}$。 \
当 $n\to\infty$ 时 $2^{n}\sin\dfrac{x}{2^{n}}\to x$，故 **原极限 $=\dfrac{\sin x}{x}$**。 \
（Ⅲ）令 $u=\sin x\to1$，每个因子 $\dfrac{1-\sqrt[k]{u}}{1-u}\to\dfrac1k$（$k=2,\dots,n$）。 \
故 **原极限 $=\prod_{k=2}^{n}\dfrac1k=\dfrac{1}{n!}$**。

+++

#### (15) 求下列极限：

（Ⅰ）设 $\lim\limits_{x\to 0}\dfrac{\ln\left[1+\dfrac{f(x)}{\sin x}\right]}{a^x-1}=\dfrac{1}{2}$（$a>0$，$a\neq 1$），求 $\lim\limits_{x\to 0}\dfrac{f(x)}{x^2}$；

（Ⅱ）设 $f(x)$ 是三次多项式，且有 $\lim\limits_{x\to 2a}\dfrac{f(x)}{x-2a}=\lim\limits_{x\to 4a}\dfrac{f(x)}{x-4a}=1$（$a\neq 0$），求 $\lim\limits_{x\to 3a}\dfrac{f(x)}{x-3a}$。
***
（Ⅰ）$a^{x}-1\sim x\ln a$；欲极限有限须 $\dfrac{f(x)}{\sin x}\to0$，则 $\ln\!\left[1+\tfrac{f(x)}{\sin x}\right]\sim\dfrac{f(x)}{\sin x}\sim\dfrac{f(x)}{x}$。 \
于是 $\dfrac{f(x)/x}{x\ln a}=\dfrac{f(x)}{x^{2}\ln a}\to\dfrac12$，得 **$\lim\limits_{x\to0}\dfrac{f(x)}{x^{2}}=\dfrac{\ln a}{2}$**。 \
（Ⅱ）由两条件知 $f(2a)=f(4a)=0$ 且 $f'(2a)=f'(4a)=1$。设 $f(x)=(x-2a)(x-4a)(\alpha x+\beta)$。 \
$f'(2a)=-2a(2a\alpha+\beta)=1,\ f'(4a)=2a(4a\alpha+\beta)=1$，解得 $\alpha=\dfrac{1}{2a^{2}},\ \beta=-\dfrac{3}{2a}$，即 $\alpha x+\beta=\dfrac{x-3a}{2a^{2}}$。 \
故 $\lim\limits_{x\to3a}\dfrac{f(x)}{x-3a}=(3a-2a)(3a-4a)\cdot\dfrac{1}{2a^{2}}=$ **$-\dfrac12$**。

+++

#### (16) 设 $f(x)$ 在 $(a,b)$ 内连续，且 $\lim\limits_{x\to a^{+}}f(x)=-\infty$，$\lim\limits_{x\to b^{-}}f(x)=-\infty$，证明：$f(x)$ 在 $(a,b)$ 内有最大值。
***
证明：任取 $x_0\in(a,b)$，记 $M=f(x_0)$。 \
由 $\lim\limits_{x\to a^{+}}f=-\infty$，存在 $c\in(a,x_0)$，使 $x\in(a,c]$ 时 $f(x)<M$；由 $\lim\limits_{x\to b^{-}}f=-\infty$，存在 $d\in(x_0,b)$，使 $x\in[d,b)$ 时 $f(x)<M$。 \
$f$ 在闭区间 $[c,d]$ 上连续，故取得最大值 $f(\xi)$，且 $f(\xi)\geqslant f(x_0)=M$。 \
而在 $(a,c)\cup(d,b)$ 上 $f(x)<M\leqslant f(\xi)$，故 $f(\xi)$ 是 $f$ 在 $(a,b)$ 上的最大值，即 **$f(x)$ 在 $(a,b)$ 内有最大值**。

+++

#### (1) 设 $f(x)$ 在 $[a,b]$ 上可导，且 $|f'(x)|<1$，当 $x\in[a,b]$ 时，有 $a<f(x)<b$，$F(x)=\dfrac{1}{2}[x+f(x)]$，证明：

（Ⅰ）存在 $x^*\in(a,b)$，使得 $F(x^*)=x^*$；\
（Ⅱ）对 $x_0\in[a,b]$，数列 $\{x_n\}$ 满足 $x_{n+1}=F(x_n)\,(n=0,1,2,\cdots)$，有 $\lim\limits_{n\to\infty}x_n=x^*$.
***

**（Ⅰ）** 令 $g(x)=F(x)-x=\dfrac{1}{2}[f(x)-x]$，它在 $[a,b]$ 上连续。

由 $a<f(x)<b$ 知：$g(a)=\dfrac{1}{2}[f(a)-a]>0$，$g(b)=\dfrac{1}{2}[f(b)-b]<0$。

由零点定理，存在 $x^*\in(a,b)$ 使 $g(x^*)=0$，即 **$F(x^*)=x^*$**（不动点存在）。

又 $g'(x)=\dfrac{1}{2}[f'(x)-1]<0$（因 $f'(x)<1$），故 $g$ 在 $[a,b]$ 上严格单调减少，从而零点 **唯一**，即不动点 $x^*$ 唯一。

**（Ⅱ）** 由 $F'(x)=\dfrac{1}{2}[1+f'(x)]$，而 $|f'(x)|<1$ 即 $-1<f'(x)<1$，得

$$0<F'(x)<1,$$

故 $F$ 在 $[a,b]$ 上严格单调增加。

**数列有定义且落在 $(a,b)$ 内：** 当 $x\in[a,b]$ 时，由 $x\ge a,\ f(x)>a$ 得 $F(x)>\dfrac{1}{2}(a+a)=a$；由 $x\le b,\ f(x)<b$ 得 $F(x)<\dfrac{1}{2}(b+b)=b$。故 $F$ 把 $[a,b]$ 映入 $(a,b)$，所有 $x_n$ 均有定义。

由 $g$ 严格减且 $g(x^*)=0$：当 $x<x^*$ 时 $g(x)>0$，即 $F(x)>x$；又 $F$ 增且 $F(x^*)=x^*$，故 $F(x)<x^*$。于是

$$x<F(x)<x^*\quad(x<x^*).$$

**情形 $x_0<x^*$：** 归纳得 $x_n<x_{n+1}<x^*$，即 $\{x_n\}$ 单调增加且有上界 $x^*$，故收敛于某 $\ell$。对 $x_{n+1}=F(x_n)$ 取极限并由 $F$ 连续得 $\ell=F(\ell)$，即 $\ell$ 为不动点，由唯一性 $\ell=x^*$。

**情形 $x_0>x^*$：** 同理当 $x>x^*$ 时 $x^*<F(x)<x$，故 $x^*<x_{n+1}<x_n$，$\{x_n\}$ 单调减少且有下界 $x^*$，收敛于唯一不动点 $x^*$。

**情形 $x_0=x^*$：** $x_n\equiv x^*$。

综上，**$\lim\limits_{n\to\infty}x_n=x^*$**。

+++

#### (2)（Ⅰ）设 $f(x)$ 是 $[0,+\infty)$ 上单调减少且非负的连续函数．证明：

$$f(k+1)\leqslant \int_k^{k+1} f(x)\,\mathrm{d}x \leqslant f(k)\quad(k=1,2,\cdots);$$

（Ⅱ）证明：$\ln(1+n)\leqslant 1+\dfrac{1}{2}+\cdots+\dfrac{1}{n}\leqslant 1+\ln n$，并求极限 $\lim\limits_{n\to\infty}\dfrac{1+\frac{1}{2}+\cdots+\frac{1}{n}}{\ln n}$.
***

**（Ⅰ）** 因 $f$ 单调减少，对任意 $x\in[k,k+1]$ 有 $f(k+1)\le f(x)\le f(k)$。区间 $[k,k+1]$ 长度为 $1$，由定积分的保序性得

$$f(k+1)=\int_k^{k+1}f(k+1)\,\mathrm{d}x\le \int_k^{k+1}f(x)\,\mathrm{d}x\le \int_k^{k+1}f(k)\,\mathrm{d}x=f(k).$$

即 **$f(k+1)\le \displaystyle\int_k^{k+1}f(x)\,\mathrm{d}x\le f(k)$**。

**（Ⅱ）** 取 $f(x)=\dfrac{1}{x}$（在 $[1,+\infty)$ 上非负、连续、单调减少），由 (Ⅰ) 得

$$\frac{1}{k+1}\le \int_k^{k+1}\frac{\mathrm{d}x}{x}=\ln(k+1)-\ln k\le \frac{1}{k}.$$

**左边不等式：** 由右半 $\ln(k+1)-\ln k\le \dfrac{1}{k}$，对 $k=1,2,\cdots,n$ 求和得

$$\sum_{k=1}^{n}\frac{1}{k}\ge \sum_{k=1}^{n}\big[\ln(k+1)-\ln k\big]=\ln(n+1)-\ln 1=\ln(1+n).$$

**右边不等式：** 由左半 $\dfrac{1}{k+1}\le \ln(k+1)-\ln k$，即 $\dfrac{1}{k}\le \ln k-\ln(k-1)\ (k\ge 2)$，对 $k=2,\cdots,n$ 求和得

$$\sum_{k=2}^{n}\frac{1}{k}\le \sum_{k=2}^{n}\big[\ln k-\ln(k-1)\big]=\ln n-\ln 1=\ln n,$$

故 $\displaystyle\sum_{k=1}^{n}\frac{1}{k}=1+\sum_{k=2}^{n}\frac{1}{k}\le 1+\ln n$。

综合两端即得 **$\ln(1+n)\le 1+\dfrac{1}{2}+\cdots+\dfrac{1}{n}\le 1+\ln n$**。

**求极限：** 记 $H_n=1+\dfrac{1}{2}+\cdots+\dfrac{1}{n}$。两端同除以 $\ln n\,(n\ge 2)$：

$$\frac{\ln(1+n)}{\ln n}\le \frac{H_n}{\ln n}\le \frac{1+\ln n}{\ln n}.$$

当 $n\to\infty$ 时，$\dfrac{\ln(1+n)}{\ln n}\to 1$，$\dfrac{1+\ln n}{\ln n}\to 1$，由夹逼定理得

$$\boxed{\ \lim_{n\to\infty}\frac{1+\frac{1}{2}+\cdots+\frac{1}{n}}{\ln n}=1\ }.$$

