---
quizify:
  format: 1
  deck: Math_880::Chapter_13
  tags: [Math, 880题, 数一, 第十三章, 线性方程组]
---

+++

#### 基础选择 (1) 已知 $\eta_1,\eta_2$ 是非齐次线性方程组 $Ax=b$ 的两个不同解，$\xi_1,\xi_2$ 是对应齐次线性方程组 $Ax=0$ 的基础解系，$k_1,k_2$ 为任意常数，则 $Ax=b$ 的通解为（　）．

;;;
A. $k_1\xi_1+k_2(\xi_1+\xi_2)+\dfrac{\eta_1-\eta_2}{2}$
B. $k_1\xi_1+k_2(\xi_1-\xi_2)+\dfrac{\eta_1+\eta_2}{2}$
C. $k_1\xi_1+k_2(\eta_1+\eta_2)+\dfrac{\eta_1-\eta_2}{2}$
D. $k_1\xi_1+k_2(\eta_1-\eta_2)+\dfrac{\eta_1+\eta_2}{2}$
;;;B
***
$Ax=b$ 的通解为 $Ax=0$ 的通解加上 $Ax=b$ 的一个特解，根据非齐次和齐次线性方程组解的性质与结构，知

$$A\left(\frac{\eta_1-\eta_2}{2}\right)=\frac{1}{2}(A\eta_1-A\eta_2)=0,$$

$$A\left(\frac{\eta_1+\eta_2}{2}\right)=\frac{1}{2}(A\eta_1+A\eta_2)=b,$$

即 $\dfrac{1}{2}(\eta_1-\eta_2)$ 是 $Ax=0$ 的解，故排除 **A、C**．

因为不能判定 $\eta_1-\eta_2$ 是否与 $\xi_1$ 线性无关，所以不能选 **D**．

事实上，由 $\dfrac{1}{2}(\eta_1+\eta_2)$ 是 $Ax=b$ 的解，且 $\xi_1$ 与 $\xi_1-\xi_2$ 线性无关，可知 $\xi_1,\xi_1-\xi_2$ 是 $Ax=0$ 的基础解系，故 **B** 正确．

【注】① $\xi_1$ 与 $\xi_1-\xi_2$ 线性无关可以从几何上看出：由于 $\xi_1$ 与 $\xi_1-\xi_2$ 不共线，故线性无关．

② 也可利用定义证明 $\xi_1$ 与 $\xi_1-\xi_2$ 线性无关．设 $k_1\xi_1+k_2(\xi_1-\xi_2)=0$，即 $(k_1+k_2)\xi_1-k_2\xi_2=0$．由已知，$\xi_1,\xi_2$ 是 $Ax=0$ 的基础解系，故线性无关，所以 $k_1+k_2=0$，$-k_2=0$，故 $k_1=k_2=0$，从而 $\xi_1$ 与 $\xi_1-\xi_2$ 线性无关．

③ 一般地，对任意两个线性无关的向量 $\xi_1$ 与 $\xi_2$，当 $\begin{vmatrix}a&c\\b&d\end{vmatrix}\neq 0$ 时，线性组合 $a\xi_1+b\xi_2$，$c\xi_1+d\xi_2$ 仍线性无关．

+++

#### 基础选择 (2) 设 $A$ 是 $n$ 阶矩阵，对方程组（Ⅰ）$Ax=0$ 和（Ⅱ）$A^{\mathrm{T}}Ax=0$，必有（　）．

;;;
A. （Ⅱ）的解是（Ⅰ）的解，（Ⅰ）的解也是（Ⅱ）的解
B. （Ⅱ）的解是（Ⅰ）的解，但（Ⅰ）的解不是（Ⅱ）的解
C. （Ⅰ）的解不是（Ⅱ）的解，（Ⅱ）的解也不是（Ⅰ）的解
D. （Ⅰ）的解是（Ⅱ）的解，但（Ⅱ）的解不是（Ⅰ）的解
;;;A
***
由 $Ax=0$，得 $A^{\mathrm{T}}Ax=A^{\mathrm{T}}(Ax)=0$，故 $Ax=0$ 的解是 $A^{\mathrm{T}}Ax=0$ 的解．

反之，若 $x$ 是 $A^{\mathrm{T}}Ax=0$ 的解，令 $Ax=b$，则 $b^{\mathrm{T}}=(Ax)^{\mathrm{T}}=x^{\mathrm{T}}A^{\mathrm{T}}$，从而

$$b^{\mathrm{T}}b=x^{\mathrm{T}}A^{\mathrm{T}}Ax=0,$$

于是 $b$ 的各分量的平方和为 $0$，故 $b=0$，从而 $Ax=0$，因此 $A^{\mathrm{T}}Ax=0$ 的解是 $Ax=0$ 的解．

【注】证明列向量 $b=0$，即证 $b$ 的每个分量为 $0$，可证 $b^{\mathrm{T}}b=0$，这是证明向量为零向量的一种方法．

+++

#### 基础选择 (3) 设 $A$ 是 $n$ 阶矩阵，若对任意的 $n$ 维列向量 $\alpha$，有 $A^{*}\alpha=0$，则 $Ax=0$ 的基础解系所含解向量的个数 $k$ 满足（　）．

;;;
A. $k=0$
B. $k=1$
C. $k>1$
D. $k=n$
;;;C
***
方程组解的判别，关键是讨论其秩．由已知，对任意 $n$ 维列向量 $\alpha$，有 $A^{*}\alpha=0$，故 $A^{*}\alpha=0$ 的基础解系有 $n$ 个，即 $n-r(A^{*})=n$，故 $r(A^{*})=0$，由 $r(A)$ 与 $r(A^{*})$ 的关系，知 $r(A)<n-1$，所以 $Ax=0$ 有 $k=n-r(A)>n-(n-1)=1$ 个基础解系，故 **C** 正确．

+++

#### 基础选择 (4) 设方程组 $\begin{cases}\lambda x_1+x_2+\lambda^{2}x_3=0,\\x_1+\lambda x_2+x_3=0,\\x_1+x_2+\lambda x_3=0\end{cases}$ 的系数矩阵为 $A$，若存在 $3$ 阶矩阵 $B\neq O$，使得 $AB=O$，则必有（　）．

;;;
A. $\lambda=-2$ 且 $|B|=0$
B. $\lambda=-2$ 且 $|B|\neq 0$
C. $\lambda=1$ 且 $|B|=0$
D. $\lambda=1$ 且 $|B|\neq 0$
;;;C
***
由 $AB=O$，知 $B$ 的每一个列向量都是 $Ax=0$ 的解．

又 $B\neq O$，知 $Ax=0$ 有非零解，从而

$$|A|=\begin{vmatrix}\lambda&1&\lambda^{2}\\1&\lambda&1\\1&1&\lambda\end{vmatrix}=(\lambda-1)^{2}=0,$$

所以 $\lambda=1$．

又若 $|B|\neq 0$，则 $B$ 可逆，故 $ABB^{-1}=A=O$，与 $A\neq O$ 矛盾，所以 $|B|=0$．

【注】由 $B\neq O$ 不能直接推得 $|B|\neq 0$，应注意矩阵不为零与行列式不为零的区别．

+++

#### 基础选择 (5) 设方程组 $\begin{cases}2x_1-3x_2+x_3=b_1,\\x_1-2x_2+x_3=b_2,\\2x_1+kx_2+3x_3=b_3\end{cases}$ 有解，则（　）．

