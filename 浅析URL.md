# 浅析URL

## URL 包含哪几部分，每部分分别有什么作用

URL = 协议 + 域名/IP + 端口号 + 路径 + 查询字符串 + 锚点

example：

https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/What_is_a_URL#%E8%87%AA%E4%B8%BB%E5%AD%A6%E4%B9%A0

HTTPS协议 + developer.mozilla.org+ :443 + zh-CN/docs/Learn/Common_questions/What_is_a_URL + #自主学习（这个是锚点，被转义城字符串了。）

HTTPS是协议，表明了浏览器必须使用何种协议，加了s，是http的安全版。还有mailto，ftp等协议。

developer.mozilla.org是域名，表明正在请求哪个web服务器，作用就是去DNS找IP地址的。因为数字难记，字母可以产生联想，容易记。这是一个三级域名，也俗称二级域名。

端口号：相当于一道门，标准的http端口是80，HTTPS是443。

zh-CN/docs/Learn/Common_questions/What_is_a_URL：是当前HTML存放在服务器上的文件路径。其实，服务器可以理解为一台没有界面的远程电脑，就是一样的文件夹。

?key1=value1&key2=value2是提供查询字符串用的。

#自主学习：相当于在页面内部加标签，实现跳转，本质上没有发送任何请求，都是在本地客户端进行的操作。

## DNS 的作用是什么，nslookup 命令怎么用

Domain name system，全称域名系统。

DNS和IP地址形成映射关系，输入域名，通过DNS查找对应的真实IP，然后访问。

nslookup 用来诊断域名解析是否正常，nslookup + google.com 直接用。



## IP 的作用是什么，ping 命令怎么用

Ip的作用是标记主机在网络中的位置，相当于户口本。

ping语法

```
ping(选项)(参数)
```

ping 选项

```
-d：使用Socket的SO_DEBUG功能；
-c<完成次数>：设置完成要求回应的次数；
-f：极限检测；
-i<间隔秒数>：指定收发信息的间隔时间；
-I<网络界面>：使用指定的网络界面送出数据包；
-l<前置载入>：设置在送出要求信息之前，先行发出的数据包；
-n：只输出数值；
-p<范本样式>：设置填满数据包的范本样式；
-q：不显示指令执行过程，开头和结尾的相关信息除外；
-r：忽略普通的Routing Table，直接将数据包送到远端主机上；
-R：记录路由过程；
-s<数据包大小>：设置数据包的大小；
-t<存活数值>：设置存活数值TTL的大小；
-v：详细显示指令的执行过程。
```

[ping详细用法的博文](https://www.cnblogs.com/machangwei-8/p/10352808.html)

## 域名是什么，分别哪几类域名

域名就是给IP地址起的名字

a.b.c

c是顶级域名，常见的有com,org,cn,edu。

b是网站名，如google，baidu,bing。

a是三级域名，可以用作业务分类，比如developer.mozilla.org，Firefox浏览器提供的开发者手册。

