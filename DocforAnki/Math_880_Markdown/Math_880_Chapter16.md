---
quizify:
  format: 1
  deck: Math_880::Chapter_16
  tags: [Math, 880题, 数一, 第十六章, 随机事件及其概率]
---

+++

#### 基础选择 (1) 设当事件 $A$ 与 $B$ 同时发生时，事件 $C$ 必发生，则（　）．

;;;
A. $P(C)=P(AB)$
B. $P(C)=P(A\cup B)$
C. $P(C)\leqslant P(A)+P(B)-1$
D. $P(C)\geqslant P(A)+P(B)-1$
;;;D
***
依题设，$AB\subset C$，故

$$1\geqslant P(A\cup B)=P(A)+P(B)-P(AB)\geqslant P(A)+P(B)-P(C),$$

即 $P(C)\geqslant P(A)+P(B)-1$．

仅由 $AB\subset C$，不能推出 $P(C)=P(AB)$ 和 $P(C)=P(A\cup B)$．

+++

#### 基础选择 (2) 对任意两个事件 $A$ 和 $B$，若 $P(AB)=0$，则（　）．

;;;
A. $P(A)P(B)=0$
B. $P(A-B)=P(A)$
C. $\bar{A}\bar{B}=\varnothing$
D. $AB=\varnothing$
;;;B
***
由 $P(AB)=0$，得 $P(A-B)=P(A)-P(AB)=P(A)$．

+++

#### 基础选择 (3) 设 $P(A)>0$，$P(B)>0$，$P(A\mid B)=P(A)$，则下列选项**不正确**的是（　）．

;;;
A. $A$ 与 $B$ 互不相容
B. $A$ 与 $B$ 相容
C. $P(B\mid A)=P(B)$
D. $P(\bar{A}\mid\bar{B})=P(\bar{A})$
;;;A
***
由 $P(A\mid B)=P(A)$ 知，$A,B$ 相互独立，故 C 正确，$\bar{A}$ 与 $\bar{B}$ 也相互独立，D 正确．

因 $P(A)>0$，$P(B)>0$，且 $A,B$ 相互独立，知 $A,B$ 必不互不相容，即相容，故 B 正确．

【注】① 若 $P(A)>0$，$P(B)>0$，则当 $A,B$ 独立时，有 $AB\neq\varnothing$，即 $A,B$ 相容．当 $AB=\varnothing$ 时，有 $A$ 与 $B$ 不独立（见《李林考研数学系列概率论与数理统计辅导讲义》第一章）．

简单地说，在 $P(A)>0$，$P(B)>0$ 的条件下，$A,B$ 相互独立与 $A,B$ 互不相容不能同时成立．

② $A,B$ 相互独立且其概率均大于零，则

$$P(B\mid A)=P(B)\Leftrightarrow P(\bar{B}\mid A)=P(\bar{B})$$

$$\Leftrightarrow P(\bar{A}\mid B)=P(\bar{A})$$

$$\Leftrightarrow P(\bar{A}\mid\bar{B})=P(\bar{A}).$$

+++

#### 基础选择 (4) 设 $A,B,C$ 是三个相互独立的随机事件，且 $0<P(C)<1$，则下列四对事件中**不相互独立**的是（　）．

;;;
A. $\overline{A\cup B}$ 与 $C$
B. $\overline{AC}$ 与 $\bar{C}$
C. $\overline{A-B}$ 与 $\bar{C}$
D. $\overline{AB}$ 与 $\bar{C}$
;;;B
***
由 $A,B,C$ 相互独立，知 $\overline{AB}$ 与 $\bar{C}$ 相互独立，$\overline{A\cup B}$ 与 $C$ 相互独立，$\overline{A-B}$ 与 $\bar{C}$ 相互独立，故排除 A，C，D．

【注】事件 $A,B,C$ 相互独立，"不重叠分组，各自运算后仍独立"（见《李林考研数学系列概率论与数理统计辅导讲义》第一章）．

+++

#### 基础选择 (5) 设 $0<P(A)<1$，$0<P(B)<1$ 且 $P(A\mid B)+P(\bar{A}\mid\bar{B})=1$，则（　）．