;;;
A. 当 $k\neq-5$ 时，$(b_1,b_2,b_3)^{\mathrm{T}}$ 为任意非零列向量
B. 当 $k=-5$ 时，$(b_1,b_2,b_3)^{\mathrm{T}}$ 为任意列向量
C. 当 $k=-5$ 时，$b_1+b_3=4b_2$
D. 当 $k\neq-5$ 时，$b_1+b_3=4b_2$
;;;C
***
对增广矩阵 $(A\mid b)$ 作初等行变换，

$$(A\mid b)=\begin{pmatrix}2&-3&1&b_1\\1&-2&1&b_2\\2&k&3&b_3\end{pmatrix}\longrightarrow\begin{pmatrix}1&-2&1&b_2\\0&1&-1&b_1-2b_2\\0&k+4&1&b_3-2b_2\end{pmatrix}$$

$$\longrightarrow\begin{pmatrix}1&-2&1&b_2\\0&1&-1&b_1-2b_2\\0&k+5&0&b_1+b_3-4b_2\end{pmatrix},$$

由方程组有解，知 $r(A)=r(A\mid b)$．

当 $k\neq-5$ 时，对任意向量 $b=(b_1,b_2,b_3)^{\mathrm{T}}$，有 $r(A)=r(A\mid b)=3$；

当 $k=-5$ 时，$r(A)=2$，当 $b_1+b_3-4b_2=0$，即 $b_1+b_3=4b_2$ 时，$r(A\mid b)=2$．

+++

#### 基础选择 (6) 设矩阵 $A_{m\times n}$，$B_{n\times m}$，则（　）．

;;;
A. 当 $m>n$ 时，$AB$ 必可逆
B. 当 $m>n$ 时，必有 $|AB|=0$
C. 当 $n>m$ 时，必有 $r(AB)<m$
D. 当 $n>m$ 时，$ABx=0$ 必有唯一解
;;;B
***
对选项 **B**，由 $r(AB)\leqslant r(A)\leqslant n<m$，而 $AB$ 为 $m\times m$ 矩阵，故必有 $|AB|=0$．

+++

#### 基础填空 (1) 设方程组 $\begin{cases}x_1+2x_2+x_3=3,\\2x_1+(k+4)x_2-5x_3=6,\\-x_1-2x_2+kx_3=-3\end{cases}$ 有无穷多解，则 $k=$ ________．
***
$-1$ 或 $0$．

对非齐次线性方程组的增广矩阵 $(A\mid b)$ 作初等行变换，

$$(A\mid b)=\begin{pmatrix}1&2&1&3\\2&k+4&-5&6\\-1&-2&k&-3\end{pmatrix}\longrightarrow\begin{pmatrix}1&2&1&3\\0&k&-7&0\\0&0&k+1&0\end{pmatrix},$$

由方程组有无穷多解，知 $r(A)=r(A\mid b)<3$，故 $k=-1$ 或 $k=0$．

+++

#### 基础解答 (1) 求方程组 $\begin{cases}2x_1-x_2+4x_3-3x_4=-4,\\x_1+x_3-x_4=-3,\\3x_1+x_2+x_3=1,\\7x_1+7x_3-3x_4=3\end{cases}$ 的通解．
***
对增广矩阵 $(A\mid b)$ 作初等行变换，

$$(A\mid b)=\begin{pmatrix}2&-1&4&-3&-4\\1&0&1&-1&-3\\3&1&1&0&1\\7&0&7&-3&3\end{pmatrix}\longrightarrow\begin{pmatrix}1&0&1&-1&-3\\0&1&-2&1&-2\\0&0&0&2&12\\0&0&0&0&0\end{pmatrix},$$

取 $x_3$ 为自由变量，令 $x_3=0$，得非齐次线性方程组的一个特解为 $x^{*}=(3,-8,0,6)^{\mathrm{T}}$．

令 $x_3=1$，解得 $x_4=0$，$x_2=2$，$x_1=-1$，故 $(-1,2,1,0)^{\mathrm{T}}$ 为对应齐次线性方程组的基础解系，所求通解为

$$k(-1,2,1,0)^{\mathrm{T}}+(3,-8,0,6)^{\mathrm{T}}\quad(k\text{ 为任意常数}).$$

+++

#### 基础解答 (2) 设方程组 $\begin{cases}2x_1+\lambda x_2-x_3=1,\\\lambda x_1-x_2+x_3=2,\\4x_1+5x_2-5x_3=-1,\end{cases}$ 问 $\lambda$ 为何值时，方程组无解、有唯一解、有无穷多解？当有无穷多解时，求其通解．
***
已知方程组的系数矩阵 $A$ 为 $3$ 阶方阵，可以通过行列式讨论参数 $\lambda$，确定其解的情况．

$$|A|=\begin{vmatrix}2&\lambda&-1\\\lambda&-1&1\\4&5&-5\end{vmatrix}=(5\lambda+4)(\lambda-1).$$

当 $\lambda\neq 1$ 且 $\lambda\neq-\dfrac{4}{5}$ 时，$|A|\neq 0$，方程组**有唯一解**．

当 $\lambda=1$ 时，$|A|=0$，对增广矩阵 $(A\mid b)$ 作初等行变换，

$$(A\mid b)=\begin{pmatrix}2&1&-1&1\\1&-1&1&2\\4&5&-5&-1\end{pmatrix}\longrightarrow\begin{pmatrix}1&-1&1&2\\0&1&-1&-1\\0&0&0&0\end{pmatrix},$$

方程组**有无穷多解**，为 $k(0,1,1)^{\mathrm{T}}+(1,-1,0)^{\mathrm{T}}$（$k$ 为任意常数）．

当 $\lambda=-\dfrac{4}{5}$ 时，

$$(A\mid b)\longrightarrow\begin{pmatrix}10&-4&-5&5\\4&5&-5&-10\\4&5&-5&-1\end{pmatrix}\longrightarrow\begin{pmatrix}10&-4&-5&5\\4&5&-5&-10\\0&0&0&9\end{pmatrix},$$

此时 $r(A)=2$，$r(A\mid b)=3$，方程组**无解**．

【注】含有参数的线性方程组解的讨论方法：

① $A_{n\times n}x=b$，可利用 $|A|$ 讨论参数（当然也可利用初等行变换）．当 $|A|\neq 0$ 时，方程组有唯一解，用克拉默法则求其唯一解；当 $|A|=0$ 时，确定参数，再利用增广矩阵施行初等行变换化为阶梯形进行判别，有解时，求出通解（应注意，$|A|=0$ 时，方程组可能无解）．

② $A_{m\times n}x=b\ (m\neq n)$，一般利用初等行变换化增广矩阵为阶梯形，讨论参数，确定其秩，从而求解．

含参数方程组是常考题，要求熟练掌握．

+++

#### 基础解答 (3) 设有方程组 ① $\begin{cases}x_1+x_2=0,\\x_2-x_4=0\end{cases}$ 与 ② $\begin{cases}x_1-x_2+x_3=0,\\x_2-x_3+x_4=0.\end{cases}$

（Ⅰ）求方程组 ① 与 ② 的基础解系；\
（Ⅱ）求方程组 ① 与 ② 的非零公共解．
***
（Ⅰ）方程组 ① 的系数矩阵为 $A=\begin{pmatrix}1&1&0&0\\0&1&0&-1\end{pmatrix}$，可求得基础解系为

$$\alpha_1=(-1,1,0,1)^{\mathrm{T}},\quad \alpha_2=(0,0,1,0)^{\mathrm{T}}.$$

