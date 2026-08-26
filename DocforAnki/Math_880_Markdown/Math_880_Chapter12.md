---
quizify:
  format: 1
  deck: Math_880::Chapter_12
  tags: [Math, 880题, 数一, 第十二章, 向量]
---

+++

#### 基础选择 (1) 若 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，$\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，则（　）．

;;;
A. $\boldsymbol{\alpha}_1$ 可由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示
B. $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示
C. $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_3$ 线性表示
D. $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性表示
;;;A
***
对于 A：由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，知 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，故 $\boldsymbol{\alpha}_1$ 必能由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．

对于 B：若 $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，而 $\boldsymbol{\alpha}_1$ 又能由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，则 $\boldsymbol{\alpha}_4$ 就能由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，这与 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关矛盾，故 $\boldsymbol{\alpha}_4$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，所以 B 不正确．

同样，C，D 也是错误的．

+++

#### 基础选择 (2) 向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 线性无关等价于（　）．

;;;
A. 存在一组不全为 $0$ 的数，使其线性组合不为 $\boldsymbol{0}$
B. 存在一个向量不能由其他向量线性表示
C. 任何一个向量均不能由其他向量线性表示
D. 其中任意两个向量线性无关
;;;C
***
由线性无关的定义，知 A，B 不正确．

对于 D：由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 线性无关，知任意两个向量也线性无关，但反过来不成立，如 $\begin{pmatrix}1\\0\end{pmatrix},\begin{pmatrix}0\\1\end{pmatrix},\begin{pmatrix}1\\1\end{pmatrix}$，其中任两个向量均线性无关，但三个 $2$ 维向量显然线性相关．

【注】讨论向量组线性相关性的常用方法．

① 判别 $n$ 维向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s$ 线性相关的步骤：\
（i）当 $s>n$ 时，必线性相关；\
（ii）当 $s=n$ 时，行列式 $|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s)|=0$；\
（iii）当 $s<n$ 时，$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s)<s$．

② 利用线性相关（无关）的等价说法：

列向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s$ 线性相关（无关）$\Leftrightarrow$ 方程组 $(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s)\begin{pmatrix}x_1\\x_2\\\vdots\\x_s\end{pmatrix}=\boldsymbol{0}$ 有非零解（只有零解）$\Leftrightarrow r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s)<s\ (=s)$．

③ 证明 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s$ 线性无关的常用方法：\
（i）定义法：设 $k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+\cdots+k_s\boldsymbol{\alpha}_s=\boldsymbol{0}$，经恒等变形（上式乘以数、向量、矩阵，重组）证 $k_1=k_2=\cdots=k_s=0$；\
（ii）用行列式或秩；\
（iii）反证法．

+++

#### 基础选择 (3) 设向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，则下列向量组线性无关的是（　）．

;;;
A. $\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_4,\boldsymbol{\alpha}_4+\boldsymbol{\alpha}_1$
B. $\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_4,\boldsymbol{\alpha}_4-\boldsymbol{\alpha}_1$
C. $\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2-\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_4,\boldsymbol{\alpha}_4-\boldsymbol{\alpha}_1$
D. $\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2-\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3-\boldsymbol{\alpha}_4,\boldsymbol{\alpha}_4-\boldsymbol{\alpha}_1$
;;;B
***
考虑到选项中每个向量均为 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 的线性组合，可直接利用结论，记

$$\boldsymbol{\beta}_1=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\quad \boldsymbol{\beta}_2=\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\quad \boldsymbol{\beta}_3=\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_4,\quad \boldsymbol{\beta}_4=\boldsymbol{\alpha}_4-\boldsymbol{\alpha}_1,$$

则

$$(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)\begin{pmatrix}1&0&0&-1\\1&1&0&0\\0&1&1&0\\0&0&1&1\end{pmatrix}\xlongequal{\text{记}}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)\cdot\boldsymbol{C},$$

由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，及 $|\boldsymbol{C}|=2\neq 0$，即 $\boldsymbol{C}$ 可逆，故 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4$ 线性无关．

【注】① 结论可用线性无关的定义或秩证明．

② 作为选择题也可用排除法，即观察出线性相关的选项，加以排除，如 A 选项，显然

$$(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2)-(\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3)+(\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_4)-(\boldsymbol{\alpha}_4+\boldsymbol{\alpha}_1)=\boldsymbol{0},$$

故线性相关，可排除 A．

+++

#### 基础选择 (4) 设向量组（Ⅰ）$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_t$，（Ⅱ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s$，则下列命题正确的是（　）．

① 若向量组（Ⅰ）可由（Ⅱ）线性表示，且 $s<t$，则必有（Ⅰ）线性相关\
② 若向量组（Ⅱ）可由（Ⅰ）线性表示，且 $s<t$，则必有（Ⅰ）线性相关\
③ 若向量组（Ⅰ）可由（Ⅱ）线性表示，且（Ⅰ）线性无关，则必有 $s\geqslant t$\
④ 若向量组（Ⅱ）可由（Ⅰ）线性表示，且（Ⅰ）线性无关，则必有 $s\geqslant t$

;;;
A. ①④
B. ①③
C. ②③
D. ②④
;;;B
***
由结论"以少表多，多的相关"，命题 ① 正确，而命题 ③ 是命题 ① 的逆否命题，故命题 ① 和命题 ③ 正确．

如 $\boldsymbol{\beta}_1=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2$，$\boldsymbol{\beta}_2=\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2$，$\boldsymbol{\beta}_3=\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2$，则 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 必线性相关．

+++

#### 基础选择 (5) 设 $\boldsymbol{\alpha}_1=(a_1,a_2,a_3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(b_1,b_2,b_3)^{\mathrm{T}},\boldsymbol{\alpha}_3=(c_1,c_2,c_3)^{\mathrm{T}}$，其中 $a_i^2+b_i^2\neq 0\ (i=1,2,3)$，则三条直线 $a_ix+b_iy+c_i=0\ (i=1,2,3)$ 恰好仅交于一点的充要条件是（　）．

;;;
A. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=3$
B. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=1$
C. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2)$
D. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2)=2$
;;;D
***
三条直线交于一点，等价于有唯一的 $x,y$ 满足方程组

$$\begin{cases}a_1x+b_1y+c_1=0,\\a_2x+b_2y+c_2=0,\\a_3x+b_3y+c_3=0,\end{cases}$$

写成向量形式，即有唯一的 $x,y$ 使得下列等式成立，

$$x\begin{pmatrix}a_1\\a_2\\a_3\end{pmatrix}+y\begin{pmatrix}b_1\\b_2\\b_3\end{pmatrix}=-\begin{pmatrix}c_1\\c_2\\c_3\end{pmatrix},$$

即 $x\boldsymbol{\alpha}_1+y\boldsymbol{\alpha}_2=-\boldsymbol{\alpha}_3$，所以 $\boldsymbol{\alpha}_3$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性表示，且表示法唯一，从而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，故

$$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2)=2.$$

【注】C 选项：$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2)$，只能说明 $\boldsymbol{\alpha}_3$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性表示，即三条直线有交点．但 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2)$ 可能为 $2$ 或 $1$，所以不能确定交点只有一个．

+++

#### 基础选择 (6) 设 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 均为 $3$ 维向量，则对任意常数 $k$ 和 $\mu$，向量组 $\boldsymbol{\alpha}_1+k\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2+\mu\boldsymbol{\alpha}_3$ 线性无关是向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关的（　）．

;;;
A. 充分必要条件
B. 充分非必要条件
C. 必要非充分条件
D. 既非充分又非必要条件
;;;C
***
记 $\boldsymbol{\beta}_1=\boldsymbol{\alpha}_1+k\boldsymbol{\alpha}_3$，$\boldsymbol{\beta}_2=\boldsymbol{\alpha}_2+\mu\boldsymbol{\alpha}_3$，则 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}1&0\\0&1\\k&\mu\end{pmatrix}$．

若 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，则矩阵 $(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$ 可逆，故

$$r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2)=r\left(\begin{pmatrix}1&0\\0&1\\k&\mu\end{pmatrix}\right)=2,$$

所以 $\boldsymbol{\alpha}_1+k\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2+\mu\boldsymbol{\alpha}_3$ 线性无关．

反之，若 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，取 $\boldsymbol{\alpha}_3=\boldsymbol{0}$，则对任意 $k,\mu$，必有 $\boldsymbol{\alpha}_1+k\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2+\mu\boldsymbol{\alpha}_3$ 线性无关，但 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，故为**必要非充分条件**．

+++

#### 基础填空 (1) 已知向量 $\boldsymbol{\alpha}_1=(1,2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(2,-1,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-2,k,4)^{\mathrm{T}}$ 线性相关，则 $k=$ ________．
***
$6$．

对于 $3$ 个 $3$ 维向量线性相关性的问题，用行列式或秩．本题用秩进行计算．

