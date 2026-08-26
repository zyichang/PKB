---
quizify:
  format: 1
  deck: Math_880::Chapter_11
  tags: [Math, 880题, 数一, 第十一章, 矩阵]
---

+++

#### 基础选择 (1) 设 $A=(a_{ij})_{3\times 3}$，$B=\begin{pmatrix}a_{21}&a_{22}+a_{23}&a_{23}\\a_{31}&a_{32}+a_{33}&a_{33}\\a_{11}&a_{12}+a_{13}&a_{13}\end{pmatrix}$，$P=\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}$，$Q=\begin{pmatrix}1&0&0\\0&1&0\\0&1&1\end{pmatrix}$，则 $B=$（　）．

;;;
A. $AQP$
B. $PAQ$
C. $QAP$
D. $APQ$
;;;B
***
根据矩阵乘法及初等矩阵，得

$$PAQ=\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}\begin{pmatrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&0\\0&1&1\end{pmatrix}$$

$$=\begin{pmatrix}a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\\a_{11}&a_{12}&a_{13}\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&0\\0&1&1\end{pmatrix}=\begin{pmatrix}a_{21}&a_{22}+a_{23}&a_{23}\\a_{31}&a_{32}+a_{33}&a_{33}\\a_{11}&a_{12}+a_{13}&a_{13}\end{pmatrix}=B.$$

故 **B** 正确．

+++

#### 基础选择 (2) 设 $A$ 是 $n\ (n\geqslant 3)$ 阶可逆方阵，下列结论正确的是（　）．

① $(A^*)^{-1}=(A^{-1})^*$\
② $(kA)^*=k^{n-1}A^*\ (k\neq 0)$\
③ $(A^*)^{\mathrm{T}}=(A^{\mathrm{T}})^*$\
④ $(A^*)^*=|A|^{n-2}A$

;;;
A. ①②
B. ②③
C. ③④
D. ①②③④
;;;D
***
利用伴随矩阵的公式 $AA^*=A^*A=|A|E$，由 $A$ 可逆，知 $|A|\neq 0$，故

$$(A^*)^{-1}=\frac{A}{|A|}.$$

又 $A^{-1}(A^{-1})^*=|A^{-1}|E$，知 $(A^{-1})^*=\dfrac{A}{|A|}$，故 $(A^*)^{-1}=(A^{-1})^*=\dfrac{A}{|A|}$，结论 ① 正确．

由 $(kA)(kA)^*=|kA|E$，知

$$(kA)^*=k^n|A|\cdot(kA)^{-1}=k^n|A|\cdot\frac{1}{k}A^{-1}=k^{n-1}|A|A^{-1}=k^{n-1}A^*,$$

故结论 ② 正确．

由 $A^{\mathrm{T}}(A^{\mathrm{T}})^*=|A^{\mathrm{T}}|E=|A|E$，知 $(A^{\mathrm{T}})^*=|A|(A^{\mathrm{T}})^{-1}$，由

$$(AA^*)^{\mathrm{T}}=(A^*)^{\mathrm{T}}A^{\mathrm{T}}=(|A|E)^{\mathrm{T}}=|A|E,$$

知 $(A^*)^{\mathrm{T}}=|A|(A^{\mathrm{T}})^{-1}$，故 $(A^{\mathrm{T}})^*=(A^*)^{\mathrm{T}}$，结论 ③ 正确．

由 $A^*(A^*)^*=|A^*|E=|A|^{n-1}E$，知

$$(A^*)^*=|A|^{n-1}(A^*)^{-1}=|A|^{n-1}(A^{-1})^*=|A|^{n-1}\cdot|A^{-1}|\cdot(A^{-1})^{-1}=|A|^{n-2}A,$$

故结论 ④ 正确．

【注】① 对公式 $AA^*=A^*A=|A|E$，可以将 $A$ 替换成 $A^{-1},kA,A^*$ 衍生出更多的公式．\
② 三种运算 “$*$” “$-1$” “$\mathrm{T}$” 是可交换的．\
③ 常用结论：$(AB)^{-1}=B^{-1}A^{-1}$，$(AB)^{\mathrm{T}}=B^{\mathrm{T}}A^{\mathrm{T}}$，$(AB)^*=B^*A^*$．

+++

#### 基础选择 (3) 设 $A=\begin{pmatrix}1&0&1\\2&1&0\\-3&2&-5\end{pmatrix}$，则行列式 $\left|\left[(E-A)^*\right]^{-1}\right|=$（　）．

;;;
A. $\dfrac{1}{4}$
B. $-\dfrac{1}{4}$
C. $\dfrac{1}{16}$
D. $-\dfrac{1}{16}$
;;;C
***
$$\left[(E-A)^*\right]^{-1}=\left[|E-A|(E-A)^{-1}\right]^{-1}$$

$$=\frac{1}{|E-A|}(E-A)=\begin{pmatrix}0&0&\dfrac{1}{4}\\[2pt]\dfrac{1}{2}&0&0\\[2pt]-\dfrac{3}{4}&\dfrac{1}{2}&-\dfrac{3}{2}\end{pmatrix},$$

由分块矩阵的行列式，知 $\left|\left[(E-A)^*\right]^{-1}\right|=(-1)^{1\times 2}\times\dfrac{1}{4}\times\dfrac{1}{4}=\dfrac{1}{16}$，故 **C** 正确．

+++

#### 基础选择 (4) 设矩阵 $A=\begin{pmatrix}1&1&1\\0&1&0\\2&k&3\\k-1&5&1\end{pmatrix}$ 与 $B=\begin{pmatrix}1&1&1\\0&1&-1\\2&3&k\\3&5&1\end{pmatrix}$ 等价，则（　）．

;;;
A. $k=1$
B. $k\neq 1$
C. $k=-1$
D. $k\neq -1$
;;;B
***
同型矩阵 $A$ 与 $B$ 等价的充分必要条件是 $r(A)=r(B)$．

由于在矩阵 $A$ 中，有 $3$ 阶子式 $\begin{vmatrix}1&1&1\\0&1&0\\2&k&3\end{vmatrix}=\begin{vmatrix}1&1\\2&3\end{vmatrix}=1\neq 0$，故 $r(A)=3$．

对矩阵 $B$ 作初等变换，得

$$B=\begin{pmatrix}1&1&1\\0&1&-1\\2&3&k\\3&5&1\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1\\0&1&-1\\0&1&k-2\\0&2&-2\end{pmatrix}\rightarrow\begin{pmatrix}1&1&1\\0&1&-1\\0&0&k-1\\0&0&0\end{pmatrix},$$

故由 $r(A)=r(B)=3$，知 $k\neq 1$．

+++

#### 基础填空 (1) 设 $\alpha=(1,2,3)^{\mathrm{T}}$，$\beta=\left(1,\dfrac{1}{2},\dfrac{1}{3}\right)^{\mathrm{T}}$，$A=\alpha\beta^{\mathrm{T}}$，则 $A^n=$ ________．
***
$3^{n-1}\begin{pmatrix}1&\dfrac{1}{2}&\dfrac{1}{3}\\[2pt]2&1&\dfrac{2}{3}\\[2pt]3&\dfrac{3}{2}&1\end{pmatrix}$．

由 $A=\alpha\beta^{\mathrm{T}}$，知 $r(A)=1$，$k=\beta^{\mathrm{T}}\alpha=3$，故

$$A^n=k^{n-1}A=3^{n-1}\begin{pmatrix}1&\dfrac{1}{2}&\dfrac{1}{3}\\[2pt]2&1&\dfrac{2}{3}\\[2pt]3&\dfrac{3}{2}&1\end{pmatrix}.$$

+++

#### 基础填空 (2) 设 $\alpha=(2,-1,3)^{\mathrm{T}}$，$\beta=(1,2,0)^{\mathrm{T}}$，$A=\alpha\beta^{\mathrm{T}}$，$E$ 是 $3$ 阶单位矩阵，则 $(A+E)^n=$ ________．
***
$\begin{pmatrix}2n+1&4n&0\\-n&-2n+1&0\\3n&6n&1\end{pmatrix}$．

由于

$$A^2=(\alpha\beta^{\mathrm{T}})(\alpha\beta^{\mathrm{T}})=\alpha(\beta^{\mathrm{T}}\alpha)\beta^{\mathrm{T}},$$

且 $\beta^{\mathrm{T}}\alpha=(1,2,0)\begin{pmatrix}2\\-1\\3\end{pmatrix}=0$，故 $A^2=O$．

又因为

$$A=\begin{pmatrix}2\\-1\\3\end{pmatrix}(1,2,0)=\begin{pmatrix}2&4&0\\-1&-2&0\\3&6&0\end{pmatrix},$$

所以

$$(A+E)^n=E^n+\mathrm{C}_n^1E^{n-1}A=E+nA=\begin{pmatrix}2n+1&4n&0\\-n&-2n+1&0\\3n&6n&1\end{pmatrix}.$$

+++

#### 基础填空 (3) 设 $A=\begin{pmatrix}1&0&1\\0&2&0\\1&0&1\end{pmatrix}$，则 $A^n=$ ________．
***
$\begin{pmatrix}2^{n-1}&0&2^{n-1}\\0&2^n&0\\2^{n-1}&0&2^{n-1}\end{pmatrix}$．

$r(A)=2$，先求 $A^2$，找出 $A^n$ 的规律．

$$A^2=\begin{pmatrix}1&0&1\\0&2&0\\1&0&1\end{pmatrix}\begin{pmatrix}1&0&1\\0&2&0\\1&0&1\end{pmatrix}=\begin{pmatrix}2&0&2\\0&4&0\\2&0&2\end{pmatrix}=2A,$$

即 $A^2=2A$，从而 $A^3=2A^2=2^2A,\cdots,A^n=2^{n-1}A$，故

$$A^n=\begin{pmatrix}2^{n-1}&0&2^{n-1}\\0&2^n&0\\2^{n-1}&0&2^{n-1}\end{pmatrix}.$$

+++

#### 基础填空 (4) 设 $B=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}$，$A=P^{-1}BP$，则 $A^4-2B^2=$ ________．
***
$\begin{pmatrix}3&0&0\\0&3&0\\0&0&-1\end{pmatrix}$．

由 $A=P^{-1}BP$，有 $A^2=P^{-1}BP\cdot P^{-1}BP=P^{-1}B^2P$，一般地，有 $A^n=P^{-1}B^nP$，所以 $A^4=P^{-1}B^4P$．

由 $B=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}$，得 $B^2=\begin{pmatrix}-1&0&0\\0&-1&0\\0&0&1\end{pmatrix}$，故 $B^4=(B^2)^2=E$，所以 $A^4=P^{-1}EP=E$，于是