方程组 ② 的系数矩阵为 $B=\begin{pmatrix}1&-1&1&0\\0&1&-1&1\end{pmatrix}$，解得基础解系为

$$\beta_1=(0,1,1,0)^{\mathrm{T}},\quad \beta_2=(-1,-1,0,1)^{\mathrm{T}}.$$

（Ⅱ）求方程组 ① 与 ② 的非零公共解，就是求 $\begin{pmatrix}A\\B\end{pmatrix}x=0$ 的非零解．

$$\begin{pmatrix}A\\B\end{pmatrix}=\begin{pmatrix}1&1&0&0\\0&1&0&-1\\1&-1&1&0\\0&1&-1&1\end{pmatrix}\longrightarrow\begin{pmatrix}1&1&0&0\\0&1&0&-1\\0&-2&1&0\\0&0&-1&2\end{pmatrix}\longrightarrow\begin{pmatrix}1&1&0&0\\0&1&0&-1\\0&0&1&-2\\0&0&0&0\end{pmatrix},$$

得基础解系 $\eta=(-1,1,2,1)^{\mathrm{T}}$，故非零公共解为 $k(-1,1,2,1)^{\mathrm{T}}$（$k$ 是不为零的任意常数）．

【注】由第（Ⅰ）问已求出 ① 与 ② 的基础解系，可令

$$k_1\alpha_1+k_2\alpha_2=l_1\beta_1+l_2\beta_2,$$

即解方程组 $k_1\alpha_1+k_2\alpha_2-l_1\beta_1-l_2\beta_2=0$，故有

$$\begin{cases}-k_1+l_2=0,\\k_1-l_1+l_2=0,\\k_2-l_1=0,\\k_1-l_2=0,\end{cases}$$

解得 $l_1=k_2=2k_1=2l_2$，即

$$k_1\alpha_1+k_2\alpha_2=k_1\alpha_1+2k_1\alpha_2=k_1(\alpha_1+2\alpha_2)$$

$$=l_1\beta_1+l_2\beta_2=2l_2\beta_1+l_2\beta_2=l_2(2\beta_1+\beta_2)=k(-1,1,2,1)^{\mathrm{T}}\ (k\neq 0),$$

其中记 $k=l_1=k_2=2k_1=2l_2$．

+++

#### 基础解答 (4) 设有方程组（Ⅰ）$\begin{cases}x_1+x_2=0,\\x_2-x_4=0,\end{cases}$（Ⅱ）$Ax=0$，其中（Ⅱ）的基础解系为 $\alpha_1=(-1,2,2,1)^{\mathrm{T}}$，$\alpha_2=(0,-1,-1,0)^{\mathrm{T}}$，求方程组（Ⅰ）与（Ⅱ）的非零公共解．
***
方程组（Ⅰ）的系数矩阵 $B=\begin{pmatrix}1&1&0&0\\0&1&0&-1\end{pmatrix}$，故（Ⅰ）的基础解系为 $\xi_1=(0,0,1,0)^{\mathrm{T}}$，$\xi_2=(-1,1,0,1)^{\mathrm{T}}$，通解为

$$k_1\xi_1+k_2\xi_2=(-k_2,k_2,k_1,k_2)^{\mathrm{T}}\quad(k_1,k_2\text{ 为任意常数}).$$

由已知，（Ⅱ）的通解为

$$l_1\alpha_1+l_2\alpha_2=(-l_1,2l_1-l_2,2l_1-l_2,l_1)^{\mathrm{T}}\quad(l_1,l_2\text{ 为任意常数}).$$

令 $(-k_2,k_2,k_1,k_2)^{\mathrm{T}}=(-l_1,2l_1-l_2,2l_1-l_2,l_1)^{\mathrm{T}}$，得

$$l_1=k_2,\quad l_2=2k_2-k_2=k_2,\quad k_1=k_2.$$

令 $k_2=k$，则（Ⅰ）与（Ⅱ）的非零公共解为 $k(-1,1,1,1)^{\mathrm{T}}$（$k$ 为不为零的任意常数）．

+++

#### 基础解答 (5) 设有方程组 ① $\begin{cases}x_1-x_4=-2,\\x_2-x_4=-4,\\-4x_2-x_3+6x_4=21,\end{cases}$ ② $\begin{cases}x_1+ax_2-x_3-x_4=-5,\\bx_2-x_3-2x_4=-11,\\x_3-2x_4=-c+1.\end{cases}$

（Ⅰ）求方程组 ① 的通解；\
（Ⅱ）当 $a,b,c$ 为何值时，方程组 ① 与 ② 同解．
***
（Ⅰ）对 ① 的增广矩阵作初等行变换，

$$(A_1\mid b_1)=\begin{pmatrix}1&0&0&-1&-2\\0&1&0&-1&-4\\0&-4&-1&6&21\end{pmatrix}\longrightarrow\begin{pmatrix}1&0&0&-1&-2\\0&1&0&-1&-4\\0&0&1&-2&-5\end{pmatrix},$$

解得 ① 的通解为

$$(x_1,x_2,x_3,x_4)^{\mathrm{T}}=(-2,-4,-5,0)^{\mathrm{T}}+k(1,1,2,1)^{\mathrm{T}}\quad(k\text{ 为任意常数}).$$

（Ⅱ）将方程组 ① 的通解 $x_1=-2+k$，$x_2=-4+k$，$x_3=-5+2k$，$x_4=k$ 代入方程组 ② 的第一个方程，得

$$(-2+k)+a(-4+k)-(-5+2k)-k=-5,$$

由 $k$ 的任意性，可得 $a=2$．同样将 ① 的通解代入 ② 的第二个方程，得

$$b(-4+k)-(-5+2k)-2k=-11,$$

解得 $b=4$．

将 ① 的通解代入 ② 中的第三个方程，得 $(-5+2k)-2k=-c+1$，解得 $c=6$，故方程组 ② 为

$$\begin{cases}x_1+2x_2-x_3-x_4=-5,\\4x_2-x_3-2x_4=-11,\\x_3-2x_4=-5.\end{cases}$$

对其增广矩阵作初等行变换，得

$$\begin{pmatrix}1&2&-1&-1&-5\\0&4&-1&-2&-11\\0&0&1&-2&-5\end{pmatrix}\longrightarrow\begin{pmatrix}1&0&0&-1&-2\\0&1&0&-1&-4\\0&0&1&-2&-5\end{pmatrix},$$

故 ② 的通解为

$$(x_1,x_2,x_3,x_4)^{\mathrm{T}}=(-2,-4,-5,0)^{\mathrm{T}}+k(1,1,2,1)^{\mathrm{T}},$$

与 ① 的通解相同．

综上所述，当 $a=2$，$b=4$，$c=6$ 时，方程组 ① 与 ② 同解．

+++

#### 基础解答 (6) 设 $n$ 阶矩阵 $A$ 满足 $|A|=0$，$A_{ij}$ 为 $|A|$ 的元素 $a_{ij}$ 对应的代数余子式，且 $A_{11}\neq 0$，求方程组 $A^{*}x=0$ 的基础解系和通解．
***
由 $|A|=0$，$A_{11}\neq 0$，得 $r(A)=n-1$，故 $r(A^{*})=1$，即 $A^{*}x=0$ 等价于方程

$$A_{11}x_1+A_{21}x_2+\cdots+A_{n1}x_n=0.\qquad ①$$

