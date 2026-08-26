---
quizify:
  format: 1
  deck: Math_880::Chapter_14
  tags: [Math, 880题, 数一, 第十四章, 相似矩阵]
---

+++

#### 基础选择 (1) 设 $\lambda=2$ 是矩阵 $\boldsymbol{A}$ 的一个特征值，且 $|\boldsymbol{A}|\neq 0$，则 $\left(\dfrac{1}{3}\boldsymbol{A}^{2}\right)^{-1}$ 有一个特征值为（　）．

;;;
A. $\dfrac{4}{3}$
B. $\dfrac{3}{4}$
C. $\dfrac{1}{2}$
D. $\dfrac{1}{4}$
;;;B
***
$\left(\dfrac{1}{3}\boldsymbol{A}^{2}\right)^{-1}=3(\boldsymbol{A}^{-1})^{2}$，由已知 $\boldsymbol{A}$ 有特征值 $\lambda=2$，故 $\boldsymbol{A}^{-1}$ 有特征值 $\dfrac{1}{2}$，$(\boldsymbol{A}^{-1})^{2}$ 有特征值 $\dfrac{1}{4}$，故所求特征值为 $\dfrac{3}{4}$．

【注】有关特征值、特征向量的结论：

| $\boldsymbol{A}$ | $\boldsymbol{A}^{n}$ | $\boldsymbol{A}+k\boldsymbol{E}$ | $f(\boldsymbol{A})$ | $\boldsymbol{A}^{-1}$ | $\boldsymbol{A}^{*}$ | $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$ | $\boldsymbol{A}^{\mathrm{T}}$ |
| --- | --- | --- | --- | --- | --- | --- | --- |
| $\lambda$ | $\lambda^{n}$ | $\lambda+k$ | $f(\lambda)$ | $\dfrac{1}{\lambda}$ | $\dfrac{\lvert\boldsymbol{A}\rvert}{\lambda}$ | $\lambda$ | $\lambda$ |
| $\boldsymbol{\alpha}$ | $\boldsymbol{\alpha}$ | $\boldsymbol{\alpha}$ | $\boldsymbol{\alpha}$ | $\boldsymbol{\alpha}$ | $\boldsymbol{\alpha}$ | $\boldsymbol{P}^{-1}\boldsymbol{\alpha}$ | / |

其中 $f(\lambda)$ 为多项式．以上结论可用特征值、特征向量的定义 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}\ (\boldsymbol{\alpha}\neq\boldsymbol{0})$ 进行验证．

+++

#### 基础选择 (2) 设 $4$ 阶实对称矩阵 $\boldsymbol{A}$ 的特征值为 $0,1,2,3$，则 $r(\boldsymbol{A})=$（　）．

;;;
A. $1$
B. $2$
C. $3$
D. $4$
;;;C
***
因实对称矩阵必相似于由特征值组成的对角矩阵，即 $\mathrm{diag}(0,1,2,3)$，且有相同的秩，即

$$r(\boldsymbol{A})=r(\mathrm{diag}(0,1,2,3))=3.$$

+++

#### 基础选择 (3) 设 $\boldsymbol{C}=\mathrm{diag}(1,2,2)$，$\boldsymbol{A}=\begin{pmatrix}2&0&0\\0&2&1\\0&0&1\end{pmatrix}$，$\boldsymbol{B}=\begin{pmatrix}2&1&0\\0&2&0\\0&0&1\end{pmatrix}$，则（　）．

;;;
A. $\boldsymbol{A}$ 与 $\boldsymbol{C}$ 相似，$\boldsymbol{B}$ 与 $\boldsymbol{C}$ 不相似
B. $\boldsymbol{A}$ 与 $\boldsymbol{C}$ 相似，$\boldsymbol{B}$ 与 $\boldsymbol{C}$ 相似
C. $\boldsymbol{A}$ 与 $\boldsymbol{C}$ 不相似，$\boldsymbol{B}$ 与 $\boldsymbol{C}$ 相似
D. $\boldsymbol{A}$ 与 $\boldsymbol{C}$ 不相似，$\boldsymbol{B}$ 与 $\boldsymbol{C}$ 不相似
;;;A
***
判别 $\boldsymbol{A},\boldsymbol{B}$ 与对角矩阵 $\boldsymbol{C}$ 是否相似，利用矩阵相似于对角矩阵的充分条件或充要条件．

由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$，得 $\boldsymbol{A}$ 的特征值为 $2,2,1$．又

$$2\boldsymbol{E}-\boldsymbol{A}=\begin{pmatrix}0&0&0\\0&0&-1\\0&0&1\end{pmatrix},$$

知 $r(2\boldsymbol{E}-\boldsymbol{A})=1$，即 $(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$ 中，特征值 $2$ 对应两个线性无关的特征向量，所以 $\boldsymbol{A}\sim\boldsymbol{C}$．

由 $|\lambda\boldsymbol{E}-\boldsymbol{B}|=0$，得 $\boldsymbol{B}$ 的特征值为 $2,2,1$．又

$$2\boldsymbol{E}-\boldsymbol{B}=\begin{pmatrix}0&-1&0\\0&0&0\\0&0&1\end{pmatrix},$$

其秩为 $2$，即 $(2\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$ 中，特征值 $2$ 只对应一个线性无关的特征向量，所以 $\boldsymbol{B}$ 不能相似于 $\boldsymbol{C}$．

+++

#### 基础选择 (4) 下列矩阵中，不能相似于对角矩阵的是（　）．

;;;
A. $\boldsymbol{A}=\begin{pmatrix}1&-1&3\\-1&2&0\\3&0&6\end{pmatrix}$
B. $\boldsymbol{B}=\begin{pmatrix}1&0&0\\0&2&0\\5&0&3\end{pmatrix}$
C. $\boldsymbol{C}=\begin{pmatrix}0&0&0\\0&0&0\\1&2&3\end{pmatrix}$
D. $\boldsymbol{D}=\begin{pmatrix}1&2&0\\0&0&3\\0&0&0\end{pmatrix}$
;;;D
***
对于 D，由于

$$|\lambda\boldsymbol{E}-\boldsymbol{D}|=\begin{vmatrix}\lambda-1&-2&0\\0&\lambda&-3\\0&0&\lambda\end{vmatrix}=\lambda^{2}(\lambda-1)=0,$$

所以 $\boldsymbol{D}$ 的特征值为 $\lambda_1=\lambda_2=0,\lambda_3=1$．

对 $\lambda_1=\lambda_2=0$，

$$0\boldsymbol{E}-\boldsymbol{D}=\begin{pmatrix}-1&-2&0\\0&0&-3\\0&0&0\end{pmatrix},$$

可知 $r(0\boldsymbol{E}-\boldsymbol{D})=2$，故 $\lambda_1=\lambda_2=0$ 只对应 $3-r(0\boldsymbol{E}-\boldsymbol{D})=3-2=1$ 个特征向量，所以 $\boldsymbol{D}$ 不能相似于对角矩阵．

对于 A：显然 $\boldsymbol{A}$ 是实对称矩阵，故必相似于对角矩阵．

对于 B：由 $|\lambda\boldsymbol{E}-\boldsymbol{B}|=0$，得 $\lambda_1=1,\lambda_2=2,\lambda_3=3$，即 $\boldsymbol{B}$ 有三个不同特征值，故它必相似于对角矩阵．

对于 C：由 $|\lambda\boldsymbol{E}-\boldsymbol{C}|=0$，得 $\lambda_1=\lambda_2=0,\lambda_3=3$，对于 $\lambda_1=\lambda_2=0$，

$$r(0\boldsymbol{E}-\boldsymbol{C})=r\begin{pmatrix}0&0&0\\0&0&0\\-1&-2&-3\end{pmatrix}=1,$$

故 $\lambda_1=\lambda_2=0$ 有两个线性无关的特征向量，故 $\boldsymbol{C}$ 相似于对角矩阵．

+++

#### 基础选择 (5) 设矩阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 相似，则必有（　）．

;;;
A. 矩阵 $\lambda\boldsymbol{E}-\boldsymbol{A}$ 与 $\lambda\boldsymbol{E}-\boldsymbol{B}$ 相等
B. $\boldsymbol{A},\boldsymbol{B}$ 同时可逆或不可逆
C. $\boldsymbol{A}$ 和 $\boldsymbol{B}$ 有相同的特征向量
D. $\boldsymbol{A}$ 和 $\boldsymbol{B}$ 均与同一个对角矩阵相似
;;;B
***
由 $\boldsymbol{A}\sim\boldsymbol{B}$，知 $|\boldsymbol{A}|=|\boldsymbol{B}|$，故 $|\boldsymbol{A}|=|\boldsymbol{B}|\neq 0$ 或 $|\boldsymbol{A}|=|\boldsymbol{B}|=0$，即 $\boldsymbol{A},\boldsymbol{B}$ 同时可逆或不可逆．

+++

#### 基础选择 (6) 设 $\boldsymbol{A}$ 为 $3$ 阶方阵，$\boldsymbol{A}$ 的三个特征值为 $1,1,2$，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 分别为对应的三个特征向量，则（　）．

;;;
A. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 必为 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量
B. $\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_3$ 必为 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量
C. $\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_2$ 必为 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量
D. $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 必为 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量，$\boldsymbol{\alpha}_3$ 不是 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量
;;;A
***
$\boldsymbol{A}$ 为抽象矩阵，用定义验证．

由已知，有 $\boldsymbol{A}\boldsymbol{\alpha}_1=\boldsymbol{\alpha}_1,\boldsymbol{A}\boldsymbol{\alpha}_2=\boldsymbol{\alpha}_2,\boldsymbol{A}\boldsymbol{\alpha}_3=2\boldsymbol{\alpha}_3$，故

$$(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{\alpha}_1=2\boldsymbol{\alpha}_1-\boldsymbol{A}\boldsymbol{\alpha}_1=2\boldsymbol{\alpha}_1-\boldsymbol{\alpha}_1=1\boldsymbol{\alpha}_1,$$

$$(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{\alpha}_2=2\boldsymbol{\alpha}_2-\boldsymbol{A}\boldsymbol{\alpha}_2=2\boldsymbol{\alpha}_2-\boldsymbol{\alpha}_2=1\boldsymbol{\alpha}_2,$$

$$(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{\alpha}_3=2\boldsymbol{\alpha}_3-\boldsymbol{A}\boldsymbol{\alpha}_3=2\boldsymbol{\alpha}_3-2\boldsymbol{\alpha}_3=0\boldsymbol{\alpha}_3,$$

所以 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是 $2\boldsymbol{E}-\boldsymbol{A}$ 的特征向量．同理可验证 B，C，D 不正确．

【注】注意定义 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}$ 中 $\boldsymbol{\alpha}\neq\boldsymbol{0}$，即特征向量一定不能是零向量．

+++

#### 基础填空 (1) 已知 $\boldsymbol{A}=\begin{pmatrix}1&2&2\\2&1&2\\2&2&1\end{pmatrix}$ 与 $\boldsymbol{B}=\begin{pmatrix}-1&0&0\\0&5&0\\0&0&a\end{pmatrix}$ 相似，则 $a=$ ________．
***
$-1$．

由 $\boldsymbol{A}\sim\boldsymbol{B}$，有 $\sum\limits_{i=1}^{3}a_{ii}=\sum\limits_{i=1}^{3}b_{ii}$，知 $1+1+1=-1+5+a$，得 $a=-1$．

+++

#### 基础填空 (2) 设 $n$ 阶方阵 $\boldsymbol{B}=\boldsymbol{A}\boldsymbol{A}^{*}$，则 $\boldsymbol{B}$ 的特征值为 ________，特征向量为 ________．
***
$|\boldsymbol{A}|$，所有 $n$ 维非零列向量．

由

$$|\lambda\boldsymbol{E}-\boldsymbol{B}|=|\lambda\boldsymbol{E}-\boldsymbol{A}\boldsymbol{A}^{*}|=\big|\lambda\boldsymbol{E}-|\boldsymbol{A}|\boldsymbol{E}\big|=\big|(\lambda-|\boldsymbol{A}|)\boldsymbol{E}\big|=0,$$

知 $\boldsymbol{B}$ 的特征值为 $\lambda=|\boldsymbol{A}|$．

由 $(|\boldsymbol{A}|\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=(|\boldsymbol{A}|\boldsymbol{E}-|\boldsymbol{A}|\boldsymbol{E})\boldsymbol{x}=\boldsymbol{O}\cdot\boldsymbol{x}=\boldsymbol{0}$，可知所有 $n$ 维非零列向量均为特征向量．

+++

#### 基础填空 (3) 设方阵 $\boldsymbol{A}$ 满足 $\boldsymbol{A}^{2}+2\boldsymbol{A}+\boldsymbol{E}=\boldsymbol{O}$，则 $\boldsymbol{A}$ 有特征值 ________．
***
$-1$．

设 $\lambda$ 是 $\boldsymbol{A}$ 的任一个特征值，$\boldsymbol{\alpha}\neq\boldsymbol{0}$ 为对应的特征向量，则 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}$，故

$$(\boldsymbol{A}^{2}+2\boldsymbol{A}+\boldsymbol{E})\boldsymbol{\alpha}=\boldsymbol{A}^{2}\boldsymbol{\alpha}+2\boldsymbol{A}\boldsymbol{\alpha}+\boldsymbol{\alpha}=\lambda^{2}\boldsymbol{\alpha}+2\lambda\boldsymbol{\alpha}+\boldsymbol{\alpha}=(\lambda^{2}+2\lambda+1)\boldsymbol{\alpha}=\boldsymbol{0},$$

由 $\boldsymbol{\alpha}\neq\boldsymbol{0}$ 知 $\lambda^{2}+2\lambda+1=0$，故 $\lambda=-1$．

【注】也可有如下解法：由已知 $|\boldsymbol{A}^{2}+2\boldsymbol{A}+\boldsymbol{E}|=|(\boldsymbol{A}+\boldsymbol{E})^{2}|=|\boldsymbol{A}+\boldsymbol{E}|^{2}=0$，故 $|\boldsymbol{E}+\boldsymbol{A}|=0$，即 $|(-1)\boldsymbol{E}-\boldsymbol{A}|=0$，所以 $\boldsymbol{A}$ 有特征值 $\lambda=-1$．

+++

#### 基础填空 (4) 设 $3$ 阶矩阵 $\boldsymbol{A}$ 的特征值为 $0,1,2$，$\boldsymbol{B}=\boldsymbol{A}^{3}-2\boldsymbol{A}^{2}$，则 $r(\boldsymbol{B})=$ ________．
***
$1$．

由已知，$\boldsymbol{A}$ 有 $3$ 个不同特征值，故 $\boldsymbol{A}$ 必相似于对角矩阵，即存在可逆矩阵 $\boldsymbol{P}$，使得

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}=\begin{pmatrix}0&0&0\\0&1&0\\0&0&2\end{pmatrix}.$$

由于

$$\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P}=\boldsymbol{P}^{-1}(\boldsymbol{A}^{3}-2\boldsymbol{A}^{2})\boldsymbol{P}=\boldsymbol{P}^{-1}\boldsymbol{A}^{3}\boldsymbol{P}-2\boldsymbol{P}^{-1}\boldsymbol{A}^{2}\boldsymbol{P}=(\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P})^{3}-2(\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P})^{2}$$

