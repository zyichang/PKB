---
quizify:
  format: 1
  deck: Math_880::Chapter_15
  tags: [Math, 880题, 数一, 第十五章, 二次型]
---

+++

#### 基础选择 (1) 二次型 $f(x_1,x_2,x_3)=x_1x_2+x_2x_3+x_1x_3$ 的矩阵为（　）．

;;;
A. $\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}$
B. $\begin{pmatrix}0&\dfrac{1}{2}&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&0&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&\dfrac{1}{2}&0\end{pmatrix}$
C. $\begin{pmatrix}1&\dfrac{1}{2}&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&1&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&\dfrac{1}{2}&1\end{pmatrix}$
D. $\begin{pmatrix}\dfrac{1}{2}&1&1\\[2pt]1&\dfrac{1}{2}&1\\[2pt]1&1&\dfrac{1}{2}\end{pmatrix}$
;;;B
***
由

$$f=(x_1,x_2,x_3)\begin{pmatrix}0&\dfrac{1}{2}&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&0&\dfrac{1}{2}\\[2pt]\dfrac{1}{2}&\dfrac{1}{2}&0\end{pmatrix}\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix},$$

知 **B** 正确．

+++

#### 基础选择 (2) 二次型 $f(x_1,x_2,x_3)=(x_1-x_2)^2+(x_2-x_3)^2+(x_3-x_1)^2$ 的标准形为（　）．

;;;
A. $f=y_1^2+y_2^2+y_3^2$
B. $f=2y_1^2+\dfrac{3}{2}y_2^2$
C. $f=y_1^2+y_2^2-y_3^2$
D. $f=2y_1^2+\dfrac{3}{2}y_2^2+y_3^2$
;;;B
***
用配方法，

$$f(x_1,x_2,x_3)=2x_1^2-2x_1(x_2+x_3)+\frac{1}{2}(x_2+x_3)^2+\frac{3}{2}x_2^2+\frac{3}{2}x_3^2-3x_2x_3$$

$$=2\left(x_1-\frac{1}{2}x_2-\frac{1}{2}x_3\right)^2+\frac{3}{2}\left(x_2^2-2x_2x_3+x_3^2\right)$$

$$=2\left(x_1-\frac{1}{2}x_2-\frac{1}{2}x_3\right)^2+\frac{3}{2}(x_2-x_3)^2.$$

令

$$\begin{cases}y_1=x_1-\dfrac{1}{2}x_2-\dfrac{1}{2}x_3,\\[2pt]y_2=x_2-x_3,\\[2pt]y_3=x_3,\end{cases}$$

则标准形为 $f=2y_1^2+\dfrac{3}{2}y_2^2$．

【注】① 下列做法是错误的：令 $\begin{cases}y_1=x_1-x_2,\\y_2=x_2-x_3,\\y_3=x_3-x_1,\end{cases}$ 则标准形为 $f=y_1^2+y_2^2+y_3^2$．错误原因是矩阵 $\begin{pmatrix}1&-1&0\\0&1&-1\\-1&0&1\end{pmatrix}$ 是**不可逆**的，线性变换要求可逆．由于二次型的秩为 $2$，所以标准形中没有 $y_3$ 项．

② 此题也可将平方项展开，写出二次型 $f$ 的矩阵 $\boldsymbol{A}$，求 $\boldsymbol{A}$ 的特征值得标准形，注意标准形不唯一．

+++

#### 基础选择 (3) 设 $\boldsymbol{A}=\begin{pmatrix}1&&\\&2&\\&&3\end{pmatrix}$ 与 $\boldsymbol{B}=\begin{pmatrix}2&&\\&3&\\&&1\end{pmatrix}$ 合同，则合同变换矩阵 $\boldsymbol{P}=$（　）．

;;;
A. $\begin{pmatrix}1&0&0\\0&0&1\\1&0&0\end{pmatrix}$
B. $\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$
C. $\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}$
D. $\begin{pmatrix}0&0&1\\1&0&0\\0&0&1\end{pmatrix}$
;;;B
***
依题意，$\boldsymbol{A}$ 的二次型 $f=x_1^2+2x_2^2+3x_3^2$ 在可逆线性变换 $\boldsymbol{x}=\boldsymbol{P}\boldsymbol{y}$ 下化为

$$f=2y_1^2+3y_2^2+y_3^2,$$

故该变换为

$$\begin{cases}x_1=0y_1+0y_2+y_3,\\x_2=y_1+0y_2+0y_3,\\x_3=0y_1+y_2+0y_3,\end{cases}$$

即 $\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}\begin{pmatrix}y_1\\y_2\\y_3\end{pmatrix}$，故 $\boldsymbol{P}=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$．

【注】① $f=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}\xrightarrow[\boldsymbol{P}\text{ 可逆}]{\boldsymbol{x}=\boldsymbol{P}\boldsymbol{y}}(\boldsymbol{P}\boldsymbol{y})^{\mathrm{T}}\boldsymbol{A}\boldsymbol{P}\boldsymbol{y}=\boldsymbol{y}^{\mathrm{T}}\boldsymbol{P}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{P}\boldsymbol{y}$，$\boldsymbol{P}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，则称 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ **合同**，$\boldsymbol{x}=\boldsymbol{P}\boldsymbol{y}$ 称为合同变换．

② $\boldsymbol{A},\boldsymbol{B}$ 合同 $\iff\boldsymbol{A}$ 与 $\boldsymbol{B}$ 的正、负惯性指数分别相等，即 $p_{\boldsymbol{A}}=p_{\boldsymbol{B}}$，$q_{\boldsymbol{A}}=q_{\boldsymbol{B}}$．

+++

#### 基础选择 (4) 设 $\boldsymbol{A}$ 是 $n$ 阶方阵，将 $\boldsymbol{A}$ 的第 $i$ 列与第 $j$ 列互换，再交换第 $i$ 行与第 $j$ 行得到 $\boldsymbol{B}$，则（　）．

;;;
A. $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 等价、相似且合同
B. $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 相似、合同但不等价
C. $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 相似但不合同
D. $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 等价但不相似
;;;A
***
$\boldsymbol{A}$ 的第 $i$ 列与第 $j$ 列、第 $i$ 行与第 $j$ 行交换，相当于右乘、左乘初等矩阵，即

$$\boldsymbol{B}=\boldsymbol{E}_{i,j}\boldsymbol{A}\boldsymbol{E}_{i,j},$$

又 $\boldsymbol{E}_{i,j}^{-1}=\boldsymbol{E}_{i,j}$，$\boldsymbol{E}_{i,j}^{\mathrm{T}}=\boldsymbol{E}_{i,j}$，故

$$\boldsymbol{B}=\boldsymbol{E}_{i,j}\boldsymbol{A}\boldsymbol{E}_{i,j}=\boldsymbol{E}_{i,j}^{-1}\boldsymbol{A}\boldsymbol{E}_{i,j}=\boldsymbol{E}_{i,j}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{E}_{i,j},$$

所以 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ **等价、相似且合同**．

+++

#### 基础选择 (5) 二次型 $f(x_1,x_2,x_3)=x_1^2+4x_2^2+4x_3^2-4x_1x_2+4x_1x_3-8x_2x_3$ 的规范形为（　）．

