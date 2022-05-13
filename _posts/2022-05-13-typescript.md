---
title: typescript
date: 2022-05-13 10:34:00 +0800
categories: [前端基础]
tags: [javascript]
pin: true
author: WinnieZ

toc: true
comments: true

math: false
mermaid: true

typora-root-url: ../../WinnieZYC.github.io

---

### object与any

https://blog.csdn.net/wq_static/article/details/50238291

```javascript
class Blablabla {
   field: Object;  //Object
}

var my = function(bla: Blablabla){
    bla.field.comingMethod();  //错误, 属性comingMethod在Object不存在
}

//修改成any类型后
class Blablabla {
   field: any;  //any
}

var my = function(bla: Blablabla){
    bla.field.comingMethod();  //OK, 只有在运行时才会关心comingMethod方法是否真的存在.
}
//可以在运行时动态分配方法
var bla = new Blablabla();
bla.field = {
    comingMethod: function(){ console.log('hi any!'); }
    //lambda表达式写法: 
    //comingMethod: ()=> console.log('hi any!')
}

my(bla); // hi any!

```

***

### getter js ts通用

![1eee6af750faf7e607501283ae2522ab](/assets/blog_res/2022-05-13-typescript.assets/1eee6af750faf7e607501283ae2522ab.png)
