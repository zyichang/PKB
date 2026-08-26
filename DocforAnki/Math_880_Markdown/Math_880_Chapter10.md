---
quizify:
  format: 1
  deck: Math_880::Chapter_10
  tags: [Math, 880题, 数一, 第十章, 行列式]
---

+++

#### 基础选择 (1) 设行列式 $D=\begin{vmatrix}3&0&4&0\\2&2&2&2\\0&-7&0&0\\5&3&-2&2\end{vmatrix}$，则 $D$ 的第 $4$ 行各元素的余子式之和 $M_{41}+M_{42}+M_{43}+M_{44}=$（　）．

;;;
A. $-28$
B. $28$
C. $14$
D. $-14$
;;;A
***
设元素 $a_{ij}$ 的代数余子式为 $A_{ij}=(-1)^{i+j}M_{ij}$，则

$$M_{41}+M_{42}+M_{43}+M_{44}$$

$$=-(-1)^{4+1}M_{41}+(-1)^{4+2}M_{42}+\left[-(-1)^{4+3}\right]M_{43}+(-1)^{4+4}M_{44}$$

$$=-A_{41}+A_{42}-A_{43}+A_{44}$$

$$=\begin{vmatrix}3&0&4&0\\2&2&2&2\\0&-7&0&0\\-1&1&-1&1\end{vmatrix}=7\begin{vmatrix}3&4&0\\2&2&2\\-1&-1&1\end{vmatrix}=-28,$$

故原式 $=-28$．

【注】$D=|a_{ij}|_{n\times n}$ 中，$a_{ij}$ 的代数余子式 $A_{ij}$ 仅与 $a_{ij}$ 的**位置**有关，而与 $a_{ij}$ 的**取值**无关，即改变 $D$ 中 $a_{ij}$ 的值，$A_{ij}$ 不改变．

+++

#### 基础选择 (2) 设 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\beta}_1,\boldsymbol{\beta}_2$ 均是 $4$ 维列向量，且 $4$ 阶行列式 $|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\beta}_1)|=a$，$|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\beta}_2,\boldsymbol{\alpha}_3)|=b$，则行列式 $|(\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_1,\boldsymbol{\beta}_1+\boldsymbol{\beta}_2)|=$（　）．

;;;
A. $a+b$
B. $a-b$
C. $b-a$
D. $-(a+b)$
;;;C
***
利用行列式的性质，有

$$|(\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_1,\boldsymbol{\beta}_1+\boldsymbol{\beta}_2)|=|(\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_1,\boldsymbol{\beta}_1)|+|(\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_1,\boldsymbol{\beta}_2)|$$

$$=-|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\beta}_1)|-|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\beta}_2)|$$

$$=-a+|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\beta}_2,\boldsymbol{\alpha}_3)|=-a+b=b-a,$$

故 **C** 正确．

+++

#### 基础选择 (3) 设 $\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 均是 $4$ 维列向量，且 $|\boldsymbol{A}|=|(\boldsymbol{\beta}_1,\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=1$，$|\boldsymbol{B}|=|(\boldsymbol{\beta}_2,\boldsymbol{\alpha}_1,3\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=3$，则 $|\boldsymbol{A}+\boldsymbol{B}|=$（　）．

;;;
A. $15$
B. $16$
C. $31$
D. $32$
;;;D
***
矩阵 $\boldsymbol{A}+\boldsymbol{B}=(\boldsymbol{\beta}_1+\boldsymbol{\beta}_2,2\boldsymbol{\alpha}_1,4\boldsymbol{\alpha}_2,2\boldsymbol{\alpha}_3)$，故

$$|\boldsymbol{A}+\boldsymbol{B}|=|(\boldsymbol{\beta}_1+\boldsymbol{\beta}_2,2\boldsymbol{\alpha}_1,4\boldsymbol{\alpha}_2,2\boldsymbol{\alpha}_3)|$$

