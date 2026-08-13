---
quizify:
  format: 1
  deck: Math_880::Chapter_8
  tags: [Math, 880题, 数一, 第八章, 无穷级数]
---

+++

#### 基础选择 (1) 设级数 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 均发散，则（　）．

;;;
A. $\sum_{n=1}^{\infty}(u_n+v_n)$ 必发散
B. $\sum_{n=1}^{\infty}u_nv_n$ 必发散
C. $\sum_{n=1}^{\infty}(|u_n|+|v_n|)$ 必发散
D. $\sum_{n=1}^{\infty}(u_n^2+v_n^2)$ 必发散
;;;C
***
由 $\sum_{n=1}^{\infty}u_n$ 发散，知 $\sum_{n=1}^{\infty}|u_n|$ 发散（否则 $\sum_{n=1}^{\infty}u_n$ 绝对收敛，故 $\sum_{n=1}^{\infty}u_n$ 收敛，与 $\sum_{n=1}^{\infty}u_n$ 发散矛盾）．

同理，由 $\sum_{n=1}^{\infty}v_n$ 发散，知 $\sum_{n=1}^{\infty}|v_n|$ 发散，于是 $\sum_{n=1}^{\infty}(|u_n|+|v_n|)$ 必发散．

A 选项：当 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 至少有一个不是正项级数时，若 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都发散，$\sum_{n=1}^{\infty}(u_n+v_n)$ 不一定发散，如 $\sum_{n=1}^{\infty}\dfrac{1}{n}$ 与 $\sum_{n=1}^{\infty}\left(-\dfrac{1}{n}\right)$ 均发散，但 $\sum_{n=1}^{\infty}\left(\dfrac{1}{n}-\dfrac{1}{n}\right)=\sum_{n=1}^{\infty}0$ 收敛．

B 选项：如 $\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{n}}$ 与 $\sum_{n=1}^{\infty}\dfrac{1}{n}$ 均发散，但 $\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{n}}\cdot\dfrac{1}{n}=\sum_{n=1}^{\infty}\dfrac{1}{n^{\frac{3}{2}}}$ 收敛．

D 选项：如 $\sum_{n=1}^{\infty}\dfrac{1}{n}$ 与 $\sum_{n=1}^{\infty}\left(-\dfrac{1}{n}\right)$ 均发散，但 $\sum_{n=1}^{\infty}\left[\dfrac{1}{n^2}+\left(-\dfrac{1}{n}\right)^2\right]=\sum_{n=1}^{\infty}\dfrac{2}{n^2}$ 收敛．

+++

#### 基础选择 (2) 下列结论正确的是（　）．

;;;
A. 若 $\sum_{n=1}^{\infty}|u_nv_n|$ 收敛，则 $\sum_{n=1}^{\infty}u_n^2$ 与 $\sum_{n=1}^{\infty}v_n^2$ 都收敛
B. 若 $\sum_{n=1}^{\infty}u_n^2$ 和 $\sum_{n=1}^{\infty}v_n^2$ 都收敛，则 $\sum_{n=1}^{\infty}(u_n+v_n)^2$ 收敛
C. 若 $\sum_{n=1}^{\infty}v_n$ 收敛且 $u_n\leqslant v_n$，则 $\sum_{n=1}^{\infty}u_n$ 收敛
D. 若 $\sum_{n=1}^{\infty}u_n$ 发散 $(u_n\geqslant0)$，则 $u_n\geqslant\dfrac{1}{n}$
;;;B
***
由
$$0\leqslant(u_n+v_n)^2=u_n^2+v_n^2+2u_nv_n\leqslant2(u_n^2+v_n^2),$$
若 $\sum_{n=1}^{\infty}u_n^2$ 和 $\sum_{n=1}^{\infty}v_n^2$ 都收敛，则 $\sum_{n=1}^{\infty}2(u_n^2+v_n^2)$ 收敛．由比较审敛法，知 $\sum_{n=1}^{\infty}(u_n+v_n)^2$ 收敛．

A 选项：不一定成立．

C 选项：缺正项级数条件，不一定成立．

D 选项：如 $\sum_{n=1}^{\infty}\dfrac{1}{2n}$ 发散，但 $\dfrac{1}{2n}<\dfrac{1}{n}$．

【注】常用不等式 $|u_nv_n|\leqslant\dfrac{1}{2}(u_n^2+v_n^2)$．

+++

#### 基础选择 (3) 下列结论正确的是（　）．

;;;
A. 若 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都收敛，则 $\sum_{n=1}^{\infty}u_nv_n$ 必收敛
B. 若 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都发散，则 $\sum_{n=1}^{\infty}u_nv_n$ 必发散
C. 若 $\sum_{n=1}^{\infty}u_n$ 收敛，$\sum_{n=1}^{\infty}v_n$ 发散，则 $\sum_{n=1}^{\infty}u_nv_n$ 必发散
D. 若 $\sum_{n=1}^{\infty}u_n$ 收敛，$\sum_{n=1}^{\infty}v_n\,(v_n>0)$ 收敛，则 $\sum_{n=1}^{\infty}|u_nv_n|$ 收敛
;;;D
***
由 $\sum_{n=1}^{\infty}u_n$ 收敛，知 $\lim\limits_{n\to\infty}u_n=0$（级数收敛的必要条件）．又
$$\lim_{n\to\infty}\frac{|u_nv_n|}{v_n}=\lim_{n\to\infty}|u_n|=0,$$
由比较审敛法的极限形式，知 $\sum_{n=1}^{\infty}|u_nv_n|$ 收敛．

对于 A：取 $u_n=v_n=\dfrac{(-1)^n}{\sqrt{n}}$，$\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都（条件）收敛，但 $\sum_{n=1}^{\infty}u_nv_n=\sum_{n=1}^{\infty}\dfrac{1}{n}$ 发散．

对于 B：取 $u_n=\dfrac{1}{n}$，$v_n=-\dfrac{1}{n}$，$\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都发散，但 $\sum_{n=1}^{\infty}u_nv_n=-\sum_{n=1}^{\infty}\dfrac{1}{n^2}$ 收敛．

对于 C：取 $u_n=\dfrac{1}{n^2}$，$v_n=\dfrac{1}{n}$，$\sum_{n=1}^{\infty}u_n$ 收敛，$\sum_{n=1}^{\infty}v_n$ 发散，但 $\sum_{n=1}^{\infty}u_nv_n=\sum_{n=1}^{\infty}\dfrac{1}{n^3}$ 收敛．

+++

#### 基础选择 (4) 设 $\sum_{n=1}^{\infty}u_n$ 收敛，则下列级数收敛的是（　）．

;;;
A. $\sum_{n=1}^{\infty}u_n^2$
B. $\sum_{n=1}^{\infty}(u_n+u_{n+1})$
C. $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{u_n}{n}$
D. $\sum_{n=1}^{\infty}(u_{2n-1}-u_{2n})$
;;;B
***
由 $\sum_{n=1}^{\infty}u_n$ 收敛，知 $\sum_{n=1}^{\infty}u_{n+1}$ 收敛，根据收敛级数的运算性质，知 $\sum_{n=1}^{\infty}(u_n+u_{n+1})$ 收敛．

取 $u_n=\dfrac{(-1)^{n-1}}{\ln(n+1)}$，则 $\sum_{n=1}^{\infty}u_n$ 收敛，但 $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{u_n}{n}=\sum_{n=1}^{\infty}\dfrac{1}{n\ln(n+1)}$ 发散，排除 C．

取 $u_n=\dfrac{(-1)^{n-1}}{n}$，则 $\sum_{n=1}^{\infty}u_n$ 收敛，但 $\sum_{n=1}^{\infty}(u_{2n-1}-u_{2n})=\sum_{n=1}^{\infty}\left(\dfrac{1}{2n-1}+\dfrac{1}{2n}\right)$ 发散，排除 D．

【注】① 当正项级数 $\sum_{n=1}^{\infty}u_n$ 收敛时，有 $\lim\limits_{n\to\infty}u_n=0$，则当 $n$ 充分大时，$|u_n|=u_n<1$（有界），故 $u_n^2<u_n$，由比较审敛法，知 $\sum_{n=1}^{\infty}u_n^2$ 收敛．

② 若条件改为 $\sum_{n=1}^{\infty}(-1)^{n-1}u_n\,(u_n>0)$ 收敛，则 $\sum_{n=1}^{\infty}(u_{2n-1}-u_{2n})$ 收敛（收敛级数加括号后仍收敛）．

③ 若条件改为 $\sum_{n=1}^{\infty}u_n^2$ 收敛，则 $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{u_n}{n}$ 绝对收敛，因 $\left|(-1)^{n-1}\dfrac{u_n}{n}\right|\leqslant\dfrac{1}{2}\left(u_n^2+\dfrac{1}{n^2}\right)$，而 $\sum_{n=1}^{\infty}\dfrac{1}{n^2}$ 收敛，由比较审敛法，可知 $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{u_n}{n}$ 绝对收敛．

+++

#### 基础选择 (5) 设 $\sum_{n=1}^{\infty}u_n\,(u_n>0)$ 收敛，则下列结论正确的是（　）．

;;;
A. $\sum_{n=1}^{\infty}u_n^2$ 收敛
B. $\sum_{n=1}^{\infty}\sqrt{u_n}$ 收敛
C. $\lim\limits_{n\to\infty}\dfrac{u_{n+1}}{u_n}<1$
D. $\lim\limits_{n\to\infty}\sqrt[n]{u_n}<1$
;;;A
***
由 $\sum_{n=1}^{\infty}u_n\,(u_n>0)$ 收敛，知 $\lim\limits_{n\to\infty}u_n=0$，故当 $n$ 充分大时，$|u_n|=u_n<1$（有界性），则 $u_n^2<u_n$，由比较审敛法，可知 $\sum_{n=1}^{\infty}u_n^2$ 收敛．

B 选项：取 $u_n=\dfrac{1}{n^2}$，则 $\sum_{n=1}^{\infty}\sqrt{u_n}=\sum_{n=1}^{\infty}\dfrac{1}{n}$ 发散．

C 与 D 不正确是由于比值法和根值法的条件是充分非必要的．

+++

#### 基础选择 (6) 下列结论正确的是（　）．

;;;
A. 若 $\sum_{n=1}^{\infty}u_n\,(u_n>0)$ 收敛，则 $\lim\limits_{n\to\infty}n^2u_n=0$
B. 若 $\sum_{n=1}^{\infty}u_n$ 收敛，则 $\sum_{n=1}^{\infty}(-1)^{n-1}u_n$ 必条件收敛
C. 若 $\sum_{n=1}^{\infty}(-1)^{n-1}u_n\,(u_n>0)$ 条件收敛，则 $\sum_{n=1}^{\infty}u_n$ 发散
D. 若 $\sum_{n=1}^{\infty}(u_{2n-1}+u_{2n})$ 收敛，则 $\sum_{n=1}^{\infty}u_n$ 必收敛
;;;C
***
由 $\sum_{n=1}^{\infty}(-1)^{n-1}u_n\,(u_n>0)$ 条件收敛，知 $\sum_{n=1}^{\infty}|(-1)^{n-1}u_n|=\sum_{n=1}^{\infty}u_n$ 发散（否则与已知条件收敛矛盾）．

对于 A：由正项级数的比较审敛法的条件是充分非必要的，知错误．对 $\sum_{n=1}^{\infty}u_n\,(u_n>0)$，有
$$\lim_{n\to\infty}n^2u_n=\lim_{n\to\infty}\frac{u_n}{\frac{1}{n^2}}=0\;\nRightarrow\;\sum_{n=1}^{\infty}u_n\ \text{收敛}.$$

B 显然不一定成立（缺正项级数条件）．D 缺正项级数条件．

+++

#### 基础选择 (7) 级数 $\sum_{n=1}^{\infty}\dfrac{\sqrt{n+1}-\sqrt{n-1}}{n}\sin(n+k)$（$k$ 为常数）（　）．

;;;
A. 绝对收敛
B. 条件收敛
C. 发散
D. 收敛性与 $k$ 有关
;;;A
***
已知级数为任意项级数，
$$\left|\frac{\sqrt{n+1}-\sqrt{n-1}}{n}\sin(n+k)\right|\leqslant\frac{\sqrt{n+1}-\sqrt{n-1}}{n},$$
而
$$\frac{\sqrt{n+1}-\sqrt{n-1}}{n}=\frac{2}{n(\sqrt{n+1}+\sqrt{n-1})}=\frac{2}{n^{\frac{3}{2}}\left(\sqrt{1+\frac{1}{n}}+\sqrt{1-\frac{1}{n}}\right)},$$
故 $\dfrac{\sqrt{n+1}-\sqrt{n-1}}{n}\sim\dfrac{1}{n^{\frac{3}{2}}}\,(n\to\infty)$，而 $\sum_{n=1}^{\infty}\dfrac{1}{n^{\frac{3}{2}}}$ 收敛，所以原级数绝对收敛，A 正确．

+++

#### 基础选择 (8) 设幂级数 $\sum_{n=1}^{\infty}a_n(x-1)^n$ 在 $x=-1$ 处条件收敛，则 $\sum_{n=1}^{\infty}a_n$（　）．

;;;
A. 发散
B. 条件收敛
C. 绝对收敛
D. 无法确定敛散性
;;;C
***
令 $x-1=t$，当 $x=-1$ 时，有 $t=-2$．

依题意，$\sum_{n=1}^{\infty}a_nt^n$ 在 $t=-2$ 处条件收敛，故 $t=-2$ 是其收敛区间的端点，即 $\sum_{n=1}^{\infty}a_nt^n$ 的收敛区间为 $(-2,2)$，故 $-2<x-1<2$，即 $-1<x<3$．

$\sum_{n=1}^{\infty}a_n(x-1)^n$ 在 $x=2$ 时为 $\sum_{n=1}^{\infty}a_n$，显然 $x=2\in(-1,3)$，故 $\sum_{n=1}^{\infty}a_n$ 绝对收敛．

+++

#### 基础填空 (1) 设 $f(x)=\sum_{n=0}^{\infty}x^n$，则 $F(x)=\dfrac{xf(x)}{1-x}$ 展开为 $x$ 的幂级数为________．
***
$\sum_{n=0}^{\infty}nx^n$，$|x|<1$．

由于 $f(x)=\sum_{n=0}^{\infty}x^n=\dfrac{1}{1-x}$，$|x|<1$，$f'(x)=\dfrac{1}{(1-x)^2}$，故
$$F(x)=\frac{xf(x)}{1-x}=\frac{x}{(1-x)^2}=xf'(x)=x\sum_{n=1}^{\infty}nx^{n-1}=\sum_{n=0}^{\infty}nx^n,\ |x|<1.$$

+++

#### 基础填空 (2) 设 $\sum_{n=0}^{\infty}a_n(x-1)^n$ 的收敛域为 $[-1,3]$，则 $\sum_{n=0}^{\infty}a_nx^{2n}$ 的收敛域为________．
***
$[-\sqrt{2},\sqrt{2}]$．

由 $-1\leqslant x\leqslant3$，知 $-2\leqslant x-1\leqslant2$，故 $\sum_{n=0}^{\infty}a_nt^n$ 的收敛域为 $[-2,2]$，令 $t=x^2$，于是 $\sum_{n=0}^{\infty}a_nx^{2n}$ 的收敛域为 $[-\sqrt{2},\sqrt{2}]$．

+++

#### 基础填空 (3) $f(x)=\int_{0}^{x}\mathrm{e}^{-t^2}\,\mathrm{d}t$ 展开为 $x$ 的幂级数为________．
***
$f(x)=\sum_{n=0}^{\infty}(-1)^n\dfrac{x^{2n+1}}{(2n+1)n!}$，$x\in(-\infty,+\infty)$．