;;;
A. $A$ 与 $B$ 互不相容
B. $A$ 与 $B$ 相互独立
C. $A$ 与 $B$ 对立
D. $A$ 与 $B$ 不相互独立
;;;B
***
由 $1-P(\bar{A}\mid\bar{B})=P(A\mid\bar{B})$，知 $P(A\mid B)=P(A\mid\bar{B})$，即

$$\frac{P(AB)}{P(B)}=\frac{P(A\bar{B})}{P(\bar{B})}=\frac{P(A)-P(AB)}{1-P(B)},$$

故可得 $P(AB)=P(A)P(B)$，即 $A,B$ 相互独立．

+++

#### 基础选择 (6) 设 $A,B$ 为任意两个事件，且 $A\subset B$，$P(B)>0$，则下列选项正确的是（　）．

;;;
A. $P(A)<P(A\mid B)$
B. $P(A)\leqslant P(A\mid B)$
C. $P(A)>P(A\mid B)$
D. $P(A)\geqslant P(A\mid B)$
;;;B
***
由 $A\subset B$，得 $AB=A$，$P(B)\leqslant 1$，故

$$P(A\mid B)=\frac{P(AB)}{P(B)}=\frac{P(A)}{P(B)}\geqslant P(A),$$

B 正确．

当 $P(B)=1$ 时，A 不正确；当 $P(B)<1$ 时，C，D 不正确．

+++

#### 基础选择 (7) 设 $A,B$ 是两个随机事件，且 $0<P(A)<1$，$P(B)>0$，$P(B\mid A)=P(B\mid\bar{A})$，则下列选项正确的是（　）．

;;;
A. $P(A\mid B)=P(\bar{A}\mid B)$
B. $P(A\mid B)\neq P(\bar{A}\mid B)$
C. $P(AB)=P(A)P(B)$
D. $P(AB)\neq P(A)P(B)$
;;;C
***
由 $P(B\mid A)=P(B\mid\bar{A})$，得

$$\frac{P(AB)}{P(A)}=\frac{P(B\bar{A})}{P(\bar{A})}=\frac{P(B)-P(AB)}{1-P(A)},$$

故 $P(AB)=P(A)P(B)$，此时，$A,B$ 相互独立，所以

$$P(A\mid B)=P(A),\quad P(\bar{A}\mid B)=P(\bar{A}).$$

由于 $0<P(A)<1$，所以选项 A，B 不一定成立．

+++

#### 基础填空 (1) 设 $P(A\mid B)=P(B\mid A)=\dfrac{1}{2}$，$P(A)=\dfrac{1}{3}$，则 $P(A\cup B)=$ ________．
***
$\dfrac{1}{2}$．

由已知，得

$$P(AB)=P(A)P(B\mid A)=\frac{1}{3}\times\frac{1}{2}=\frac{1}{6},$$

又 $P(AB)=P(B)P(A\mid B)$，知 $P(B)=\dfrac{1}{3}$，故

$$P(A\cup B)=P(A)+P(B)-P(AB)=\frac{1}{3}+\frac{1}{3}-\frac{1}{6}=\frac{1}{2}.$$

+++

#### 基础填空 (2) 已知事件 $A,B$ 相互独立且互不相容，则 $\min\{P(A),P(B)\}=$ ________．
***
$0$．

由已知，$P(A)\geqslant 0$，$P(B)\geqslant 0$，$P(AB)=P(A)P(B)=0$，故 $P(A)$，$P(B)$ 中至少有一个为 $0$，所以 $\min\{P(A),P(B)\}=0$．

+++

#### 基础填空 (3) 设事件 $A,B,C$ 满足 $P(A)=P(B)=P(C)=\dfrac{1}{4}$，$P(AB)=P(BC)=0$，$P(AC)=\dfrac{1}{8}$，则 $A,B,C$ 三个事件中至少出现一个的概率为 ________．
***
$\dfrac{5}{8}$．

由 $ABC\subset AB$，知 $P(ABC)\leqslant P(AB)=0$，所以 $P(ABC)=0$，故所求概率为

$$P(A\cup B\cup C)=P(A)+P(B)+P(C)-P(AB)-P(AC)-P(BC)+P(ABC)$$