$$=16\left[|(\boldsymbol{\beta}_1,\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|+|(\boldsymbol{\beta}_2,\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|\right]$$

$$=16\left[|(\boldsymbol{\beta}_1,\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|+\frac{1}{3}|(\boldsymbol{\beta}_2,\boldsymbol{\alpha}_1,3\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|\right]$$

$$=16\times\left(1+\frac{1}{3}\times 3\right)=16\times 2=32,$$

所以 **D** 正确．

+++

#### 基础选择 (4) 设 $3$ 阶矩阵 $\boldsymbol{A}=(a_{ij})_{3\times 3}$ 满足 $\boldsymbol{A}^{\mathrm{T}}=k\boldsymbol{A}^{*}\ (k>0)$，若 $a_{11}=a_{12}=a_{13}=c>0$，则 $c=$（　）．

;;;
A. $\dfrac{\sqrt{3}}{3k}$
B. $\dfrac{\sqrt{3}k^2}{3}$
C. $\sqrt{3}k^2$
D. $\dfrac{\sqrt{3}}{k^2}$
;;;A
***
由

$$|\boldsymbol{A}^{*}|=|\boldsymbol{A}|^{3-1}=|\boldsymbol{A}|^{2},\quad |\boldsymbol{A}^{\mathrm{T}}|=|k\boldsymbol{A}^{*}|=k^{3}|\boldsymbol{A}^{*}|,\quad |\boldsymbol{A}^{\mathrm{T}}|=|\boldsymbol{A}|,$$

可知 $|\boldsymbol{A}|=k^{3}|\boldsymbol{A}|^{2}$，故

$$|\boldsymbol{A}|\left(k^{3}|\boldsymbol{A}|-1\right)=0,$$

于是有 $|\boldsymbol{A}|=0$ 或 $|\boldsymbol{A}|=\dfrac{1}{k^{3}}$．又 $\boldsymbol{A}^{\mathrm{T}}=k\boldsymbol{A}^{*}$，即 $a_{ji}=kA_{ji}$，故

$$|\boldsymbol{A}|=a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}=\frac{1}{k}\left(a_{11}^{2}+a_{12}^{2}+a_{13}^{2}\right)=\frac{3c^{2}}{k}\neq 0,$$

于是 $\dfrac{3c^{2}}{k}=\dfrac{1}{k^{3}}$，$c=\sqrt{\dfrac{1}{3k^{2}}}=\dfrac{\sqrt{3}}{3k}$，故 **A** 正确．

【注】设 $\boldsymbol{A}$ 是 $n$ 阶方阵，则 $|\boldsymbol{A}^{*}|=|\boldsymbol{A}|^{n-1}$．

+++

#### 基础填空 (1) $\begin{vmatrix}k&0&-1&1\\0&k&1&-1\\-1&1&k&0\\1&-1&0&k\end{vmatrix}=$ ________．
***
$k^{2}(k^{2}-4)$．

将第 $2,3,4$ 行加到第 $1$ 行，提取 $k$，再用行列式性质，有

$$\begin{vmatrix}k&0&-1&1\\0&k&1&-1\\-1&1&k&0\\1&-1&0&k\end{vmatrix}=k\begin{vmatrix}1&1&1&1\\0&k&1&-1\\-1&1&k&0\\1&-1&0&k\end{vmatrix}=k\begin{vmatrix}1&1&1&1\\0&k&1&-1\\0&2&k+1&1\\0&0&k&k\end{vmatrix}$$

$$=k^{2}\begin{vmatrix}k&1&-1\\2&k+1&1\\0&1&1\end{vmatrix}=k^{2}\begin{vmatrix}k&2&-1\\2&k&1\\0&0&1\end{vmatrix}=k^{2}(k^{2}-4).$$

+++

#### 基础填空 (2) 若 $\begin{vmatrix}\lambda-a&-1&-1\\-1&\lambda-a&1\\-1&1&\lambda-a\end{vmatrix}=0$，则 $\lambda=$ ________．
***
$a+1$ 或 $a-2$．

原式

$$=\begin{vmatrix}\lambda-a-1&\lambda-a-1&0\\-1&\lambda-a&1\\-1&1&\lambda-a\end{vmatrix}=\begin{vmatrix}\lambda-a-1&0&0\\-1&\lambda-a+1&1\\-1&2&\lambda-a\end{vmatrix}$$

$$=(\lambda-a-1)\left[(\lambda-a)^{2}+(\lambda-a)-2\right]=0,$$

得 $\lambda=a+1$ 或 $\lambda=a-2$．

+++

#### 基础填空 (3) $D_4=\begin{vmatrix}1&0&0&1\\0&2&0&1\\0&0&3&1\\1&1&1&4\end{vmatrix}=$ ________．
***
$13$．

箭形（爪形）行列式，利用主对角线元素将第 $4$ 行前 $3$ 个元素化为零．

$$D_4=\begin{vmatrix}1&0&0&1\\0&2&0&1\\0&0&3&1\\1&1&1&4\end{vmatrix}=\begin{vmatrix}1&0&0&1\\0&2&0&1\\0&0&3&1\\0&0&0&4-1-\dfrac{1}{2}-\dfrac{1}{3}\end{vmatrix}$$

$$=1\times 2\times 3\times\left(4-1-\frac{1}{2}-\frac{1}{3}\right)=13.$$

+++

#### 基础填空 (4) 行列式 $D_4=\begin{vmatrix}0&1&2&0\\1&0&0&2\\0&3&4&0\\3&0&0&4\end{vmatrix}=$ ________．
***
$-4$．

数字型行列式，每行（列）有 $2$ 个元素为 $0$，可以直接按一行（一列）展开计算；考虑到元素有规律，可以利用行列式的性质，交换第 $1,4$ 行，再交换第 $2,4$ 列，得

$$D_4=-\begin{vmatrix}3&0&0&4\\1&0&0&2\\0&3&4&0\\0&1&2&0\end{vmatrix}=\begin{vmatrix}3&4&0&0\\1&2&0&0\\0&0&4&3\\0&0&2&1\end{vmatrix}=\begin{vmatrix}3&4\\1&2\end{vmatrix}\begin{vmatrix}4&3\\2&1\end{vmatrix}=-4.$$

+++

#### 基础填空 (5) 行列式 $D_4=\begin{vmatrix}a&-1&0&0\\0&a&-1&0\\0&0&a&-1\\4&3&2&a+1\end{vmatrix}=$ ________．
***
$a^{4}+a^{3}+2a^{2}+3a+4$．

按第 $1$ 列展开．

$$D_4=a\begin{vmatrix}a&-1&0\\0&a&-1\\3&2&a+1\end{vmatrix}+4\cdot(-1)^{4+1}\begin{vmatrix}-1&0&0\\a&-1&0\\0&a&-1\end{vmatrix}$$

$$=a\left[a\begin{vmatrix}a&-1\\2&a+1\end{vmatrix}+3\cdot(-1)^{3+1}\begin{vmatrix}-1&0\\a&-1\end{vmatrix}\right]+4$$

$$=a^{4}+a^{3}+2a^{2}+3a+4.$$

+++

#### 基础填空 (6) 设 $f(x)=\begin{vmatrix}x&-2x&1&2\\1&x&1&-1\\3&2&3x&1\\1&1&1&x\end{vmatrix}$，则 $x^{3}$ 的系数为 ________．
***
$6$．

若按第 $1$ 行展开，只有 $-2x$ 乘以其代数余子式会出现 $x^{3}$ 项，故只要求出这一项即可．

$$(-2x)\cdot(-1)^{1+2}\begin{vmatrix}1&1&-1\\3&3x&1\\1&1&x\end{vmatrix}=2x\begin{vmatrix}1&0&-1\\3&3x-3&1\\1&0&x\end{vmatrix}=2x(3x-3)(x+1)$$

$$=6x^{3}-6x,$$

故 $x^{3}$ 的系数为 $6$．

+++

#### 基础填空 (7) 设 $\boldsymbol{A}$ 是 $n$ 阶方阵，且 $\boldsymbol{A}\boldsymbol{A}^{\mathrm{T}}=\boldsymbol{E}$，$|\boldsymbol{A}|<0$，则 $|\boldsymbol{A}+\boldsymbol{E}|=$ ________．
***
$0$．

将 $\boldsymbol{A}+\boldsymbol{E}$ 变成矩阵乘积的形式，

$$|\boldsymbol{A}+\boldsymbol{E}|=|\boldsymbol{A}+\boldsymbol{A}\boldsymbol{A}^{\mathrm{T}}|=|\boldsymbol{A}(\boldsymbol{E}+\boldsymbol{A}^{\mathrm{T}})|=|\boldsymbol{A}||\boldsymbol{E}+\boldsymbol{A}^{\mathrm{T}}|$$

$$=|\boldsymbol{A}||\boldsymbol{E}^{\mathrm{T}}+\boldsymbol{A}^{\mathrm{T}}|=|\boldsymbol{A}||(\boldsymbol{E}+\boldsymbol{A})^{\mathrm{T}}|=|\boldsymbol{A}||\boldsymbol{E}+\boldsymbol{A}|,$$

故 $(1-|\boldsymbol{A}|)|\boldsymbol{A}+\boldsymbol{E}|=0$，由 $|\boldsymbol{A}|<0$，知 $1-|\boldsymbol{A}|>0$，所以 $|\boldsymbol{A}+\boldsymbol{E}|=0$．

+++

#### 基础填空 (8) 设 $\boldsymbol{A}$ 是 $n$ 阶方阵，$\boldsymbol{E}$ 是 $n$ 阶单位矩阵，且 $\boldsymbol{A}^{2}=\boldsymbol{A}$，$\boldsymbol{A}\neq\boldsymbol{E}$，则 $|\boldsymbol{A}|=$ ________．
***
$0$．

**解法 1** 利用矩阵的秩．

由 $\boldsymbol{A}^{2}=\boldsymbol{A}$，可知 $\boldsymbol{A}(\boldsymbol{A}-\boldsymbol{E})=\boldsymbol{O}$，故

$$r(\boldsymbol{A})+r(\boldsymbol{A}-\boldsymbol{E})\leqslant n.$$

又 $\boldsymbol{A}-\boldsymbol{E}\neq\boldsymbol{O}$，知 $r(\boldsymbol{A}-\boldsymbol{E})\geqslant 1$，从而 $r(\boldsymbol{A})<n$，于是 $|\boldsymbol{A}|=0$．

**解法 2** 利用齐次线性方程组．

由 $\boldsymbol{A}(\boldsymbol{A}-\boldsymbol{E})=\boldsymbol{O}$，知 $\boldsymbol{A}-\boldsymbol{E}$ 的列向量组是 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 的解．又 $\boldsymbol{A}-\boldsymbol{E}\neq\boldsymbol{O}$，知 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 有非零解，故 $|\boldsymbol{A}|=0$．

【注】结论：设 $\boldsymbol{A},\boldsymbol{B}$ 均为 $n$ 阶方阵，且 $\boldsymbol{A}\boldsymbol{B}=\boldsymbol{O}$，则 ① $r(\boldsymbol{A})+r(\boldsymbol{B})\leqslant n$；② $\boldsymbol{B}$ 的列向量组是 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 的解．

+++

#### 基础填空 (9) 设 $\boldsymbol{A},\boldsymbol{B}$ 均为 $n$ 阶方阵，且 $|\boldsymbol{A}|=|\boldsymbol{B}|=|\boldsymbol{A}^{-1}+\boldsymbol{B}|=2$，则 $|\boldsymbol{A}+\boldsymbol{B}^{-1}|=$ ________．
***
$2$．

$$|\boldsymbol{A}+\boldsymbol{B}^{-1}|=|\boldsymbol{E}\boldsymbol{A}+\boldsymbol{B}^{-1}|=|\boldsymbol{B}^{-1}\boldsymbol{B}\boldsymbol{A}+\boldsymbol{B}^{-1}|$$

$$=|\boldsymbol{B}^{-1}||\boldsymbol{B}\boldsymbol{A}+\boldsymbol{E}|=|\boldsymbol{B}^{-1}||\boldsymbol{B}\boldsymbol{A}+\boldsymbol{A}^{-1}\boldsymbol{A}|$$

$$=|\boldsymbol{B}^{-1}||\boldsymbol{B}+\boldsymbol{A}^{-1}||\boldsymbol{A}|=\frac{1}{2}\times 2\times 2=2.$$

【注】求行列式 $|\boldsymbol{A}\pm\boldsymbol{B}|$，利用 $\boldsymbol{E}$ 作恒等变形化为矩阵积的行列式．

+++

#### 基础填空 (10) 设 $|\boldsymbol{A}|=2$，$|\boldsymbol{B}|=-2$，其中 $\boldsymbol{A},\boldsymbol{B}$ 均为 $n$ 阶方阵，则 $|\boldsymbol{A}^{-1}\boldsymbol{B}^{*}-\boldsymbol{A}^{*}\boldsymbol{B}^{-1}|=$ ________．
***
$(-4)^{n-1}$．

因为 $\boldsymbol{A}^{*}=|\boldsymbol{A}|\boldsymbol{A}^{-1}=2\boldsymbol{A}^{-1}$，$\boldsymbol{B}^{*}=|\boldsymbol{B}|\boldsymbol{B}^{-1}=-2\boldsymbol{B}^{-1}$，所以

$$|\boldsymbol{A}^{-1}\boldsymbol{B}^{*}-\boldsymbol{A}^{*}\boldsymbol{B}^{-1}|=|\boldsymbol{A}^{-1}\cdot(-2\boldsymbol{B}^{-1})-2\boldsymbol{A}^{-1}\boldsymbol{B}^{-1}|$$

$$=|-4\boldsymbol{A}^{-1}\boldsymbol{B}^{-1}|=(-4)^{n}|\boldsymbol{A}|^{-1}\cdot|\boldsymbol{B}|^{-1}$$

$$=(-4)^{n}\cdot\frac{1}{2}\cdot\left(-\frac{1}{2}\right)=(-4)^{n-1}.$$

+++

#### 基础填空 (11) 设 $3$ 阶方阵 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，$\boldsymbol{B}=(3\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2,3\boldsymbol{\alpha}_2-2\boldsymbol{\alpha}_1,2\boldsymbol{\alpha}_3-\boldsymbol{\alpha}_1-2\boldsymbol{\alpha}_2)$，且 $|\boldsymbol{B}|=14$，则 $|\boldsymbol{A}|=$ ________．
***
$1$．

由 $\boldsymbol{B}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}3&-2&-1\\-1&3&-2\\0&0&2\end{pmatrix}$，知

$$|\boldsymbol{B}|=|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|\begin{vmatrix}3&-2&-1\\-1&3&-2\\0&0&2\end{vmatrix}=|\boldsymbol{A}|\cdot 14=14,$$

故 $|\boldsymbol{A}|=1$．

+++

#### 基础填空 (12) 设 $\boldsymbol{A}=(a_{ij})_{n\times n}$ 为 $n$ 阶方阵，$|\boldsymbol{A}|=1$，且 $\boldsymbol{A}$ 的每列元素之和均为 $k\ (k\neq 0)$，则 $\boldsymbol{A}$ 的代数余子式之和 $A_{11}+A_{12}+\cdots+A_{1n}=$ ________．
***
$\dfrac{1}{k}$．

依题意，由 $\boldsymbol{A}\cdot\boldsymbol{A}^{*}=|\boldsymbol{A}|\boldsymbol{E}$，可知

$$|\boldsymbol{A}|=\begin{vmatrix}k&k&\cdots&k\\a_{21}&a_{22}&\cdots&a_{2n}\\\vdots&\vdots&&\vdots\\a_{n1}&a_{n2}&\cdots&a_{nn}\end{vmatrix}=k\begin{vmatrix}1&1&\cdots&1\\a_{21}&a_{22}&\cdots&a_{2n}\\\vdots&\vdots&&\vdots\\a_{n1}&a_{n2}&\cdots&a_{nn}\end{vmatrix}$$

按第一行展开，得 $k(A_{11}+A_{12}+\cdots+A_{1n})=1$，故

$$A_{11}+A_{12}+\cdots+A_{1n}=\frac{1}{k}.$$

+++

#### 基础解答 (1) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}b&a&a&\cdots&a\\a&b&a&\cdots&a\\\vdots&\vdots&\vdots&&\vdots\\a&a&a&\cdots&b\end{vmatrix}$．
***
**解法 1** $D_n$ 的各列元素之和相等，用行加法．

$$D_n=\begin{vmatrix}b+(n-1)a&b+(n-1)a&b+(n-1)a&\cdots&b+(n-1)a\\a&b&a&\cdots&a\\\vdots&\vdots&\vdots&&\vdots\\a&a&a&\cdots&b\end{vmatrix}$$

$$=\left[b+(n-1)a\right]\begin{vmatrix}1&1&1&\cdots&1\\a&b&a&\cdots&a\\\vdots&\vdots&\vdots&&\vdots\\a&a&a&\cdots&b\end{vmatrix}$$

$$=\left[b+(n-1)a\right]\begin{vmatrix}1&1&1&\cdots&1\\0&b-a&0&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\0&0&0&\cdots&b-a\end{vmatrix}$$

$$=\left[b+(n-1)a\right](b-a)^{n-1}.$$

**解法 2** $D_n$ 除主对角线上元素以外，其余列元素均相同，可用加边法．

$$D_n=D_{n+1}=\begin{vmatrix}1&a&a&\cdots&a\\0&b&a&\cdots&a\\0&a&b&\cdots&a\\\vdots&\vdots&\vdots&&\vdots\\0&a&a&\cdots&b\end{vmatrix}=\begin{vmatrix}1&a&a&\cdots&a\\-1&b-a&0&\cdots&0\\-1&0&b-a&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\-1&0&0&\cdots&b-a\end{vmatrix},$$

为箭形行列式，故 $D_n=(b-a)^{n-1}\cdot\left[b+(n-1)a\right]$．

【注】当 $\lambda_1,\lambda_2,\cdots,\lambda_n$ 均不为零时，箭形行列式

$$D_{n+1}=\begin{vmatrix}\lambda_0&a_1&a_2&\cdots&a_n\\b_1&\lambda_1&0&\cdots&0\\b_2&0&\lambda_2&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\b_n&0&0&\cdots&\lambda_n\end{vmatrix}=\left(\lambda_0-\sum_{i=1}^{n}\frac{b_ia_i}{\lambda_i}\right)\lambda_1\lambda_2\cdots\lambda_n.$$

本结论见《李林考研数学系列线性代数辅导讲义》第一章．

+++

#### 基础解答 (2) 证明：$D_n=\begin{vmatrix}x&-1&0&\cdots&0&0\\0&x&-1&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&x&-1\\a_n&a_{n-1}&a_{n-2}&\cdots&a_2&x+a_1\end{vmatrix}=x^{n}+\sum_{i=1}^{n}a_ix^{n-i}$．
***
**证法 1** 用数学归纳法．

当 $n=1$ 时，$D_1=x+a_1$；当 $n=2$ 时，

$$D_2=\begin{vmatrix}x&-1\\a_2&a_1+x\end{vmatrix}=x^{2}+a_1x+a_2,$$

结论成立．

假设当 $n=k-1$ 时，结论成立，有

$$D_{k-1}=x^{k-1}+a_1x^{(k-1)-1}+a_2x^{(k-1)-2}+\cdots+a_{k-2}x+a_{k-1},$$

则当 $n=k$ 时，将 $D_k$ 按第 $1$ 列展开，得

$$D_k=xD_{k-1}+a_k=x^{k}+a_1x^{k-1}+\cdots+a_{k-2}x^{2}+a_{k-1}x+a_k,$$

故对任意正整数 $n$，有 $D_n=x^{n}+a_1x^{n-1}+\cdots+a_{n-1}x+a_n$，结论成立．

**证法 2** 用递推法，将 $D_n$ 按第 $1$ 列展开，得

$$D_n=xD_{n-1}+(-1)^{n+1}a_n\cdot(-1)^{n-1}=xD_{n-1}+a_n,\qquad ①$$

故

$$D_{n-1}=xD_{n-2}+a_{n-1},\cdots,D_3=xD_2+a_3,\ D_2=xD_1+a_2=x^{2}+a_1x+a_2,$$

将其依次代入 ① 式，得 $D_n=x^{n}+a_1x^{n-1}+\cdots+a_{n-1}x+a_n$．

【注】此题也可对第 $n$ 行展开进行计算．

+++

#### 基础解答 (3) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}2&-1&0&\cdots&0&0\\-1&2&-1&\cdots&0&0\\0&-1&2&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&2&-1\\0&0&0&\cdots&-1&2\end{vmatrix}$．
***
$D_n$ 为三对角行列式，用递推法，将 $D_n$ 按第 $1$ 行展开．

$$D_n=2D_{n-1}+(-1)\times(-1)^{1+2}\begin{vmatrix}-1&-1&0&\cdots&0&0\\0&2&-1&\cdots&0&0\\0&-1&2&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&2&-1\\0&0&0&\cdots&-1&2\end{vmatrix}$$

$$=2D_{n-1}-D_{n-2},$$

即

$$D_n-D_{n-1}=D_{n-1}-D_{n-2}=D_{n-2}-D_{n-3}=\cdots=D_2-D_1=\begin{vmatrix}2&-1\\-1&2\end{vmatrix}-2=1,$$

故

$$D_n=D_{n-1}+1=(D_{n-2}+1)+1=D_{n-2}+2=\cdots=D_1+(n-1)=2+(n-1)=n+1.$$

+++

#### 基础解答 (4) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}a_1&b_1&0&\cdots&0&0\\0&a_2&b_2&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&a_{n-1}&b_{n-1}\\b_n&0&0&\cdots&0&a_n\end{vmatrix}+\begin{vmatrix}a_1&0&0&\cdots&0&b_n\\b_1&a_2&0&\cdots&0&0\\0&b_2&a_3&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&a_{n-1}&0\\0&0&0&\cdots&b_{n-1}&a_n\end{vmatrix}$，其中 $a_i,b_i$ 均不为 $0$．
***
记 $D_n=D_1+D_2$．$D_1$ 按第 $1$ 列展开，得

$$D_1=a_1\begin{vmatrix}a_2&b_2&0&\cdots&0&0\\0&a_3&b_3&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&a_{n-1}&b_{n-1}\\0&0&0&\cdots&0&a_n\end{vmatrix}+(-1)^{n+1}b_n\begin{vmatrix}b_1&0&0&\cdots&0&0\\a_2&b_2&0&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&b_{n-2}&0\\0&0&0&\cdots&a_{n-1}&b_{n-1}\end{vmatrix}$$

$$=a_1a_2\cdots a_n+(-1)^{n+1}b_1b_2\cdots b_n.$$

$D_2$ 是 $D_1$ 的转置行列式，故 $D_2=D_1=a_1a_2\cdots a_n+(-1)^{n+1}b_1b_2\cdots b_n$，故

$$D_n=2a_1a_2\cdots a_n+2(-1)^{n+1}b_1b_2\cdots b_n.$$

+++

#### 综合选择 (1) 设 $\boldsymbol{A}$ 是 $3$ 阶可逆矩阵，$\boldsymbol{A}^{-1}$ 的特征值为 $3,2,1$，则 $|\boldsymbol{A}|$ 的代数余子式之和 $A_{11}+A_{22}+A_{33}=$（　）．

;;;
A. $\dfrac{1}{6}$
B. $\dfrac{1}{3}$
C. $\dfrac{1}{2}$
D. $1$
;;;D
***
因为伴随矩阵 $\boldsymbol{A}^{*}$ 的主对角线元素为 $A_{11},A_{22},A_{33}$，所以 $A_{11}+A_{22}+A_{33}$ 的值等于 $\boldsymbol{A}^{*}$ 的 $3$ 个特征值之和，故只需求 $\boldsymbol{A}^{*}$ 的 $3$ 个特征值．

由 $\boldsymbol{A}^{-1}$ 的特征值为 $3,2,1$，可知 $\boldsymbol{A}$ 的特征值为 $\dfrac{1}{3},\dfrac{1}{2},1$，则

$$|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=\frac{1}{3}\times\frac{1}{2}\times 1=\frac{1}{6},$$

故 $\boldsymbol{A}^{*}$ 的 $3$ 个特征值分别为 $\dfrac{|\boldsymbol{A}|}{\lambda_1}=\dfrac{1}{2}$，$\dfrac{|\boldsymbol{A}|}{\lambda_2}=\dfrac{1}{3}$，$\dfrac{|\boldsymbol{A}|}{\lambda_3}=\dfrac{1}{6}$，所以

$$A_{11}+A_{22}+A_{33}=\frac{1}{2}+\frac{1}{3}+\frac{1}{6}=1.$$

【注】结论：设 $\lambda_1,\lambda_2,\cdots,\lambda_n$ 为矩阵 $\boldsymbol{A}$ 的特征值，则\
① $|\boldsymbol{A}|=\lambda_1\lambda_2\cdots\lambda_n$；\
② $a_{11}+a_{22}+\cdots+a_{nn}=\lambda_1+\lambda_2+\cdots+\lambda_n$；\
③ $\boldsymbol{A}^{-1}$ 的特征值为 $\dfrac{1}{\lambda_1},\dfrac{1}{\lambda_2},\cdots,\dfrac{1}{\lambda_n}\ (\lambda_i\neq 0,i=1,2,\cdots,n)$；\
④ $\boldsymbol{A}^{*}$ 的特征值为 $\dfrac{|\boldsymbol{A}|}{\lambda_1},\dfrac{|\boldsymbol{A}|}{\lambda_2},\cdots,\dfrac{|\boldsymbol{A}|}{\lambda_n}\ (\lambda_i\neq 0,i=1,2,\cdots,n)$．

（见《李林考研数学系列线性代数辅导讲义》第五章）

+++

#### 综合选择 (2) $|\boldsymbol{A}|=\begin{vmatrix}0&0&0&1\\1&0&0&0\\0&1&0&0\\0&0&1&0\end{vmatrix}$ 的所有代数余子式 $A_{ij}$ 之和 $\displaystyle\sum_{i=1}^{4}\sum_{j=1}^{4}A_{ij}=$（　）．

;;;
A. $4$
B. $-4$
C. $1$
D. $-1$
;;;B
***
求 $\displaystyle\sum_{i=1}^{4}\sum_{j=1}^{4}A_{ij}$，只要求 $\boldsymbol{A}^{*}=(A_{ji})_{4\times 4}$，由 $\boldsymbol{A}^{*}=|\boldsymbol{A}|\boldsymbol{A}^{-1}$，可知先求 $|\boldsymbol{A}|$ 和 $\boldsymbol{A}^{-1}$．

由分块矩阵求逆，得

$$\boldsymbol{A}^{-1}=\begin{pmatrix}0&0&0&1\\1&0&0&0\\0&1&0&0\\0&0&1&0\end{pmatrix}^{-1}=\begin{pmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\1&0&0&0\end{pmatrix}.$$

又 $|\boldsymbol{A}|=(-1)^{4+1}=-1$（按第 $1$ 行展开），故

$$\boldsymbol{A}^{*}=|\boldsymbol{A}|\boldsymbol{A}^{-1}=-\boldsymbol{A}^{-1}=\begin{pmatrix}0&-1&0&0\\0&0&-1&0\\0&0&0&-1\\-1&0&0&0\end{pmatrix}=\begin{pmatrix}A_{11}&A_{21}&A_{31}&A_{41}\\A_{12}&A_{22}&A_{32}&A_{42}\\A_{13}&A_{23}&A_{33}&A_{43}\\A_{14}&A_{24}&A_{34}&A_{44}\end{pmatrix},$$

所以

$$\sum_{i=1}^{4}\sum_{j=1}^{4}A_{ij}=(-1)+(-1)+(-1)+(-1)=-4.$$

+++

#### 综合选择 (3) 设 $\boldsymbol{A}$ 是 $3$ 阶方阵，$\boldsymbol{A}^{*}$ 是 $\boldsymbol{A}$ 的伴随矩阵，$|\boldsymbol{A}|=\dfrac{1}{2}$，则 $|(2\boldsymbol{A})^{-1}-2\boldsymbol{A}^{*}|=$（　）．

;;;
A. $\dfrac{1}{2}$
B. $-\dfrac{1}{2}$
C. $-\dfrac{1}{4}$
D. $\dfrac{1}{4}$
;;;C
***
**解法 1** 由 $\boldsymbol{A}^{*}=|\boldsymbol{A}|\boldsymbol{A}^{-1}=\dfrac{1}{2}\boldsymbol{A}^{-1}$，则

$$|(2\boldsymbol{A})^{-1}-2\boldsymbol{A}^{*}|=\left|\frac{1}{2}\boldsymbol{A}^{-1}-2\cdot\frac{1}{2}\boldsymbol{A}^{-1}\right|=\left|\frac{1}{2}\boldsymbol{A}^{-1}-\boldsymbol{A}^{-1}\right|$$

$$=\left|-\frac{1}{2}\boldsymbol{A}^{-1}\right|=\left(-\frac{1}{2}\right)^{3}|\boldsymbol{A}^{-1}|$$

$$=-\frac{1}{8}|\boldsymbol{A}|^{-1}=-\frac{1}{8}\times\left(\frac{1}{2}\right)^{-1}=-\frac{1}{4}.$$

**解法 2** 由 $\boldsymbol{A}^{-1}=|\boldsymbol{A}|^{-1}\boldsymbol{A}^{*}=2\boldsymbol{A}^{*}$，则

$$|(2\boldsymbol{A})^{-1}-2\boldsymbol{A}^{*}|=\left|\frac{1}{2}\cdot 2\boldsymbol{A}^{*}-2\boldsymbol{A}^{*}\right|$$

$$=|\boldsymbol{A}^{*}-2\boldsymbol{A}^{*}|=|-\boldsymbol{A}^{*}|=(-1)^{3}|\boldsymbol{A}^{*}|$$

$$=-|\boldsymbol{A}|^{3-1}=-\left(\frac{1}{2}\right)^{2}=-\frac{1}{4}.$$

+++

#### 综合填空 (1) 设 $\boldsymbol{A},\boldsymbol{B}$ 均为 $n$ 阶方阵，$|\boldsymbol{A}|=6$，$|\boldsymbol{B}|=1$，$\boldsymbol{C}=\begin{pmatrix}\boldsymbol{A}&3\boldsymbol{A}^{*}\\\left(\dfrac{\boldsymbol{B}}{2}\right)^{-1}&\boldsymbol{O}\end{pmatrix}$，则 $|\boldsymbol{C}|=$ ________．
***
$(-1)^{n}\cdot 6^{2n-1}$．

$$|\boldsymbol{C}|=\begin{vmatrix}\boldsymbol{A}&3\boldsymbol{A}^{*}\\\left(\dfrac{\boldsymbol{B}}{2}\right)^{-1}&\boldsymbol{O}\end{vmatrix}=(-1)^{n\times n}\left|\left(\frac{\boldsymbol{B}}{2}\right)^{-1}\right||3\boldsymbol{A}^{*}|,$$

而

$$\left|\left(\frac{\boldsymbol{B}}{2}\right)^{-1}\right|=|2\boldsymbol{B}^{-1}|=2^{n}|\boldsymbol{B}|^{-1}=2^{n},$$

$$|3\boldsymbol{A}^{*}|=3^{n}|\boldsymbol{A}^{*}|=3^{n}\cdot|\boldsymbol{A}|^{n-1}=3^{n}\cdot 6^{n-1},$$

故

$$|\boldsymbol{C}|=(-1)^{n^{2}}2^{n}\cdot 3^{n}\cdot 6^{n-1}=(-1)^{n^{2}}\cdot 6^{2n-1}=(-1)^{n}\cdot 6^{2n-1}.$$

+++

#### 综合填空 (2) 设 $\boldsymbol{A}$ 是 $m\times n$ 矩阵，$\boldsymbol{B}$ 是 $n\times m$ 矩阵，当 $m>n$ 时，$|\boldsymbol{A}\boldsymbol{B}|=$ ________．
***
$0$．

由已知，$\boldsymbol{A}\boldsymbol{B}$ 是 $m$ 阶方阵．由

$$r(\boldsymbol{A}\boldsymbol{B})\leqslant r(\boldsymbol{B})\leqslant\min\{m,n\},$$

故当 $m>n$ 时，有 $r(\boldsymbol{A}\boldsymbol{B})\leqslant n<m$，故 $|\boldsymbol{A}\boldsymbol{B}|=0$．

+++

#### 综合填空 (3) 设 $\boldsymbol{A},\boldsymbol{B}$ 均为 $3$ 阶方阵，满足 $\boldsymbol{A}^{2}\boldsymbol{B}-\boldsymbol{A}-\boldsymbol{B}=\boldsymbol{E}$，若 $\boldsymbol{A}=\begin{pmatrix}1&0&1\\0&2&0\\-2&0&1\end{pmatrix}$，则 $|\boldsymbol{B}|=$ ________．
***
$\dfrac{1}{2}$．

由已知 $\boldsymbol{A}^{2}\boldsymbol{B}-\boldsymbol{A}-\boldsymbol{B}=\boldsymbol{E}$，得 $(\boldsymbol{A}^{2}-\boldsymbol{E})\boldsymbol{B}=\boldsymbol{A}+\boldsymbol{E}$，即

$$(\boldsymbol{A}+\boldsymbol{E})(\boldsymbol{A}-\boldsymbol{E})\boldsymbol{B}=\boldsymbol{A}+\boldsymbol{E},$$

而 $\boldsymbol{A}+\boldsymbol{E}=\begin{pmatrix}2&0&1\\0&3&0\\-2&0&2\end{pmatrix}$，可知 $\boldsymbol{A}+\boldsymbol{E}$ 可逆，故 $(\boldsymbol{A}-\boldsymbol{E})\boldsymbol{B}=\boldsymbol{E}$，两边取行列式，得

$$|\boldsymbol{A}-\boldsymbol{E}||\boldsymbol{B}|=1.$$

而

$$|\boldsymbol{A}-\boldsymbol{E}|=\begin{vmatrix}0&0&1\\0&1&0\\-2&0&0\end{vmatrix}=2,$$

故 $|\boldsymbol{B}|=\dfrac{1}{2}$．

+++

#### 综合填空 (4) 设 $\boldsymbol{A}$ 是 $3$ 阶方阵，且满足 $|\boldsymbol{A}-\boldsymbol{E}|=|\boldsymbol{A}+2\boldsymbol{E}|=|2\boldsymbol{A}+3\boldsymbol{E}|=0$，则 $|2\boldsymbol{A}^{*}-3\boldsymbol{E}|=$ ________．
***
$126$．

先求出 $\boldsymbol{A}$ 的特征值，再求 $2\boldsymbol{A}^{*}-3\boldsymbol{E}$ 的特征值．

由 $|\boldsymbol{A}-\boldsymbol{E}|=|(-1)(\boldsymbol{E}-\boldsymbol{A})|=(-1)^{3}|\boldsymbol{E}-\boldsymbol{A}|=0$，得 $|1\cdot\boldsymbol{E}-\boldsymbol{A}|=0$，可知 $\lambda_1=1$ 是 $\boldsymbol{A}$ 的一个特征值．

同理，由 $|\boldsymbol{A}+2\boldsymbol{E}|=|2\boldsymbol{A}+3\boldsymbol{E}|=0$，得 $\boldsymbol{A}$ 的特征值 $\lambda_2=-2$，$\lambda_3=-\dfrac{3}{2}$，故

$$|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=3\neq 0\quad(\boldsymbol{A}\ \text{可逆}),$$

所以 $\boldsymbol{A}^{*}$ 的特征值分别为

$$\frac{|\boldsymbol{A}|}{\lambda_1}=\frac{3}{1}=3,\quad \frac{|\boldsymbol{A}|}{\lambda_2}=\frac{3}{-2}=-\frac{3}{2},\quad \frac{|\boldsymbol{A}|}{\lambda_3}=-2,$$

于是 $2\boldsymbol{A}^{*}-3\boldsymbol{E}$ 的特征值分别为

$$2\times 3-3=3,\quad 2\times\left(-\frac{3}{2}\right)-3=-6,\quad 2\times(-2)-3=-7,$$

所以 $|2\boldsymbol{A}^{*}-3\boldsymbol{E}|=3\times(-6)\times(-7)=126$．

【注】设 $\boldsymbol{A}$ 的特征值为 $\lambda$，则 $f(\boldsymbol{A})$ 的特征值为 $f(\lambda)$，其中 $f(x)$ 为多项式．

+++

#### 综合填空 (5) 设 $\boldsymbol{A}$ 是 $3$ 阶方阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，且 $\boldsymbol{A}\boldsymbol{\alpha}_1=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2$，$\boldsymbol{A}\boldsymbol{\alpha}_2=\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$，$\boldsymbol{A}\boldsymbol{\alpha}_3=\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_1$，则 $|\boldsymbol{A}|=$ ________．
***
$2$．

**解法 1** 利用行列式的性质，由 $\boldsymbol{A}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_1)$，可知

$$|\boldsymbol{A}||(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|=|(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_1)|$$

$$=2|(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_1)|$$

$$=2|(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,-\boldsymbol{\alpha}_1,-\boldsymbol{\alpha}_2)|$$

$$=2|(\boldsymbol{\alpha}_3,-\boldsymbol{\alpha}_1,-\boldsymbol{\alpha}_2)|=2|(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)|.$$

由于 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，故 $|\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3|\neq 0$，所以 $|\boldsymbol{A}|=2$．

**解法 2** 利用矩阵的乘法及相似矩阵的性质．

$$\boldsymbol{A}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_3+\boldsymbol{\alpha}_1)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}1&0&1\\1&1&0\\0&1&1\end{pmatrix}.$$

记 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，由已知，$\boldsymbol{P}$ 可逆，$\boldsymbol{B}=\begin{pmatrix}1&0&1\\1&1&0\\0&1&1\end{pmatrix}$，故 $\boldsymbol{A}\boldsymbol{P}=\boldsymbol{P}\boldsymbol{B}$，即 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，所以

$$|\boldsymbol{A}|=|\boldsymbol{B}|=\begin{vmatrix}1&0&1\\1&1&0\\0&1&1\end{vmatrix}=2.$$

+++

#### 综合解答 (1) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}b-a_1^{2}&-a_1a_2&\cdots&-a_1a_n\\-a_2a_1&b-a_2^{2}&\cdots&-a_2a_n\\\vdots&\vdots&&\vdots\\-a_na_1&-a_na_2&\cdots&b-a_n^{2}\end{vmatrix}$．
***
$D_n$ 除主对角线元素外，第 $i$ 行 $(i=1,2,\cdots)$ 元素分别是 $a_1,a_2,\cdots,a_{i-1},a_{i+1},\cdots,a_n$ 的倍数，即：$(-a_i)a_1,(-a_i)a_2,\cdots,(-a_i)a_{i-1},(-a_i)a_{i+1},\cdots,(-a_i)a_n$．

可考虑用加边法，

$$D_n=D_{n+1}=\begin{vmatrix}1&a_1&a_2&\cdots&a_n\\0&b-a_1^{2}&-a_1a_2&\cdots&-a_1a_n\\0&-a_2a_1&b-a_2^{2}&\cdots&-a_2a_n\\\vdots&\vdots&\vdots&&\vdots\\0&-a_na_1&-a_na_2&\cdots&b-a_n^{2}\end{vmatrix}=\begin{vmatrix}1&a_1&a_2&\cdots&a_n\\a_1&b&0&\cdots&0\\a_2&0&b&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\a_n&0&0&\cdots&b\end{vmatrix},$$

为箭形行列式，故

$$D_n=b^{n-1}\left(b-\sum_{i=1}^{n}a_i^{2}\right).$$

+++

#### 综合解答 (2) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}a+b_1&a&\cdots&a\\a&a+b_2&\cdots&a\\\vdots&\vdots&&\vdots\\a&a&\cdots&a+b_n\end{vmatrix}\ (b_i\neq 0)$．
***
$D_n$ 中除主对角线外，各列元素分别相同，用加边法．

$$D_n=D_{n+1}=\begin{vmatrix}1&0&0&\cdots&0\\1&a+b_1&a&\cdots&a\\1&a&a+b_2&\cdots&a\\\vdots&\vdots&\vdots&&\vdots\\1&a&a&\cdots&a+b_n\end{vmatrix}=\begin{vmatrix}1&-a&-a&\cdots&-a\\1&b_1&0&\cdots&0\\1&0&b_2&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\1&0&0&\cdots&b_n\end{vmatrix},$$

该行列式为箭形行列式，故可求得

$$D_n=\left(1+\sum_{i=1}^{n}\frac{a}{b_i}\right)\prod_{j=1}^{n}b_j.$$

【注】① 将行列式添加一行或一列，使其升阶后的行列式的值不变，这种方法称为“**加边法**”．

② 行列式除主对角线外，第 $i\ (i=1,2,\cdots,n)$ 行（列）元素分别与第 $j\ (j\neq i)$ 行（列）元素有倍数关系或相同，此类行列式的计算可采用“加边法”．

+++

#### 综合解答 (3) 计算 $n$ 阶行列式 $D_n=\begin{vmatrix}a_0&-1&0&\cdots&0&0\\a_1&x&-1&\cdots&0&0\\a_2&0&x&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\a_{n-2}&0&0&\cdots&x&-1\\a_{n-1}&0&0&\cdots&0&x\end{vmatrix}$．
***
按第 $n$ 行展开，用递推法．

$$D_n=(-1)^{n+1}a_{n-1}\cdot(-1)^{n-1}+(-1)^{n+n}\cdot x\cdot D_{n-1}=a_{n-1}+xD_{n-1}$$

$$=a_{n-1}+a_{n-2}x+x^{2}D_{n-2}=\cdots=a_0x^{n-1}+a_1x^{n-2}+\cdots+a_{n-2}x+a_{n-1}.$$

+++

#### 综合解答 (4) 计算 $D_n=\begin{vmatrix}a&b&0&\cdots&0&0\\c&a&b&\cdots&0&0\\0&c&a&\cdots&0&0\\\vdots&\vdots&\vdots&&\vdots&\vdots\\0&0&0&\cdots&a&b\\0&0&0&\cdots&c&a\end{vmatrix}\ (a^{2}-4bc\geqslant 0)$．
***
三对角行列式，用递推法．

按第 $1$ 列展开，得

$$D_n=aD_{n-1}-bcD_{n-2},\qquad ①$$

将 ① 式化为

$$D_n-kD_{n-1}=\mu(D_{n-1}-kD_{n-2}),\qquad ②$$

其中

$$\begin{cases}k+\mu=a,\\ k\mu=bc.\end{cases}\qquad ③$$

令

$$D_{n-i}-kD_{n-i-1}=\Delta_{n-i}\quad(i=0,1,2,\cdots,n-2),\qquad ④$$

则递推式 ② 为 $\Delta_n=\mu\Delta_{n-1}$，反复利用这个递推式，得

$$\Delta_n=\mu\Delta_{n-1}=\mu^{2}\Delta_{n-2}=\cdots=\mu^{n-2}\Delta_2,\qquad ⑤$$

将 ④ 式代入 ⑤ 式右端，由 ③ 式可得

$$\Delta_n=\mu^{n-2}(D_2-kD_1)=\mu^{n-2}(a^{2}-bc-ka)$$

$$=\mu^{n-2}\left[a^{2}-k\mu-(a-\mu)a\right]=\mu^{n-2}\cdot\mu(a-k)=\mu^{n}.$$

将 ④ 式取 $i=0$，得 $D_n=\mu^{n}+kD_{n-1}$，反复利用这个递推式，得

$$D_n=\mu^{n}+kD_{n-1}=\mu^{n}+k(\mu^{n-1}+kD_{n-2})$$

$$=\mu^{n}+k\mu^{n-1}+k^{2}(\mu^{n-2}+kD_{n-3})$$

$$=\mu^{n}+k\mu^{n-1}+k^{2}\mu^{n-2}+k^{3}D_{n-3}=\cdots$$

$$=\mu^{n}+k\mu^{n-1}+k^{2}\mu^{n-2}+\cdots+k^{n-2}\mu^{2}+k^{n-1}D_1,$$

将 $D_1=a=k+\mu$ 代入上式，得

$$D_n=\mu^{n}+k\mu^{n-1}+k^{2}\mu^{n-2}+\cdots+k^{n-2}\mu^{2}+k^{n-1}\mu+k^{n},$$

故

$$D_n=\begin{cases}\dfrac{\mu^{n+1}-k^{n+1}}{\mu-k},&k\neq\mu,\\[2mm] (n+1)\mu^{n},&k=\mu.\end{cases}$$

由 ③ 式，知 $\mu,k$ 是一元二次方程 $x^{2}-ax+bc=0$ 的两个根，故

$$\mu=\frac{a\pm\sqrt{a^{2}-4bc}}{2},\quad k=\frac{a\mp\sqrt{a^{2}-4bc}}{2}.$$

【注】此题推出了一般三对角行列式的结论．

+++

#### 拓展解答 (1) 设矩阵 $\boldsymbol{A}$ 为 $3$ 阶非零实矩阵，$\boldsymbol{A}^{\mathrm{T}}=\boldsymbol{A}^{*}$，且 $|\boldsymbol{E}+\boldsymbol{A}|=|\boldsymbol{E}-\boldsymbol{A}|=0$，计算行列式 $|\boldsymbol{A}^{2}-\boldsymbol{A}-3\boldsymbol{E}|$．
***
由 $\boldsymbol{A}^{\mathrm{T}}=\boldsymbol{A}^{*}$，$\boldsymbol{A}\boldsymbol{A}^{*}=\boldsymbol{A}\boldsymbol{A}^{\mathrm{T}}=|\boldsymbol{A}|\boldsymbol{E}$，知

$$|\boldsymbol{A}||\boldsymbol{A}^{\mathrm{T}}|=|\boldsymbol{A}|^{2}=\left||\boldsymbol{A}|\boldsymbol{E}\right|=|\boldsymbol{A}|^{3},$$

即 $|\boldsymbol{A}|^{2}(1-|\boldsymbol{A}|)=0$，故 $|\boldsymbol{A}|=0$ 或 $|\boldsymbol{A}|=1$．

又 $\boldsymbol{A}\neq\boldsymbol{O}$，不妨设 $a_{11}\neq 0$，由已知 $\boldsymbol{A}^{\mathrm{T}}=\boldsymbol{A}^{*}$，得 $a_{ji}=A_{ji}$，故

$$|\boldsymbol{A}|=a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}=a_{11}^{2}+a_{12}^{2}+a_{13}^{2}\neq 0,$$