;;;
A. $f=z_1^2$
B. $f=z_1^2-z_2^2$
C. $f=z_1^2+z_2^2+z_3^2$
D. $f=z_1^2+z_2^2-z_3^2$
;;;A
***
判定规范形，只要确定二次型的秩及正、负惯性指数，可以通过求二次型矩阵 $\boldsymbol{A}$ 的特征值来确定．

$f$ 的矩阵为 $\boldsymbol{A}=\begin{pmatrix}1&-2&2\\-2&4&-4\\2&-4&4\end{pmatrix}$，由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=\lambda^2(\lambda-9)=0$，得 $\lambda_1=9$，$\lambda_2=\lambda_3=0$，所以 $r(\boldsymbol{A})=1$，正惯性指数 $p=1$，负惯性指数 $q=0$，故 **A** 正确．

+++

#### 基础选择 (6) 设二次型 $f(x_1,x_2,x_3)=x_1^2+x_2^2+x_3^2-4x_1x_2-4x_1x_3-4x_2x_3$，则 $f(x_1,x_2,x_3)=1$ 在空间直角坐标系下表示的二次曲面为（　）．

;;;
A. 椭球面
B. 柱面
C. 单叶双曲面
D. 双叶双曲面
;;;C
***
二次型矩阵 $\boldsymbol{A}=\begin{pmatrix}1&-2&-2\\-2&1&-2\\-2&-2&1\end{pmatrix}$，由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-1&2&2\\2&\lambda-1&2\\2&2&\lambda-1\end{vmatrix}=(\lambda-3)^2(\lambda+3)=0,$$

可得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=3$，$\lambda_3=-3$，故 $f$ 经正交变换的标准形为 $3y_1^2+3y_2^2-3y_3^2$，而 $3y_1^2+3y_2^2-3y_3^2=1$ 表示**单叶双曲面**．

+++

#### 基础选择 (7) 若二次曲面 $x^2+(k+2)y^2+kz^2+2xy=5$ 表示一个椭球面，则（　）．

;;;
A. $k>0$
B. $k<0$
C. $k>-1$
D. $k<-1$
;;;A
***
$$f=x^2+(k+2)y^2+kz^2+2xy=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x},\quad \boldsymbol{x}=(x,y,z)^{\mathrm{T}}.$$

二次型的矩阵 $\boldsymbol{A}=\begin{pmatrix}1&1&0\\1&k+2&0\\0&0&k\end{pmatrix}$，$f=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=5$ 化为标准形后为椭球面，则 $r(\boldsymbol{A})=p+0=3$，即 $\boldsymbol{A}$ 的合同标准形的对角元素均为正，用配方法，得

$$x^2+(k+2)y^2+kz^2+2xy=(x+y)^2+(k+1)y^2+kz^2,$$

故 $k+1>0$ 且 $k>0$，得 $k>0$，故 **A** 正确．

+++

#### 基础填空 (1) 已知二次型 $f(x_1,x_2,x_3)=x_1^2+4x_2^2+4x_3^2+2ax_1x_2-2x_1x_3+4x_2x_3$ 正定，则 $a$ 的取值范围为 ________．
***
$-2<a<1$．

二次型 $f$ 的矩阵为 $\boldsymbol{A}=\begin{pmatrix}1&a&-1\\a&4&2\\-1&2&4\end{pmatrix}$．由已知，$\boldsymbol{A}$ 的顺序主子式分别为

$$\Delta_1=1>0,\quad \Delta_2=\begin{vmatrix}1&a\\a&4\end{vmatrix}=4-a^2>0,$$

$$\Delta_3=\begin{vmatrix}1&a&-1\\a&4&2\\-1&2&4\end{vmatrix}=-4(a-1)(a+2)>0,$$

解得 $-2<a<2$ 且 $-2<a<1$，故 $-2<a<1$．

+++

#### 基础解答 (1) 设二次型 $f(x_1,x_2,x_3)=2x_1^2+5x_2^2+5x_3^2+4x_1x_2-4x_1x_3-8x_2x_3$．

（Ⅰ）求一个正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$，将 $f$ 化为标准形；\
（Ⅱ）利用配方法，将 $f$ 化为标准形．
***
（Ⅰ）二次型 $f$ 的矩阵为 $\boldsymbol{A}=\begin{pmatrix}2&2&-2\\2&5&-4\\-2&-4&5\end{pmatrix}$．由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-2&-2&2\\-2&\lambda-5&4\\2&4&\lambda-5\end{vmatrix}=(\lambda-1)^2(\lambda-10)=0,$$

得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=1$，$\lambda_3=10$．