$$=\frac{1}{4}+\frac{1}{4}+\frac{1}{4}-0-\frac{1}{8}-0+0=\frac{5}{8}.$$

+++

#### 基础填空 (4) 设 $P(A)=0.1$，$P(B\mid A)=0.9$，$P(B\mid\bar{A})=0.2$，则 $P(A\mid B)=$ ________．
***
$\dfrac{1}{3}$．

由条件概率公式，有 $P(A\mid B)=\dfrac{P(AB)}{P(B)}=\dfrac{P(A)P(B\mid A)}{P(B)}$．又

$$P(B)=P(AB\cup\bar{A}B)=P(AB)+P(\bar{A}B)=P(A)P(B\mid A)+P(\bar{A})P(B\mid\bar{A})$$

$$=0.1\times 0.9+(1-0.1)\times 0.2=0.27,$$

故 $P(A\mid B)=\dfrac{1}{3}$．

【注】$B=\Omega\cdot B=(A+\bar{A})B=AB+\bar{A}B$，$\Omega$ 表示全集，且 $AB$ 与 $\bar{A}B$ 互不相容．

+++

#### 基础填空 (5) 设 $A,B$ 为随机事件，且 $P(\bar{A})=0.3$，$P(B)=0.4$，$P(A-B)=0.5$，则 $P(B\mid A\cup\bar{B})=$ ________．
***
$\dfrac{1}{4}$．

由条件概率公式，有

$$P(B\mid A\cup\bar{B})=\frac{P\big(B\cap(A\cup\bar{B})\big)}{P(A\cup\bar{B})}=\frac{P\big((AB)\cup(B\bar{B})\big)}{P(A\cup\bar{B})}$$

$$=\frac{P(AB)}{P(A\cup\bar{B})}=\frac{P(A)-P(A\bar{B})}{P(A)+P(\bar{B})-P(A\bar{B})}$$

$$=\frac{P(A)-P(A-B)}{P(A)+P(\bar{B})-P(A-B)}=\frac{0.2}{0.8}=\frac{1}{4}.$$

+++

#### 基础填空 (6) 设在三次独立重复试验中，事件 $A$ 发生的概率相等，若已知 $A$ 至少出现一次的概率为 $\dfrac{19}{27}$，则 $A$ 在一次试验中发生的概率 $p=$ ________．
***
$\dfrac{1}{3}$．

依题设，本题为伯努利概型．

设每次试验中事件 $A$ 发生的概率为 $p$，事件 $A$ 发生的次数为 $k\ (k=0,1,\cdots,n)$，则 $A$ 至少发生一次的概率 $P\{k\geqslant 1\}=1-(1-p)^n$，解得

$$p=1-\sqrt[n]{1-P\{k\geqslant 1\}}.$$

由已知，$P\{k\geqslant 1\}=\dfrac{19}{27}$，$n=3$，故 $p=1-\sqrt[3]{1-\dfrac{19}{27}}=\dfrac{1}{3}$．

+++

#### 基础填空 (7) 在区间 $(0,1)$ 内任取两个数 $x,y$，则 $xy\leqslant\dfrac{2}{9}$ 的概率为 ________．
***
$\dfrac{2}{9}\left(1+\ln\dfrac{9}{2}\right)$．

设事件

$$A=\left\{(x,y)\ \middle|\ xy\leqslant\frac{2}{9},\ 0<x<1,\ 0<y<1\right\},$$

$$D=\{(x,y)\mid 0<x<1,\ 0<y<1\},$$

则事件 $A$ 的样本位于区域 $D_1$ 中（如图 16-1 阴影部分所示），由几何概型公式

$$P(A)=\frac{S_{D_1}}{S_D}=\frac{2}{9}\times 1+\int_{\frac{2}{9}}^{1}\frac{2}{9x}\,\mathrm{d}x=\frac{2}{9}\left(1+\ln\frac{9}{2}\right).$$

+++

#### 基础填空 (8) 某人向同一目标独立重复射击，每次射击命中目标的概率为 $p\ (0<p<1)$，则此人第 $6$ 次射击恰好第 $2$ 次命中目标的概率为 ________．
***
$5p^2(1-p)^4$．

