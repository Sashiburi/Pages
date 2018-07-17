---
title: HTML学习
date: 2018-07-12 12:37:49
tags: html
---

## HTML简介 ##

### 什么是HTML? ###

HTML 是用来描述网页的一种语言

<!-- more -->

- HTML 指的是超文本标记语言 (Hyper Text Markup Language)
- HTML 不是一种编程语言，而是一种标记语言 (markup language)
- 标记语言是一套标记标签 (markup tag)
- HTML 使用标记标签来描述网页

### HTML 标签 ###

HTML 标记标签通常被称为 HTML 标签 (HTML tag)。

- HTML 标签是由尖括号包围的关键词，比如 `<html>`
- HTML 标签通常是成对出现的，比如 `<b>` 和 `</b>`
- 标签对中的第一个标签是开始标签，第二个标签是结束标签
- 开始和结束标签也被称为开放标签和闭合标签

### HTML 文档 = 网页 ###

- HTML 文档描述网页
- HTML 文档包含 HTML 标签和纯文本
- HTML 文档也被称为网页

Web 浏览器的作用是读取 HTML 文档，并以网页的形式显示出它们。浏览器不会显示 HTML 标签，而是使用标签来解释页面的内容：

    <html>
    <body>
    
    <h1>我的第一个标题</h1>
    
    <p>我的第一个段落。</p>
    
    </body>
    </html>

## 基本的 HTML 标签 - 四个实例 ##

### HTML 标题 ###

HTML 标题（Heading）是通过 `<h1> - <h6>` 等标签进行定义的。

**实例**

    <h1>This is a heading</h1>
    <h2>This is a heading</h2>
    <h3>This is a heading</h3>

### HTML 段落 ###

HTML 段落是通过 `<p>` 标签进行定义的。

**实例**

    <p>This is a paragraph.</p>
    <p>This is another paragraph.</p>

### HTML 链接 ###

HTML 链接是通过 `<a>` 标签进行定义的。

**实例**
    
    <a href="http://www.w3school.com.cn">This is a link</a>

### HTML 图像 ###

HTML 图像是通过 `<img>` 标签进行定义的。

    <img src="w3school.jpg" width="104" height="142" />

## HTML 元素 ##

HTML 元素指的是从开始标签（start tag）到结束标签（end tag）的所有代码。

### HTML 元素语法 ###

- HTML 元素以开始标签起始
- HTML 元素以结束标签终止
- 元素的内容是开始标签与结束标签之间的内容
- 某些 HTML 元素具有空内容（empty content）
- 空元素在开始标签中进行关闭（以开始标签的结束而结束）
- 大多数 HTML 元素可拥有属性

### 嵌套的 HTML 元素 ###

大多数 HTML 元素可以嵌套（可以包含其他 HTML 元素）。

HTML 文档由嵌套的 HTML 元素构成。

**HTML 文档实例**
    
    <html>
    
    <body>
    <p>This is my first paragraph.</p>
    </body>
    
    </html>

上面的例子包含三个 HTML 元素。

### HTML 实例解释 ###

**`<p>` 元素：**

    <p>This is my first paragraph.</p>

这个 `<p>` 元素定义了 HTML 文档中的一个段落。

这个元素拥有一个开始标签 `<p>`，以及一个结束标签 `</p>`。

元素内容是：This is my first paragraph。

**`<body>` 元素：**

    <body>
    <p>This is my first paragraph.</p>
    </body>

`<body>` 元素定义了 HTML 文档的主体。

这个元素拥有一个开始标签 `<body>`，以及一个结束标签 `</body>`。

元素内容是另一个 HTML 元素（p 元素）。

**`<html>` 元素：**

    <html>
    
    <body>
    <p>This is my first paragraph.</p>
    </body>
    
    </html>

`<html>` 元素定义了整个 HTML 文档。

这个元素拥有一个开始标签 `<html>`，以及一个结束标签 `</html>`。