$$=\begin{pmatrix}0&0&0\\0&1&0\\0&0&8\end{pmatrix}-2\begin{pmatrix}0&0&0\\0&1&0\\0&0&4\end{pmatrix}=\begin{pmatrix}0&0&0\\0&-1&0\\0&0&0\end{pmatrix}\xlongequal{\text{记}}\boldsymbol{C},$$

故 $\boldsymbol{B}$ 与 $\boldsymbol{C}$ 相似，从而 $r(\boldsymbol{B})=r(\boldsymbol{C})=1$．

+++

#### 基础解答 (1) 设 $\boldsymbol{A}=\begin{pmatrix}1&2&2\\2&1&2\\2&2&1\end{pmatrix}$．（Ⅰ）求 $\boldsymbol{A}$ 的全部特征值和特征向量；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$；（Ⅲ）求正交矩阵 $\boldsymbol{Q}$，使 $\boldsymbol{Q}^{-1}\boldsymbol{A}\boldsymbol{Q}=\boldsymbol{\Lambda}$．
***
（Ⅰ）由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-1&-2&-2\\-2&\lambda-1&-2\\-2&-2&\lambda-1\end{vmatrix}=\begin{vmatrix}\lambda-5&-2&-2\\\lambda-5&\lambda-1&-2\\\lambda-5&-2&\lambda-1\end{vmatrix}$$

$$=(\lambda-5)\begin{vmatrix}1&-2&-2\\1&\lambda-1&-2\\1&-2&\lambda-1\end{vmatrix}=(\lambda-5)\begin{vmatrix}1&-2&-2\\0&\lambda+1&0\\0&0&\lambda+1\end{vmatrix}=(\lambda-5)(\lambda+1)^{2},$$

可得 $\boldsymbol{A}$ 的特征值 $\lambda_1=5,\lambda_2=\lambda_3=-1$．

对于 $\lambda_1=5$，解方程组 $(5\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，

$$5\boldsymbol{E}-\boldsymbol{A}=\begin{pmatrix}4&-2&-2\\-2&4&-2\\-2&-2&4\end{pmatrix}\to\begin{pmatrix}-2&-2&4\\-2&4&-2\\0&0&0\end{pmatrix}\to\begin{pmatrix}1&1&-2\\0&1&-1\\0&0&0\end{pmatrix},$$

解得 $\boldsymbol{\alpha}_1=(1,1,1)^{\mathrm{T}}$，即 $k_1\boldsymbol{\alpha}_1$（$k_1$ 是任意非零常数）是 $\lambda_1=5$ 对应的全部特征向量．

对于 $\lambda_2=\lambda_3=-1$，

$$(-1)\boldsymbol{E}-\boldsymbol{A}=\begin{pmatrix}-2&-2&-2\\-2&-2&-2\\-2&-2&-2\end{pmatrix}\to\begin{pmatrix}1&1&1\\0&0&0\\0&0&0\end{pmatrix},$$

解得 $\boldsymbol{\alpha}_2=(-1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-1,0,1)^{\mathrm{T}}$，即 $k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3$（$k_2,k_3$ 是不同时为零的任意常数）是 $\lambda_2=\lambda_3=-1$ 对应的全部特征向量．

（Ⅱ）令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，则

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}=\begin{pmatrix}5&0&0\\0&-1&0\\0&0&-1\end{pmatrix}.$$

（Ⅲ）由（Ⅱ），知 $\lambda_2=\lambda_3=-1$ 为二重特征值，对其特征向量 $\boldsymbol{\alpha}_2=(-1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-1,0,1)^{\mathrm{T}}$ 正交化，令 $\boldsymbol{\beta}_2=\boldsymbol{\alpha}_2=(-1,1,0)^{\mathrm{T}}$，

$$\boldsymbol{\beta}_3=\boldsymbol{\alpha}_3-\frac{(\boldsymbol{\alpha}_3,\boldsymbol{\beta}_2)}{(\boldsymbol{\beta}_2,\boldsymbol{\beta}_2)}\boldsymbol{\beta}_2=(-1,0,1)^{\mathrm{T}}-\frac{1}{2}(-1,1,0)^{\mathrm{T}}=\left(-\frac{1}{2},-\frac{1}{2},1\right)^{\mathrm{T}}=\frac{1}{2}(-1,-1,2)^{\mathrm{T}}.$$

再对 $\boldsymbol{\alpha}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3$ 单位化，得

$$\boldsymbol{\gamma}_1=\frac{1}{\sqrt{3}}(1,1,1)^{\mathrm{T}},\quad\boldsymbol{\gamma}_2=\frac{1}{\sqrt{2}}(-1,1,0)^{\mathrm{T}},\quad\boldsymbol{\gamma}_3=\frac{1}{\sqrt{6}}(-1,-1,2)^{\mathrm{T}},$$

令 $\boldsymbol{Q}=(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)$，则 $\boldsymbol{Q}$ 为正交矩阵，使得

$$\boldsymbol{Q}^{-1}\boldsymbol{A}\boldsymbol{Q}=\boldsymbol{\Lambda}=\begin{pmatrix}5&0&0\\0&-1&0\\0&0&-1\end{pmatrix}.$$

【注】① 此题属于基础题，计算 $|\lambda\boldsymbol{E}-\boldsymbol{A}|$ 时，先化简再计算．② 考虑到三行不成比例，且 $|5\boldsymbol{E}-\boldsymbol{A}|=0$，故 $r(5\boldsymbol{E}-\boldsymbol{A})<3$，初等行变换后至少有一行元素全为 $0$，所以可以将其中任意一行写成 $(0,0,0)$，放到最后一行，这个小技巧希望读者能掌握．

+++

#### 基础解答 (2) 判别下列矩阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 是否相似．若相似，求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$．

（Ⅰ）$\boldsymbol{A}=\begin{pmatrix}1&1&1\\1&1&1\\1&1&1\end{pmatrix},\boldsymbol{B}=\begin{pmatrix}3&0&0\\0&0&0\\0&0&0\end{pmatrix}$；\
（Ⅱ）$\boldsymbol{A}=\begin{pmatrix}2&0&0\\0&0&1\\0&1&0\end{pmatrix},\boldsymbol{B}=\begin{pmatrix}1&0&0\\0&-1&0\\0&-6&2\end{pmatrix}$．
***
（Ⅰ）$\boldsymbol{A}$ 为实对称矩阵，$\boldsymbol{B}$ 为对角矩阵，而实对称矩阵必相似于对角矩阵，且与其相似的对角矩阵的对角线元素必为其特征值，故只要判别 $\boldsymbol{B}$ 的特征值 $3,0,0$ 是否为 $\boldsymbol{A}$ 的特征值即可．

由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=\lambda^{2}(\lambda-3)=0$，得 $\boldsymbol{A}$ 的特征值为 $3,0,0$，故 $\boldsymbol{A}\sim\boldsymbol{B}$．

由 $(3\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{A}$ 的特征向量 $\boldsymbol{\alpha}_1=(1,1,1)^{\mathrm{T}}$；

由 $(0\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{A}$ 的特征向量 $\boldsymbol{\alpha}_2=(-1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-1,0,1)^{\mathrm{T}}$．

令

$$\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=\begin{pmatrix}1&-1&-1\\1&1&0\\1&0&1\end{pmatrix},$$

则 $\boldsymbol{P}$ 可逆，且 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$．

（Ⅱ）$\boldsymbol{A}$ 是实对称矩阵，故 $\boldsymbol{A}$ 相似于对角矩阵．又

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=(\lambda-1)(\lambda+1)(\lambda-2),\quad|\lambda\boldsymbol{E}-\boldsymbol{B}|=(\lambda-1)(\lambda+1)(\lambda-2),$$

知 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 都有三个不同特征值 $\lambda_1=2,\lambda_2=-1,\lambda_3=1$，因此 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 均相似于对角矩阵 $\begin{pmatrix}2&0&0\\0&-1&0\\0&0&1\end{pmatrix}$，所以 $\boldsymbol{A}\sim\boldsymbol{B}$．

由 $(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0},(-\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0},(\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，可分别求得 $\boldsymbol{A}$ 的特征向量为

$$\boldsymbol{\alpha}_1=(1,0,0)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,-1,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(0,1,1)^{\mathrm{T}}.$$

令 $\boldsymbol{P}_1=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，则 $\boldsymbol{P}_1^{-1}\boldsymbol{A}\boldsymbol{P}_1=\mathrm{diag}(2,-1,1)$．

同理可求得 $\boldsymbol{B}$ 属于 $\lambda_1=2,\lambda_2=-1,\lambda_3=1$ 的特征向量分别为

$$\boldsymbol{\beta}_1=(0,0,1)^{\mathrm{T}},\boldsymbol{\beta}_2=(0,1,2)^{\mathrm{T}},\boldsymbol{\beta}_3=(1,0,0)^{\mathrm{T}}.$$

令 $\boldsymbol{P}_2=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)$，则 $\boldsymbol{P}_2^{-1}\boldsymbol{B}\boldsymbol{P}_2=\mathrm{diag}(2,-1,1)$，故 $\boldsymbol{P}_1^{-1}\boldsymbol{A}\boldsymbol{P}_1=\boldsymbol{P}_2^{-1}\boldsymbol{B}\boldsymbol{P}_2$，即

$$\boldsymbol{P}_2\boldsymbol{P}_1^{-1}\boldsymbol{A}\boldsymbol{P}_1\boldsymbol{P}_2^{-1}=\boldsymbol{B}=(\boldsymbol{P}_1\boldsymbol{P}_2^{-1})^{-1}\boldsymbol{A}(\boldsymbol{P}_1\boldsymbol{P}_2^{-1}),$$

令 $\boldsymbol{P}=\boldsymbol{P}_1\boldsymbol{P}_2^{-1}=\begin{pmatrix}0&-2&1\\1&-1&0\\1&1&0\end{pmatrix}$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$．

【注】① 判别两个同阶方阵 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 是否相似，可先利用矩阵相似的必要条件：$|\boldsymbol{A}|=|\boldsymbol{B}|,\mathrm{tr}(\boldsymbol{A})=\mathrm{tr}(\boldsymbol{B}),r(\boldsymbol{A})=r(\boldsymbol{B}),|\lambda\boldsymbol{E}-\boldsymbol{A}|=|\lambda\boldsymbol{E}-\boldsymbol{B}|,\lambda\boldsymbol{E}-\boldsymbol{A}\sim\lambda\boldsymbol{E}-\boldsymbol{B}$，$\lambda$ 为实数．（特别地，$\lambda$ 为特征值也成立）② 看 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 是否相似于同一个对角矩阵．③ 若 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 是同阶实对称矩阵，则 $\boldsymbol{A}\sim\boldsymbol{B}\Longleftrightarrow\boldsymbol{A},\boldsymbol{B}$ 有相同的特征值及重数．

+++

#### 基础解答 (3) 设矩阵 $\boldsymbol{A}=\begin{pmatrix}2&-1&2\\5&a&3\\-1&b&-2\end{pmatrix}$ 有特征向量 $\boldsymbol{\alpha}=(1,1,-1)^{\mathrm{T}}$．（Ⅰ）确定参数 $a,b$ 及 $\boldsymbol{\alpha}$ 对应的特征值 $\lambda$；（Ⅱ）问 $\boldsymbol{A}$ 能否相似于对角矩阵，说明理由．
***
（Ⅰ）已知 $\boldsymbol{A}$ 的一个特征向量 $\boldsymbol{\alpha}$，确定 $\boldsymbol{A}$ 中的参数 $a,b$，利用定义 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}$，得

$$\begin{pmatrix}2&-1&2\\5&a&3\\-1&b&-2\end{pmatrix}\begin{pmatrix}1\\1\\-1\end{pmatrix}=\lambda\begin{pmatrix}1\\1\\-1\end{pmatrix},$$

比较等式两边对应元素，得 $\lambda=-1,a=-3,b=0$．

（Ⅱ）由（Ⅰ），知 $\boldsymbol{A}=\begin{pmatrix}2&-1&2\\5&-3&3\\-1&0&-2\end{pmatrix}$，则

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-2&1&-2\\-5&\lambda+3&-3\\1&0&\lambda+2\end{vmatrix}=(\lambda+1)^{3},$$

得 $\boldsymbol{A}$ 的三重特征值 $\lambda_1=\lambda_2=\lambda_3=-1$．

由

$$r(-\boldsymbol{E}-\boldsymbol{A})=r\begin{pmatrix}-3&1&-2\\-5&2&-3\\1&0&1\end{pmatrix}=2,$$

可知三重特征值 $-1$ 只对应一个线性无关的特征向量，故 $\boldsymbol{A}$ 不能相似于对角矩阵．

+++

#### 基础解答 (4) 设 $\boldsymbol{A}=\begin{pmatrix}1&-1&1\\x&4&y\\-3&-3&5\end{pmatrix}$，$\boldsymbol{A}\sim\boldsymbol{\Lambda}$，且 $\lambda=2$ 是 $\boldsymbol{A}$ 的二重特征值，求 $x,y$ 的值及可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$．
***
由 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$，知 $\boldsymbol{A}$ 有 $3$ 个线性无关的特征向量，$\lambda=2$ 是二重特征值，应该对应有两个线性无关的特征向量，故 $r(2\boldsymbol{E}-\boldsymbol{A})=3-2=1$，即

$$r(2\boldsymbol{E}-\boldsymbol{A})=r\begin{pmatrix}1&1&-1\\-x&-2&-y\\3&3&-3\end{pmatrix}=r\begin{pmatrix}1&1&-1\\0&x-2&-x-y\\0&0&0\end{pmatrix}=1,$$

所以 $x=2,y=-2$，故 $\boldsymbol{A}=\begin{pmatrix}1&-1&1\\2&4&-2\\-3&-3&5\end{pmatrix}$．

又 $\boldsymbol{A}$ 的另一个特征值 $\lambda_3$ 满足 $\lambda_1+\lambda_2+\lambda_3=2+2+\lambda_3=\sum\limits_{i=1}^{3}a_{ii}=10$，故 $\lambda_3=6$．

对 $\lambda_1=\lambda_2=2$，由 $(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_1=(1,-1,0)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,1,1)^{\mathrm{T}}$；

对 $\lambda_3=6$，由 $(6\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_3=(1,-2,3)^{\mathrm{T}}$．

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}=\mathrm{diag}(2,2,6)$．

+++

#### 基础解答 (5) 设 $\boldsymbol{A}$ 是 $3$ 阶矩阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是线性无关的 $3$ 维列向量，且 $\boldsymbol{A}\boldsymbol{\alpha}_1=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$，$\boldsymbol{A}\boldsymbol{\alpha}_2=2\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$，$\boldsymbol{A}\boldsymbol{\alpha}_3=2\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3$．（Ⅰ）求 $\boldsymbol{A}$ 的全部特征值；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$ 及 $\boldsymbol{\Lambda}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$，并计算 $|\boldsymbol{A}-2\boldsymbol{E}|$．
***
（Ⅰ）由已知，有

$$\boldsymbol{A}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,2\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,2\boldsymbol{\alpha}_2+3\boldsymbol{\alpha}_3)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}1&0&0\\1&2&2\\1&1&3\end{pmatrix}.\qquad ①$$

