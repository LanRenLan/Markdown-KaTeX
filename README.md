# Markdown 和 KaTeX 指南

## Markdown

### 标题

Markdown 支持六个等级的标题，分别使用1-6个井号（`#`）来表示：

```markdown
# 标题1
## 标题2
### 标题3
#### 标题4
##### 标题5
###### 标题6
```

### 段落和换行

Markdown中的段落是由一个或多个连续的文本行组成，段落之间通过一个以上的空行来分隔。另外，可以在段落内的句子之间插入两个以上的空格来实现换行效果。

### 强调

在文本周围使用一对星号（`*`）或者下划线（`_`）来表示*斜体*。使用两对星号或者下划线表示**粗体**。使用三对星号或者下划线表示***粗斜体***。

### 列表

Markdown支持无序和有序列表。

- 无序列表使用星号、加号或者减号表示。
- 有序列表使用数字后面跟上点号表示。

### 链接和图片

链接使用 `[]()` 来表示，其中方括号中是链接的描述，圆括号中是链接的地址。

图片使用 `![]()` 来表示，其中方括号中是图片的描述，圆括号中是图片的地址。

### 代码块和行内代码

行内代码使用一对反引号（\`）来包裹。

代码块使用三对反引号来包裹，并且在第一对反引号后面可以添加语言标识，表示代码的语言类型。

### 表格

Markdown使用以下的符号来创建表格：

- 列与列之间用管道符（`|`）分隔。
- 表头与其他行之间，使用一行只包含短横线（`-`）和管道符的行进行分隔。

### 引用

Markdown 使用 `>` 来创建引用。

以上是 Markdown 的基本语法。接下来，我们将进入 KaTeX 的部分。

## KaTeX

KaTeX 是一种在网络上显示数学公式的语言。其语法和 LaTeX 的数学模式非常相似。在这个指南中，我们将介绍一些基本的 KaTeX 语法和一些数学公式的例子。

### 基本语法

KaTeX 支持大部分 LaTeX 的数学模式语法。例如：

- 上标和下标：`x^{2}`, `x_{1}`
- 分数：`\frac{a}{b}`
- 平方根和 n 次方根：`\sqrt{x}`, `\sqrt[n]{x}`
- Greek 字母：`\alpha`, `\beta`, `\gamma`, `\Gamma`, `\Delta`
- 大括号：`\{`, `\}`
- 括号和方括号：`(`, `)`, `[`, `]`
- 绝对值符号：`|x|`
-

 求和和积分：`\sum`, `\int`
- 乘号和点积：`\times`, `\cdot`

等等。

### 数学公式示例

接下来，我们会列举一些常见的数学公式作为 KaTeX 语法的示例。

**勾股定理**

对于任何直角三角形，直角两边的平方和等于斜边的平方。

$$c^{2}=a^{2}+b^{2}$$

**二项式定理**

对于所有的实数 a 和 b 以及非负整数 n，有：

$$(a+b)^{n}=\sum_{k=0}^{n}\binom{n}{k}a^{k}b^{n-k}$$

其中，\(\binom{n}{k}\) 是组合数，表示从 n 个元素中选出 k 个元素的选法数目。

**欧拉公式**

复数的一种表达方式：

$$e^{i \theta}=\cos(\theta)+i\sin(\theta)$$

**洛必达法则**

当函数的极限形式为"0/0"或"∞/∞"时，可以通过求这两个函数的导数的极限来求原极限。

$$\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$$

**拉普拉斯变换**

拉普拉斯变换能将一个函数的时间变量变换为复数的 s 域变量，常用于解常微分方程。定义为：

$$F(s) = \int_{0}^{\infty} e^{-st}f(t) dt$$

**斯特林公式**

斯特林公式提供了阶乘函数的一个近似公式：

$$n! \sim \sqrt{2 \pi n} \left(\frac{n}{e}\right)^n$$

**波尔兹曼熵公式**

热力学的基本公式之一，其中，S 是系统的熵，k 是玻尔兹曼常数，W 是微观状态的数量。

$$S = k \ln W$$

**傅立叶变换**

傅立叶变换将一个信号从时域变换到频域。定义为：

$$F(\omega) = \int_{-\infty}^{+\infty} f(t) e^{-i \omega t} dt$$

**贝塞尔函数**

贝塞尔函数是解贝塞尔微分方程的一类函数。第一类贝塞尔函数定义为：

$$J_{\nu}(x) = \frac{1}{\pi}\int_{0}^{\pi}\cos(\nu t - x\sin t) dt$$

接下来我们将进入一些复杂的公式部分。

### 复杂公式

**标准模型拉格朗日量**

标准模型是描述了微观粒子物理学的一个理论模型，其拉格

朗日量如下：

$$
\begin{aligned}
\mathcal{L}_{\text{SM}} =& - \frac{1}{4} W_{\mu \nu}^{i} W^{\mu \nu i} - \frac{1}{4} B_{\mu \nu} B^{\mu \nu} - \frac{1}{4} G_{\mu \nu}^{a} G_{a}^{\mu \nu} + \overline{Q}_{L}^{i} i \gamma^{\mu} D_{\mu} Q_{L}^{i} + \overline{u}_{R}^{i} i \gamma^{\mu} D_{\mu} u_{R}^{i} \\
&+ \overline{d}_{R}^{i} i \gamma^{\mu} D_{\mu} d_{R}^{i} + \overline{L}_{L}^{i} i \gamma^{\mu} D_{\mu} L_{L}^{i} + \overline{e}_{R}^{i} i \gamma^{\mu} D_{\mu} e_{R}^{i} - \mu^{2} \phi^{\dagger} \phi - \lambda (\phi^{\dagger} \phi)^{2} \\
&+ (D_{\mu} \phi)^{\dagger} (D^{\mu} \phi) + \overline{Q}_{L}^{i} \phi_{i j} u_{R}^{j} - \overline{Q}_{L}^{i} \tilde{\phi}_{i j} d_{R}^{j} + \overline{L}_{L}^{i} \phi_{i j} e_{R}^{j} + \text{h.c.}
\end{aligned}
$$

以上就是Markdown和KaTeX的语法和用法的全面介绍。这些公式和符号的美，在于它们可以用简单的形式，描述出复杂的现象和关系。希望你在阅读和学习这份文档的过程中，能感受到这种美。