$$\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=\begin{pmatrix}1&2&-2\\2&-1&k\\3&1&4\end{pmatrix}\rightarrow\begin{pmatrix}1&2&-2\\0&-5&k+4\\0&-5&10\end{pmatrix}\rightarrow\begin{pmatrix}1&2&-2\\0&-5&k+4\\0&0&6-k\end{pmatrix},$$

由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，则 $r(\boldsymbol{A})<3$，故 $k=6$．

+++

#### 基础填空 (2) 已知 $3$ 维线性空间的一组基为 $\boldsymbol{\alpha}_1=(1,1,0),\boldsymbol{\alpha}_2=(1,0,1),\boldsymbol{\alpha}_3=(0,1,1)$，则向量 $\boldsymbol{\beta}=(2,0,0)$ 在上述基下的坐标为 ________．
***
$(1,1,-1)$．

设 $\boldsymbol{\beta}$ 在基 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 下的坐标为 $(x_1,x_2,x_3)$，则 $\boldsymbol{\beta}=x_1\boldsymbol{\alpha}_1+x_2\boldsymbol{\alpha}_2+x_3\boldsymbol{\alpha}_3$，即

$$\begin{cases}x_1+x_2=2,\\x_1+x_3=0,\\x_2+x_3=0,\end{cases}$$

解方程组，得 $x_1=x_2=1,x_3=-1$，故 $\boldsymbol{\beta}$ 在基下的坐标为 $(1,1,-1)$．

+++

#### 基础填空 (3) 设 $3$ 维向量空间的两组基分别为 $\boldsymbol{\alpha}_1=(1,2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(2,3,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(3,1,2)^{\mathrm{T}}$；$\boldsymbol{\beta}_1=(-1,-1,2)^{\mathrm{T}},\boldsymbol{\beta}_2=(-1,2,-1)^{\mathrm{T}},\boldsymbol{\beta}_3=(3,1,2)^{\mathrm{T}}$，则从 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 到 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 的过渡矩阵为 ________．
***
$\begin{pmatrix}1&0&0\\-1&1&0\\0&-1&1\end{pmatrix}$．

设过渡矩阵为 $\boldsymbol{P}$，则 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\boldsymbol{P}$，则

$$\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)^{-1}(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=\begin{pmatrix}1&2&3\\2&3&1\\3&1&2\end{pmatrix}^{-1}\begin{pmatrix}-1&-1&3\\-1&2&1\\2&-1&2\end{pmatrix}=\begin{pmatrix}1&0&0\\-1&1&0\\0&-1&1\end{pmatrix}.$$

+++

#### 基础解答 (1) 设向量组 $\boldsymbol{\alpha}_1=(1,1,1,2)^{\mathrm{T}},\boldsymbol{\alpha}_2=(3,a+4,2a+5,a+7)^{\mathrm{T}},\boldsymbol{\alpha}_3=(4,6,8,10)^{\mathrm{T}},\boldsymbol{\alpha}_4=(2,3,2a+3,5)^{\mathrm{T}},\boldsymbol{\alpha}=(0,1,3,b)^{\mathrm{T}}$．

（Ⅰ）求向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 的秩及其一个极大线性无关组；\
（Ⅱ）若 $\boldsymbol{\alpha}$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性表示，求 $a,b$ 的取值．
***
对 $(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4\ \vdots\ \boldsymbol{\alpha})$ 作初等行变换，有

$$(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4\ \vdots\ \boldsymbol{\alpha})=\begin{pmatrix}1&3&4&2&0\\1&a+4&6&3&1\\1&2a+5&8&2a+3&3\\2&a+7&10&5&b\end{pmatrix}$$

$$\rightarrow\begin{pmatrix}1&3&4&2&0\\0&a+1&2&1&1\\0&2a+2&4&2a+1&3\\0&a+1&2&1&b\end{pmatrix}\rightarrow\begin{pmatrix}1&3&4&2&0\\0&a+1&2&1&1\\0&0&0&2a-1&1\\0&0&0&0&b-1\end{pmatrix}.$$

（Ⅰ）当 $a\neq\dfrac{1}{2}$ 时，$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=3$，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 是一个极大线性无关组；

当 $a=\dfrac{1}{2}$ 时，$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=2$，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 是一个极大线性无关组．

（Ⅱ）由于 $\boldsymbol{\alpha}$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性表示，即方程组 $x_1\boldsymbol{\alpha}_1+x_2\boldsymbol{\alpha}_2+x_3\boldsymbol{\alpha}_3+x_4\boldsymbol{\alpha}_4=\boldsymbol{\alpha}$ 无解，故 $a=\dfrac{1}{2}$ 或 $b\neq 1$．

+++

#### 基础解答 (2) 设向量组 $\boldsymbol{\alpha}_1=(0,4,2)^{\mathrm{T}},\boldsymbol{\alpha}_2=(1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-2,4,3)^{\mathrm{T}},\boldsymbol{\alpha}_4=(-1,1,1)^{\mathrm{T}}$，求 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 的一个极大线性无关组，并将其余向量用极大线性无关组线性表示．
***
利用结论：列（行）向量组作初等行（列）变换，相关性不变（且向量的位置不变）．

$$(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=\begin{pmatrix}0&1&-2&-1\\4&1&4&1\\2&0&3&1\end{pmatrix}\rightarrow\begin{pmatrix}2&0&3&1\\4&1&4&1\\0&1&-2&-1\end{pmatrix}$$

$$\rightarrow\begin{pmatrix}2&0&3&1\\0&1&-2&-1\\0&1&-2&-1\end{pmatrix}\rightarrow\begin{pmatrix}2&0&3&1\\0&1&-2&-1\\0&0&0&0\end{pmatrix}\rightarrow\begin{pmatrix}1&0&\dfrac{3}{2}&\dfrac{1}{2}\\0&1&-2&-1\\0&0&0&0\end{pmatrix},$$

则 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=2$，故取 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 为一个极大线性无关组，且

$$\boldsymbol{\alpha}_3=\frac{3}{2}\boldsymbol{\alpha}_1-2\boldsymbol{\alpha}_2,\quad \boldsymbol{\alpha}_4=\frac{1}{2}\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2.$$

【注】由矩阵 $\begin{pmatrix}2&0&3&1\\0&1&-2&-1\\0&0&0&0\end{pmatrix}$，得 $\boldsymbol{\alpha}_3=3\boldsymbol{\alpha}_1-2\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_4=\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2$ 是错误的．

+++

#### 基础解答 (3) 设 $\boldsymbol{\alpha}_1=(1,0,2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(1,1,3,5)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,-1,a,1)^{\mathrm{T}},\boldsymbol{\beta}=(1,b,4,7)^{\mathrm{T}}$，$a,b$ 为何值时，$\boldsymbol{\beta}$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示；$a,b$ 为何值时，$\boldsymbol{\beta}$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，并写出表达式．
***
$\boldsymbol{\beta}$ 是否可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，等价于方程组 $\boldsymbol{\beta}=x_1\boldsymbol{\alpha}_1+x_2\boldsymbol{\alpha}_2+x_3\boldsymbol{\alpha}_3$ 是否有解，即考虑方程组

$$\begin{cases}x_1+x_2+x_3=1,\\x_2-x_3=b,\\2x_1+3x_2+ax_3=4,\\3x_1+5x_2+x_3=7,\end{cases}\qquad ①$$

对 ① 的增广矩阵作初等行变换化为阶梯形，

$$\overline{\boldsymbol{A}}=\begin{pmatrix}1&1&1&1\\0&1&-1&b\\2&3&a&4\\3&5&1&7\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1&1\\0&1&-1&b\\0&1&a-2&2\\0&2&-2&4\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1&1\\0&1&-1&b\\0&0&a-1&2-b\\0&0&0&4-2b\end{pmatrix}.$$

（Ⅰ）当 $4-2b\neq 0$，即 $b\neq 2$ 时，方程组无解，此时 $\boldsymbol{\beta}$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．

（Ⅱ）当 $b=2$ 且 $a\neq 1$ 时，$r(\boldsymbol{A})=r(\overline{\boldsymbol{A}})=3$，方程组有唯一解 $(-1,2,0)^{\mathrm{T}}$，即

$$\boldsymbol{\beta}=-\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2,$$

线性表示唯一．

（Ⅲ）当 $b=2$ 且 $a=1$ 时，$r(\boldsymbol{A})=r(\overline{\boldsymbol{A}})=2<3$，方程组有无穷多解．令 $x_3=t$，则 $x_2=t+2$，$x_1=-1-2t$（$t$ 为任意常数），故

$$\boldsymbol{\beta}=(-1-2t)\boldsymbol{\alpha}_1+(2+t)\boldsymbol{\alpha}_2+t\boldsymbol{\alpha}_3,$$

线性表示不唯一．

【注】此类含参数的向量组的线性表示以及互为线性表示（等价）问题是常考题型．

+++

#### 基础解答 (4) 设向量组 $\boldsymbol{\alpha}_1=(1,2,-3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(3,0,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(9,6,-7)^{\mathrm{T}}$ 与向量组 $\boldsymbol{\beta}_1=(0,1,-1)^{\mathrm{T}},\boldsymbol{\beta}_2=(k,2,1)^{\mathrm{T}},\boldsymbol{\beta}_3=(\mu,1,0)^{\mathrm{T}}$ 有相同的秩，且 $\boldsymbol{\beta}_3$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，求 $k,\mu$ 的值．
***
由 $\boldsymbol{\beta}_3$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，知方程组

$$\begin{pmatrix}1&3&9\\2&0&6\\-3&1&-7\end{pmatrix}\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\begin{pmatrix}\mu\\1\\0\end{pmatrix}$$

有解，对增广矩阵进行初等行变换，

$$\begin{pmatrix}1&3&9&\mu\\2&0&6&1\\-3&1&-7&0\end{pmatrix}\rightarrow\begin{pmatrix}1&3&9&\mu\\0&-6&-12&1-2\mu\\0&10&20&3\mu\end{pmatrix}\rightarrow\begin{pmatrix}1&3&9&\mu\\0&1&2&\dfrac{2\mu-1}{6}\\0&0&0&\dfrac{3\mu}{10}-\dfrac{2\mu-1}{6}\end{pmatrix},$$

故 $\dfrac{3\mu}{10}-\dfrac{2\mu-1}{6}=0$，解得 $\mu=5$．

又 $\boldsymbol{\alpha}_1$ 与 $\boldsymbol{\alpha}_2$ 线性无关，且 $\boldsymbol{\alpha}_3=3\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2$，故 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=2$，由已知

$$r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=2,$$

所以

$$|(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)|=\begin{vmatrix}0&k&5\\1&2&1\\-1&1&0\end{vmatrix}=0,$$

解得 $k=15$．

【注】由 $\begin{pmatrix}1&3&9\\0&1&2\\0&0&0\end{pmatrix}\rightarrow\begin{pmatrix}1&0&3\\0&1&2\\0&0&0\end{pmatrix}$，知 $\boldsymbol{\alpha}_3=3\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2$．

+++

#### 基础解答 (5) 设有向量组（Ⅰ）$\boldsymbol{\alpha}_1=(2,3,5)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,1,2)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,0,0)^{\mathrm{T}}$，（Ⅱ）$\boldsymbol{\beta}_1=(3,1,2)^{\mathrm{T}},\boldsymbol{\beta}_2=(1,1,1)^{\mathrm{T}},\boldsymbol{\beta}_3=(1,1,-1)^{\mathrm{T}},\boldsymbol{\beta}_4=(2,1,0)^{\mathrm{T}}$，证明：向量组（Ⅰ）与（Ⅱ）等价．
***
证明向量组（Ⅰ）与（Ⅱ）等价的基本方法是定义法，即证明（Ⅰ）与（Ⅱ）可以互相线性表示，而线性表示的问题可转化为解非齐次线性方程组，解方程组一般用初等变换．

记 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3),\boldsymbol{B}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4)$，则