因 $A_{11}\neq 0$，故方程 ① 有下列线性无关的解，

$$\alpha_1=(-A_{21},A_{11},0,\cdots,0)^{\mathrm{T}},$$

$$\alpha_2=(-A_{31},0,A_{11},0,\cdots,0)^{\mathrm{T}},$$

$$\cdots\cdots$$

$$\alpha_{n-1}=(-A_{n1},0,\cdots,0,A_{11})^{\mathrm{T}},$$

解向量个数为 $n-r(A^{*})=n-1$，故 $\alpha_1,\alpha_2,\cdots,\alpha_{n-1}$ 是原方程组的**基础解系**，通解为

$$k_1\alpha_1+k_2\alpha_2+\cdots+k_{n-1}\alpha_{n-1}\quad(k_1,k_2,\cdots,k_{n-1}\text{ 为任意常数}).$$

+++

#### 基础解答 (7) 已知 $4\times 3$ 矩阵 $A=(\alpha_1,\alpha_2,\alpha_3)$，非齐次线性方程组 $Ax=\beta$ 的通解为 $(1,2,-1)^{\mathrm{T}}+k(1,-2,3)^{\mathrm{T}}$，$k$ 为任意常数，令 $B=(\alpha_1,\alpha_2,\alpha_3,\beta+\alpha_3)$，求方程组 $By=\alpha_1-\alpha_2$ 的通解．
***
由 $Ax=\beta$ 的通解结构及已知条件，有

$$r(A)=r(\alpha_1,\alpha_2,\alpha_3)=3-1=2,$$

$$(\alpha_1,\alpha_2,\alpha_3)\begin{pmatrix}1\\2\\-1\end{pmatrix}=\beta,\quad(\alpha_1,\alpha_2,\alpha_3)\begin{pmatrix}1\\-2\\3\end{pmatrix}=0,$$

即 $\alpha_1+2\alpha_2-\alpha_3=\beta$，$\alpha_1-2\alpha_2+3\alpha_3=0$，故

$$r(B)=r(\alpha_1,\alpha_2,\alpha_3,\beta+\alpha_3)=r(\alpha_1,\alpha_2,\alpha_3,\alpha_1+2\alpha_2)$$

$$\xrightarrow{\text{初等列变换}}r(\alpha_1,\alpha_2,\alpha_3,0)=r(\alpha_1,\alpha_2,\alpha_3)=2,$$

所以 $By=0$ 有 $4-r(B)=2$ 个基础解．又

$$(\alpha_1,\alpha_2,\alpha_3,\beta+\alpha_3)\begin{pmatrix}1\\-2\\3\\0\end{pmatrix}=\alpha_1-2\alpha_2+3\alpha_3=0,$$

$$(\alpha_1,\alpha_2,\alpha_3,\alpha_1+2\alpha_2)\begin{pmatrix}1\\2\\0\\-1\end{pmatrix}=\alpha_1+2\alpha_2-(\alpha_1+2\alpha_2)=0,$$

及 $(\alpha_1,\alpha_2,\alpha_3,\beta+\alpha_3)\begin{pmatrix}1\\-1\\0\\0\end{pmatrix}=\alpha_1-\alpha_2$，故 $By=\alpha_1-\alpha_2$ 的通解为

$$k_1(1,-2,3,0)^{\mathrm{T}}+k_2(1,2,0,-1)^{\mathrm{T}}+(1,-1,0,0)^{\mathrm{T}}\quad(k_1,k_2\text{ 为任意常数}).$$

+++

#### 综合选择 (1) 设 $P_i(x_i,y_i)$，$i=1,2,3$ 为平面上三个不同的点，又 $A=\begin{pmatrix}x_1&y_1&1\\x_2&y_2&1\\x_3&y_3&1\end{pmatrix}$，则三点 $P_1,P_2,P_3$ 在同一条直线上的充要条件是（　）．

;;;
A. $r(A)=1$
B. $r(A)=2$
C. $|A|=0$
D. $|A|\neq 0$
;;;B
***
从几何上考虑，由 $P_1,P_2,P_3$ 在 $xOy$ 面中是在同一直线上的三点，知空间中的三点 $M_1(x_1,y_1,1)$，$M_2(x_2,y_2,1)$，$M_3(x_3,y_3,1)$ 在同一平面 $z=1$ 上，即为同一空间直线上三个不同点，因此三个向量 $\overrightarrow{OM_1},\overrightarrow{OM_2},\overrightarrow{OM_3}$ 共面但不共线，

$$|A|=\overrightarrow{OM_1},\overrightarrow{OM_2},\overrightarrow{OM_3}\ \text{的混合积}=0,$$

故 $r(A)<3$，又不共线，知 $r(A)>1$，故 $r(A)=2$．

+++

#### 综合选择 (2) 设 $A$ 是 $m\times n$ 矩阵，$m<n$，且 $A$ 的行向量组线性无关，$b_1,b_2$ 分别为 $m$ 维、$n$ 维非零列向量，则下列选项**错误**的是（　）．

;;;
A. $A^{\mathrm{T}}x=0$ 只有零解
B. $A^{\mathrm{T}}Ax=0$ 必有非零解
C. $Ax=b_1$ 必有无穷多个解
D. $A^{\mathrm{T}}x=b_2$ 必有唯一解
;;;D
***
由 $r(A)=A$ 的行秩 $=A$ 的列秩，及 $A$ 的行向量组线性无关，可知 $r(A)=m$．

对于 **A**，$A^{\mathrm{T}}$ 是 $n\times m$ 矩阵，$r(A^{\mathrm{T}})=r(A)=m$，即 $A^{\mathrm{T}}$ 的列向量组线性无关，故 $A^{\mathrm{T}}x=0$ 只有零解．

对于 **B**，$A^{\mathrm{T}}A$ 是 $n\times n$ 矩阵，由 $r(A^{\mathrm{T}}A)\leqslant r(A)=m<n$，故 $A^{\mathrm{T}}Ax=0$ 必有非零解．

对于 **C**，$A$ 是 $m\times n$ 矩阵，$r(A)=m$，故 $r(A)=r(A\mid b_1)=m<n$，即 $Ax=b_1$ 必有无穷多个解．

对于 **D**，$A^{\mathrm{T}}$ 是 $n\times m$ 矩阵，$A^{\mathrm{T}}x=b_2$ 有唯一解 $\Leftrightarrow r(A^{\mathrm{T}})=r(A^{\mathrm{T}}\mid b_2)=m$，但 $A^{\mathrm{T}}$ 的列向量只是 $m$ 个线性无关的 $n$ 维向量（$m<n$），它不能表示任一个 $n$ 维向量，故 $A^{\mathrm{T}}x=b_2$ 可能无解，故选 **D**．

+++

#### 综合选择 (3) 设 $A$ 是 $m\times n$ 矩阵，则非齐次线性方程组 $Ax=b$ 有无穷多解的充分必要条件是（　）．

;;;
A. $r(A\mid b)<n$
B. $Ax=0$ 有非零解
C. $Ax=b$ 有两个不同解
D. $A$ 的列向量组线性相关
;;;C
***
$Ax=b$ 有无穷多解 $\Leftrightarrow r(A)=r(A\mid b)<n$．

对于 **A**，由 $r(A\mid b)<n\nRightarrow r(A)=r(A\mid b)$，故排除 **A**．

对于 **B**，$Ax=0$ 有非零解 $\nRightarrow Ax=b$ 有无穷多解，因为 $Ax=0$ 有非零解 $\Leftrightarrow r(A)<n$，但可能 $r(A)\neq r(A\mid b)$，即 $Ax=b$ 可能无解．