对 $\lambda_1=\lambda_2=1$，由 $(\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，解得 $\boldsymbol{\alpha}_1=(2,1,2)^{\mathrm{T}}$，$\boldsymbol{\alpha}_2=(-2,2,1)^{\mathrm{T}}$；对 $\lambda_3=10$，由 $(10\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，解得 $\boldsymbol{\alpha}_3=(1,2,-2)^{\mathrm{T}}$．

由 $\boldsymbol{\alpha}_1$ 与 $\boldsymbol{\alpha}_2$ 已正交，将 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 单位化，得

$$\boldsymbol{\gamma}_1=\frac{1}{3}(2,1,2)^{\mathrm{T}},\quad \boldsymbol{\gamma}_2=\frac{1}{3}(-2,2,1)^{\mathrm{T}},\quad \boldsymbol{\gamma}_3=\frac{1}{3}(1,2,-2)^{\mathrm{T}},$$

令 $\boldsymbol{Q}=(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)$，则 $\boldsymbol{Q}$ 为正交矩阵，$\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 为正交变换，标准形为

$$f=y_1^2+y_2^2+10y_3^2.$$

（Ⅱ）用配方法．

$$f=2x_1^2+5x_2^2+5x_3^2+4x_1x_2-4x_1x_3-8x_2x_3$$

$$=2x_1^2+4x_1(x_2-x_3)+5x_2^2+5x_3^2-8x_2x_3$$

$$=2\left[x_1^2+2x_1(x_2-x_3)+(x_2-x_3)^2-(x_2-x_3)^2\right]+5x_2^2+5x_3^2-8x_2x_3$$

$$=2(x_1+x_2-x_3)^2-2(x_2-x_3)^2+5x_2^2+5x_3^2-8x_2x_3$$

$$=2(x_1+x_2-x_3)^2+3x_2^2+3x_3^2-4x_2x_3$$

$$=2(x_1+x_2-x_3)^2+3\left[x_2^2-\frac{4}{3}x_2x_3+\left(\frac{2}{3}x_3\right)^2-\left(\frac{2}{3}x_3\right)^2\right]+3x_3^2$$

$$=2(x_1+x_2-x_3)^2+3\left(x_2-\frac{2}{3}x_3\right)^2+\frac{5}{3}x_3^2.$$

令 $\begin{cases}y_1=x_1+x_2-x_3,\\[2pt]y_2=x_2-\dfrac{2}{3}x_3,\\[2pt]y_3=x_3,\end{cases}$ 矩阵 $\begin{pmatrix}1&1&-1\\[2pt]0&1&-\dfrac{2}{3}\\[2pt]0&0&1\end{pmatrix}$ 可逆，则 $f=2y_1^2+3y_2^2+\dfrac{5}{3}y_3^2$．

【注】配方法："一次一个字母"，即一次配方解决一个字母且线性变换要求可逆．

+++

#### 基础解答 (2) 已知二次型 $f=2x_1^2+3x_2^2+3x_3^2+2ax_2x_3\ (a>0)$，经过正交变换化成标准形 $y_1^2+2y_2^2+5y_3^2$，求参数 $a$ 及所用的正交变换．
***
二次型 $f$ 的矩阵为 $\boldsymbol{A}=\begin{pmatrix}2&0&0\\0&3&a\\0&a&3\end{pmatrix}$，则

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=(\lambda-2)(\lambda^2-6\lambda+9-a^2).$$

由已知正交变换下的标准形为 $y_1^2+2y_2^2+5y_3^2$，故 $\boldsymbol{A}$ 的特征值为

$$\lambda_1=1,\quad \lambda_2=2,\quad \lambda_3=5,$$

所以 $|1\cdot\boldsymbol{E}-\boldsymbol{A}|=0$，即 $4-a^2=0$，得 $a=2\ (a>0)$．

对 $\lambda_1=1$，由 $(1\cdot\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_1=(0,1,-1)^{\mathrm{T}}$；\
对 $\lambda_2=2$，由 $(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_2=(1,0,0)^{\mathrm{T}}$；\
对 $\lambda_3=5$，由 $(5\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_3=(0,1,1)^{\mathrm{T}}$．

显然 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 已两两正交，单位化得

$$\boldsymbol{\gamma}_1=\frac{1}{\sqrt{2}}(0,1,-1)^{\mathrm{T}},\quad \boldsymbol{\gamma}_2=(1,0,0)^{\mathrm{T}},\quad \boldsymbol{\gamma}_3=\frac{1}{\sqrt{2}}(0,1,1)^{\mathrm{T}},$$

令 $\boldsymbol{Q}=(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)$，则 $\boldsymbol{Q}$ 为正交矩阵，$\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 为所求正交变换．

+++

#### 基础解答 (3) 证明：$n$ 阶矩阵 $\boldsymbol{A}$ 正定的充分必要条件是存在可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{A}=\boldsymbol{P}^{\mathrm{T}}\boldsymbol{P}$．
***
（**充分性**）对 $\forall\boldsymbol{x}\neq\boldsymbol{0}$，则 $\boldsymbol{P}\boldsymbol{x}\neq\boldsymbol{0}$（因 $\boldsymbol{P}$ 可逆，$\boldsymbol{P}\boldsymbol{x}=\boldsymbol{0}$ 只有零解），

$$\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{P}^{\mathrm{T}}\boldsymbol{P}\boldsymbol{x}=(\boldsymbol{P}\boldsymbol{x})^{\mathrm{T}}(\boldsymbol{P}\boldsymbol{x})>0.$$

由二次型正定的定义，知 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 是正定的，故 $\boldsymbol{A}$ 正定．

（**必要性**）由 $\boldsymbol{A}$ 正定，所以 $\boldsymbol{A}$ 的特征值 $\lambda_i>0\ (i=1,2,\cdots,n)$，且存在正交矩阵 $\boldsymbol{Q}$，使得

$$\boldsymbol{A}=\boldsymbol{Q}\boldsymbol{\Lambda}\boldsymbol{Q}^{-1}=\boldsymbol{Q}\begin{pmatrix}\lambda_1&&\\&\ddots&\\&&\lambda_n\end{pmatrix}\boldsymbol{Q}^{\mathrm{T}}=\boldsymbol{Q}\begin{pmatrix}\sqrt{\lambda_1}&&\\&\ddots&\\&&\sqrt{\lambda_n}\end{pmatrix}\begin{pmatrix}\sqrt{\lambda_1}&&\\&\ddots&\\&&\sqrt{\lambda_n}\end{pmatrix}\boldsymbol{Q}^{\mathrm{T}},$$

取 $\boldsymbol{P}=\begin{pmatrix}\sqrt{\lambda_1}&&\\&\ddots&\\&&\sqrt{\lambda_n}\end{pmatrix}\boldsymbol{Q}^{\mathrm{T}}$，则 $\boldsymbol{A}=\boldsymbol{P}^{\mathrm{T}}\boldsymbol{P}$．

【注】此题可作为判别 $\boldsymbol{A}$ 是否正定的一个结论．

+++

#### 综合选择 (1) 二次型 $f(x_1,x_2,x_3)=x_1x_2+x_2x_3$ 的正、负惯性指数分别为（　）．

;;;
A. $p=1,q=1$
B. $p=1,q=2$
C. $p=1,q=0$
D. $p=0,q=2$
;;;A
***
求正、负惯性指数，可通过标准形（规范形）或特征值得到．已知二次型 $f$ 中没有平方项，先作可逆线性变换产生平方项，再化为标准形或求其矩阵的特征值．

令 $\begin{cases}x_1=y_1+y_2,\\x_2=y_1-y_2,\\x_3=y_3,\end{cases}$ 矩阵 $\begin{pmatrix}1&1&0\\1&-1&0\\0&0&1\end{pmatrix}$ 可逆，则

$$f=(y_1+y_2)(y_1-y_2)+(y_1-y_2)y_3=y_1^2-y_2^2+y_1y_3-y_2y_3.$$

用配方法化为标准形，得

$$f=\left(y_1+\frac{1}{2}y_3\right)^2-\left(y_2+\frac{1}{2}y_3\right)^2,$$

令 $\begin{cases}z_1=y_1+\dfrac{1}{2}y_3,\\[2pt]z_2=y_2+\dfrac{1}{2}y_3,\\[2pt]z_3=y_3,\end{cases}$ 矩阵 $\begin{pmatrix}1&0&\dfrac{1}{2}\\[2pt]0&1&\dfrac{1}{2}\\[2pt]0&0&1\end{pmatrix}$ 可逆，故二次型为 $f=z_1^2-z_2^2$，所以 $p=1$，$q=1$．

+++

#### 综合选择 (2) $\boldsymbol{A}$ 是 $n$ 阶实对称矩阵，则 $\boldsymbol{A}$ 合同于矩阵 $\boldsymbol{B}$ 的充分必要条件是（　）．

① $r(\boldsymbol{A})=r(\boldsymbol{B})$，\
② $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 的正惯性指数相等，\
③ $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 均正定矩阵，\
④ $\boldsymbol{B}$ 是实对称矩阵．

;;;
A. ① 成立
B. ④ 成立
C. ①②④ 均成立
D. ③ 成立
;;;C
***
首先 ④ 是必要条件．

若 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 合同，则存在可逆矩阵 $\boldsymbol{C}$，使得 $\boldsymbol{C}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C}=\boldsymbol{B}$，故 $r(\boldsymbol{A})=r(\boldsymbol{B})$，且正、负惯性指数不变，即 $p_{\boldsymbol{A}}=p_{\boldsymbol{B}}$；反之，若 $r(\boldsymbol{A})=r(\boldsymbol{B})$，且 $p_{\boldsymbol{A}}=p_{\boldsymbol{B}}$，由于

$$p_{\boldsymbol{A}}+q_{\boldsymbol{A}}=r(\boldsymbol{A}),\quad p_{\boldsymbol{B}}+q_{\boldsymbol{B}}=r(\boldsymbol{B}),$$

故 $q_{\boldsymbol{A}}=q_{\boldsymbol{B}}$，所以 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 合同．③ 是充分条件．

【注】存在可逆矩阵 $\boldsymbol{C}$，使得 $\boldsymbol{C}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C}=\boldsymbol{B}$，称 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 合同，定义中并没有要求 $\boldsymbol{A},\boldsymbol{B}$ 是实对称矩阵，但当 $\boldsymbol{A}$ 是实对称阵时，由 $(\boldsymbol{C}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C})^{\mathrm{T}}=\boldsymbol{B}^{\mathrm{T}}$，即 $\boldsymbol{C}^{\mathrm{T}}\boldsymbol{A}^{\mathrm{T}}\boldsymbol{C}=\boldsymbol{B}^{\mathrm{T}}$，故 $\boldsymbol{C}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C}=\boldsymbol{B}^{\mathrm{T}}=\boldsymbol{B}$，说明 $\boldsymbol{B}$ 也是实对称矩阵．一般情况下，只讨论对称矩阵的正、负惯性指数．

+++

#### 综合选择 (3) 方程 $(x-y)^2+(y-z)^2+(z-x)^2=1$ 表示的曲面是（　）．

;;;
A. 椭球面
B. 单叶双曲面
C. 双叶双曲面
D. 柱面
;;;D
***
令

$$f(x,y,z)=(x-y)^2+(y-z)^2+(z-x)^2=2x^2+2y^2+2z^2-2yz-2zx-2xy,$$

则二次型的矩阵为

$$\boldsymbol{A}=\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}.$$