于是 $|\boldsymbol{A}|=1$．由

$$|\boldsymbol{E}+\boldsymbol{A}|=|(-1)(-\boldsymbol{E}-\boldsymbol{A})|=(-1)^{3}|-\boldsymbol{E}-\boldsymbol{A}|=0,$$

得 $|-\boldsymbol{E}-\boldsymbol{A}|=0$，故 $\lambda_1=-1$ 是 $\boldsymbol{A}$ 的一个特征值．

同理，由 $|\boldsymbol{E}-\boldsymbol{A}|=0$，得 $\lambda_2=1$ 是 $\boldsymbol{A}$ 的一个特征值．

由 $1=|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=(-1)\cdot 1\cdot\lambda_3$，得 $\lambda_3=-1$．

又 $\boldsymbol{A}^{2}-\boldsymbol{A}-3\boldsymbol{E}$ 的特征值分别为 $-1,-3,-1$，故

$$|\boldsymbol{A}^{2}-\boldsymbol{A}-3\boldsymbol{E}|=(-1)\times(-3)\times(-1)=-3.$$

【注】① 若 $\lambda$ 为 $\boldsymbol{A}$ 的特征值，则 $f(\boldsymbol{A})$ 的特征值为 $f(\lambda)$，其中 $f(x)$ 为多项式．