记 $\boldsymbol{B}=\begin{pmatrix}1&0&0\\1&2&2\\1&1&3\end{pmatrix}$，由 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 线性无关，记 $\boldsymbol{C}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，则 $\boldsymbol{C}$ 可逆．

由 ① 式，知 $\boldsymbol{A}\boldsymbol{C}=\boldsymbol{C}\boldsymbol{B}$，即 $\boldsymbol{C}^{-1}\boldsymbol{A}\boldsymbol{C}=\boldsymbol{B}$，因此 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 有相同的特征值．

由

$$|\lambda\boldsymbol{E}-\boldsymbol{B}|=\begin{vmatrix}\lambda-1&0&0\\-1&\lambda-2&-2\\-1&-1&\lambda-3\end{vmatrix}=(\lambda-1)^{2}(\lambda-4)=0,$$

得 $\boldsymbol{B}$ 的特征值为 $1,1,4$，即为 $\boldsymbol{A}$ 的全部特征值．

（Ⅱ）先求 $\boldsymbol{B}$ 的特征向量．

对 $\lambda_1=\lambda_2=1$，由 $(\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，可解得基础解系为 $\boldsymbol{\eta}_1=(-1,1,0)^{\mathrm{T}},\boldsymbol{\eta}_2=(-2,0,1)^{\mathrm{T}}$；

对 $\lambda_3=4$，由 $(4\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，可解得基础解系为 $\boldsymbol{\eta}_3=(0,1,1)^{\mathrm{T}}$．

令 $\boldsymbol{P}_1=(\boldsymbol{\eta}_1,\boldsymbol{\eta}_2,\boldsymbol{\eta}_3)$，则

$$\boldsymbol{P}_1^{-1}\boldsymbol{B}\boldsymbol{P}_1=\boldsymbol{\Lambda}=\begin{pmatrix}1&0&0\\0&1&0\\0&0&4\end{pmatrix},$$

于是 $\boldsymbol{P}_1^{-1}\boldsymbol{C}^{-1}\boldsymbol{A}\boldsymbol{C}\boldsymbol{P}_1=\boldsymbol{\Lambda}$，即 $(\boldsymbol{C}\boldsymbol{P}_1)^{-1}\boldsymbol{A}(\boldsymbol{C}\boldsymbol{P}_1)=\boldsymbol{\Lambda}$．令

$$\boldsymbol{P}=\boldsymbol{C}\boldsymbol{P}_1=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}-1&-2&0\\1&0&1\\0&1&1\end{pmatrix}=(-\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2,-2\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3),$$

则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$．

又由 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$，则 $\boldsymbol{A}-2\boldsymbol{E}\sim\boldsymbol{\Lambda}-2\boldsymbol{E}$，故

$$|\boldsymbol{A}-2\boldsymbol{E}|=|\boldsymbol{\Lambda}-2\boldsymbol{E}|=\begin{vmatrix}-1&0&0\\0&-1&0\\0&0&2\end{vmatrix}=2.$$

+++

#### 基础解答 (6) 设实矩阵 $\boldsymbol{A}=\begin{pmatrix}-1&0&2\\a&1&1\\1&0&0\end{pmatrix}$ 有三个线性无关的特征向量．（Ⅰ）求 $a$ 的值；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$ 为对角矩阵．
***
（Ⅰ）由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda+1&0&-2\\-a&\lambda-1&-1\\-1&0&\lambda\end{vmatrix}=(\lambda-1)^{2}(\lambda+2)=0,$$

得 $\boldsymbol{A}$ 的特征值 $\lambda_1=\lambda_2=1,\lambda_3=-2$．

因为 $\boldsymbol{A}$ 有三个线性无关的特征向量，所以对应二重特征值 $1$，$\boldsymbol{A}$ 应有两个线性无关的特征向量，故 $r(\boldsymbol{E}-\boldsymbol{A})=1$．而

$$\boldsymbol{E}-\boldsymbol{A}=\begin{pmatrix}2&0&-2\\-a&0&-1\\-1&0&1\end{pmatrix}\to\begin{pmatrix}1&0&-1\\0&0&a+1\\0&0&0\end{pmatrix},$$

故 $a+1=0$，即 $a=-1$．

（Ⅱ）对应于 $\lambda_1=\lambda_2=1$，由 $(\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_1=(0,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_2=(1,0,1)^{\mathrm{T}}$；

对应于 $\lambda_3=-2$，由 $(-2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_3=(-2,-1,1)^{\mathrm{T}}$．

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=\begin{pmatrix}0&1&-2\\1&0&-1\\0&1&1\end{pmatrix}$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\begin{pmatrix}1&&\\&1&\\&&-2\end{pmatrix}$．

+++

#### 基础解答 (7) 设 $\boldsymbol{A}$ 是 $3$ 阶实对称矩阵，$\boldsymbol{A}\sim\boldsymbol{B}$，$\boldsymbol{B}=\begin{pmatrix}1&2&3\\2&4&6\\3&6&9\end{pmatrix}$，$\boldsymbol{A}$ 的二重特征值对应的特征向量为 $\boldsymbol{\alpha}_1=(1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,2,1)^{\mathrm{T}}$．（Ⅰ）求 $\boldsymbol{A}$ 的特征值与特征向量；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$．
***
（Ⅰ）由 $\boldsymbol{A}\sim\boldsymbol{B}$ 知，$\boldsymbol{A}$ 与 $\boldsymbol{B}$ 有相同的特征值，而由 $|\mu\boldsymbol{E}-\boldsymbol{B}|=0$，可得 $\boldsymbol{B}$ 的特征值为 $\mu_1=\mu_2=0,\mu_3=14$，故 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=0,\lambda_3=14$．

由已知，二重特征值 $\lambda_1=\lambda_2=0$ 对应的特征向量为 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$，且 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2$ 线性无关，设 $\lambda_3=14$ 对应的特征向量为 $\boldsymbol{\alpha}_3=(x_1,x_2,x_3)^{\mathrm{T}}$，因为 $\boldsymbol{A}$ 是实对称矩阵，故

$$\begin{cases}\boldsymbol{\alpha}_3^{\mathrm{T}}\boldsymbol{\alpha}_1=0,\\ \boldsymbol{\alpha}_3^{\mathrm{T}}\boldsymbol{\alpha}_2=0,\end{cases}\quad\text{即}\quad\begin{cases}x_1+x_2=0,\\ 2x_2+x_3=0,\end{cases}$$

解得 $\boldsymbol{\alpha}_3=(1,-1,2)^{\mathrm{T}}$．

综上所述，$\boldsymbol{A}$ 的特征值 $\lambda_1=\lambda_2=0$ 对应的特征向量为 $k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2$（$k_1,k_2$ 不同时为 $0$），特征值 $\lambda_3=14$ 对应的特征向量为 $k_3\boldsymbol{\alpha}_3\ (k_3\neq 0)$．

（Ⅱ）令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=\begin{pmatrix}1&0&1\\1&2&-1\\0&1&2\end{pmatrix}$，则 $\boldsymbol{P}$ 可逆，使得

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\begin{pmatrix}0&0&0\\0&0&0\\0&0&14\end{pmatrix}.$$

+++

#### 基础解答 (8) 已知 $\boldsymbol{A}\sim\boldsymbol{B}$，$\boldsymbol{A}=\begin{pmatrix}1&a&-1\\1&5&1\\4&12&6\end{pmatrix}$，$\boldsymbol{B}=\begin{pmatrix}b&&\\&b&\\&&c\end{pmatrix}$，求 $a,b,c$ 的值．
***
由 $\boldsymbol{A}\sim\boldsymbol{B}$，知 $\boldsymbol{A},\boldsymbol{B}$ 有相同的特征值 $\lambda_1=\lambda_2=b,\lambda_3=c$．又

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\begin{vmatrix}\lambda-1&-a&1\\-1&\lambda-5&-1\\-4&-12&\lambda-6\end{vmatrix}=\begin{vmatrix}\lambda-2&-a&1\\0&\lambda-5&-1\\2-\lambda&-12&\lambda-6\end{vmatrix}=(\lambda-2)(\lambda^{2}-10\lambda+13-a),$$

二重特征值 $\lambda_1=\lambda_2=b$ 有两种情况：$b=2$ 或 $b\neq 2$．

当 $b=2$ 时，由 $b$ 是二重特征值，则 $\lambda^{2}-10\lambda+13-a$ 会有因式 $\lambda-2$，故可得 $a=-3$．又 $\boldsymbol{A}\sim\boldsymbol{B}$，知 $\sum\limits_{i=1}^{3}a_{ii}=\sum\limits_{i=1}^{3}b_{ii}$，即 $1+5+6=2b+c$，故 $c=8$，且此时有

$$r(2\boldsymbol{E}-\boldsymbol{A})=r\begin{pmatrix}1&3&1\\-1&-3&-1\\-4&-12&-4\end{pmatrix}=1,$$

即 $\lambda=2$ 有两个线性无关的特征向量，使得 $\boldsymbol{A}\sim\boldsymbol{B}$，所以 $a=-3,b=2,c=8$．

若 $b\neq 2$，由 $2$ 是 $\boldsymbol{A}$ 的特征值，故 $c=2$，又由 $1+5+6=b+b+c=2b+2$，知 $b=5$，此时 $\lambda^{2}-10\lambda+13-a=(\lambda-5)^{2}$，即得 $a=-12$．而

$$r(5\boldsymbol{E}-\boldsymbol{A})=r\begin{pmatrix}4&12&1\\-1&0&-1\\-4&-12&-1\end{pmatrix}=2\neq 1,$$

即 $\lambda_1=\lambda_2=b=5$，只有一个线性无关特征向量，因此 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 不相似．

综上所述，$a=-3,b=2,c=8$．

+++

#### 基础解答 (9) 设 $3$ 阶实对称矩阵 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=1,\lambda_3=-1$，$\boldsymbol{\alpha}_1=(1,1,1)^{\mathrm{T}}$，$\boldsymbol{\alpha}_2=(2,2,1)^{\mathrm{T}}$ 是 $\lambda_1=\lambda_2=1$ 对应的特征向量．（Ⅰ）求 $\boldsymbol{A}$ 的属于 $\lambda_3=-1$ 的特征向量；（Ⅱ）求矩阵 $\boldsymbol{A}$．
***
（Ⅰ）设 $\lambda_3=-1$ 对应的特征向量为 $\boldsymbol{\alpha}_3=(x_1,x_2,x_3)^{\mathrm{T}}$，由实对称矩阵不同特征值对应的特征向量必正交，可知

$$\begin{cases}\boldsymbol{\alpha}_3^{\mathrm{T}}\boldsymbol{\alpha}_1=x_1+x_2+x_3=0,\\ \boldsymbol{\alpha}_3^{\mathrm{T}}\boldsymbol{\alpha}_2=2x_1+2x_2+x_3=0,\end{cases}$$

解得 $\boldsymbol{\alpha}_3=(-1,1,0)^{\mathrm{T}}$．故 $\boldsymbol{A}$ 的属于 $\lambda_3=-1$ 的特征向量为 $k\boldsymbol{\alpha}_3\ (k\neq 0)$．

（Ⅱ）令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=\begin{pmatrix}1&2&-1\\1&2&1\\1&1&0\end{pmatrix}$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}=\mathrm{diag}(1,1,-1)$，故

$$\boldsymbol{A}=\boldsymbol{P}\boldsymbol{\Lambda}\boldsymbol{P}^{-1}=\begin{pmatrix}1&2&-1\\1&2&1\\1&1&0\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&0\\0&0&-1\end{pmatrix}\begin{pmatrix}1&2&-1\\1&2&1\\1&1&0\end{pmatrix}^{-1}=\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}.$$

+++

#### 基础解答 (10) （Ⅰ）设 $\boldsymbol{A}$ 是 $n$ 阶实对称矩阵，且 $\boldsymbol{A}^{2}=\boldsymbol{A}$，$r(\boldsymbol{A})=r\ (r<n)$，计算 $|3\boldsymbol{E}-\boldsymbol{A}|$；\
（Ⅱ）设 $\boldsymbol{A}$ 是 $n$ 阶矩阵，且 $\boldsymbol{A}^{2}=\boldsymbol{A}$，$r(\boldsymbol{A})=r\ (r<n)$，计算 $|3\boldsymbol{E}-\boldsymbol{A}|$．
***
（Ⅰ）由 $\boldsymbol{A}$ 是实对称矩阵，知 $\boldsymbol{A}$ 必相似于对角矩阵 $\boldsymbol{\Lambda}$，由 $\boldsymbol{A}^{2}=\boldsymbol{A}$ 知，$\boldsymbol{A}$ 的特征值的取值是 $0$ 与 $1$．

又 $r(\boldsymbol{A})=r$，故 $r(\boldsymbol{\Lambda})=r$，即有

$$\boldsymbol{A}\sim\boldsymbol{\Lambda}=\mathrm{diag}(\underbrace{1,1,\cdots,1}_{r\ \text{个}},0,\cdots,0),$$

从而 $\boldsymbol{A}$ 的特征值 $\lambda=1$ 的重数为 $r$，$\lambda=0$ 的重数为 $n-r$，故 $3\boldsymbol{E}-\boldsymbol{A}$ 的特征值 $\lambda=2$ 的重数为 $r$，$\lambda=3$ 的重数为 $n-r$，所以 $|3\boldsymbol{E}-\boldsymbol{A}|=2^{r}\cdot 3^{n-r}$．

（Ⅱ）由 $\boldsymbol{A}^{2}=\boldsymbol{A}$，知 $\boldsymbol{A}$ 的特征值是 $0$ 与 $1$，但没有 $\boldsymbol{A}$ 是实对称矩阵的条件，所以要检验 $\boldsymbol{A}$ 是否相似于对角矩阵．

由 $\boldsymbol{A}-\boldsymbol{A}^{2}=\boldsymbol{A}(\boldsymbol{E}-\boldsymbol{A})=\boldsymbol{O}$，知 $r(\boldsymbol{A})+r(\boldsymbol{E}-\boldsymbol{A})\leqslant n$．又

$$r(\boldsymbol{A})+r(\boldsymbol{E}-\boldsymbol{A})\geqslant r(\boldsymbol{A}+\boldsymbol{E}-\boldsymbol{A})=r(\boldsymbol{E})=n,$$

故 $r(\boldsymbol{A})+r(\boldsymbol{E}-\boldsymbol{A})=n$，即有 $r(\boldsymbol{E}-\boldsymbol{A})=n-r(\boldsymbol{A})=n-r$．

对于 $\lambda=1$，$(\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，而 $r(\boldsymbol{E}-\boldsymbol{A})=n-r$，故 $\boldsymbol{A}$ 有 $r$ 个线性无关的特征向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_r$；

对于 $\lambda=0$，$(0\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，即 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$，而 $r(\boldsymbol{A})=r$，故 $\boldsymbol{A}$ 有 $n-r$ 个线性无关的特征向量 $\boldsymbol{\alpha}_{r+1},\boldsymbol{\alpha}_{r+2},\cdots,\boldsymbol{\alpha}_n$，所以 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)$，使得

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\mathrm{diag}(\underbrace{1,1,\cdots,1}_{r\ \text{个}},0,\cdots,0)=\boldsymbol{\Lambda},$$

可得 $3\boldsymbol{E}-\boldsymbol{A}\sim 3\boldsymbol{E}-\boldsymbol{\Lambda}$，所以

$$|3\boldsymbol{E}-\boldsymbol{A}|=|3\boldsymbol{E}-\boldsymbol{\Lambda}|=2^{r}\cdot 3^{n-r}.$$

【注】$n$ 阶方阵 $\boldsymbol{A}$ 满足 $\boldsymbol{A}^{2}=\boldsymbol{A}$，求 $\boldsymbol{A}$ 的特征值．由定义，设 $\lambda$ 是 $\boldsymbol{A}$ 的任一个特征值，$\boldsymbol{\alpha}$ 是对应的特征向量，即有 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}\ (\boldsymbol{\alpha}\neq\boldsymbol{0})$，故 $\boldsymbol{A}^{2}\boldsymbol{\alpha}=\lambda\boldsymbol{A}\boldsymbol{\alpha}=\lambda^{2}\boldsymbol{\alpha}$，即有 $(\boldsymbol{A}^{2}-\boldsymbol{A})\boldsymbol{\alpha}=(\lambda^{2}-\lambda)\boldsymbol{\alpha}=\boldsymbol{0}$，而 $\boldsymbol{\alpha}\neq\boldsymbol{0}$，故 $\lambda^{2}-\lambda=0$，得 $\lambda=0,\lambda=1$，即 $\boldsymbol{A}$ 的特征值的取值只能为 $0$ 或 $1$，但有多少个特征值取 $0$ 或 $1$，不能确定，还需要其他条件才能确定．事实上满足 $\boldsymbol{A}^{2}=\boldsymbol{A}$ 的矩阵不唯一，如 $\begin{pmatrix}1&0\\0&0\end{pmatrix},\begin{pmatrix}1&0\\0&1\end{pmatrix}$ 都满足 $\boldsymbol{A}^{2}=\boldsymbol{A}$．

+++

#### 综合选择 (1) 设 $\boldsymbol{A},\boldsymbol{B}$ 是 $n$ 阶可逆矩阵，且 $\boldsymbol{A}^{-1}\sim\boldsymbol{B}^{-1}$，则下列结果中正确的个数为（　）．

① $\boldsymbol{A}\boldsymbol{B}\sim\boldsymbol{B}\boldsymbol{A}$　② $\boldsymbol{A}\sim\boldsymbol{B}$　③ $\boldsymbol{A}^{2}\sim\boldsymbol{B}^{2}$　④ $\boldsymbol{A}^{\mathrm{T}}\sim\boldsymbol{B}^{\mathrm{T}}$

;;;
A. $1$
B. $2$
C. $3$
D. $4$
;;;D
***
利用矩阵相似的定义．由

$$\boldsymbol{B}\boldsymbol{A}=\boldsymbol{E}\boldsymbol{B}\boldsymbol{A}=\boldsymbol{A}^{-1}\boldsymbol{A}\boldsymbol{B}\boldsymbol{A}=\boldsymbol{A}^{-1}(\boldsymbol{A}\boldsymbol{B})\boldsymbol{A},$$

知 $\boldsymbol{A}\boldsymbol{B}\sim\boldsymbol{B}\boldsymbol{A}$．由 $\boldsymbol{A}^{-1}\sim\boldsymbol{B}^{-1}$ 知，存在可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}^{-1}\boldsymbol{P}=\boldsymbol{B}^{-1}$．两边同时求逆，得

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B},\qquad ①$$