由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$，得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=0$，$\lambda_2=\lambda_3=3$，即 $p_{\boldsymbol{A}}=2$，$q_{\boldsymbol{A}}=0$，故 $f$ 在正交变换下的标准形为 $0\cdot y_1^2+3y_2^2+3y_3^2$，所以曲面为**柱面**．

【注】设 $f(x,y,z)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$，$\boldsymbol{x}=(x,y,z)^{\mathrm{T}}$．$\boldsymbol{A}$ 的特征值为 $\lambda_1,\lambda_2,\lambda_3$，则 $f(x,y,z)=1$ 按特征值符号有如下情形：

① 全正，为椭球面（含球面）；\
② 两正一负，为单叶双曲面；\
③ 两负一正，为双叶双曲面；\
④ 两正一零，为椭圆柱面（含圆柱面）；\
⑤ 一正一负一零，为双曲柱面；\
⑥ 一正两零，为两个平行平面．

+++

#### 综合选择 (4) 设 $n$ 元二次型 $f(x_1,x_2,\cdots,x_n)=(x_1+a_1x_2)^2+(x_2+a_2x_3)^2+\cdots+(x_n+a_nx_1)^2$，其中 $a_i\ (i=1,2,\cdots,n)$ 均为实数，若二次型正定，则（　）．

;;;
A. $1+(-1)^{n+1}a_1a_2\cdots a_n\neq 0$
B. $1+(-1)^{n+1}a_1a_2\cdots a_n=0$
C. $1-(-1)^{n+1}a_1a_2\cdots a_n\neq 0$
D. $1-(-1)^{n+1}a_1a_2\cdots a_n=0$
;;;A
***
由正定二次型的定义，可知 $f(x_1,x_2,\cdots,x_n)$ 正定的充分必要条件是对任意 $x_1,x_2,\cdots,x_n$，有 $f(x_1,x_2,\cdots,x_n)\geqslant 0$，其中当且仅当方程组 ① 只有零解时等号成立．

$$\begin{cases}x_1+a_1x_2=0,\\x_2+a_2x_3=0,\\\cdots\\x_n+a_nx_1=0.\end{cases}\qquad ①$$

方程组 ① 只有零解的充分必要条件是其系数行列式不为零，即

$$\begin{vmatrix}1&a_1&0&\cdots&0&0\\0&1&a_2&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&1&a_{n-1}\\a_n&0&0&\cdots&0&1\end{vmatrix}=1+(-1)^{n+1}a_1a_2\cdots a_n\neq 0,$$

因此，当 $1+(-1)^{n+1}a_1a_2\cdots a_n\neq 0$ 时，对任意不全为 $0$ 的 $x_1,x_2,\cdots,x_n$ 都有

$$f(x_1,x_2,\cdots,x_n)>0,$$

故正定，**A** 正确．

【注】按第 $1$ 列展开计算行列式．

+++

#### 综合填空 (1) 若 $3$ 阶实对称矩阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}=\begin{pmatrix}1&0&0\\0&0&3\\0&3&0\end{pmatrix}$ 合同，则二次型 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 的规范形为 ________．
***
$y_1^2+y_2^2-y_3^2$．

求规范形的关键是确定正、负惯性指数．由 $\boldsymbol{A},\boldsymbol{B}$ 合同，知 $p_{\boldsymbol{A}}=p_{\boldsymbol{B}}$，$q_{\boldsymbol{A}}=q_{\boldsymbol{B}}$．由

$$|\lambda\boldsymbol{E}-\boldsymbol{B}|=\begin{vmatrix}\lambda-1&0&0\\0&\lambda&-3\\0&-3&\lambda\end{vmatrix}=(\lambda-1)(\lambda^2-9)=0,$$

得 $\boldsymbol{B}$ 的特征值为 $\lambda_1=1$，$\lambda_2=3$，$\lambda_3=-3$，故 $p_{\boldsymbol{B}}=2$，$q_{\boldsymbol{B}}=1$，即有 $p_{\boldsymbol{A}}=2$，$q_{\boldsymbol{A}}=1$，所以规范形为 $y_1^2+y_2^2-y_3^2$．

+++

#### 综合填空 (2) 设 $\boldsymbol{A}$ 是 $n$ 阶矩阵，方程组 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{b}$ 有唯一解，则二次型 $\boldsymbol{x}^{\mathrm{T}}(\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A})\boldsymbol{x}$ 的正惯性指数为 ________．
***
$n$．

由已知，$\boldsymbol{A}\boldsymbol{x}=\boldsymbol{b}$ 有唯一解，故 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 只有零解．

即 $\forall\boldsymbol{x}\neq\boldsymbol{0}$，有 $\boldsymbol{A}\boldsymbol{x}\neq\boldsymbol{0}$，故 $\boldsymbol{x}^{\mathrm{T}}(\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A})\boldsymbol{x}=(\boldsymbol{A}\boldsymbol{x})^{\mathrm{T}}(\boldsymbol{A}\boldsymbol{x})>0$，所以二次型正定，于是二次型的正惯性指数为 $n$．

【注】由 $(\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A})^{\mathrm{T}}=\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}$ 知，$\boldsymbol{A}^{\mathrm{T}}\boldsymbol{A}$ 是对称矩阵．