$$(\boldsymbol{A}\ \vdots\ \boldsymbol{B})=\begin{pmatrix}2&0&1&3&1&1&2\\3&1&0&1&1&1&1\\5&2&0&2&1&-1&0\end{pmatrix}\rightarrow\begin{pmatrix}1&0&0&0&1&3&2\\0&1&0&1&-2&-8&-5\\0&0&1&3&-1&-5&-2\end{pmatrix},$$

故 $\boldsymbol{AX}=\boldsymbol{B}$ 有唯一解，且 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，即

$$\boldsymbol{\beta}_1=0\cdot\boldsymbol{\alpha}_1+1\cdot\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3,$$

$$\boldsymbol{\beta}_2=1\cdot\boldsymbol{\alpha}_1+(-2)\boldsymbol{\alpha}_2+(-1)\boldsymbol{\alpha}_3,$$

$$\boldsymbol{\beta}_3=3\cdot\boldsymbol{\alpha}_1+(-8)\boldsymbol{\alpha}_2+(-5)\boldsymbol{\alpha}_3,$$

$$\boldsymbol{\beta}_4=2\cdot\boldsymbol{\alpha}_1+(-5)\boldsymbol{\alpha}_2+(-2)\boldsymbol{\alpha}_3.$$

又

$$(\boldsymbol{B}\ \vdots\ \boldsymbol{A})=\begin{pmatrix}3&1&1&2&2&0&1\\1&1&1&1&3&1&0\\2&1&-1&0&5&2&0\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1&1&3&1&0\\0&-1&-3&-2&-1&0&0\\0&0&4&3&-5&-3&1\end{pmatrix},$$

显然 $r(\boldsymbol{B})=r(\boldsymbol{B}\ \vdots\ \boldsymbol{A})=3$，故 $\boldsymbol{BX}=\boldsymbol{A}$ 有无穷多解，即 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4$ 线性表示．

综上可知，向量组（Ⅰ）与（Ⅱ）等价．

【注】证明（Ⅰ）与（Ⅱ）等价，其实只要证明 $\boldsymbol{AX}=\boldsymbol{B}$ 有解，且 $\boldsymbol{BX}=\boldsymbol{A}$ 有解即可．

+++

#### 基础解答 (6) 设向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性无关，且可由向量组 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性表示，证明：这两个向量组等价．
***
由已知条件，知每一个 $\boldsymbol{\alpha}_i$ 可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性表示．

令 $\boldsymbol{\alpha}_i=a_{i1}\boldsymbol{\beta}_1+a_{i2}\boldsymbol{\beta}_2+\cdots+a_{ik}\boldsymbol{\beta}_k\ (i=1,2,3,\cdots,k)$，即

$$(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k)\begin{pmatrix}a_{11}&a_{21}&\cdots&a_{k1}\\a_{12}&a_{22}&\cdots&a_{k2}\\\vdots&\vdots&&\vdots\\a_{1k}&a_{2k}&\cdots&a_{kk}\end{pmatrix}.$$

记 $\boldsymbol{C}=(a_{ji})_{k\times k}$，则 $k\geqslant r(\boldsymbol{C})\geqslant r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)=k$，故 $r(\boldsymbol{C})=k$，所以 $\boldsymbol{C}$ 可逆，于是

$$(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)\boldsymbol{C}^{-1}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k),$$

即 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性表示，所以两个向量组等价．

【注】用矩阵表达已知条件是线性代数中常用的方法．

+++

#### 基础解答 (7) 设向量组（Ⅰ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_s$，（Ⅱ）$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_t$，$r(Ⅰ)=r(Ⅱ)$，且向量组（Ⅰ）可由（Ⅱ）线性表示．证明：向量组（Ⅰ）与（Ⅱ）等价．
***
依题设，只需证明（Ⅱ）可由（Ⅰ）线性表示．

令 $r(Ⅰ)=r(Ⅱ)=r\ (r\leqslant s,r\leqslant t)$，则不妨设（Ⅰ）与（Ⅱ）的极大线性无关组分别为 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r$ 与 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_r$．

由已知（Ⅰ）可由（Ⅱ）线性表示，而（Ⅱ）可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_r$ 线性表示，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r$ 可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_r$ 线性表示，从而向量组（Ⅲ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r,\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_r$ 的秩也为 $r$，而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r$ 线性无关，故它也是（Ⅲ）的一个极大线性无关组，所以 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_r$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r$ 线性表示，于是向量组（Ⅱ）可由（Ⅰ）线性表示．

综合所述，向量组（Ⅰ）与（Ⅱ）等价．

【注】设有向量组（Ⅰ）与（Ⅱ），则

① $r(Ⅰ)=r(Ⅱ)$ 推不出（Ⅰ）与（Ⅱ）等价；\
② 若 $r(Ⅰ)=r(Ⅱ)$，且（Ⅰ）可由（Ⅱ）或（Ⅱ）可由（Ⅰ）线性表示 $\Rightarrow$（Ⅰ）与（Ⅱ）等价．

+++

#### 基础解答 (8) 设向量组（Ⅰ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$，（Ⅱ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$，（Ⅲ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5$，且 $r(Ⅰ)=r(Ⅱ)=3,r(Ⅲ)=4$，证明：向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4$ 的秩为 $4$．
***
**证法 1** 依题意，只要证 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4$ 线性无关，用定义．

设

$$k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3+k_4(\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4)=\boldsymbol{0},\qquad ①$$

由 $r(Ⅰ)=r(Ⅱ)=3$，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性相关，故 $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．

设 $\boldsymbol{\alpha}_4=\lambda_1\boldsymbol{\alpha}_1+\lambda_2\boldsymbol{\alpha}_2+\lambda_3\boldsymbol{\alpha}_3$，将其代入 ① 式，得

$$(k_1-\lambda_1k_4)\boldsymbol{\alpha}_1+(k_2-\lambda_2k_4)\boldsymbol{\alpha}_2+(k_3-\lambda_3k_4)\boldsymbol{\alpha}_3+k_4\boldsymbol{\alpha}_5=\boldsymbol{0}.$$

