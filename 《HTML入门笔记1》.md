# HTML入门笔记

## HTML是谁发明的？
> HTML 的全名是“超文本标记语言”（HyperText Markup Language），上个世纪90年代由欧洲核子研究中心的物理学家蒂姆·伯纳斯-李（Tim Berners-Lee）发明。
它的最大特点就是支持超链接，点击链接就可以跳转到其他网页，从而构成了整个互联网。
> 引用自[网道HTML-1.1]（https://wangdoc.com/html/intro.html）

正是因为伟大的李爵士，人类开始了网上冲浪的历史，前端工程师们开始有饭吃。
![利爵士帅照](http://t2.gstatic.com/licensed-image?q=tbn:ANd9GcQi-4GrRiraxgytp4QE_LvAVI3etbINALVH_8LfqWCCeAou6h_vb5-VvOme1kAY)

## HTML 起手应该写什么?
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
## 常用的表章节的标签有哪些，分别是什么意思（h1~h6、section、article、main、aside 等等）?
- 标题h1~h6
  h1是最高级别的标题，h6是最低级别的标题。下一级标题都是上一级标题的子标题，比如，一个h1后面可以有多个h2，每个h2后面又可以有多个h3。
- 章节section
  <section>标签表示一个含有主题的独立部分，通常用在文档里面表示一个章节，比如<article>可以包含多个section。section总是多个一起使用，一个页面不能只有一个section。
- 文章article
  <article>标签表示页面里面一段完整的内容，即使页面的其他部分不存在，也具有独立使用的意义，通常用来表示一篇文章或者一个论坛帖子。它可以有自己的标题（h1到h6）。
- 段落p
  <p>标签是一个块级元素，代表文章的一个段落（paragraph）。不仅是文本，任何想以段落显示的内容，比如图片和表单项，都可以放进<p>元素。
- 头部header
  <header>标签可以用在多个场景，既可以表示整个网页的头部，也可以表示一篇文章或者一个区块的头部。如果用在网页的头部，就称为“页眉”。网站导航和搜索栏通常会放在<header>里面。
- 脚部footer
  <footer>标签表示网页、文章或章节的尾部。如果用于整张网页的尾部，就称为“页尾”，通常包含版权信息或者其他相关信息。
- 主要内容main
  <main>标签表示页面的主体内容，一个页面只能有一个<main>。
- 旁支内容aside
  <aside>标签用来放置与网页或文章主要内容间接相关的部分。网页级别的<aside>，可以用来放置侧边栏，但不一定就在页面的侧边；文章级别的<aside>，可以用来放置补充信息、评论或注释。
- 划分div
  <div> 是一个通用标签，表示一个区块（division）。它没有语义，如果网页需要一个块级元素容器，又没有其他合适的标签，就可以使用这个标签。

## 全局属性有哪些?
所有标签都有的属性：
- class
- contentdditalbe
- hidden
- id
- style
- tabindex
- title

常用的内容标签有哪些，分别是什么意思（a、strong、em、code、pre 等等）
- a
  - <a>是链接的意思，用户点击后可以跳转到指定的网址。
  - 比如 < a href="https://qq.com/">腾讯网</a>
  - <a>标签还可以放置段落、图像、多媒体等。
- strong
  - 强调内容的重要性，会以粗体显示
- em
  - 也表示强调，会以斜体表示，全称（emphasize)
- code
  - 行内标签，标签内容是计算机代码，浏览器默认以等宽字体表示。
- pre
  - 块级元素，表示保留原来的格式，浏览器会显示标签内部的换行和空格，也会以等宽字体显示标签内容。