+++

#### 综合填空 (3) 设 $\boldsymbol{A}$ 是 $3$ 阶实对称矩阵，二次型 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 经过正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 后的标准形为 $y_1^2+y_2^2-y_3^2$，则二次型 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}^{*}\boldsymbol{x}$ 的规范形为 ________．
***
$-y_1^2-y_2^2+y_3^2$．

由 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 经正交变换下的标准形，知 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=1$，$\lambda_3=-1$，且

$$|\boldsymbol{A}|=1\times 1\times(-1)=-1.$$

又 $\boldsymbol{A}^{*}$ 的特征值为

$$\frac{|\boldsymbol{A}|}{\lambda_1}=-1,\quad \frac{|\boldsymbol{A}|}{\lambda_2}=-1,\quad \frac{|\boldsymbol{A}|}{\lambda_3}=1,$$

故 $p_{\boldsymbol{A}^{*}}=1$，$q_{\boldsymbol{A}^{*}}=2$，所以 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}^{*}\boldsymbol{x}$ 的规范形为 $-y_1^2-y_2^2+y_3^2$．

【注】① $\boldsymbol{A}$ 是可逆实对称矩阵，则 $\boldsymbol{A}^{-1},\boldsymbol{A}^{*}$ 都是实对称矩阵．

② 讨论正、负惯性指数时，应掌握惯性定理：二次型 $f$ 经可逆线性变换，其正、负惯性指数不变，且 $p+q=r(f)$，其秩 $r(f)$ 也不变．

+++

#### 综合解答 (1) 设二次型 $f(x_1,x_2,x_3)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=x_1^2+ax_2^2+x_3^2+2x_1x_2-2ax_1x_3-2x_2x_3$ 的正负惯性指数都是 $1$．

（Ⅰ）求 $a$ 的值；\
（Ⅱ）求可逆线性变换 $\boldsymbol{x}=\boldsymbol{B}\boldsymbol{y}$，将 $f(x_1,x_2,x_3)$ 化为标准形．
***
（Ⅰ）二次型的矩阵为 $\boldsymbol{A}=\begin{pmatrix}1&1&-a\\1&a&-1\\-a&-1&1\end{pmatrix}$．

由已知 $p+q=2=r(\boldsymbol{A})$，故 $|\boldsymbol{A}|=-(a-1)^2(a+2)=0$，解得 $a=1$ 或 $a=-2$．当 $a=1$ 时，$r(\boldsymbol{A})=1$，不合题意，故 $a=-2$，所以

$$\boldsymbol{A}=\begin{pmatrix}1&1&2\\1&-2&-1\\2&-1&1\end{pmatrix}.$$

（Ⅱ）由（Ⅰ）知，二次型为

$$f(x_1,x_2,x_3)=x_1^2-2x_2^2+x_3^2+2x_1x_2+4x_1x_3-2x_2x_3,$$

由配方法，得

$$f(x_1,x_2,x_3)=x_1^2+2x_1(x_2+2x_3)+(x_2+2x_3)^2-(x_2+2x_3)^2-2x_2^2+x_3^2-2x_2x_3$$

$$=(x_1+x_2+2x_3)^2-3x_2^2-6x_2x_3-3x_3^2$$

$$=(x_1+x_2+2x_3)^2-3(x_2^2+2x_2x_3+x_3^2)$$

$$=(x_1+x_2+2x_3)^2-3(x_2+x_3)^2.$$

令 $\begin{cases}y_1=x_1+x_2+2x_3,\\y_2=x_2+x_3,\\y_3=x_3,\end{cases}$ 即 $\boldsymbol{y}=\boldsymbol{C}\boldsymbol{x}$，其中 $\boldsymbol{C}=\begin{pmatrix}1&1&2\\0&1&1\\0&0&1\end{pmatrix}$，且 $\boldsymbol{C}$ 可逆，故

$$\boldsymbol{x}=\boldsymbol{C}^{-1}\boldsymbol{y}=\begin{pmatrix}1&1&2\\0&1&1\\0&0&1\end{pmatrix}^{-1}\begin{pmatrix}y_1\\y_2\\y_3\end{pmatrix},$$

即 $\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\begin{pmatrix}1&-1&-1\\0&1&-1\\0&0&1\end{pmatrix}\begin{pmatrix}y_1\\y_2\\y_3\end{pmatrix}$ 为所求可逆变换，所以

$$f=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}\xrightarrow{\boldsymbol{x}=\boldsymbol{C}^{-1}\boldsymbol{y}}(\boldsymbol{C}^{-1}\boldsymbol{y})^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C}^{-1}\boldsymbol{y}=\boldsymbol{y}^{\mathrm{T}}(\boldsymbol{C}^{-1})^{\mathrm{T}}\boldsymbol{A}\boldsymbol{C}^{-1}\boldsymbol{y}.$$

令 $\boldsymbol{B}=\boldsymbol{C}^{-1}$，则 $\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{B}=\boldsymbol{\Lambda}=\begin{pmatrix}1&0&0\\0&-3&0\\0&0&0\end{pmatrix}$，标准形为 $y_1^2-3y_2^2$．

【注】用配方法求可逆线性变换（不是正交变换）是常用方法．

+++

#### 综合解答 (2) 设 $3$ 阶实对称矩阵 $\boldsymbol{A}=(a_{ij})_{3\times 3}$ 有特征值 $\lambda_1=\lambda_2=2$，且 $\sum\limits_{i=1}^{3}a_{ii}=1$，$\boldsymbol{\alpha}=(1,0,-2)^{\mathrm{T}}$ 是方程组 $\boldsymbol{A}^{*}\boldsymbol{x}=4\boldsymbol{\alpha}$ 的解向量．

（Ⅰ）求矩阵 $\boldsymbol{A}$；\
（Ⅱ）求正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$，将二次型 $f(x_1,x_2,x_3)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 化为标准形．
***
（Ⅰ）由已知 $\boldsymbol{A}^{*}\boldsymbol{\alpha}=4\boldsymbol{\alpha}$，等式两边同时左乘 $\boldsymbol{A}$，得 $\boldsymbol{A}\boldsymbol{A}^{*}\boldsymbol{\alpha}=4\boldsymbol{A}\boldsymbol{\alpha}$，即

$$|\boldsymbol{A}|\boldsymbol{\alpha}=4\boldsymbol{A}\boldsymbol{\alpha},\qquad ①$$

故 $\boldsymbol{A}\boldsymbol{\alpha}=\dfrac{|\boldsymbol{A}|}{4}\boldsymbol{\alpha}$．又

$$\sum_{i=1}^{3}a_{ii}=1=\sum_{i=1}^{3}\lambda_i=\lambda_1+\lambda_2+\lambda_3=2+2+\lambda_3,$$

得 $\lambda_3=-3$，于是有 $|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=-12$．

由 ① 式，得 $\boldsymbol{A}\boldsymbol{\alpha}=-3\boldsymbol{\alpha}$，$\lambda_3=-3$ 对应的特征向量为 $\boldsymbol{\alpha}_3=\boldsymbol{\alpha}=(1,0,-2)^{\mathrm{T}}$．

