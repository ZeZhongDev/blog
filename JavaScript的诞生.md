# JavaScript的诞生

1993年，最早的图形接口网页浏览器 NCSA Mosaic由NCSA(国家超级电脑应用中心发明)，1994年Mosaic的主要开发人员创立了Netscape公司，发明了网景浏览器。

网景创始人马克，认为HTML需要一种胶水语言，让网页设计师和兼职程序员更好的组装图片和插件，并且代码可以直接编写在网页中。

因此，在1995年，网景招募了布兰登.艾克，尝试把scheme语言嵌入到网页中。管理层出现了分歧，但是整个公司都是Java的信徒，最终和sun公司进行商业合作，推出一门简化版的Java语言。但是布兰登，并没有这样做，因为他对Java一点兴趣都没有，应付了事，10天就设计了JavaScript。

他的思路

```
（1）借鉴C语言的基本语法；

（2）借鉴Java语言的数据类型和内存管理；

（3）借鉴Scheme语言，将函数提升到"第一等公民"（first class）的地位；

（4）借鉴Self语言，使用基于原型（prototype）的继承机制。
```



因此JavaScript的风格是简化的函数式编程+简化的面向对象编程。

布兰德曾这样形容：

```
"与其说我爱Javascript，不如说我恨它。它是C语言和Self语言一夜情的产物。十八世纪英国文学家约翰逊博士说得好：'它的优秀之处并非原创，它的原创之处并不优秀。'（the part that is good is not original, and the part that is original is not good.）"
```

JavaScript是低开高走的发展路线，至今仍然存在很多问题。

参考阮一峰的1篇博文，有很多设计的坑，目前还看不懂写的是什么。

[Javascript的10个设计缺陷](http://www.ruanyifeng.com/blog/2011/06/10_design_defects_in_javascript.html)