$$A^4-2B^2=E-2B^2=\begin{pmatrix}3&0&0\\0&3&0\\0&0&-1\end{pmatrix}.$$

+++

#### 基础填空 (5) 设 $A$ 是 $n$ 阶方阵，且 $|A|=2$，将 $A$ 的第 $i$ 行与第 $j$ 行互换得到 $B$，则行列式 $\left|B^{-1}B^*B^{\mathrm{T}}\right|=$ ________．
***
$(-2)^{n-1}$．

依题设，$B=E_{i,j}A$，则 $|B|=|E_{i,j}||A|=-|A|=-2$，故

$$\left|B^{-1}B^*B^{\mathrm{T}}\right|=|B^{-1}||B^*||B^{\mathrm{T}}|=|B|^{-1}|B|^{n-1}\cdot|B|=|B|^{n-1}=(-2)^{n-1}.$$

+++

#### 基础填空 (6) 设 $A=\begin{pmatrix}1&2&3&4\\2&3&4&5\\3&4&5&6\\4&5&6&7\end{pmatrix}$，则 $r(A)=$ ________．
***
$2$．

利用初等行变换化 $A$ 为阶梯形，

$$A=\begin{pmatrix}1&2&3&4\\2&3&4&5\\3&4&5&6\\4&5&6&7\end{pmatrix}\longrightarrow\begin{pmatrix}1&2&3&4\\0&-1&-2&-3\\0&0&0&0\\0&0&0&0\end{pmatrix},$$

故 $r(A)=2$．

+++

#### 基础填空 (7) 若 $A^n=O$，$n$ 为正整数，则 $(E-A)^{-1}=$ ________．
***
$E+A+A^2+\cdots+A^{n-1}$．

用可逆矩阵的定义，并注意到 $A^n=O$，

$$(E-A)(E+A+A^2+\cdots+A^{n-1})=E,$$

故

$$(E-A)^{-1}=E+A+A^2+\cdots+A^{n-1}.$$

【注】由 $A^n=O$，则化零多项式为 $x^n$．用多项式除法，即用 $x^n$ 除以 $x-1$，也可求 $(E-A)^{-1}$（计算量大）．

+++

#### 基础填空 (8) 若 $A^n=E$，$n$ 为正整数，则 $(A^*)^n=$ ________．
***
$E$．

由 $A^n=E$，知 $|A|^n=1$．

又 $A^*A=AA^*=|A|E$，得 $(AA^*)^n=(AA^*)(AA^*)\cdots(AA^*)=|A|^nE$．

因 $A$ 与 $A^*$ 可交换，故 $(AA^*)^n=A^n(A^*)^n=|A|^nE=E$，于是 $(A^*)^n=E$．

【注】伴随矩阵的常用计算公式：$AA^*=A^*A=|A|E$．

+++

#### 基础填空 (9) 设方阵 $A$ 满足 $A^2-3A-2E=O$，则 $A^{-1}=$ ________．
***
$\dfrac{1}{2}(A-3E)$．

利用可逆矩阵的定义．

由 $A^2-3A-2E=O$，得 $A(A-3E)=2E$，即 $A\cdot\dfrac{1}{2}(A-3E)=E$，故

$$A^{-1}=\frac{1}{2}(A-3E).$$

+++

#### 基础填空 (10) 设方阵 $A$ 满足 $A^2=A$，则 $(A+E)^{-1}=$ ________．
***
$-\dfrac{1}{2}(A-2E)$．

由 $A^2=A$，知 $A^2-A-2E+2E=O$，即 $(A+E)(A-2E)=-2E$，故

$$(A+E)^{-1}=-\frac{1}{2}(A-2E).$$

【注】下列解法是错误的：\
由 $A^2=A$，得 $A(A-E)=O$，于是当 $A=O$ 时，$(A+E)^{-1}=E^{-1}=E$；当 $A=E$ 时，$(A+E)^{-1}=(2E)^{-1}=\dfrac{1}{2}E$．

错误原因在于忽略了矩阵运算与数的运算的区别：由 $AB=O$ 不能得出 $A=O$ 或 $B=O$．

+++

#### 基础填空 (11) 设 $A$ 是 $n$ 阶可逆矩阵，将 $A$ 的第 $i$ 行和第 $j$ 行交换得 $B$，则行列式 $\left|AB^{-1}\right|=$ ________．
***
$-1$．

依题意，$B=E_{i,j}A$，$E_{i,j}$ 为单位矩阵 $E$ 交换第 $i,j$ 行后所得的初等矩阵，则

$$AB^{-1}=A(E_{i,j}A)^{-1}=AA^{-1}E_{i,j}^{-1}=E_{i,j}^{-1}=E_{i,j},$$

故 $\left|AB^{-1}\right|=|E_{i,j}|=-1$．

+++

#### 基础填空 (12) 设存在 $3$ 阶矩阵 $A$，对任意的 $x,y,z$ 有 $A\begin{pmatrix}x\\y\\z\end{pmatrix}=\begin{pmatrix}z\\x\\y\end{pmatrix}$，则 $A=$ ________．
***
$\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$．

依题设，有

$$\begin{pmatrix}x\\y\\z\end{pmatrix}\xrightarrow{\ \text{交换}1,2\text{行}\ }\begin{pmatrix}y\\x\\z\end{pmatrix}\xrightarrow{\ \text{交换}1,3\text{行}\ }\begin{pmatrix}z\\x\\y\end{pmatrix},$$