由 $r(Ⅲ)=4$，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5$ 线性无关，故

$$\begin{cases}k_1-\lambda_1k_4=0,\\k_2-\lambda_2k_4=0,\\k_3-\lambda_3k_4=0,\\k_4=0,\end{cases}$$

解得 $k_4=k_3=k_2=k_1=0$ 且解唯一，所以 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4$ 线性无关，即秩为 $4$．

**证法 2** 利用向量组的秩证明．

由 $r(Ⅱ)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=r(Ⅰ)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=3$，知 $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．

又 $r(Ⅲ)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5)=4$，知 $\boldsymbol{\alpha}_5$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，故 $\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4$ 也不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示（否则由 $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，可得 $\boldsymbol{\alpha}_5$ 也能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示），故

$$r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_5-\boldsymbol{\alpha}_4)=r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)+1=3+1=4.$$

+++

#### 基础解答 (9) 设 $\boldsymbol{A}$ 是 $3$ 阶方阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 为 $\boldsymbol{A}$ 的分别属于特征值 $-2,1$ 的特征向量，且 $\boldsymbol{A\alpha}_3=\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$，证明：$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关．
***
**证法 1** 由特征值的定义，有 $\boldsymbol{A\alpha}_1=-2\boldsymbol{\alpha}_1,\boldsymbol{A\alpha}_2=\boldsymbol{\alpha}_2$．

设

$$k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3=\boldsymbol{0},\qquad ①$$

用 $\boldsymbol{A}$ 左乘 ① 式，得

$$-2k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3(\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3)=\boldsymbol{0}.\qquad ②$$

① $-$ ②，得 $3k_1\boldsymbol{\alpha}_1-k_3\boldsymbol{\alpha}_2=\boldsymbol{0}$，由于 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 是 $\boldsymbol{A}$ 的属于不同特征值的特征向量，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，所以 $k_1=k_3=0$，代入式 ① 得 $k_2\boldsymbol{\alpha}_2=\boldsymbol{0}$，又 $\boldsymbol{\alpha}_2\neq\boldsymbol{0}$（$\boldsymbol{\alpha}_2$ 是特征向量），故 $k_2=0$，从而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关．

**证法 2** 由

$$\boldsymbol{A\alpha}_1=-2\boldsymbol{\alpha}_1\Rightarrow(\boldsymbol{A}-\boldsymbol{E})\boldsymbol{\alpha}_1=-3\boldsymbol{\alpha}_1,$$

$$\boldsymbol{A\alpha}_2=\boldsymbol{\alpha}_2\Rightarrow(\boldsymbol{A}-\boldsymbol{E})\boldsymbol{\alpha}_2=\boldsymbol{0},$$

$$\boldsymbol{A\alpha}_3=\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3\Rightarrow(\boldsymbol{A}-\boldsymbol{E})\boldsymbol{\alpha}_3=\boldsymbol{\alpha}_2,$$

设

$$k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3=\boldsymbol{0},\qquad ①$$

用 $\boldsymbol{A}-\boldsymbol{E}$ 左乘 ① 式，得 $-3k_1\boldsymbol{\alpha}_1+k_3\boldsymbol{\alpha}_2=\boldsymbol{0}$，由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，知 $k_1=k_3=0$，代入 ① 式，得 $k_2=0$，从而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关．

【注】用定义法证明线性无关，选择适当的矩阵乘以定义式，需根据题目的条件而定，但目标是使定义式"变短"，从而证明定义式中的所有 $k=0$．

+++

#### 基础解答 (10) 设矩阵 $\boldsymbol{A}_{5\times 4}$ 的秩为 $2$，$\boldsymbol{\alpha}_1=(1,1,2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(-1,1,4,-1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(5,-1,-8,9)^{\mathrm{T}}$ 是方程组 $\boldsymbol{Ax}=\boldsymbol{0}$ 的解向量，求 $\boldsymbol{Ax}=\boldsymbol{0}$ 的解空间的一组标准正交基．
***
先求 $\boldsymbol{Ax}=\boldsymbol{0}$ 的解空间的一组基，再将其正交单位化，解空间的维数就是 $\boldsymbol{Ax}=\boldsymbol{0}$ 的基础解系所含解向量的个数，故 $n-r(\boldsymbol{A})=4-2=2$．

又 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 的分量不成比例，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，所以 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 是 $\boldsymbol{Ax}=\boldsymbol{0}$ 的解空间的一组基．

将 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 正交化，令

$$\boldsymbol{\beta}_1=\boldsymbol{\alpha}_1=(1,1,2,3)^{\mathrm{T}},$$

$$\boldsymbol{\beta}_2=\boldsymbol{\alpha}_2-\frac{(\boldsymbol{\alpha}_2,\boldsymbol{\beta}_1)}{(\boldsymbol{\beta}_1,\boldsymbol{\beta}_1)}\boldsymbol{\beta}_1=(-1,1,4,-1)^{\mathrm{T}}-\frac{1}{3}(1,1,2,3)^{\mathrm{T}}=\frac{2}{3}(-2,1,5,-3)^{\mathrm{T}}.$$

将 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2$ 单位化，

$$\boldsymbol{r}_1=\frac{\boldsymbol{\beta}_1}{\|\boldsymbol{\beta}_1\|}=\frac{1}{\sqrt{15}}(1,1,2,3)^{\mathrm{T}},$$

$$\boldsymbol{r}_2=\frac{\boldsymbol{\beta}_2}{\|\boldsymbol{\beta}_2\|}=\frac{1}{\sqrt{39}}(-2,1,5,-3)^{\mathrm{T}},$$

故 $\boldsymbol{r}_1,\boldsymbol{r}_2$ 为所求的一组标准正交基．

【注】① 解空间的维数为 $2$，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，应从 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 中找出基（不唯一），再正交化，不能直接对 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 正交化（标准正交基肯定是线性无关的）．

② 向量 $k\boldsymbol{\beta}\ (k\neq 0)$ 与 $\boldsymbol{\beta}$ 的单位化向量是相同的，即 $\dfrac{\boldsymbol{\beta}}{\|\boldsymbol{\beta}\|}=\dfrac{k\boldsymbol{\beta}}{\|k\boldsymbol{\beta}\|}$．

+++

#### 综合选择 (1) 设 $\boldsymbol{A}$ 是 $m\times n$ 矩阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_t$ 是 $n$ 维列向量，向量组（Ⅰ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_t$，（Ⅱ）$\boldsymbol{A\alpha}_1,\boldsymbol{A\alpha}_2,\cdots,\boldsymbol{A\alpha}_t$，则正确的是（　）．

;;;
A. 若（Ⅰ）线性无关，则（Ⅱ）线性无关
B. 若（Ⅱ）线性相关，则（Ⅰ）线性相关
C. 若（Ⅱ）线性无关，则（Ⅰ）线性无关
D. （Ⅰ）与（Ⅱ）具有相同的线性相关性
;;;C
***
对选项 C，用反证法，假设 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_t$ 线性相关，则存在不全为零的数 $k_1,k_2,\cdots,k_t$，使得

$$k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+\cdots+k_t\boldsymbol{\alpha}_t=\boldsymbol{0},\qquad ①$$

① 式两边同乘以 $\boldsymbol{A}$，得

$$\boldsymbol{A}(k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+\cdots+k_t\boldsymbol{\alpha}_t)=k_1\boldsymbol{A\alpha}_1+k_2\boldsymbol{A\alpha}_2+\cdots+k_t\boldsymbol{A\alpha}_t=\boldsymbol{0},$$

故 $\boldsymbol{A\alpha}_1,\boldsymbol{A\alpha}_2,\cdots,\boldsymbol{A\alpha}_t$ 线性相关，即（Ⅱ）线性相关，与条件矛盾，所以（Ⅰ）线性无关．

取矩阵 $\boldsymbol{A}=\boldsymbol{O}$，知 A，B 不正确，而 D 显然不正确．

+++

#### 综合选择 (2) 设三维列向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，$\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，记 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\boldsymbol{A}_{3\times 3}$，$(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)=(\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)\boldsymbol{B}_{3\times 3}$，则（　）．

;;;
A. 存在矩阵 $\boldsymbol{A}_{3\times 3}$，使得 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性无关
B. 不存在矩阵 $\boldsymbol{A}_{3\times 3}$，使得 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性相关
C. 存在矩阵 $\boldsymbol{B}_{3\times 3}$，使得 $\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3$ 线性无关
D. 不存在矩阵 $\boldsymbol{B}_{3\times 3}$，使得 $\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3$ 线性相关
;;;C
***
由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 线性无关，当 $\boldsymbol{B}_{3\times 3}$ 可逆时，有 $\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3$ 线性无关．

对于 A，因 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关，无论 $\boldsymbol{A}_{3\times 3}$ 是什么矩阵，$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 均线性相关．

