#### 认识javascript引擎

- 为什么需要javascript引擎
  - 高级的编程语言都是需要转成最终的机器指令来执行的
  - 事实上我们编写的javascript无论是交给浏览器或者node执行，最后都是需要被cpu执行的
  - 但是cpu只认识自己的指令集，实际上是机器语言，才能被cpu执行
  - 所以我们需要javascript引擎帮助我们将javascript代码翻译成cpu指令来执行
- 比较常见的javascript引擎
  - javascriptCore： webkit中的javascript引擎，Apple公司开发（小程序用的就是javascriptCore ）
  - V8：google开发的强大javascript引擎



#### 浏览器内核和JS引擎的关系

- 以webkit为例，webkit‘事实上由两部分组成：

  ![webkit](C:\Users\22452\Desktop\深入javascript高级语法\images\Webkit图解.png)

  - WebCore：负责HTML解析, css解析， 布局， 渲染等相关的工作
  - JavascriptCore： 解析， 执行Javascript代码