② 计算抽象行列式常用到以下公式：\
（i）若 $\boldsymbol{A}$ 是 $n$ 阶方阵，则 $|k\boldsymbol{A}|=k^{n}|\boldsymbol{A}|$；\
（ii）若 $\boldsymbol{A},\boldsymbol{B}$ 是同型方阵，则 $|\boldsymbol{A}\boldsymbol{B}|=|\boldsymbol{A}||\boldsymbol{B}|$；\
（iii）若 $\boldsymbol{A}$ 是 $n$ 阶方阵，则 $|\boldsymbol{A}^{*}|=|\boldsymbol{A}|^{n-1}$；\
（iv）若 $\boldsymbol{A}$ 是 $n$ 阶可逆方阵，则 $|\boldsymbol{A}^{-1}|=|\boldsymbol{A}|^{-1}$；\
（v）若 $\boldsymbol{A}$ 的特征值为 $\lambda_1,\lambda_2,\cdots,\lambda_n$，则 $|\boldsymbol{A}|=\lambda_1\lambda_2\cdots\lambda_n$；\
（vi）若 $\boldsymbol{A}\sim\boldsymbol{B}$，则 $|\boldsymbol{A}|=|\boldsymbol{B}|$．

+++

#### 拓展解答 (2) 设 $\boldsymbol{A}$ 为 $3$ 阶非零实矩阵，且 $\boldsymbol{A}^{\mathrm{T}}=k\boldsymbol{A}^{*}$（$k$ 为非零常数）．