由 $\boldsymbol{A}$ 是实对称矩阵，令 $\lambda_1=\lambda_2=2$ 对应的特征向量为 $\boldsymbol{x}=(x_1,x_2,x_3)^{\mathrm{T}}$，则 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{\alpha}_3=0$，即 $x_1-2x_3=0$，解得 $\boldsymbol{\alpha}_1=(0,1,0)^{\mathrm{T}}$，$\boldsymbol{\alpha}_2=(2,0,1)^{\mathrm{T}}$．

由 $\boldsymbol{A}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=(\lambda_1\boldsymbol{\alpha}_1,\lambda_2\boldsymbol{\alpha}_2,\lambda_3\boldsymbol{\alpha}_3)$，得

$$\boldsymbol{A}=(\lambda_1\boldsymbol{\alpha}_1,\lambda_2\boldsymbol{\alpha}_2,\lambda_3\boldsymbol{\alpha}_3)(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)^{-1}=\begin{pmatrix}0&4&-3\\2&0&0\\0&2&6\end{pmatrix}\begin{pmatrix}0&2&1\\1&0&0\\0&1&-2\end{pmatrix}^{-1}=\begin{pmatrix}1&0&2\\0&2&0\\2&0&-2\end{pmatrix}.$$

（Ⅱ）由于 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 已正交，所以只需将 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 单位化，得

$$\boldsymbol{\gamma}_1=\frac{\boldsymbol{\alpha}_1}{\|\boldsymbol{\alpha}_1\|}=\begin{pmatrix}0\\1\\0\end{pmatrix},\quad \boldsymbol{\gamma}_2=\frac{\boldsymbol{\alpha}_2}{\|\boldsymbol{\alpha}_2\|}=\frac{1}{\sqrt{5}}\begin{pmatrix}2\\0\\1\end{pmatrix},\quad \boldsymbol{\gamma}_3=\frac{\boldsymbol{\alpha}_3}{\|\boldsymbol{\alpha}_3\|}=\frac{1}{\sqrt{5}}\begin{pmatrix}1\\0\\-2\end{pmatrix}.$$

令 $\boldsymbol{Q}=(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)$，为正交矩阵，$\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 为所求正交变换，标准形为 $2y_1^2+2y_2^2-3y_3^2$．

+++

#### 综合解答 (3) 设方程组 $\begin{cases}(k+3)x_1+x_2+2x_3=0,\\2kx_1+(k-1)x_2+x_3=0,\\(k-3)x_1-3x_2+kx_3=0\end{cases}$ 有非零解，且 $\boldsymbol{A}=\begin{pmatrix}3&1&2\\1&k&-2\\2&-2&9\end{pmatrix}$ 是正定矩阵．

（Ⅰ）求 $k$ 的值；\
（Ⅱ）设 $\boldsymbol{x}=(x_1,x_2,x_3)^{\mathrm{T}}$，求 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{x}=1$ 时，$\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 的最大值．
***
（Ⅰ）由已知，齐次线性方程组有非零解，故其系数行列式为零，即

$$\begin{vmatrix}k+3&1&2\\2k&k-1&1\\k-3&-3&k\end{vmatrix}=\begin{vmatrix}k&1&2\\k&k-1&1\\0&-3&k\end{vmatrix}=k(k+1)(k-3)=0,$$

解得 $k=0,-1$ 或 $3$．

又由于 $\boldsymbol{A}$ 正定，故 $a_{ii}>0$（正定的必要条件），所以 $k=3$，由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-3&-1&-2\\-1&\lambda-3&2\\-2&2&\lambda-9\end{vmatrix}=(\lambda-1)(\lambda-4)(\lambda-10),$$

可知 $\boldsymbol{A}$ 的特征值为 $\lambda_1=1$，$\lambda_2=4$，$\lambda_3=10$，全大于 $0$，故 $k=3$ 为所求．

（Ⅱ）因 $\boldsymbol{A}$ 为实对称矩阵，故存在正交矩阵 $\boldsymbol{P}$，经正交变换 $\boldsymbol{x}=\boldsymbol{P}\boldsymbol{y}$ 化二次型 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 为标准形，于是 $\boldsymbol{y}^{\mathrm{T}}\boldsymbol{y}=\boldsymbol{y}^{\mathrm{T}}\boldsymbol{P}^{\mathrm{T}}\boldsymbol{P}\boldsymbol{y}=(\boldsymbol{P}\boldsymbol{y})^{\mathrm{T}}(\boldsymbol{P}\boldsymbol{y})=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{x}=1$，所以

$$\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=y_1^2+4y_2^2+10y_3^2\leqslant 10(y_1^2+y_2^2+y_3^2)=10\times 1=10,$$

即最大值为 $10$．

+++

#### 综合解答 (4) 设 $n$ 阶实对称矩阵 $\boldsymbol{A}$ 只有两个不同的特征值 $\lambda_1=1$ 和 $\lambda_2$，且 $\boldsymbol{A}$ 属于 $\lambda_1=1$ 的特征向量仅有 $k(1,0,\cdots,0,1)^{\mathrm{T}}\ (k\neq 0)$．

（Ⅰ）求矩阵 $\boldsymbol{A}$；\
（Ⅱ）当 $\lambda_2$ 满足什么条件时，$\boldsymbol{A}$ 是正定矩阵．
***
（Ⅰ）设 $\lambda_2$ 对应的特征向量为 $\boldsymbol{x}=(x_1,x_2,\cdots,x_n)^{\mathrm{T}}$，由 $\boldsymbol{A}$ 是实对称矩阵，得 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{\alpha}_n=0$，其中 $\boldsymbol{\alpha}_n=(1,0,\cdots,0,1)^{\mathrm{T}}$，即 $x_1+x_n=0$．解此方程，得 $\lambda_2$ 对应的特征向量为

$$\boldsymbol{\alpha}_1=\begin{pmatrix}0\\1\\0\\\vdots\\0\end{pmatrix},\ \boldsymbol{\alpha}_2=\begin{pmatrix}0\\0\\1\\\vdots\\0\end{pmatrix},\ \cdots,\ \boldsymbol{\alpha}_{n-2}=\begin{pmatrix}0\\\vdots\\0\\1\\0\end{pmatrix},\ \boldsymbol{\alpha}_{n-1}=\begin{pmatrix}-1\\0\\\vdots\\0\\1\end{pmatrix},$$

显然，$\lambda_1=1$ 与 $\lambda_2$ 对应的 $n-1$ 个特征向量已两两正交，则单位化得正交矩阵

$$\boldsymbol{Q}=\begin{pmatrix}0&0&\cdots&0&-\dfrac{1}{\sqrt{2}}&\dfrac{1}{\sqrt{2}}\\[2pt]1&0&\cdots&0&0&0\\0&1&\cdots&0&0&0\\\vdots&\vdots&&\vdots&\vdots&\vdots\\0&0&\cdots&1&0&0\\0&0&\cdots&0&\dfrac{1}{\sqrt{2}}&\dfrac{1}{\sqrt{2}}\end{pmatrix},$$

