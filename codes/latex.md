### 加粗 `\textbf{}`

`\bold{}` 或许能用，但不是适配性最好的方案

对数学公式应使用 `\mathbf{}`

### 无限 `\infty`

### 被圈的文本 `\textcircled{}`

```markdown
{\large{\textcircled{\small{1}}}} {\LARGE{\textcircled{\small{999}}}}
```

$\textcircled{\small 1}$

通过 `\footnotesize`、`\scriptsize`、`\tiny`，`\Large`、`\LARGE`、`\huge` 等关键字可以修改圆圈和文本大小

但这种方法许多渲染器都不支持，大多数情况还是用 `unicode` 好了

```text
① ② ③ ④ ⑤ ⑥ ⑦ ⑧ ⑨ ⓪
```

### 左向大括号

```markdown
X=
\left\{\begin{matrix}
Line 1\\
Line 2 
\end{matrix}\right.
```

$X=
\left\{\begin{matrix}
Line 1\\
Line 2
\end{matrix}\right.$

### 双括号包裹矩阵

```markdown
\begin{pmatrix}
Line 1\\
Line 2
\end{pmatrix}
```

$
\begin{pmatrix}
Line 1\\
Line 2
\end{pmatrix}$