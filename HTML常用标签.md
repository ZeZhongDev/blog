## a 标签的用法
a 标签是可跳转的链接，点击后，浏览器会跳转到指定的网址。
格式为：
```html
<a href="https://taobao.com/">淘宝网</a>
```
除了文字外，a标签内部还可以放图片，段落，多媒体。
比如
```html
<a href="https://taobao.com/">
    <img src="/dog.png" alt="一只欢快的狗子">
</a>
```
a 标签常用的属性有：href,title,target,download
<br>
**href属性值**
是要跳转的地址，可以是URL，也可以是一个锚点。比如
```html
<a href = "#xxx">跳转到xxx </a>
<p id="xxx"> 锚点</p>
```
**title**
```html
<a href="https://xiedaimala.com/" title="跳转到饥人谷">饥人谷首页</a>
```
鼠标停留在链接上，会提示title里面的内容。我在测试的时候，怎么都看不到提示的内容，原来是title写成了tittle，vscode还不报错，只能认知看每一个字母或者用webstorm这种更智能的编辑器。
**target**
_self：当前窗口打开，默认值。
_blank：新窗口打开。
_parent：上层窗口打开，需要有父级窗口，或者类似于iframe这种嵌套，没有的等同于_self。
_top：顶层窗口打开。如果当前窗口就是顶层窗口，这个值等同于_self。
**download**
```html
<a href="dog.pngt" download>下载狗子的图片</a>
```
直接下载Google.com，这种行为在Chrome里不允许。

a标签还有mailto和tel标签，用来发邮件和打电话，都可以启动默认的邮件应用和电话拨号。
还有一些其它属性可以参考MDN。

## img 标签的用法
最简单的用法就是上文中插入狗子图片，再写一次。
```html
<img src="dao.png" alt="狗子" width="200">
```
alt是图片加载失败后，给出的文字提示。没有这个属性，用户只能看到一张裂开的图片，体验不好。
width是图片的宽度，不用加style,这是行内自带的属性，也不用加px，只有一个单位，默认是px。
height是高度，没什么好说的。
值得注意的是，可写一个值，写了width，就不用谢height，浏览器会自适应，就是保持原来宽高的比例。
切记，一个前端绝对不能让图片变形，胡乱定义width和height就会导致这种事情发生。
假如手机端显示width：2000px,无法看到全部，可以在css reset中写下面的代码，自适应。
```css
img{
    max-width: 100%;
}
```
还有事件onload和onerror，就是图片加载成功和失败分别调用的JavaScript事件。

img还是一个可替换元素，可以理解为img是一个空元素。它的内容是浏览器请求了src资源，用这个图片替换掉了img，下载之前浏览器也不知道这个标签占用的宽和高。

## table 标签的用法

```html
<table border="1px">
    <tr>
        <th scope="col">姓名</th>
        <th scope="col">性别</th>
        <th scope="col">年龄</th>
        <th scope="col">职称</th>
    </tr>
    <tr>
        <th scope="row">A君</th>
        <td>男</td>
        <td>25</td>
        <td>职员</td>
    </tr>
    <tr>
        <th scope="row">B君</th>
        <td>男</td>
        <td>31</td>
        <td>主管</td>
    </tr>
</table>
```
这个没什么好写的，还有一些合并单元格，样式，比如table-layout,border-collapse,border-spacing。

## 其他感想
HTML的学习，多查mdn，忘了就去搜，见的次数多，就眼熟了。
前端的学习，能及时反馈，挺好的。至少现在学的HTML是这样，所见即所得，不知道后面的内容bug好不好找。

