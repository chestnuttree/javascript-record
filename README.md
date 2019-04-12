# javascript-record
personal learning record

## 字符集
    https://blog.csdn.net/qq_42068856/article/details/83792174#commentBox
    
    
## 客户端javascript和服务端javascript

    在客户端，JavaScript需要依赖浏览器提供的JavaScript引擎解析执行，浏览器还提供了对DOM的解析，所以客户端的JavaScript不仅应用核心语法ECMAScript，还 会操作DOM和BOM。常见的应用场景如用户交互、动画特效、表单验证、发送Ajax请求等。
    
    在服务端，JavaScript不依赖浏览器，而是由特定的运行环境提供的JavaScript引擎解析执行，例如Node.js。服务器端的JavaScript应用核心语法ECMAScript，但 是不操作DOM和BOM。它常常用来做一些在客户端做不到的事情，例如操作数据库、操作文件等等。另外，在客户端的ajax操作只能发送请求，而接收请求和做出相应的操作就需要服务器端的JavaScript来完成。
    
    简而言之，客户端的JavaScript主要用来处理页面的交互，而服务器端的JavaScript主要用来处理数据交互。

## 可选分号

   JavaScript并不是在所有换行处都填补分号：只有在缺少了分号就无法正常解析代码的时候，JavaScript才会填补分号
   有些程序员喜欢保守的在语句前加一个分号，这样哪怕之前的语句被修改了、分号被误删了，当前语句还是会正确的解析：

    var x=0
    ;[x,x+1,x+2].forEach(console.log)（ps:以‘( [’开头的语句非常常见）
    
    如果当前语句和下一行语句无法合并解析，JavaScript则在第一行后填补分号，这是通用规则。但有两个例外。 
    第一个例外，在涉及return、break和continue语句的场景中，如果这三个关键字后紧跟着换行，JavaScript则会在还行处填补分号
    第二个例外，在涉及‘++’和‘–’运算符的时候，这些运算符可以作为表达式的前缀，也可以当作表达式的后缀。如果将其用作后缀表达式，它和表达式应当在同一行，否则，行尾将填补分号，同时‘++’或‘–’将会作为下一行代码的前缀操作符并与之一起解析，如下代码：

    x
    ++
    y

    这段代码将解析为：
    x;++y;
    1

    而不是：
    x++;y;
    
  ## 数据类型
  ### 原始类型
     数字、字符串、布尔值、null、undifined
  ### 对象类型
     解释：属性的集合（每个属性都是有‘名/值对’组成，值可以是原始类型，也可以是对象）
     特殊对象：
         全局对象（global object）
         数组
         函数
         
   #### 函数
       构造函数：用函数来初始化（new）一个新对象，每个构造函数定义了一类（class）对象
       类 ：对一群具有相同特征的对象的集合的描述；
       对象：真实存在的对象个体；       
   ##### 类
     类可以看成对象类型的子类型
     Array
     Function
     Date
     RegExp
     Error

  