故

$$A=E_{1,3}\cdot E_{1,2}=\begin{pmatrix}0&0&1\\0&1&0\\1&0&0\end{pmatrix}\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}.$$

+++

#### 基础填空 (13) 设 $\alpha=(k,0,\cdots,0,k)^{\mathrm{T}}\ (k\neq 0)$，且 $A=E-\alpha\alpha^{\mathrm{T}}$，$A^{-1}=E+\dfrac{1}{k}\alpha\alpha^{\mathrm{T}}$，则 $k=$ ________．
***
$-1$ 或 $\dfrac{1}{2}$．

$$AA^{-1}=(E-\alpha\alpha^{\mathrm{T}})\left(E+\frac{1}{k}\alpha\alpha^{\mathrm{T}}\right)=E-\alpha\alpha^{\mathrm{T}}+\frac{1}{k}\alpha\alpha^{\mathrm{T}}-\frac{1}{k}\alpha\alpha^{\mathrm{T}}\alpha\alpha^{\mathrm{T}}.$$

而 $\alpha^{\mathrm{T}}\alpha=2k^2$，故

$$AA^{-1}=E+\left(-1+\frac{1}{k}-\frac{2k^2}{k}\right)\alpha\alpha^{\mathrm{T}}=E,$$

于是 $-1+\dfrac{1}{k}-2k=0$，解得 $k=-1$ 或 $k=\dfrac{1}{2}$．

+++

#### 基础解答 (1) 设 $A=\begin{pmatrix}2&-1&3\\a&1&b\\4&c&6\end{pmatrix}$，且 $BA=O$，$B$ 是 $3$ 阶方阵，$r(B)>1$，求 $A^n$．
***
由 $BA=O$，知 $r(A)+r(B)\leqslant 3$．由 $r(B)>1$，得 $r(A)\leqslant 3-r(B)\leqslant 1$．显然 $r(A)\geqslant 1$，故 $r(A)=1$，所以 $A$ 的行向量成比例，即

$$\frac{a}{2}=\frac{1}{-1}=\frac{b}{3},\quad \frac{2}{4}=\frac{-1}{c}=\frac{3}{6},$$

解得 $a=-2$，$b=-3$，$c=-2$，故

$$A=\begin{pmatrix}2&-1&3\\-2&1&-3\\4&-2&6\end{pmatrix}=\begin{pmatrix}1\\-1\\2\end{pmatrix}(2,-1,3)\xlongequal{\text{记}}\alpha\beta^{\mathrm{T}},$$

则 $\beta^{\mathrm{T}}\alpha=9$，于是

$$A^n=9^{n-1}A=9^{n-1}\begin{pmatrix}2&-1&3\\-2&1&-3\\4&-2&6\end{pmatrix}.$$

【注】结论：\
① $r(A)=1\Leftrightarrow A=\alpha\beta^{\mathrm{T}}$（$\alpha,\beta$ 为非零列向量）；\
② $r(A)=1\Rightarrow A^n=k^{n-1}A$，其中 $k=\beta^{\mathrm{T}}\alpha=\sum\limits_{i=1}^{n}a_{ii}=\sum\limits_{i=1}^{n}\lambda_i\ (i=1,2,\cdots,n)$，$\lambda_i$ 为 $A$ 的特征值．

+++

#### 基础解答 (2) 设 $\alpha,\beta$ 是 $n$ 维列向量，且 $\alpha^{\mathrm{T}}\beta=2$，证明：$A=E+\alpha\beta^{\mathrm{T}}$ 可逆，并求 $A^{-1}$．
***
$$A^2=(E+\alpha\beta^{\mathrm{T}})(E+\alpha\beta^{\mathrm{T}})=E+\alpha\beta^{\mathrm{T}}+\alpha\beta^{\mathrm{T}}+\alpha(\beta^{\mathrm{T}}\alpha)\beta^{\mathrm{T}}$$

$$=E+4\alpha\beta^{\mathrm{T}}=4E+4\alpha\beta^{\mathrm{T}}-3E=4A-3E,$$

即 $A(A-4E)=-3E$，故 $A$ 可逆，且 $A^{-1}=\dfrac{4E-A}{3}$．

【注】结论：设 $\alpha,\beta$ 为 $n$ 维列向量，$k_1\neq 0$，$\beta^{\mathrm{T}}\alpha\neq\dfrac{1}{k_1}$，则 $A=E-k_1\alpha\beta^{\mathrm{T}}$ 可逆，且

$$A^{-1}=E-k_2\alpha\beta^{\mathrm{T}},$$

其中 $k_1,k_2$ 满足 $\beta^{\mathrm{T}}\alpha=\dfrac{1}{k_1}+\dfrac{1}{k_2}$．（见《李林考研数学系列线性代数辅导讲义》第二章）

+++

#### 基础解答 (3) 设 $A^{-1}=\begin{pmatrix}1&1&1\\1&2&1\\1&1&3\end{pmatrix}$，求 $(A^*)^{-1}$．
***
$(A^*)^{-1}=(A^{-1})^*$，又 $A^{-1}(A^{-1})^*=|A^{-1}|E$，故 $(A^{-1})^*=|A^{-1}|A$．

而 $|A^{-1}|=\begin{vmatrix}1&1&1\\1&2&1\\1&1&3\end{vmatrix}=2$，对 $A^{-1}$ 用初等行变换求 $A$，

$$\left(\begin{array}{ccc|ccc}1&1&1&1&0&0\\1&2&1&0&1&0\\1&1&3&0&0&1\end{array}\right)\longrightarrow\left(\begin{array}{ccc|ccc}1&1&1&1&0&0\\0&1&0&-1&1&0\\0&0&2&-1&0&1\end{array}\right)\longrightarrow\left(\begin{array}{ccc|ccc}1&0&0&\dfrac{5}{2}&-1&-\dfrac{1}{2}\\0&1&0&-1&1&0\\0&0&1&-\dfrac{1}{2}&0&\dfrac{1}{2}\end{array}\right),$$

故 $A=\begin{pmatrix}\dfrac{5}{2}&-1&-\dfrac{1}{2}\\[2pt]-1&1&0\\[2pt]-\dfrac{1}{2}&0&\dfrac{1}{2}\end{pmatrix}$，所以

$$(A^*)^{-1}=(A^{-1})^*=|A^{-1}|\cdot A=\begin{pmatrix}5&-2&-1\\-2&2&0\\-1&0&1\end{pmatrix}.$$

+++

#### 基础解答 (4) 设 $A=\begin{pmatrix}2&1&1\\1&2&1\\1&1&2\end{pmatrix}$，证明：$A^2=5A-4E$，并求 $A^{-1}$．
***
$A$ 是对称矩阵，将 $A$ 拆成两个矩阵，$A=E+\begin{pmatrix}1&1&1\\1&1&1\\1&1&1\end{pmatrix}=E+\alpha\alpha^{\mathrm{T}}$，其中 $\alpha=(1,1,1)^{\mathrm{T}}$，故

$$A^2=(E+\alpha\alpha^{\mathrm{T}})^2=E+2\alpha\alpha^{\mathrm{T}}+\alpha\alpha^{\mathrm{T}}\alpha\alpha^{\mathrm{T}}=E+2\alpha\alpha^{\mathrm{T}}+3\alpha\alpha^{\mathrm{T}}$$

$$=E+5\alpha\alpha^{\mathrm{T}}=5E+5\alpha\alpha^{\mathrm{T}}-4E=5A-4E.$$

又由 $A^2-5A=A(A-5E)=-4E$，知

$$A^{-1}=\frac{A-5E}{-4}=\begin{pmatrix}\dfrac{3}{4}&-\dfrac{1}{4}&-\dfrac{1}{4}\\[2pt]-\dfrac{1}{4}&\dfrac{3}{4}&-\dfrac{1}{4}\\[2pt]-\dfrac{1}{4}&-\dfrac{1}{4}&\dfrac{3}{4}\end{pmatrix}.$$