依题设，可知第 $6$ 次射击命中且前 $5$ 次射击恰好命中 $1$ 次，故前 $5$ 次射击中恰有 $1$ 次命中的概率为 $C_5^1 p(1-p)^4=5p(1-p)^4$，第 $6$ 次射击恰好第 $2$ 次命中的概率为

$$p\cdot 5p(1-p)^4=5p^2(1-p)^4.$$

+++

#### 基础解答 (1) 设事件 $A,B$ 相互独立，$A,C$ 互不相容，且 $P(A)=0.4$，$P(B)=0.3$，$P(C)=0.4$，$P(B\mid C)=0.2$，求下列概率：（Ⅰ）$P(A\cup B)$；（Ⅱ）$P(C\mid A\cup B)$；（Ⅲ）$P(AB\mid\bar{C})$．
***
（Ⅰ）

$$P(A\cup B)=P(A)+P(B)-P(AB)=P(A)+P(B)-P(A)P(B)$$

$$=0.4+0.3-0.4\times 0.3=0.58.$$

（Ⅱ）

$$P(C\mid A\cup B)=\frac{P[C(A\cup B)]}{P(A\cup B)}=\frac{P(BC)}{P(A\cup B)}$$

$$=\frac{P(C)P(B\mid C)}{P(A\cup B)}=\frac{0.4\times 0.2}{0.58}\approx 0.138.$$

（Ⅲ）

$$P(AB\mid\bar{C})=\frac{P(AB\bar{C})}{P(\bar{C})}=\frac{P(AB)}{1-P(C)}$$

$$=\frac{P(A)P(B)}{1-P(C)}=\frac{0.4\times 0.3}{1-0.4}=0.2.$$

+++

#### 基础解答 (2) 设 $A_1,A_2,\cdots,A_n$ 为 $n$ 个相互独立的事件，且 $P(A_k)=p_k\ (k=1,2,\cdots,n)$，求下列事件的概率：（Ⅰ）$A=\{n$ 个事件全不发生$\}$；（Ⅱ）$B=\{n$ 个事件不全发生$\}$；（Ⅲ）$C=\{n$ 个事件中至少有一个发生$\}$．
***
（Ⅰ）$n$ 个事件全不发生，即 $n$ 个事件的对立事件同时发生，故

$$P(A)=P(\bar{A}_1\bar{A}_2\cdots\bar{A}_n)=\prod_{k=1}^{n}P(\bar{A}_k)=\prod_{k=1}^{n}(1-p_k).$$

（Ⅱ）$n$ 个事件不全发生，即 $n$ 个事件中至多有 $n-1$ 个发生，故

$$P(B)=1-P\{A_1A_2\cdots A_n\}=1-\prod_{k=1}^{n}P(A_k)=1-\prod_{k=1}^{n}p_k.$$

（Ⅲ）

$$P(C)=P(A_1\cup A_2\cup\cdots\cup A_n)=1-P\left(\bigcap_{k=1}^{n}\bar{A}_k\right)=1-\prod_{k=1}^{n}(1-p_k).$$

+++

#### 基础解答 (3) 对某一目标依次进行了三次独立的射击，设第一、第二、第三次射击命中的概率分别为 $0.4,0.5$ 和 $0.7$，求：（Ⅰ）三次射击中恰好有一次命中的概率；（Ⅱ）三次射击中至少有一次命中的概率．
***
设 $A_i=\{$第 $i$ 次命中$\}\ (i=1,2,3)$，$B$ 为恰有一次命中，$C$ 为至少有一次命中，则 $B=A_1\bar{A}_2\bar{A}_3\cup\bar{A}_1A_2\bar{A}_3\cup\bar{A}_1\bar{A}_2A_3$，$C=A_1\cup A_2\cup A_3$．

（Ⅰ）由已知，$A_1,A_2,A_3$ 相互独立且互不相容，故

$$P(B)=P(A_1\bar{A}_2\bar{A}_3)+P(\bar{A}_1A_2\bar{A}_3)+P(\bar{A}_1\bar{A}_2A_3)$$

