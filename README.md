# 丘维声《高等代数》学习笔记

《高等代数》，丘维声，北京大学，视频：共151讲，[B站视频链接](https://www.bilibili.com/video/av39523603)

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [丘维声《高等代数》学习笔记](#丘维声高等代数学习笔记)
	- [前言](#前言)
	- [第一章 线性方程组的解法](#第一章-线性方程组的解法)
		- [1. .1 解线性方程组的矩阵消元法](#1-1-解线性方程组的矩阵消元法)
			- [加减消元法](#加减消元法)
			- [矩阵的初等行变化](#矩阵的初等行变化)
			- [在有理数集内解线性方程组](#在有理数集内解线性方程组)
		- [1.2 线性方程组解的情况及其判别情况](#12-线性方程组解的情况及其判别情况)
		- [1.3 数域](#13-数域)
			- [习题1.3 思路](#习题13-思路)
	- [第二章 行列式](#第二章-行列式)
		- [2.1 n元排列](#21-n元排列)
			- [习题 2.1](#习题-21)
		- [2.2 n阶行列式的定义](#22-n阶行列式的定义)
			- [习题2.2](#习题22)
		- [2.3 行列式的性质](#23-行列式的性质)
			- [习题 2.3](#习题-23)
		- [2.4 行列式按一行（列）展开](#24-行列式按一行列展开)
			- [习题2.4](#习题24)
		- [2.5 克莱姆法则](#25-克莱姆法则)
			- [习题2.5](#习题25)
		- [2.6 行列式按k行（列）展开](#26-行列式按k行列展开)
	- [第三章 线性空间](#第三章-线性空间)
		- [3.1 线性空间的定义](#31-线性空间的定义)
			- [习题3.1](#习题31)
		- [3.2 线性子空间](#32-线性子空间)
			- [习题8.1](#习题81)
			- [习题 8.2](#习题-82)
		- [3.3 线性相关与线性无关的向量组](#33-线性相关与线性无关的向量组)
			- [习题 3.2](#习题-32)
		- [3.4 极大线性无关组和向量组的秩](#34-极大线性无关组和向量组的秩)
		- [3.5 基与维数](#35-基与维数)
			- [习题3.3](#习题33)
		- [3.6 矩阵的秩](#36-矩阵的秩)
		- [3.7 线性方程组有解的判别](#37-线性方程组有解的判别)
		- [3.8 齐次线性方程组解集的结构](#38-齐次线性方程组解集的结构)
		- [3.9 非齐次线性方程组的解集结构](#39-非齐次线性方程组的解集结构)
		- [3.10 子空间的运算](#310-子空间的运算)
		- [3.11 线性空间的同构](#311-线性空间的同构)
		- [3.12 映射的乘法，可逆映射](#312-映射的乘法可逆映射)
	- [参考](#参考)

<!-- /TOC -->

## 前言

> 视频1、2

* n元线性方程组和其解法
* 矩阵的定义（由n元线性方程组的系数得到）
  * 通常由 _A_ 表示
  * 对于线性方程组，可以得到**增广矩阵**
* **高等代数研究对象**：
  * **n元线性方程组**
    * 研究**解的情况的判别**和**解集的结构**
  * **矩阵**
  * **n维向量空间**
  * **线性空间**（由n维向量空间抽象而来）
  * **线性映射**（研究线性空间，就离不开线性映射）
  * **双线性函数**
  * **具有度量的线性空间**
    * 欧几里得空间
    * 酉空间
    * 等等
  * **与度量有关的线性变换**
    * 正交变换
    * 对称变换
    * 酉变换
    * Hermite变换
* **线性代数的主线：**
  * 线性空间
  * 线性映射
* 一元高次方程的求根
  * 一元多项式环
  * 环的概念
  * 域的概念
  * 群的概念
* **数学的思维方式**
  * 观察客观现象
    * 提出研究的问题
    * 抓住主要特征
  * 抽象出概念或建立模型
  * 探索
    * 运用直觉、类比、归纳、联想、推理
  * 猜测（可能的规律）
  * 论证
    * 深入分析
    * 运用定义、公理、已证明的定理进行推理
  * 揭示事物内在规律

## 第一章 线性方程组的解法

### 1. .1 解线性方程组的矩阵消元法

> 视频3、4、5

#### 加减消元法

* 不同方程的乘以系数后和其他方程加减，以消除方程中某个（些）系数
* 如果以矩阵方式来写，把矩阵转换为阶梯型矩阵，即左下角的元素全为0
  * 首先针对矩阵第一列，其次第二列，直到最后一列
* 当主元全是1，其他元素都是0 时，增广矩阵的最后一列即为X的解

#### 矩阵的初等行变化

1. 把一行的倍数加到另外一行
2. 两行互换
3. 一行乘以一个非零系数

**结论**：矩阵的初等行变换得到的解与原方程组同解

作业，习题1.1的1和2

#### 在有理数集内解线性方程组

**有且只有如下三种情况：**

* **无解**：阶梯形方程组无解，从而原方程组无解
  * 视频中的例子是最后一行：_0 x<sub>3</sub>= -2_
* **有无穷多个解**，从而原方程有无穷多个解
  * 视频的例子是最后一行：_0 x<sub>2</sub> = 0_
  * _x<sub>2</sub>_ 是自由未知量（主变量以外的未知量）
  * _x<sub>1</sub>, x<sub>3</sub>_ 是主变量（以主元为系数的未知量）
* **有唯一的解**

当有解的时候，要么有一个解，要么有无穷多个解。

> 从两条直线来考虑这个问题，它们要么相交，要么重叠，要么平行。

**方程组是否有解的总结：**

* 如果线性方程的增广矩阵经过初等变换成阶梯矩阵后
  * 相应的阶梯矩阵方程组如果出现 _0 = d_ （其中 _d_ 是非零数），那么原方程组无解，否则有解。
* 当有解时
  * 若阶梯形矩阵的非零行的数目 _r = n_ （未知量数目），那么方程有唯一解
  * 如 _r < n_，那么方程有无穷多个解。

### 1.2 线性方程组解的情况及其判别情况

> 视频5、6

证明：n元线形方程组的增广矩阵经过初等行变换成阶梯矩阵有 _r_ 个非零行，显然有 _n + 1_ 列。

* 情况1： *"0 = d"*，无解
* 情况2： 不出现*"0 = d"*
  * 由于 _J_ 的第 _r_ 个主元 _b<sub>rt</sub>_ 不能位于第 _n+1_ 列，因此 _t ≤ n_
  * 因为只能位于对角线的右上方，所以有 _t ≥ r_
  * 情况 2.1：_r = n_
    * _J<sub>1</sub>_ 有n个主元，最后一列的 _(C<sub>1</sub>, C<sub>2</sub>, ..., C<sub>n</sub>)_ 是方程唯一解
  * 情况 2.2：_r < n_
    * 有 _n - r_个自由未知量

### 1.3 数域

> 视频7

定义1：复数集的一个非空子集K，如果满足：

（1）*0， 1 ∈ K*

（2）*a，b ∈ K* → *a ± b, ab ∈ K*

（3）*a，b ∈ K*，且 *b ≠ 0 → <sup>a</sup>/<sub>b</sub> ∈ K*

上面 *K* 是一个数域

**数域举例：**

- 有理数域 *Q* （最小的数域）
- 实数域 *R*
- 复数域 *C* （最大的数域）

对于例子：

-  _a<sub>11</sub>x1 + a<sub>12</sub>x<sub>2</sub> = b<sub>1</sub>_
- _a<sub>21</sub>x1 + a<sub>22</sub>x<sub>2</sub> = b<sub>2</sub>_

其增广矩阵转化为阶梯矩阵后可得

$$
\begin{pmatrix} a_{11} & a_{12} & b_1\\ 0 & a_{22} - \frac{a_{21}}{a_{11}}a_{12} & b_2 - \frac{a_{21}}{a_{11}}b_1 \end{pmatrix}
$$


所以需要第二行第二个元素部位*0*，意味着

* _(<sup> a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub> </sup>/<sub> a<sub>11</sub> </sub>) ≠ 0_，即
* _a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub> ≠ 0_

表达式_a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub> ≠ 0_ 用  _|A|_ 来表示，称为**行列式**，这里是**二阶行列式**

#### 习题1.3 思路

1. 令 *Q(i) = {a + bi | a, b ∈ Q}*, 证明 *Q(i)* 是一个数域

证明思路：

* 0 = 0 + 0i ∈ Q(i), 1 = 1 + 0 i ∈ Q(i)
* α = a + bi, β = c + di
  - α ± β = (a ± c) + (b ± d)i ∈ Q(i)
  - αβ = (ac - bd) + (ad + bc)i ∈ Q(i)
  - β ≠ 0，则c、d不全为0，则$ \frac{\alpha}{\beta} = \frac{a+bi}{c+di} = \frac{(a+bi)(c-di)}{(c+di)(c-di)}=\frac{ac+bd}{c^2+d^2}+\frac{(bc-ad)}{c^2+d^2}i \in Q(i) $

2. 令 $F=\{\frac{a_0+a_1e+\cdots+a_ne^n}{b_0+b_1e+\cdots+b_ne^n}$ ，n、m为任意非负整数，a<sub>i</sub>，b<sub>i</sub> 数域 Z，0 ≤ i ≤ n, 0 ≤ j ≤ m。证明F是一个数域，其中e是自然对数的底。

证明思路：

* 对于 0、1∈ F的思路同上题目
* 对于F中的两个数 α、β
  * 令$\alpha=\frac{a_0+a_1e+\cdots+a_{n_\alpha}e^{n_\alpha}}{b_0+b_1e+\cdots+b_{n_\alpha}e^n_{n_\alpha}}, \beta=\frac{a_0+a_1e+\cdots+a_{n_\beta}e^{n_\beta}}{b_0+b_1e+\cdots+b_{n_\beta}e^n_{n_\beta}}$
  * 则 $\alpha\beta=\frac{a_0^2+2a_0a_1e+\cdots+a_{n_\alpha}a_{n_\beta}e^{n_\alpha+n_\beta}}{b_0^2+2b_0b_1e+\cdots+b_{n_\alpha}b_{n_\beta}e^n_{n_\alpha+n_\beta}}$，所以 αβ ∈ F
  * 同样的思路 α ± β ∈ F，<sup>α</sup>/<sub>β</sub> ∈ F

## 第二章 行列式

先研究属于 _K_ 上二元一次方程组，例子：

- _a<sub>11</sub>x1 + a<sub>12</sub>x<sub>2</sub> = b<sub>1</sub>_
- _a<sub>21</sub>x1 + a<sub>22</sub>x<sub>2</sub> = b<sub>2</sub>_

在 1.3节中讨论过 当 _a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub> ≠ 0_时方程有唯一解；_a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub> = 0_是有无穷多个解，为了方便记忆，把表达式 _a<sub>11</sub>a<sub>22</sub> - a<sub>21</sub>a<sub>12</sub>_写作：

$$
\left|\begin{array}{ll}{a_{11}} & {a_{12}} \\ {a_{21}} & {a_{22}}\end{array}\right|=a_{11}a_{22}-a_{12}a_{21}
$$

这是**2阶行列式**。把系数矩阵记作_A_，那么它对应的行列式记作 _|A|_ 或 det(A)。

**数域 _K_ 上的系数矩阵 _A_ 有唯一解 <==> _|A| ≠ 0_**

### 2.1 n元排列

**_n_元排列**：_1, 2, ..., n_ 的一个全排列。排列个数有 _n!_ 个。

**排列方法**：

1. **顺序**：数字从小到大排列（对 a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>，任取一对数_a<sub>i</sub>a<sub>j</sub>_，如果_a<sub>i</sub><a<sub>j</sub>_，则称这一对数构成一个顺序
2. **逆序**：数字从大到小排列（对 a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>，任取一对数_a<sub>i</sub>a<sub>j</sub>_，如果_a<sub>i</sub>>a<sub>j</sub>_，则称这一对数构成一个逆序

**逆序数**：一个 _n_ 元排列中逆序的总数称为**逆序数**，记作_**τ(a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>)**_。

* 例如_τ(2431) = 2_，因为有24、31这两个逆序数对。

**偶（奇）排列：**逆序数个数为偶（奇）数，那么这个排列称为**偶（奇）排列**。

**对换：**一个排列里的两个数字互换位置，称为一次**对换**。

**定理1：对换会改变数列奇偶性。**

**定理2：任一n元排列与排列123...n可经过一系列对换互变，并且所做对换的次数与这个n元排列有相同的奇偶性。**

#### 习题 2.1

2\. (1) $\tau = \frac{(n-1)(n-2)}{2}$, (2) $\tau=n-1$
4\. (1) k - 2, (2) n - k - 1
6\. $|A| = 2*4 + 15 = 23$，因此有唯一解$x_1 = 2, x_2 = -1$


### 2.2 n阶行列式的定义

定义1：n阶行列式

$$
\left|
\begin{array}{cccc}
{a_{11}} & {a_{12}} & {\cdots} & {a_{1n}} \\
{a_{21}} & {a_{22}} & {\cdots} & {a_{2n}} \\
{\vdots} & {\vdots} &  & {\vdots} \\
{a_{n1}} & {a_{n2}} & {\cdots} & {a_{mn}}
\end{array}
\right|
= \sum_{j_1j_2\vdots j_n}(-1)^{\tau(j_1j_2\cdots j_n)}a_{1j_1}a_{2j_2}\cdots a_{nj_n}
$$

简记作$|A|$或 $\mathbb{det} A$。

**命题1**：n阶上三角形行列式的值等于它的主对角线上n个元素的乘积。

#### 习题2.2

2\. (1) -49, (2) 103, (3) $a_{11}a_{22}a_{33}$, (4) $ca_1b_2 - ca_2b_1$

可以用下面的Python代码来验证结果：

``` python
import numpy as np
A = np.array([[1, 4, 2],[3, 5, 1],[2, 1, 6]])
print(np.linalg.det(a))
```

4\. 不是

5\. 四次，5和5

6\. 如果元素相同，|A| = 0，为偶数

### 2.3 行列式的性质

> [视频12](https://www.bilibili.com/video/av39523603/?p=12)

**性质1**：行列互换（矩阵转置），行列式的值不变。
$$
|A| = |A^T|
$$

**性质2**：行列式一行的公因子可以提出去。即为
$$
\left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {k a_{i 1}} & {k a_{i 2}} & {\cdots} & {k a_{i n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{nn}}\end{array}\right|=k \left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{i 1}} & {a_{i 2}} & {\cdots} & {a_{i n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{nn}}\end{array}\right|
$$

**性质3**：行列式中若有某一行是两组数的和，则此行列式等于两个行列式的和，这两个行列式的这一行分别是第一组数和第二组数，而其余各行于原来行列式的相应各行相同，即
$$
\left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {b_{1} + c_1} & {b_{2}+c_2} & {\cdots} & {b_{n}+c_n} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{nn}}\end{array}\right|=\left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {b_{1}} & {b_{2}} & {\cdots} & {b_{n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{nn}}\end{array}\right| + \left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {c_1} & {c_2} & {\cdots} & {c_n} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{nn}}\end{array}\right|
$$

**性质4**：两行互换，行列式反号，即
$$
\left|\begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{i 1}} & {a_{i 2}} & {\cdots} & {a_{i n}} \\ {\vdots} & {\vdots} & & {\vdots} \\ {a_{k 1}} & {a_{k 2}} & {\cdots} & {a_{k n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{m}}\end{array}\right| = -
\left| \begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{k 1}} & {a_{k 2}} & {\cdots} & {a_{k n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{i 1}} & {a_{i 2}} & {\cdots} & {a_{i n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{m}}\end{array}\right|
$$

**性质5**：两行相同，行列式的值为0。即
$$
\left|\begin{array}{cccc}{a_{11}} & {a_{12}} & {\cdots} & {a_{1 n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{i 1}} & {a_{i 2}} & {\cdots} & {a_{i n}} \\ {\vdots} & {\vdots} & & {\vdots} \\ {a_{i 1}} & {a_{i 2}} & {\cdots} & {a_{i n}} \\ {\vdots} & {\vdots} &  & {\vdots} \\ {a_{n 1}} & {a_{n 2}} & {\cdots} & {a_{m}}\end{array}\right| = 0
$$

**性质6**：两行成比例，行列式的值为0。

**性质7**：把一行的倍数加到另一行上，行列式的值不变。（根据性质3和性质5可以证明）

上述七个行列式性质可以总结为如下的图：

![2.3.Determinant-rules](img/2.3.Determinant-rules.png)

#### 习题 2.3

2\. (1) $(a + n-1)(a - 1)^{n-1}$，思路为把所有行加到第一行，第一行的每一个元素相同，可以提取出一个倍数$(a+n-1)$，第一行元素全为1，再把所有行减去第一行，因此仅剩右对角线上元素为$a-1$，可得

2\. (2)  $\left((\sum_{i=1}^na_i)-b\right)(-b)^{(n-1)}$，同上，把所有的列加到第一列

3\. (1) 所有列相加得0，所以为0

3\. (2) 利用性质7，做列的加减

4\. (1) $a_1 - \sum_{i=2}^{n}a_ib_i$，利用性质7做列加减，让第一列除了第一个元素外其他元素都为0

4\. (2) 0，利用性质3，把第一行的每个元素拆分为2个，因此有两个行列式，发现两个行列式的除了第一行外都成比例，根据性质6，分别为0。

### 2.4 行列式按一行（列）展开

> [视频14](https://www.bilibili.com/video/av39523603/?p=14)

**定义1**：n阶行列式$|A|$中，花去第$i$行和第$j$列，剩下的元素按原来次序组成的$n-1$阶行列式称为矩阵$A$的$(i, j)$的**余子式**，记作$M_{ij}$。令
$$
A_{ij} = (-1)^{i+j}M_{ij}
$$

称为$A_{ij}$是$A$的$(i, j)$的**代数余子式**。

对于一个$n=3$的矩阵有，$|A| = a_{11}A_{11}+a_{12}A_{12}+a_{13}A_{13}$，可以推广得到

**定理1**：n阶行列式$|A|$等于它的第$i$行元素与自己的代数余子式的乘积之和，即
$$
|A| = \sum_{j=1}^{n} a_{ij}A_{ij}
$$

**定理2**：n阶行列式$|A|$等于它的第$j$列元素与自己的代数余子式的乘积之和，即
$$
|A| = \sum_{l=1}^{n} a_{lj}A_{lj}
$$

**定理3**：n阶行列式$|A|$的第$i$行元素与第$k$行相应元素的**代数余子式**的乘积之和等于0，即
$$
a_{i1}A_{k1}+a_{i2}A_{k2}+\cdots+a_{in}A_{kn}=0，当k\neq i.
$$

**定理4**：n阶行列式$|A|$的第$j$列元素与第$l$列（$l \neq j$）相应元素的**代数余子式**的乘积之和等于0，即
$$
a_{1j}A_{1l}+a_{2j}A_{2l}+\cdots+a_{nj}A_{nl}=0，当l\neq i.
$$

**范德蒙行列式**：
$$
\left| \begin{array}{ccccc}{1} & {1} & {1} & {\cdots} & {1} \\ {a_{1}} & {a_{2}} & {a_{3}} & {\cdots} & {a_{n}} \\ {a_{1}^{2}} & {a_{2}^{2}} & {a_{3}^{2}} & {\cdots} & {a_{n}^{2}} \\ {\vdots} & {\vdots} & {\vdots} & { } & {\vdots} \\ {a_{1}^{n-2}} & {a_{2}^{n-2}} & {a_{3}^{n-2}} & {\cdots} & {a_{n}^{n-2}} \\ {a_{1}^{n-1}} & {a_{2}^{r-1}} & {a_{3}^{n-1}} & {\cdots} & {a_{n}^{n-1}}\end{array}\right|
= \prod_{1 \leq j<i \leq n}\left(a_{i}-a_{j}\right)
$$

#### 习题2.4

1\. (3)    $(\lambda^2+\lambda-10)(\lambda-1)$

2\. $-(n-1)!\sum_{i=1}^{n}a_i$ （第一列加到第二列，依次类推，第i列加到第i+1列）

7\. $x\left[\sum_{i}^{n-1}(-1)^i(x-y)^{n-1-i}(z-x){i}\right]$

12\. 参考例题7的思路：
$$
\begin{align*}
D_{1}&=1+x^{2} \\
D_{2}&=\left(1+x^{2}\right)^{2}-x^{2}\\
\Rightarrow D_2 - D_1 &= x^4\\
\\
D_{n}&=\left(1+x^{2}\right) D_{n-1}-x^{2} D_{n-2}\\
\Rightarrow D_{n}-D_{n-1} &= x^{2}\left(D_{n-1}-D_{n-2}\right)\\
\Rightarrow D_{n}-D_{n-1} &=x^{2(n-2)}\left(D_{2}-D_{1}\right)\\
\Rightarrow D_{n}-D_{1}&=\sum_{i=2}^{n} x^{2 i}
\\
\Rightarrow D_{n}=1+\sum_{i=1}^{n} x^{2 i}
\end{align*}
$$
13\. $\prod_{1 \leq j<i \leq n}\left(x_{i}-x_{j}\right)$（第k+1行减去第k行，转换为范德蒙行列式）

### 2.5 克莱姆法则

> [视频16](https://www.bilibili.com/video/av39523603/?p=16)

**定理1**：数域$K$上$n$个方程的$n$元线性方程组有唯一解的充分必要条件是它的系数行列式（即系数矩阵$A$的行列式$|A|$）不等于0。

**推论1**：数域$K$上$n$个方程的$n$元齐次线性方程组只有零解的充分必要条件是它的系数行列式不等于0.它有非零解的充分必要条件是它的系数行列式等于0。

#### 习题2.5

2\. 有唯一解

4\. a = 1 或 b = 0

### 2.6 行列式按k行（列）展开

概念类似于行列式按一行（列）展开。

**定义1**：$n$阶行列式$|A|$中任意取定$k$行、$k$列（$1\leq k <n$），位于这些行列交叉处的$k^2$个元素按原来的排法组成的k阶行列式，称为$|A|$的一个**$k$阶子式**（1）。划去这个k阶子式所在的行和列，剩下的元素按原来的排法组成的（$n-k$）阶行列式，称为余子式，在它前面乘以$(-1)^{(i_1+i_2+\cdots +i_k)+(j_1+j_2+\cdots +j_k)}$，则为子式（1）的**代数余子式**。

定理1（拉普拉斯定理）：在$n$阶行列式$|A|$中，取定第$i_1, i_2, \cdots, i_k$行（$i_1<i_2<\cdots<i_k$），则这$k$行元素形成的所有$k$阶子式与它们自己的代数余子式的乘机之和等于$|A|$，即
$$
|A|=\sum_{1 \leqslant j_{1}<j_{2}<\cdots<j_{k} \leqslant n} A \left( \begin{array}{c}{i_{1}, i_{2}, \cdots, i_{k}} \\ {j_{1}, j_{2}, \cdots, j_{k}}\end{array}\right)(-1)^{\left(i_{1}+\cdots+i_{k}\right)+\left(j_{1}+\cdots+j_{k}\right)} A \left( \begin{array}{l}{i_{1}^{\prime}, i_{2}^{\prime}, \cdots, i_{n-k}^{\prime}} \\ {j_{1}^{\prime}, j_{2}^{\prime}, \cdots, j_{n-k}^{\prime}}\end{array}\right)
$$
**推论1**：下式成立：
$$
\left| \begin{array}{ll}{A} & {0} \\ {C} & {B}\end{array}\right|=|A||B|
$$


## 第三章 线性空间

### 3.1 线性空间的定义

令$K^n:=\{(a_1, a_2, \cdots, a_n)|a_k \in K, i=1,2,\cdots,n\}$ 是数域$K$上的一个线性空间。称作数域$K$的$n$维空间。

**规定**：$(a_1, a_2, \cdots, a_n) = (b_1, b_2, \cdots, b_n)  \Longleftrightarrow a_i = b_i$

* 加法：$(a_1, a_2, \cdots, a_n) + (b_1, b_2, \cdots, b_n)  := (a_1+b_1, a_2+b_2, \cdots, a_n+b_n)$
* 数量乘法：$k(a_1, a_2, \cdots, a_n) = (ka_1, ka_2, \cdots, ka_n)$

若**对应法则** $f: A \longrightarrow B$，对于每一个$a \in A$都有唯一的$b \in B$，则称$f$是$A$到$B$的一个**映射**。其中A为**定义域**（domain），B为**培域**（co-domain）。

$f$的**值域**或**像**$f(A):=\{f(a) | a \in A\}$

* 若$f(A)=B$，则$f$称为**满射**。
* 若A中不同元素在$f$下的像不同，则称$f$是**单射**。
* 若$f$既是单射，又是满射，则$f$称为一个**双射**（或一一对应）

$S \times M:=\{(a, b) | a \in S, b \in M\}$称为$S$与$M$的**笛卡尔积**。

**定义1**：非空集合$S$上一个**代数运算**时指$S\times S$到 $S$的一个映射。

**定义3**：设$V$是一个非空集合，$K$是一个数域

* 如果$V$上有一个运算，称为**加法**，即$(\alpha, \beta) \rightarrow \alpha + \beta$；
* $K$与$V$之间有一个运算称为**数量乘法**，即$K\times V \rightarrow V:(k, \alpha)\rightarrow k\alpha$.
* 且满足如下8条运算法则：
  1. $\alpha + \beta = \beta + \alpha, \forall \alpha, \beta \in V$
  2. $(\alpha + \beta) + \gamma = \alpha + (\beta + \gamma), \forall \alpha, \beta, \gamma \in V$
  3. 把元素(0, 0, ..., 0)记作**0**, 它使得 $\textbf{0} + \alpha = \alpha + \textbf{0} = \alpha$
  4. $\alpha+(-\alpha)=(-\alpha)+\alpha=0$，称$-\alpha$是$\alpha$的负元素。
  5. $1\alpha=\alpha, \forall \alpha \in V$
  6. $(kl)\alpha=k(l\alpha), \forall k, l \in K, \alpha \in V$
  7. $(k+l)\alpha=k\alpha + l\alpha, \forall k, l \in K, \alpha \in V$
  8. $k(\alpha + \beta)=k\alpha + k\beta, \forall k \in K, \alpha, \beta \in V$

$\mathbb{R}^X:=\{$非空集合$X$到$\mathbb{R}$的映射$\}$，定义为$X$上的一个实值函数。

规定:

* $(f+g)(x):=f(x)+g(x), \forall x \in X$;
* $(kf)(x) := kf(x), \forall x \in X$.
* 零函数 $0(x)=0, \forall x \in X$.

运算性质：

1. 设$V$是数域$K$上的一个线性空间，$V$的零元唯一。
2. 每个$\alpha \in V$的负元唯一。
3. $0\alpha=0, \forall \alpha \in V$
4. $k0=0, \forall k \in K$
5. 若$k \alpha=0$，则$k=0$或$\alpha=0$。
6. $(-1)\alpha=-\alpha$

#### 习题3.1

1\. （1）[0 0 0 0]<sup>T</sup> （2）[0 0 0 0]<sup>0</sup>
2\. (-21 7 15 13)
3\. （2）不能
6\.  加法和乘法后仍属于$U$
7\.  是

### 3.2 线性子空间

> 这部分内容对应下册8.2节

**定义**：设$V$是数域$K$上的一个线性空间。$U$是$V$的一个非空子集。如果$U$对于$V$的加法和数量乘法也称为数域$K$上的一个线性空间，那么称$U$是$V$的一个**线性子空间**。

**定理**1：设$U$是域$F$上线性空间$V$的一个非空子集，则$U$是$V$的一个子空间的充分必要条件是：$U$**对于$V$的加法和纯量乘法都封闭**，即

* $\alpha, \beta \in U \Rightarrow \alpha + \beta \in U$
* $\alpha \in U, k \in F \Rightarrow k \alpha \in U$

在$K^n$中，给定向量组$\alpha_1, \cdots, \alpha_s$, $\beta \in K^n \Leftrightarrow$存在$K$中一组数$l_1, l_2, \cdots, l_s$，使得$\beta = l_1\alpha_1 + \cdots + l_s\alpha_s$，此时称$\beta$可以由向量组$\alpha_1, \cdots, \alpha_s$**线性表出**。

数域$K$上的$n$元线性方程组
$$
\left\{\begin{array}{l}{a_{11} x_{1}+a_{12} x_{2}+\cdots+a_{1 n} x_{n}=b_{1}} \\ {a_{21} x_{1}+a_{22} x_{2}+\cdots+a_{2 n} x_{n}=b_{2}} \\ {\cdots} \\ {a_{s 1} x_{1}+a_{s 2} x_{2}+\cdots+a_{s n} x_{n}=b_{s}}\end{array}\right.
$$
可以写成$x_{1} \boldsymbol{\alpha}_{1}+x_{2} \boldsymbol{a}_{2}+\cdots+x_{n} \boldsymbol{\alpha}_{n}=\boldsymbol{\beta}$，其**有解**

$\Longleftrightarrow$有$K$种一组数$c_1, c_2, \cdots, c_n$使得下式成立：
$$
c_{1} \boldsymbol{a}_{1}+c_{2} \boldsymbol{a}_{2}+\cdots+c_{n} \boldsymbol{a}_{n}=\boldsymbol{\beta}
$$
$\Longleftrightarrow \beta$可以由$\boldsymbol{\alpha}_{1}, \boldsymbol{\alpha}_{2}, \cdots, \boldsymbol{\alpha}_{n}$**线性表出**。

#### 习题8.1

1\. (1) Yes (2) Yes (3) Yes (4) No (5) Yes
2\.
3\. (1) Yes (2) Yes (3) Yes
7\.
8\. 线性相关
9\. （1）相关：$cos2x = 2cos^2x-1$（2）相关：$cos(3x) = 4cos^3(x) - 3cosx$ （3）无关 (4) 有关 (5) 有关 (6)有关 (7)有关

#### 习题 8.2

1. （1） 不是，例如 (1, ..., 1)、(-1, ..., 1)的和即不符合（2） 是

### 3.3 线性相关与线性无关的向量组

> 视频23，对应教材3.2节

$\overrightarrow{c}$与$\overrightarrow{a}$**共线** $\Longleftrightarrow$ 有不全为0的实数$k_1$, $k_2$使得 $k_1\overrightarrow{c}+k_2\overrightarrow{a}=\overrightarrow{0}$；

$\overrightarrow{c}$与$\overrightarrow{a}$**不共线** $\Longleftrightarrow$  $k_1\overrightarrow{c}+k_2\overrightarrow{a}=\overrightarrow{0}$ 可推出$k_1$, $k_2=0$。

**定义1**：设$V$是数域$K$上的一个线性空间，$V$中的一个向量组$\alpha_1, \alpha_2, \cdots, \alpha_s (S \geq 1)$，如果有$K$中不全为0的书$k_1, \cdots, k_s$，使得
$$
k_{1} \boldsymbol{\alpha}_{1}+\cdots+k_{s} \boldsymbol{\alpha}_{s}=\mathbf{0}
$$
则称向量组$\boldsymbol{\alpha}_{1}, \cdots, \boldsymbol{\alpha}_{s}(s \geqslant 1)$**线性相关**（否则称**线性无关**）

$\Longleftrightarrow$ 齐次线性方程组 $x_{1} \boldsymbol{\alpha}_{1}+\cdots+x_{s} \boldsymbol{a}_{s}=\mathbf{0}$ 有非零解。

$\Longleftrightarrow$以$\alpha_1, \cdots, \alpha_n$为列向量的矩阵$A$的行列式等于0。



$K^s$中，列向量方程组$\alpha_1, \cdots, \alpha_n$线性无关

$\Longleftrightarrow$ 线性方程组$x_{1} \boldsymbol{\alpha}_{1}+\cdots+x_{s} \boldsymbol{a}_{s}=\mathbf{0}$ 只有零解。



设$V$施数域$K$上的一个线性空间：

1. $\alpha$线性相关$\Longleftrightarrow$有$k \neq 0$使得$k\alpha=0$ $\Longrightarrow \alpha=0$

   $\alpha$线性无关$\Longleftrightarrow \alpha \neq 0$

2. 向量组$\alpha_1, \cdots, \alpha_{s}$如果有一个***部分组***线性相关，那么$\alpha_1, \cdots, \alpha_{s}$线性相关。从而，如果$\alpha_1, \cdots, \alpha_{s}$线性无关，任何一个***部分组***都线性无关。

3. 凡是含有$0$的向量组，都是线性相关。

4. 向量组$\alpha_1, \cdots, \alpha_{s} (s \ge 2)$线性相关$\Longleftrightarrow$其中至少有一个向量可以由其余的向量线性表出。

   证明：有$K$中不全为0的数$k_1, \cdots, k_s$，使得$k_1\alpha_1+\cdots+k_s\alpha_s=0$，设$k_i \neq 0$，由(1)式得$\alpha_i=-\frac{k_1}{k_i}\alpha_1-\cdots-\frac{k_{i-1}}{k_i}\alpha_{i-1}-\frac{k_{i+1}}{k_i}\alpha_{i-1}-\cdots-\frac{k_{s}}{k_i}\alpha_{s}$

5. 向量组$\alpha_1, \cdots, \alpha_{s} (s \ge 2)$线性无关$\Longleftrightarrow$每一个向量不可以由其余的向量线性表出。

**命题1**：设$\beta$可以由$\alpha_1, \cdots, \alpha_{s}$线性表出，则表出方式唯一$\Longleftrightarrow$$\alpha_1, \cdots, \alpha_{s}$线性无关。

**命题2**：设$\alpha_1, \cdots, \alpha_{s}$线性无关，$\alpha_1, \cdots, \alpha_{s}, \beta$线性相关$\Longleftrightarrow$设$\beta$可以由$\alpha_1, \cdots, \alpha_{s}$线性表出。

#### 习题 3.2

1\. (1) No (2) No (3) Yes
2\. (2) 线性相关，行列式为0
5\. 线性无关，行列式不为0
9\.行列式为23
12\. 范德蒙行列式 $\prod_{1 \leq j<i \leq n}\left(a_{i}-a_{j}\right) != 0$，所以线性无关

### 3.4 极大线性无关组和向量组的秩

> 视频25第20分钟起

$<\alpha_1, \cdots, \alpha_s>=\{k_1\alpha_1+\cdots+k_s\alpha_s|k_i \in K, i=1,\cdots,s\}$

当$\alpha_1, \cdots, \alpha_{s}$线性相关时

**定义1**：向量组$\alpha_1, \cdots, \alpha_{s}$的一个部分组称为，这个向量组的一个***极大线性无关组***，如果满足：

1. 这个部分组线性无关；
2. 从向量组的其余向量（如果有的话）中，任取一个添进来，得到的新的部分组都线性相关。

**定义3**：向量组$\alpha_1, \cdots, \alpha_{s}$的任意一个极大线性无关组所含向量的个数称为向量组$\alpha_1, \cdots, \alpha_{s}$的**秩**。记作：

* $rank\{\alpha_1, \cdots, \alpha_{s}\}$

**只含0向量的向量的秩为0。**

**命题3**：向量组$\alpha_1, \cdots, \alpha_{s}$*线性无关*$\Longleftrightarrow$那么$\alpha_1, \cdots, \alpha_{s}$是向量$\alpha_1, \cdots, \alpha_{s}$的一个*极大线性无关组*。$\Longleftrightarrow$$rank\{\alpha_1, \cdots, \alpha_{s}\} = s$。

**命题4**：若向量组（$I$）可以由向量组（$II$）线性表出，则$rank(I) \leq rank(II)$

**推论4**：等价的向量组有相等的秩。

### 3.5 基与维数

设$V$是数域$K$上的线性空间。

**定义1**：$V$的一个有限子集$\{\alpha_1, \cdots, \alpha_{s}\}$线性相（无）关$\Longleftrightarrow$$\alpha_1, \cdots, \alpha_{s}$线性相（无）关。

$V$的一个无限子集$S$线性无关$\Longleftrightarrow$$S$有一个有限子集线性无关$\Longleftrightarrow$$V$的无线子集$S$线性无关。$\Longleftrightarrow$$S$任意一个有限子集线性无关。

空集$\phi$定义为线性无关。

**定义2**：设$V$是数域$K$上的线性空间，$V$的一个子集$S$如果满足下述两个条件：

1. $S$是线性无关的
2. $V$中任意一个向量可以由$S$中的向量线性表出

则称$S$是$V$的一个**基**。

在定义2中，如果$S=\{\alpha_1, \cdots, \alpha_{s}\}$，则向量组$\alpha_1, \cdots, \alpha_{s}$是$V$的一个有序基。

$\{0\}$的一个基规定为$\phi$（空集）。

**定理1**：任何一个数域上的任一个线性空间$K^n$都有一个基。

**定义3**：若$V$有一个基是有限子集，则称$V$是**有限维的**。若$V$有一个基是无限子集，则称$V$是**无限维的**。

**定理2**：若$V$是*有限维*的，则$V$的**任意两个基所含向量的个数相等**。

**定义4**：$K^n$的非零子空间$U$的一个基所含向量的个数称为$U$的维数，记作$\mathbb{dim}_kU$。

几何空间中三个不共面向量是一个基，从而集合空间是三维的。

**命题2**：如果$\mathbb{dim} V=n$，则$V$中任意$n$个线性无关的向量都是$V$的一个基。

**命题3**：设$\mathbb{dim} V=n$，若$V$中每一个向量可以由向量组$\alpha_1, \cdots, \alpha_{n}$线性表出，$\alpha_1, \cdots, \alpha_n$是$V$的一个基。

**命题4**：设$\mathbb{dim} V=n$，则$V$中任意一个线性无关的向量组都可以扩充成$V$的一个基。

#### 习题3.3

1. $\{\alpha_1, \alpha_2\}$, $rank\{\dots\}=2$.
2. $\{\alpha_1, \alpha_3\}$, $rank\{\dots\}=2$.
3. (1) $det([3,-1],[4,3]) != 0$ (2) $\{\alpha_1, \alpha_2, \alpha_3, \alpha_4\}$

设向量组$\alpha_1, \cdots, \alpha_{s}$的一个<u>极大线性无关组</u>（不妨设）为：$\alpha_1, \cdots, \alpha_{m} (m \leq s)$。

* 由于$\alpha_j=0\alpha1+\cdots+0\alpha_{j-1}+1\alpha_j+0\alpha_{j+1}+\cdots+0\alpha_s$。因此，$\alpha_1, \cdots, \alpha_{m}$中的每一个向量都可以由向量组$\alpha_1, \cdots, \alpha_{s}$线性表出。
* 反之，$\alpha_j (1 \leq i \leq M)$，可由$\alpha_1, \cdots, \alpha_{m}$线性表出。对于$\alpha_j (M < i \leq s)$ ，根据定义，$\alpha_1, \cdots, \alpha_{m}, \alpha_j$是线性相关。因此，可由可由$\alpha_1, \cdots, \alpha_{m}$线性表出（根据上一节的命题2）。

**定义2**：若向量组$\alpha_1, \cdots, \alpha_{s}$中的每一个向量都可以由向量组$\beta_1, \cdots, \beta_{r}$线性表出，则称$\alpha_1, \cdots, \alpha_{s}$可由$\beta_1, \cdots, \beta_{r}$线性表出。若向量组$\alpha_1, \cdots, \alpha_{s}$与$\beta_1, \cdots, \beta_{r}$可以**互相线性表出**，则称这两个向量组**等价**。

**命题1**：向量组$\alpha_1, \cdots, \alpha_{s}$与它的任意一个极大线性无关组**等价**。

向量组的等价具有性质：

1. 每一个向量组与自身等价（反身性）
2. 若$\alpha_1, \cdots, \alpha_{s} \cong \beta_1, \cdots, \beta_{r}$，那么$\beta_1, \cdots, \beta_{r} \cong \alpha_1, \cdots, \alpha_{s}$（对称性）
3. $\alpha_1, \cdots, \alpha_{s} \cong \beta_1, \cdots, \beta_{r}$，$\gamma_1, \cdots, \gamma_{s} \cong \beta_1, \cdots, \beta_{r}$，那么$\gamma_1, \cdots, \gamma_{s} \cong \alpha_1, \cdots, \alpha_{s}$（传递性）

**命题2**：向量组$\alpha_1, \cdots, \alpha_{s}$的任意两个个极大线性无关组**等价**。

**引理1**：设$\beta_1, \cdots, \beta_{r}$可由$\alpha_1, \cdots, \alpha_{s}$线性表出，如果$r > s$，那么$\beta_1, \cdots, \beta_{r}$线性相关。

---

> [视频32](https://www.bilibili.com/video/av39523603/?p=32)

**定义5**：设$V$是数域$K$上的线性空间，$V$的一个非空子集$S$如果满足两个条件：

1. $S$线性无关，
2. 对于$\beta \notin S$（若有的话），有$S \cup\{\beta\}$**线性相关**，那么$S$是$V$的一个**极大线性无关集**。

当$V \notin \{0\}$，$S$是$V$的一个基 $\Longleftrightarrow$ $S$是$V$的一个极大线性无关集。

**命题6**：$<\alpha_1, \dots, \alpha_s>=\{k_1\alpha_1+\dots+k_s\alpha_s|k_1,\dots,k_s \in K\}$,	则$\alpha_1, \dots, \alpha_s$的一个极大线性无关组是$<\alpha_1, \dots, \alpha_s>$的一个基，从而$dim<\alpha_1, \dots, \alpha_s> = Rank\{\alpha_1, \dots, \alpha_s\}$。

---

>  [视频33](https://www.bilibili.com/video/av39523603/?p=33)

**命题7**：$<\alpha_1, \dots, \alpha_s>=<\beta_1, \dots, \beta_r> \Longleftrightarrow \{\alpha_1, \dots, \alpha_s\} \cong \{\beta_1, \dots, \beta_r\}$。



对于一个矩阵$A$，有

* 列秩等于列空间的维度，$rank\{\alpha_1, \dots, \alpha_n\} = dim<\alpha_1, \dots, \alpha_n>$；
* 行秩等于行空间的维度，$rank\{\gamma_1, \dots, \gamma_n\}=dim<\gamma_1, \dots, \gamma_n>$。

数域$K$上$S \times n$阶梯矩阵$J$，设$J$的非零行的个数为$r$，从而$J$有$r$个主元。

$$J=\left(\begin{array}{cccccc}
{0} & \cdots & {c_{1j_1}}  & \cdots & {c_{1j_2}} & {\dots} & {c_{1, j_{r}}}  & \cdots & {c_{1 n}} \\
{0} & \cdots & {0}  & \cdots  & {c_{23}} & {\dots} & {c_{2,n-1}}  & \cdots & {c_{2 n}} \\
{\vdots} & \cdots & {\vdots}  & \cdots & {\vdots}  & \cdots & {\vdots} & \cdots & {\vdots} \\
{0} & \cdots & {0}  & \cdots & {0} & {\cdots} & {0}  & \cdots & {c_{n-1, n}} \\
{0} & \cdots & {0}  & \cdots & {0} & {\cdots} & {0}  & \cdots & {0}\end{array}\right)$$

列向量表示为$\alpha_1, \dots, \alpha_{j_1}, \dots, \alpha_{j_2}, \dots, \alpha_{j_r}, \dots, \alpha_{n}$；行向量表示为$\gamma_1, \gamma_2, \dots, \gamma_{r}$。

对于**主元构成的列向量组**，组成的矩阵式上三角矩阵，因此这些向量组**线性无关**。

它们的延伸组$\alpha_{j_1}, \alpha_{j_2}, \dots, \alpha_{j_r}$也线性无关，从而$rank\{\alpha_{j_1}, \alpha_{j_2}, \dots, \alpha_{j_r}\}=r$。



考虑集合

$$U=
\begin{Bmatrix}
\left.
\begin{pmatrix}
a_1\\
\vdots\\
a_r\\
0\\
\vdots\\
0
\end{pmatrix} \right| a_1, \dots, a_r \in K
\end{Bmatrix} \subseteq K^s$$

对于其中的每个向量，可以表示为 $a_1\epsilon_1+\dots+a_r\epsilon_r$，那么$U$的一个基是$\epsilon_1, \dots, \epsilon_r$，从而$\mathbb{dim}U = r$。

---

> [视频34](https://www.bilibili.com/video/av39523603/?p=34)

### 3.6 矩阵的秩

**定理1**：阶梯型矩阵$J$的行秩和列秩相等，它们都等于$J$的非零行个数；并且$J$的主元所在的列构成列向量组的一个极大线性无关组。

**定理**2：矩阵的初等行变换不改变矩阵的行秩。

**定理3**：矩阵的初等行变换不改变矩阵的列向量的线性相关性，从而不改变矩阵的秩。即

* 设矩阵$C$经过初等行变换变成矩阵$D$，则$C$的列向量组线性相关当且仅当$D$的列向量组线性相关；
* 设矩阵$A$经过初等行变换变成矩阵$B$，并且设$B$的第$j_1, j_2, \dots, j_r$列构成$B$的列向量组的一个极大线性无关组，则$A$的第$j_1, j_2, \dots, j_r$列构成$A$的列向量的一个极大线性无关组；从而$A$的秩等于$B$的秩。

---

> [视频35](https://www.bilibili.com/video/av39523603/?p=35)

**定理4**：<u>**任意矩阵的行秩等于它的列秩**</u>。

**定义1**：矩阵$A$的行秩与列秩统称为$A$的秩。

**推论1**：设矩阵$A$经过初等行变换化成阶梯矩阵$J$，则$A$的秩等于$J$的非零行个数。设$J$的主元所在的列示第$j_1, \dots, j_r$列，则$j_1, \dots, j_r$列构成$A$的列向量组的一个极大线性无关组。

---

> [视频36](https://www.bilibili.com/video/av39523603/?p=36)

矩阵转置不改变其秩：$$\mathtt{rank}(A)=\mathtt{rank}(A')$$

**推论2**：矩阵的初等列变换不改变矩阵的秩。

**定理5**：任一非零矩阵的秩等于它的不为零的子式的最高阶数。

---

> [视频37](https://www.bilibili.com/video/av39523603/?p=37)

**推论3**：设$s \times n$矩阵$A$的秩为$r$，则$A$的不等于零的$r$阶子式所在的列（行）构成$A$的列（行）向量组的一个极大线性无关组。

**满秩矩阵**：矩阵的秩等于级数时，其为满秩矩阵。

**推论1**：$n$级矩阵$A$满秩的充分必要条件是$|A| \neq 0$。

### 3.7 线性方程组有解的判别

**定理1（线性方程组有解判别定理）**：数域$K$上线性方程组有解的充要条件是：它的系数矩阵与增广矩阵的秩相等。

> [视频38](https://www.bilibili.com/video/av39523603/?p=38)

**定理2**：数域$K$上$n$元线性方程组有解时：

* 如果系数矩阵$A$的秩**等于**$n$，那么方程组有**唯一解**；
* 如果$A$的秩**小于**$n$，那么方程组有**无穷多个解**。

### 3.8 齐次线性方程组解集的结构

数域$K$上的$n$元齐次线性方程组
$$
x_1\alpha_1+\dots+x_n\alpha_n=0 \tag{1}
$$
的解集记作$W$。

设（1）有非零解，$W \subseteq K^n$

**性质1**：若$\gamma, \delta \in \boldsymbol{W}$，则$\gamma +  \delta \in W$。

**性质2**：若$\gamma \in \boldsymbol{W}, k \in K$，则$k\gamma\in W$。

因此，齐次线性方程组的解集$W$是$K^n$的一个子空间，称它为方程组（1）的**解空间**。

* 如果方程组的系数矩阵A的秩等于n，那么W={0}。
* 如果$\mathtt{rank}(A) < n$，那么$W$是非零子空间，此时把解空间$W$的一个基称为齐次线性方程组的一个**基础解系**。

**定义1**：齐次线性方程组有非零解时，如果它的有限多个解${\eta}_{1}, {\eta}_{2}, \cdots, {\eta}_{t}$满足：

* ${\eta}_{1}, {\eta}_{2}, \cdots, {\eta}_{t}$线性无关
* 齐次线性方程组的每个解都可以由${\eta}_{1}, {\eta}_{2}, \cdots, {\eta}_{t}$线性表出。

那么${\eta}_{1}, {\eta}_{2}, \cdots, {\eta}_{t}$是齐次线性方程组的一个**基础解系**。

**定理1**：数域$K$上$n$元齐次线性方程组的解空间W的维数为$\mathtt{dim} W = n - \mathtt{rank}(A)$。

---

> [视频39](https://www.bilibili.com/video/av39523603/?p=39)

### 3.9 非齐次线性方程组的解集结构

数域$K$上的$n$元齐次线性方程组
$$
x_1\alpha_1+\dots+x_n\alpha_n=\beta \tag{1}
$$
的解集定义为$U$。上述非齐次方程组的导出组为：
$$
x_1\alpha_1+\dots+x_n\alpha_n = 0 \tag{2}
$$
的解空间记作$W$。

**性质1**：若$\gamma, \delta \in \boldsymbol{W}$，则$\gamma -  \delta \in W$。

---

> [视频40](https://www.bilibili.com/video/av39523603/?p=40)

**性质2**：若$\gamma \in \boldsymbol{U}, \eta \in \boldsymbol{W}$，$\gamma=(a_1, \dots, a_n)', \eta=(c_1, \dots, c_n)'$, 则$\gamma + \eta \in \boldsymbol{U}$。

**定理1**：如果数域$K$上$n$元非齐次方程组（1）有解，那么它的解集$U$为：
$$
U = \{\boldsymbol{\gamma}_0 + \boldsymbol{\eta} | \boldsymbol{\eta} \in W\}
$$
其中$\eta_0$是非齐次线性方程组(1)的一个解（称为**特解**），$W$是方程组(1)的导出组的解空间。

### 3.10 子空间的运算

> 见教材下册 8.2

**定理1**：设$V_1$与$V_2$都是V的子空间，则$V_1 \cap V_2$也是$V$的子空间。

多个子空间的交：
$$
V_1 \cap V_2 \cap \cdots \cap V_s
$$
记作$\bigcap_{i=1}^{s}$，其也是$V$的一个子空间。

---

> [视频41](https://www.bilibili.com/video/av39523603/?p=41)

但注意，并集$\cup$运算后的空间不是子空间，因为不满足加法封闭。

> 可参考线性子空间的定义：[3.2 线性子空间](#32-线性子空间)

**定理2**：设$V_1$与$V_2$都是V的子空间，则$V_1 + V_2$也是$V$的子空间，称为**子空间的和**。

**命题1**：设$V_1, V_2, V_3$都是域$F$上线性空间$V$的子空间，则
$$
V_1 \cap (V_2 + V_3) \supseteq (V_1 \cap V_2) + (V_1 \cap V_3),\\
V_1 + (V_2 \cap V_3) \subseteq (V_1 + V_2) \cap (V_1 + V_3)
$$
**命题2**：设$\alpha_1, \dots, \alpha_s$和$\beta_1, \dots, \beta_s$是域$F$上线性空间$V$的两个向量组，则
$$
<\alpha_1, \cdots, \alpha_s> + <\beta_1, \cdots, \beta_s> = <\alpha_1, \cdots, \alpha_s,\beta_1, \cdots, \beta_s>
$$
**定理4**（<u>子空间的维数公式</u>）：设$V_1, V_2$都是域$F$上线性空间$V$的有限子空间，则$V_1 \cap V2， V_1+V_2$也是有限维的，并且
$$
\dim V_1 + \dim V_2 = \dim(V_1 + V_2) + \dim(V_1 \cap V_2)
$$

---

> [视频42](https://www.bilibili.com/video/av39523603/?p=42)

**推论1**：设$V_1, V_2$都是域$F$上线性空间$V$的有限子空间，则
$$
\dim(V_1 + V_2) = \dim V_1 + \dim V_2 \Longleftrightarrow V_1 \cap V_2 = 0
$$

---

**子空间的直和**

**定义1**：设$V_1, V_2$都是域$F$上线性空间$V$的有限子空间，如果$V_1 + V_2$中每个向量$\alpha$都可以唯一的表示为
$$
\alpha = \alpha_1 + \alpha_2, \quad \alpha_1 \in V_1, \alpha_2 \in V_2,
$$
那么和$V_1 + V_2$称为**<u>直和</u>**，记作$V_1 \bigoplus  V_2$。称$V_1$为$V_2$的一个**<u>补空间</u>**，反之亦然。

**定理5**：设$V_1, V_2$都是域$F$上线性空间$V$的有限子空间，则下述命题互相等价：

1. 和$V_1 + V_2$是直和；
2. 和$V_1 + V_2$中零向量的表法唯一；
3. $V_1 \cap V_2 = 0$

---

> [视频43](https://www.bilibili.com/video/av39523603/?p=43)

4. 设有$V1$的基$S_1$和$V2$的基$S_2$，如果任何一个$S_1 \cup S_2$的子集线性无关，那么$S_1 \cup S_2$线性无关。

**定理6**：设$V_1, V_2$都是域$F$上线性空间$V$的有限维子空间，则下述命题互相等价：

1. 和$V_1 + V_2$是直和；
2. $\dim (V_1 + V_2) = \dim V_1 + \dim V_2$；
3. $V_1$的一个基与$V_2$的一个基合起来是$V_1 + V_2$的一个基。

**命题3**：设$V$是域$F$上的n维线性空间，则$V$的每一个子空间$U$都有补空间。

---

> [视频44](https://www.bilibili.com/video/av39523603/?p=44)

**定理7**：设$V_1, V_2$都是域$F$上线性空间$V$的无限维子空间，则下述命题互相等价：

1. 和$V_1 + V_2$是直和；
2. $V_1$的一个基与$V_2$的一个基合起来是$V_1 + V_2$的一个基。

**命题4**：设$V$是域$F$上的无线维线性空间，则$V$的每一个子空间$U$都有补空间。

**定义2**：设$V_1, V_2, \cdots, V_s$都是域$F$上线性空间$V$的子空间，如果$V_1 + V_2 + \cdots + V_s$中每个向量$\alpha$都可以唯一的表示为
$$
\alpha = \alpha_1 + \alpha_2 + \cdots + \alpha_s, \quad \alpha_i \in V_i, i=1, 2, \cdots, s,
$$
那么和$V_1 + V_2 + \cdots + V_s$称为**<u>直和</u>**，记作$V_1 \bigoplus  V_2 \bigoplus  \cdots \bigoplus V_s$或$\bigoplus_{i=1}^s V_i$。

**定理8**：设$V_1, V_2, \cdots, V_s$都是域$F$上线性空间$V$的子空间，则下述命题互相等价：

1. 和$V_1 + V_2 + \cdots + V_s$是直和；
2. 和$\sum^s_{i=1} V_i$中零向量的表法唯一；
3. $V_i \cap (\sum_{j \neq i} V_j) = 0, i \neq 1,2,\cdots,s$。

**定理9**：设$V_1, V_2, \cdots, V_s$都是域$F$上线性空间$V$的有限维子空间，则下述命题互相等价：

1. 和$V_1 + V_2 + \cdots + V_s$是直和；
2. $\dim (V_1 + V_2 + \cdots + V_s) = \dim V_1 + \dim V_2  + \cdots + \dim V_s$；
3. $V_1$的一个基，$V_2$的一个基，$\cdots$，$V_s$的一个基，合起来是$V_1 + V_2 + \cdots + V_s$的一个基。

---

> [视频45](https://www.bilibili.com/video/av39523603/?p=45)

### 3.11 线性空间的同构

设$V_1$和$V'$都是数域$K$上的线性空间，如果$V$到$V'$有一个双射$\sigma$，并且满足：

* **保持加法运算**：$\sigma(\alpha + \beta) = \sigma(\alpha) + \sigma(\beta)$
* **保持加法数乘**：$\sigma(k\alpha) = k \sigma(\alpha)$

那么称$\sigma$是$V$到$V'$的一个同构映射，此时称呼$V$与$V'$是同构的，记作$V \cong V'$。

设$\sigma$是$V$到$V'$的一个同构映射，那么有：

**性质1**：$\sigma(0) = 0'$

**性质2**：$\sigma(-\alpha) = -\sigma(\alpha), \quad \forall \alpha \in V$

---

> [视频46](https://www.bilibili.com/video/av39523603/?p=46)

**性质3**：对于$V$中任一向量组$\alpha_1, \alpha_2, \cdots, \alpha_s$，$F$中任意一组元素$k_1, k_2, \cdots, k_s$，有
$$
\alpha(k_1\alpha_1+\cdots+k_s\alpha_s) = k_1\sigma(\alpha_1)+\cdots+k_s\sigma(\alpha_s)
$$
**性质4**：$V$中的向量组$\alpha_1, \alpha_2, \cdots, \alpha_s$线性相关当且仅当$\sigma(\alpha_1), \sigma(\alpha_2), \cdots, \sigma(\alpha_s)$是$V'$中线性相关的向量组。

**性质5**：如果$\alpha_1, \alpha_2, \cdots, \alpha_s$是$V$的一个基，那么$\sigma(\alpha_1), \sigma(\alpha_2), \cdots, \sigma(\alpha_s)$是$V'$的一个基。

**定理1**：域$F$上两个有限维线性空间**同构的充分必要条件**是它们的**维数相等**。

---

> [视频47](https://www.bilibili.com/video/av39523603/?p=47)

**推论1**：数域$K$上任何一个$n$维的线性空间$V$与$K^n$**同构**。

**命题1**：设$\sigma$是域$F$上线性空间$V$到$V'$的一个同构映射，如果$U$是$V$的一个子空间，那么$\sigma(U)$是$V'$的一个子空间；如果$U$是有限维的，那么$\sigma(U)$也是有限维的，并且$\dim \sigma(U) = \dim U$。

> [视频48](https://www.bilibili.com/video/av39523603/?p=48)

### 3.12 映射的乘法，可逆映射

**定义1**（**<u>映射的乘法</u>**）：设$f: A \rightarrow B, g: B \rightarrow C$，令$(gf)(a) := g(f(a)), \forall a \in A$，则称$gf$为$g$与$f$的乘法。

> 可以理解为相继做了两次映射（或合成）
>
> $h(gf) = (hg)f$

**定义2**（**<u>恒等变换</u>**）：线性空间$V$上的任意向量$\alpha$均映射成自身，那么这一线性变换为**恒等变换**，记作$I$。

**命题1**：假设$f: A \rightarrow B$，则$f I_A = f, I_B f = f$

> 可以理解恒等变换类似实数1，和任何数相乘仍为此数

**定义3**：设$f: A \rightarrow B$，如果存在$g: B \rightarrow A$，使得$gf = I_A$，且$fg=I_B$，那么称$f$是**可逆映射**，把$g$称为$f$的**逆映射**。

若$f$可逆，则$f$的逆映射唯一，把$f$的逆映射记作$f^{-1}$，此时有
$$
f^{-1}f = I_A, ff^{-1} = I_B
$$
因此$f^{-1}$也是可逆映射，并且$(f^{-1})^{-1} = f$。

---

> [视频49](https://www.bilibili.com/video/av39523603/?p=49)

**定理1**：$f: A \rightarrow B$是**可逆映射** $\Longleftrightarrow$ $f$是**双射**（单射+满射）。

> 可以根据可逆映射的概念来理解，可逆且唯一

### 3.13 集合的划分，等价关系

>[视频50](https://www.bilibili.com/video/av39523603/?p=50)

**定义1**：如果集合$S$是它的一些非空子集的并集，其中每两个不相等的子集的交是空集（称为不相交），那么把这些子集组成的集合称为$S$的一个**划分**。

> 这里举了个例子：日期以星期几作为一个划分

探索集合的划分

* a与b在同一个子集 $\Longleftrightarrow$ a与b模T同余，记作$a \equiv  b \quad(\text{mod } T)$。
* a与b模T同余$\Longleftrightarrow$$(a, b) \in (H_0 \times H_0)\cup(H_1 \times H_1)\cup \cdots \cup(H_6 \times H_6)$

**定义2**：设$S$是一个非空集合，$S \times S$的一个子集$W$称为$S$上的**二元关系**：

* 若$(a, b) \in W$，则称a与b有W关系，记作$a \widetilde{w} b$，或$a \sim b$；
* 若$(a, b) \notin W$，则称a与b没有W关系；

**定义3**：$S$上的一个二元关系$\sim$如果满足如下性质：

* $a \sim a, \forall a \in S$（反射性）
* 若$a \sim b$，则$b \sim a$（对称性）
* 若$a \sim b$且$b \sim c$，则$a \sim c$（传递性）

那么称$\sim$是S上的**等价关系**。

---

> [视频51](https://www.bilibili.com/video/av39523603/?p=51)

**定义4**：设$\sim$是S上的一个等价关系，任给$a \in S$，令$\bar{a} := \{x \in S | x \sim a\}$，则把$\bar{a}$称为$a$的**等价类**。

由于$a \sim a$，因此$a \in \bar{a}$，把$a$称为$\bar{a}$的一个**代表**。

**性质1**：$\bar{a} = \bar{b} \Longleftrightarrow a \sim b$。 

**性质2**：若$\bar{a} \neq \bar{b}$，则$\bar{a} \cap \bar{b} = \phi$。

**定理1**：如果集合$S$上有一个等价关系，那么所有等价类组成的集合是$S$的一个划分。

> $U_{a \in S} \bar{a} := \{x \in S| \exist c \in S,  x \in \bar{c}\}$

## 参考

1. [数学学习小组](https://github.com/yuerYDP/Math_learning_group)

[回到顶部](#丘维声高等代数学习笔记)