+++

#### 基础解答 (5) 设方阵 $A,B$ 满足 $|B|\neq 0$，$(A-E)^{-1}=(B-E)^{\mathrm{T}}$，求 $A^{-1}$（用 $B$ 表示）．
***
考虑到 $(A-E)^{-1}$ 无公式可用，在已知等式两边同时乘以 $(A-E)$．

依题意，$(A-E)^{-1}=(B-E)^{\mathrm{T}}=B^{\mathrm{T}}-E$，等式两边同时乘以 $(A-E)$，得

$$(A-E)(A-E)^{-1}=(A-E)(B^{\mathrm{T}}-E),$$

故 $E=AB^{\mathrm{T}}-A-B^{\mathrm{T}}+E$，即 $A(B^{\mathrm{T}}-E)=B^{\mathrm{T}}$．

由 $|B|\neq 0$，知 $|B^{\mathrm{T}}|\neq 0$，故 $B^{\mathrm{T}}$ 可逆，于是 $A(B^{\mathrm{T}}-E)(B^{\mathrm{T}})^{-1}=B^{\mathrm{T}}\cdot(B^{\mathrm{T}})^{-1}=E$，所以

$$A^{-1}=(B^{\mathrm{T}}-E)(B^{\mathrm{T}})^{-1}=E-(B^{\mathrm{T}})^{-1}.$$

+++

#### 基础解答 (6) 设 $A=\begin{pmatrix}1&0&0\\2&3&0\\0&4&5\end{pmatrix}$，$B=(E+A)^{-1}(E-A)$，求 $\left[(E+B)^2\right]^{-1}$．
***
由于 $\left[(E+B)^2\right]^{-1}=\left[(E+B)^{-1}\right]^2$，且

$$(E+B)^{-1}=\left[E+(E+A)^{-1}(E-A)\right]^{-1}$$

$$=\left[(E+A)^{-1}(E+A)+(E+A)^{-1}(E-A)\right]^{-1}$$

$$=\left[(E+A)^{-1}(E+A+E-A)\right]^{-1}=\left[2(E+A)^{-1}\right]^{-1}$$

$$=\frac{1}{2}(E+A)=\frac{1}{2}\begin{pmatrix}2&0&0\\2&4&0\\0&4&6\end{pmatrix}=\begin{pmatrix}1&0&0\\1&2&0\\0&2&3\end{pmatrix},$$

故

$$\left[(E+B)^2\right]^{-1}=\left[(E+B)^{-1}\right]^2=\begin{pmatrix}1&0&0\\1&2&0\\0&2&3\end{pmatrix}^2=\begin{pmatrix}1&0&0\\3&4&0\\2&10&9\end{pmatrix}.$$

+++

#### 基础解答 (7) 已知方阵 $A,B,(A+B)$ 均可逆，求 $(A^{-1}+B^{-1})^{-1}$．
***
求抽象矩阵的逆，常用可逆的定义与 $(AB)^{-1}=B^{-1}A^{-1}$．

$$A^{-1}+B^{-1}=A^{-1}(E+AB^{-1})=A^{-1}(BB^{-1}+AB^{-1})=A^{-1}(B+A)B^{-1},$$

故由已知条件，知 $A^{-1}+B^{-1}$ 可逆，且

$$(A^{-1}+B^{-1})^{-1}=\left[A^{-1}(B+A)B^{-1}\right]^{-1}=B(A+B)^{-1}A.$$

【注】由于 $A^{-1}(A+B)B^{-1}=B^{-1}(A+B)A^{-1}$，等式两边同时取逆，故

$$B(A+B)^{-1}A=A(A+B)^{-1}B,$$

即本题的答案还可以写成 $A(A+B)^{-1}B$．

+++

#### 基础解答 (8) 设 $AB=BA$，$A$ 可逆，证明：$A^{-1}B=BA^{-1}$．
***
由 $AB=BA$，得 $A^{-1}(AB)A^{-1}=A^{-1}(BA)A^{-1}$，故

$$A^{-1}(AB)A^{-1}=(A^{-1}A)BA^{-1}=BA^{-1},$$

$$A^{-1}(BA)A^{-1}=A^{-1}B(AA^{-1})=A^{-1}B,$$

于是 $A^{-1}B=BA^{-1}$（即 $A^{-1}$ 与 $B$ 可交换）．

+++

#### 基础解答 (9) 设 $A,B$ 都是 $n$ 阶方阵，且 $A^2=A$，$B^2=B$，$(A+B)^2=A+B$，证明：$AB=BA$．
***
由已知，

$$(A+B)^2=A^2+AB+BA+B^2=A+AB+BA+B=A+B,$$

故

$$AB+BA=O.\qquad ①$$

① 式左乘 $A$，得 $A^2B+ABA=AB+ABA=O$．　②

① 式右乘 $A$，得 $ABA+BA^2=ABA+BA=O$．　③

由 ②③ 式，可知 $AB=-ABA=BA$．

【注】① 下列解法是错误的：\
由 $(A+B)^2=A^2+2AB+B^2=A+2AB+B=A+B$，及 $(A+B)^2=(B+A)^2=B^2+2BA+A^2=B+2BA+A=A+B$，故 $AB=BA=O$．

错误原因是矩阵乘法没有交换律，也没有消去律．

② 由 $AB=BA$ 可得 $(AB)^2=A^2B^2$，但反之不一定成立．例如 $A=\begin{pmatrix}1&0\\0&0\end{pmatrix}$，$B=\begin{pmatrix}0&1\\0&0\end{pmatrix}$，满足 $(AB)^2=A^2B^2$，但 $AB\neq BA$．

+++

#### 基础解答 (10) 设 $A$ 为 $2n+1$ 阶正交矩阵，且 $|A|=1$，证明：$A-E$ 不可逆．
***
只要证 $|A-E|=0$，由 $A$ 是正交矩阵，知 $AA^{\mathrm{T}}=A^{\mathrm{T}}A=E$，所以

$$|A-E|=|A(E-A^{\mathrm{T}})|=|A||E-A^{\mathrm{T}}|$$

$$=|A|\left|(E-A)^{\mathrm{T}}\right|=|A||E-A|$$

$$=|-(A-E)|=(-1)^{2n+1}|A-E|=-|A-E|,$$

故 $|A-E|=0$，所以 $A-E$ 不可逆．

+++

#### 基础解答 (11) 设 $n$ 阶方阵 $A,B$ 满足 $A^2=E$，$B^2=E$，且 $|A|+|B|=0$，证明：$A+B$ 不可逆．
***
由已知，只要证明 $|A+B|=0$．

由 $A^2=E$，$B^2=E$，知 $|A^2|=|A|^2=|E|=1$，及 $|B^2|=|B|^2=|E|=1$，故 $|A|=\pm 1$，$|B|=\pm 1$，由 $|A|+|B|=0$，可知 $|A|$ 与 $|B|$ 异号．

而

$$|A+B|=|AB^2+A^2B|=|A(B+A)B|=|A||A+B||B|,$$

由于 $|A||B|=-1$，故 $|A+B|=-|A+B|$，所以 $|A+B|=0$，从而 $A+B$ 不可逆．

+++

#### 基础解答 (12) 设 $A=\begin{pmatrix}1&0&1\\0&2&0\\-1&0&1\end{pmatrix}$，$AB+E=A^2+B$，求 $B$．
***
由 $AB+E=A^2+B$，可得 $AB-B=A^2-E$，则 $(A-E)B=A^2-E$．

又由 $A-E=\begin{pmatrix}0&0&1\\0&1&0\\-1&0&0\end{pmatrix}$，可知 $A-E$ 可逆，故

$$B=(A-E)^{-1}(A^2-E)=(A-E)^{-1}(A-E)(A+E)=A+E=\begin{pmatrix}2&0&1\\0&3&0\\-1&0&2\end{pmatrix}.$$