故 $\boldsymbol{A}\sim\boldsymbol{B}$．① 式两边同时取转置，得 $\boldsymbol{P}^{\mathrm{T}}\boldsymbol{A}^{\mathrm{T}}(\boldsymbol{P}^{-1})^{\mathrm{T}}=\boldsymbol{B}^{\mathrm{T}}$，即 $\boldsymbol{P}^{\mathrm{T}}\boldsymbol{A}^{\mathrm{T}}(\boldsymbol{P}^{\mathrm{T}})^{-1}=\boldsymbol{B}^{\mathrm{T}}$，故 $\boldsymbol{A}^{\mathrm{T}}\sim\boldsymbol{B}^{\mathrm{T}}$．

又由 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}\cdot\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{P}^{-1}\boldsymbol{A}^{2}\boldsymbol{P}=\boldsymbol{B}^{2}$，可知 $\boldsymbol{A}^{2}\sim\boldsymbol{B}^{2}$．

综上所述，**D** 正确．

+++

#### 综合选择 (2) 设矩阵 $\boldsymbol{B}$ 相似于 $\boldsymbol{A}=\begin{pmatrix}1&1&0&0\\1&1&0&0\\0&0&2&2\\0&0&2&2\end{pmatrix}$，则 $r_1=r(\boldsymbol{B})$，$r_2=r(\boldsymbol{B}-\boldsymbol{E})$，$r_3=r(\boldsymbol{B}-2\boldsymbol{E})$ 满足（　）．

;;;
A. $r_1<r_2<r_3$
B. $r_2<r_3<r_1$
C. $r_3<r_1<r_2$
D. $r_1<r_3<r_2$
;;;D
***
由于 $\boldsymbol{A}$ 是实对称矩阵，所以 $\boldsymbol{A}$ 相似于对角矩阵．又

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=\lambda^{2}(\lambda-2)(\lambda-4)=0,$$

得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=0,\lambda_3=2,\lambda_4=4$．

而 $\boldsymbol{B}\sim\boldsymbol{A}$，故 $\boldsymbol{B}$ 的特征值也是 $\lambda_1=\lambda_2=0,\lambda_3=2,\lambda_4=4$，且 $\boldsymbol{B}$ 也相似于对角矩阵，故

$$r(\boldsymbol{B})=r(0\boldsymbol{E}-\boldsymbol{B})=4-2=2,\qquad r(\boldsymbol{B}-2\boldsymbol{E})=r(2\boldsymbol{E}-\boldsymbol{B})=4-1=3.$$

由于 $1$ 不是 $\boldsymbol{B}$ 的特征值，所以 $|\boldsymbol{E}-\boldsymbol{B}|\neq 0$，故 $r(\boldsymbol{B}-\boldsymbol{E})=4$，**D** 正确．

【注】① 由 $\boldsymbol{B}\sim\boldsymbol{\Lambda}$，知二重特征值 $\lambda_1=\lambda_2=0$ 对应两个线性无关的特征向量，故 $r(0\boldsymbol{E}-\boldsymbol{B})=4-2=2$．由 $\lambda_3=2$ 是单根，故对应一个特征向量，故 $r(2\boldsymbol{E}-\boldsymbol{B})=4-1=3$．

② $n$ 阶矩阵 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$ 的有关定理（一个充分条件，两个充要条件）：\
（ⅰ）（充分条件）$\boldsymbol{A}$ 有 $n$ 个不同的特征值 $\Rightarrow\boldsymbol{A}\sim\boldsymbol{\Lambda}$；\
（ⅱ）（充要条件）$\boldsymbol{A}\sim\boldsymbol{\Lambda}\Longleftrightarrow\boldsymbol{A}$ 有 $n$ 个线性无关的特征向量；\
（ⅲ）（充要条件）$\boldsymbol{A}\sim\boldsymbol{\Lambda}\Longleftrightarrow\boldsymbol{A}$ 的 $k$ 重特征值 $\lambda_k$ 对应 $k$ 个线性无关的特征向量（即 $r(\lambda_k\boldsymbol{E}-\boldsymbol{A})=n-k$）．

这三个基本定理必须熟练掌握．

+++

#### 综合选择 (3) 与 $\boldsymbol{\Lambda}=\begin{pmatrix}0&&\\&1&\\&&-1\end{pmatrix}$ 既相似又合同的矩阵是（　）．

;;;
A. $\boldsymbol{A}=\begin{pmatrix}1&0&0\\0&1&-1\\0&2&-2\end{pmatrix}$
B. $\boldsymbol{B}=\begin{pmatrix}1&0&0\\0&-1&-2\\0&-2&-4\end{pmatrix}$
C. $\boldsymbol{C}=\begin{pmatrix}1&0&0\\0&-\dfrac{1}{2}&\dfrac{1}{2}\\0&\dfrac{1}{2}&-\dfrac{1}{2}\end{pmatrix}$
D. $\boldsymbol{D}=\begin{pmatrix}1&0&0\\0&-1&2\\0&2&2\end{pmatrix}$
;;;C
***
对于 A，由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$ 可得特征值 $\lambda_1=0,\lambda_2=1,\lambda_3=-1$，故 $\boldsymbol{A}$ 与 $\boldsymbol{\Lambda}$ 相似（因 $\boldsymbol{A}$ 有 $3$ 个不同特征值且与 $\boldsymbol{\Lambda}$ 的特征值相同）．但 $\boldsymbol{A}$ 不是实对称矩阵，而 $\boldsymbol{\Lambda}$ 是实对称矩阵，故 $\boldsymbol{A}$ 与 $\boldsymbol{\Lambda}$ 不合同．

对于 B，由 $|\lambda\boldsymbol{E}-\boldsymbol{B}|=0$ 可得特征值 $\lambda_1=0,\lambda_2=1,\lambda_3=-5$，与 $\boldsymbol{\Lambda}$ 的特征值不同，所以 $\boldsymbol{B}$ 与 $\boldsymbol{\Lambda}$ 不相似，排除 B．

对于 C，由 $|\lambda\boldsymbol{E}-\boldsymbol{C}|=0$ 可得特征值 $\lambda_1=0,\lambda_2=-1,\lambda_3=1$，故 $\boldsymbol{C}$ 与 $\boldsymbol{\Lambda}$ 相似，且实对称矩阵 $\boldsymbol{C}$ 的正、负惯性指数与 $\boldsymbol{\Lambda}$ 的正、负惯性指数分别相等，所以 **C** 正确．

对于 D，由 $|\lambda\boldsymbol{E}-\boldsymbol{D}|=0$ 可得特征值 $\lambda_1=1,\lambda_2=3,\lambda_3=-2$，与 $\boldsymbol{\Lambda}$ 的特征值不同，故与 $\boldsymbol{\Lambda}$ 不相似（或根据迹不同也可知不相似）；$\boldsymbol{D}$ 的正惯性指数为 $2$，与 $\boldsymbol{\Lambda}$ 的正惯性指数不同，故 $\boldsymbol{D}$ 与 $\boldsymbol{\Lambda}$ 也不合同．

+++

#### 综合选择 (4) 下列矩阵中，与矩阵 $\begin{pmatrix}1&1&0\\0&1&1\\0&0&1\end{pmatrix}$ 相似的是（　）．

;;;
A. $\begin{pmatrix}1&1&-1\\0&1&1\\0&0&1\end{pmatrix}$
B. $\begin{pmatrix}1&0&-1\\0&1&1\\0&0&1\end{pmatrix}$
C. $\begin{pmatrix}1&1&-1\\0&1&0\\0&0&1\end{pmatrix}$
D. $\begin{pmatrix}1&0&-1\\0&1&0\\0&0&1\end{pmatrix}$
;;;A
***
记已知条件矩阵及选项 A，B，C，D 的矩阵分别为 $\boldsymbol{A},\boldsymbol{A}_1,\boldsymbol{A}_2,\boldsymbol{A}_3,\boldsymbol{A}_4$．由

$$|\lambda\boldsymbol{E}-\boldsymbol{A}|=|\lambda\boldsymbol{E}-\boldsymbol{A}_1|=|\lambda\boldsymbol{E}-\boldsymbol{A}_2|=|\lambda\boldsymbol{E}-\boldsymbol{A}_3|=|\lambda\boldsymbol{E}-\boldsymbol{A}_4|=(\lambda-1)^{3},$$

可知五个矩阵的特征值均为 $\lambda_1=\lambda_2=\lambda_3=1$．

由 $1\boldsymbol{E}-\boldsymbol{A}=\begin{pmatrix}0&-1&0\\0&0&-1\\0&0&0\end{pmatrix}$，知 $r(\boldsymbol{E}-\boldsymbol{A})=2$，故三重特征值 $1$ 只有一个线性无关的特征向量，所以 $\boldsymbol{A}$ 不相似于对角矩阵．同理，$\boldsymbol{A}_1,\boldsymbol{A}_2,\boldsymbol{A}_3,\boldsymbol{A}_4$ 都不相似于对角矩阵．

作为选择题，可用两个矩阵相似的必要条件，利用排除法．由

$$1\boldsymbol{E}-\boldsymbol{A}_1=\begin{pmatrix}0&-1&1\\0&0&-1\\0&0&0\end{pmatrix},\ \text{知}\ r(\boldsymbol{E}-\boldsymbol{A}_1)=2,$$

$$1\boldsymbol{E}-\boldsymbol{A}_2=\begin{pmatrix}0&0&1\\0&0&-1\\0&0&0\end{pmatrix},\ \text{知}\ r(\boldsymbol{E}-\boldsymbol{A}_2)=1,$$

$$1\boldsymbol{E}-\boldsymbol{A}_3=\begin{pmatrix}0&-1&1\\0&0&0\\0&0&0\end{pmatrix},\ \text{知}\ r(\boldsymbol{E}-\boldsymbol{A}_3)=1,$$

$$1\boldsymbol{E}-\boldsymbol{A}_4=\begin{pmatrix}0&0&1\\0&0&0\\0&0&0\end{pmatrix},\ \text{知}\ r(\boldsymbol{E}-\boldsymbol{A}_4)=1,$$

