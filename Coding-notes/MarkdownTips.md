(Markdown笔记)
---
<常规命令>
- 代码 ` `` `
- 代码块 ` ```xx``` `
- 标题 ` # ## .. `
- 换行 ` </br> `
- 分隔符 ` --- `
- 表格 (第二行 : 表示对其方式。 :---左对齐，:---:居中对其，---:右对齐)
    ```
    | column a | column b |
    | ---: | :--- | 
    | content a | content b |
    | xx | xx |
    ```
- 加粗 ` <b> xx </b> 或者 **xx** `
- 超链接 ` [超链接文本] (超链接url) `
- 图片 ` ![alt] (图片path) `
- 引用 ` > xxx `
- 改变字体颜色 `<font color='red'> xxx </font>`



---
<公式>
- 行间公式 (自动换行,语法与行内公式都相同↓)`$$ xx $$` $$ xx $$
- 行内公式 $ xx $
    - 估计值 $\hat{x}$  ,`$\hat{x}$`
    - 分数 $\frac{a}{b}$ ,`$\frac{a}{b}$`
    - 累加 $\sum_{a}^{b}$, `$\sum_{a}^{b}$`
    - 累乘 $\prod_{a}^{b}$, `$\prod_{a}^{b}$`
    - 上标 $a^{b}$,`$a^{b}$`
    - 下标 $a_{b}$,`$a_{b}$`
    - 自适应高度的括号(如包含矩阵的括号) 
    $\left( 
        \begin{bmatrix}
        a\\
        b\\
        c\\
        d
        \end{bmatrix}
    \right)$
    ```
    $\left( 
        \begin{bmatrix}
        a\\
        b\\
        c\\
        d
        \end{bmatrix}
    \right)$
    ```
    - 逆矩阵 $A^{(-1)}$,`$A^{(-1)}$`
    - 矩阵转置 $A^T$,`$A^T$`
    - 单位矩阵 $I$,`$I$`
    - $\sqrt{a+b}$,`$\sqrt{a+b}$`
    - $\sqrt[n]{a+b}$,`$\sqrt[n]{a+b}$`
    - 对数 $ln{a+b}$,`$ln{a+b}$`
    - 对数 $\log_{a}^{b}$,`$\log_{a}^{b}$`
    - 向量 $\vec{a}$,`$\vec{a}$`
    - 方括号 $[,\big[,\bigg[,\Big[,\Bigg[$, `$[,\big[,\bigg[,\Big[,\Bigg[$`



    - 花括号（在花括号前加一个斜线，花括号默认在公式内不显示） $\{$ 或 $\}$,`\{,\}`
    - 矩阵表示模板
        $$
        \begin{matrix}
        0&1&1\\
        0&1&1\\
        0&1&1\\
        \end{matrix}
        $$
        ```
        $$
        \begin{matrix}
        0&1&1\\
        0&1&1\\
        0&1&1\\
        \end{matrix}
        $$
        ```
    - 矩阵边框(将模板中matrix替换为如下表示)
        - 小括号边框 `pmatrix`
        - 中括号边框 `bmatrix`
        - 大括号边框 `Bmatrix`
        - 单竖线边框 `vmatrix`
        - 双竖线边框 `Vmatrix`
    - 单边大括号
        $$
        a = \left\{
        \begin{matrix}
        b\\
        c
        \end{matrix}
        \right.
        $$
        ```
        $$
        a = \left\{
        \begin{matrix}
        b\\
        c
        \end{matrix}
        \right.
        $$
        ```




    - 特殊数学字符
        - $\partial$, `\partial` (偏导 | partial derivative )
        - $\alpha$, `$\alpha$`
        - $\beta$, `$\beta$`
        - $\gamma$, `$\gamma$`
        - $\delta$, `$\delta$`
        - $\zeta$, `$\zeta$`
        - $\lambda$, `$\lambda$`
        - $\mu$, `$\mu$`
        - $\nu$, `$\nu$`
        - $\xi$, `$\xi$`
        - $\omicron$, `$\omicron$`
        - $\pi$, `$\pi$`
        - $\rho$, `$\rho$`
        - $\sigma$, `$\sigma$`
        - $\tau$, `$\tau$`
        - $\upsilon$, `$\upsilon$`
        - $\phi$, `$\phi$`
        - $\varphi$, `$\varphi$`
        - $\chi$, `$\chi$`
        - $\psi$, `$\psi$`
        - $\omega$, `$\omega$`
        - $\epsilon$, `$\epsilon$`
        - $\varepsilon$, `$\varepsilon$`
        - $\eta$, `$\eta$`
        - $\theta$, `$\theta$`
        - $\iota$, `$\iota$`
        - $\kappa$, `$\kappa$`
        - $\in$, `$\in$`
        - $\ni$, `$\ni$`
        - $\notin$, `$\notin$` 
        - $\pm$, `$\pm$`
        - $\times$, `$\times$`
        - $\ast$, `$\ast$`
        - $\mid$, `$\mid$`
        - $\leq$, `$\leq$`
        - $\geq$, `$\geq$`
        - $\ll$, `$\ll$`
        - $\gg$, `$\gg$`
        - $\approx$, `$\approx$`
        - $\lim$, `$\lim$`
        - $\infty$, `$\infty$`
        - $\uparrow$, `$\uparrow$`
        - $\downarrow$, `$\downarrow$`
        - 空集： $\emptyset$, `$\emptyset$`
        - 子集：$\subset$ $\supset$, `$\subset$ $\supset$`
        - 非子集：$\not\subset$, `$\not\subset$`
        - 真子集：$\subseteq$ $\supseteq$, `$\subseteq$ $\supseteq$`
        - 并集：$\cup$ $\bigcup$, `$\cup$ $\bigcup$`
        - 交集：$\cap$ $\bigcap$, `$\cap$ $\bigcap$`
        - 导数：$\prime$, `$\prime$`
        - 积分：$\int$, `$\int$`
        - 双重积分：$\iint$, `$\iint$`
        - 三重积分：$\iiint$, `$\iiint$`
        - 曲线积分：$\oint$, `$\oint$`
        - 梯度：$\nabla$, `$\nabla$`







---
特殊问题
- Vscode中如何使用markdown导出pdf
    - 首先在vscode中安装Markdown Pdf插件
    - 初始安装完后，在markdown文件内右键点击会出现导出pdf的选项。但导出pdf后发现公式没有被正确识别渲染，全部是以源码形式导出
    - 找到vscode用户路径：`C://Users/<username>/.vscode/extensions/yzane.markdown-pdf-1.4.1/template/template.html`
    - 打开这个文件，在文件末尾加上如下代码。关闭后从vscode中再次导出pdf，公式即可正常显示。
```
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/x-mathjax-config"> MathJax.Hub.Config({ tex2jax: {inlineMath: [['$', '$']]}, messageStyle: "none" });</script>
```

- <font color='red'>Vscode Markdown导PDF</font>：上一条解决方案，在复杂公式中仍然会出错（如：单边大括号，矩阵等）。经多轮实验，有效解决方案如下：
    - 在vscode中，安装拓展包‘markdown preview enhanced’, 不要用默认的preview或其他拓展包的preview功能。
    - 通过‘markdown preview enhanced’中的显示内容，确认语法是否有误，进行调整
    - 语法确认无误后，右键单击preview的页面，选择‘open in browser’，在浏览器中打开内容。浏览器中显示的内容格式与preview中显示的是完全一样的
    - 在浏览器中选择打印功能（ctrl+p），选择‘导出为pdf’，即可将浏览器中看到的内容格式，完全保存到pdf中。（不要选microsoft print to pdf，仍然可能会有格式识别错误）
    - 另注：Markdown PDF第三方插件的PDF导出功能，不能识别复杂公式（包括网上说的改.vscode template的方法，效果都不够）。pandoc第三方插件功能有报错。