$$=P(A_1)P(\bar{A}_2)P(\bar{A}_3)+P(\bar{A}_1)P(A_2)P(\bar{A}_3)+P(\bar{A}_1)P(\bar{A}_2)P(A_3)$$

$$=0.4\times 0.5\times 0.3+0.6\times 0.5\times 0.3+0.6\times 0.5\times 0.7=0.36.$$

（Ⅱ）

$$P(C)=P(A_1\cup A_2\cup A_3)=1-P(\overline{A_1\cup A_2\cup A_3})=1-P(\bar{A}_1\bar{A}_2\bar{A}_3)$$

$$=1-P(\bar{A}_1)P(\bar{A}_2)P(\bar{A}_3)=1-0.6\times 0.5\times 0.3=0.91.$$

+++

#### 基础解答 (4) 设 $A,B$ 是两个随机事件，证明：$1-P(\bar{A})-P(\bar{B})\leqslant P(AB)\leqslant P(A\cup B)\leqslant P(A)+P(B)$．
***
由 $P(A\cup B)=P(A)+P(B)-P(AB)$，而 $P(AB)\geqslant 0$，故

$$P(A\cup B)\leqslant P(A)+P(B).$$

而 $AB\subset A\cup B$，所以 $P(AB)\leqslant P(A\cup B)$．又由

$$1-P(\bar{A})-P(\bar{B})=1-[1-P(A)]-[1-P(B)]$$

$$=P(A)+P(B)-1=P(AB)+P(A\cup B)-1$$

$$=P(AB)-[1-P(A\cup B)]\leqslant P(AB).$$

综上所述，命题得证．

+++

#### 综合选择 (1) 设某人毫无准备地参加一项测验，其中有 $5$ 道是非题，他随机地选择"是"或"非"，则该人至少答对 $1$ 题的概率为（　）．

;;;
A. $\dfrac{1}{5}$
B. $\dfrac{1}{32}$
C. $\dfrac{5}{32}$
D. $\dfrac{31}{32}$
;;;D
***
设 $A_i=\{$第 $i$ 题答对$\}$，则 $P(A_i)=\dfrac{1}{2}\ (i=1,2,\cdots,5)$，由于是随机选择，故

$$P\left(\bigcup_{i=1}^{5}A_i\right)=1-P\left(\bigcap_{i=1}^{5}\bar{A}_i\right)=1-\prod_{i=1}^{5}P(\bar{A}_i)=1-\left(\frac{1}{2}\right)^5=\frac{31}{32}.$$

+++

#### 综合选择 (2) 有一根长为 $L$ 的木棒，将其任意折成三段，记事件 $A=\{$中间一段为三段中的最长者$\}$，则 $P(A)=$（　）．

;;;
A. $\dfrac{1}{2}$
B. $\dfrac{1}{3}$
C. $\dfrac{1}{4}$
D. $\dfrac{2}{3}$
;;;B
***
此问题是几何概型．

设折得的三段长度依次为 $x,L-x-y,y$，则样本空间为

$$\Omega=\{(x,y)\mid 0\leqslant x\leqslant L,\ 0\leqslant y\leqslant L,\ 0\leqslant x+y\leqslant L\}.$$

事件 $A$ 相应的子区域 $\Omega_1$，应满足 $0<x<L-x-y$，$0<y<L-x-y$，即

$$\Omega_1=\left\{(x,y)\ \middle|\ 0<y<L-2x,\ 0<y<\frac{1}{2}(L-x)\right\},$$

如图 16-2 所示，可知 $\Omega$ 的面积为 $\dfrac{1}{2}L^2$，$\Omega_1$ 的面积为 $\dfrac{1}{6}L^2$，故

$$P(A)=\frac{\frac{1}{6}L^2}{\frac{1}{2}L^2}=\frac{1}{3}.$$

+++

#### 综合填空 (1) 设甲、乙两人独立地对同一目标射击一次，其命中率分别为 $0.5$ 和 $0.4$，已知目标被命中，则它是乙射中的概率为 ________．
***
$\dfrac{4}{7}$．

设 $A=\{$甲射击一次命中目标$\}$，$B=\{$乙射击一次命中目标$\}$，由已知，所求概率为

