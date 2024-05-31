# 电子笔记基础——Markdown与Latex

来自视频：https://www.bilibili.com/video/BV1Fg411j7CW/?vd_source=1d0891b41fe4e23dbf197eaf61dfa468

## 第一部分 Markdown使用

---

### 常用输入

cm^3^，H~2~O (^^上标，~~下标)

[] + TOC 目录

:joy: 表情包见[emoji表](./emoji_table.md)

---

### 快捷键

Ctrl + 1/2/3/4/5/6/0 切换到对应级别标题

Ctrl+/- 改变标题级别

Ctrl + / 进入源代码模式

Ctrl + T 表格

Ctrl + K 链接

Ctrl + Shift + Q 或 > + space 引用

Ctrl + B 加粗

Ctrl + I 倾斜

Ctrl + U 下划线

Ctrl + Q 高亮（高级设置中自定义键位）

---

### 列表

无序列表 “-” / “+” / “*” ，Ctrl + ] or tab 降级，Ctrl + [ 升级

- AAA

- BBB
    - BBA
    - BBB
- CCC



有序列表 数字 + .，  Ctrl + ] or tab 降级，Ctrl + [ 升级

1. dsa 
2. das 
    1. dsad
        1. ​	dsd 
    2. dsad
3. dsad



任务列表 Ctrl + Shift + X （或在”段落“选项卡中找到）

- [x] 早餐
- [x] 午餐
- [ ] 晚餐

---

### 代码

行内代码 `int num = 1` （打开源代码模式查看输入方式）

代码块 Ctrl + Shift + K

```c
for (int i = 0 i < 4; i++)
{
	PID_Calc(&pmotor[i]);
}
```

---

行内公式$sin2x=2sinxcosx$

公式块 Ctrl + Shift + M
$$
E_{\rm k} = \frac1 2 m v^2
\tag {1.1}
$$

---

### 表格

|      | MON  | TUE  | WED  | THU  | FRI  | SAT  | SUN  |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 早餐 |      |      |      |      |      |      |      |
| 午餐 |      |      |      |      |      |      |      |
| 晚餐 |      |      |      |      |      |      |      |

---

### 引用

[^]脚注

> 这是一个引用[^1]

[^1]:这是一个测试，对脚注的测试

---

### 链接

[链接名称](https://www.bilibili.com/video/BV1Fg411j7CW/?spm_id_from=333.999.0.0&vd_source=1d0891b41fe4e23dbf197eaf61dfa468)

如[前面](# 第一部分 Markdown使用)所说

---

### 图片

普通插入方式(前三种针对本地，最后一种针对网络)

方式一：绝对路径 / 直接粘贴

![](E:\College Data\Technic Learning\Markdown And Latex\img/infantry3.jpg)

方式二：相对路径（.表示当前目录，..表示上一级目录）

![](./img/infantry3.jpg)

方式三：Html标签

<img src="./img/infantry3.jpg" style="zoom:10%;" />

方式四：网络图片

<img src="https://rm-static.djicdn.com/teams/1525667569344-logo_green_800x800.png?x-oss-process=image/resize,h_64,m_lfit">

---

图床插入：暂时用不到，掠过





## 第二部分 Latex公式

---

### 希腊字母

$$
\alpha, \beta, \delta, \lambda, \phi, \varphi \\
\Alpha, \Beta, \Delta, \Lambda, \Phi
$$
上标^，下标_，上下标多于一个字符时，使用大括号标注

默认斜体，加“rm”或者“\text”表示直立体/罗马体（roman）；英文字母只有在表示变量或单一字符的函数名称时，才可使用斜体，其余情况都应使用直立体/罗马体

---

### 运算符

$$
+,-, \times, \cdot, \div \\
\log_6 10 \\
\frac {1} {s + 1} \, \sqrt[3]{x + y} \\
\lim_{x \to 0} \frac{x}{\sin x} \\
\sum_{i = 0}^N \,\prod_{i = 0}^N \\
\int_{-\infty}^0 f(x)\,\text{d}x \\
\iint, \iiint, \iiiint, \oint, \oiint, \oiiint \\
$$

---

### 其它符号

$$
\infty, \partial, \nabla, \propto, \degree \\
\cup, \cap, \in, \notin, \subset, \subseteq, \subsetneq, \subsetneqq, \varnothing \\
\forall, \exists, \nexists, \because, \therefore, \cdots, \vdots, \ddots \\
\pm, \mp, >, <, \ge, \le, \gg, \ll, \ne, \approx, \equiv \\
\vec x, \overrightarrow{AB}, \bar x, \overline{AB} \\
\lceil, \rceil, \lfloor, \rfloor \\
\left(0, \frac {1} {a} \right) \\
\left. \frac {\partial f} {\partial x} \right |_{x=0}
$$

---

### 环境输入

begin 和 end用于建立环境

分段函数
$$
f(x) = 
\begin{cases}
\sin x, & -\pi \le x \le \pi \\
0, & \text{其它}
\end{cases}
$$
矩阵
$$
\bf A = 
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{bmatrix}
,
\bf B^{\rm T} = 
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
,
\bf C = 
\begin{vmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{vmatrix}
$$