故只有 $r(\boldsymbol{E}-\boldsymbol{A}_1)=r(\boldsymbol{E}-\boldsymbol{A})=2$，而 $r(\boldsymbol{E}-\boldsymbol{A})$ 与 $r(\boldsymbol{E}-\boldsymbol{A}_2),r(\boldsymbol{E}-\boldsymbol{A}_3),r(\boldsymbol{E}-\boldsymbol{A}_4)$ 均不相等，所以 $\boldsymbol{E}-\boldsymbol{A}$ 与 $\boldsymbol{E}-\boldsymbol{A}_2,\boldsymbol{E}-\boldsymbol{A}_3,\boldsymbol{E}-\boldsymbol{A}_4$ 均不相似，故 **A** 正确．

【注】结论：① $\boldsymbol{A}\sim\boldsymbol{B}\Rightarrow r(\boldsymbol{A})=r(\boldsymbol{B})$；② $\boldsymbol{A}\sim\boldsymbol{B}\Rightarrow r(\lambda\boldsymbol{E}-\boldsymbol{A})=r(\lambda\boldsymbol{E}-\boldsymbol{B})$．

+++

#### 综合选择 (5) 设 $\boldsymbol{B}=\begin{pmatrix}1&-1&0\\-1&1&0\\0&0&1\end{pmatrix},\boldsymbol{C}=\begin{pmatrix}3&0&0\\0&2&0\\0&0&0\end{pmatrix},\boldsymbol{D}=\begin{pmatrix}1&2&0\\-2&1&0\\0&0&1\end{pmatrix}$，则与矩阵 $\boldsymbol{A}=\begin{pmatrix}1&1&0\\1&1&0\\0&0&1\end{pmatrix}$ 不合同的矩阵的个数为（　）．

;;;
A. $3$ 个
B. $2$ 个
C. $1$ 个
D. $0$ 个
;;;C
***
由于 $\boldsymbol{A}$ 是实对称矩阵，故与 $\boldsymbol{A}$ 合同的矩阵也必为实对称矩阵，显然矩阵 $\boldsymbol{B},\boldsymbol{C}$ 均是实对称矩阵，矩阵 $\boldsymbol{D}$ 不是实对称矩阵，由此可知，$\boldsymbol{A}$ 与 $\boldsymbol{D}$ 不可能合同．

又由

$$\boldsymbol{x}^{\mathrm{T}}\boldsymbol{A}\boldsymbol{x}=x_1^{2}+x_2^{2}+x_3^{2}+2x_1x_2=(x_1+x_2)^{2}+x_3^{2},$$

可知 $\boldsymbol{A}$ 的正、负惯性指数分别为 $p=2,q=0$．

同理，由 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{B}\boldsymbol{x}=x_1^{2}+x_2^{2}+x_3^{2}-2x_1x_2=(x_1-x_2)^{2}+x_3^{2}$，$\boldsymbol{x}^{\mathrm{T}}\boldsymbol{C}\boldsymbol{x}=3x_1^{2}+2x_2^{2}$，可知矩阵 $\boldsymbol{B},\boldsymbol{C}$ 的正、负惯性指数相同，即 $p=2,q=0$．

综上可知，矩阵 $\boldsymbol{A}$ 与矩阵 $\boldsymbol{B},\boldsymbol{C}$ 均合同，**C** 正确．

【注】① 本题也可以求 $\boldsymbol{A},\boldsymbol{B},\boldsymbol{C}$ 的特征值，从而求得正、负惯性指数．② 若 $\boldsymbol{A},\boldsymbol{B}$ 为 $n$ 阶实对称矩阵，则 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 合同的充分必要条件是 $\boldsymbol{A}$ 与 $\boldsymbol{B}$ 有相同的正、负惯性指数．

+++

#### 综合填空 (1) 设 $\boldsymbol{A}$ 是 $3$ 阶方阵，$\boldsymbol{\alpha}$ 为 $3$ 维列向量，$\boldsymbol{P}=(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha})$ 为可逆矩阵，$\boldsymbol{B}=\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$，且 $\boldsymbol{A}^{3}\boldsymbol{\alpha}+2\boldsymbol{A}^{2}\boldsymbol{\alpha}=3\boldsymbol{A}\boldsymbol{\alpha}$，则 $|\boldsymbol{A}+\boldsymbol{E}|=$ ________．
***
$-4$．

由 $\boldsymbol{B}=\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$，知 $\boldsymbol{A}\boldsymbol{P}=\boldsymbol{P}\boldsymbol{B}$，故

$$\boldsymbol{A}\boldsymbol{P}=\boldsymbol{A}(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha})=(\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha},\boldsymbol{A}^{3}\boldsymbol{\alpha})=(\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha},3\boldsymbol{A}\boldsymbol{\alpha}-2\boldsymbol{A}^{2}\boldsymbol{\alpha})$$

$$=(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha})\begin{pmatrix}0&0&0\\1&0&3\\0&1&-2\end{pmatrix}=\boldsymbol{P}\boldsymbol{B},$$

故 $\boldsymbol{B}=\begin{pmatrix}0&0&0\\1&0&3\\0&1&-2\end{pmatrix}$，则

$$|\boldsymbol{A}+\boldsymbol{E}|=|\boldsymbol{P}\boldsymbol{B}\boldsymbol{P}^{-1}+\boldsymbol{P}\boldsymbol{P}^{-1}|=|\boldsymbol{P}|\cdot|\boldsymbol{B}+\boldsymbol{E}|\cdot|\boldsymbol{P}^{-1}|=|\boldsymbol{B}+\boldsymbol{E}|=\begin{vmatrix}1&0&0\\1&1&3\\0&1&-1\end{vmatrix}=-4.$$

+++

#### 综合填空 (2) 设 $\boldsymbol{A}_{3\times 3}$ 是秩为 $1$ 的实对称矩阵，$\lambda_1=2$ 是 $\boldsymbol{A}$ 的一个特征值，对应的特征向量为 $\boldsymbol{\alpha}_1=(-1,1,1)^{\mathrm{T}}$，则方程组 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 的基础解系为 ________．
***
$\boldsymbol{\alpha}_2=(1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,0,1)^{\mathrm{T}}$．

由 $r(\boldsymbol{A})=1$，$\boldsymbol{A}$ 为实对称矩阵，故 $\boldsymbol{A}\sim\boldsymbol{\Lambda}=\mathrm{diag}(\lambda_1,\lambda_2,\lambda_3)$，且 $\lambda_1=2,\lambda_2=\lambda_3=0$．

设 $\lambda_2=\lambda_3=0$ 对应的特征向量为 $\boldsymbol{\alpha}=(x_1,x_2,x_3)^{\mathrm{T}}$，则 $\boldsymbol{\alpha}$ 与 $\boldsymbol{\alpha}_1$ 正交，即

$$\boldsymbol{\alpha}_1^{\mathrm{T}}\boldsymbol{\alpha}=-x_1+x_2+x_3=0,$$

解得 $\boldsymbol{\alpha}_2=(1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,0,1)^{\mathrm{T}}$．

由 $(0\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，知 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$ 的基础解系为 $\boldsymbol{\alpha}_2=(1,1,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,0,1)^{\mathrm{T}}$．

+++

#### 综合解答 (1) 已知 $\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$ 是 $3$ 阶可逆矩阵，$\boldsymbol{B}$ 是 $3$ 阶矩阵，且 $\boldsymbol{B}\boldsymbol{A}=(\boldsymbol{\alpha}_1,-4\boldsymbol{\alpha}_3,-\boldsymbol{\alpha}_2)$．（Ⅰ）求 $\boldsymbol{B}$ 的全部特征值；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$ 和对角矩阵 $\boldsymbol{\Lambda}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P}=\boldsymbol{\Lambda}$．
***
（Ⅰ）由已知，有

$$\boldsymbol{B}\boldsymbol{A}=\boldsymbol{B}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)=(\boldsymbol{B}\boldsymbol{\alpha}_1,\boldsymbol{B}\boldsymbol{\alpha}_2,\boldsymbol{B}\boldsymbol{\alpha}_3)=(\boldsymbol{\alpha}_1,-4\boldsymbol{\alpha}_3,-\boldsymbol{\alpha}_2)=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}1&0&0\\0&0&-1\\0&-4&0\end{pmatrix}.$$

记 $\boldsymbol{C}=\begin{pmatrix}1&0&0\\0&0&-1\\0&-4&0\end{pmatrix}$，则 $\boldsymbol{B}\boldsymbol{A}=\boldsymbol{A}\boldsymbol{C}$，故 $\boldsymbol{A}^{-1}\boldsymbol{B}\boldsymbol{A}=\boldsymbol{C}$．

又由

$$|\lambda\boldsymbol{E}-\boldsymbol{C}|=\begin{vmatrix}\lambda-1&0&0\\0&\lambda&1\\0&4&\lambda\end{vmatrix}=(\lambda-1)(\lambda-2)(\lambda+2)=0,$$

得 $\boldsymbol{C}$ 的特征值为 $\lambda_1=1,\lambda_2=2,\lambda_3=-2$，也是 $\boldsymbol{B}$ 的特征值．

（Ⅱ）求 $\boldsymbol{C}$ 的特征向量．

对于 $\lambda_1=1$，由 $(1\boldsymbol{E}-\boldsymbol{C})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\xi}_1=(1,0,0)^{\mathrm{T}}$；

对于 $\lambda_2=2$，由 $(2\boldsymbol{E}-\boldsymbol{C})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\xi}_2=\left(0,-\dfrac{1}{2},1\right)^{\mathrm{T}}$；

对于 $\lambda_3=-2$，由 $(-2\boldsymbol{E}-\boldsymbol{C})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\xi}_3=\left(0,\dfrac{1}{2},1\right)^{\mathrm{T}}$．

令 $\boldsymbol{P}_1=(\boldsymbol{\xi}_1,\boldsymbol{\xi}_2,\boldsymbol{\xi}_3)=\begin{pmatrix}1&0&0\\0&-\dfrac{1}{2}&\dfrac{1}{2}\\0&1&1\end{pmatrix}$，则

$$\boldsymbol{P}_1^{-1}\boldsymbol{C}\boldsymbol{P}_1=\boldsymbol{\Lambda}=\mathrm{diag}(1,2,-2).\qquad ①$$

将 $\boldsymbol{A}^{-1}\boldsymbol{B}\boldsymbol{A}=\boldsymbol{C}$ 代入 ① 式，得 $\boldsymbol{P}_1^{-1}\boldsymbol{A}^{-1}\boldsymbol{B}\boldsymbol{A}\boldsymbol{P}_1=\boldsymbol{\Lambda}$，即 $(\boldsymbol{A}\boldsymbol{P}_1)^{-1}\boldsymbol{B}(\boldsymbol{A}\boldsymbol{P}_1)=\boldsymbol{\Lambda}$．令

$$\boldsymbol{P}=\boldsymbol{A}\boldsymbol{P}_1=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)\begin{pmatrix}1&0&0\\0&-\dfrac{1}{2}&\dfrac{1}{2}\\0&1&1\end{pmatrix}=\left(\boldsymbol{\alpha}_1,-\frac{1}{2}\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3,\frac{1}{2}\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3\right),$$

则 $\boldsymbol{P}$ 为所求可逆矩阵，使得 $\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P}=\boldsymbol{\Lambda}$．

+++

#### 综合解答 (2) 设 $\boldsymbol{A}$ 是 $n\ (n\geqslant 2)$ 阶矩阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 是 $n$ 维列向量，且 $\boldsymbol{A}\boldsymbol{\alpha}_1=\boldsymbol{\alpha}_2,\boldsymbol{A}\boldsymbol{\alpha}_2=\boldsymbol{\alpha}_3,\cdots,\boldsymbol{A}\boldsymbol{\alpha}_{n-1}=\boldsymbol{\alpha}_n,\boldsymbol{A}\boldsymbol{\alpha}_n=\boldsymbol{0},\boldsymbol{\alpha}_n\neq\boldsymbol{0}$．（Ⅰ）证明：$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 线性无关；（Ⅱ）求可逆矩阵 $\boldsymbol{P}$ 及三角矩阵 $\boldsymbol{B}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$．
***
（Ⅰ）用定义证．设

$$k_1\boldsymbol{\alpha}_1+k_2\boldsymbol{\alpha}_2+\cdots+k_n\boldsymbol{\alpha}_n=\boldsymbol{0},\qquad ①$$

由已知条件，有

$$\boldsymbol{A}\boldsymbol{\alpha}_1=\boldsymbol{\alpha}_2,\quad\boldsymbol{A}^{2}\boldsymbol{\alpha}_1=\boldsymbol{A}\boldsymbol{\alpha}_2=\boldsymbol{\alpha}_3,\quad\cdots\cdots$$

$$\boldsymbol{A}^{n-1}\boldsymbol{\alpha}_1=\boldsymbol{A}^{n-2}\boldsymbol{\alpha}_2=\cdots=\boldsymbol{A}\boldsymbol{\alpha}_{n-1}=\boldsymbol{\alpha}_n,\quad\boldsymbol{A}^{n}\boldsymbol{\alpha}_1=\boldsymbol{A}^{n-1}\boldsymbol{\alpha}_2=\cdots=\boldsymbol{A}\boldsymbol{\alpha}_n=\boldsymbol{0}.$$

用 $\boldsymbol{A}^{n-1}$ 左乘 ① 式，得 $k_1\boldsymbol{\alpha}_n=\boldsymbol{0}$，由 $\boldsymbol{\alpha}_n\neq\boldsymbol{0}$，得 $k_1=0$．

依次用 $\boldsymbol{A}^{n-2},\boldsymbol{A}^{n-3},\cdots,\boldsymbol{A}$ 左乘 ① 式，可得 $k_2=k_3=\cdots=k_{n-1}=0$，代入 ① 式，可得 $k_n=0$，故 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 线性无关．

（Ⅱ）

$$\boldsymbol{A}(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)=(\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\cdots,\boldsymbol{\alpha}_n,\boldsymbol{0})=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\begin{pmatrix}0&&&&\\1&0&&&\\&1&\ddots&&\\&&\ddots&0&\\&&&1&0\end{pmatrix},$$

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)$，由（Ⅰ），知 $\boldsymbol{P}$ 可逆，则

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}=\begin{pmatrix}0&&&&\\1&0&&&\\&1&\ddots&&\\&&\ddots&0&\\&&&1&0\end{pmatrix}.$$

+++

#### 综合解答 (3) 设 $\boldsymbol{A}_{3\times 3}$ 有三个不同的特征值 $\lambda_1,\lambda_2,\lambda_3$，它们对应的特征向量分别为 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$，令 $\boldsymbol{\beta}=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$．（Ⅰ）证明：$\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta}$ 线性无关；（Ⅱ）若 $\boldsymbol{A}^{3}\boldsymbol{\beta}=\boldsymbol{A}\boldsymbol{\beta}$，求 $r(\boldsymbol{A}-\boldsymbol{E})$．
***
（Ⅰ）用定义证．设

$$k_1\boldsymbol{\beta}+k_2\boldsymbol{A}\boldsymbol{\beta}+k_3\boldsymbol{A}^{2}\boldsymbol{\beta}=\boldsymbol{0},\qquad ①$$

