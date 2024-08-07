Markdown法语入门
===
[toc]

# 概要：
---
markdown的需要注意的重点+基本语法+VScode快捷键

需要注意的重点：
---
- 任何语法标记基本都需要后跟一个空格
- 块标记相关自带换行,不用操心连续键入两个Enter来换段
- 注意内联标记，键入两个Enter才能换行
- .md是markdown的后缀
- vscode使用markdown插件推荐Markdown Preview Enhanced
- vsCode的快捷键全部可以用，CTRL+/直接注释一行，可以使用行失效
- 阅读建议，除了注意重点和快捷键，其余部分扫读目录即可


# 快捷键：
-

control+K 之后松开+V=预览效果


# 语法：
-

## 1. 在文字下方使用=，表示这一行是一级标题

这是效果
=
## 2. 在文字下方使用-，表示这一行是二级标题

这是效果
-

- 用#,##,###等标记标题级别,效果略
<!-- # 一级标题 -->
<!-- ## 二级 -->
<!-- ### 三级 -->

## 3. 使用空格行表示换段落，也就是连续键入两个Enter即可。
搭配CTRL键，实现光标从任意位置开始都方便成功进行换段落

这是效果

##  4. 使用** **强调文本内容

**这是效果**

## 5. 使用** 斜体话文本内容

*这是效果*

## 6. 使用>作为一行的开始，表示引用文本。>>表示引用嵌套引用

>这是引用效果
>>这是引用中嵌套引用的效果
> - 引用中嵌套无序列表
> - *嵌套斜体*和**嵌套粗体**


## 7. 使用序号1.（英文输入法的句号）开头,表示有序列表。以此类推。可以在有序列表嵌套有序列表，键入Enter+Tab，其他和有序列表一样。注意列表嵌套一定要使用Tab键

    1. 这是效果
    2. 有序列表2
        1. 嵌入列表
        2. 键入Enter+Tab
    3. 有序列表3

## 8. 使用-开头，表示无序列表。以此类推。键入Enter+Tab,可以在无序列表中嵌套无序或有序列表。
- 一个无序列表
- 注意增加空格才能生效，生效变成**蓝色**
    - 嵌套无序列表
    1. 嵌套有序列表
    2. 嵌套**有序***列表*
    - 嵌套无序列表
    >**嵌套***引用*

## 9.代码块，使用Tab，缩进代码块内容。使用``(英文输入1旁边的那个符号)，表示代码语句。注意Enter两次。使用```包裹代码块也可以

`假设这是代码，这是效果`

这是代码的效果

`function Dog(name) {
	this.name = name;
}`

这是代码块的效果

    假设我是代码，请注意tab代码块
    <html>
        <head>
        </head>
    </html>
 
这是代码块的效果2

    function Dog(name) {
        this.name = name;
    }
这是代码块的效果3
```
    function Dog(name) {
        this.name = name;
    }
```

 
## 10. 图片和超链接直接使用HTML语法就行

这是Markdown<a href="https://markdown.com.cn/" alt="这是效果" title="超链接例子" >官方教程</a>链接

这是Markdown图片例子效果

<img href="没找图片超链接资源" alt="这是图片链接失效" title="图片">

<img href="https://markdown.com.cn/hero.png" alt="markdown官方的一个图片" title="图片">

## 11. 任务列表-[x]没完成的任务,-[ ]已经完成的任务

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
---
（这是分割线）

## 12. markdown实现目录[toc]置于开头，自动根据#的等级生成目录，但无法跳转。还有可以跳转的，暂时没用到不学