【注】此题属于解矩阵方程，这类题分两类：\
① 将复杂矩阵方程化简为下列三者之一：$AX=B$，$XA=B$，$AXB=C$，当 $A,B$ 可逆时，解得 $X=A^{-1}B$，$X=BA^{-1}$，$X=A^{-1}CB^{-1}$．\
② 当 $A$ 不可逆时，问题转化为解非齐次线性方程组．

+++

#### 基础解答 (13) 设 $A=\begin{pmatrix}0&2\\1&2\end{pmatrix}$，且 $(A^{\mathrm{T}}B^{-1})^{\mathrm{T}}-A(B^{\mathrm{T}}A)^{-1}=(E-B^{-1})^{\mathrm{T}}$，求 $B$．
***
由 $(A^{\mathrm{T}}B^{-1})^{\mathrm{T}}-A(B^{\mathrm{T}}A)^{-1}=(E-B^{-1})^{\mathrm{T}}$，得

$$(B^{-1})^{\mathrm{T}}A-A(A^{-1})(B^{\mathrm{T}})^{-1}=E^{\mathrm{T}}-(B^{-1})^{\mathrm{T}},$$

即 $(B^{-1})^{\mathrm{T}}A-(B^{\mathrm{T}})^{-1}+(B^{-1})^{\mathrm{T}}=E$．因为 $(B^{\mathrm{T}})^{-1}=(B^{-1})^{\mathrm{T}}$，所以 $(B^{\mathrm{T}})^{-1}=A^{-1}$，即

$$B^{\mathrm{T}}=A,\quad B=A^{\mathrm{T}}=\begin{pmatrix}0&1\\2&2\end{pmatrix}.$$

+++

#### 基础解答 (14) 设 $A=\begin{pmatrix}\dfrac{1}{3}&0&0\\[2pt]0&\dfrac{1}{4}&0\\[2pt]0&0&\dfrac{1}{7}\end{pmatrix}$，$A^{-1}BA=6A+BA$，求 $B$．
***
由 $A^{-1}BA=6A+BA$，得 $A^{-1}BA-BA=6A$，即 $(A^{-1}-E)BA=6A$．

由已知，$A$ 可逆，$A^{-1}-E$ 可逆，故 $B=(A^{-1}-E)^{-1}(6A)A^{-1}=6(A^{-1}-E)^{-1}$．

又

$$A^{-1}=\begin{pmatrix}3&0&0\\0&4&0\\0&0&7\end{pmatrix},\quad (A^{-1}-E)^{-1}=\begin{pmatrix}\dfrac{1}{2}&0&0\\[2pt]0&\dfrac{1}{3}&0\\[2pt]0&0&\dfrac{1}{6}\end{pmatrix},$$

故

$$B=6(A^{-1}-E)^{-1}=\begin{pmatrix}3&0&0\\0&2&0\\0&0&1\end{pmatrix}.$$

【注】设 $a_1,a_2,a_3$ 均不为零，则

$$\begin{pmatrix}a_1&0&0\\0&a_2&0\\0&0&a_3\end{pmatrix}^{-1}=\begin{pmatrix}\dfrac{1}{a_1}&0&0\\[2pt]0&\dfrac{1}{a_2}&0\\[2pt]0&0&\dfrac{1}{a_3}\end{pmatrix},\quad\begin{pmatrix}0&0&a_1\\0&a_2&0\\a_3&0&0\end{pmatrix}^{-1}=\begin{pmatrix}0&0&\dfrac{1}{a_3}\\[2pt]0&\dfrac{1}{a_2}&0\\[2pt]\dfrac{1}{a_1}&0&0\end{pmatrix}.$$

+++

#### 基础解答 (15) 设 $A=\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}$，$B=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}$，$C=\begin{pmatrix}1&-4&3\\2&0&-1\\1&-2&0\end{pmatrix}$，且 $AXB=C$，求矩阵 $X$．
***
$A$ 与 $B$ 为初等矩阵，故可逆，由 $AXB=C$，得 $X=A^{-1}CB^{-1}$，故

$$X=A^{-1}CB^{-1}=ACB$$

$$=\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&-4&3\\2&0&-1\\1&-2&0\end{pmatrix}\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}=\begin{pmatrix}2&-1&0\\1&3&-4\\1&0&-2\end{pmatrix}.$$

+++

#### 基础解答 (16) 设矩阵 $A$ 满足 $A\begin{pmatrix}1&2\\0&1\end{pmatrix}=\begin{pmatrix}2&1\\3&2\end{pmatrix}A$，求矩阵 $A$．
***
已知矩阵方程无法利用矩阵运算化简，则令 $A=\begin{pmatrix}x_1&x_2\\x_3&x_4\end{pmatrix}$，代入等式转化为解方程，有

$$\begin{pmatrix}x_1&x_2\\x_3&x_4\end{pmatrix}\begin{pmatrix}1&2\\0&1\end{pmatrix}=\begin{pmatrix}2&1\\3&2\end{pmatrix}\begin{pmatrix}x_1&x_2\\x_3&x_4\end{pmatrix},$$

即

$$\begin{pmatrix}x_1&2x_1+x_2\\x_3&2x_3+x_4\end{pmatrix}=\begin{pmatrix}2x_1+x_3&2x_2+x_4\\3x_1+2x_3&3x_2+2x_4\end{pmatrix},$$

比较两边对应元素，得

$$\begin{cases}x_1=2x_1+x_3,\\2x_1+x_2=2x_2+x_4,\\x_3=3x_1+2x_3,\\2x_3+x_4=3x_2+2x_4,\end{cases}$$

此方程组只有零解 $x_1=x_2=x_3=x_4=0$，故 $A=O$．

+++

#### 综合选择 (1) 设 $A=\begin{pmatrix}1&2&k\\1&k+1&1\\k&2&1\end{pmatrix}$，$B$ 是 $3$ 阶非零矩阵，且 $AB=O$，则（　）．

;;;
A. 当 $k=1$ 时，$r(B)=1$
B. 当 $k=-3$ 时，$r(B)=1$
C. 当 $k=1$ 时，$r(B)=2$
D. 当 $k=-3$ 时，$r(B)=2$
;;;B
***
由 $AB=O$ 知，$r(A)+r(B)\leqslant 3$．

若 $k=1$，则 $r(A)=1$，故 $r(B)\leqslant 2$，所以 $r(B)=1$ 或 $r(B)=2$，A，C 不正确．

若 $k=-3$，则 $r(A)=2$，故 $r(B)\leqslant 3-r(A)=1$，又 $B$ 是非零矩阵，故 $r(B)\geqslant 1$，从而 $r(B)=1$．

+++

#### 综合选择 (2) 设 $A=\begin{pmatrix}a&b&b\\b&a&b\\b&b&a\end{pmatrix}$（$a,b$ 均不为 $0$），且 $r(A^*)=1$，则必有（　）．

;;;
A. $a=b$
B. $a=b$ 或 $a+2b\neq 0$
C. $a+2b=0$
D. $a\neq b$ 且 $a+2b\neq 0$
;;;C
***
由 $r(A^*)=1$，知 $r(A)=n-1=3-1=2$，故 $|A|=0$．又

$$|A|=\begin{vmatrix}a&b&b\\b&a&b\\b&b&a\end{vmatrix}=(a+2b)\begin{vmatrix}1&0&0\\1&a-b&0\\1&0&a-b\end{vmatrix}=(a+2b)(a-b)^2=0,$$

得 $a+2b=0$ 或 $a=b$．

又当 $a=b$ 时，$r(A)=1\neq 2$，故 $a+2b=0$（由 $a,b$ 均不为零，可知 $a+2b=0$ 已经蕴含 $a\neq b$），故 **C** 正确．

【注】设 $A$ 是 $n$ 阶方阵，则

$$r(A^*)=\begin{cases}n\Leftrightarrow r(A)=n,\\1\Leftrightarrow r(A)=n-1,\\0\Leftrightarrow r(A)<n-1.\end{cases}$$

+++

#### 综合选择 (3) 设 $A=\begin{pmatrix}a_{11}&a_{12}&a_{13}\\a_{21}&a_{22}&a_{23}\\a_{31}&a_{32}&a_{33}\end{pmatrix}$，$P=\begin{pmatrix}0&0&1\\0&1&0\\1&0&0\end{pmatrix}$，且 $P^nAP^m=A$，则正整数 $n,m$ 可以为（　）．