对于 B，D，无论 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 和 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 是否相关，均存在 $\boldsymbol{A}_{3\times 3},\boldsymbol{B}_{3\times 3}$ 使得 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 和 $\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3$ 线性相关，故 B，D 不正确．

+++

#### 综合选择 (3) 设向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 满足 $k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3=\boldsymbol{0}$，$k_1,k_2,k_3$ 为常数，且 $k_1k_3\neq 0$，则（　）．

;;;
A. $\boldsymbol{\alpha}_1$ 与 $\boldsymbol{\alpha}_3$ 等价
B. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 与 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_3$ 等价
C. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 与 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 等价
D. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_3$ 与 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 等价
;;;C
***
两个向量组等价是指这两个向量组可以互相线性表示．

由已知条件 $k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3=\boldsymbol{0}$，$k_1k_3\neq 0$，$k_2$ 是否为零不能确定，故不能确定 $\boldsymbol{\alpha}_2$ 是否可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_3$ 线性表示，所以 B，D 排除；同样也不能确定 $\boldsymbol{\alpha}_1$ 与 $\boldsymbol{\alpha}_3$ 是否等价，所以 A 不正确．

对于 C，由 $k_1k_3\neq 0$，知 $\boldsymbol{\alpha}_1$ 可由 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，即 $\boldsymbol{\alpha}_1=-\dfrac{k_2}{k_1}\boldsymbol{\alpha}_2-\dfrac{k_3}{k_1}\boldsymbol{\alpha}_3$．同理，$\boldsymbol{\alpha}_3$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性表示，又 $\boldsymbol{\alpha}_2=\boldsymbol{\alpha}_2+0\cdot\boldsymbol{\alpha}_3=\boldsymbol{\alpha}_2+0\cdot\boldsymbol{\alpha}_1$，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 与 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 等价．

+++

#### 综合选择 (4) 设 $n$ 维向量组（Ⅰ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k\ (k<n)$ 线性无关，则 $n$ 维向量组（Ⅱ）$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 也线性无关的充要条件是（　）．

;;;
A. $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性表示
B. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性表示
C. 向量组（Ⅰ）与向量组（Ⅱ）等价
D. 矩阵 $(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)$ 与 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k)$ 等价
;;;D
***
对于 A：在选项 A 的条件下，可得 $r(Ⅱ)\leqslant r(Ⅰ)$，不能保证 $r(Ⅱ)=r(Ⅰ)$，故不能推得（Ⅱ）线性无关．

对于 B：由 $k\geqslant r(Ⅱ)\geqslant r(Ⅰ)=k$，得 $r(Ⅱ)=k$，故 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性无关，选项 B 的条件是充分条件，但不是必要条件，如（Ⅰ）$\begin{pmatrix}1\\0\end{pmatrix}$，（Ⅱ）$\begin{pmatrix}0\\1\end{pmatrix}$，均线性无关，但（Ⅰ）不能由（Ⅱ）线性表示．

对于 C：由（Ⅰ）与（Ⅱ）等价，即（Ⅰ）与（Ⅱ）可互为线性表示，故 C 不是必要条件．

对于 D：矩阵 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)$ 与 $\boldsymbol{B}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k)$ 等价是指：$\boldsymbol{A}$ 经过有限次初等变换化为 $\boldsymbol{B}$，故矩阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 等价的充分必要条件是 $r(\boldsymbol{A})=r(\boldsymbol{B})$．

在 D 的条件下，可知 $r(\boldsymbol{A})=r(\boldsymbol{B})$，又 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性无关，故 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性无关．反之，若 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k$ 线性无关，故 $r(Ⅱ)=r(Ⅰ)=k$，即 $r(\boldsymbol{A})=r(\boldsymbol{B})=k$，所以 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 等价．

【注】应注意向量组（Ⅰ）与（Ⅱ）等价与矩阵 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k)$ 与 $\boldsymbol{B}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_k)$ 等价的区别：

向量组（Ⅰ）与（Ⅱ）等价 $\Rightarrow r(Ⅰ)=r(Ⅱ)$，但反之不成立；\
同型矩阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 等价 $\Leftrightarrow r(\boldsymbol{A})=r(\boldsymbol{B})$．

+++

#### 综合选择 (5) 设 $4$ 维列向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，$\boldsymbol{\beta}_i\ (i=1,2,3,4)$ 为非零列向量，且 $\boldsymbol{\beta}_i$ 与 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 均正交，则 $r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4)=$（　）．

;;;
A. $1$
B. $2$
C. $3$
D. $4$
;;;A
***
令 $\boldsymbol{A}=\begin{pmatrix}\boldsymbol{\alpha}_1^{\mathrm{T}}\\\boldsymbol{\alpha}_2^{\mathrm{T}}\\\boldsymbol{\alpha}_3^{\mathrm{T}}\end{pmatrix}$，由 $\boldsymbol{\beta}_i$ 与 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 正交，知 $\boldsymbol{\beta}_i\ (i=1,2,3,4)$ 均是方程组 $\boldsymbol{Ax}=\boldsymbol{0}$ 的非零解向量．

由 $r(\boldsymbol{A})=3$，知 $\boldsymbol{Ax}=\boldsymbol{0}$ 的基础解系最多只含一个非零解向量，故

$$1\leqslant r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4)\leqslant n-r(\boldsymbol{A})=4-3=1,$$

从而 $r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\beta}_4)=1$，**A** 正确．

【注】① 列向量 $\boldsymbol{\alpha}$ 是 $\boldsymbol{Ax}=\boldsymbol{0}$ 的解 $\Leftrightarrow\boldsymbol{\alpha}$ 与 $\boldsymbol{A}$ 的行向量均正交；

② 列向量 $\boldsymbol{\alpha}$ 是 $\boldsymbol{Ax}=\boldsymbol{\beta}$ 的解 $\Rightarrow\boldsymbol{\beta}$ 可由 $\boldsymbol{A}$ 的列向量组线性表示（线性组合的系数为向量 $\boldsymbol{\alpha}$ 在对应向量组下的坐标）．

+++

#### 综合选择 (6) 设 $\boldsymbol{A},\boldsymbol{B}$ 均是 $m\times n$ 矩阵，则 $\boldsymbol{Ax}=\boldsymbol{0}$ 与 $\boldsymbol{Bx}=\boldsymbol{0}$ 同解的充要条件是（　）．

;;;
A. $\boldsymbol{A},\boldsymbol{B}$ 的列向量组等价
B. $\boldsymbol{A},\boldsymbol{B}$ 的行向量组等价
C. $\boldsymbol{A},\boldsymbol{B}$ 是等价矩阵
D. $\boldsymbol{A}^{\mathrm{T}}\boldsymbol{x}=\boldsymbol{0}$ 与 $\boldsymbol{B}^{\mathrm{T}}\boldsymbol{x}=\boldsymbol{0}$ 同解
;;;B
***
对于 B：若 $\boldsymbol{Ax}=\boldsymbol{0}$ 与 $\boldsymbol{Bx}=\boldsymbol{0}$ 同解，考虑方程组

$$（Ⅰ）\boldsymbol{Ax}=\boldsymbol{0},\quad（Ⅱ）\begin{cases}\boldsymbol{Ax}=\boldsymbol{0},\\\boldsymbol{Bx}=\boldsymbol{0},\end{cases}\quad（Ⅲ）\boldsymbol{Bx}=\boldsymbol{0},$$

则（Ⅰ）（Ⅱ）（Ⅲ）同解，故 $r(\boldsymbol{A})=r\begin{pmatrix}\boldsymbol{A}\\\boldsymbol{B}\end{pmatrix}=r(\boldsymbol{B})$，即 $\boldsymbol{A},\boldsymbol{B}$ 的行向量组等价．反之，若 $\boldsymbol{A},\boldsymbol{B}$ 的行向量组等价，记

$$\boldsymbol{A}=\begin{pmatrix}\boldsymbol{\alpha}_1\\\boldsymbol{\alpha}_2\\\vdots\\\boldsymbol{\alpha}_m\end{pmatrix},\quad \boldsymbol{B}=\begin{pmatrix}\boldsymbol{\beta}_1\\\boldsymbol{\beta}_2\\\vdots\\\boldsymbol{\beta}_m\end{pmatrix},$$

即列向量组 $\boldsymbol{\alpha}_1^{\mathrm{T}},\boldsymbol{\alpha}_2^{\mathrm{T}},\cdots,\boldsymbol{\alpha}_m^{\mathrm{T}}$ 与 $\boldsymbol{\beta}_1^{\mathrm{T}},\boldsymbol{\beta}_2^{\mathrm{T}},\cdots,\boldsymbol{\beta}_m^{\mathrm{T}}$ 等价，故存在矩阵 $\boldsymbol{P},\boldsymbol{Q}$，使得

