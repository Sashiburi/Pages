---
title: css
date: 2018-07-16 22:50:14
tags: css
---

## css选择器 ##

### 基础选择器及优先级 ###

<!-- more -->

一般来说，选择器的优先级（从上往下依次降低）是：


	1. 在属性后面使用 !important 会覆盖页面内任何位置定义的元素样式。
	
	2. 作为style属性写在元素内的样式
	
	3. id选择器
	
	4. 类选择器
	
	5. 标签选择器
	
	6. 通配符选择器

那么究竟是class选择器优先级高，还是伪类选择器优先级高呢？来段代码效果，一目了然：
 
效果：
	
![](https://i.imgur.com/ZCEk9og.png)

注意一样的样式代码，前后顺序不同，导致的效果变化：
 
效果：

![](https://i.imgur.com/X0U33TC.png)
 
也就是说：**伪类选择器和类选择器的优先级是一样的，谁在后面谁起作用，因为我们知道后面的样式会覆盖前面的样式**

### 父子选择器/派生选择器 ###

    div span i {}

**浏览器遍历父子选择器的顺序：自右向左。**

### 直接子元素选择器 ###

    div > span {}

### 并列选择器 ###

	div.wrapper {}

**多个条件选择一个元素**

### 分组选择器 ###

	div,
	p,
	span{}

## css权重 ##

!important: infinity

行内样式：1000

id选择器：100

类选择器、伪类选择器、属性选择器：10

标签选择器：1

通配符选择器：0

**进制：256**   

### 权重计算 ###

同一行相加

## 定位positon ##

### 绝对定位 ###

absolute：

1. 脱离原来位置进行定位

2. 相对于最近的有定位的父级进行定位，如果没有，则相对于文档进行定位

### 相对定位 ###

relative： 

1. 保留原来位置进行定位

2. 相对于自己原来的位置进行定位

### 固定定位 ###

fixed

1. 生成绝对定位的元素，相对于浏览器窗口进行定位。

## float ##

float:left/right

1. 浮动元素产生了浮动流，所有产生了浮动流的元素，块级元素看不到他们。产生了bfc(block fomat context)的元素，文本类属性(inline)及
 
文本都能看到他们。