对于 **C**，设 $Ax=b$ 有两个不同解 $\alpha_1,\alpha_2$，则 $\alpha_1-\alpha_2$ 是 $Ax=0$ 的非零解 $\Rightarrow r(A)<n$，且 $Ax=b$ 有解，即 $r(A)=r(A\mid b)<n$，故 $Ax=b$ 有无穷多解．而 $Ax=b$ 有无穷多解时，肯定有两个不同解，故 **C** 正确．

对于 **D**，$A$ 的列向量组线性相关 $\Leftrightarrow Ax=0$ 有非零解．而 $Ax=0$ 有非零解 $\nRightarrow Ax=b$ 有无穷多解（可能无解）．

+++

#### 综合选择 (4) 设三个不同平面的方程为 $a_{i1}x+a_{i2}y+a_{i3}z=b_i\ (i=1,2,3)$ 相交于一条直线，三个平面方程组成方程组的系数矩阵和增广矩阵分别记为 $A$ 和 $\overline{A}$，则（　）．

;;;
A. $r(A)=2$，$r(\overline{A})=2$
B. $r(A)=2$，$r(\overline{A})=3$
C. $r(A)=1$，$r(\overline{A})=2$
D. $r(A)=1$，$r(\overline{A})=1$
;;;A
***
用排除法，依题设，三个不同平面交于一条直线，则方程组

$$\begin{cases}a_{11}x+a_{12}y+a_{13}z=b_1,\\a_{21}x+a_{22}y+a_{23}z=b_2,\\a_{31}x+a_{32}y+a_{33}z=b_3\end{cases}$$

有无穷多解，故 $r(A)=r(\overline{A})<3$，排除 **B、C**．

若 $r(A)=1$，$r(\overline{A})=1$，则三个平面重合，故排除 **D**．

【注】三个平面的位置关系，即讨论线性方程组 $Ax=b$ 的解，从而可用系数矩阵 $A$ 及增广矩阵 $\overline{A}$ 的秩进行判断：

① 三平面相交于一点，则 $Ax=b$ 有唯一解，$r(A)=r(\overline{A})=3$．

② 三平面重合，则 $Ax=b$ 有无穷多解，$r(A)=r(\overline{A})=1$．

③ 三平面平行，或有两平面重合、另一个平面与它们平行，则 $Ax=b$ 无解，$r(A)=1$，$r(\overline{A})=2$．

④ 三平面交于一直线，或有两个平面相交、另一个平面与其中一个平面重合，则 $Ax=b$ 有无穷多解，$r(A)=2$，$r(\overline{A})=2$．

⑤ 三平面两两相交且三平面互不平行，或有两个平面平行、另一个平面与这两个平面分别相交，则 $Ax=b$ 无解，$r(A)=2$，$r(\overline{A})=3$．

+++

#### 综合选择 (5) 设 $A^{\mathrm{T}}=(\alpha_1,\alpha_2,\cdots,\alpha_{n-1})$ 是 $n\times(n-1)$ 矩阵，$r(A^{\mathrm{T}})=n-1$，$\beta_1,\beta_2$ 是与 $\alpha_1,\alpha_2,\cdots,\alpha_{n-1}$ 都正交的两个不同的 $n$ 维列向量，$k$ 是任意常数，则方程组 $Ax=0$ 的通解为（　）．

;;;
A. $k(\beta_1-\beta_2)$
B. $k(\beta_1+\beta_2)$
C. $k\beta_1$
D. $k\beta_2$
;;;A
***
由已知，$r(A)=r(A^{\mathrm{T}})=n-1$，$Ax=0$ 的基础解系有 $n-r(A)=1$ 个向量．

因为 $\beta_1,\beta_2$ 与 $\alpha_1,\alpha_2,\cdots,\alpha_{n-1}$ 都正交，所以

$$\alpha_i^{\mathrm{T}}\cdot\beta_1=0,\quad\alpha_i^{\mathrm{T}}\cdot\beta_2=0,\quad i=1,2,\cdots,n-1,$$

从而

$$A\beta_j=\begin{pmatrix}\alpha_1^{\mathrm{T}}\\\alpha_2^{\mathrm{T}}\\\vdots\\\alpha_{n-1}^{\mathrm{T}}\end{pmatrix}\beta_j=\begin{pmatrix}0\\0\\\vdots\\0\end{pmatrix},\quad j=1,2,$$

由此可知 $\beta_1,\beta_2$ 是 $Ax=0$ 的两个不同解，故 $k(\beta_1-\beta_2)$ 是 $Ax=0$ 的通解．

由于 $\beta_1,\beta_2$ 可能是零向量，故排除 **C、D**；由于 $\beta_1+\beta_2$ 也可能是零向量，故排除 **B**．

+++

#### 综合填空 (1) 设 $\alpha_1,\alpha_2,\alpha_3,\beta$ 均为三维列向量，$A=(\beta-\alpha_1-2\alpha_2-3\alpha_3,\alpha_1,\alpha_2,\alpha_3)$，则方程组 $Ax=\beta$ 的一个特解为 ________．
***
$(1,1,2,3)^{\mathrm{T}}$．

设 $Ax=\beta$ 有特解 $\alpha^{*}=(x_1,x_2,x_3,x_4)^{\mathrm{T}}$，则

$$A\alpha^{*}=(\beta-\alpha_1-2\alpha_2-3\alpha_3,\alpha_1,\alpha_2,\alpha_3)\begin{pmatrix}x_1\\x_2\\x_3\\x_4\end{pmatrix}$$

$$=(\beta-\alpha_1-2\alpha_2-3\alpha_3)x_1+\alpha_1x_2+\alpha_2x_3+\alpha_3x_4$$

$$=\beta x_1+(x_2-x_1)\alpha_1+(x_3-2x_1)\alpha_2+(x_4-3x_1)\alpha_3=\beta.$$

只要取 $x_1=x_2=1$，$x_3=2x_1=2$，$x_4=3x_1=3$ 即可，故 $Ax=\beta$ 有一个特解为 $(1,1,2,3)^{\mathrm{T}}$．

+++

#### 综合填空 (2) 设 $A=(a_{ij})_{3\times 3}$ 为实矩阵，且 $A_{ij}=a_{ij}\ (i,j=1,2,3)$，其中 $A_{ij}$ 为 $a_{ij}$ 的代数余子式，$a_{33}=1$，$|A|=1$，则方程组 $A\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\begin{pmatrix}0\\0\\1\end{pmatrix}$ 的解为 ________．
***
$(x_1,x_2,x_3)^{\mathrm{T}}=(0,0,1)^{\mathrm{T}}$．

由已知，$A_{ij}=a_{ij}$，知 $A^{*}=A^{\mathrm{T}}$，故

$$\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=A^{-1}\begin{pmatrix}0\\0\\1\end{pmatrix}=\frac{A^{*}}{|A|}\begin{pmatrix}0\\0\\1\end{pmatrix}=A^{\mathrm{T}}\begin{pmatrix}0\\0\\1\end{pmatrix}=\begin{pmatrix}a_{31}\\a_{32}\\1\end{pmatrix}.$$

又

$$|A|=a_{31}A_{31}+a_{32}A_{32}+a_{33}A_{33}=a_{31}^{2}+a_{32}^{2}+1=1,$$