$$P(B\mid A\cup B)=\frac{P\big(B(A\cup B)\big)}{P(A\cup B)}=\frac{P(B)}{P(A\cup B)},$$

其中 $A\cup B$ 表示目标被命中．又

$$P(A\cup B)=P(A)+P(B)-P(AB)=P(A)+P(B)-P(A)P(B)$$

$$=0.5+0.4-0.5\times 0.4=0.7,$$

故 $P(B\mid A\cup B)=\dfrac{0.4}{0.7}=\dfrac{4}{7}$．

+++

#### 综合填空 (2) 设 $P(A)=0.5$，$P(B)=0.7$，则 $P(A\cup B)$ 的最大值与最小值分别是 ________．
***
$1,\ 0.7$．

由 $P(A)+P(B)=0.5+0.7>1$，此时 $AB\neq\varnothing$，所以 $P(AB)$ 的最小值为 $0.2$，故 $P(A\cup B)$ 的最大值为 $1$．

又当 $A\subset B$ 或 $A\supset B$，会使 $A\cup B$ 最小，本题应取 $A\subset B$，故 $P(A\cup B)=P(B)=0.7$ 为最小值．

+++

#### 综合填空 (3) 设 $A,B$ 是两个随机事件，$0<P(B)<1$，$AB=\bar{A}\bar{B}$，则 $P(\bar{A}\mid B)+P(A\mid\bar{B})=$ ________．
***
$2$．

由 $AB=\bar{A}\bar{B}$，知 $(AB)(\bar{A}\bar{B})=A\bar{A}B\bar{B}=\varnothing$，而 $(AB)(\bar{A}\bar{B})=AB=\bar{A}\bar{B}$，所以 $\bar{A}\bar{B}=\varnothing$．

又由对偶律 $\bar{A}\bar{B}=\overline{A\cup B}=\varnothing$，故 $A\cup B=\Omega$（$\Omega$ 表示全集），从而 $A$ 与 $B$ 为对立事件（因 $AB=\varnothing$），于是 $A=\bar{B}$，$\bar{A}=B$，故

$$P(\bar{A}\mid B)+P(A\mid\bar{B})=2.$$

+++

#### 综合填空 (4) 设进行一系列独立试验，每次试验成功的概率均为 $p$，则在试验成功 $2$ 次之前已经失败 $3$ 次的概率为 ________．
***
$4p^2(1-p)^3$．

令 $A=\{$试验成功 $2$ 次之前已经失败 $3$ 次$\}$，$A_5=\{$第 $5$ 次试验成功$\}$，$B_3=\{$试验 $4$ 次失败 $3$ 次$\}$．

依题设，$A_5$ 与 $B_3$ 独立，且 $A=A_5B_3$，而

$$P(B_3)=C_4^1 p(1-p)^3=4p(1-p)^3,\quad P(A_5)=p,$$

故

$$P(A)=P(A_5B_3)=P(A_5)\cdot P(B_3)=4p^2(1-p)^3.$$

+++

#### 综合填空 (5) 已知 $10$ 部手机中有 $7$ 个合格品和 $3$ 个次品，每次任取一个作测试，测试后不放回，直到将 $3$ 个次品都找到为止，则需要测试 $7$ 次的概率为 ________．
***
$\dfrac{2}{15}$．

用古典概型计算．

测试 $7$ 次，就是从 $10$ 件手机中不放回地抽取 $7$ 件，故基本事件总数为 $A_{10}^{7}$．

设 $A=\{7$ 次测试后 $3$ 个次品都已找到$\}$，故存在两种情况：第一种情况是在前 $6$ 次测试中有 $2$ 次找到次品，而在第 $7$ 次测试时找到最后一个次品；第二种情况是前 $7$ 次测试均为合格品，最后剩下的 $3$ 件就是次品．所以 $A$ 所包含的基本事件数为 $C_6^2\cdot C_4^2\cdot A_7^4\cdot 3!+C_7^7\cdot 7!$，故

$$P(A)=\frac{C_6^2\cdot C_4^2\cdot A_7^4\cdot 3!+C_7^7\cdot 7!}{A_{10}^{7}}=\frac{2}{15}.$$