;;;
A. $n=m=4$
B. $n=5,m=4$
C. $n=4,m=5$
D. $n=m=5$
;;;A
***
$P$ 是初等矩阵，$P$ 左乘 $A$，相当于把 $A$ 的第 $1,3$ 行交换，故交换偶数次，相当于不变，右乘 $A$ 相当于把 $A$ 的第 $1,3$ 列交换，同理交换偶数次，相当于不变，故 **A** 正确．

+++

#### 综合填空 (1) 设 $A,B$ 是 $n$ 阶方阵，$|A|=2$，$|B|=3$，$A^*,B^*$ 分别是 $A,B$ 的伴随矩阵，$C=\begin{pmatrix}A&O\\O&B\end{pmatrix}$，则 $C^*=$ ________．
***
$\begin{pmatrix}3A^*&O\\O&2B^*\end{pmatrix}$．

由 $C\cdot C^*=|C|E$，得

$$C^*=|C|C^{-1}=\begin{vmatrix}A&O\\O&B\end{vmatrix}\begin{pmatrix}A&O\\O&B\end{pmatrix}^{-1}$$

$$=|A||B|\begin{pmatrix}A^{-1}&O\\O&B^{-1}\end{pmatrix}=\begin{pmatrix}|A|A^{-1}|B|&O\\O&|B|B^{-1}|A|\end{pmatrix}$$

$$=\begin{pmatrix}|B|A^*&O\\O&|A|B^*\end{pmatrix}=\begin{pmatrix}3A^*&O\\O&2B^*\end{pmatrix}.$$

【注】$\begin{pmatrix}A&O\\O&B\end{pmatrix}^{-1}=\begin{pmatrix}A^{-1}&O\\O&B^{-1}\end{pmatrix}$，$\begin{pmatrix}O&A\\B&O\end{pmatrix}^{-1}=\begin{pmatrix}O&B^{-1}\\A^{-1}&O\end{pmatrix}$（其中 $A,B$ 均可逆）．

+++

#### 综合填空 (2) 设 $A$ 是 $n$ 阶可逆矩阵，$A$ 的每行元素之和均为 $k$，则 $A^{-1}$ 的每行元素之和均为 ________．
***
$\dfrac{1}{k}$．

先说明 $k\neq 0$，由已知，将 $|A|$ 的第 $2,3,\cdots,n$ 列加到第 $1$ 列，有

$$|A|=\begin{vmatrix}a_{11}&a_{12}&\cdots&a_{1n}\\a_{21}&a_{22}&\cdots&a_{2n}\\\vdots&\vdots&&\vdots\\a_{n1}&a_{n2}&\cdots&a_{nn}\end{vmatrix}=\begin{vmatrix}k&a_{12}&\cdots&a_{1n}\\k&a_{22}&\cdots&a_{2n}\\\vdots&\vdots&&\vdots\\k&a_{n2}&\cdots&a_{nn}\end{vmatrix},$$

由 $A$ 可逆，故 $|A|\neq 0$，所以 $k\neq 0$．

将 $A,A^{-1},E$ 写成分块矩阵（以列分块），有

$$A=(\alpha_1,\alpha_2,\cdots,\alpha_n),\quad A^{-1}=(\beta_1,\beta_2,\cdots,\beta_n),\quad E=(e_1,e_2,\cdots,e_n),$$

由 $A^{-1}A=E$，得 $A^{-1}(\alpha_1,\alpha_2,\cdots,\alpha_n)=E=(e_1,e_2,\cdots,e_n)$，故 $A^{-1}\alpha_i=e_i\ (i=1,2,\cdots,n)$，于是

$$A^{-1}\alpha_1+A^{-1}\alpha_2+\cdots+A^{-1}\alpha_n=A^{-1}(\alpha_1+\alpha_2+\cdots+\alpha_n)=A^{-1}\begin{pmatrix}k\\k\\\vdots\\k\end{pmatrix}=e_1+e_2+\cdots+e_n=\begin{pmatrix}1\\1\\\vdots\\1\end{pmatrix},$$

即

$$(\beta_1,\beta_2,\cdots,\beta_n)\begin{pmatrix}k\\k\\\vdots\\k\end{pmatrix}=k(\beta_1+\beta_2+\cdots+\beta_n)=\begin{pmatrix}1\\1\\\vdots\\1\end{pmatrix},$$

故

$$\beta_1+\beta_2+\cdots+\beta_n=\frac{1}{k}\begin{pmatrix}1\\1\\\vdots\\1\end{pmatrix}=\begin{pmatrix}\dfrac{1}{k}\\[2pt]\dfrac{1}{k}\\\vdots\\[2pt]\dfrac{1}{k}\end{pmatrix},$$

即 $A^{-1}$ 的每行元素之和均为 $\dfrac{1}{k}$．

【注】此题也可作为一个结论，在做选择、填空题时直接运用．

+++

#### 综合填空 (3) 设 $A=\begin{pmatrix}1&-1&-1&-1\\-1&1&-1&-1\\-1&-1&1&-1\\-1&-1&-1&1\end{pmatrix}$，则 $A^n\ (n\geqslant 1)=$ ________．
***
$A^n=\begin{cases}4^{k-1}A,&n=2k-1,\\4^kE,&n=2k\end{cases}\ (k=1,2,\cdots)$．

找出 $A^n$ 的规律．

$$A^2=\begin{pmatrix}1&-1&-1&-1\\-1&1&-1&-1\\-1&-1&1&-1\\-1&-1&-1&1\end{pmatrix}\begin{pmatrix}1&-1&-1&-1\\-1&1&-1&-1\\-1&-1&1&-1\\-1&-1&-1&1\end{pmatrix}=\begin{pmatrix}4&0&0&0\\0&4&0&0\\0&0&4&0\\0&0&0&4\end{pmatrix}=4E,$$

$$A^3=\begin{pmatrix}1&-1&-1&-1\\-1&1&-1&-1\\-1&-1&1&-1\\-1&-1&-1&1\end{pmatrix}\cdot 4E=4A,$$

故

$$A^n=\begin{cases}4^{k-1}A,&n=2k-1,\\4^kE,&n=2k\end{cases}\quad(k=1,2,\cdots).$$

+++

#### 综合填空 (4) 设 $A=\begin{pmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\0&0&0&0\end{pmatrix}$，则 $(E+A)^{-1}=$ ________．
***
$\begin{pmatrix}1&-1&1&-1\\0&1&-1&1\\0&0&1&-1\\0&0&0&1\end{pmatrix}$．

注意到 $A$ 的特殊性，

$$A^2=\begin{pmatrix}0&0&1&0\\0&0&0&1\\0&0&0&0\\0&0&0&0\end{pmatrix},\quad A^3=\begin{pmatrix}0&0&0&1\\0&0&0&0\\0&0&0&0\\0&0&0&0\end{pmatrix},\quad A^4=O,$$

故 $E-A^4=E$，从而 $(E+A)(E-A+A^2-A^3)=E$，故

$$(E+A)^{-1}=E-A+A^2-A^3=\begin{pmatrix}1&-1&1&-1\\0&1&-1&1\\0&0&1&-1\\0&0&0&1\end{pmatrix}.$$

【注】一般地，设 $A$ 是 $n$ 阶方阵，且 $A^k=O$，则 $E-A^k=E$，即 $E^k-A^k=E$，故

$$(E-A)(E+A+A^2+\cdots+A^{k-1})=E,$$

从而 $(E-A)^{-1}=E+A+A^2+\cdots+A^{k-1}$．进一步，当 $k$ 为偶数时，有 $E-(-A)^k=E$，从而可计算 $(E+A)^{-1}$．

+++

