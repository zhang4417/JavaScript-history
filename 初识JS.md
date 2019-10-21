
## JavaScript 的历史
* 1995年，【网景】招募了布兰登·艾克，目标是把[Scheme](https://zh.wikipedia.org/wiki/Scheme)语言嵌入到Netscape Navigator浏览器当中，艾克在1995年5月仅花了十天时间就把原型设计出来了。
* 最初命名为Mocha，1995年9月改名为LiveScript，同年12月，Netscape Navigator 2.0 Beta 3中部署时被重命名为JavaScript。但其实与Java完全不同，因此人们对JavaScript造成了巨大误解。
* JavaScript推出后在浏览器上大获成功，【微软】公司在不久后就为Internet Explorer 3浏览器推出了JScript，以与处于市场领导地位的网景产品同台竞争。
* 1996年11月，网景正式向ECMA（欧洲计算机制造商协会）提交语言标准。1997年6月，ECMA以JavaScript语言为基础制定了ECMAScript标准规范ECMA-262。JavaScript成为了ECMAScript最著名的实现之一。
  
JavaScript的基本特点如下：
1. 是一种解释性脚本语言（代码不进行预编译）。
2. 主要用来向HTML页面添加交互行为。
3. 可以直接嵌入HTML页面，但写成单独的js文件有利于结构和行为的分离。

JavaScript常用来完成以下任务：

1. 嵌入动态文本于HTML页面
2. 对浏览器事件作出响应
3. 读写HTML元素
4. 在数据被提交到服务器之前验证数据
5. 检测访客的浏览器信息
6. 控制cookies，包括创建和修改等

JavaScript从支持许多C语言的结构化编程语法（例如if条件语句、while循环、switch语句、do-while循环等）。但作用域是一个例外：JavaScript只支持使用var关键字来定义变量的函数作用域。ECMAScript加入了let关键字来支持块级作用域，意味着JavaScript现在既支持函数作用域又支持块级作用域。正如C语言一样，JavaScript中的表达式和语句是不同的。与C不同，JavaScript支持自动在语句末添加分号;这在另一方面也是他的一个缺点。

以下是一个简单的JavaScript Hello World︰
~~~HTML
<!DOCTYPE HTML>
<html>
    <head>
    <title>简单的JavaScript Hello World</title>
        <script type="text/javascript">
            document.write("Hello, world!");   // 在浏览器视窗内直接显示
            alert("Hello, world!");            // 弹窗显示
            console.log("Hello, world!");      // 在控制台（console）里显示，需要先开启开发工具控制台
        </script>
    </head>
    <body>
　　　　HTML内容……
    </body>
</html>
~~~

Javascript缺陷——[阮一峰日志](ruanyifeng.com/blog/2011/06/10_design_defects_in_javascript.html)：
1. 不适合开发大型程序
2. 非常小的标准库
3. null和undefined
4. 全局变量难以控制
5. 自动插入行尾分号
6. 加号运算符
7. NaN
8. 数组和对象的区分
9. ==用来判断两个值是否相等。当两个值类型不同时，会发生自动转换，得到的结果非常不符合直觉。
10. 基本类型的包装对象
    
如果遵守良好的编程规范，加上第三方函数库的帮助，Javascript的这些缺陷大部分可以回避。随着引擎如V8和框架如Node.js的发展，及其事件驱动及异步IO等特性，JavaScript逐渐被用来编写服务器端程序。且在近几年中，Node.js的出世，让JavaScript也具有了一定的服务器功能，且在某些方面比PHP的效果更为显著。