由 $\mathrm{e}^x=1+x+\dfrac{x^2}{2!}+\dfrac{x^3}{3!}+\cdots+\dfrac{x^n}{n!}+\cdots$，$x\in(-\infty,+\infty)$，知
$$f(x)=\int_{0}^{x}\mathrm{e}^{-t^2}\,\mathrm{d}t=\int_{0}^{x}\left[1-t^2+\frac{t^4}{2!}-\frac{t^6}{3!}+\cdots+(-1)^n\frac{t^{2n}}{n!}+\cdots\right]\mathrm{d}t$$
$$=\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+1}}{(2n+1)n!},\ x\in(-\infty,+\infty).$$

+++

#### 基础填空 (4) 设 $f(x)=\begin{cases}-1,&-\pi<x\leqslant0,\\ 1+x^2,&0<x\leqslant\pi,\end{cases}$ $f(x)$ 以 $2\pi$ 为周期的傅里叶级数的和函数为 $S(x)$，则 $S(\pi)=$________．
***
$\dfrac{1}{2}\pi^2$．

根据收敛定理，得 $S(\pi)=\dfrac{1}{2}[f(\pi-0)+f(-\pi+0)]=\dfrac{1}{2}\left[(1+\pi^2)+(-1)\right]=\dfrac{1}{2}\pi^2$．

+++

#### 基础填空 (5) 设 $f(x)=\begin{cases}x,&0\leqslant x\leqslant\frac{1}{2},\\ 2(1-x),&\frac{1}{2}<x<1,\end{cases}$ $f(x)$ 的傅里叶级数为 $\dfrac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos n\pi x$，$x\in(-\infty,+\infty)$，其和函数为 $S(x)$，$a_n=2\int_{0}^{1}f(x)\cos n\pi x\,\mathrm{d}x$，则 $S\left(\dfrac{1}{2}\right)=$________，$S(99)=$________．
***
$\dfrac{3}{4}$，$0$．

根据收敛定理，由已知，$f(x)$ 在 $x=\dfrac{1}{2}$ 处间断，故
$$S\left(\frac{1}{2}\right)=\frac{1}{2}\left[f\left(\frac{1}{2}-0\right)+f\left(\frac{1}{2}+0\right)\right]=\frac{\frac{1}{2}+1}{2}=\frac{3}{4}.$$

由已知，可视 $f(x)$ 是以 $2\times1=2$ 为周期的偶函数（作偶延拓），故
$$S(99)=S(99-2\times50)=S(99-100)=S(-1)=S(1)=0.$$

+++

#### 基础解答 (1) 判别下列级数的敛散性：

（Ⅰ）$\sum_{n=1}^{\infty}\dfrac{n^{n+\frac{1}{n}}}{\left(n+\frac{1}{n}\right)^{n}}$；\
（Ⅱ）$\sum_{n=1}^{\infty}\dfrac{a^n}{n^p}\,(a>0,\ p>0)$；\
（Ⅲ）$\sum_{n=1}^{\infty}\dfrac{1}{\int_{0}^{n}\sqrt{1+x^3}\,\mathrm{d}x}$；\
（Ⅳ）$\sum_{n=1}^{\infty}\left(a^{\frac{1}{n}}-a^{\frac{1}{n+1}}\right)(a>0)$；\
（Ⅴ）$\sum_{n=1}^{\infty}\left[\dfrac{1}{n}-\ln\left(1+\dfrac{1}{n}\right)\right]$；\
（Ⅵ）$\sum_{n=1}^{\infty}\left(\sqrt[n]{a}-\sqrt{1+\dfrac{1}{n}}\right)(a>0)$．
***
（Ⅰ）由
$$\lim_{n\to\infty}\frac{n^{n+\frac{1}{n}}}{\left(n+\frac{1}{n}\right)^{n}}=\lim_{n\to\infty}\frac{n^n\cdot\sqrt[n]{n}}{n^n\cdot\left(1+\frac{1}{n^2}\right)^{n}}=1\neq0,$$
故级数发散（根据级数收敛的必要条件）．

（Ⅱ）用比值法，$\lim\limits_{n\to\infty}\dfrac{a^{n+1}}{(n+1)^p}\cdot\dfrac{n^p}{a^n}=a$．

当 $0<a<1$ 时，级数收敛；当 $a>1$ 时，级数发散；当 $a=1$ 时，$\sum_{n=1}^{\infty}\dfrac{1}{n^p}$ 为 $p$ 级数．当 $0<p\leqslant1$ 时，级数发散；当 $p>1$ 时，级数收敛．

（Ⅲ）用比较审敛法，
$$\frac{1}{\int_{0}^{n}\sqrt{1+x^3}\,\mathrm{d}x}<\frac{1}{\int_{0}^{n}\sqrt{x^3}\,\mathrm{d}x}=\frac{1}{\frac{2}{5}n^{\frac{5}{2}}},$$
而 $\sum_{n=1}^{\infty}\dfrac{1}{n^{\frac{5}{2}}}$ 收敛，故级数收敛．

（Ⅳ）$a^{\frac{1}{n}}-a^{\frac{1}{n+1}}=a^{\frac{1}{n+1}}\left(a^{\frac{1}{n}-\frac{1}{n+1}}-1\right)=a^{\frac{1}{n+1}}\left[a^{\frac{1}{n(n+1)}}-1\right]\sim\dfrac{\ln a}{n(n+1)}\sim\dfrac{\ln a}{n^2}\,(n\to\infty)$，而 $\sum_{n=1}^{\infty}\dfrac{\ln a}{n^2}$ 收敛，由比较审敛法，知原级数收敛．

（Ⅴ）由泰勒公式，得
$$\frac{1}{n}-\ln\left(1+\frac{1}{n}\right)=\frac{1}{n}-\left[\frac{1}{n}-\frac{1}{2}\cdot\frac{1}{n^2}+o\left(\frac{1}{n^2}\right)\right]=\frac{1}{2n^2}+o\left(\frac{1}{n^2}\right),$$
即 $\lim\limits_{n\to\infty}\dfrac{\frac{1}{n}-\ln\left(1+\frac{1}{n}\right)}{\frac{1}{2n^2}}=1$，由比较审敛法，知原级数收敛．

【注】比较审敛法的极限形式：设有正项级数 $\sum_{n=1}^{\infty}u_n$，$\sum_{n=1}^{\infty}v_n$．$\lim\limits_{n\to\infty}\dfrac{u_n}{v_n}=l$，则

$0<l<+\infty$，$\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 的敛散性相同；\
$l=0$，当 $\sum_{n=1}^{\infty}v_n$ 收敛时，$\sum_{n=1}^{\infty}u_n$ 也收敛；\
$l=+\infty$，当 $\sum_{n=1}^{\infty}v_n$ 发散时，$\sum_{n=1}^{\infty}u_n$ 也发散．

利用其判别级数的敛散性，关键是找同阶或等价无穷小．

（Ⅵ）由泰勒公式，得
$$\sqrt[n]{a}-\sqrt{1+\frac{1}{n}}=\mathrm{e}^{\frac{\ln a}{n}}-\left(1+\frac{1}{n}\right)^{\frac{1}{2}}$$
$$=1+\frac{1}{n}\ln a+\frac{1}{2}\cdot\frac{1}{n^2}\ln^2a+o\left(\frac{1}{n^2}\right)-\left[1+\frac{1}{2}\cdot\frac{1}{n}+\frac{1}{2}\cdot\frac{1}{2}\cdot\left(-\frac{1}{2}\right)\cdot\frac{1}{n^2}+o\left(\frac{1}{n^2}\right)\right]$$
$$=\left(\ln a-\frac{1}{2}\right)\cdot\frac{1}{n}+\frac{1}{n^2}\left(\frac{1}{2}\ln^2a+\frac{1}{8}\right)+o\left(\frac{1}{n^2}\right).$$

当 $\ln a-\dfrac{1}{2}=0$，即 $a=\sqrt{\mathrm{e}}$ 时，级数收敛；

当 $\ln a-\dfrac{1}{2}\neq0$，即 $a\neq\sqrt{\mathrm{e}}$ 时，级数发散．

+++

#### 基础解答 (2) 判别下列级数的敛散性，若收敛，判断是条件收敛还是绝对收敛：

（Ⅰ）设 $\sum_{n=1}^{\infty}(-1)^{n-1}a_n\mathrm{e}^n$ 收敛，判别 $\sum_{n=1}^{\infty}a_n$ 的敛散性；\
（Ⅱ）$\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{1}{\ln(1+n)}$；\
（Ⅲ）$\sum_{n=1}^{\infty}\dfrac{(-1)^n}{\sqrt{n}-\ln n}$；\
（Ⅳ）$\sum_{n=1}^{\infty}(-1)^{n-1}(\sqrt[n]{3}-1)$．
***
（Ⅰ）由已知条件，知 $\lim\limits_{n\to\infty}(-1)^{n-1}a_n\mathrm{e}^n=0$，即 $\lim\limits_{n\to\infty}a_n\mathrm{e}^n=0$，故当 $n$ 充分大时，
$$|a_n\mathrm{e}^n|\leqslant M\,(M>0),$$
所以 $|a_n|\leqslant\dfrac{M}{\mathrm{e}^n}$，而 $\sum_{n=1}^{\infty}\dfrac{M}{\mathrm{e}^n}$ 收敛，故 $\sum_{n=1}^{\infty}a_n$ 绝对收敛．

（Ⅱ）$\sum_{n=1}^{\infty}\left|(-1)^{n-1}\dfrac{1}{\ln(1+n)}\right|=\sum_{n=1}^{\infty}\dfrac{1}{\ln(1+n)}$，由 $\dfrac{1}{\ln(1+n)}>\dfrac{1}{n}$，而 $\sum_{n=1}^{\infty}\dfrac{1}{n}$ 发散，由比较审敛法，知原级数不绝对收敛．

又 $\lim\limits_{n\to\infty}\dfrac{1}{\ln(1+n)}=0$，$\left\{\dfrac{1}{\ln(1+n)}\right\}$ 单调减少，由莱布尼茨定理，知原级数条件收敛．

（Ⅲ）由 $\dfrac{1}{\sqrt{n}-\ln n}\geqslant\dfrac{1}{\sqrt{n}}$，而 $\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{n}}$ 发散，知 $\sum_{n=1}^{\infty}\dfrac{(-1)^n}{\sqrt{n}-\ln n}$ 不绝对收敛．

令 $f(x)=\dfrac{1}{\sqrt{x}-\ln x}$，则 $\lim\limits_{x\to+\infty}f(x)=\lim\limits_{x\to+\infty}\dfrac{1}{\sqrt{x}-\ln x}=0$，
$$f'(x)=\frac{-\left(\frac{1}{2\sqrt{x}}-\frac{1}{x}\right)}{(\sqrt{x}-\ln x)^2}=\frac{-(\sqrt{x}-2)}{2x(\sqrt{x}-\ln x)^2}<0\ (x>4),$$
故 $\lim\limits_{n\to\infty}\dfrac{1}{\sqrt{n}-\ln n}=0$，且 $\left\{\dfrac{1}{\sqrt{n}-\ln n}\right\}(n>4)$ 单调减少，由莱布尼茨定理，知原级数条件收敛．

（Ⅳ）$\sqrt[n]{3}-1=\mathrm{e}^{\frac{\ln3}{n}}-1\sim\dfrac{\ln3}{n}\,(n\to\infty)$，而 $\sum_{n=1}^{\infty}\dfrac{\ln3}{n}$ 发散，由比较审敛法，知 $\sum_{n=1}^{\infty}(\sqrt[n]{3}-1)$ 发散，即原级数不绝对收敛．

又 $\lim\limits_{n\to\infty}(\sqrt[n]{3}-1)=0$，且 $\{\sqrt[n]{3}-1\}$ 单调减少，由莱布尼茨定理，知原级数条件收敛．

+++

#### 基础解答 (3) 求下列级数的收敛域：

（Ⅰ）$\sum_{n=1}^{\infty}\dfrac{(-1)^nx^n}{2^n\sqrt{n}}$；\
（Ⅱ）$\sum_{n=1}^{\infty}\dfrac{(x-3)^n}{n\cdot3^n}$；\
（Ⅲ）$\sum_{n=1}^{\infty}(-1)^nn^nx^n$；\
（Ⅳ）$\sum_{n=1}^{\infty}\dfrac{x^{2n-1}}{3^n}$．
***
（Ⅰ）利用公式 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\lim\limits_{n\to\infty}\dfrac{2^n\sqrt{n}}{2^{n+1}\sqrt{n+1}}=\dfrac{1}{2}=\rho$，故 $R=\dfrac{1}{\rho}=2$．

当 $x=2$ 时，$\sum_{n=1}^{\infty}\dfrac{(-1)^n2^n}{2^n\sqrt{n}}=\sum_{n=1}^{\infty}\dfrac{(-1)^n}{\sqrt{n}}$ 条件收敛（根据莱布尼茨定理）；

当 $x=-2$ 时，$\sum_{n=1}^{\infty}\dfrac{(-1)^n(-2)^n}{2^n\sqrt{n}}=\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{n}}$ 发散，所以级数的收敛域为 $(-2,2]$．

（Ⅱ）记 $a_n=\dfrac{1}{n3^n}$，$x-3=t$，则 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\lim\limits_{n\to\infty}\dfrac{n3^n}{(n+1)3^{n+1}}=\dfrac{1}{3}$，故级数 $\sum_{n=1}^{\infty}\dfrac{t^n}{n3^n}$ 的收敛半径为 $3$．

当 $|x-3|<3$ 时，即 $0<x<6$，级数收敛．

当 $x=0$ 时，$\sum_{n=1}^{\infty}(-1)^n\dfrac{1}{n}$ 条件收敛；当 $x=6$ 时，$\sum_{n=1}^{\infty}\dfrac{1}{n}$ 发散，故收敛域为 $[0,6)$．

（Ⅲ）$\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\lim\limits_{n\to\infty}\dfrac{(n+1)^{n+1}}{n^n}=\lim\limits_{n\to\infty}(n+1)\left(1+\dfrac{1}{n}\right)^n=+\infty$，故 $R=0$，所以级数仅在 $x=0$ 处收敛．

（Ⅳ）级数 $\sum_{n=1}^{\infty}\dfrac{x^{2n-1}}{3^n}$ 只含 $x$ 的奇次幂项，简称缺项，不能直接利用公式，用比值法，
$$\lim_{n\to\infty}\left|\frac{u_{n+1}(x)}{u_n(x)}\right|=\lim_{n\to\infty}\left|\frac{x^{2(n+1)-1}}{3^{n+1}}\cdot\frac{3^n}{x^{2n-1}}\right|=\frac{x^2}{3}.$$

当 $\dfrac{x^2}{3}<1$ 时，即 $|x|<\sqrt{3}$，级数收敛；当 $\dfrac{x^2}{3}>1$ 时，即 $|x|>\sqrt{3}$，级数发散，故收敛半径为 $R=\sqrt{3}$．

当 $x=\sqrt{3}$ 时，$\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{3}}$ 发散（一般项不趋于 $0$）；

当 $x=-\sqrt{3}$ 时，$\sum_{n=1}^{\infty}\dfrac{-1}{\sqrt{3}}$ 发散，故收敛域为 $(-\sqrt{3},\sqrt{3})$．

+++

#### 基础解答 (4) 求下列级数的收敛域：