由已知，有

$$\boldsymbol{A}\boldsymbol{\beta}=\boldsymbol{A}(\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3)=\lambda_1\boldsymbol{\alpha}_1+\lambda_2\boldsymbol{\alpha}_2+\lambda_3\boldsymbol{\alpha}_3,\quad\boldsymbol{A}^{2}\boldsymbol{\beta}=\lambda_1^{2}\boldsymbol{\alpha}_1+\lambda_2^{2}\boldsymbol{\alpha}_2+\lambda_3^{2}\boldsymbol{\alpha}_3.$$

将 $\boldsymbol{\beta}=\boldsymbol{\alpha}_1+\boldsymbol{\alpha}_2+\boldsymbol{\alpha}_3$ 及以上两式代入 ① 式，整理得

$$(k_1+k_2\lambda_1+k_3\lambda_1^{2})\boldsymbol{\alpha}_1+(k_1+k_2\lambda_2+k_3\lambda_2^{2})\boldsymbol{\alpha}_2+(k_1+k_2\lambda_3+k_3\lambda_3^{2})\boldsymbol{\alpha}_3=\boldsymbol{0},$$

由于 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 是不同特征值对应的特征向量，故它们线性无关，故

$$\begin{cases}k_1+k_2\lambda_1+k_3\lambda_1^{2}=0,\\ k_1+k_2\lambda_2+k_3\lambda_2^{2}=0,\\ k_1+k_2\lambda_3+k_3\lambda_3^{2}=0,\end{cases}$$

其系数行列式 $\begin{vmatrix}1&\lambda_1&\lambda_1^{2}\\1&\lambda_2&\lambda_2^{2}\\1&\lambda_3&\lambda_3^{2}\end{vmatrix}\neq 0$，所以 $k_1=k_2=k_3=0$，故 $\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta}$ 线性无关．

（Ⅱ）由 $\boldsymbol{A}^{3}\boldsymbol{\beta}=\boldsymbol{A}\boldsymbol{\beta}$，有

$$\boldsymbol{A}(\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta})=(\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta},\boldsymbol{A}^{3}\boldsymbol{\beta})=(\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta})=(\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta})\begin{pmatrix}0&0&0\\1&0&1\\0&1&0\end{pmatrix}.$$

令 $\boldsymbol{P}=(\boldsymbol{\beta},\boldsymbol{A}\boldsymbol{\beta},\boldsymbol{A}^{2}\boldsymbol{\beta})$，故 $\boldsymbol{A}\boldsymbol{P}=\boldsymbol{P}\boldsymbol{B}$，其中 $\boldsymbol{B}=\begin{pmatrix}0&0&0\\1&0&1\\0&1&0\end{pmatrix}$，即 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，所以 $\boldsymbol{A}-\boldsymbol{E}$ 与 $\boldsymbol{B}-\boldsymbol{E}$ 相似，故 $r(\boldsymbol{A}-\boldsymbol{E})=r(\boldsymbol{B}-\boldsymbol{E})$．而

$$r(\boldsymbol{B}-\boldsymbol{E})=r\begin{pmatrix}-1&0&0\\1&-1&1\\0&1&-1\end{pmatrix}=2,$$

所以 $r(\boldsymbol{A}-\boldsymbol{E})=2$．

+++

#### 综合解答 (4) 设 $\boldsymbol{A}=\begin{pmatrix}1&a&0&2\\0&1&2&0\\0&0&-1&b\\0&0&0&-1\end{pmatrix}$ 有四个线性无关的特征向量．（Ⅰ）求可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$；（Ⅱ）求 $(2\boldsymbol{E}-\boldsymbol{A}^{2})^{-1}$．
***
（Ⅰ）由 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0$，得 $\boldsymbol{A}$ 的特征值为 $\lambda_1=\lambda_2=1,\lambda_3=\lambda_4=-1$．

由 $\boldsymbol{A}$ 有 $4$ 个线性无关的特征向量，知二重特征值 $\lambda_1=\lambda_2=1,\lambda_3=\lambda_4=-1$ 分别对应有两个线性无关的特征向量，故

$$r(\boldsymbol{E}-\boldsymbol{A})=r\begin{pmatrix}0&-a&0&-2\\0&0&-2&0\\0&0&2&-b\\0&0&0&2\end{pmatrix}=2,$$

得 $a=0$，同理，由 $r(-\boldsymbol{E}-\boldsymbol{A})=2$，得 $b=0$．

对 $\lambda_1=\lambda_2=1$，由 $(\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_1=(1,0,0,0)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,1,0,0)^{\mathrm{T}}$；

对 $\lambda_3=\lambda_4=-1$，由 $(-\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_3=(1,0,0,-1)^{\mathrm{T}},\boldsymbol{\alpha}_4=(0,1,-1,0)^{\mathrm{T}}$．

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3,\boldsymbol{\alpha}_4)$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\mathrm{diag}(1,1,-1,-1)$．

（Ⅱ）由（Ⅰ）知

$$\boldsymbol{A}=\begin{pmatrix}1&0&0&2\\0&1&2&0\\0&0&-1&0\\0&0&0&-1\end{pmatrix}\xlongequal{\text{分块}}\begin{pmatrix}\boldsymbol{E}_2&\boldsymbol{B}\\\boldsymbol{O}&-\boldsymbol{E}_2\end{pmatrix},$$

故

$$\boldsymbol{A}^{2}=\begin{pmatrix}\boldsymbol{E}_2&\boldsymbol{B}\\\boldsymbol{O}&-\boldsymbol{E}_2\end{pmatrix}\begin{pmatrix}\boldsymbol{E}_2&\boldsymbol{B}\\\boldsymbol{O}&-\boldsymbol{E}_2\end{pmatrix}=\begin{pmatrix}\boldsymbol{E}_2&\boldsymbol{O}\\\boldsymbol{O}&\boldsymbol{E}_2\end{pmatrix}=\boldsymbol{E},$$

其中 $\boldsymbol{E}$ 为 $4$ 阶单位矩阵，所以 $(2\boldsymbol{E}-\boldsymbol{A}^{2})^{-1}=\boldsymbol{E}^{-1}=\boldsymbol{E}$．

+++

#### 综合解答 (5) 设 $\boldsymbol{\alpha}=(a_1,a_2,\cdots,a_n)^{\mathrm{T}},\boldsymbol{\beta}=(b_1,b_2,\cdots,b_n)^{\mathrm{T}}$ 均为非零列向量，$\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}$．（Ⅰ）求 $\boldsymbol{A}$ 的全部特征值；（Ⅱ）问 $\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}$ 满足什么条件时，$\boldsymbol{A}$ 可以相似于对角矩阵 $\boldsymbol{\Lambda}$，并求可逆矩阵 $\boldsymbol{P}$，使 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$．
***
（Ⅰ）

$$\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}=\begin{pmatrix}a_1\\a_2\\\vdots\\a_n\end{pmatrix}(b_1,b_2,\cdots,b_n)=\begin{pmatrix}a_1b_1&a_1b_2&\cdots&a_1b_n\\a_2b_1&a_2b_2&\cdots&a_2b_n\\\vdots&\vdots&&\vdots\\a_nb_1&a_nb_2&\cdots&a_nb_n\end{pmatrix}.$$

用定义，设 $\boldsymbol{A}$ 的任一个特征值为 $\lambda$，对应的特征向量为 $\boldsymbol{\xi}$，则

$$\boldsymbol{A}\boldsymbol{\xi}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}=\lambda\boldsymbol{\xi}.\qquad ①$$

① 式两边左乘 $\boldsymbol{\beta}^{\mathrm{T}}$，得 $\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}=\lambda\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}$．

当 $\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}\neq 0$ 时，有 $\lambda=\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}=\sum\limits_{i=1}^{n}a_ib_i$；当 $\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}=0$ 时，由 ① 式知 $\lambda=0$，故 $\boldsymbol{A}$ 的特征值为 $\lambda=0$ 或 $\lambda=\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}=\sum\limits_{i=1}^{n}a_ib_i$．

（Ⅱ）当 $\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}=\sum\limits_{i=1}^{n}a_ib_i=0$ 时，由（Ⅰ）知，$\boldsymbol{A}$ 的全部特征值为 $\lambda=0$（$n$ 重根），因 $\boldsymbol{\alpha}\neq\boldsymbol{0},\boldsymbol{\beta}\neq\boldsymbol{0}$，故 $\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\neq\boldsymbol{O}$．于是 $r(\boldsymbol{A})=1$，但对应 $\lambda=0$（$n$ 重根）的线性无关的特征向量满足 $(0\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，即 $\boldsymbol{A}\boldsymbol{x}=\boldsymbol{0}$，只有 $n-r(\boldsymbol{A})=n-1$ 个基础解系，即只有 $n-1$ 个线性无关的特征向量，故 $\boldsymbol{A}$ 不能相似于对角矩阵．

当 $\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}=\sum\limits_{i=1}^{n}a_ib_i\neq 0$ 时，对于 $\lambda=\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}$，由 $(\lambda\boldsymbol{E}-\boldsymbol{A})\boldsymbol{\xi}=(\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}\boldsymbol{E}-\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}})\boldsymbol{\xi}=\boldsymbol{0}$，以及

$$(\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}\boldsymbol{E}-\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}})\boldsymbol{\alpha}=(\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta})\boldsymbol{\alpha}-\boldsymbol{\alpha}(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})=\boldsymbol{0},$$

知对应的特征向量 $\boldsymbol{\xi}_1=\boldsymbol{\alpha}$，对于 $\lambda=0$，由 $(0\boldsymbol{E}-\boldsymbol{A})\boldsymbol{\xi}=\boldsymbol{0}$，即 $\boldsymbol{A}\boldsymbol{\xi}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}=\boldsymbol{0}$，故

$$\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\xi}=b_1x_1+b_2x_2+\cdots+b_nx_n=0.\qquad ②$$

因 $\boldsymbol{\beta}\neq\boldsymbol{0}$，不妨设 $b_1\neq 0$，解方程 ② 得线性无关的特征向量为

$$\boldsymbol{\xi}_2=(b_2,-b_1,0,\cdots,0)^{\mathrm{T}},\ \boldsymbol{\xi}_3=(b_3,0,-b_1,0,\cdots,0)^{\mathrm{T}},\ \cdots,\ \boldsymbol{\xi}_n=(b_n,0,\cdots,0,-b_1)^{\mathrm{T}}.$$

令

$$\boldsymbol{P}=(\boldsymbol{\xi}_1,\boldsymbol{\xi}_2,\cdots,\boldsymbol{\xi}_n)=\begin{pmatrix}a_1&b_2&b_3&\cdots&b_n\\a_2&-b_1&0&\cdots&0\\a_3&0&-b_1&\cdots&0\\\vdots&\vdots&\vdots&&\vdots\\a_n&0&0&\cdots&-b_1\end{pmatrix},$$

使 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\mathrm{diag}\left(\sum\limits_{i=1}^{n}a_ib_i,0,\cdots,0\right)$．

【注】① 此题 $\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}$，显然 $r(\boldsymbol{A})=1$，故 $\boldsymbol{A}^{2}=k\boldsymbol{A}$，其中 $k=\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}=\sum\limits_{i=1}^{n}a_ib_i$，即 $\boldsymbol{A}^{2}=(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})\boldsymbol{A}$．设 $\boldsymbol{A}$ 的任一个特征值为 $\lambda$，则 $\boldsymbol{A}^{2}-(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})\boldsymbol{A}$ 有特征值 $\lambda^{2}-(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})\lambda$．而 $\boldsymbol{A}^{2}-(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})\boldsymbol{A}=\boldsymbol{O}$，故 $\lambda^{2}-(\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha})\lambda=0$，从而 $\boldsymbol{A}$ 有特征值 $\lambda=0,\lambda=\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}=\sum\limits_{i=1}^{n}a_ib_i$（这实际上是秩为 $1$ 的矩阵特征值的结论）．

② 求 $\boldsymbol{A}$ 的特征值、特征向量的常用方法：（ⅰ）当 $\boldsymbol{A}$ 是具体矩阵时，用公式 $|\lambda\boldsymbol{E}-\boldsymbol{A}|=0,(\lambda\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$；（ⅱ）当 $\boldsymbol{A}$ 是抽象矩阵时，用定义 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}\ (\boldsymbol{\alpha}\neq\boldsymbol{0})$．

+++

#### 综合解答 (6) 设 $n\ (n\geqslant 2)$ 阶矩阵 $\boldsymbol{A}=\begin{pmatrix}a&1&1&\cdots&1\\1&a&1&\cdots&1\\1&1&a&\cdots&1\\\vdots&\vdots&\vdots&&\vdots\\1&1&1&\cdots&a\end{pmatrix}$．（Ⅰ）求可逆矩阵 $\boldsymbol{P}$ 及对角矩阵 $\boldsymbol{\Lambda}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}$；（Ⅱ）求 $r(\boldsymbol{A}^{*})$．
***
（Ⅰ）

$$\boldsymbol{A}=\begin{pmatrix}a-1&&&\\&a-1&&\\&&\ddots&\\&&&a-1\end{pmatrix}+\begin{pmatrix}1&1&\cdots&1\\1&1&\cdots&1\\\vdots&\vdots&&\vdots\\1&1&\cdots&1\end{pmatrix}\xlongequal{\text{记}}(a-1)\boldsymbol{E}+\boldsymbol{B}.$$

由 $r(\boldsymbol{B})=1$，$|\lambda\boldsymbol{E}-\boldsymbol{B}|=0$，得 $\boldsymbol{B}$ 的特征值为

$$\lambda_1=\sum\limits_{i=1}^{n}a_{ii}=n,\quad\lambda_2=\lambda_3=\cdots=\lambda_n=0,$$

于是 $\boldsymbol{A}$ 的特征值为 $n+(a-1),0+(a-1),\cdots,0+(a-1)$．

下求 $\boldsymbol{B}$ 的特征向量．由 $(n\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，得 $\boldsymbol{\alpha}_1=(1,1,\cdots,1)^{\mathrm{T}}$；由 $(0\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，得

$$\boldsymbol{\alpha}_2=(1,-1,0,\cdots,0)^{\mathrm{T}},\boldsymbol{\alpha}_3=(1,0,-1,\cdots,0)^{\mathrm{T}},\cdots,\boldsymbol{\alpha}_n=(1,0,0,\cdots,-1)^{\mathrm{T}},$$

由特征值、特征向量的性质，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 也是 $\boldsymbol{A}$ 的特征向量．

令 $\boldsymbol{P}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)$，则 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\mathrm{diag}(n+(a-1),a-1,\cdots,a-1)$．

（Ⅱ）由（Ⅰ），知 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$，故 $|\boldsymbol{A}|=|\boldsymbol{\Lambda}|=(n+a-1)(a-1)^{n-1}$，所以

$$r(\boldsymbol{A})=\begin{cases}n,&a\neq 1-n\ \text{且}\ a\neq 1,\\ n-1,&a=1-n,\\ 1,&a=1,\end{cases}$$

故

$$r(\boldsymbol{A}^{*})=\begin{cases}n,&a\neq 1-n\ \text{且}\ a\neq 1,\\ 1,&a=1-n,\\ 0,&a=1.\end{cases}$$

【注】① 设 $\boldsymbol{B}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}\ (\boldsymbol{\alpha}\neq\boldsymbol{0})$，$\boldsymbol{A}=(a-1)\boldsymbol{E}+\boldsymbol{B}$，则

