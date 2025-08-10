---
title: latex syntex
date: 2025-08-10 17:50:00 +0800
categories: [syntex]
tags: [latex]     # TAG names should always be lowercase
math: true
---
# LaTeX 入门指南

## 1. 什么是 LaTeX？

LaTeX（发音：/ˈlɑːtɛx/ 或 /ˈleɪtɛx/）是一种基于 TeX 的排版系统，由 Leslie Lamport 开发。它特别适合生成包含复杂数学公式、科技图表和专业排版需求的高质量文档。

与 Word 等"所见即所得"（WYSIWYG）编辑器不同，LaTeX 采用"标记语言"方式工作——你专注于内容和结构，LaTeX 负责处理排版细节，最终生成美观、专业的文档（通常是 PDF 格式）。

## 2. 环境搭建

### 2.1 本地安装
- **TeX Live**：跨平台（Windows/macOS/Linux），包含完整的 TeX 系统（推荐新手使用）
- **MiKTeX**：主要面向 Windows，体积较小，可按需安装组件
- **MacTeX**：专为 macOS 设计的 TeX 发行版

### 2.2 在线编辑器（推荐新手）
- **Overleaf**：最流行的在线 LaTeX 编辑器，无需安装，支持实时预览和协作
- **ShareLaTeX**：与 Overleaf 类似的在线平台
- **Papeeria**：另一个在线 LaTeX 编辑工具

## 3. 第一个 LaTeX 文档

创建一个 `.tex` 文件（例如 `first_document.tex`），输入以下内容：
```tex
\documentclass{article} % 文档类型：文章

\begin{document} % 文档开始

Hello, LaTeX! 这是我的第一个 LaTeX 文档。

数学公式示例：$a^2 + b^2 = c^2$

\end{document} % 文档结束
```
### 编译过程
1. 将上述代码保存为 `.tex` 文件
2. 使用 LaTeX 编译器（如 pdflatex）编译：`pdflatex first_document.tex`
3. 会生成一个 `first_document.pdf` 文件，这就是最终的文档

## 4. 基本文档结构

一个完整的 LaTeX 文档通常包含以下部分：
```tex
\documentclass{article} % 文档类声明

% 导言区：设置文档属性、引入宏包
\usepackage[utf8]{inputenc} % 支持UTF-8编码
\usepackage{graphicx} % 支持插入图片
\usepackage{amsmath} % 增强数学公式支持

\title{文档标题}
\author{作者名称}
\date{\today} % 使用当前日期

\begin{document} % 正文开始

\maketitle % 生成标题

\section{引言} % 一级标题
这是引言部分的内容。

\subsection{研究背景} % 二级标题
这是研究背景部分。

% 更多内容...

\end{document} % 正文结束
```
## 5. 文本格式

### 5.1 基本格式\textbf{粗体文本}
```tex
\textit{斜体文本}
\textsf{无衬线字体}
\textsc{小型大写字母}
\underline{下划线文本}
```

### 5.2 段落与换行
- 空行表示新段落
- `\\` 强制换行（不开始新段落）
- `\par` 开始新段落

## 6. 数学公式

LaTeX 最强大的功能之一就是排版数学公式。

### 6.1 行内公式
用 `$...$` 包裹公式：
勾股定理：$a^2 + b^2 = c^2$

圆的面积：$S = \pi r^2$
效果：
勾股定理：$a^2 + b^2 = c^2$

圆的面积：$S = \pi r^2$

### 6.2 独立公式
用 `$$...$$` 或 `equation` 环境包裹：

```tex

$$ E = mc^2 $$

\begin{equation}
\sum_{i=1}^n i = \frac{n(n+1)}{2}
\end{equation}


\begin{equation}
\sum_{i=1}^n i = \frac{n(n+1)}{2}
\end{equation}
```

$$ E = mc^2 $$

\begin{equation}
\sum_{i=1}^n i = \frac{n(n+1)}{2}
\end{equation}


\begin{equation}
\sum_{i=1}^n i = \frac{n(n+1)}{2}
\end{equation}

### 6.3 常用数学符号

| 符号 | LaTeX 代码 | 符号 | LaTeX 代码 |
|------|------------|------|------------|
| $\alpha$ | `\alpha` | $\beta$ | `\beta` |
| $\gamma$ | `\gamma` | $\delta$ | `\delta` |
| $\sum$ | `\sum` | $\int$ | `\int` |
| $\lim$ | `\lim` | $\sqrt{x}$ | `\sqrt{x}` |
| $\frac{a}{b}$ | `\frac{a}{b}` | $\times$ | `\times` |
| $\leq$ | `\leq` | $\geq$ | `\geq` |

## 7. 列表

### 7.1 无序列表
```tex
\begin{itemize}
    \item 项目一
    \item 项目二
    \begin{itemize}
        \item 子项目1
        \item 子项目2
    \end{itemize}
    \item 项目三
\end{itemize}
```
- 项目一
- 项目二
  - 子项目1
  - 子项目2
- 项目三

### 7.2 有序列表
```tex
\begin{enumerate}
    \item 第一步
    \item 第二步
    \item 第三步
\end{enumerate}
```

1. 第一步
2. 第二步
3. 第三步

## 8. 表格
```tex
\begin{tabular}{|c|c|c|} % c表示居中对齐，|表示竖线
    \hline % 横线
    姓名 & 年龄 & 性别 \\
    \hline
    张三 & 20 & 男 \\
    \hline
    李四 & 22 & 女 \\
    \hline
\end{tabular}
```


## 9. 插入图片
```tex
% 需要在导言区引入graphicx包
\usepackage{graphicx}

\begin{figure}[h] % h表示尝试在此处插入
    \centering % 居中
    \includegraphics[width=0.5\textwidth]{image.jpg} % 图片路径和宽度
    \caption{这是图片的说明文字} % 图片标题
    \label{fig:example} % 标签，用于引用
\end{figure}
```

## 10. 交叉引用
```tex
% 引用图片
如图 \ref{fig:example} 所示...

% 引用章节
参见第 \ref{sec:introduction} 节...

% 引用公式
如公式 \ref{eq:sum} 所示...
```

## Appendix


- [overleaf](https://www.overleaf.com/)
- [overleaf-learn](https://www.overleaf.com/learn)
- [LaTeX 符号表](https://www.caam.rice.edu/~heinken/latex/symbols.pdf)
- [通用 LaTeX 数学公式语法手册](http://www.uinio.com/Math/LaTex/)
- [simpletex](https://simpletex.cn/ai/latex_ocr)