（Ⅰ）$\sum_{n=1}^{\infty}\dfrac{x^{n^2}}{2^n}$；\
（Ⅱ）$\sum_{n=1}^{\infty}\dfrac{x^{2n+1}}{3^n+n^2}$；\
（Ⅲ）$\sum_{n=1}^{\infty}\left(1+\dfrac{1}{n}\right)^{-n^2}x^n$；\
（Ⅳ）$\sum_{n=2}^{\infty}\left(\dfrac{1}{n\ln n}+\dfrac{1}{2^n}\right)x^n$．
***
（Ⅰ）缺项，用比值法，
$$\lim_{n\to\infty}\left|\frac{u_{n+1}(x)}{u_n(x)}\right|=\lim_{n\to\infty}\left|\frac{x^{(n+1)^2}}{2^{n+1}}\cdot\frac{2^n}{x^{n^2}}\right|=\lim_{n\to\infty}\frac{|x|^{2n+1}}{2}.$$

当 $|x|<1$ 时，$\lim\limits_{n\to\infty}\dfrac{|x|^{2n+1}}{2}=0<1$，级数收敛；

当 $|x|>1$ 时，$\lim\limits_{n\to\infty}\dfrac{|x|^{2n+1}}{2}=+\infty$，级数发散；

当 $|x|=1$ 时，$\lim\limits_{n\to\infty}\dfrac{|x|^{2n+1}}{2}=\dfrac{1}{2}<1$，级数收敛，故收敛域为 $[-1,1]$．

（Ⅱ）缺项，用比值法，
$$\lim_{n\to\infty}\left|\frac{u_{n+1}(x)}{u_n(x)}\right|=\lim_{n\to\infty}\left|\frac{x^{2(n+1)+1}}{3^{n+1}+(n+1)^2}\cdot\frac{3^n+n^2}{x^{2n+1}}\right|=\lim_{n\to\infty}\frac{3^n+n^2}{3^{n+1}+(n+1)^2}\cdot x^2=\lim_{n\to\infty}\frac{1+\frac{n^2}{3^n}}{1+\frac{(n+1)^2}{3^{n+1}}}\cdot\frac{x^2}{3}=\frac{x^2}{3}.$$

当 $\dfrac{x^2}{3}<1$ 时，即 $-\sqrt{3}<x<\sqrt{3}$，级数收敛．当 $x=\sqrt{3}$ 时，级数为 $\sum_{n=1}^{\infty}\dfrac{3^n\cdot\sqrt{3}}{3^n+n^2}$，由于
$$\lim_{n\to\infty}\frac{3^n\cdot\sqrt{3}}{3^n+n^2}=\lim_{n\to\infty}\frac{\sqrt{3}}{1+\frac{n^2}{3^n}}=\sqrt{3}\neq0,$$
故级数发散，同理 $x=-\sqrt{3}$ 时，级数发散，所以收敛域为 $(-\sqrt{3},\sqrt{3})$．

（Ⅲ）不缺项，用公式，$\lim\limits_{n\to\infty}\sqrt[n]{|a_n|}=\lim\limits_{n\to\infty}\left(1+\dfrac{1}{n}\right)^{-n}=\mathrm{e}^{-1}$，收敛半径 $R=\mathrm{e}$．

当 $x=\mathrm{e}$ 时，级数为 $\sum_{n=1}^{\infty}\left(1+\dfrac{1}{n}\right)^{-n^2}\cdot\mathrm{e}^n$，记 $b_n=\left(1+\dfrac{1}{n}\right)^{-n^2}\mathrm{e}^n=\left[\dfrac{\mathrm{e}}{\left(1+\frac{1}{n}\right)^n}\right]^n$，由于 $\left(1+\dfrac{1}{n}\right)^n<\mathrm{e}$，故 $b_n>1$，即 $\lim\limits_{n\to\infty}b_n\neq0$，所以级数发散，同理 $x=-\mathrm{e}$ 也是发散点，故收敛域为 $(-\mathrm{e},\mathrm{e})$．

（Ⅳ）$\sum_{n=2}^{\infty}\left(\dfrac{1}{n\ln n}+\dfrac{1}{2^n}\right)x^n=\sum_{n=2}^{\infty}\dfrac{x^n}{n\ln n}+\sum_{n=2}^{\infty}\dfrac{x^n}{2^n}$．

对 $\sum_{n=2}^{\infty}\dfrac{x^n}{n\ln n}$，用公式，$\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\lim\limits_{n\to\infty}\dfrac{n\ln n}{(n+1)\ln(n+1)}=1$，收敛半径 $R_1=1$．

当 $x=1$ 时，$\sum_{n=2}^{\infty}\dfrac{1}{n\ln n}$ 发散；当 $x=-1$ 时，$\sum_{n=2}^{\infty}\dfrac{(-1)^n}{n\ln n}$ 是交错级数，且 $\lim\limits_{n\to\infty}\dfrac{1}{n\ln n}=0$，$\left\{\dfrac{1}{n\ln n}\right\}(n\geqslant2)$ 单调减少，故收敛，所以收敛域为 $[-1,1)$．

对 $\sum_{n=2}^{\infty}\dfrac{x^n}{2^n}$，$\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\dfrac{1}{2}$，收敛半径 $R_2=2$．当 $x=\pm2$ 时，级数发散，收敛域为 $(-2,2)$．

综上所述，所求级数收敛域为 $[-1,1)$．

【注】① $\sum_{n=2}^{\infty}\dfrac{1}{n\ln n}$ 用积分判别法：由于 $\int_{2}^{+\infty}\dfrac{\mathrm{d}x}{x\ln x}=\ln(\ln x)\Big|_{2}^{+\infty}=+\infty$，反常积分发散，故级数 $\sum_{n=2}^{\infty}\dfrac{1}{n\ln n}$ 发散．

② 设级数 $\sum_{n=0}^{\infty}a_nx^n$ 与 $\sum_{n=0}^{\infty}b_nx^n$ 的收敛半径分别为 $R_1$ 和 $R_2$，则当 $R_1\neq R_2$ 时，$\sum_{n=0}^{\infty}(a_n+b_n)x^n$ 的收敛半径 $R=\min\{R_1,R_2\}$．

+++

#### 基础解答 (5) 求下列幂级数的收敛域及和函数：

（Ⅰ）$\sum_{n=1}^{\infty}\dfrac{x^{n-1}}{n2^n}$；\
（Ⅱ）$\sum_{n=0}^{\infty}\dfrac{(n-1)^2}{n+1}x^n$；\
（Ⅲ）$\sum_{n=0}^{\infty}\dfrac{n^2+1}{n!}x^n$；\
（Ⅳ）$\sum_{n=0}^{\infty}\dfrac{(-1)^n(n+1)}{(2n+3)!}x^{2n}$．
***
（Ⅰ）易求得 $\sum_{n=1}^{\infty}\dfrac{x^{n-1}}{n2^n}$ 的收敛半径 $R=2$，收敛域为 $[-2,2)$．

令 $S(x)=\sum_{n=1}^{\infty}\dfrac{x^{n-1}}{n2^n}$，则 $xS(x)=\sum_{n=1}^{\infty}\dfrac{x^n}{n2^n}$，
$$[xS(x)]'=\left[\sum_{n=1}^{\infty}\frac{1}{n}\left(\frac{x}{2}\right)^n\right]'=\sum_{n=1}^{\infty}\left[\frac{1}{n}\left(\frac{x}{2}\right)^n\right]'=\frac{1}{2}\sum_{n=1}^{\infty}\left(\frac{x}{2}\right)^{n-1}=\frac{1}{2}\cdot\frac{1}{1-\frac{x}{2}}=\frac{1}{2-x},$$
两边同时积分，得 $xS(x)-0\cdot S(0)=\int_{0}^{x}\dfrac{\mathrm{d}t}{2-t}=-\ln(2-x)+\ln2$．

当 $x\neq0$ 时，$S(x)=-\dfrac{1}{x}\ln\left(1-\dfrac{x}{2}\right)$；当 $x=0$ 时，$S(0)=\dfrac{1}{2}$，故
$$S(x)=\begin{cases}-\dfrac{1}{x}\ln\left(1-\dfrac{x}{2}\right),&-2\leqslant x<0,\ 0<x<2,\\[2mm]\dfrac{1}{2},&x=0.\end{cases}$$

（Ⅱ）先求收敛半径，用公式
$$\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=\lim_{n\to\infty}\frac{(n+1-1)^2}{n+1+1}\cdot\frac{n+1}{(n-1)^2}=1,$$
故收敛半径 $R=1$，当 $x=\pm1$ 时，由于一般式不趋于零，所以发散，故收敛域为 $(-1,1)$．

令 $S(x)=\sum_{n=0}^{\infty}\dfrac{(n-1)^2}{n+1}x^n=\sum_{n=0}^{\infty}\dfrac{(n+1-2)^2}{n+1}x^n=\sum_{n=0}^{\infty}(n+1)x^n-4\sum_{n=0}^{\infty}x^n+4\sum_{n=0}^{\infty}\dfrac{x^n}{n+1}$，

记 $S_1(x)=\sum_{n=0}^{\infty}(n+1)x^n$，$S_2(x)=4\sum_{n=0}^{\infty}x^n$，$S_3=4\sum_{n=0}^{\infty}\dfrac{x^n}{n+1}$，
$$S_1(x)=\sum_{n=0}^{\infty}(x^{n+1})'=\left(\sum_{n=0}^{\infty}x^{n+1}\right)'=\left(\frac{x}{1-x}\right)'=\frac{1}{(1-x)^2},\ |x|<1,$$
$$S_2(x)=4\sum_{n=0}^{\infty}x^n=\frac{4}{1-x},\ |x|<1,\qquad xS_3(x)=4\sum_{n=0}^{\infty}\frac{x^{n+1}}{n+1},$$
则 $[xS_3(x)]'=4\sum_{n=0}^{\infty}x^n=\dfrac{4}{1-x}$，积分得 $xS_3(x)-0=-4\ln(1-x)\ (-1<x<1)$，故
$$S(x)=S_1(x)-S_2(x)+S_3(x)=\frac{1}{(1-x)^2}-\frac{4}{1-x}-\frac{4}{x}\ln(1-x)=\frac{4x-3}{(1-x)^2}-\frac{4}{x}\ln(1-x)\ (|x|<1\ \text{且}\ x\neq0).$$

当 $x=0$ 时，$S(0)=1$．

（Ⅲ）由 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=0$，知收敛半径 $R=+\infty$，故收敛域为 $(-\infty,+\infty)$．

令 $S(x)=\sum_{n=0}^{\infty}\dfrac{n^2+1}{n!}x^n$，则
$$S(x)=\sum_{n=0}^{\infty}\frac{n^2}{n!}x^n+\sum_{n=0}^{\infty}\frac{x^n}{n!}=\sum_{n=1}^{\infty}\frac{n}{(n-1)!}x^n+\mathrm{e}^x=\sum_{n=1}^{\infty}\frac{n-1+1}{(n-1)!}x^n+\mathrm{e}^x$$
$$=\sum_{n=2}^{\infty}\frac{x^n}{(n-2)!}+\sum_{n=1}^{\infty}\frac{x^n}{(n-1)!}+\mathrm{e}^x=x^2\sum_{n=2}^{\infty}\frac{x^{n-2}}{(n-2)!}+x\sum_{n=1}^{\infty}\frac{x^{n-1}}{(n-1)!}+\mathrm{e}^x=x^2\mathrm{e}^x+x\mathrm{e}^x+\mathrm{e}^x,\ x\in(-\infty,+\infty).$$

【注】$\sum_{n=0}^{\infty}\dfrac{x^n}{n!}=\mathrm{e}^x$，$x\in(-\infty,+\infty)$．

（Ⅳ）级数 $\sum_{n=0}^{\infty}\dfrac{(-1)^n(n+1)}{(2n+3)!}x^{2n}$ 缺项，用比值法，
$$\lim_{n\to\infty}\left|\frac{u_{n+1}(x)}{u_n(x)}\right|=\lim_{n\to\infty}\left|\frac{(-1)^{n+1}(n+2)x^{2(n+1)}}{[2(n+1)+3]!}\cdot\frac{(2n+3)!}{(-1)^n(n+1)x^{2n}}\right|=\lim_{n\to\infty}\frac{x^2}{2(n+1)(2n+5)}=0\ (\text{对任意}\ x),$$
故收敛域为 $(-\infty,+\infty)$．考虑到分母为 $(2n+3)!$，用 $\sin x$ 的展开式，
$$\sin x=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+1)!}x^{2n+1}=x-\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+3)!}x^{2n+3},$$
故 $\sum_{n=0}^{\infty}\dfrac{(-1)^n}{(2n+3)!}x^{2n+3}=x-\sin x$，即 $\sum_{n=0}^{\infty}\dfrac{(-1)^n}{(2n+3)!}x^{2n+2}=1-\dfrac{\sin x}{x}\ (x\neq0)$，

上式两边同时对 $x$ 求导，得 $\sum_{n=0}^{\infty}\dfrac{2(n+1)(-1)^n}{(2n+3)!}x^{2n+1}=-\dfrac{1}{x^2}(x\cos x-\sin x)$，故
$$S(x)=\sum_{n=0}^{\infty}\frac{(-1)^n(n+1)}{(2n+3)!}x^{2n}=\frac{1}{2x^3}(\sin x-x\cos x),\ x\neq0,$$
当 $x=0$ 时，$S(0)=\dfrac{1}{6}$，所以
$$S(x)=\begin{cases}\dfrac{1}{2x^3}(\sin x-x\cos x),&x\neq0,\\[2mm]\dfrac{1}{6},&x=0.\end{cases}$$

+++

#### 基础解答 (6) 将下列函数展开为 $x$ 的幂级数，并确定收敛域：

（Ⅰ）$f_1(x)=\dfrac{1}{x^2-3x+2}$；\
（Ⅱ）$f_2(x)=\ln(1-x-2x^2)$；\
（Ⅲ）$f_3(x)=\ln(x+\sqrt{1+x^2})$；\
（Ⅳ）$f_4(x)=x\arctan x-\ln\sqrt{1+x^2}$．
***
（Ⅰ）$f_1(x)=\dfrac{1}{x^2-3x+2}=\dfrac{1}{(1-x)(2-x)}=\dfrac{1}{1-x}-\dfrac{1}{2-x}$，由于 $\dfrac{1}{1-x}=\sum_{n=0}^{\infty}x^n$，$|x|<1$，则
$$\frac{1}{2-x}=\frac{1}{2}\cdot\frac{1}{1-\frac{x}{2}}=\frac{1}{2}\sum_{n=0}^{\infty}\left(\frac{x}{2}\right)^n=\sum_{n=0}^{\infty}\frac{x^n}{2^{n+1}},\ |x|<2,$$
所以 $f_1(x)=\dfrac{1}{1-x}-\dfrac{1}{2-x}=\sum_{n=0}^{\infty}\left(1-\dfrac{1}{2^{n+1}}\right)x^n$，$x\in(-1,1)$．

（Ⅱ）由 $\ln(1-x-2x^2)=\ln[(1-2x)(1+x)]=\ln(1+x)+\ln(1-2x)$，且
$$\ln(1+x)=\sum_{n=1}^{\infty}(-1)^{n+1}\frac{x^n}{n},\ -1<x\leqslant1,$$
$$\ln(1-2x)=\sum_{n=1}^{\infty}(-1)^{n+1}\frac{(-2x)^n}{n}=-\sum_{n=1}^{\infty}\frac{2^nx^n}{n}\ \left(-\frac{1}{2}\leqslant x<\frac{1}{2}\right),$$
故 $f_2(x)=\ln(1-x-2x^2)=\sum_{n=1}^{\infty}\dfrac{(-1)^{n+1}-2^n}{n}x^n$，$x\in\left[-\dfrac{1}{2},\dfrac{1}{2}\right)$．