知 $a_{31}=a_{32}=0$，所以 $(x_1,x_2,x_3)^{\mathrm{T}}=(0,0,1)^{\mathrm{T}}$．

+++

#### 综合解答 (1) 设 $A$ 是 $m\times n$ 矩阵，$r(A)=n-2$，非齐次线性方程组 $Ax=b$ 的 $3$ 个解向量 $\alpha_1,\alpha_2,\alpha_3$ 满足 $\alpha_1+\alpha_2=(1,2,3,4)^{\mathrm{T}}$，$\alpha_2+2\alpha_3=(-2,1,5,3)^{\mathrm{T}}$，$2\alpha_3+3\alpha_1=(11,5,-6,7)^{\mathrm{T}}$，求方程组 $Ax=b$ 的通解．
***
依题设，找出 $Ax=0$ 的基础解及 $Ax=b$ 的一个特解．

由解的性质，$A\alpha_1=b$，$A\alpha_2=b$，故 $A\left(\dfrac{\alpha_1+\alpha_2}{2}\right)=b$，取

$$\eta^{*}=\frac{1}{2}(\alpha_1+\alpha_2)=\left(\frac{1}{2},1,\frac{3}{2},2\right)^{\mathrm{T}}$$

为 $Ax=b$ 的特解．又

$$A(\alpha_1+\alpha_2)=2b,\quad A(\alpha_2+2\alpha_3)=3b,\quad A(2\alpha_3+3\alpha_1)=5b,$$

故

$$A\left[3(\alpha_1+\alpha_2)-2(\alpha_2+2\alpha_3)\right]=6b-6b=0,$$

$$A\left[(2\alpha_3+3\alpha_1)-(\alpha_1+\alpha_2)-(\alpha_2+2\alpha_3)\right]=5b-5b=0,$$

所以

$$\eta_1=3(\alpha_1+\alpha_2)-2(\alpha_2+2\alpha_3)=(7,4,-1,6)^{\mathrm{T}},$$

$$\eta_2=(2\alpha_3+3\alpha_1)-(\alpha_1+\alpha_2)-(\alpha_2+2\alpha_3)=(12,2,-14,0)^{\mathrm{T}}$$

为 $Ax=0$ 的解，且线性无关（不成比例）．

又 $r(A)=n-2$，故 $\eta_1,\eta_2$ 是 $Ax=0$ 的基础解系，故 $Ax=b$ 的通解为

$$k_1(7,4,-1,6)^{\mathrm{T}}+k_2(12,2,-14,0)^{\mathrm{T}}+\left(\frac{1}{2},1,\frac{3}{2},2\right)^{\mathrm{T}}\quad(k_1,k_2\text{ 为任意常数}).$$

+++

#### 综合解答 (2) 设 $A=(\alpha_1,\alpha_2,\alpha_3,\alpha_4)$ 是 $4$ 阶矩阵，非齐次线性方程组 $Ax=\beta$ 的通解为 $(1,2,2,1)^{\mathrm{T}}+k(1,-2,4,0)^{\mathrm{T}}$，$k$ 为任意常数，记 $B=(\alpha_3,\alpha_2,\alpha_1,\beta-\alpha_4)$．

（Ⅰ）证明：$r(B)=2$；\
（Ⅱ）求方程组 $Bx=\alpha_1-\alpha_2$ 的通解．
***
（Ⅰ）由 $Ax=\beta$ 的解的结构，知 $r(A)=r(\alpha_1,\alpha_2,\alpha_3,\alpha_4)=3$，并有

$$(\alpha_1,\alpha_2,\alpha_3,\alpha_4)\begin{pmatrix}1\\2\\2\\1\end{pmatrix}=\beta,\quad(\alpha_1,\alpha_2,\alpha_3,\alpha_4)\begin{pmatrix}1\\-2\\4\\0\end{pmatrix}=0,$$

即

$$\alpha_1+2\alpha_2+2\alpha_3+\alpha_4=\beta,\qquad ①$$

$$\alpha_1-2\alpha_2+4\alpha_3=0.\qquad ②$$

由 ① 式，知

$$B=(\alpha_3,\alpha_2,\alpha_1,\beta-\alpha_4)=(\alpha_3,\alpha_2,\alpha_1,\alpha_1+2\alpha_2+2\alpha_3),$$

又由 ② 式，知 $\alpha_1,\alpha_2,\alpha_3$ 线性相关，由于 $r(A)=3$，故 $r(B)=r(\alpha_3,\alpha_2,\alpha_1)=2$．

（Ⅱ）由 $(\alpha_3,\alpha_2,\alpha_1,\beta-\alpha_4)\begin{pmatrix}0\\-1\\1\\0\end{pmatrix}=\alpha_1-\alpha_2$，知 $(0,-1,1,0)^{\mathrm{T}}$ 是 $Bx=\alpha_1-\alpha_2$ 的一个解．

又由于

$$(\alpha_3,\alpha_2,\alpha_1,\alpha_1+2\alpha_2+2\alpha_3)\begin{pmatrix}4\\-2\\1\\0\end{pmatrix}=4\alpha_3-2\alpha_2+\alpha_1=0,$$

$$(\alpha_3,\alpha_2,\alpha_1,\alpha_1+2\alpha_2+2\alpha_3)\begin{pmatrix}2\\-4\\0\\1\end{pmatrix}=\alpha_1-2\alpha_2+4\alpha_3=0,$$

且 $(4,-2,1,0)^{\mathrm{T}}$ 与 $(2,-4,0,1)^{\mathrm{T}}$ 线性无关，故 $Bx=\alpha_1-\alpha_2$ 的通解为

$$(0,-1,1,0)^{\mathrm{T}}+k_1(4,-2,1,0)^{\mathrm{T}}+k_2(2,-4,0,1)^{\mathrm{T}},$$

其中 $k_1,k_2$ 为任意常数．

+++

#### 综合解答 (3) 设 $A$ 为 $3\times 4$ 矩阵，$r(A)=1$，若向量组 $\alpha_1=(1,2,0,2)^{\mathrm{T}}$，$\alpha_2=(-1,-1,1,a)^{\mathrm{T}}$，$\alpha_3=(1,-1,a,5)^{\mathrm{T}}$，$\alpha_4=(2,a,-3,-5)^{\mathrm{T}}$ 与方程组 $Ax=0$ 的基础解系等价，求 $Ax=0$ 的通解．
***
由 $\alpha_1,\alpha_2,\alpha_3,\alpha_4$ 与 $Ax=0$ 的基础解系等价，知 $\alpha_1,\alpha_2,\alpha_3,\alpha_4$ 必是 $Ax=0$ 的解，又 $r(A)=1$，知 $Ax=0$ 有 $n-r(A)=4-1=3$ 个线性无关的解向量，故

$$r(\alpha_1,\alpha_2,\alpha_3,\alpha_4)=3,$$

其极大线性无关组是 $Ax=0$ 的基础解系．

对 $(\alpha_1,\alpha_2,\alpha_3,\alpha_4)$ 作初等行变换，有

$$(\alpha_1,\alpha_2,\alpha_3,\alpha_4)=\begin{pmatrix}1&-1&1&2\\2&-1&-1&a\\0&1&a&-3\\2&a&5&-5\end{pmatrix}\longrightarrow\begin{pmatrix}1&-1&1&2\\0&1&-3&a-4\\0&0&a+3&1-a\\0&0&0&(1-a)(a-4)\end{pmatrix}.$$