$$(\boldsymbol{\alpha}_1^{\mathrm{T}},\boldsymbol{\alpha}_2^{\mathrm{T}},\cdots,\boldsymbol{\alpha}_m^{\mathrm{T}})=(\boldsymbol{\beta}_1^{\mathrm{T}},\boldsymbol{\beta}_2^{\mathrm{T}},\cdots,\boldsymbol{\beta}_m^{\mathrm{T}})\boldsymbol{P},$$

$$(\boldsymbol{\beta}_1^{\mathrm{T}},\boldsymbol{\beta}_2^{\mathrm{T}},\cdots,\boldsymbol{\beta}_m^{\mathrm{T}})=(\boldsymbol{\alpha}_1^{\mathrm{T}},\boldsymbol{\alpha}_2^{\mathrm{T}},\cdots,\boldsymbol{\alpha}_m^{\mathrm{T}})\boldsymbol{Q},$$

所以 $\boldsymbol{A}=\boldsymbol{P}^{\mathrm{T}}\boldsymbol{B},\boldsymbol{B}=\boldsymbol{Q}^{\mathrm{T}}\boldsymbol{A}$，故由 $\boldsymbol{Ax}=\boldsymbol{0}$ 得 $\boldsymbol{Bx}=\boldsymbol{Q}^{\mathrm{T}}\boldsymbol{Ax}=\boldsymbol{0}$，反之，由 $\boldsymbol{Bx}=\boldsymbol{0}$，得

$$\boldsymbol{Ax}=\boldsymbol{P}^{\mathrm{T}}\boldsymbol{Bx}=\boldsymbol{0},$$

即 $\boldsymbol{Ax}=\boldsymbol{0}$ 与 $\boldsymbol{Bx}=\boldsymbol{0}$ 同解．

对于 A，由 B 的证明知显然不正确．

对于 C，相当于 $r(\boldsymbol{A})=r(\boldsymbol{B})$，它是必要条件而非充分条件．

对于 D，举反例．如 $\boldsymbol{A}=\begin{pmatrix}1&0&0\\2&0&0\end{pmatrix},\boldsymbol{B}=\begin{pmatrix}2&0&0\\1&0&0\end{pmatrix}$，显然，$\boldsymbol{Ax}=\boldsymbol{0},\boldsymbol{Bx}=\boldsymbol{0}$ 同解，但 $\boldsymbol{A}^{\mathrm{T}}\boldsymbol{x}=\boldsymbol{0}$ 与 $\boldsymbol{B}^{\mathrm{T}}\boldsymbol{x}=\boldsymbol{0}$ 不同解．

+++

#### 综合填空 (1) 设向量组 $\boldsymbol{\alpha}_1=(1,k+2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(2,-1,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(k-1,1,-1)^{\mathrm{T}}$ 线性相关，但任意两个向量线性无关，则 $k=$ ________．
***
$-5$．

由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性相关 $\Leftrightarrow|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=0$．

而

$$|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=\begin{vmatrix}1&2&k-1\\k+2&-1&1\\3&1&-1\end{vmatrix}=(k+1)(k+5)=0,$$

解得 $k=-1$ 或 $k=-5$．

当 $k=-1$ 时，$\boldsymbol{\alpha}_1=(1,1,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(2,-1,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-2,1,-1)^{\mathrm{T}}$，显然，$\boldsymbol{\alpha}_2$ 与 $\boldsymbol{\alpha}_3$ 线性相关，故 $k=-5$．

+++

#### 综合解答 (1) 设 $\boldsymbol{A}=\begin{pmatrix}1&0&0&0\\1&2&0&0\\2&4&3&-3\end{pmatrix}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)$，$\boldsymbol{B}=\begin{pmatrix}1&0&0&0\\0&2&0&0\\0&0&3&0\end{pmatrix}$．

（Ⅰ）求向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 的一个极大线性无关组；\
（Ⅱ）求可逆矩阵 $\boldsymbol{P}_{3\times 3},\boldsymbol{Q}_{4\times 4}$，使得 $\boldsymbol{PAQ}=\boldsymbol{B}$．
***
（Ⅰ）对 $\boldsymbol{A}$ 进行初等行变换，得

$$\boldsymbol{A}=\begin{pmatrix}1&0&0&0\\1&2&0&0\\2&4&3&-3\end{pmatrix}\rightarrow\begin{pmatrix}1&0&0&0\\1&2&0&0\\0&0&3&-3\end{pmatrix}\rightarrow\begin{pmatrix}1&0&0&0\\0&2&0&0\\0&0&3&-3\end{pmatrix}\xlongequal{\text{记}}\boldsymbol{C},$$

显然，向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4$ 的一个极大线性无关组．

（Ⅱ）对 $\boldsymbol{C}$ 作初等列变换，得

$$\boldsymbol{C}=\begin{pmatrix}1&0&0&0\\0&2&0&0\\0&0&3&-3\end{pmatrix}\rightarrow\begin{pmatrix}1&0&0&0\\0&2&0&0\\0&0&3&0\end{pmatrix}=\boldsymbol{B},$$

故 $\boldsymbol{E}_{21}(-1)\boldsymbol{E}_{32}(-2)\boldsymbol{A}\boldsymbol{E}_{34}(1)=\boldsymbol{B}$，其中 $\boldsymbol{E}_{ij}(a)$ 表示单位矩阵第 $j$ 行（或第 $i$ 列）乘以 $a$ 加到第 $i$ 行（或第 $j$ 列）上，则有

$$\boldsymbol{P}=\boldsymbol{E}_{21}(-1)\boldsymbol{E}_{32}(-2)=\begin{pmatrix}1&0&0\\-1&1&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&0\\0&-2&1\end{pmatrix}=\begin{pmatrix}1&0&0\\-1&1&0\\0&-2&1\end{pmatrix},$$

$$\boldsymbol{Q}=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&1&1\\0&0&0&1\end{pmatrix},$$

使得 $\boldsymbol{PAQ}=\boldsymbol{B}$．

+++

#### 综合解答 (2) 设向量组 $\boldsymbol{\alpha}_1=(1,0,1)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,1,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,3,5)^{\mathrm{T}}$ 不能由向量组 $\boldsymbol{\beta}_1=(1,1,1)^{\mathrm{T}},\boldsymbol{\beta}_2=(1,2,3)^{\mathrm{T}},\boldsymbol{\beta}_3=(3,4,a)^{\mathrm{T}}$ 线性表示，求 $a$ 的值，并将 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 用 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．
***
$4$ 个 $3$ 维向量 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\alpha}_i\ (i=1,2,3)$ 一定线性相关．若 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性无关，则 $\boldsymbol{\alpha}_i\ (i=1,2,3)$ 可由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性表示，这与题设矛盾，于是 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性相关，从而

$$|(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)|=\begin{vmatrix}1&1&3\\1&2&4\\1&3&a\end{vmatrix}=a-5=0,$$

解得 $a=5$，此时，向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 不能由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性表示．

令 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)$，对 $\boldsymbol{A}$ 进行初等行变换．

$$\boldsymbol{A}=\begin{pmatrix}1&0&1&1&1&3\\0&1&3&1&2&4\\1&1&5&1&3&5\end{pmatrix}\rightarrow\begin{pmatrix}1&0&0&2&1&5\\0&1&0&4&2&10\\0&0&1&-1&0&-2\end{pmatrix},$$

故 $\boldsymbol{\beta}_1=2\boldsymbol{\alpha}_1+4\boldsymbol{\alpha}_2-\boldsymbol{\alpha}_3$，$\boldsymbol{\beta}_2=\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2$，$\boldsymbol{\beta}_3=5\boldsymbol{\alpha}_1+10\boldsymbol{\alpha}_2-2\boldsymbol{\alpha}_3$．

【注】向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 不能由 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性表示，相当于方程组 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)\boldsymbol{x}=\boldsymbol{\alpha}_i\ (i=1,2,3)$ 无解．若 $3$ 个 $3$ 维列向量 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性无关，则方程组必有解（因 $r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=r(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3,\boldsymbol{\alpha}_i)=3$），故矛盾，则 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 线性相关．事实上，对 $\boldsymbol{A}_{m\times n}$，若 $r(\boldsymbol{A})=m$（即 $\boldsymbol{A}$ 行满秩），则 $\boldsymbol{A}_{m\times n}\boldsymbol{x}=\boldsymbol{b}$ 必有解．

+++

#### 综合解答 (3) 设 $\boldsymbol{A}$ 是 $3$ 阶矩阵，$\boldsymbol{\alpha}_i\ (i=1,2,3)$ 是 $3$ 维非零列向量，且 $\boldsymbol{A\alpha}_i=i\boldsymbol{\alpha}_i\ (i=1,2,3)$，$\boldsymbol{\alpha}=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$，证明：$\boldsymbol{\alpha},\boldsymbol{A\alpha},\boldsymbol{A}^2\boldsymbol{\alpha}$ 线性无关．
***
由 $\boldsymbol{A\alpha}_1=\boldsymbol{\alpha}_1,\boldsymbol{A\alpha}_2=2\boldsymbol{\alpha}_2,\boldsymbol{A\alpha}_3=3\boldsymbol{\alpha}_3$，且 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是非零列向量，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是不同特征值对应的特征向量，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关．设