（Ⅲ）由 $f_3(x)=\ln(x+\sqrt{1+x^2})$，得 $f_3'(x)=\dfrac{1+\frac{2x}{2\sqrt{1+x^2}}}{x+\sqrt{1+x^2}}=\dfrac{1}{\sqrt{1+x^2}}$，而
$$\frac{1}{\sqrt{1+x^2}}=1-\frac{1}{2}x^2+\frac{1\times3}{2\times4}x^4-\frac{1\times3\times5}{2\times4\times6}x^6+\cdots\ (-1\leqslant x\leqslant1),$$
故
$$\ln(x+\sqrt{1+x^2})=\int_{0}^{x}f_3'(t)\,\mathrm{d}t+f_3(0)=x-\frac{1}{2\times3}x^3+\frac{1\times3}{2\times4\times5}x^5-\frac{1\times3\times5}{2\times4\times6\times7}x^7+\cdots$$
$$=x+\sum_{n=1}^{\infty}(-1)^n\frac{(2n-1)!!}{n!\,2^n(2n+1)}x^{2n+1},\ |x|\leqslant1.$$

【注】由 $f_3(x)-f_3(0)=\int_{0}^{x}f_3'(t)\,\mathrm{d}t$，其中 $f_3(0)=0$，知 $f_3(x)=f_3(0)+\int_{0}^{x}f_3'(t)\,\mathrm{d}t$．

（Ⅳ）$f_4(x)=x\arctan x-\ln\sqrt{1+x^2}=\int_{0}^{x}\arctan t\,\mathrm{d}t$，而
$$\arctan t=t-\frac{1}{3}t^3+\frac{1}{5}t^5-\frac{1}{7}t^7+\cdots+\frac{(-1)^n}{2n+1}t^{2n+1}+\cdots,\ |t|\leqslant1,$$
故
$$f_4(x)=\frac{1}{2}x^2-\frac{1}{3\times4}x^4+\frac{1}{5\times6}x^6-\frac{1}{7\times8}x^8+\cdots+\frac{(-1)^n}{(2n+1)(2n+2)}x^{2n+2}+\cdots,\ |x|\leqslant1.$$

【注】此题也可以分别将 $x\arctan x$ 和 $\ln\sqrt{1+x^2}$ 展开为 $x$ 的幂级数．
$$\ln\sqrt{1+x^2}=\frac{1}{2}\ln(1+x^2)=\frac{1}{2}\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+2}}{n+1}=\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+2}}{2n+2},\ |x|\leqslant1,$$
$$(\arctan x)'=\frac{1}{1+x^2}=\sum_{n=0}^{\infty}(-1)^nx^{2n},$$
积分得 $\int_{0}^{x}(\arctan t)'\,\mathrm{d}t=\arctan x-\arctan0=\sum_{n=0}^{\infty}(-1)^n\dfrac{x^{2n+1}}{2n+1}$，故 $x\arctan x=\sum_{n=0}^{\infty}(-1)^n\dfrac{x^{2n+2}}{2n+1}$，$|x|\leqslant1$，所以
$$x\arctan x-\ln\sqrt{1+x^2}=\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+2}}{2n+1}-\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+2}}{2n+2}=\sum_{n=0}^{\infty}(-1)^n\left(\frac{1}{2n+1}-\frac{1}{2n+2}\right)x^{2n+2}=\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+2}}{(2n+1)(2n+2)},\ |x|\leqslant1.$$

+++

#### 基础解答 (7) 将 $f(x)=\dfrac{x}{x^2-5x+6}$ 展开为 $x-5$ 的幂级数．
***
$$f(x)=\frac{x}{x^2-5x+6}=\frac{3}{x-3}-\frac{2}{x-2}=\frac{3}{2+(x-5)}-\frac{2}{3+(x-5)}$$
$$=\frac{3}{2}\cdot\frac{1}{1+\frac{1}{2}(x-5)}-\frac{2}{3}\cdot\frac{1}{1+\frac{1}{3}(x-5)}=\frac{3}{2}\sum_{n=0}^{\infty}(-1)^n\left(\frac{x-5}{2}\right)^n-\frac{2}{3}\sum_{n=0}^{\infty}(-1)^n\left(\frac{x-5}{3}\right)^n$$
$$=\sum_{n=0}^{\infty}(-1)^n\left(\frac{3}{2^{n+1}}-\frac{2}{3^{n+1}}\right)(x-5)^n,$$
收敛域取 $-1<\dfrac{x-5}{2}<1$ 与 $-1<\dfrac{x-5}{3}<1$ 的交集，即 $3<x<7$．

+++

#### 基础解答 (8) 将 $f(x)=\sin\dfrac{\pi}{2}x$ 在 $x=-2$ 处进行幂级数展开．
***
$$f(x)=\sin\frac{\pi}{2}x=\sin\frac{\pi}{2}(x+2-2)=-\sin\left[\pi-\frac{\pi}{2}(x+2)\right]=-\sin\frac{\pi}{2}(x+2)$$
$$=-\sum_{n=0}^{\infty}(-1)^n\frac{1}{(2n+1)!}\left[\frac{\pi}{2}(x+2)\right]^{2n+1}=\sum_{n=0}^{\infty}\frac{(-1)^{n+1}}{(2n+1)!}\left(\frac{\pi}{2}\right)^{2n+1}(x+2)^{2n+1}\ (-\infty<x<+\infty).$$

【注】将函数 $f(x)$ 展开为幂级数，常用两种方法：