#### 综合解答 (1) 设 $A=\begin{pmatrix}0&0&0&1\\0&0&0&2\\0&0&0&3\\3&2&1&0\end{pmatrix}$，求 $A^n\ (n\geqslant 1)$．
***
利用分块矩阵表达 $A$．令 $\alpha=(1,2,3)^{\mathrm{T}}$，$\beta^{\mathrm{T}}=(3,2,1)$，则

$$A=\begin{pmatrix}O&\alpha\\\beta^{\mathrm{T}}&0\end{pmatrix},\quad A^2=\begin{pmatrix}O&\alpha\\\beta^{\mathrm{T}}&0\end{pmatrix}\begin{pmatrix}O&\alpha\\\beta^{\mathrm{T}}&0\end{pmatrix}=\begin{pmatrix}\alpha\beta^{\mathrm{T}}&O\\O&\beta^{\mathrm{T}}\alpha\end{pmatrix},$$

$$A^3=\begin{pmatrix}\alpha\beta^{\mathrm{T}}&O\\O&\beta^{\mathrm{T}}\alpha\end{pmatrix}\begin{pmatrix}O&\alpha\\\beta^{\mathrm{T}}&0\end{pmatrix}=\begin{pmatrix}O&\alpha\beta^{\mathrm{T}}\alpha\\\beta^{\mathrm{T}}\alpha\beta^{\mathrm{T}}&0\end{pmatrix}=\begin{pmatrix}O&(\beta^{\mathrm{T}}\alpha)\alpha\\(\beta^{\mathrm{T}}\alpha)\beta^{\mathrm{T}}&0\end{pmatrix}=\beta^{\mathrm{T}}\alpha A,$$

$$A^4=\beta^{\mathrm{T}}\alpha A^2,\cdots.$$

又

$$\alpha\beta^{\mathrm{T}}=\begin{pmatrix}1\\2\\3\end{pmatrix}(3,2,1)=\begin{pmatrix}3&2&1\\6&4&2\\9&6&3\end{pmatrix},\quad \beta^{\mathrm{T}}\alpha=(3,2,1)\begin{pmatrix}1\\2\\3\end{pmatrix}=10,$$

故

$$A^n=\begin{cases}10^{k-1}A=\begin{pmatrix}O&10^{k-1}\alpha\\10^{k-1}\beta^{\mathrm{T}}&0\end{pmatrix},&n=2k-1,\\[6pt]10^{k-1}A^2=\begin{pmatrix}10^{k-1}\alpha\beta^{\mathrm{T}}&O\\O&10^{k}\end{pmatrix},&n=2k\end{cases}\quad(k=1,2,\cdots).$$

+++

#### 综合解答 (2) 设 $A=\begin{pmatrix}-1&1&1&-1\\1&-1&-1&1\\1&-1&-1&1\\-1&1&1&-1\end{pmatrix}$，证明：$A^2+4A=O$，并求 $(E+A)^{-1}$．
***
$$A^2=\begin{pmatrix}-1&1&1&-1\\1&-1&-1&1\\1&-1&-1&1\\-1&1&1&-1\end{pmatrix}\begin{pmatrix}-1&1&1&-1\\1&-1&-1&1\\1&-1&-1&1\\-1&1&1&-1\end{pmatrix}=-\begin{pmatrix}-4&4&4&-4\\4&-4&-4&4\\4&-4&-4&4\\-4&4&4&-4\end{pmatrix}=-4A,$$

即 $A^2+4A=O$．

又

$$(E+A)^2=E+2A+A^2=E+2A-4A=-2(E+A)+3E,$$

即 $(E+A)(E+A+2E)=3E$，故

$$(E+A)^{-1}=\frac{1}{3}(A+3E)=\frac{1}{3}\begin{pmatrix}2&1&1&-1\\1&2&-1&1\\1&-1&2&1\\-1&1&1&2\end{pmatrix}.$$

+++

#### 综合解答 (3) 设 $A=\begin{pmatrix}0&1&0\\1&0&0\\0&1&1\end{pmatrix}$，证明：$A^n=A^{n-2}+A^2-E\ (n\geqslant 3)$，并计算 $A^{100}$．
***
用数学归纳法．

当 $n=3$ 时，

$$A^2=\begin{pmatrix}1&0&0\\0&1&0\\1&1&1\end{pmatrix},\quad A^3=\begin{pmatrix}0&1&0\\1&0&0\\1&2&1\end{pmatrix},$$

故满足 $A^3=A+A^2-E$．

假设 $A^{n-1}=A^{n-3}+A^2-E\ (n>3)$ 成立，则

$$A^n=A(A^{n-1})=A(A^{n-3}+A^2-E)=A^{n-2}+A^3-A$$

$$=A^{n-2}+(A^2+A-E)-A=A^{n-2}+A^2-E,$$

故对 $n\geqslant 3$，所证等式成立．

由递推关系，得

$$A^{100}=A^{98}+A^2-E=(A^{96}+A^2-E)+A^2-E=A^{96}+2(A^2-E)$$

$$=\cdots=A^2+49(A^2-E)=50A^2-49E=\begin{pmatrix}1&0&0\\0&1&0\\50&50&1\end{pmatrix}.$$

+++

#### 综合解答 (4) 设 $A=\begin{pmatrix}1&1&2\\0&-2&-4\\-1&-1&-1\end{pmatrix}$，证明：$A$ 可逆，并将 $A$ 表示为初等矩阵的乘积．
***
由 $|A|=\begin{vmatrix}1&1&2\\0&-2&-4\\-1&-1&-1\end{vmatrix}=-2\neq 0$，可知 $A$ 可逆．

将 $A$ 作一系列初等行变换（相当于左乘初等矩阵），化 $A$ 为单位矩阵．

$$\begin{pmatrix}1&1&2\\0&-2&-4\\-1&-1&-1\end{pmatrix}\xrightarrow{\ \text{第}1\text{行加到第}3\text{行}\ }\begin{pmatrix}1&1&2\\0&-2&-4\\0&0&1\end{pmatrix}$$

$$\xrightarrow{\ \text{第}2\text{行}\times\frac{1}{2}\text{加到第}1\text{行}\ }\begin{pmatrix}1&0&0\\0&-2&-4\\0&0&1\end{pmatrix}\xrightarrow{\ \text{第}2\text{行}\times\left(-\frac{1}{2}\right)\ }\begin{pmatrix}1&0&0\\0&1&2\\0&0&1\end{pmatrix}$$

$$\xrightarrow{\ \text{第}3\text{行}\times(-2)\text{加到第}2\text{行}\ }\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}.$$

将上述 $4$ 次初等行变换用初等矩阵表达，得

$$E_{23}(-2)\cdot E_2\left(-\frac{1}{2}\right)\cdot E_{12}\left(\frac{1}{2}\right)\cdot E_{31}(1)A=E,$$

其中，$E_{ij}(a)$ 表示第 $j$ 行乘以 $a$ 加到第 $i$ 行上，$E_k(b)$ 表示第 $k$ 行乘以 $b$，故

$$A=\left[E_{23}(-2)\cdot E_2\left(-\frac{1}{2}\right)\cdot E_{12}\left(\frac{1}{2}\right)\cdot E_{31}(1)\right]^{-1}$$

$$=\left[E_{31}(1)\right]^{-1}\cdot\left[E_{12}\left(\frac{1}{2}\right)\right]^{-1}\cdot\left[E_2\left(-\frac{1}{2}\right)\right]^{-1}\cdot\left[E_{23}(-2)\right]^{-1}$$

$$=E_{31}(-1)\cdot E_{12}\left(-\frac{1}{2}\right)\cdot E_2(-2)\cdot E_{23}(2)$$

$$=\begin{pmatrix}1&0&0\\0&1&0\\-1&0&1\end{pmatrix}\begin{pmatrix}1&-\dfrac{1}{2}&0\\[2pt]0&1&0\\[2pt]0&0&1\end{pmatrix}\begin{pmatrix}1&0&0\\0&-2&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&0&0\\0&1&2\\0&0&1\end{pmatrix}.$$

+++