$$\boldsymbol{A}\boldsymbol{\alpha}=[(a-1)\boldsymbol{E}+\boldsymbol{B}]\boldsymbol{\alpha}=(a-1)\boldsymbol{\alpha}+\boldsymbol{B}\boldsymbol{\alpha}=(a-1)\boldsymbol{\alpha}+\lambda\boldsymbol{\alpha}=(a-1+\lambda)\boldsymbol{\alpha},$$

故 $\boldsymbol{\alpha}$ 是 $\boldsymbol{A}$ 对应特征值 $a-1+\lambda$ 的特征向量．事实上，一般地，设 $\boldsymbol{A}\boldsymbol{\alpha}=\lambda\boldsymbol{\alpha}\ (\boldsymbol{\alpha}\neq\boldsymbol{0})$，$f(x)$ 为多项式，则 $\boldsymbol{\alpha}$ 为 $f(\boldsymbol{A})$ 的特征向量．

② 此题直接求矩阵 $\boldsymbol{A}$ 的特征值和特征向量较烦琐，将 $\boldsymbol{A}$ 写成 $\boldsymbol{A}=(a-1)\boldsymbol{E}+\boldsymbol{B}$，利用 $r(\boldsymbol{B})=1$ 求 $\boldsymbol{B}$ 的特征值和特征向量较方便．

+++

#### 综合解答 (7) 设 $\boldsymbol{A}$ 是 $2$ 阶矩阵，$\boldsymbol{\alpha}$ 是非零向量，且 $\boldsymbol{\alpha}$ 不是 $\boldsymbol{A}$ 的特征向量．（Ⅰ）证明：$\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha}$ 线性无关；（Ⅱ）记 $\boldsymbol{P}=(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha})$，若 $\boldsymbol{A}^{2}\boldsymbol{\alpha}-2\boldsymbol{A}\boldsymbol{\alpha}=8\boldsymbol{\alpha}$，证明：$\boldsymbol{A}$ 相似于对角矩阵，并求 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$．
***
（Ⅰ）用反证法．假设 $\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha}$ 线性相关，则存在不全为零的常数 $k_1,k_2$，使得

$$k_1\boldsymbol{\alpha}+k_2\boldsymbol{A}\boldsymbol{\alpha}=\boldsymbol{0}.$$

显然 $k_2\neq 0$（若 $k_2=0$，则 $k_1\boldsymbol{\alpha}=\boldsymbol{0}$，由 $\boldsymbol{\alpha}$ 为非零向量，知 $k_1=0$），则有 $\boldsymbol{A}\boldsymbol{\alpha}=-\dfrac{k_1}{k_2}\boldsymbol{\alpha}$，这与 $\boldsymbol{\alpha}$ 不是 $\boldsymbol{A}$ 的特征向量矛盾，故 $\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha}$ 线性无关．

（Ⅱ）由于

$$\boldsymbol{A}\boldsymbol{P}=\boldsymbol{A}(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha})=(\boldsymbol{A}\boldsymbol{\alpha},\boldsymbol{A}^{2}\boldsymbol{\alpha})=(\boldsymbol{A}\boldsymbol{\alpha},8\boldsymbol{\alpha}+2\boldsymbol{A}\boldsymbol{\alpha})=(\boldsymbol{\alpha},\boldsymbol{A}\boldsymbol{\alpha})\begin{pmatrix}0&8\\1&2\end{pmatrix}=\boldsymbol{P}\begin{pmatrix}0&8\\1&2\end{pmatrix},$$

故 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\begin{pmatrix}0&8\\1&2\end{pmatrix}\xlongequal{\text{记}}\boldsymbol{B}$．又由

$$|\lambda\boldsymbol{E}-\boldsymbol{B}|=\begin{vmatrix}\lambda&-8\\-1&\lambda-2\end{vmatrix}=\lambda^{2}-2\lambda-8=(\lambda+2)(\lambda-4)=0,$$

得 $\boldsymbol{B}$ 的特征值为 $\lambda_1=-2,\lambda_2=4$，同时也是 $\boldsymbol{A}$ 的两个不同特征值，故 $\boldsymbol{A}$ 相似于对角矩阵．

+++

#### 综合解答 (8) 设 $\boldsymbol{\alpha},\boldsymbol{\beta}$ 为 $3$ 维单位列向量，且 $\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}=0$，记 $\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}}$．（Ⅰ）证明：$\boldsymbol{A}$ 相似于对角矩阵；（Ⅱ）若存在 $3$ 维列向量 $\boldsymbol{\gamma}\neq\boldsymbol{0}$，使得 $\boldsymbol{A}\boldsymbol{\gamma}=\boldsymbol{0}$，记 $\boldsymbol{P}=(\boldsymbol{\gamma},2(\boldsymbol{\alpha}+\boldsymbol{\beta}),\boldsymbol{\beta}-\boldsymbol{\alpha})$，求 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}$．
***
（Ⅰ）由 $\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}=0$，知 $\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}=(\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta})^{\mathrm{T}}=0$，即 $\boldsymbol{\alpha},\boldsymbol{\beta}$ 为单位正交列向量．

由已知 $\boldsymbol{A}\boldsymbol{\alpha}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\alpha}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\alpha}=\boldsymbol{\beta}$，$\boldsymbol{A}\boldsymbol{\beta}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}\boldsymbol{\beta}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}}\boldsymbol{\beta}=\boldsymbol{\alpha}$，则

$$\boldsymbol{A}(\boldsymbol{\alpha}+\boldsymbol{\beta})=\boldsymbol{\alpha}+\boldsymbol{\beta},\quad\boldsymbol{A}(\boldsymbol{\alpha}-\boldsymbol{\beta})=-(\boldsymbol{\alpha}-\boldsymbol{\beta}).$$

由已知，$\boldsymbol{\alpha},\boldsymbol{\beta}$ 为单位正交列向量，所以 $\boldsymbol{\alpha},\boldsymbol{\beta}$ 线性无关，故 $\boldsymbol{\alpha}+\boldsymbol{\beta}\neq\boldsymbol{0},\boldsymbol{\alpha}-\boldsymbol{\beta}\neq\boldsymbol{0}$，所以 $1,-1$ 是 $\boldsymbol{A}$ 的特征值，又

$$r(\boldsymbol{A})=r(\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}})\leqslant r(\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}})+r(\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}})=1+1=2,$$

故 $\boldsymbol{A}$ 不可逆，所以 $0$ 是 $\boldsymbol{A}$ 的特征值，即 $\boldsymbol{A}$ 有三个不同的特征值 $1,-1,0$，从而

$$\boldsymbol{A}\sim\begin{pmatrix}1&&\\&-1&\\&&0\end{pmatrix}.$$

（Ⅱ）由 $\boldsymbol{A}\boldsymbol{\gamma}=\boldsymbol{0},\boldsymbol{\gamma}\neq\boldsymbol{0}$，知 $\boldsymbol{\gamma}$ 是特征值 $0$ 对应的特征向量，所以 $0,1,-1$ 分别对应的特征向量为 $\boldsymbol{\gamma},2(\boldsymbol{\alpha}+\boldsymbol{\beta}),\boldsymbol{\beta}-\boldsymbol{\alpha}$，故

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\begin{pmatrix}0&&\\&1&\\&&-1\end{pmatrix}.$$

【注】① 若 $\boldsymbol{\alpha}+\boldsymbol{\beta}$ 是 $\boldsymbol{A}$ 的特征向量，则 $k(\boldsymbol{\alpha}+\boldsymbol{\beta})\ (k\neq 0)$ 也是 $\boldsymbol{A}$ 的特征向量．

② 由 $\boldsymbol{A}=\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}}$，可得

$$\boldsymbol{A}^{\mathrm{T}}=(\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}+\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}})^{\mathrm{T}}=(\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}})^{\mathrm{T}}+(\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}})^{\mathrm{T}}=\boldsymbol{\beta}\boldsymbol{\alpha}^{\mathrm{T}}+\boldsymbol{\alpha}\boldsymbol{\beta}^{\mathrm{T}}=\boldsymbol{A},$$

故 $\boldsymbol{A}$ 是实对称矩阵，所以 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$．

+++

#### 综合解答 (9) 设 $\boldsymbol{A}=\begin{pmatrix}1&a_{12}&a_{13}\\1&a_{22}&a_{23}\\1&a_{32}&a_{33}\end{pmatrix}$ 可逆，$\boldsymbol{B}$ 是 $3$ 阶实对称矩阵，且满足 $\boldsymbol{B}\boldsymbol{A}=\begin{pmatrix}1&2a_{12}&2a_{13}\\1&2a_{22}&2a_{23}\\1&2a_{32}&2a_{33}\end{pmatrix}$．（Ⅰ）求 $\boldsymbol{B}$ 的特征值和对应的特征向量；（Ⅱ）求正交矩阵 $\boldsymbol{Q}$，使得 $\boldsymbol{Q}^{\mathrm{T}}\boldsymbol{B}\boldsymbol{Q}=\boldsymbol{\Lambda}$．
***
（Ⅰ）由 $\boldsymbol{B}\boldsymbol{A}=\begin{pmatrix}1&2a_{12}&2a_{13}\\1&2a_{22}&2a_{23}\\1&2a_{32}&2a_{33}\end{pmatrix}$，得

$$\boldsymbol{B}\begin{pmatrix}1\\1\\1\end{pmatrix}=\begin{pmatrix}1\\1\\1\end{pmatrix},\quad\boldsymbol{B}\begin{pmatrix}a_{12}\\a_{22}\\a_{32}\end{pmatrix}=2\begin{pmatrix}a_{12}\\a_{22}\\a_{32}\end{pmatrix},\quad\boldsymbol{B}\begin{pmatrix}a_{13}\\a_{23}\\a_{33}\end{pmatrix}=2\begin{pmatrix}a_{13}\\a_{23}\\a_{33}\end{pmatrix},$$

所以 $\boldsymbol{B}$ 的特征值为 $\lambda_1=1,\lambda_2=\lambda_3=2$，$\lambda_1=1$ 对应的特征向量 $\boldsymbol{\alpha}_1=(1,1,1)^{\mathrm{T}}$．

令 $\lambda_2=\lambda_3=2$ 对应的特征向量为 $\boldsymbol{x}=(x_1,x_2,x_3)^{\mathrm{T}}$，由 $\boldsymbol{B}$ 为实对称矩阵，故 $\boldsymbol{x}^{\mathrm{T}}\boldsymbol{\alpha}_1=0$，即 $x_1+x_2+x_3=0$，解得

$$\boldsymbol{\alpha}_2=(-1,0,1)^{\mathrm{T}},\boldsymbol{\alpha}_3=(-1,1,0)^{\mathrm{T}}.$$

故 $\boldsymbol{B}$ 的对应 $\lambda_2=\lambda_3=2$ 的特征向量为 $k_2\boldsymbol{\alpha}_2+k_3\boldsymbol{\alpha}_3$，其中 $k_2,k_3$ 为不全为 $0$ 的任意常数．

（Ⅱ）对 $\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 正交化，令

$$\boldsymbol{\beta}_2=\boldsymbol{\alpha}_2=\begin{pmatrix}-1\\0\\1\end{pmatrix},\quad\boldsymbol{\beta}_3=\begin{pmatrix}-1\\1\\0\end{pmatrix}-\frac{1}{2}\begin{pmatrix}-1\\0\\1\end{pmatrix}=\frac{1}{2}\begin{pmatrix}-1\\2\\-1\end{pmatrix},$$

再单位化，得

$$\boldsymbol{\gamma}_1=\frac{1}{\sqrt{3}}\begin{pmatrix}1\\1\\1\end{pmatrix},\quad\boldsymbol{\gamma}_2=\frac{1}{\sqrt{2}}\begin{pmatrix}-1\\0\\1\end{pmatrix},\quad\boldsymbol{\gamma}_3=\frac{1}{\sqrt{6}}\begin{pmatrix}-1\\2\\-1\end{pmatrix}.$$

令 $\boldsymbol{Q}=(\boldsymbol{\gamma}_1,\boldsymbol{\gamma}_2,\boldsymbol{\gamma}_3)$，则 $\boldsymbol{Q}$ 为正交矩阵，使得

$$\boldsymbol{Q}^{-1}\boldsymbol{B}\boldsymbol{Q}=\boldsymbol{Q}^{\mathrm{T}}\boldsymbol{B}\boldsymbol{Q}=\boldsymbol{\Lambda}=\begin{pmatrix}1&&\\&2&\\&&2\end{pmatrix}.$$

+++

#### 综合解答 (10) 设 $\boldsymbol{A},\boldsymbol{B}$ 均是 $n$ 阶矩阵．（Ⅰ）证明：$\boldsymbol{A}\boldsymbol{B}$ 与 $\boldsymbol{B}\boldsymbol{A}$ 有相同的特征值；（Ⅱ）若 $\boldsymbol{A}\boldsymbol{B}=\boldsymbol{B}\boldsymbol{A}$，且 $\boldsymbol{A}$ 有 $n$ 个不同的特征值，证明：$\boldsymbol{B}$ 相似于对角矩阵．
***
（Ⅰ）$\boldsymbol{A},\boldsymbol{B}$ 均是抽象矩阵，用特征值、特征向量的定义证明．

设 $\lambda$ 是 $\boldsymbol{A}\boldsymbol{B}$ 的任一个特征值，$\boldsymbol{\xi}$ 为 $\boldsymbol{A}\boldsymbol{B}$ 对应的特征向量，则

$$\boldsymbol{A}\boldsymbol{B}\boldsymbol{\xi}=\lambda\boldsymbol{\xi},\qquad ①$$

① 式左乘 $\boldsymbol{B}$，得 $\boldsymbol{B}\boldsymbol{A}\boldsymbol{B}\boldsymbol{\xi}=\boldsymbol{B}\boldsymbol{A}(\boldsymbol{B}\boldsymbol{\xi})=\lambda\boldsymbol{B}\boldsymbol{\xi}$．

若 $\boldsymbol{B}\boldsymbol{\xi}\neq\boldsymbol{0}$，上式表明 $\lambda$ 是 $\boldsymbol{B}\boldsymbol{A}$ 的特征值，$\boldsymbol{B}\boldsymbol{\xi}$ 为对应的特征向量；