（Ⅰ）证明：$\boldsymbol{A}$ 是可逆矩阵；\
（Ⅱ）求行列式 $|\boldsymbol{A}^{-1}|+|(\boldsymbol{A}^{*})^{-1}|$．
***
（Ⅰ）因为 $\boldsymbol{A}\neq\boldsymbol{O}$，不妨设 $a_{11}\neq 0$．由 $\boldsymbol{A}^{\mathrm{T}}=k\boldsymbol{A}^{*}$，知 $a_{ji}=kA_{ji}$．

将 $|\boldsymbol{A}|$ 按第一行展开，得

$$|\boldsymbol{A}|=a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}=\frac{1}{k}\left(a_{11}^{2}+a_{12}^{2}+a_{13}^{2}\right)\neq 0,$$

即 $\boldsymbol{A}$ 是可逆矩阵．

（Ⅱ）由 $\boldsymbol{A}\boldsymbol{A}^{*}=\dfrac{1}{k}\boldsymbol{A}\boldsymbol{A}^{\mathrm{T}}=|\boldsymbol{A}|\boldsymbol{E}$，且

$$\left|\frac{1}{k}\boldsymbol{A}\boldsymbol{A}^{\mathrm{T}}\right|=\frac{1}{k^{3}}|\boldsymbol{A}||\boldsymbol{A}^{\mathrm{T}}|=\frac{1}{k^{3}}|\boldsymbol{A}|^{2},\quad \left||\boldsymbol{A}|\boldsymbol{E}\right|=|\boldsymbol{A}|^{3},$$

可知 $\dfrac{1}{k^{3}}|\boldsymbol{A}|^{2}=|\boldsymbol{A}|^{3}$，整理得 $|\boldsymbol{A}|^{2}\left(\dfrac{1}{k^{3}}-|\boldsymbol{A}|\right)=0$，又由（Ⅰ）知 $|\boldsymbol{A}|\neq 0$，故

$$|\boldsymbol{A}|=\frac{1}{k^{3}},\quad |\boldsymbol{A}^{-1}|=\frac{1}{|\boldsymbol{A}|}=k^{3}.$$

又由 $(\boldsymbol{A}^{*})^{-1}=\dfrac{\boldsymbol{A}}{|\boldsymbol{A}|}$，知

$$|(\boldsymbol{A}^{*})^{-1}|=\left|\frac{\boldsymbol{A}}{|\boldsymbol{A}|}\right|=\frac{1}{|\boldsymbol{A}|^{3}}|\boldsymbol{A}|=\frac{1}{|\boldsymbol{A}|^{2}}=k^{6},$$

故 $|\boldsymbol{A}^{-1}|+|(\boldsymbol{A}^{*})^{-1}|=k^{3}+k^{6}$．