① 直接法：求泰勒系数 $a_n=\dfrac{f^{(n)}(x_0)}{n!}$，证明余项 $R_n(x)=\dfrac{f^{(n+1)}(\xi)}{(n+1)!}(x-x_0)^{n+1}$ 的极限 $\lim\limits_{n\to\infty}R_n(x)=0$，则
$$f(x)=f(x_0)+\frac{f'(x_0)}{1!}(x-x_0)+\cdots+\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n+\cdots,\ x\in(a,b),$$
其中 $(a,b)$ 为级数的收敛域．

② 间接法：利用函数展开为幂级数的唯一性和常用函数的幂级数，借助于幂级数的四则运算、逐项求导、逐项积分以及变量代换等方法，求得函数的幂级数展开式．

一般简单函数采用直接法．

+++

#### 基础解答 (9) 求下列级数的和：

（Ⅰ）$\sum_{n=2}^{\infty}\dfrac{1}{(n^2-1)2^n}$；\
（Ⅱ）$\sum_{n=0}^{\infty}\dfrac{2n+1}{n!}$．
***
（Ⅰ）所求级数的和为幂级数 $\sum_{n=2}^{\infty}\dfrac{x^n}{n^2-1}$ 的和函数 $S(x)$ 在 $x=\dfrac{1}{2}$ 处的值．

令 $S(x)=\sum_{n=2}^{\infty}\dfrac{x^n}{n^2-1}\ (|x|<1)$，则
$$S(x)=\sum_{n=2}^{\infty}\frac{1}{2}\left(\frac{1}{n-1}-\frac{1}{n+1}\right)x^n=\frac{1}{2}x\left(\sum_{n=2}^{\infty}\frac{x^{n-1}}{n-1}-\frac{1}{x}\sum_{n=2}^{\infty}\frac{x^n}{n+1}\right)(x\neq0),$$
而 $\sum_{n=2}^{\infty}\dfrac{x^{n-1}}{n-1}=\sum_{n=1}^{\infty}\dfrac{x^n}{n}$，$\dfrac{1}{x^2}\sum_{n=2}^{\infty}\dfrac{x^{n+1}}{n+1}=\dfrac{1}{x^2}\sum_{n=3}^{\infty}\dfrac{x^n}{n}\ (x\neq0)$，

令 $g(x)=\sum_{n=1}^{\infty}\dfrac{x^n}{n}$，则 $g'(x)=\sum_{n=1}^{\infty}x^{n-1}=\dfrac{1}{1-x}$，$|x|<1$，故
$$g(x)=g(x)-g(0)=\int_{0}^{x}g'(t)\,\mathrm{d}t=\int_{0}^{x}\frac{\mathrm{d}t}{1-t}=-\ln(1-x),$$
从而
$$S(x)=\frac{x}{2}\left\{-\ln(1-x)-\frac{1}{x^2}\left[-\ln(1-x)-x-\frac{x^2}{2}\right]\right\}=\frac{x+2}{4}+\frac{1-x^2}{2x}\ln(1-x),\ |x|<1,\ x\neq0,$$
故 $\sum_{n=2}^{\infty}\dfrac{1}{(n^2-1)2^n}=S\left(\dfrac{1}{2}\right)=\dfrac{5}{8}-\dfrac{3}{4}\ln2$．

【注】也可将 $\sum_{n=1}^{\infty}\dfrac{x^n}{n}=-\ln(1-x)$，$|x|<1$ 视为常用结果．

（Ⅱ）构造幂级数，令 $S(x)=\sum_{n=0}^{\infty}\dfrac{2n+1}{n!}x^{2n}$，易求得其收敛域为 $(-\infty,+\infty)$，则
$$S(x)=\sum_{n=0}^{\infty}\left(\frac{x^{2n+1}}{n!}\right)'=\left(\sum_{n=0}^{\infty}\frac{x^{2n+1}}{n!}\right)'=\left[x\sum_{n=0}^{\infty}\frac{(x^2)^n}{n!}\right]'=(x\cdot\mathrm{e}^{x^2})'=(1+2x^2)\mathrm{e}^{x^2},\ x\in(-\infty,+\infty),$$
故 $\sum_{n=0}^{\infty}\dfrac{2n+1}{n!}=S(1)=3\mathrm{e}$．

+++

#### 基础解答 (10) （Ⅰ）证明：$y(x)=1+\dfrac{x^3}{3!}+\dfrac{x^6}{6!}+\dfrac{x^9}{9!}+\cdots+\dfrac{x^{3n}}{(3n)!}+\cdots\ (-\infty<x<+\infty)$ 满足微分方程 $y''+y'+y=\mathrm{e}^x$；

（Ⅱ）利用（Ⅰ）的结果求 $\sum_{n=0}^{\infty}\dfrac{x^{3n}}{(3n)!}$．
***
（Ⅰ）
$$y(x)=1+\frac{x^3}{3!}+\frac{x^6}{6!}+\frac{x^9}{9!}+\cdots+\frac{x^{3n}}{(3n)!}+\cdots,$$
$$y'(x)=\frac{x^2}{2!}+\frac{x^5}{5!}+\frac{x^8}{8!}+\cdots+\frac{x^{3n-1}}{(3n-1)!}+\cdots,$$
$$y''(x)=x+\frac{x^4}{4!}+\frac{x^7}{7!}+\cdots+\frac{x^{3n-2}}{(3n-2)!}+\cdots,$$
故 $y''+y'+y=\sum_{n=0}^{\infty}\dfrac{x^n}{n!}=\mathrm{e}^x$．

（Ⅱ）由（Ⅰ），解初值问题：
$$\begin{cases}y''+y'+y=\mathrm{e}^x,\\ y(0)=1,\ y'(0)=0,\end{cases}$$
可得 $y(x)=\dfrac{2}{3}\mathrm{e}^{-\frac{x}{2}}\cos\dfrac{\sqrt{3}}{2}x+\dfrac{1}{3}\mathrm{e}^x$ 为所求和函数．

+++

#### 基础解答 (11) 将 $f(x)=1-x^2\ (0\leqslant x\leqslant\pi)$ 展开为余弦级数，并求 $\sum_{n=1}^{\infty}\dfrac{(-1)^{n-1}}{n^2}$．
***
依题意，$b_n=0$，且
$$a_n=\frac{2}{\pi}\int_{0}^{\pi}f(x)\cos nx\,\mathrm{d}x=\frac{2}{\pi}\left[\int_{0}^{\pi}\cos nx\,\mathrm{d}x-\int_{0}^{\pi}x^2\cos nx\,\mathrm{d}x\right]$$
$$=\frac{2}{\pi}\left[0-\frac{1}{n}\int_{0}^{\pi}x^2\,\mathrm{d}(\sin nx)\right]=-\frac{2}{n\pi}\left[x^2\sin nx\Big|_{0}^{\pi}-\int_{0}^{\pi}2x\sin nx\,\mathrm{d}x\right]=-\frac{4}{n^2\pi}\int_{0}^{\pi}x\,\mathrm{d}(\cos nx)$$
$$=-\frac{4}{n^2\pi}\left[x\cos nx\Big|_{0}^{\pi}-\int_{0}^{\pi}\cos nx\,\mathrm{d}x\right]=-\frac{4}{n^2\pi}\cdot\pi\cdot(-1)^n=\frac{(-1)^{n+1}\cdot4}{n^2},$$
$$a_0=\frac{2}{\pi}\int_{0}^{\pi}(1-x^2)\,\mathrm{d}x=2\left(1-\frac{\pi^2}{3}\right).$$

由 $f(x)$ 在 $[0,\pi]$ 上连续，根据收敛定理，有
$$f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos nx=1-\frac{\pi^2}{3}+\sum_{n=1}^{\infty}\frac{(-1)^{n+1}\cdot4}{n^2}\cos nx.$$

当 $x=0$ 时，$f(0)=1-\dfrac{\pi^2}{3}+\sum_{n=1}^{\infty}\dfrac{4\cdot(-1)^{n+1}}{n^2}$，故 $\sum_{n=1}^{\infty}\dfrac{(-1)^{n-1}}{n^2}=\dfrac{\pi^2}{12}$．

+++

#### 基础解答 (12) 将 $f(x)=\begin{cases}1,&1<x<2,\\ 3-x,&2\leqslant x\leqslant3\end{cases}$ 展开为以 $2$ 为周期的傅里叶级数．
***
$$a_0=\frac{1}{1}\int_{1}^{3}f(x)\,\mathrm{d}x=\int_{1}^{2}\mathrm{d}x+\int_{2}^{3}(3-x)\,\mathrm{d}x=\frac{3}{2},$$
$$a_n=\frac{1}{1}\int_{1}^{3}f(x)\cos\frac{n\pi x}{1}\,\mathrm{d}x=\int_{1}^{2}\cos n\pi x\,\mathrm{d}x+\int_{2}^{3}(3-x)\cos n\pi x\,\mathrm{d}x=\frac{1}{n^2\pi^2}[1-(-1)^n]=\begin{cases}0,&n\ \text{为偶数},\\[1mm]\dfrac{2}{n^2\pi^2},&n\ \text{为奇数},\end{cases}$$
$$b_n=\frac{1}{1}\int_{1}^{3}f(x)\sin\frac{n\pi x}{1}\,\mathrm{d}x=\int_{1}^{2}\sin n\pi x\,\mathrm{d}x+\int_{2}^{3}(3-x)\sin n\pi x\,\mathrm{d}x=\frac{(-1)^n}{n\pi},$$
故
$$f(x)\sim\frac{a_0}{2}+\sum_{n=1}^{\infty}\left(a_n\cos\frac{n\pi x}{l}+b_n\sin\frac{n\pi x}{l}\right)=\frac{3}{4}+\frac{2}{\pi^2}\sum_{n=1}^{\infty}\frac{\cos(2n-1)\pi x}{(2n-1)^2}+\frac{1}{\pi}\sum_{n=1}^{\infty}(-1)^n\frac{1}{n}\sin n\pi x,$$
由收敛定理，其和函数为
$$S(x)=\begin{cases}1,&1<x\leqslant2,\\ 3-x,&2<x<3,\\[1mm]\dfrac{1}{2},&x=1,\ x=3.\end{cases}$$

+++

#### 综合选择 (1) 级数 $\sum_{n=1}^{\infty}\left[(-1)^n\ln\left(1+\dfrac{1}{\sqrt{n}}\right)+\dfrac{\sin kn\pi}{n^2}\right]$（$k$ 为常数）（　）。

;;;
A. 条件收敛
B. 绝对收敛
C. 发散
D. 敛散性与 $k$ 有关
;;;A
***
由 $\left|\dfrac{\sin kn\pi}{n^2}\right|\leqslant\dfrac{1}{n^2}$，知 $\sum_{n=1}^{\infty}\dfrac{\sin kn\pi}{n^2}$ **绝对收敛**。

由
$$\left|(-1)^n\ln\left(1+\frac{1}{\sqrt{n}}\right)\right|=\ln\left(1+\frac{1}{\sqrt{n}}\right)\sim\frac{1}{\sqrt{n}},$$
而 $\sum_{n=1}^{\infty}\dfrac{1}{\sqrt{n}}$ 发散，知 $\sum_{n=1}^{\infty}(-1)^n\ln\left(1+\dfrac{1}{\sqrt{n}}\right)$ 不绝对收敛。

而 $\lim\limits_{n\to\infty}\ln\left(1+\dfrac{1}{\sqrt{n}}\right)=0$，且 $\left\{\ln\left(1+\dfrac{1}{\sqrt{n}}\right)\right\}$ 单调减少，由交错级数的莱布尼茨定理，知 $\sum_{n=1}^{\infty}(-1)^n\ln\left(1+\dfrac{1}{\sqrt{n}}\right)$ 条件收敛，所以原级数**条件收敛**，A 正确。

+++

#### 综合选择 (2) 设 $a>0$，$\sum_{n=1}^{\infty}\dfrac{a^n n!}{n^n}$ 收敛，$\sum_{n=2}^{\infty}\dfrac{\sqrt{n+2}-\sqrt{n-2}}{n^a}$ 发散，则（　）。

;;;
A. $a>\mathrm{e}$
B. $a=\mathrm{e}$
C. $\dfrac{1}{2}<a<\mathrm{e}$
D. $0<a\leqslant\dfrac{1}{2}$
;;;D
***
记 $u_n=\dfrac{a^n n!}{n^n}$，用比值法，
$$\lim_{n\to\infty}\frac{u_{n+1}}{u_n}=\lim_{n\to\infty}\frac{a^{n+1}(n+1)!}{(n+1)^{n+1}}\cdot\frac{n^n}{a^n n!}=\lim_{n\to\infty}\frac{a}{\left(1+\frac{1}{n}\right)^n}=\frac{a}{\mathrm{e}},$$
则级数 $\sum_{n=1}^{\infty}\dfrac{a^n n!}{n^n}$ 当 $a<\mathrm{e}$ 时收敛，当 $a>\mathrm{e}$ 时发散，当 $a=\mathrm{e}$ 时，比值法失效。

又由 $\left(1+\dfrac{1}{n}\right)^n<\mathrm{e}$，知 $\dfrac{u_{n+1}}{u_n}>1$，故 $\lim\limits_{n\to\infty}u_n\neq0$，从而当 $a=\mathrm{e}$ 时级数发散。

$$\frac{\sqrt{n+2}-\sqrt{n-2}}{n^a}=\frac{4}{n^a\left(\sqrt{n+2}+\sqrt{n-2}\right)}=\frac{4}{n^{a+\frac{1}{2}}\left(\sqrt{1+\frac{2}{n}}+\sqrt{1-\frac{2}{n}}\right)},$$
即 $\dfrac{\sqrt{n+2}-\sqrt{n-2}}{n^a}\sim\dfrac{2}{n^{a+\frac{1}{2}}}\ (n\to\infty)$。而 $\sum_{n=1}^{\infty}\dfrac{2}{n^{a+\frac{1}{2}}}$ 当 $0<a+\dfrac{1}{2}\leqslant1$ 时发散，由 $0<a+\dfrac{1}{2}\leqslant1$ 与 $a<\mathrm{e}$ 及 $a>0$（已知），得 $0<a\leqslant\dfrac{1}{2}$，故 D 正确。

【注】常见不等式：$\left(1+\dfrac{1}{n}\right)^n<\mathrm{e}<\left(1+\dfrac{1}{n}\right)^{n+1}$（$n$ 为正整数）。

+++

#### 综合选择 (3) 设 $u_n=\dfrac{|a_n|+a_n}{2}$，$v_n=\dfrac{|a_n|-a_n}{2}$，则下列四个级数

（Ⅰ）$\sum_{n=1}^{\infty}a_n$\
（Ⅱ）$\sum_{n=1}^{\infty}|a_n|$\
（Ⅲ）$\sum_{n=1}^{\infty}u_n$\
（Ⅳ）$\sum_{n=1}^{\infty}v_n$

的收敛性关系是（　）。

;;;
A. 若（Ⅰ）收敛，则（Ⅲ）和（Ⅳ）都收敛
B. 若（Ⅱ）收敛，则（Ⅰ）、（Ⅲ）和（Ⅳ）都收敛
C. 若（Ⅲ）和（Ⅳ）发散，则（Ⅰ）和（Ⅱ）都发散
D. （Ⅰ）（Ⅱ）（Ⅲ）（Ⅳ）的收敛性无确定的关系
;;;B
***
若 $\sum_{n=1}^{\infty}|a_n|$ 收敛，则 $\sum_{n=1}^{\infty}a_n$ 收敛。由
$$0\leqslant u_n=\frac{|a_n|+a_n}{2}\leqslant|a_n|,\qquad 0\leqslant v_n=\frac{|a_n|-a_n}{2}\leqslant|a_n|,$$
由比较审敛法，知 $\sum_{n=1}^{\infty}u_n$ 与 $\sum_{n=1}^{\infty}v_n$ 都收敛。

+++

#### 综合选择 (4) 设有两个数列 $\{a_n\}$ 与 $\{b_n\}$，若 $\lim\limits_{n\to\infty}b_n=0$，则（　）。

;;;
A. 当 $\sum_{n=1}^{\infty}a_n$ 收敛时，$\sum_{n=1}^{\infty}a_nb_n$ 收敛
B. 当 $\sum_{n=1}^{\infty}|a_n|$ 收敛时，$\sum_{n=1}^{\infty}a_nb_n$ 收敛
C. 当 $\sum_{n=1}^{\infty}a_n$ 发散时，$\sum_{n=1}^{\infty}a_nb_n$ 发散
D. 当 $\sum_{n=1}^{\infty}|a_n|$ 发散时，$\sum_{n=1}^{\infty}a_n^2b_n^2$ 发散
;;;B
***
对于 B：由 $\lim\limits_{n\to\infty}b_n=0$，知 $\{b_n\}$ 有界，即存在 $M>0$，使得 $|b_n|\leqslant M$，故 $|a_nb_n|\leqslant M|a_n|$。又因为 $\sum_{n=1}^{\infty}|a_n|$ 收敛，所以由比较审敛法，知 $\sum_{n=1}^{\infty}|a_nb_n|$ 收敛，故 $\sum_{n=1}^{\infty}a_nb_n$ 收敛，B 正确。

对于 A：若取 $a_n=b_n=\dfrac{(-1)^n}{\sqrt{n}}$，则 $\sum_{n=1}^{\infty}a_n$ 收敛，$\lim\limits_{n\to\infty}b_n=0$，但 $\sum_{n=1}^{\infty}a_nb_n=\sum_{n=1}^{\infty}\dfrac{1}{n}$ 发散，排除 A。

对于 C、D：若取 $a_n=b_n=\dfrac{1}{n}$，则可排除 C、D。

+++

#### 综合选择 (5) 判别级数 $\dfrac{1}{\sqrt{2}-1}-\dfrac{1}{\sqrt{2}+1}+\dfrac{1}{\sqrt{3}-1}-\dfrac{1}{\sqrt{3}+1}+\cdots+\dfrac{1}{\sqrt{n}-1}-\dfrac{1}{\sqrt{n}+1}+\cdots$ 的敛散性，正确的结论是（　）。

;;;
A. 由莱布尼茨定理，可推得该级数收敛
B. 由于添加括号后级数发散，故原级数发散
C. 由于各项取绝对值后得到的级数发散，故原级数发散
D. 由 $\lim\limits_{n\to\infty}\dfrac{1}{\sqrt{n}-1}=0$，可知原级数收敛
;;;B
***
对于 B：由级数的性质，知 $\sum_{n=1}^{\infty}a_n$ 收敛 $\Rightarrow$ 添加括号后仍收敛。其逆否命题成立，即添加括号后的级数发散，原级数也发散，故 B 正确。

对于 A：级数一般项不单调，不能用莱布尼茨定理，排除 A。

对于 C：$\sum_{n=1}^{\infty}|a_n|$ 收敛 $\Rightarrow$ $\sum_{n=1}^{\infty}a_n$ 收敛，但 $\sum_{n=1}^{\infty}|a_n|$ 发散时 $\sum_{n=1}^{\infty}a_n$ 可能条件收敛，不一定有 $\sum_{n=1}^{\infty}a_n$ 发散，排除 C。

对于 D：$\lim\limits_{n\to\infty}a_n=0$ 是 $\sum_{n=1}^{\infty}a_n$ 收敛的必要条件，不是充分条件，排除 D。

+++

#### 综合选择 (6) $\sum_{n=0}^{\infty}(-1)^n\dfrac{n+1}{(2n+1)!}=$（　）。

;;;
A. $\dfrac{1}{2}(\sin 1+\cos 1)$
B. $2\sin 1+\cos 1$
C. $\sin 1+2\cos 1$
D. $\sin 1+\cos 1$
;;;A
***
$$\sum_{n=0}^{\infty}(-1)^n\frac{n+1}{(2n+1)!}=\frac{1}{2}\sum_{n=0}^{\infty}(-1)^n\frac{2(n+1)}{(2n+1)!}$$
$$=\frac{1}{2}\left[\sum_{n=0}^{\infty}(-1)^n\frac{1}{(2n+1)!}+\sum_{n=0}^{\infty}(-1)^n\frac{2n+1}{(2n+1)!}\right]$$
$$=\frac{1}{2}\left[\sum_{n=0}^{\infty}(-1)^n\frac{1}{(2n+1)!}+\sum_{n=0}^{\infty}(-1)^n\frac{1}{(2n)!}\right]=\frac{1}{2}(\sin 1+\cos 1).$$

【注】$\sin x=\sum_{n=0}^{\infty}(-1)^n\dfrac{x^{2n+1}}{(2n+1)!}$，$\cos x=\sum_{n=0}^{\infty}(-1)^n\dfrac{x^{2n}}{(2n)!}$。

+++

#### 综合选择 (7) 设级数 $\sum_{n=2}^{\infty}\dfrac{1}{n\ln^p n}$ 与 $\int_0^{+\infty}\mathrm{e}^{(p^2-4)x}\mathrm{d}x$ 都收敛，则（　）。

;;;
A. $1<p<2$
B. $0<p<2$
C. $-2<p<2$
D. $1\leqslant p<2$
;;;A
***
令 $f(x)=\dfrac{1}{x\ln^p x}$，$x\in[2,+\infty)$，则 $f(x)$ 单调减少且非负，用积分判别法，可知
$$\int_2^{+\infty}\frac{\mathrm{d}x}{x\ln^p x}=\begin{cases}+\infty, & \text{发散},\ p\leqslant1,\\[4pt] \dfrac{1}{(p-1)\ln^{p-1}2}, & \text{收敛},\ p>1.\end{cases}$$
$$\int_0^{+\infty}\mathrm{e}^{(p^2-4)x}\mathrm{d}x=\frac{1}{p^2-4}\int_0^{+\infty}\mathrm{e}^{(p^2-4)x}\mathrm{d}\left[(p^2-4)x\right]=\left.\frac{1}{p^2-4}\mathrm{e}^{(p^2-4)x}\right|_0^{+\infty}.$$
当 $p^2-4<0$，即当 $-2<p<2$ 时，收敛，故 $1<p<2$，A 正确。

+++

#### 综合填空 (1) 设 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径为 $3$，则 $\sum_{n=0}^{\infty}na_n(x+1)^{n+1}$ 的收敛区间为________。
***
$(-4,2)$。

根据逐项求导收敛半径不变，即 $\sum_{n=0}^{\infty}a_nx^n$ 与 $\sum_{n=1}^{\infty}na_nx^{n-1}$ 收敛半径相同。令 $x+1=t$，则 $\sum_{n=1}^{\infty}na_nt^{n+1}$ 与 $t^2\sum_{n=1}^{\infty}na_nt^{n-1}$ 收敛半径相同，故由 $|x+1|<3$，得 $-4<x<2$，收敛区间为 $(-4,2)$。

+++

#### 综合填空 (2) 设 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径为 $R=1$，则 $\sum_{n=0}^{\infty}\dfrac{a_n}{n!}x^n$ 的收敛域为________。
***
$(-\infty,+\infty)$。

由 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径 $R=1$，知 $\forall x_0\in(-1,1)$，级数 $\sum_{n=0}^{\infty}a_nx_0^n$ 绝对收敛（阿贝尔定理），故存在 $M>0$，使得当 $n$ 充分大时，有 $|a_nx_0^n|\leqslant M$，因此 $\forall x\in(-\infty,+\infty)$，有
$$\left|\frac{a_n}{n!}x^n\right|=\left|\frac{a_nx_0^n}{n!}\cdot\frac{x^n}{x_0^n}\right|\leqslant\frac{1}{n!}\cdot\frac{M}{|x_0|^n}\cdot|x|^n,$$
而 $\sum_{n=0}^{\infty}\dfrac{M}{n!\,|x_0|^n}\cdot|x|^n$ 对任何 $x\in(-\infty,+\infty)$ 都收敛，故级数 $\sum_{n=0}^{\infty}\dfrac{a_n}{n!}x^n$ 对任何 $x\in(-\infty,+\infty)$ 都收敛，即收敛域为 $(-\infty,+\infty)$。

【注】对 $\sum_{n=0}^{\infty}\dfrac{M}{n!\,|x_0|^n}\cdot|x|^n$，用比值法，对任何 $x\in(-\infty,+\infty)$，有
$$\lim_{n\to\infty}\frac{M|x|^{n+1}}{(n+1)!\,|x_0|^{n+1}}\cdot\frac{n!\,|x_0|^n}{M|x|^n}=\lim_{n\to\infty}\frac{|x|}{(n+1)|x_0|}=0,$$
故其收敛半径为 $R=+\infty$。

以下解法是错误的：由 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径 $R=1$ 推出 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=1$，故 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{(n+1)!}\dfrac{n!}{a_n}\right|=\lim\limits_{n\to\infty}\dfrac{1}{n+1}\left|\dfrac{a_{n+1}}{a_n}\right|=0=\rho$，所以 $\sum_{n=0}^{\infty}\dfrac{a_n}{n!}x^n$ 的收敛半径 $R=+\infty$。

错误的原因是求收敛半径的公式 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\rho$，则 $R=\dfrac{1}{\rho}\ (\rho\neq0)$，条件是充分非必要的；其实证明收敛半径公式用的是正项级数的比值法，而正项级数的比值法（根值法、比较法）的条件是充分非必要的。

例如：求 $\sum_{n=0}^{\infty}\dfrac{2+(-1)^n}{2^n}x^n$ 的收敛半径。用根值公式，$\lim\limits_{n\to\infty}\sqrt[n]{|a_n|}=\lim\limits_{n\to\infty}\sqrt[n]{\dfrac{2+(-1)^n}{2^n}}=\dfrac{1}{2}$，故收敛半径 $R=2$。但
$$\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=\lim_{n\to\infty}\left|\frac{2+(-1)^{n+1}}{2^{n+1}}\cdot\frac{2^n}{2+(-1)^n}\right|=\lim_{n\to\infty}\frac{1}{2}\cdot\frac{2+(-1)^{n+1}}{2+(-1)^n}=\begin{cases}\dfrac{1}{6}, & n\text{ 为偶数},\\[4pt] \dfrac{3}{2}, & n\text{ 为奇数},\end{cases}$$
故 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|$ 不存在，即 $R=2$ 不能保证 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|$ 存在。

+++

#### 综合填空 (3) $\lim\limits_{n\to\infty}\dfrac{1}{n}\sum_{k=1}^{n}\dfrac{1}{3^k}\left(1+\dfrac{1}{k}\right)^{k^2}=$________。
***
$0$。

由级数和的定义，$\lim\limits_{n\to\infty}\sum_{k=1}^{n}\dfrac{1}{3^k}\left(1+\dfrac{1}{k}\right)^{k^2}=\sum_{k=1}^{\infty}\dfrac{1}{3^k}\left(1+\dfrac{1}{k}\right)^{k^2}$。

判别级数 $\sum_{k=1}^{\infty}\dfrac{1}{3^k}\left(1+\dfrac{1}{k}\right)^{k^2}$ 是否收敛，若收敛，则 $\sum_{k=1}^{\infty}\dfrac{1}{3^k}\left(1+\dfrac{1}{k}\right)^{k^2}=S$ 为常数。

用根值法，
$$\lim_{k\to\infty}\sqrt[k]{a_k}=\lim_{k\to\infty}\left[\frac{1}{3^k}\left(1+\frac{1}{k}\right)^{k^2}\right]^{\frac{1}{k}}=\frac{\mathrm{e}}{3}<1,$$
故级数收敛，又 $\lim\limits_{n\to\infty}\dfrac{1}{n}=0$，所以原极限 $=0$。

+++

#### 综合填空 (4) $\lim\limits_{n\to\infty}\left(\dfrac{1}{a}+\dfrac{2}{a^2}+\cdots+\dfrac{n}{a^n}\right)\ (a>1)=$________。
***
$\dfrac{a}{(1-a)^2}$。

依题意，问题转化为求级数 $\sum_{n=1}^{\infty}\dfrac{n}{a^n}$ 的和。构造幂级数 $S(x)=\sum_{n=1}^{\infty}nx^n$，则
$$S(x)=\sum_{n=1}^{\infty}nx^n=x\sum_{n=1}^{\infty}nx^{n-1}=x\left(\sum_{n=0}^{\infty}x^n\right)'=x\left(\frac{1}{1-x}\right)'=\frac{x}{(1-x)^2},\quad|x|<1,$$
令 $x=\dfrac{1}{a}$，则
$$\lim_{n\to\infty}\left(\frac{1}{a}+\frac{2}{a^2}+\cdots+\frac{n}{a^n}\right)=S\left(\frac{1}{a}\right)=\frac{\frac{1}{a}}{\left(1-\frac{1}{a}\right)^2}=\frac{a}{(1-a)^2}.$$

+++

#### 综合填空 (5) 设 $\sum_{n=1}^{\infty}(-1)^{n-1}u_n=2$，$\sum_{n=1}^{\infty}u_{2n-1}=5$，则 $\sum_{n=1}^{\infty}u_n=$________。
***
$8$。

利用收敛级数的定义。令
$$\tau_n=\sum_{k=1}^{n}(-1)^{k-1}u_k,\quad \sigma_n=\sum_{k=1}^{n}u_{2k-1},\quad S_n=\sum_{k=1}^{n}u_k,$$
则
$$S_{2n}=-(u_1-u_2+u_3-u_4+\cdots+u_{2n-1}-u_{2n})+2(u_1+u_3+\cdots+u_{2n-1})=-\tau_{2n}+2\sigma_n,$$
故
$$\lim_{n\to\infty}S_{2n}=-\lim_{n\to\infty}\tau_{2n}+2\lim_{n\to\infty}\sigma_n=-2+2\times5=8.$$
又 $S_{2n+1}=S_{2n}+u_{2n+1}$，且 $\lim\limits_{n\to\infty}S_{2n+1}=\lim\limits_{n\to\infty}S_{2n}+\lim\limits_{n\to\infty}u_{2n+1}=8$，故 $\lim\limits_{n\to\infty}S_n=8$，即 $\sum_{n=1}^{\infty}u_n=8$。

【注】由 $\sum_{n=1}^{\infty}u_{2n-1}=S$ 收敛，根据收敛级数的必要条件，知 $\lim\limits_{n\to\infty}u_{2n+1}=0$。

+++

#### 综合填空 (6) 设 $\sum_{n=1}^{\infty}u_n\ (u_n>0)$ 发散，$S_n=u_1+u_2+\cdots+u_n$，则 $\sum_{n=1}^{\infty}\left(\dfrac{1}{S_n}-\dfrac{1}{S_{n+1}}\right)=$________。
***
$\dfrac{1}{u_1}$。

由正项级数 $\sum_{n=1}^{\infty}u_n$ 发散，知 $\lim\limits_{n\to\infty}S_n=+\infty$。记 $S_n'$ 为所求级数的部分和，则
$$S_n'=\left(\frac{1}{S_1}-\frac{1}{S_2}\right)+\left(\frac{1}{S_2}-\frac{1}{S_3}\right)+\cdots+\left(\frac{1}{S_n}-\frac{1}{S_{n+1}}\right)=\frac{1}{S_1}-\frac{1}{S_{n+1}},$$
故 $\lim\limits_{n\to\infty}S_n'=\dfrac{1}{S_1}=\dfrac{1}{u_1}$。

+++

#### 综合解答 (1) 已知函数 $y=y(x)$ 满足方程 $y'=x+y$，且 $y(0)=1$，讨论级数 $\sum_{n=1}^{\infty}\left[y\left(\dfrac{1}{n}\right)-1-\dfrac{1}{n}\right]$ 的敛散性。
***
由 $y'=x+y$，得 $y''=1+y'$，又 $y(0)=1$，知 $y'(0)=1$，$y''(0)=2$，根据麦克劳林公式，有
$$y\left(\frac{1}{n}\right)=y(0)+y'(0)\frac{1}{n}+\frac{1}{2}y''(0)\frac{1}{n^2}+o\left(\frac{1}{n^2}\right)=1+\frac{1}{n}+\frac{1}{n^2}+o\left(\frac{1}{n^2}\right),$$
所以 $\left|y\left(\dfrac{1}{n}\right)-1-\dfrac{1}{n}\right|$ 与 $\dfrac{1}{n^2}$ 是等价无穷小（$n\to\infty$）。而 $\sum_{n=1}^{\infty}\dfrac{1}{n^2}$ 收敛，由比较审敛法，知 $\sum_{n=1}^{\infty}\left[y\left(\dfrac{1}{n}\right)-1-\dfrac{1}{n}\right]$ **绝对收敛**。

【注】此题也可先解微分方程 $\begin{cases}y'-y=x,\\ y(0)=1,\end{cases}$ 得 $y=y(x)$，再用麦克劳林公式展开 $y\left(\dfrac{1}{n}\right)$。

+++

#### 综合解答 (2) 求 $\sum_{n=1}^{\infty}\dfrac{x^n}{n\left[3^n+(-2)^n\right]}$ 的收敛区间，并讨论在端点处的敛散性。
***
先用公式求收敛半径。
$$\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=\lim_{n\to\infty}\frac{n\left[3^n+(-2)^n\right]}{(n+1)\left[3^{n+1}+(-2)^{n+1}\right]}=\lim_{n\to\infty}\frac{1+\left(-\frac{2}{3}\right)^n}{3\left[1+\left(-\frac{2}{3}\right)^{n+1}\right]}=\frac{1}{3},$$
故收敛半径 $R=3$，收敛区间为 $(-3,3)$。

当 $x=3$ 时，级数为 $\sum_{n=1}^{\infty}\dfrac{3^n}{n\left[3^n+(-2)^n\right]}$，
$$\frac{3^n}{n\left[3^n+(-2)^n\right]}=\frac{1}{1+\left(-\frac{2}{3}\right)^n}\cdot\frac{1}{n}\geqslant\frac{1}{2n},$$
而 $\sum_{n=1}^{\infty}\dfrac{1}{2n}$ 发散，由比较审敛法，知级数发散。

当 $x=-3$ 时，级数为 $\sum_{n=1}^{\infty}\dfrac{(-3)^n}{n\left[3^n+(-2)^n\right]}$，拆成两个级数，
$$\frac{(-3)^n}{n\left[3^n+(-2)^n\right]}=\frac{(-1)^n\left[3^n+(-2)^n\right]-2^n}{3^n+(-2)^n}\cdot\frac{1}{n}=(-1)^n\frac{1}{n}-\frac{2^n}{3^n+(-2)^n}\cdot\frac{1}{n}.$$
$\sum_{n=1}^{\infty}(-1)^n\dfrac{1}{n}$ 条件收敛，对 $\sum_{n=1}^{\infty}\dfrac{2^n}{3^n+(-2)^n}\cdot\dfrac{1}{n}$，用比值法，
$$\lim_{n\to\infty}\frac{a_{n+1}}{a_n}=\lim_{n\to\infty}\frac{2^{n+1}}{3^{n+1}+(-2)^{n+1}}\cdot\frac{1}{n+1}\cdot\frac{\left[3^n+(-2)^n\right]\cdot n}{2^n}=2\lim_{n\to\infty}\frac{3^n+(-2)^n}{3^{n+1}+(-2)^{n+1}}=\frac{2}{3}\lim_{n\to\infty}\frac{1+\left(-\frac{2}{3}\right)^n}{1+\left(-\frac{2}{3}\right)^{n+1}}=\frac{2}{3}<1,$$
故级数收敛，所以 $\sum_{n=1}^{\infty}\dfrac{x^n}{n\left[3^n+(-2)^n\right]}$ 在 $x=-3$ 处收敛。

+++

#### 综合解答 (3) （Ⅰ）设 $k>0$，$x>0$，证明不等式：$kx<(1+k^2x^2)\arctan kx$；\
（Ⅱ）判别级数 $\sum_{n=1}^{\infty}\dfrac{(-1)^n\arctan kn}{n}\ (k>0)$ 是绝对收敛，还是条件收敛。
***
（Ⅰ）令 $g(x)=kx-(1+k^2x^2)\arctan kx$，则
$$g'(x)=k-(1+k^2x^2)\frac{k}{1+k^2x^2}-2k^2x\arctan kx=-2k^2x\arctan kx<0,$$
故 $g(x)$ 单调减少。又 $g(0)=0$，所以 $g(x)<g(0)=0$，所证不等式成立。

（Ⅱ）由 $\left|\dfrac{(-1)^n\arctan kn}{n}\right|\sim\dfrac{\pi}{2n}\ (n\to\infty)$，而 $\sum_{n=1}^{\infty}\dfrac{\pi}{2n}$ 发散，故级数不绝对收敛。

$\lim\limits_{n\to\infty}\dfrac{\arctan kn}{n}=0$，令 $f(x)=\dfrac{\arctan kx}{x}$，则
$$f'(x)=\frac{kx-(1+k^2x^2)\arctan kx}{x^2(1+k^2x^2)}<0\quad(\text{由（Ⅰ）}),$$
所以 $f(n)$ 单调减少。由莱布尼茨定理，知级数**条件收敛**。

+++

#### 综合解答 (4) 设数列 $\{a_n\}$ 满足 $a_n=a_0+nd$，$n=1,2,\cdots$，其中 $a_0\neq0$，$d\neq0$ 为常数。\
（Ⅰ）求 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛域；\
（Ⅱ）求 $\sum_{n=0}^{\infty}\dfrac{a_n}{2^n}$。
***
（Ⅰ）利用公式求收敛半径。
$$\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=\lim_{n\to\infty}\left|\frac{a_0+(n+1)d}{a_0+nd}\right|=1,$$
故 $R=1$，收敛区间为 $(-1,1)$。

当 $x=\pm1$ 时，$\sum_{n=0}^{\infty}(\pm1)^n\cdot a_n$ 发散（由 $\lim\limits_{n\to\infty}a_n\neq0$），故收敛域为 $(-1,1)$。

（Ⅱ）求 $\sum_{n=0}^{\infty}a_nx^n$ 的和函数 $S(x)$。
$$S(x)=\sum_{n=0}^{\infty}a_nx^n=\sum_{n=0}^{\infty}(a_0+nd)x^n=\sum_{n=0}^{\infty}a_0x^n+d\sum_{n=0}^{\infty}nx^n,$$
记为 $S_1(x)+S_2(x)$，其中
$$S_1(x)=\sum_{n=0}^{\infty}a_0x^n=\frac{a_0}{1-x},$$
$$S_2(x)=d\sum_{n=0}^{\infty}nx^n=dx\sum_{n=0}^{\infty}nx^{n-1}=dx\left(\sum_{n=0}^{\infty}x^n\right)'=dx\left(\frac{1}{1-x}\right)'=\frac{dx}{(1-x)^2},$$
故 $S(x)=\dfrac{a_0}{1-x}+\dfrac{dx}{(1-x)^2}$。令 $x=\dfrac{1}{2}$，得 $\sum_{n=0}^{\infty}\dfrac{a_n}{2^n}=2a_0+2d$。

+++

#### 综合解答 (5) 设 $\dfrac{1}{1-x-x^2}=\sum_{n=0}^{\infty}a_nx^n$。证明：\
（Ⅰ）$a_0=1$，$a_1=1$，$a_{n+2}=a_{n+1}+a_n\ (n=0,1,2,\cdots)$；\
（Ⅱ）$\sum_{n=1}^{\infty}\dfrac{a_{n+1}}{a_na_{n+2}}$ 收敛，并求其和。
***
（Ⅰ）由 $\dfrac{1}{1-x-x^2}=\sum_{n=0}^{\infty}a_nx^n$，得 $(1-x-x^2)\sum_{n=0}^{\infty}a_nx^n=1$，即
$$\sum_{n=0}^{\infty}a_nx^n-\sum_{n=0}^{\infty}a_nx^{n+1}-\sum_{n=0}^{\infty}a_nx^{n+2}=1,$$
变形为
$$\left(a_0+a_1x+\sum_{n=0}^{\infty}a_{n+2}x^{n+2}\right)-\left(a_0x+\sum_{n=0}^{\infty}a_{n+1}x^{n+2}\right)-\sum_{n=0}^{\infty}a_nx^{n+2}=1.$$
比较上式两边同次幂系数，得
$$a_0=1,\quad a_1-a_0=0,\quad a_{n+2}-a_{n+1}-a_n=0\ (n=0,1,2,\cdots),$$
故 $a_0=1$，$a_1=1$，$a_{n+2}=a_{n+1}+a_n\ (n=0,1,2,\cdots)$。

（Ⅱ）$\sum_{n=1}^{\infty}\dfrac{a_{n+1}}{a_na_{n+2}}=\sum_{n=1}^{\infty}\dfrac{a_{n+2}-a_n}{a_na_{n+2}}=\sum_{n=1}^{\infty}\left(\dfrac{1}{a_n}-\dfrac{1}{a_{n+2}}\right)$，又其前 $n$ 项的和为
$$S_n=\left(\frac{1}{a_1}-\frac{1}{a_3}\right)+\left(\frac{1}{a_2}-\frac{1}{a_4}\right)+\cdots+\left(\frac{1}{a_n}-\frac{1}{a_{n+2}}\right)=\frac{1}{a_1}+\frac{1}{a_2}-\frac{1}{a_{n+1}}-\frac{1}{a_{n+2}},$$
由 $a_0=a_1=1$，$a_2=a_0+a_1=2$，$a_{n+2}=a_n+a_{n+1}$，得 $\lim\limits_{n\to\infty}a_n=+\infty$，故
$$\lim_{n\to\infty}S_n=\frac{1}{a_1}+\frac{1}{a_2}=\frac{3}{2},\quad\text{即}\quad \sum_{n=1}^{\infty}\frac{a_{n+1}}{a_na_{n+2}}=\frac{3}{2}.$$

+++

#### 综合解答 (6) 设 $f(x)$ 在 $[a,b]$ 上可导，且满足 $a\leqslant f(x)\leqslant b$，$|f'(x)|\leqslant k<1$，$u_0\in[a,b]$，$u_n=f(u_{n-1})\ (n=1,2,\cdots)$，证明：\
（Ⅰ）$\sum_{n=1}^{\infty}(u_{n+1}-u_n)$ 绝对收敛；\
（Ⅱ）$\lim\limits_{n\to\infty}u_n$ 存在。
***
（Ⅰ）
$$|u_{n+1}-u_n|=|f(u_n)-f(u_{n-1})|=|f'(\xi_n)|\,|u_n-u_{n-1}|\leqslant k|u_n-u_{n-1}|\leqslant k^2|u_{n-1}-u_{n-2}|\leqslant\cdots\leqslant k^n|u_1-u_0|,$$
而 $\sum_{n=1}^{\infty}k^n|u_1-u_0|$ 收敛（等比级数 $k<1$），由比较审敛法，知 $\sum_{n=1}^{\infty}(u_{n+1}-u_n)$ 绝对收敛。

（Ⅱ）由（Ⅰ），知 $\sum_{n=1}^{\infty}(u_{n+1}-u_n)$ 绝对收敛，从而 $\sum_{n=1}^{\infty}(u_{n+1}-u_n)$ 收敛，故其部分和的极限 $\lim\limits_{n\to\infty}S_n=\lim\limits_{n\to\infty}(u_{n+1}-u_1)$ 存在，从而 $\lim\limits_{n\to\infty}u_{n+1}$ 存在（$u_1$ 是一个数），即 $\lim\limits_{n\to\infty}u_n$ 存在。

+++

#### 综合解答 (7) 讨论 $\sum_{n=1}^{\infty}\sin\sqrt{n^2+1}\,\pi$ 的敛散性，若收敛，判断是绝对收敛还是条件收敛。
***
由
$$\sin\sqrt{n^2+1}\,\pi=\sin\left[n\pi+\left(\sqrt{n^2+1}-n\right)\pi\right]=(-1)^n\sin\left(\sqrt{n^2+1}-n\right)\pi=(-1)^n\sin\frac{\pi}{\sqrt{n^2+1}+n},$$
且 $\sin\dfrac{\pi}{\sqrt{n^2+1}+n}>0$，知原级数是交错级数。

由 $\left|\sin\sqrt{n^2+1}\,\pi\right|=\sin\dfrac{\pi}{\sqrt{n^2+1}+n}\sim\dfrac{\pi}{2n}\ (n\to\infty)$，且 $\sum_{n=1}^{\infty}\dfrac{\pi}{2n}$ 发散，知原级数不绝对收敛。

又 $\lim\limits_{n\to\infty}\sin\dfrac{\pi}{\sqrt{n^2+1}+n}=0$，且 $\left\{\sin\dfrac{\pi}{\sqrt{n^2+1}+n}\right\}$ 单调减少，由莱布尼茨定理，知原级数**条件收敛**。

+++

#### 综合解答 (8) 设 $a_n=\int_{-\infty}^{+\infty}x^{2n}\mathrm{e}^{-nx^2}\mathrm{d}x\ (n=1,2,\cdots)$，证明：级数 $\sum_{n=1}^{\infty}a_n$ 收敛。
***
先利用分部积分法求 $a_n$，
$$a_n=\int_{-\infty}^{+\infty}x^{2n}\mathrm{e}^{-nx^2}\mathrm{d}x=-\left.\frac{1}{2n}x^{2n-1}\mathrm{e}^{-nx^2}\right|_{-\infty}^{+\infty}+\frac{2n-1}{2n}\int_{-\infty}^{+\infty}x^{2n-2}\mathrm{e}^{-nx^2}\mathrm{d}x$$
$$=\frac{2n-1}{2n}\int_{-\infty}^{+\infty}x^{2n-2}\mathrm{e}^{-nx^2}\mathrm{d}x=-\left.\frac{2n-1}{(2n)^2}x^{2n-3}\mathrm{e}^{-nx^2}\right|_{-\infty}^{+\infty}+\frac{(2n-1)(2n-3)}{(2n)^2}\int_{-\infty}^{+\infty}x^{2n-4}\mathrm{e}^{-nx^2}\mathrm{d}x$$
$$=\frac{(2n-1)(2n-3)}{(2n)^2}\int_{-\infty}^{+\infty}x^{2n-4}\mathrm{e}^{-nx^2}\mathrm{d}x=\cdots=\frac{(2n-1)\cdot(2n-3)\cdot\cdots\cdot3\cdot1}{(2n)^n}\int_{-\infty}^{+\infty}\mathrm{e}^{-nx^2}\mathrm{d}x.$$
而 $\int_{-\infty}^{+\infty}\mathrm{e}^{-nx^2}\mathrm{d}x=\sqrt{\dfrac{\pi}{n}}$，则 $a_n=\dfrac{(2n-1)\cdot(2n-3)\cdot\cdots\cdot3\cdot1}{(2n)^n}\cdot\sqrt{\dfrac{\pi}{n}}$，用比值法，
$$\lim_{n\to\infty}\frac{a_{n+1}}{a_n}=\lim_{n\to\infty}\frac{(2n+1)(2n-1)\cdots1}{(2n+2)^{n+1}}\cdot\frac{(2n)^n}{(2n-1)(2n-3)\cdots1}\cdot\sqrt{\frac{n}{n+1}}=\lim_{n\to\infty}\frac{2n+1}{2n+2}\left(\frac{n}{n+1}\right)^n\cdot\sqrt{\frac{n}{n+1}}=\frac{1}{\mathrm{e}}<1,$$
故 $\sum_{n=1}^{\infty}a_n$ 收敛。

+++

#### 综合解答 (9) 设 $a_0=0$，$a_{n+1}=\sqrt{2+a_n}\ (n=0,1,2,\cdots)$。\
（Ⅰ）证明：$\lim\limits_{n\to\infty}a_n$ 存在，并求其值；\
（Ⅱ）判别 $\sum_{n=1}^{\infty}(-1)^{n-1}\sqrt{2-a_n}$ 是绝对收敛，还是条件收敛。
***
（Ⅰ）用单调有界准则，由 $a_0=0$，$a_1=\sqrt{2+0}=\sqrt{2}>a_0$，设 $0\leqslant a_{n-1}<a_n$，则 $2+a_{n-1}<2+a_n$，故 $\sqrt{2+a_{n-1}}<\sqrt{2+a_n}$，即 $a_n<a_{n+1}$，由归纳法，知 $\{a_n\}$ 单调增加。

又 $a_1=\sqrt{2}<2$，设 $a_n<2$，则 $a_{n+1}=\sqrt{2+a_n}<2$，由归纳法，知 $\{a_n\}$ 有上界，所以 $\lim\limits_{n\to\infty}a_n$ 存在，记 $\lim\limits_{n\to\infty}a_n=a$，则 $a=\sqrt{2+a}$，解得 $a=2$，即 $\lim\limits_{n\to\infty}a_n=2$。

（Ⅱ）设 $u_n=\sqrt{2-a_n}$，用比值法，
$$\lim_{n\to\infty}\frac{u_{n+1}}{u_n}=\lim_{n\to\infty}\frac{\sqrt{2-a_{n+1}}}{\sqrt{2-a_n}}=\lim_{n\to\infty}\sqrt{\frac{2-\sqrt{2+a_n}}{2-a_n}}=\lim_{n\to\infty}\sqrt{\frac{4-(2+a_n)}{(2-a_n)\left(2+\sqrt{2+a_n}\right)}}=\lim_{n\to\infty}\frac{1}{\sqrt{2+\sqrt{2+a_n}}}=\frac{1}{2}<1,$$
故原级数**绝对收敛**。

+++

#### 综合解答 (10) 将 $f(x)=x\mathrm{e}^x$ 在 $x=2$ 处展开为幂级数，并求 $f^{(n)}(2)$。
***
$$f(x)=x\mathrm{e}^x=(x-2+2)\mathrm{e}^{x-2+2}=\mathrm{e}^2\left[(x-2)+2\right]\mathrm{e}^{x-2}=\mathrm{e}^2\left[(x-2)+2\right]\sum_{n=0}^{\infty}\frac{(x-2)^n}{n!}$$
$$=\mathrm{e}^2\sum_{n=0}^{\infty}\frac{(x-2)^{n+1}}{n!}+2\mathrm{e}^2\left[1+\sum_{n=1}^{\infty}\frac{(x-2)^n}{n!}\right]=\mathrm{e}^2\sum_{n=0}^{\infty}\frac{(x-2)^{n+1}}{n!}+2\mathrm{e}^2\left[1+\sum_{n=0}^{\infty}\frac{(x-2)^{n+1}}{(n+1)!}\right]$$
$$=2\mathrm{e}^2+\sum_{n=0}^{\infty}\frac{\mathrm{e}^2(n+3)}{(n+1)!}(x-2)^{n+1},\quad x\in(-\infty,+\infty).$$
由 $a_{n+1}=\dfrac{\mathrm{e}^2(n+3)}{(n+1)!}$，可知 $a_n=\dfrac{\mathrm{e}^2(n+2)}{n!}$，故
$$f^{(n)}(2)=n!\,a_n=\mathrm{e}^2(n+2).$$

+++

#### 综合解答 (11) 将 $f(x)=\dfrac{x-1}{3-x}$ 在 $x=1$ 处展开为幂级数，并求 $f^{(n)}(1)$。
***
$$f(x)=\frac{x-1}{3-x}=(x-1)\cdot\frac{1}{3-x}=(x-1)\cdot\frac{1}{2-(x-1)}=\frac{1}{2}(x-1)\cdot\frac{1}{1-\frac{x-1}{2}}$$
$$=\frac{1}{2}(x-1)\left[1+\frac{x-1}{2}+\frac{(x-1)^2}{2^2}+\cdots+\frac{(x-1)^n}{2^n}+\cdots\right]$$
$$=\frac{1}{2}\left[(x-1)+\frac{(x-1)^2}{2}+\frac{(x-1)^3}{2^2}+\cdots+\frac{(x-1)^{n+1}}{2^n}+\cdots\right],$$
其中 $|x-1|<2$。

$$f^{(n)}(1)=n!\,a_n=\frac{n!}{2^n}.$$

+++

#### 综合解答 (12) 将 $f(x)=\sin x+x\cos x$ 展开为 $x$ 的幂级数，并求 $\sum_{n=0}^{\infty}(-1)^n\dfrac{n+1}{(2n+1)!}$ 的和。
***
$$f(x)=\sin x+x\cos x=\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n+1}}{(2n+1)!}+x\sum_{n=0}^{\infty}(-1)^n\frac{x^{2n}}{(2n)!}$$
$$=\sum_{n=0}^{\infty}(-1)^n\left[\frac{1}{(2n+1)!}+\frac{1}{(2n)!}\right]x^{2n+1}=\sum_{n=0}^{\infty}(-1)^n\frac{2(n+1)}{(2n+1)!}x^{2n+1},\quad x\in(-\infty,+\infty).$$
令 $x=1$，则
$$\sum_{n=0}^{\infty}(-1)^n\frac{n+1}{(2n+1)!}=\frac{1}{2}f(1)=\frac{1}{2}(\sin 1+\cos 1).$$