若 $\boldsymbol{B}\boldsymbol{\xi}=\boldsymbol{0}$，则由 $\lambda\boldsymbol{\xi}=\boldsymbol{A}\boldsymbol{B}\boldsymbol{\xi}=\boldsymbol{0}$，又 $\boldsymbol{\xi}\neq\boldsymbol{0}$，故 $\lambda=0$，即 $\boldsymbol{A}\boldsymbol{B}$ 有特征值 $0$，从而 $|\boldsymbol{A}\boldsymbol{B}|=0$．又 $|\boldsymbol{B}\boldsymbol{A}|=|\boldsymbol{A}\boldsymbol{B}|=0$，即 $|0\boldsymbol{E}-\boldsymbol{B}\boldsymbol{A}|=0$，故 $\boldsymbol{B}\boldsymbol{A}$ 也有特征值 $0$．

综上所述，$\boldsymbol{A}\boldsymbol{B}$ 与 $\boldsymbol{B}\boldsymbol{A}$ 有相同的特征值．

（Ⅱ）由 $\boldsymbol{A}$ 有 $n$ 个不同特征值，知 $\boldsymbol{A}\sim\boldsymbol{\Lambda}$，即存在可逆矩阵 $\boldsymbol{P}$，使得

$$\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{\Lambda}=\mathrm{diag}(\lambda_1,\lambda_2,\cdots,\lambda_n).$$

由 $\boldsymbol{A}\boldsymbol{B}=\boldsymbol{B}\boldsymbol{A}$，得

$$(\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P})(\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P})=(\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P})(\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}),\qquad ②$$

令 $\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P}=(C_{ij})_{n\times n}$，代入 ② 式，得

$$\begin{pmatrix}\lambda_1&&&\\&\lambda_2&&\\&&\ddots&\\&&&\lambda_n\end{pmatrix}\begin{pmatrix}C_{11}&C_{12}&\cdots&C_{1n}\\C_{21}&C_{22}&\cdots&C_{2n}\\\vdots&\vdots&&\vdots\\C_{n1}&C_{n2}&\cdots&C_{nn}\end{pmatrix}=\begin{pmatrix}C_{11}&C_{12}&\cdots&C_{1n}\\C_{21}&C_{22}&\cdots&C_{2n}\\\vdots&\vdots&&\vdots\\C_{n1}&C_{n2}&\cdots&C_{nn}\end{pmatrix}\begin{pmatrix}\lambda_1&&&\\&\lambda_2&&\\&&\ddots&\\&&&\lambda_n\end{pmatrix},$$

比较等式两边元素，得 $\lambda_iC_{ij}=C_{ij}\lambda_j\ (i,j=1,2,\cdots,n)$．

当 $i\neq j$ 时，有 $(\lambda_i-\lambda_j)C_{ij}=0$，而 $\lambda_i\neq\lambda_j$ 故 $C_{ij}=0$，即

$$\boldsymbol{P}^{-1}\boldsymbol{B}\boldsymbol{P}=\begin{pmatrix}C_{11}&&&\\&C_{22}&&\\&&\ddots&\\&&&C_{nn}\end{pmatrix},$$

故 $\boldsymbol{B}$ 相似于对角矩阵．

+++

#### 综合解答 (11) 设 $\boldsymbol{A}$ 是 $n$ 阶实对称矩阵，$\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n$ 是 $\boldsymbol{A}$ 的 $n$ 个单位正交特征向量，对应的特征值为 $\lambda_1,\lambda_2,\cdots,\lambda_n$，证明：$\boldsymbol{A}=\lambda_1\boldsymbol{\alpha}_1\boldsymbol{\alpha}_1^{\mathrm{T}}+\lambda_2\boldsymbol{\alpha}_2\boldsymbol{\alpha}_2^{\mathrm{T}}+\cdots+\lambda_n\boldsymbol{\alpha}_n\boldsymbol{\alpha}_n^{\mathrm{T}}$．
***
令 $\boldsymbol{Q}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)$，由已知，有

$$\boldsymbol{A}=\boldsymbol{Q}\,\mathrm{diag}(\lambda_1,\lambda_2,\cdots,\lambda_n)\,\boldsymbol{Q}^{-1}=\boldsymbol{Q}\,\mathrm{diag}(\lambda_1,\lambda_2,\cdots,\lambda_n)\,\boldsymbol{Q}^{\mathrm{T}},$$

故

$$\boldsymbol{A}=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\cdots,\boldsymbol{\alpha}_n)\begin{pmatrix}\lambda_1&&&\\&\lambda_2&&\\&&\ddots&\\&&&\lambda_n\end{pmatrix}\begin{pmatrix}\boldsymbol{\alpha}_1^{\mathrm{T}}\\\boldsymbol{\alpha}_2^{\mathrm{T}}\\\vdots\\\boldsymbol{\alpha}_n^{\mathrm{T}}\end{pmatrix}=\lambda_1\boldsymbol{\alpha}_1\boldsymbol{\alpha}_1^{\mathrm{T}}+\lambda_2\boldsymbol{\alpha}_2\boldsymbol{\alpha}_2^{\mathrm{T}}+\cdots+\lambda_n\boldsymbol{\alpha}_n\boldsymbol{\alpha}_n^{\mathrm{T}}.$$

+++

#### 拓展解答 (1) 设 $\boldsymbol{A}$ 是 $3$ 阶实对称矩阵，存在可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\mathrm{diag}(1,2,-1)$，且 $\boldsymbol{\alpha}_1=(1,k+1,2)^{\mathrm{T}}$，$\boldsymbol{\alpha}_2=(k-1,-k,1)^{\mathrm{T}}$ 分别为 $\boldsymbol{A}$ 的特征值 $\lambda_1=1,\lambda_2=2$ 的特征向量，$\boldsymbol{A}^{*}$ 的特征值 $\lambda_0$ 对应的特征向量 $\boldsymbol{\beta}=(2,-5k,2k+1)^{\mathrm{T}}$．（Ⅰ）求 $\lambda_0$ 与 $k$ 的值；（Ⅱ）求矩阵 $(\boldsymbol{A}^{-1})^{*}$．
***
（Ⅰ）设 $\lambda_3=-1$ 对应的特征向量为 $\boldsymbol{\alpha}_3=(x_1,x_2,x_3)^{\mathrm{T}}$，由 $\boldsymbol{A}$ 是实对称矩阵，知 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 两两正交，故

$$\begin{cases}\boldsymbol{\alpha}_1^{\mathrm{T}}\boldsymbol{\alpha}_2=k-1-k(k+1)+2=0,&①\\ \boldsymbol{\alpha}_1^{\mathrm{T}}\boldsymbol{\alpha}_3=x_1+(k+1)x_2+2x_3=0,&②\\ \boldsymbol{\alpha}_2^{\mathrm{T}}\boldsymbol{\alpha}_3=(k-1)x_1-kx_2+x_3=0,&③\end{cases}$$

由 ① 解得 $k=1$ 或 $k=-1$．

当 $k=1$ 时，由 ②③ 解得 $\boldsymbol{\alpha}_3=(-4,1,1)^{\mathrm{T}}$，且

$$\boldsymbol{\alpha}_1=(1,2,2)^{\mathrm{T}},\boldsymbol{\alpha}_2=(0,-1,1)^{\mathrm{T}},\boldsymbol{\beta}=(2,-5,3)^{\mathrm{T}}.$$

又由已知 $\boldsymbol{A}^{*}\boldsymbol{\beta}=\lambda_0\boldsymbol{\beta}$，两边同时左乘 $\boldsymbol{A}$，得 $\boldsymbol{A}\boldsymbol{A}^{*}\boldsymbol{\beta}=\lambda_0\boldsymbol{A}\boldsymbol{\beta}$，$|\boldsymbol{A}|\boldsymbol{\beta}=\lambda_0\boldsymbol{A}\boldsymbol{\beta}$，即

$$\boldsymbol{A}\boldsymbol{\beta}=\frac{|\boldsymbol{A}|}{\lambda_0}\boldsymbol{\beta}=-\frac{2}{\lambda_0}\boldsymbol{\beta}\quad(|\boldsymbol{A}|=\lambda_1\lambda_2\lambda_3=-2),$$

故 $\boldsymbol{\beta}$ 应是 $\boldsymbol{A}$ 的特征向量，但 $\boldsymbol{\beta}$ 与 $\boldsymbol{A}$ 的特征向量 $\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3$ 任一个都不共线，即 $\boldsymbol{\beta}$ 不是 $\boldsymbol{A}$ 的特征向量，所以 $k=1$ 不合题意，舍去．

当 $k=-1$ 时，$\boldsymbol{\alpha}_1=(1,0,2)^{\mathrm{T}}$，且

$$\boldsymbol{\alpha}_2=(-2,1,1)^{\mathrm{T}},\quad\boldsymbol{\alpha}_3=(-2,-5,1)^{\mathrm{T}},\quad\boldsymbol{\beta}=(2,5,-1)^{\mathrm{T}},$$

故 $\boldsymbol{A}\boldsymbol{\alpha}_3=\lambda_3\boldsymbol{\alpha}_3=-\boldsymbol{\alpha}_3$，两边同时左乘 $\boldsymbol{A}^{*}$，得 $\boldsymbol{A}^{*}\boldsymbol{A}\boldsymbol{\alpha}_3=-\boldsymbol{A}^{*}\boldsymbol{\alpha}_3$，即 $|\boldsymbol{A}|\boldsymbol{\alpha}_3=-\boldsymbol{A}^{*}\boldsymbol{\alpha}_3$，又 $\boldsymbol{\alpha}_3=-\boldsymbol{\beta}$，$|\boldsymbol{A}|=-2$，故

$$-2(-\boldsymbol{\beta})=-\boldsymbol{A}^{*}(-\boldsymbol{\beta}),$$

即 $\boldsymbol{A}^{*}\boldsymbol{\beta}=2\boldsymbol{\beta}$，所以 $\lambda_0=2,k=-1$．

（Ⅱ）

$$\boldsymbol{A}=\boldsymbol{P}\begin{pmatrix}1&&\\&2&\\&&-1\end{pmatrix}\boldsymbol{P}^{-1}=\begin{pmatrix}1&-2&-2\\0&1&-5\\2&1&1\end{pmatrix}\begin{pmatrix}1&&\\&2&\\&&-1\end{pmatrix}\begin{pmatrix}1&-2&-2\\0&1&-5\\2&1&1\end{pmatrix}^{-1}=\begin{pmatrix}\dfrac{7}{5}&-1&-\dfrac{1}{5}\\-1&-\dfrac{1}{2}&\dfrac{1}{2}\\-\dfrac{1}{5}&\dfrac{1}{2}&\dfrac{11}{10}\end{pmatrix},$$

故 $(\boldsymbol{A}^{-1})^{*}=\dfrac{\boldsymbol{A}}{|\boldsymbol{A}|}=-\dfrac{1}{2}\boldsymbol{A}$．

+++

#### 拓展解答 (2) 设 $\boldsymbol{A}=\begin{pmatrix}k&-2&2\\-3&3&-1\\-15&8&-6\end{pmatrix}$，$\boldsymbol{B}=\begin{pmatrix}1&0&2\\0&2&0\\0&4&-1\end{pmatrix}$，且 $\boldsymbol{A}\sim\boldsymbol{B}$，求 $k$ 的值及可逆矩阵 $\boldsymbol{P}$，使得 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$．
***
由 $\boldsymbol{A}\sim\boldsymbol{B}$，知 $\boldsymbol{A},\boldsymbol{B}$ 有相同的迹，即

$$k+3+(-6)=1+2+(-1),$$

解得 $k=5$．由

$$|\lambda\boldsymbol{E}-\boldsymbol{B}|=\begin{vmatrix}\lambda-1&0&-2\\0&\lambda-2&0\\0&-4&\lambda+1\end{vmatrix}=(\lambda-1)(\lambda-2)(\lambda+1)=0,$$

得 $\boldsymbol{B}$ 的三个不同特征值分别为 $\lambda_1=1,\lambda_2=2,\lambda_3=-1$，由此可知，$\boldsymbol{B}$ 相似于对角矩阵．

由 $(1\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\alpha}_1=(1,0,0)^{\mathrm{T}}$；

由 $(2\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\alpha}_2=(8,3,4)^{\mathrm{T}}$；

由 $(-\boldsymbol{E}-\boldsymbol{B})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\alpha}_3=(1,0,-1)^{\mathrm{T}}$．

令 $\boldsymbol{P}_1=(\boldsymbol{\alpha}_1,\boldsymbol{\alpha}_2,\boldsymbol{\alpha}_3)$，则

$$\boldsymbol{P}_1^{-1}\boldsymbol{B}\boldsymbol{P}_1=\begin{pmatrix}1&0&0\\0&2&0\\0&0&-1\end{pmatrix}=\boldsymbol{\Lambda}.$$

又由于 $\boldsymbol{A}\sim\boldsymbol{B}$，故 $1,2,-1$ 也是 $\boldsymbol{A}$ 的特征值．

由 $(1\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\beta}_1=(1,1,-1)^{\mathrm{T}}$；

由 $(2\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\beta}_2=(0,1,1)^{\mathrm{T}}$；

由 $(-\boldsymbol{E}-\boldsymbol{A})\boldsymbol{x}=\boldsymbol{0}$，得特征向量 $\boldsymbol{\beta}_3=(1,0,-3)^{\mathrm{T}}$．

令 $\boldsymbol{P}_2=(\boldsymbol{\beta}_1,\boldsymbol{\beta}_2,\boldsymbol{\beta}_3)$，则

$$\boldsymbol{P}_2^{-1}\boldsymbol{A}\boldsymbol{P}_2=\begin{pmatrix}1&0&0\\0&2&0\\0&0&-1\end{pmatrix}=\boldsymbol{\Lambda}.$$

综上可得，$\boldsymbol{P}_2^{-1}\boldsymbol{A}\boldsymbol{P}_2=\boldsymbol{P}_1^{-1}\boldsymbol{B}\boldsymbol{P}_1$，即 $(\boldsymbol{P}_2\boldsymbol{P}_1^{-1})^{-1}\boldsymbol{A}(\boldsymbol{P}_2\boldsymbol{P}_1^{-1})=\boldsymbol{B}$，故 $\boldsymbol{P}^{-1}\boldsymbol{A}\boldsymbol{P}=\boldsymbol{B}$，其中

$$\boldsymbol{P}=\boldsymbol{P}_2\boldsymbol{P}_1^{-1}=\begin{pmatrix}1&0&1\\1&1&0\\-1&1&-3\end{pmatrix}\begin{pmatrix}1&8&1\\0&3&0\\0&4&-1\end{pmatrix}^{-1}=\begin{pmatrix}1&-\dfrac{8}{3}&0\\1&-\dfrac{11}{3}&1\\-1&\dfrac{1}{3}&2\end{pmatrix}.$$