当 $a=-3$ 时，$\alpha_1,\alpha_2,\alpha_4$ 是一个极大线性无关组，故 $Ax=0$ 的通解为

$$k_1(1,2,0,2)^{\mathrm{T}}+k_2(1,1,-1,3)^{\mathrm{T}}+k_3(2,-3,-3,-5)^{\mathrm{T}},$$

其中 $k_1,k_2,k_3$ 为任意常数．

当 $a=1$ 时，$\alpha_1,\alpha_2,\alpha_3$ 是一个极大线性无关组，故 $Ax=0$ 的通解为

$$k_1(1,2,0,2)^{\mathrm{T}}+k_2(-1,-1,1,1)^{\mathrm{T}}+k_3(1,-1,1,5)^{\mathrm{T}},$$

其中 $k_1,k_2,k_3$ 为任意常数．

当 $a=4$ 时，$\alpha_1,\alpha_2,\alpha_3$ 是一个极大线性无关组，故 $Ax=0$ 的通解为

$$k_1(1,2,0,2)^{\mathrm{T}}+k_2(-1,-1,1,4)^{\mathrm{T}}+k_3(1,-1,4,5)^{\mathrm{T}},$$

其中 $k_1,k_2,k_3$ 为任意常数．

+++

#### 综合解答 (4) 已知平面上三条不同直线的方程分别为 $l_1:ax+2by+3c=0$，$l_2:bx+2cy+3a=0$，$l_3:cx+2ay+3b=0$，证明：这三条直线交于一点的充分必要条件为 $a+b+c=0$．
***
**（必要性）** 设三条直线交于一点，则非齐次线性方程组

$$\begin{cases}ax+2by=-3c,\\bx+2cy=-3a,\\cx+2ay=-3b\end{cases}$$

有唯一解，故 $r(A)=r(\overline{A})=2$，其中

$$A=\begin{pmatrix}a&2b\\b&2c\\c&2a\end{pmatrix},\quad \overline{A}=\begin{pmatrix}a&2b&-3c\\b&2c&-3a\\c&2a&-3b\end{pmatrix}.$$

由 $r(\overline{A})=2<3$ 知 $|\overline{A}|=0$，即

$$\begin{vmatrix}a&2b&-3c\\b&2c&-3a\\c&2a&-3b\end{vmatrix}=(a+b+c)\begin{vmatrix}1&2&-3\\b&2c&-3a\\c&2a&-3b\end{vmatrix}$$

$$=(a+b+c)\begin{vmatrix}1&0&0\\b&2(c-b)&3(b-a)\\c&2(a-c)&3(c-b)\end{vmatrix}$$

$$=6(a+b+c)(a^{2}+b^{2}+c^{2}-ab-ac-bc)$$

$$=3(a+b+c)\left[(a-b)^{2}+(b-c)^{2}+(c-a)^{2}\right]=0.$$

又三条直线互不相同，故 $(a-b)^{2}+(b-c)^{2}+(c-a)^{2}\neq 0$，于是 $a+b+c=0$．

**（充分性）** 若 $a+b+c=0$，则 $|\overline{A}|=0$，故 $r(\overline{A})<3$．

又 $\begin{vmatrix}a&2b\\b&2c\end{vmatrix}=2(ac-b^{2})$，将 $c=-(a+b)$ 代入上式，得

$$\begin{vmatrix}a&2b\\b&2c\end{vmatrix}=-2\left[a(a+b)+b^{2}\right]=-2\left[\left(a+\frac{b}{2}\right)^{2}+\frac{3}{4}b^{2}\right]\neq 0,$$

故 $r(A)\geqslant 2$，$r(\overline{A})\geqslant 2$，又显然 $r(A)\leqslant 2$，所以 $r(A)=r(\overline{A})=2$，故方程组有唯一解，即三条直线交于一点．

+++

#### 综合解答 (5) 设 $A=\begin{pmatrix}1&-2&3\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}$ 有特征向量 $\alpha_1=(1,2,1)^{\mathrm{T}}$，$\alpha_2=(-1,1,1)^{\mathrm{T}}$，$\alpha_3=(-1,3,2)^{\mathrm{T}}$，且 $r(A)=1$，求方程组 $\begin{cases}x_1-2x_2+3x_3=-1,\\a_{21}x_1+a_{22}x_2+a_{23}x_3=3,\\a_{31}x_1+a_{32}x_2+a_{33}x_3=2\end{cases}$ 的通解．
***
$A$ 中有 $6$ 个未知参数，不能用初等行变换求解，利用特征向量的定义

$$A\alpha=\lambda\alpha\quad(\alpha\neq 0).$$

由已知，有

$$A\alpha_1=\begin{pmatrix}1&-2&3\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}\begin{pmatrix}1\\2\\1\end{pmatrix}=\lambda_1\begin{pmatrix}1\\2\\1\end{pmatrix},$$

得 $\lambda_1=0$，即 $A\alpha_1=0$．同理

$$A\alpha_2=\begin{pmatrix}1&-2&3\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}\begin{pmatrix}-1\\1\\1\end{pmatrix}=\lambda_2\begin{pmatrix}-1\\1\\1\end{pmatrix},$$

得 $\lambda_2=0$，即 $A\alpha_2=0$．

$$A\alpha_3=\begin{pmatrix}1&-2&3\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}\begin{pmatrix}-1\\3\\2\end{pmatrix}=\lambda_3\begin{pmatrix}-1\\3\\2\end{pmatrix},$$

得 $\lambda_3=1$，即 $A\alpha_3=\alpha_3$．

又 $3-r(A)=3-1=2$，$Ax=0$ 有两个基础解，故所求通解为 $k_1\alpha_1+k_2\alpha_2+\alpha_3$，$k_1,k_2$ 为任意常数．

+++

#### 综合解答 (6) 设 $A$ 是 $3$ 阶方阵，$A=(a_{ij})_{3\times 3}$，且 $a_{ij}=A_{ij}$，$i,j=1,2,3$，其中 $A_{ij}$ 为 $a_{ij}$ 的代数余子式，$a_{33}\neq 0$，$b=(a_{13},a_{23},a_{33})^{\mathrm{T}}$，求非齐次线性方程组 $Ax=b$ 的解．
***
求抽象方程组 $Ax=b$ 的通解，首先要讨论秩，从而确定解的情况．

由已知，$b=(a_{13},a_{23},a_{33})^{\mathrm{T}}$ 是 $A$ 中的第 $3$ 列，且 $a_{ij}=A_{ij}$，故

$$|A|=a_{13}A_{13}+a_{23}A_{23}+a_{33}A_{33}=a_{13}^{2}+a_{23}^{2}+a_{33}^{2}>0\quad(\text{因 }a_{33}\neq 0),$$

所以 $r(A)=3$，即 $Ax=b$ 有唯一解 $x=A^{-1}b$．而 $A^{-1}=\dfrac{A^{*}}{|A|}$，故

$$x=\frac{1}{|A|}\begin{pmatrix}A_{11}&A_{21}&A_{31}\\A_{12}&A_{22}&A_{32}\\A_{13}&A_{23}&A_{33}\end{pmatrix}\begin{pmatrix}a_{13}\\a_{23}\\a_{33}\end{pmatrix}=\frac{1}{|A|}\begin{pmatrix}0\\0\\|A|\end{pmatrix}=\begin{pmatrix}0\\0\\1\end{pmatrix}.$$

+++