+++

#### 综合填空 (6) 在 $n$ 重伯努利试验中，事件 $A$ 发生的概率为 $p$，则事件 $A$ 发生奇数次的概率为 ________．
***
$\dfrac{1}{2}\left[1-(1-2p)^n\right]$．

设 $A_1=\{n$ 次试验中 $A$ 出现奇数次$\}$，$A_2=\{n$ 次试验中 $A$ 出现偶数次$\}$，则

$$P(A_1)=C_n^1 pq^{n-1}+C_n^3 p^3 q^{n-3}+C_n^5 p^5 q^{n-5}+\cdots,$$

$$P(A_2)=C_n^0 p^0 q^{n}+C_n^2 p^2 q^{n-2}+C_n^4 p^4 q^{n-4}+\cdots,$$

其中 $q=1-p$，故

$$P(A_1)+P(A_2)=(p+q)^n=1,$$

$$P(A_2)-P(A_1)=(q-p)^n=(1-2p)^n,$$

两式相减，得所求概率为 $P(A_1)=\dfrac{1}{2}\left[1-(1-2p)^n\right]$．

+++

#### 综合解答 (1) 设甲盒中有 $4$ 个红球和 $2$ 个白球，乙盒中有 $2$ 个红球和 $4$ 个白球，掷一枚均匀的硬币，若正面出现，则从甲盒中任取一球，若反面出现，则从乙盒中任取一球，设每次取出的球观看颜色后放回原盒中．（Ⅰ）若前两次都取得红球，求第三次也取得红球的概率；（Ⅱ）若前两次都取得红球，求红球都来自甲盒的概率．
***
（Ⅰ）设 $A_i=\{$第 $i$ 次取得红球$\}\ (i=1,2,3)$，$B_j=\{$第 $j$ 次掷硬币出现正面$\}\ (j=1,2,3)$．

依题设，易知 $B_j$ 为第 $j$ 次从甲盒中取球．将"掷一次硬币，再由硬币出现的结果从相应的盒中取出"看作一次试验，则每次试验是重复的，且相互独立，所以它们的结果 $A_1,A_2,A_3$ 是相互独立的，且

$$P(A_i)=P(A_1),\quad i=1,2,3,$$

故所求概率为 $P(A_3\mid A_1A_2)=P(A_3)=P(A_1)$．

又由全概率公式，得

$$P(A_1)=P(B_1)P(A_1\mid B_1)+P(\bar{B}_1)P(A_1\mid\bar{B}_1)$$

$$=\frac{1}{2}\times\frac{4}{6}+\frac{1}{2}\times\frac{2}{6}=\frac{1}{2},$$

故 $P(A_3\mid A_1A_2)=\dfrac{1}{2}$．

（Ⅱ）由于两次试验是独立重复的，所以 $A_1B_1$ 与 $A_2B_2$ 是相互独立的，且

$$P(A_2B_2)=P(A_1B_1)=P(B_1)P(A_1\mid B_1)=\frac{1}{2}\times\frac{4}{6}=\frac{1}{3}.$$

由条件概率公式，得

$$P(B_1B_2\mid A_1A_2)=\frac{P(A_1A_2B_1B_2)}{P(A_1A_2)}=\frac{P(A_1B_1)P(A_2B_2)}{P(A_1)P(A_2)}=\frac{\left(\frac{1}{3}\right)^2}{\left(\frac{1}{2}\right)^2}=\frac{4}{9}.$$

+++

#### 综合解答 (2) 设一批产品中有 $15\%$ 的次品，进行独立重复抽样检验，若抽取 $20$ 个样品，则抽出的 $20$ 个样品中，可能性最大的次品数是多少？并求其概率．
***
设 $X=\{$抽取 $20$ 个样品中的次品数$\}$，则 $X\sim B(20,0.15)$．所求问题是，当 $k$ 为多少时，$P\{X=k\}=C_{20}^{k}\times 0.15^k\times(1-0.15)^{20-k}\ (k=0,1,\cdots,20)$ 最大．

设当 $k=k_0$ 时，$P\{X=k\}$ 最大，则有

