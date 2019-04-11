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
    ;[x,x+1,x+2].forEach(console.log)