#### 综合解答 (7) 设 $A$ 是 $m\times n$ 矩阵，$b$ 为 $m$ 维列向量，证明：线性方程组 $A^{\mathrm{T}}Ax=A^{\mathrm{T}}b$ 必有解．
***
只要证明 $r(A^{\mathrm{T}}A)=r(A^{\mathrm{T}}A\mid A^{\mathrm{T}}b)$．

记 $A=(\alpha_1,\alpha_2,\cdots,\alpha_n)$，则

$$r(A^{\mathrm{T}}A\mid A^{\mathrm{T}}b)=r(A^{\mathrm{T}}(\alpha_1,\alpha_2,\cdots,\alpha_n)\mid A^{\mathrm{T}}b)=r\left[(A^{\mathrm{T}}\alpha_1,A^{\mathrm{T}}\alpha_2,\cdots,A^{\mathrm{T}}\alpha_n)\mid A^{\mathrm{T}}b\right]$$

$$=r\left[A^{\mathrm{T}}(\alpha_1,\alpha_2,\cdots,\alpha_n\mid b)\right]\leqslant r(A^{\mathrm{T}})=r(A^{\mathrm{T}}A).$$

又 $r(A^{\mathrm{T}}A\mid A^{\mathrm{T}}b)\geqslant r(A^{\mathrm{T}}A)$，故 $r(A^{\mathrm{T}}A\mid A^{\mathrm{T}}b)=r(A^{\mathrm{T}}A)$，所以方程组 $A^{\mathrm{T}}Ax=A^{\mathrm{T}}b$ 必有解．

+++

#### 拓展解答 (1) 设 $A$ 是 $5\times 4$ 矩阵，$r(A)=2$，已知 $\alpha_1,\alpha_2,\alpha_3$ 是非齐次线性方程组 $Ax=b$ 的三个解向量，且 $\alpha_1+\alpha_2=(4,6,-8,4)^{\mathrm{T}}$，$\alpha_3=(1,2,-1,1)^{\mathrm{T}}$，又 $(0,1,-3,0)^{\mathrm{T}}$ 是 $Ax=0$ 的解，求 $Ax=b$ 的通解．
***
由已知条件及 $Ax=b$ 的通解结构，只需求 $Ax=0$ 的基础解系，而基础解系有 $n-r(A)=4-2=2$ 个，$(0,1,-3,0)^{\mathrm{T}}$ 是 $Ax=0$ 的一个解，于是再求一个与 $(0,1,-3,0)^{\mathrm{T}}$ 线性无关的解即可．

注意到 $\alpha_1+\alpha_2-2\alpha_3$ 是 $Ax=0$ 的解，事实上，

$$A(\alpha_1+\alpha_2-2\alpha_3)=A\alpha_1+A\alpha_2-2A\alpha_3=b+b-2b=0,$$

且

$$\alpha_1+\alpha_2-2\alpha_3=(4,6,-8,4)^{\mathrm{T}}-2(1,2,-1,1)^{\mathrm{T}}=(2,2,-6,2)^{\mathrm{T}},$$

又 $(2,2,-6,2)^{\mathrm{T}}$ 与 $(0,1,-3,0)^{\mathrm{T}}$ 线性无关（分量不成比例），所以 $Ax=b$ 的通解为

$$k_1\begin{pmatrix}0\\1\\-3\\0\end{pmatrix}+k_2\begin{pmatrix}2\\2\\-6\\2\end{pmatrix}+\begin{pmatrix}1\\2\\-1\\1\end{pmatrix}\quad(k_1,k_2\text{ 为任意常数}).$$

【注】结论：设 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 是 $Ax=b$ 的 $n$ 个解，当 $k_1+k_2+\cdots+k_n=1$ 时，$k_1\alpha_1+k_2\alpha_2+\cdots+k_n\alpha_n$ 也是 $Ax=b$ 的解．

+++

#### 拓展解答 (2) 设 $A$ 是 $3$ 阶矩阵，向量 $\beta=(3,3,3)^{\mathrm{T}}$，非齐次线性方程组 $Ax=\beta$ 的通解为 $k_1(1,2,-2)^{\mathrm{T}}+k_2(2,1,2)^{\mathrm{T}}+(1,1,1)^{\mathrm{T}}$，$k_1,k_2$ 为任意常数．

（Ⅰ）证明：任意 $3$ 维列向量 $\alpha$ 可由 $A$ 的三个特征向量线性表示；\
（Ⅱ）若 $\alpha=(1,2,-1)^{\mathrm{T}}$，求 $A\alpha$．
***
（Ⅰ）依题设，$(1,1,1)^{\mathrm{T}}$ 是 $Ax=\beta$ 的特解，$(1,2,-2)^{\mathrm{T}}$，$(2,1,2)^{\mathrm{T}}$ 是 $Ax=0$ 的基础解系，故

$$A\begin{pmatrix}1\\1\\1\end{pmatrix}=\begin{pmatrix}3\\3\\3\end{pmatrix}=3\begin{pmatrix}1\\1\\1\end{pmatrix},$$

所以 $\lambda_1=3$ 是 $A$ 的特征值，$\alpha_1=(1,1,1)^{\mathrm{T}}$ 是 $A$ 的一个特征向量．

$$A\begin{pmatrix}1\\2\\-2\end{pmatrix}=0=0\begin{pmatrix}1\\2\\-2\end{pmatrix},\quad A\begin{pmatrix}2\\1\\2\end{pmatrix}=0=0\cdot\begin{pmatrix}2\\1\\2\end{pmatrix},$$

故 $\lambda_2=\lambda_3=0$ 为 $A$ 的特征值，$\alpha_2=(1,2,-2)^{\mathrm{T}}$，$\alpha_3=(2,1,2)^{\mathrm{T}}$ 是 $A$ 的特征向量．而

$$|(\alpha_1,\alpha_2,\alpha_3)|=\begin{vmatrix}1&1&2\\1&2&1\\1&-2&2\end{vmatrix}=-3\neq 0,$$

故 $\alpha_1,\alpha_2,\alpha_3$ 为三个线性无关的 $3$ 维列向量，即 $\alpha_1,\alpha_2,\alpha_3$ 可作为 $\mathbf{R}^{3}$ 的一组基，所以任意 $3$ 维列向量 $\alpha$ 可由 $\alpha_1,\alpha_2,\alpha_3$ 线性表示．

（Ⅱ）由（Ⅰ）可设 $\alpha=x_1\alpha_1+x_2\alpha_2+x_3\alpha_3$，即

$$x_1\begin{pmatrix}1\\1\\1\end{pmatrix}+x_2\begin{pmatrix}1\\2\\-2\end{pmatrix}+x_3\begin{pmatrix}2\\1\\2\end{pmatrix}=\begin{pmatrix}1\\2\\-1\end{pmatrix},$$

解方程组

$$\begin{cases}x_1+x_2+2x_3=1,\\x_1+2x_2+x_3=2,\\x_1-2x_2+2x_3=-1,\end{cases}$$

得唯一解 $(x_1,x_2,x_3)^{\mathrm{T}}=\left(1,\dfrac{2}{3},-\dfrac{1}{3}\right)^{\mathrm{T}}$，故

$$A\alpha=A(x_1\alpha_1+x_2\alpha_2+x_3\alpha_3)=x_1A\alpha_1+x_2A\alpha_2+x_3A\alpha_3=3x_1\begin{pmatrix}1\\1\\1\end{pmatrix}=3\begin{pmatrix}1\\1\\1\end{pmatrix}=\begin{pmatrix}3\\3\\3\end{pmatrix}.$$