故 $\boldsymbol{Q}^{-1}\boldsymbol{A}\boldsymbol{Q}=\boldsymbol{\Lambda}=\operatorname{diag}(\lambda_2,\cdots,\lambda_2,1)$，于是

$$\boldsymbol{A}=\boldsymbol{Q}\boldsymbol{\Lambda}\boldsymbol{Q}^{-1}=\boldsymbol{Q}\boldsymbol{\Lambda}\boldsymbol{Q}^{\mathrm{T}}=\begin{pmatrix}\dfrac{1}{2}(1+\lambda_2)&0&\cdots&0&\dfrac{1}{2}(1-\lambda_2)\\[2pt]0&\lambda_2&\cdots&0&0\\\vdots&\vdots&&\vdots&\vdots\\0&0&\cdots&\lambda_2&0\\[2pt]\dfrac{1}{2}(1-\lambda_2)&0&\cdots&0&\dfrac{1}{2}(1+\lambda_2)\end{pmatrix}.$$

（Ⅱ）由于 $\boldsymbol{A}$ 是实对称矩阵，所以 $\boldsymbol{A}$ 正定的充要条件是其特征值全大于 $0$，故 $\lambda_2>0$．

【注】证明矩阵是正定矩阵，应先验证其是对称矩阵．

+++

#### 综合解答 (5) 设 $\boldsymbol{A}$ 是实对称矩阵，证明：$\boldsymbol{A}$ 可逆的充要条件是存在方阵 $\boldsymbol{B}$，使得 $\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}$ 为正定矩阵．
***
（**必要性**）因 $\boldsymbol{A}$ 可逆，取 $\boldsymbol{B}=\boldsymbol{A}^{-1}$，由 $\boldsymbol{A}$ 是实对称矩阵，有

$$\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}=\boldsymbol{A}\boldsymbol{A}^{-1}+(\boldsymbol{A}^{-1})^{\mathrm{T}}\boldsymbol{A}=\boldsymbol{E}+\boldsymbol{E}=2\boldsymbol{E}.$$

显然 $\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}$ 是正定的．

（**充分性**）由已知 $\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}$ 正定，根据正定的定义，对 $\forall\boldsymbol{x}\neq\boldsymbol{0}$，有

$$\boldsymbol{x}^{\mathrm{T}}(\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A})\boldsymbol{x}>0.$$

而

$$\boldsymbol{x}^{\mathrm{T}}(\boldsymbol{A}\boldsymbol{B}+\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A})\boldsymbol{x}=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{B}\boldsymbol{x}+\boldsymbol{x}^{\mathrm{T}}\boldsymbol{B}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}(\boldsymbol{B}\boldsymbol{x})+(\boldsymbol{B}\boldsymbol{x})^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$$

$$=2\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{B}\boldsymbol{x}=2(\boldsymbol{A}\boldsymbol{x})^{\mathrm{T}}\boldsymbol{B}\boldsymbol{x},$$

即对 $\forall\boldsymbol{x}\neq\boldsymbol{0}$，有 $2(\boldsymbol{A}\boldsymbol{x})^{\mathrm{T}}\boldsymbol{B}\boldsymbol{x}>0$，故 $\boldsymbol{A}\boldsymbol{x}\neq\boldsymbol{0}$，所以 $\boldsymbol{A}$ 可逆．

+++

#### 拓展解答 (1) 设二次型 $f(x_1,x_2,\cdots,x_n)=nx_1^2+nx_2^2+\cdots+nx_n^2-(x_1+x_2+\cdots+x_n)^2$．

（Ⅰ）求二次型 $f(x_1,x_2,\cdots,x_n)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 的秩；\
（Ⅱ）求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$，并求二次型的正惯性指数．
***
（Ⅰ）

$$f(x_1,x_2,\cdots,x_n)=(n-1)x_1^2+(n-1)x_2^2+\cdots+(n-1)x_n^2-2x_1x_2-2x_1x_3-\cdots-2x_1x_n-2x_2x_3-\cdots-2x_2x_n-\cdots-2x_{n-1}x_n,$$

故二次型的矩阵为

$$\boldsymbol{A}=\begin{pmatrix}n-1&-1&-1&\cdots&-1&-1\\-1&n-1&-1&\cdots&-1&-1\\-1&-1&n-1&\cdots&-1&-1\\\vdots&\vdots&\vdots&&\vdots&\vdots\\-1&-1&-1&\cdots&n-1&-1\\-1&-1&-1&\cdots&-1&n-1\end{pmatrix},$$

注意到 $\boldsymbol{A}$ 的各行元素之和均为 $0$，利用初等变换得

$$\boldsymbol{A}\to\begin{pmatrix}n-1&-1&-1&\cdots&-1&0\\-1&n-1&-1&\cdots&-1&0\\-1&-1&n-1&\cdots&-1&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\-1&-1&-1&\cdots&n-1&0\\-1&-1&-1&\cdots&-1&0\end{pmatrix}\to\begin{pmatrix}n&0&0&\cdots&0&0\\0&n&0&\cdots&0&0\\0&0&n&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&n&0\\0&0&0&\cdots&0&0\end{pmatrix},$$

所以 $r(\boldsymbol{A})=n-1$．

（Ⅱ）由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$，解得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=\cdots=\lambda_{n-1}=n$，$\lambda_n=0$．

