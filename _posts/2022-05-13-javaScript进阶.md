---
title: javascript进阶
date: 2022-05-13 10:34:00 +0800
categories: [xiaozhoubg]
tags: [javascript]
pin: false
author: WinnieZ

toc: true
comments: true

math: false
mermaid: true

typora-root-url: ../../WinnieZYC.github.io

---

1.原始类型和引用类型

2.浅拷贝深拷贝 深拷贝：递归和转化为json

3.包装对象 Number() String() Boolean()

![1](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/1.png)

4.对象转换 显式和隐式 parseInt和parseFloat有截取的效果

![2](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/2.png)

![3](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/3.png)

5.作用域 

![3](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/3-16524291789771.png)

6.闭包与模块化

![4](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/4.png)

![5](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/5.png)

![8](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/8.png)

![9](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/9.png)

![10](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/10.png)

![11](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/11.png)

![12](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/12.png)

![15](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/15.png)

![16](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/16.png)

![17](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/17.png)

![18](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/18.png)

![19](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/19.png)

![1](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/1-16524291926262.png)

![2](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/2-16524291926263.png)

![3](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/3-16524291926264.png)

![4](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/4-16524291926265.png)

没传入参数的是undefined,if(undefined){}

7.面向对象 class es6才有

8.原型对象

![6](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/6.png)

![7](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/7.png)

9.this关键字

![8](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/8-16524292322656.png)

箭头函数没有自己的this值，箭头函数中所使用的this都是来自函数作用域链，它的取值遵循普通普通变量一样的规则，在函数作用域链中一层一层往上找。

![9](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/9-16524292380237.png)

9.bind、apply、call方法

call 继承 多重继承

![10](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/10-16524292471408.png)

![11](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/11-16524292510869.png)

![12](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/12-165242925479710.png)

![13](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/13-165242926651711.png)

call,apply都会在改变指向时调用方法，bind会返回一个新的函数

![14](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/14.png)

![15](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/15-165242928252312.png)

11.异步编程

![16](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/16-165242928754413.png)

解决方法：

回调函数

Promise resolve

Promise async

![17](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/17-165242929188414.png)

因为函数是瞬间执行的，所以相当于没有return

![18](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/18-165242930057815.png)

getTea()方法中，fn为传入的函数，在getTea()中执行fn()然后再退出

![19](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/19-165242930733116.png)

<br/>

![20](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/20.png)

![21](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/21.png)

![22](/assets/blog_res/2022-05-13-javaScript%E8%BF%9B%E9%98%B6.assets/22.png)

正则表达式

/123/