【注】$\dfrac{1}{(2n+1)!}+\dfrac{1}{(2n)!}=\dfrac{2(n+1)}{(2n+1)!}$。

+++

#### 综合解答 (13) 将 $f(x)=\dfrac{x\mathrm{e}^x-\mathrm{e}^x+1}{x^2}$ 展开为 $x$ 的幂级数，并求 $\sum_{n=1}^{\infty}\dfrac{n}{(n+1)!}$ 的和。
***
直接展开较为复杂，考虑到
$$\frac{x\mathrm{e}^x-\mathrm{e}^x+1}{x^2}=\left(\frac{\mathrm{e}^x-1}{x}\right)'.$$
令 $g(x)=\dfrac{\mathrm{e}^x-1}{x}$，则
$$g(x)=\frac{\mathrm{e}^x-1}{x}=\frac{1}{x}\left(1+x+\frac{x^2}{2!}+\cdots+\frac{x^n}{n!}+\cdots-1\right)\quad(|x|<\infty,\ x\neq0)$$
$$=1+\frac{x}{2!}+\cdots+\frac{x^{n-1}}{n!}+\cdots,$$
故
$$f(x)=\left(\frac{\mathrm{e}^x-1}{x}\right)'=\frac{1}{2!}+\frac{2}{3!}x+\cdots+\frac{n}{(n+1)!}x^{n-1}+\cdots,$$
所以
$$\frac{x\mathrm{e}^x-\mathrm{e}^x+1}{x^2}=\sum_{n=1}^{\infty}\frac{n}{(n+1)!}x^{n-1},\quad|x|<\infty,\ x\neq0.$$
令 $x=1$，得 $\sum_{n=1}^{\infty}\dfrac{n}{(n+1)!}=1$。