$$k_1\boldsymbol{\alpha}+k_2\boldsymbol{A\alpha}+k_3\boldsymbol{A}^2\boldsymbol{\alpha}=\boldsymbol{0}.\qquad ①$$

又

$$\boldsymbol{A\alpha}=\boldsymbol{A}(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3)=\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3,$$

$$\boldsymbol{A}^2\boldsymbol{\alpha}=\boldsymbol{A}(\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3)=\boldsymbol{\alpha}_1+4\boldsymbol{\alpha}_2+9\boldsymbol{\alpha}_3,$$

将上两式代入 ① 式，得

$$k_1(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3)+k_2(\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3)+k_3(\boldsymbol{\alpha}_1+4\boldsymbol{\alpha}_2+9\boldsymbol{\alpha}_3)=\boldsymbol{0},$$

即

$$(k_1+k_2+k_3)\boldsymbol{\alpha}_1+(k_1+2k_2+4k_3)\boldsymbol{\alpha}_2+(k_1+3k_2+9k_3)\boldsymbol{\alpha}_3=\boldsymbol{0}.$$

由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，知

$$\begin{cases}k_1+k_2+k_3=0,\\k_1+2k_2+4k_3=0,\\k_1+3k_2+9k_3=0.\end{cases}$$

由于齐次线性方程组系数行列式为范德蒙德行列式且不为零，故只有零解 $k_1=k_2=k_3=0$，从而 $\boldsymbol{\alpha},\boldsymbol{A\alpha},\boldsymbol{A}^2\boldsymbol{\alpha}$ 线性无关．

+++

#### 综合解答 (4) 设 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，其中 $\boldsymbol{\alpha}_1=(1,0,1)^{\mathrm{T}},\boldsymbol{\alpha}_2=(1,1,2)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,2,a)^{\mathrm{T}}$，$\boldsymbol{B}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2)$，其中 $\boldsymbol{\beta}_1=(-1,2,1)^{\mathrm{T}},\boldsymbol{\beta}_2=(1,0,b)^{\mathrm{T}}$．

（Ⅰ）问 $a,b$ 为何值时，$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2$ 不能同时由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示？\
（Ⅱ）问 $a,b$ 为何值时，$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2$ 可同时由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示，并求表达式？
***
（Ⅰ）对增广矩阵 $(\boldsymbol{A}\ \vdots\ \boldsymbol{B})$ 施行初等行变换，有

$$\begin{pmatrix}1&1&1&-1&1\\0&1&2&2&0\\1&2&a&1&b\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1&-1&1\\0&1&2&2&0\\0&1&a-1&2&b-1\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1&-1&1\\0&1&2&2&0\\0&0&a-3&0&b-1\end{pmatrix}.$$

当 $a=3,b\neq 1$ 时，$\boldsymbol{AX}=\boldsymbol{B}$ 无解，即 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2$ 不能同时由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示．

（Ⅱ）当 $a\neq 3$ 时，对任意 $b$，$\boldsymbol{AX}=\boldsymbol{B}$ 有唯一解 $\boldsymbol{\eta}_1,\boldsymbol{\eta}_2$，记 $\boldsymbol{X}=(\boldsymbol{\eta}_1,\boldsymbol{\eta}_2)$，则 $\boldsymbol{A\eta}_1=\boldsymbol{\beta}_1$ 的解为 $(-3,2,0)^{\mathrm{T}}$，$\boldsymbol{A\eta}_2=\boldsymbol{\beta}_2$ 的解为 $\left(1+\dfrac{b-1}{a-3},\dfrac{-2(b-1)}{a-3},\dfrac{b-1}{a-3}\right)^{\mathrm{T}}$，即表达式为

$$\boldsymbol{\beta}_1=-3\boldsymbol{\alpha}_1+2\boldsymbol{\alpha}_2+0\cdot\boldsymbol{\alpha}_3,$$

$$\boldsymbol{\beta}_2=\left(1+\frac{b-1}{a-3}\right)\boldsymbol{\alpha}_1-\frac{2(b-1)}{a-3}\boldsymbol{\alpha}_2+\frac{b-1}{a-3}\boldsymbol{\alpha}_3.$$

当 $a=3,b=1$ 时，$\boldsymbol{AX}=\boldsymbol{B}$ 有无穷多解，$\boldsymbol{A\eta}_1=\boldsymbol{\beta}_1$ 的解为

$$k(1,-2,1)^{\mathrm{T}}+(-2,0,1)^{\mathrm{T}},$$

$\boldsymbol{A\eta}_2=\boldsymbol{\beta}_2$ 的解为 $l(1,-2,1)^{\mathrm{T}}+(1,0,0)^{\mathrm{T}}$，故全部解为

$$\boldsymbol{X}=\begin{pmatrix}k-2&l+1\\-2k&-2l\\k+1&l\end{pmatrix}\ (k,l\ \text{为任意常数}),$$

表达式为 $\boldsymbol{\beta}_1=(k-2)\boldsymbol{\alpha}_1-2k\boldsymbol{\alpha}_2+(k+1)\boldsymbol{\alpha}_3$，$\boldsymbol{\beta}_2=(l+1)\boldsymbol{\alpha}_1-2l\boldsymbol{\alpha}_2+l\boldsymbol{\alpha}_3$，其中 $k,l$ 为任意常数．

+++

#### 综合解答 (5) 设 $n$ 维向量组 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k\ (k<n)$ 线性无关，且 $\boldsymbol{\alpha}_{k+1}=\lambda_1\boldsymbol{\alpha}_1+\lambda_2\boldsymbol{\alpha}_2+\cdots+\lambda_k\boldsymbol{\alpha}_k$，$\lambda_i\neq 0,i=1,2,\cdots,k$，证明：$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 中任何 $k$ 个向量都线性无关．
***
**证法 1**（用定义）由已知条件，需证明从 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 中去掉一个后，剩下的 $k$ 个是线性无关的，不失一般性，不妨设去掉 $\boldsymbol{\alpha}_1$，即需证明 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 线性无关．

设

$$\mu_2\boldsymbol{\alpha}_2+\mu_3\boldsymbol{\alpha}_3+\cdots+\mu_k\boldsymbol{\alpha}_k+\mu_{k+1}\boldsymbol{\alpha}_{k+1}=\boldsymbol{0},\qquad ①$$

将 $\boldsymbol{\alpha}_{k+1}=\lambda_1\boldsymbol{\alpha}_1+\lambda_2\boldsymbol{\alpha}_2+\cdots+\lambda_k\boldsymbol{\alpha}_k$ 代入 ① 式整理得

$$\mu_{k+1}\lambda_1\boldsymbol{\alpha}_1+(\mu_2+\mu_{k+1}\lambda_2)\boldsymbol{\alpha}_2+\cdots+(\mu_k+\mu_{k+1}\lambda_k)\boldsymbol{\alpha}_k=\boldsymbol{0},$$

由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性无关，故有

$$\mu_{k+1}\lambda_1=\mu_2+\mu_{k+1}\lambda_2=\cdots=\mu_k+\mu_{k+1}\lambda_k=0.$$

又 $\lambda_i\neq 0\ (i=1,2,\cdots,k)$，可得 $\mu_{k+1}=0,\mu_2=0,\cdots,\mu_k=0$，故 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 线性无关．

**证法 2** 不失一般性，考查向量组（Ⅰ）$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$，（Ⅱ）$\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$．

由已知条件，（Ⅰ）与（Ⅱ）可互为线性表示，所以 $r(Ⅰ)=r(Ⅱ)=k$，即（Ⅱ）中 $k$ 个向量是线性无关的．

**证法 3**（反证法）假设 $\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 线性相关，而已知 $\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性无关，故 $\boldsymbol{\alpha}_{k+1}$ 可由 $\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性表示，设

$$\boldsymbol{\alpha}_{k+1}=a_2\boldsymbol{\alpha}_2+\cdots+a_k\boldsymbol{\alpha}_k,\qquad ①$$

又

$$\boldsymbol{\alpha}_{k+1}=\lambda_1\boldsymbol{\alpha}_1+\lambda_2\boldsymbol{\alpha}_2+\cdots+\lambda_k\boldsymbol{\alpha}_k.\qquad ②$$

② $-$ ① 得

$$\boldsymbol{0}=\lambda_1\boldsymbol{\alpha}_1+(\lambda_2-a_2)\boldsymbol{\alpha}_2+\cdots+(\lambda_k-a_k)\boldsymbol{\alpha}_k,$$

其中至少有 $\lambda_1\neq 0$，这表明 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k$ 线性相关，与已知条件矛盾，故 $\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_k,\boldsymbol{\alpha}_{k+1}$ 线性无关．

