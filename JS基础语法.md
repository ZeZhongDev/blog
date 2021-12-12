

## 表达式和语句

一条语句执行一个动作，一个表达式产生一个值。

一个表达式执行后一定会生成一个值，哪怕是var name，也会有undefined。

语句不一定会产生值，语句主要是来执行动作，程序有一系列的语句构成。

## 标识符的规则



在JavaScript中，标识符只能包含字母或数字或下划线（“_”）或美元符号（“$”），且不能以数字开头。 标识符与字符串不同之处在于字符串是数据，而标识符是代码的一部分。 在JavaScript 中，无法将标识符转换为字符串，但有时可以将字符串解析为标识符。

## if else 语句



```js
if (condition) {
  code to run if condition is true
} else {
  run some other code instead
}
```

## while for 语句

```js
var n = 0;
var x = 0;

while (n < 3) {
  n++;
  x += n;
}
```



## break continue

**continue 语句“跳过”循环中的一个迭代。**

```js
i = 0;
n = 0;
while (i < 5) {
   i++;
   if (i === 3) {
      continue;
   }
   n += i;
}
```

**break 语句“跳出”循环。**

```js
for (i = 0; i < 10; i++) {
    if (i === 3) { break; }
    text += "number is " + i + "<br>";
}
```

## label

从执行的语句块中跳出来

```js
const cars = ["BMW", "Volvo", "Saab", "Ford"];
list: {
  text += cars[0] + "<br>";
  text += cars[1] + "<br>";
  break list;
  text += cars[2] + "<br>";
  text += cars[3] + "<br>";
}
```