$$P\{X=k_0\}\geqslant P\{X=k_0-1\},\quad P\{X=k_0\}\geqslant P\{X=k_0+1\},$$

考虑任意两项的比值，

$$\frac{P\{X=k\}}{P\{X=k-1\}}=\frac{C_{20}^{k}\times 0.15^k\times 0.85^{20-k}}{C_{20}^{k-1}\times 0.15^{k-1}\times 0.85^{20-k+1}}=\frac{(20-k+1)\times 0.15}{0.85\times k},$$

则 $P\{X=k\}\geqslant P\{X=k-1\}$，当且仅当 $k\leqslant(20+1)\times 0.15=3.15$．

同理，$P\{X=k\}\geqslant P\{X=k+1\}$，当且仅当 $k\geqslant(20+1)\times 0.15-1=2.15$，故当 $P\{X=k\}$ 最大时，$k=3$，且

$$P\{X=3\}=C_{20}^{3}\times 0.15^3\times 0.85^{17}\approx 0.242\,8.$$

【注】本题是求二项分布中最大可能目标数，一般结论是：若 $X\sim B(n,p)$，如果 $(n+1)p$ 不是整数，则当 $k=[(n+1)p]$（向下取整）时，$P\{X=k\}$ 取得最大值；如果 $(n+1)p$ 是整数，则当 $k=(n+1)p$ 或 $k=(n+1)p-1$ 时，$P\{X=k\}$ 取得最大值．

如本题，$[(20+1)\times 0.15]=[3.15]=3$．

+++

#### 拓展解答 (1) 有三个盒子，第一个盒子中有 $3$ 个黑球、$1$ 个白球，第二个盒子中有 $2$ 个黑球、$3$ 个白球，第三个盒子中有 $3$ 个黑球、$2$ 个白球．（Ⅰ）任取一个盒子，再从该盒子中取出一个球，求这个球是白球的概率；（Ⅱ）已知取出的是白球，求此球属于第三个盒子的概率．
***
（Ⅰ）设 $A=\{$取出的是白球$\}$，$B_i=\{$取到第 $i$ 只盒子$\}$，$i=1,2,3$．

依题设，$P(B_i)=\dfrac{1}{3}$，由全概率公式，得

$$P(A)=\sum_{i=1}^{3}P(B_i)P(A\mid B_i)=\frac{1}{3}\times\left(\frac{1}{4}+\frac{3}{5}+\frac{2}{5}\right)=\frac{5}{12}.$$

（Ⅱ）由（Ⅰ）及贝叶斯公式，得

$$P(B_3\mid A)=\frac{P(B_3)P(A\mid B_3)}{P(A)}=\frac{\frac{1}{3}\times\frac{2}{5}}{\frac{5}{12}}=\frac{8}{25}.$$

+++

#### 拓展解答 (2) 从 $1,2,\cdots,n$ 这 $n$ 个数中任意相继不放回地取出两个数，求取出的第二个数比第一个数大的概率．
***
令 $A_i=\{$第一次取出的数为 $i\}$，$i=1,2,\cdots,n$，$B=\{$取出的第二个数比第一个数大$\}$，则 $A_1,A_2,\cdots,A_n$ 构成一个完备事件组．

由于在 $A_i$ 发生的条件下，第二个数只能取到余下的 $n-1$ 个数之一，且只有它取到后 $n-i$ 个数时，$B$ 才发生，故 $P(B\mid A_i)=\dfrac{n-i}{n-1}$，$i=1,2,\cdots,n$．

又 $P(A_i)=\dfrac{1}{n}$，$i=1,2,\cdots,n$，由全概率公式，有

$$P(B)=\sum_{i=1}^{n}P(A_i)P(B\mid A_i)=\sum_{i=1}^{n}\frac{1}{n}\cdot\frac{n-i}{n-1}$$

$$=\frac{1}{n(n-1)}\left[(n-1)+(n-2)+\cdots+1+0\right]$$

$$=\frac{1}{n(n-1)}\cdot\frac{n(n-1)}{2}=\frac{1}{2}.$$

【注】由于此题所求事件较复杂，故不易直接用古典概型计算，但通过全概率公式所得结果与直觉是吻合的．