对 $\lambda_1=\lambda_2=\cdots=\lambda_{n-1}=n$，解 $(n\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{A}$ 的特征向量为

$$\boldsymbol{\alpha}_1=\begin{pmatrix}-1\\1\\0\\\vdots\\0\end{pmatrix},\ \boldsymbol{\alpha}_2=\begin{pmatrix}-1\\0\\1\\0\\\vdots\\0\end{pmatrix},\ \cdots,\ \boldsymbol{\alpha}_{n-1}=\begin{pmatrix}-1\\0\\\vdots\\0\\1\end{pmatrix},$$

对 $\lambda_n=0$，解 $(0\cdot\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{A}$ 的特征向量为 $\boldsymbol{\alpha}_n=(1,1,\cdots,1)^{\mathrm{T}}$．

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)$，则 $\boldsymbol{P}$ 可逆，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$．

由于 $\boldsymbol{A}$ 的特征值为

$$\lambda_1=\lambda_2=\cdots=\lambda_{n-1}=n>0,\quad \lambda_n=0,$$

故二次型的正惯性指数为 $n-1$．

【注】$\boldsymbol{A}=n\boldsymbol{E}+\begin{pmatrix}-1&-1&\cdots&-1&-1\\-1&-1&\cdots&-1&-1\\\vdots&\vdots&&\vdots&\vdots\\-1&-1&\cdots&-1&-1\end{pmatrix}\xlongequal{\text{记}}n\boldsymbol{E}+\boldsymbol{B}$，其中 $r(\boldsymbol{B})=1$．

求 $\boldsymbol{A}$ 的特征值、特征向量时，可利用秩为 $1$ 的矩阵的特征值、特征向量的结论，见《李林考研数学系列线性代数辅导讲义》．

+++

#### 拓展解答 (2) 设 $\boldsymbol{A}$ 为 $3$ 阶实对称矩阵，二次型 $f(x_1,x_2,x_3)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 在正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 下的标准形为 $-y_1^2+2y_2^2+ay_3^2$，其中 $\boldsymbol{Q}$ 的第 $1$ 列为 $\left(\dfrac{1}{\sqrt{3}},\dfrac{1}{\sqrt{3}},\dfrac{1}{\sqrt{3}}\right)^{\mathrm{T}}$，且 $|\boldsymbol{A}|=-4$．

（Ⅰ）求 $a$ 的值；\
（Ⅱ）求正交矩阵 $\boldsymbol{Q}$．
***
（Ⅰ）由二次型在正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 下的标准形为 $-y_1^2+2y_2^2+ay_3^2$，知矩阵 $\boldsymbol{A}$ 的特征值分别为 $\lambda_1=-1$，$\lambda_2=2$，$\lambda_3=a$．

又由 $|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=(-1)\times 2\times a=-4$，得 $a=2$．

（Ⅱ）由正交矩阵 $\boldsymbol{Q}$ 的第 $1$ 列为 $\left(\dfrac{1}{\sqrt{3}},\dfrac{1}{\sqrt{3}},\dfrac{1}{\sqrt{3}}\right)^{\mathrm{T}}$，可知特征值 $\lambda_1=-1$ 对应的特征向量为 $\boldsymbol{\alpha}_1=(1,1,1)^{\mathrm{T}}$．令 $\boldsymbol{\alpha}=(x_1,x_2,x_3)^{\mathrm{T}}$ 是 $\lambda_2=\lambda_3=2$ 对应的特征向量，则由

$$\boldsymbol{\alpha}_1^{\mathrm{T}}\boldsymbol{\alpha}=x_1+x_2+x_3=0,$$

解得 $\boldsymbol{\alpha}_2=(1,-1,0)^{\mathrm{T}}$，$\boldsymbol{\alpha}_3=\left(\dfrac{1}{2},\dfrac{1}{2},-1\right)^{\mathrm{T}}$ 是 $\lambda_2=\lambda_3$ 对应的特征向量，且 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 正交．

将 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 单位化，得

$$\boldsymbol{\gamma}_1=\frac{1}{\sqrt{3}}\begin{pmatrix}1\\1\\1\end{pmatrix},\quad \boldsymbol{\gamma}_2=\frac{1}{\sqrt{2}}\begin{pmatrix}1\\-1\\0\end{pmatrix},\quad \boldsymbol{\gamma}_3=\frac{1}{\sqrt{6}}\begin{pmatrix}1\\1\\-2\end{pmatrix},$$

则

$$\boldsymbol{Q}=\begin{pmatrix}\dfrac{1}{\sqrt{3}}&\dfrac{1}{\sqrt{2}}&\dfrac{1}{\sqrt{6}}\\[4pt]\dfrac{1}{\sqrt{3}}&-\dfrac{1}{\sqrt{2}}&\dfrac{1}{\sqrt{6}}\\[4pt]\dfrac{1}{\sqrt{3}}&0&-\dfrac{2}{\sqrt{6}}\end{pmatrix}$$

为所求的正交矩阵．

+++

#### 拓展解答 (3) 设 $3$ 阶实对称矩阵 $\boldsymbol{A}$ 满足 $\boldsymbol{A}^2=2\boldsymbol{A}$，已知二次型 $f(x_1,x_2,x_3)=\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}$ 经正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 化为 $\lambda y_2^2+\lambda y_3^2\ (\lambda\neq 0)$，其中 $\boldsymbol{Q}=\dfrac{1}{\sqrt{2}}\begin{pmatrix}1&0&a\\0&c&0\\b&0&1\end{pmatrix}\ (b>0,c>0)$．

（Ⅰ）求 $a,b,c$ 的值；\
（Ⅱ）求一个可逆线性变换 $\boldsymbol{x}=\boldsymbol{P}\boldsymbol{z}$ 化 $f$ 为规范形．
***
（Ⅰ）由 $\boldsymbol{Q}$ 是正交矩阵，知

$$\begin{cases}\left(\dfrac{1}{\sqrt{2}}\right)^2+\left(\dfrac{b}{\sqrt{2}}\right)^2=1,\\[4pt]\left(\dfrac{c}{\sqrt{2}}\right)^2=1,\\[4pt]\left(\dfrac{a}{\sqrt{2}}\right)^2+\left(\dfrac{1}{\sqrt{2}}\right)^2=1,\end{cases}$$

得 $\begin{cases}b=1,\\c=\sqrt{2},\\a=\pm 1.\end{cases}$ 当 $a=1$ 时，$\boldsymbol{Q}$ 的第 $1$ 列与第 $3$ 列不正交，故 $a=-1$．

综上所述，$a=-1$，$b=1$，$c=\sqrt{2}$．

（Ⅱ）由已知，$f$ 经正交变换 $\boldsymbol{x}=\boldsymbol{Q}\boldsymbol{y}$ 化为标准形 $2y_2^2+2y_3^2$．

令 $\begin{cases}z_1=y_1,\\z_2=\sqrt{2}y_2,\\z_3=\sqrt{2}y_3,\end{cases}$ 即 $\begin{pmatrix}z_1\\z_2\\z_3\end{pmatrix}=\begin{pmatrix}1&0&0\\0&\sqrt{2}&0\\0&0&\sqrt{2}\end{pmatrix}\begin{pmatrix}y_1\\y_2\\y_3\end{pmatrix}$，故

$$\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\boldsymbol{Q}\begin{pmatrix}1&0&0\\0&\sqrt{2}&0\\0&0&\sqrt{2}\end{pmatrix}^{-1}\begin{pmatrix}z_1\\z_2\\z_3\end{pmatrix}=\begin{pmatrix}\dfrac{1}{\sqrt{2}}&0&-\dfrac{1}{\sqrt{2}}\\[4pt]0&1&0\\[4pt]\dfrac{1}{\sqrt{2}}&0&\dfrac{1}{\sqrt{2}}\end{pmatrix}\begin{pmatrix}1&0&0\\[2pt]0&\dfrac{1}{\sqrt{2}}&0\\[2pt]0&0&\dfrac{1}{\sqrt{2}}\end{pmatrix}\begin{pmatrix}z_1\\z_2\\z_3\end{pmatrix}$$

$$=\begin{pmatrix}\dfrac{1}{\sqrt{2}}&0&-\dfrac{1}{2}\\[4pt]0&\dfrac{1}{\sqrt{2}}&0\\[4pt]\dfrac{1}{\sqrt{2}}&0&\dfrac{1}{2}\end{pmatrix}\begin{pmatrix}z_1\\z_2\\z_3\end{pmatrix}.$$

令 $\boldsymbol{P}=\begin{pmatrix}\dfrac{1}{\sqrt{2}}&0&-\dfrac{1}{2}\\[4pt]0&\dfrac{1}{\sqrt{2}}&0\\[4pt]\dfrac{1}{\sqrt{2}}&0&\dfrac{1}{2}\end{pmatrix}$，则 $\boldsymbol{x}=\boldsymbol{P}\boldsymbol{z}$ 为所求的一个可逆线性变换，规范形为 $z_2^2+z_3^2$．
