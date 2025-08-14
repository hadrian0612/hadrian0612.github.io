---
title: markdown syntex
date: 2025-08-10 17:50:00 +0800
categories: [syntex]
tags: [markdown]     # TAG names should always be lowercase
pin: false # 将文章置顶
math: true
mermaid: true
---

# 标题
使用`#`，可表示1-6级标题。
```md
# 一级标题
## 二级标题
### 三级标题
```
# 段落
段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用两个以上空格加上回车（引用中换行省略回车）。

# 区块引用
```md
> 区块引用
>> 嵌套引用
```
> 区块引用
>> 嵌套引用



# 代码区块
```c
void main()
{
printf("Hello, Markdown.");
}
```

# 强调

```md
*斜体*，_斜体_
**粗体**，__粗体__
```
*斜体*，_斜体_  

**粗体**，__粗体__

# 列表
使用`·`、`+`、或`-`标记无序列表，如：
> \-（+\*） 第一项
> \-（+\*） 第二项
> \- （+\*）第三项

**注意**：标记后面最少有一个_空格_或_制表符_。若不在引用区块中，必须和前方段落之间存在空行。

效果：
> + 第一项
> + 第二项
> + 第三项

有序列表的标记方式是将上述的符号换成数字,并辅以`.`，如：
> 1 . 第一项   
> 2 . 第二项    
> 3 . 第三项    

效果：
> 1. 第一项
> 2. 第二项
> 3. 第三项

# 分割线
分割线最常使用就是三个或以上`*`，还可以使用`-`和`_`。

# 链接
```md
[bilibili](https://www.bilibili.com/)
```
[bilibili](https://www.bilibili.com/)

# 图片
```md
![image_name](/favicons/web-app-manifest-512x512.png)
https://cdn.jsdelivr.net/gh/hadrian0612/image/favicons/web-app-manifest-512x512.png
```
![image_name](/favicons/web-app-manifest-512x512.png)

# 转义字符
```md
\ 使得符号变普通符号
```

# 符号'`'

```md
`123`
```

`123`

# 表格
使用竖线 `|` 分隔列，短横线 `-` 表示表头分隔。
```md
| 姓名 | 年龄 | 职业   |
|------|------|--------|
| 张三 | 25   | 工程师 |
| 李四 | 30   | 设计师 |
```

效果：  

| 姓名 | 年龄 | 职业   |
|------|------|--------|
| 张三 | 25   | 工程师 |
| 李四 | 30   | 设计师 |

# Appendix
[Markdown是什么](https://github.com/younghz/Markdown)