+++

#### 综合解答 (14) 求级数 $\sum_{n=0}^{\infty}x\mathrm{e}^{-nx}$ 的收敛域及和函数。
***
所给级数不是幂级数。

由 $\sum_{n=0}^{\infty}x\mathrm{e}^{-nx}=x\sum_{n=0}^{\infty}\left(\mathrm{e}^{-x}\right)^n$，令 $\mathrm{e}^{-x}=t$，而 $\sum_{n=0}^{\infty}t^n=\dfrac{1}{1-t}$，$t\in(-1,1)$，故当 $-1<\mathrm{e}^{-x}<1$（$\mathrm{e}^{-x}>0$ 恒成立），即 $x>0$ 时，原级数收敛，且
$$\sum_{n=0}^{\infty}x\mathrm{e}^{-nx}=\frac{x}{1-\mathrm{e}^{-x}}=\frac{x\mathrm{e}^x}{\mathrm{e}^x-1},\quad x\in(0,+\infty).$$
当 $x=0$，级数和为 $0$，故
$$\sum_{n=0}^{\infty}x\mathrm{e}^{-nx}=\begin{cases}\dfrac{x\mathrm{e}^x}{\mathrm{e}^x-1}, & x>0,\\[6pt] 0, & x=0.\end{cases}$$

+++

#### 综合解答 (15) 设 $a_0=3$，$a_1=5$，且 $na_n=\dfrac{2}{3}a_{n-1}-(n-1)a_{n-1}\ (n>1)$，证明：当 $|x|<1$ 时，$\sum_{n=0}^{\infty}a_nx^n$ 收敛，并求其和函数。
***
由 $na_n=\dfrac{2}{3}a_{n-1}-(n-1)a_{n-1}$，可知 $a_{n+1}=\dfrac{1}{n+1}\left(\dfrac{2}{3}-n\right)a_n$。

因为
$$\lim_{n\to\infty}\left|\frac{a_{n+1}x^{n+1}}{a_nx^n}\right|=\lim_{n\to\infty}\left|\frac{\frac{1}{n+1}\left(\frac{2}{3}-n\right)a_n}{a_n}\right|\cdot|x|=|x|<1,$$
所以当 $|x|<1$ 时，$\sum_{n=0}^{\infty}a_nx^n$ 绝对收敛，故 $\sum_{n=0}^{\infty}a_nx^n$ 收敛。