#### 综合解答 (5) 设 $A=\begin{pmatrix}1&0&0\\0&-2&0\\0&0&1\end{pmatrix}$，且 $A^*BA=2BA-8E$，求 $B$．
***
由 $A^*BA=2BA-8E$，得 $(A^*-2E)BA=-8E$，可验证 $(A^*-2E)$ 可逆，故

$$B=(A^*-2E)^{-1}(-8E)A^{-1}$$

$$=-8(A^*-2E)^{-1}A^{-1}=-8\left[A(A^*-2E)\right]^{-1}$$

$$=-8(AA^*-2A)^{-1}=-8(|A|E-2A)^{-1},$$

而 $|A|=-2$，故

$$B=-8(-2E-2A)^{-1}=-8\left[-2(E+A)\right]^{-1}=-8\cdot\left(-\frac{1}{2}\right)(E+A)^{-1}=4(E+A)^{-1}.$$

又

$$(E+A)^{-1}=\begin{pmatrix}2&0&0\\0&-1&0\\0&0&2\end{pmatrix}^{-1}=\begin{pmatrix}\dfrac{1}{2}&0&0\\[2pt]0&-1&0\\[2pt]0&0&\dfrac{1}{2}\end{pmatrix},$$

所以

$$B=4\begin{pmatrix}\dfrac{1}{2}&0&0\\[2pt]0&-1&0\\[2pt]0&0&\dfrac{1}{2}\end{pmatrix}=\begin{pmatrix}2&0&0\\0&-4&0\\0&0&2\end{pmatrix}.$$

【注】① 由 $A=\begin{pmatrix}1&0&0\\0&-2&0\\0&0&1\end{pmatrix}$，知 $A$ 可逆，$A^*$ 也可逆，直接计算 $A^*-2E$，证明 $A^*-2E$ 可逆，计算量较大．可考虑利用 $A$ 的特征值 $\lambda_1=1,\lambda_2=-2,\lambda_3=1$，故 $A^*$ 的特征值为

$$\frac{|A|}{\lambda_1}=\frac{-2}{1}=-2,\quad\frac{|A|}{\lambda_2}=\frac{-2}{-2}=1,\quad\frac{|A|}{\lambda_3}=\frac{-2}{1}=-2,$$

$A^*-2E$ 的特征值为 $-2-2,1-2,-2-2$，故 $|A^*-2E|=(-4)\times(-1)\times(-4)\neq 0$，所以 $A^*-2E$ 可逆．

② 验证 $A^*-2E$ 可逆，也可利用公式 $AA^*=|A|E=-2E$，故 $A^*=-2A^{-1}$，即

$$A^*-2E=-2A^{-1}-2E=-2(A^{-1}+E)=-2\left[\begin{pmatrix}1&0&0\\0&-\dfrac{1}{2}&0\\0&0&1\end{pmatrix}+\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}\right]=-2\begin{pmatrix}2&0&0\\0&\dfrac{1}{2}&0\\0&0&2\end{pmatrix},$$

显然可逆．

+++

#### 综合解答 (6) 设矩阵 $X$ 满足 $\begin{pmatrix}1&0&1\\2&1&-1\\-1&-1&2\end{pmatrix}X=\begin{pmatrix}0&1\\2&0\\-2&1\end{pmatrix}$，求 $X$．
***
记 $A=\begin{pmatrix}1&0&1\\2&1&-1\\-1&-1&2\end{pmatrix}$，则 $|A|=0$，故 $A$ 不可逆．

令 $X=\begin{pmatrix}x_1&y_1\\x_2&y_2\\x_3&y_3\end{pmatrix}$，则 $A\begin{pmatrix}x_1\\x_2\\x_3\end{pmatrix}=\begin{pmatrix}0\\2\\-2\end{pmatrix}$，$A\begin{pmatrix}y_1\\y_2\\y_3\end{pmatrix}=\begin{pmatrix}1\\0\\1\end{pmatrix}$，只要解两个非齐次线性方程组．对增广矩阵作初等行变换，

$$\left(\begin{array}{ccc|c}1&0&1&0\\2&1&-1&2\\-1&-1&2&-2\end{array}\right)\longrightarrow\left(\begin{array}{ccc|c}1&0&1&0\\0&1&-3&2\\0&0&0&0\end{array}\right),$$

解得其通解为 $(x_1,x_2,x_3)^{\mathrm{T}}=k_1(-1,3,1)^{\mathrm{T}}+(0,2,0)^{\mathrm{T}}$．

同样解得另一个方程组的通解为 $(y_1,y_2,y_3)^{\mathrm{T}}=k_2(-1,3,1)^{\mathrm{T}}+(1,-2,0)^{\mathrm{T}}$，故

$$X=\begin{pmatrix}-k_1&1-k_2\\2+3k_1&-2+3k_2\\k_1&k_2\end{pmatrix}\quad(k_1,k_2\text{ 为任意常数}).$$

+++

#### 拓展解答 (1) 设 $A=\begin{pmatrix}3&2&2\\0&1&1\\0&0&3\end{pmatrix}$，$B=\begin{pmatrix}1&0&0\\0&0&0\\0&0&-1\end{pmatrix}$，若矩阵 $X$ 满足 $AX+2B=BA+2X$，求 $X^2$．
***
$AX+2B=BA+2X$ 变形为

$$(A-2E)X=B(A-2E).$$

由 $A-2E=\begin{pmatrix}1&2&2\\0&-1&1\\0&0&1\end{pmatrix}$ 可逆，知 $X=(A-2E)^{-1}B(A-2E)$，由此可得

$$X^2=(A-2E)^{-1}B^2(A-2E)$$

$$=\begin{pmatrix}1&2&2\\0&-1&1\\0&0&1\end{pmatrix}^{-1}\begin{pmatrix}1&0&0\\0&0&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&2&2\\0&-1&1\\0&0&1\end{pmatrix}$$

$$=\begin{pmatrix}1&2&-4\\0&-1&1\\0&0&1\end{pmatrix}\begin{pmatrix}1&0&0\\0&0&0\\0&0&1\end{pmatrix}\begin{pmatrix}1&2&2\\0&-1&1\\0&0&1\end{pmatrix}$$

$$=\begin{pmatrix}1&2&-2\\0&0&1\\0&0&1\end{pmatrix}.$$

+++

#### 拓展解答 (2) 设分块矩阵 $P=\begin{pmatrix}A&C\\O&B\end{pmatrix}$ 为正交矩阵，$A,B$ 分别是 $m$ 阶和 $n$ 阶方阵，证明：$A$ 与 $B$ 是正交矩阵．
***
要证 $A,B$ 是正交矩阵，只要证 $A^{\mathrm{T}}A=E_m$，$B^{\mathrm{T}}B=E_n$．

依题设，$P^{\mathrm{T}}P=E$，则

$$P^{\mathrm{T}}P=\begin{pmatrix}A&C\\O&B\end{pmatrix}^{\mathrm{T}}\begin{pmatrix}A&C\\O&B\end{pmatrix}=\begin{pmatrix}A^{\mathrm{T}}&O\\C^{\mathrm{T}}&B^{\mathrm{T}}\end{pmatrix}\begin{pmatrix}A&C\\O&B\end{pmatrix}$$

$$=\begin{pmatrix}A^{\mathrm{T}}A&A^{\mathrm{T}}C\\C^{\mathrm{T}}A&C^{\mathrm{T}}C+B^{\mathrm{T}}B\end{pmatrix}=E=\begin{pmatrix}E_m&O\\O&E_n\end{pmatrix},$$

故

$$A^{\mathrm{T}}A=E_m,\quad A^{\mathrm{T}}C=O,\quad C^{\mathrm{T}}A=O,\quad C^{\mathrm{T}}C+B^{\mathrm{T}}B=E_n.$$

由 $P$ 是正交矩阵，故 $P$ 可逆，$|P|=|A||B|\neq 0$，因此 $|A|\neq 0$，$A$ 可逆，从而 $A^{\mathrm{T}}$ 可逆．由 $A^{\mathrm{T}}C=O$ 知 $C=O$，所以 $B^{\mathrm{T}}B=E_n$，于是 $A,B$ 是正交矩阵．