+++

#### 综合解答 (6) 设矩阵 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m)$，$\boldsymbol{\alpha}_i$ 为 $n$ 维列向量，$i=1,2,\cdots,m$，且 $m\leqslant n$，证明：$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m$ 线性无关的充分必要条件是 $|\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}|\neq 0$．
***
（Ⅰ）当 $m=n$ 时，利用结论．

$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m$ 线性无关 $\Leftrightarrow|\boldsymbol{A}|=|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m)|\neq 0$，由

$$|\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}|=|\boldsymbol{A}^{\mathrm{T}}||\boldsymbol{A}|=|\boldsymbol{A}|^2,$$

知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m$ 线性无关 $\Leftrightarrow|\boldsymbol{A}|\neq 0\Leftrightarrow|\boldsymbol{A}|^2\neq 0\Leftrightarrow|\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}|\neq 0$．

（Ⅱ）当 $m<n$ 时，$\boldsymbol{A}$ 不是方阵，不能取行列式，利用方程组证．

$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m$ 线性无关 $\Leftrightarrow(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m)\boldsymbol{x}=\boldsymbol{Ax}=\boldsymbol{0}$ 只有零解 $\Rightarrow\boldsymbol{A}^{\mathrm{T}}\boldsymbol{Ax}=\boldsymbol{0}$ 只有零解 $\Leftrightarrow|\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}|\neq 0$．

$|\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}|\neq 0\Leftrightarrow\boldsymbol{A}^{\mathrm{T}}\boldsymbol{Ax}=\boldsymbol{0}$ 只有零解 $\Rightarrow\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}^{\mathrm{T}}\boldsymbol{Ax}=(\boldsymbol{Ax})^{\mathrm{T}}(\boldsymbol{Ax})=\boldsymbol{0}$ 只有零解 $\Rightarrow\boldsymbol{Ax}=\boldsymbol{0}$ 只有零解 $\Leftrightarrow\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_m$ 线性无关．

综上所述命题得证．

+++

#### 综合解答 (7) 设 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 与 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 是 $3$ 维向量空间的两组基，若向量 $\boldsymbol{\gamma}$ 在这两组基下的坐标分别为 $(x_1,x_2,x_3)$ 与 $(y_1,y_2,y_3)$，且 $x_1=y_1,x_2=-y_1+y_2,x_3=-y_2+y_3$．

（Ⅰ）求由基 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 到基 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 的过渡矩阵；\
（Ⅱ）若 $\boldsymbol{\alpha}_1=(1,2,3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(2,3,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(3,1,2)^{\mathrm{T}}$，求 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$．
***
（Ⅰ）依题设，有

$$(x_1,x_2,x_3)=(y_1,y_2,y_3)\begin{pmatrix}1&-1&0\\0&1&-1\\0&0&1\end{pmatrix}.\qquad ①$$

设过渡矩阵 $\boldsymbol{P}$，则 $(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\boldsymbol{P}$（$\boldsymbol{P}$ 可逆）．又

$$(y_1,y_2,y_3)=(x_1,x_2,x_3)(\boldsymbol{P}^{\mathrm{T}})^{-1},$$

即 $(x_1,x_2,x_3)=(y_1,y_2,y_3)\cdot\boldsymbol{P}^{\mathrm{T}}$，故由 ① 式，知

$$\boldsymbol{P}=\begin{pmatrix}1&-1&0\\0&1&-1\\0&0&1\end{pmatrix}^{\mathrm{T}}=\begin{pmatrix}1&0&0\\-1&1&0\\0&-1&1\end{pmatrix}.$$

（Ⅱ）

$$(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\boldsymbol{P}=\begin{pmatrix}1&2&3\\2&3&1\\3&1&2\end{pmatrix}\begin{pmatrix}1&0&0\\-1&1&0\\0&-1&1\end{pmatrix}=\begin{pmatrix}-1&-1&3\\-1&2&1\\2&-1&2\end{pmatrix},$$

故 $\boldsymbol{\beta}_1=(-1,-1,2)^{\mathrm{T}},\boldsymbol{\beta}_2=(-1,2,-1)^{\mathrm{T}},\boldsymbol{\beta}_3=(3,1,2)^{\mathrm{T}}$．

【注】设 $n$ 维向量 $\boldsymbol{\alpha}$ 在基 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 下的坐标为 $(x_1,x_2,\cdots,x_n)$，在基 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 下的坐标为 $(y_1,y_2,\cdots,y_n)$，$\boldsymbol{P}$ 为从基 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 到基 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 的过渡矩阵，则有 $(y_1,y_2,\cdots,y_n)=(x_1,x_2,\cdots,x_n)(\boldsymbol{P}^{\mathrm{T}})^{-1}$．

+++

#### 拓展选择 (1) 设向量 $\boldsymbol{\alpha}_1=(a_1,a_2,a_3)^{\mathrm{T}},\boldsymbol{\alpha}_2=(b_1,b_2,b_3)^{\mathrm{T}},\boldsymbol{\alpha}_3=(c_1,c_2,c_3)^{\mathrm{T}},\boldsymbol{\alpha}_4=(d_1,d_2,d_3)^{\mathrm{T}}$，则三个平面 $a_1x+b_1y+c_1z+d_1=0,a_2x+b_2y+c_2z+d_2=0,a_3x+b_3y+c_3z+d_3=0$ 两两相交成三条平行直线的充分必要条件是（　）．

;;;
A. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=1,r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=2$
B. $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=2,r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)=3$
C. 在 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 中任意两个向量均线性无关，且 $\boldsymbol{\alpha}_4$ 可由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示
D. 在 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 中任意两个向量均线性无关，且 $\boldsymbol{\alpha}_4$ 不能由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性表示
;;;D
***
由三个平面两两相交，知方程组

$$\begin{cases}a_1x+b_1y+c_1z+d_1=0,\\a_2x+b_2y+c_2z+d_2=0,\\a_3x+b_3y+c_3z+d_3=0\end{cases}$$

无解，故 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\neq r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)$，可排除 C．

若 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=1$，则三个平面的法向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 共线，那么这三个平面必平行或重合，由此可排除 A．

当三个平面两两相交，三条交线相互平行时，这三个平面的法向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 共面且互不平行，故

$$|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=\begin{vmatrix}a_1&b_1&c_1\\a_2&b_2&c_2\\a_3&b_3&c_3\end{vmatrix}=0,$$

且任意两行不成比例，从而有 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=2$，但当 $r(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=2$ 时，不能保证任两个平面不平行，故 B 选项中的条件是必要条件．

+++

#### 拓展解答 (1) 设 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 为 $n$ 维向量空间 $\mathbf{R}^n$ 的一组基，且 $\boldsymbol{\beta}_1=\boldsymbol{\alpha}_1,\boldsymbol{\beta}_2=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\beta}_n=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\cdots+\boldsymbol{\alpha}_n$．

（Ⅰ）证明：$\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 也是 $\mathbf{R}^n$ 的一组基，并写出由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 到 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 的过渡矩阵 $\boldsymbol{P}$；\
（Ⅱ）设向量 $\boldsymbol{\alpha}\in\mathbf{R}^n$，$\boldsymbol{\alpha}$ 在基 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 下的坐标为 $(n,n-1,\cdots,2,1)^{\mathrm{T}}$，求 $\boldsymbol{\alpha}$ 在基 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 下的坐标．
***
（Ⅰ）依题设，有

$$(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\begin{pmatrix}1&1&\cdots&1\\0&1&\cdots&1\\\vdots&\vdots&&\vdots\\0&0&\cdots&1\end{pmatrix}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\boldsymbol{P}.$$

而 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 线性无关，且 $|\boldsymbol{P}|=1\neq 0$，故 $\boldsymbol{P}$ 可逆，所以 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 线性无关，即 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 为 $\mathbf{R}^n$ 的一组基，$\boldsymbol{P}$ 为所求过渡矩阵．

（Ⅱ）由已知

$$\boldsymbol{\alpha}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\begin{pmatrix}n\\n-1\\\vdots\\1\end{pmatrix}.$$

由（Ⅰ），知 $(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n)\boldsymbol{P}^{-1}$，所以

$$\boldsymbol{\alpha}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\begin{pmatrix}n\\n-1\\\vdots\\1\end{pmatrix}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n)\boldsymbol{P}^{-1}\begin{pmatrix}n\\n-1\\\vdots\\1\end{pmatrix}$$

$$=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n)\begin{pmatrix}1&-1&0&\cdots&0\\0&1&-1&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\0&0&0&\cdots&1\end{pmatrix}\begin{pmatrix}n\\n-1\\\vdots\\1\end{pmatrix}=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n)\begin{pmatrix}1\\1\\\vdots\\1\end{pmatrix},$$

故 $\boldsymbol{\alpha}$ 在基 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\cdots,\boldsymbol{\beta}_n$ 下的坐标为 $(1,1,\cdots,1)^{\mathrm{T}}$．