令 $y(x)=\sum_{n=0}^{\infty}a_nx^n$，则
$$y'(x)=\sum_{n=1}^{\infty}na_nx^{n-1}=a_1+\sum_{n=2}^{\infty}na_nx^{n-1}=a_1+\sum_{n=1}^{\infty}(n+1)a_{n+1}x^n$$
$$=5+\sum_{n=1}^{\infty}\left(\frac{2}{3}a_n-na_n\right)x^n=5+\frac{2}{3}\left(\sum_{n=0}^{\infty}a_nx^n-a_0\right)-x\sum_{n=1}^{\infty}na_nx^{n-1}$$
$$=5+\frac{2}{3}y(x)-\frac{2}{3}\times3-xy'(x)=3+\frac{2}{3}y(x)-xy'(x),$$
故 $(x+1)y'(x)-\dfrac{2}{3}y(x)=3$，即
$$y'-\frac{2}{3(x+1)}y=\frac{3}{x+1}.$$
解一阶线性微分方程，得 $y=C(x+1)^{\frac{2}{3}}-\dfrac{9}{2}$，由 $y(0)=a_0=3$，得 $C=\dfrac{15}{2}$，故
$$y(x)=\sum_{n=0}^{\infty}a_nx^n=\frac{15}{2}(x+1)^{\frac{2}{3}}-\frac{9}{2}.$$

+++

#### 综合解答 (16) 设 $f(x)=\sum_{n=1}^{\infty}\dfrac{x^n}{n^2}$，证明：$f(x)+f(1-x)+\ln x\ln(1-x)=\sum_{n=1}^{\infty}\dfrac{1}{n^2}$。
***
因为 $\sum_{n=1}^{\infty}\dfrac{x^n}{n^2}$ 的收敛域为 $[-1,1]$，所以 $f(1-x)$ 的定义域为 $[0,2]$。

令 $F(x)=f(x)+f(1-x)+\ln x\ln(1-x)$，定义域为 $x\in(0,1)$，由于
$$f'(x)=\left(\sum_{n=1}^{\infty}\frac{x^n}{n^2}\right)'=\sum_{n=1}^{\infty}\frac{x^{n-1}}{n}=\frac{1}{x}\sum_{n=1}^{\infty}\frac{x^n}{n}=\frac{1}{x}\int_0^x\left(\sum_{n=1}^{\infty}\frac{t^n}{n}\right)'\mathrm{d}t=\frac{1}{x}\int_0^x\frac{1}{1-t}\mathrm{d}t=-\frac{1}{x}\ln(1-x),$$
$$f'(1-x)=\frac{1}{x-1}\ln x,$$
$$\left[\ln x\ln(1-x)\right]'=\frac{1}{x}\ln(1-x)-\frac{1}{1-x}\ln x,$$
所以
$$F'(x)=f'(x)-f'(1-x)+\left[\ln x\ln(1-x)\right]'=0,\quad x\in(0,1),$$
故 $F(x)\equiv C$。又由于
$$C=\lim_{x\to1^-}F(x)=f(1)+f(0)+\lim_{x\to1^-}\ln\left[1+(x-1)\right]\ln(1-x)=f(1)=\sum_{n=1}^{\infty}\frac{1}{n^2},$$
所以
$$f(x)+f(1-x)+\ln x\ln(1-x)=\sum_{n=1}^{\infty}\frac{1}{n^2},\quad x\in(0,1).$$

+++

#### 综合解答 (17) 设 $f(x)=\sum_{n=0}^{\infty}\dfrac{a_n}{n!}x^n$ 满足 $\begin{cases}f''(x)-f'(x)-2f(x)=0,\\ f(0)=0,\ f'(0)=1,\end{cases}$ 求 $f(x)$ 及 $a_n$。
***
特征方程为 $r^2-r-2=0$，得 $r_1=-1$，$r_2=2$，故通解为
$$f(x)=C_1\mathrm{e}^{-x}+C_2\mathrm{e}^{2x}.$$
由 $f(0)=0$，$f'(0)=1$，得 $C_1+C_2=0$，$-C_1+2C_2=1$，解得 $C_1=-\dfrac{1}{3}$，$C_2=\dfrac{1}{3}$，故
$$f(x)=-\frac{1}{3}\mathrm{e}^{-x}+\frac{1}{3}\mathrm{e}^{2x}.$$
将 $f(x)$ 展开为 $x$ 的幂级数，
$$f(x)=-\frac{1}{3}\mathrm{e}^{-x}+\frac{1}{3}\mathrm{e}^{2x}=-\frac{1}{3}\sum_{n=0}^{\infty}\frac{(-x)^n}{n!}+\frac{1}{3}\sum_{n=0}^{\infty}\frac{(2x)^n}{n!}$$
$$=-\frac{1}{3}\sum_{n=0}^{\infty}\frac{(-1)^nx^n}{n!}+\frac{1}{3}\sum_{n=0}^{\infty}\frac{2^nx^n}{n!}=\sum_{n=0}^{\infty}\left[\left(-\frac{1}{3}\right)(-1)^n+\frac{2^n}{3}\right]\frac{x^n}{n!},$$
故 $a_n=\dfrac{1}{3}\left[(-1)^{n+1}+2^n\right]$。

+++

#### 综合解答 (18) 求形如 $\sum_{n=1}^{\infty}b_n\sin nx$ 的级数，使其在 $(0,\pi)$ 内的和函数为 $\dfrac{1}{2}(\pi-x)$，当 $x=\dfrac{\pi}{2}$ 时，求此级数的和。
***
将 $\dfrac{1}{2}(\pi-x)$ 展开为傅里叶级数，其系数即为 $b_n$。

先定义一个以 $2\pi$ 为周期的函数 $f(x)$，它在 $(-\pi,\pi)$ 内的定义如下：
$$f(x)=\begin{cases}-\dfrac{1}{2}(\pi+x), & -\pi<x<0,\\[4pt] 0, & x=0,\\[4pt] \dfrac{1}{2}(\pi-x), & 0<x<\pi.\end{cases}$$
$f(x)$ 为奇函数，其傅里叶级数为正弦级数 $\sum_{n=1}^{\infty}b_n\sin nx$，其中
$$b_n=\frac{2}{\pi}\int_0^{\pi}f(x)\sin nx\,\mathrm{d}x=\frac{1}{\pi}\int_0^{\pi}(\pi-x)\sin nx\,\mathrm{d}x=\frac{1}{n}.$$
$f(x)$ 在 $(0,\pi)$ 内连续，由收敛定理，知
$$\sum_{n=1}^{\infty}\frac{1}{n}\sin nx=\frac{1}{2}(\pi-x),\quad x\in(0,\pi),$$
当 $x=\dfrac{\pi}{2}$ 时，$\sum_{n=1}^{\infty}\dfrac{1}{n}\sin\dfrac{n\pi}{2}=1-\dfrac{1}{3}+\dfrac{1}{5}-\dfrac{1}{7}+\cdots=\dfrac{\pi}{4}$。

+++

#### 拓展解答 (1) 设 $a_n=\int_0^1x^n\sqrt{1-x^2}\,\mathrm{d}x$，$b_n=\int_0^{\frac{\pi}{2}}\sin^n t\,\mathrm{d}t\ (n=1,2,\cdots)$，求级数 $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{a_n}{b_n}$ 的和。
***
$$a_n=\int_0^1x^n\sqrt{1-x^2}\,\mathrm{d}x\ \xlongequal{x=\sin t}\ \int_0^{\frac{\pi}{2}}\sin^n t\cdot\cos^2 t\,\mathrm{d}t$$
$$=\int_0^{\frac{\pi}{2}}\sin^n t\left(1-\sin^2 t\right)\mathrm{d}t=\int_0^{\frac{\pi}{2}}\sin^n t\,\mathrm{d}t-\int_0^{\frac{\pi}{2}}\sin^{n+2}t\,\mathrm{d}t=b_n-b_{n+2}.$$
又
$$b_{n+2}=\int_0^{\frac{\pi}{2}}\sin^{n+2}t\,\mathrm{d}t=-\int_0^{\frac{\pi}{2}}\sin^{n+1}t\,\mathrm{d}(\cos t)=-\left[\left.\cos t\cdot\sin^{n+1}t\right|_0^{\frac{\pi}{2}}-\int_0^{\frac{\pi}{2}}\cos t\cdot(n+1)\sin^n t\cdot\cos t\,\mathrm{d}t\right]$$
$$=(n+1)\int_0^{\frac{\pi}{2}}\sin^n t\left(1-\sin^2 t\right)\mathrm{d}t=(n+1)b_n-(n+1)b_{n+2},$$
移项得 $b_{n+2}=\dfrac{n+1}{n+2}b_n$，所以 $a_n=b_n-b_{n+2}=b_n-\dfrac{n+1}{n+2}b_n=\dfrac{b_n}{n+2}$，故 $\dfrac{a_n}{b_n}=\dfrac{1}{n+2}$，则
$$\sum_{n=1}^{\infty}(-1)^{n-1}\frac{a_n}{b_n}=\sum_{n=1}^{\infty}(-1)^{n-1}\frac{1}{n+2}.$$
构造幂级数，令 $S(x)=\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{1}{n+2}\cdot x^{n+2}$，则
$$S'(x)=\sum_{n=1}^{\infty}(-1)^{n-1}x^{n+1}=\frac{x^2}{1+x},\quad|x|<1,$$
积分得
$$S(x)-S(0)=\int_0^x\frac{t^2}{1+t}\mathrm{d}t=\frac{1}{2}x^2-x+\ln(x+1),\quad-1<x\leqslant1.$$
$S(0)=0$，令 $x=1$，故 $\sum_{n=1}^{\infty}(-1)^{n-1}\dfrac{1}{n+2}=\ln 2-\dfrac{1}{2}$。

+++

#### 拓展解答 (2) 设 $a_0=1$，$a_1=0$，$(n+1)a_{n+1}=na_n+a_{n-1}\ (n=1,2,\cdots)$，$S(x)=\sum_{n=0}^{\infty}a_nx^n$。\
（Ⅰ）求 $\lim\limits_{n\to\infty}a_n$，并计算级数 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径；\
（Ⅱ）求 $S(x)$ 满足的一阶微分方程，并求和函数 $S(x)$。
***
（Ⅰ）由已知递推关系 $(n+1)a_{n+1}=na_n+a_{n-1}$，得
$$a_{n+1}-a_n=-\frac{1}{n+1}(a_n-a_{n-1})=-\frac{1}{n+1}\cdot\left(-\frac{1}{n}\right)(a_{n-1}-a_{n-2})=\cdots=\frac{(-1)^n}{(n+1)!}(a_1-a_0)=\frac{(-1)^{n+1}}{(n+1)!},$$
故
$$a_{n+1}=a_0+\sum_{k=1}^{n+1}(a_k-a_{k-1})=1+\sum_{k=1}^{n+1}\frac{(-1)^k}{k!}=\sum_{k=0}^{n+1}\frac{(-1)^k}{k!},$$
即 $a_n=\sum_{k=0}^{n}\dfrac{(-1)^k}{k!}$。注意到 $\sum_{n=0}^{\infty}\dfrac{(-1)^nx^n}{n!}=\mathrm{e}^{-x}$，故 $\lim\limits_{n\to\infty}a_n=\mathrm{e}^{-1}$。

由 $\lim\limits_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|=\dfrac{\mathrm{e}^{-1}}{\mathrm{e}^{-1}}=1$，故 $\sum_{n=0}^{\infty}a_nx^n$ 的收敛半径 $R=1$。

（Ⅱ）由 $S(x)=\sum_{n=0}^{\infty}a_nx^n$，有 $S'(x)=\sum_{n=1}^{\infty}na_nx^{n-1}$，则 $xS'(x)=\sum_{n=1}^{\infty}na_nx^n$，将 $na_n=(n+1)a_{n+1}-a_{n-1}$ 代入，得
$$xS'(x)=\sum_{n=1}^{\infty}\left[(n+1)a_{n+1}-a_{n-1}\right]x^n=\sum_{n=1}^{\infty}(n+1)a_{n+1}x^n-\sum_{n=1}^{\infty}a_{n-1}x^n$$
$$=-a_1+\sum_{n=1}^{\infty}na_nx^{n-1}-x\sum_{n=0}^{\infty}a_nx^n=0+\sum_{n=1}^{\infty}na_nx^{n-1}-x\sum_{n=0}^{\infty}a_nx^n=S'(x)-xS(x),$$
即 $(1-x)S'(x)=xS(x)$，变形为 $\dfrac{S'(x)}{S(x)}=\dfrac{x}{1-x}$，积分得
$$\ln|S(x)|=\int\frac{x}{1-x}\mathrm{d}x=-x-\ln(1-x)+C.$$
由 $x=0$，$S(0)=1$ 得 $C=0$，考虑到 $S(0)=1>0$，故 $\ln S(x)=-x-\ln(1-x)$，即
$$S(x)=\frac{\mathrm{e}^{-x}}{1-x},\quad x\in(-1,1).$$

+++

#### 拓展解答 (3) 设 $f(x)$ 满足 $f''(x)+2f'(x)+f(x)=0$，且 $f(0)=1$，$f'(0)=0$，$a_n=\int_n^{+\infty}f(x)\mathrm{d}x$。\
（Ⅰ）求 $f(x)$ 及 $a_n$；\
（Ⅱ）求级数 $\sum_{n=1}^{\infty}a_n$ 的和。
***
（Ⅰ）已知方程的特征方程为 $r^2+2r+1=0$，得特征根为 $r_1=r_2=-1$，故通解为
$$f(x)=C_1\mathrm{e}^{-x}+C_2x\mathrm{e}^{-x}.$$
由 $f(0)=1$，$f'(0)=0$，得 $C_1=C_2=1$。所以
$$f(x)=\mathrm{e}^{-x}+x\mathrm{e}^{-x}=(1+x)\mathrm{e}^{-x}.$$
$$a_n=\int_n^{+\infty}f(x)\mathrm{d}x=\int_n^{+\infty}(1+x)\mathrm{e}^{-x}\mathrm{d}x=-\int_n^{+\infty}(1+x)\mathrm{d}\mathrm{e}^{-x}=-\left[\left.(1+x)\mathrm{e}^{-x}\right|_n^{+\infty}-\int_n^{+\infty}\mathrm{e}^{-x}\mathrm{d}x\right]=(1+n)\mathrm{e}^{-n}+\mathrm{e}^{-n}=n\mathrm{e}^{-n}+2\mathrm{e}^{-n}.$$

（Ⅱ）$\sum_{n=1}^{\infty}a_n=\sum_{n=1}^{\infty}n\mathrm{e}^{-n}+2\sum_{n=1}^{\infty}\mathrm{e}^{-n}$，而 $\sum_{n=1}^{\infty}\mathrm{e}^{-n}=\dfrac{\mathrm{e}^{-1}}{1-\mathrm{e}^{-1}}=\dfrac{1}{\mathrm{e}-1}$。令
$$S(x)=\sum_{n=1}^{\infty}n\mathrm{e}^{-nx}=-\sum_{n=1}^{\infty}\left(\mathrm{e}^{-nx}\right)'=-\left(\sum_{n=1}^{\infty}\mathrm{e}^{-nx}\right)'=-\left(\frac{\mathrm{e}^{-x}}{1-\mathrm{e}^{-x}}\right)'=\frac{\mathrm{e}^x}{\left(\mathrm{e}^x-1\right)^2},\quad x>0.$$
令 $x=1$，则 $\sum_{n=1}^{\infty}n\mathrm{e}^{-n}=S(1)=\dfrac{\mathrm{e}}{(\mathrm{e}-1)^2}$，故
$$\sum_{n=1}^{\infty}a_n=\frac{\mathrm{e}}{(\mathrm{e}-1)^2}+\frac{2}{\mathrm{e}-1}=\frac{3\mathrm{e}-2}{(\mathrm{e}-1)^2}.$$