元素内容是另一个 HTML 元素（body 元素）。

**不要忘记结束标签**

即使您忘记了使用结束标签，大多数浏览器也会正确地显示 HTML：

    <p>This is a paragraph
    <p>This is a paragraph

上面的例子在大多数浏览器中都没问题，但不要依赖这种做法。忘记使用结束标签会产生不可预料的结果或错误。

### 空的 HTML 元素 ###

没有内容的 HTML 元素被称为空元素。空元素是在开始标签中关闭的。

`<br>` 就是没有关闭标签的空元素（`<br>` 标签定义换行）。

在 XHTML、XML 以及未来版本的 HTML 中，所有元素都必须被关闭。

在开始标签中添加斜杠，比如 `<br />`，是关闭空元素的正确方法，HTML、XHTML 和 XML 都接受这种方式。

即使 <br> 在所有浏览器中都是有效的，但使用 `<br />` 其实是更长远的保障。

**HTML 提示：使用小写标签**

HTML 标签对大小写不敏感：`<P>` 等同于 `<p>`。许多网站都使用大写的 HTML 标签。

## HTML 属性 ##

**属性为 HTML 元素提供附加信息。**

HTML 标签可以拥有**属性**。属性提供了有关 HTML 元素的**更多的信息**。

属性总是以**名称/值对**的形式出现，比如：**name="value"**。

属性总是在 HTML 元素的**开始标签**中规定。

### 属性实例 ###

HTML 链接由 `<a> `标签定义。链接的地址在 href 属性中指定：

    <a href="http://www.w3school.com.cn">This is a link</a>

**HTML 提示：使用小写属性**

属性值应该始终被包括在引号内。双引号是最常用的，不过使用单引号也没有问题。

在某些个别的情况下，比如属性值本身就含有双引号，那么您必须使用单引号，例如：

    name='Bill "HelloWorld" Gates'

**HTML 属性参考手册**

[完整的 HTML 参考手册](http://www.w3school.com.cn/tags/index.asp)

如需更多关于标准属性的信息，请访问：

[HTML 标准属性参考手册](http://www.w3school.com.cn/tags/html_ref_standardattributes.asp)

## HTML 标题 ##

### HTML 标题 ###

标题（Heading）是通过 `<h1> - <h6>` 等标签进行定义的。

`<h1>` 定义最大的标题。`<h6>` 定义最小的标题。

**实例**

    <h1>This is a heading</h1>
    <h2>This is a heading</h2>
    <h3>This is a heading</h3>

**注释：**浏览器会自动地在标题的前后添加空行。

**注释：**默认情况下，HTML 会自动地在块级元素前后添加一个额外的空行，比如段落、标题元素前后。

**标题很重要**

请确保将 HTML heading 标签只用于标题。不要仅仅是为了产生粗体或大号的文本而使用标题。

搜索引擎使用标题为您的网页的结构和内容编制索引。

因为用户可以通过标题来快速浏览您的网页，所以用标题来呈现文档结构是很重要的。

应该将 h1 用作主标题（最重要的），其后是 h2（次重要的），再其次是 h3，以此类推。

### HTML 水平线 ###

`<hr /> `标签在 HTML 页面中创建水平线。

hr 元素可用于分隔内容。

**实例**

    <p>This is a paragraph</p>
    <hr />
    <p>This is a paragraph</p>
    <hr />
    <p>This is a paragraph</p>

**提示：**使用水平线 (`<hr>` 标签) 来分隔文章中的小节是一个办法（但并不是唯一的办法）。

### HTML 注释 ###

可以将注释插入 HTML 代码中，这样可以提高其可读性，使代码更易被人理解。浏览器会忽略注释，也不会显示它们。

注释是这样写的：

**实例**

    <!-- This is a comment -->

**注释：**开始括号之后（左边的括号）需要紧跟一个叹号，结束括号之前（右边的括号）不需要。



