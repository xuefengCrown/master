# master
to be master
学习最佳编程实践，向高手学习。

编程不只是技术，它更是思想。
编程语言不只是技术，而且也是思维习惯，这是改变起来最慢的东西。
主要从Lisp和Scheme，以及c, c++, python, java, perl 中学习。
更要从Linux， Unix中学习。（源代码）
从大神的书和经验中学习。
从科学方法论中学习。
从哲学中学习。

《SICP》
《Composing Programs》
《design of computer programs》

1. 自顶向下设计方法
poker-hand

2. 如果想要在函数执行前做点什么
def timecall(fn, *args): # 跟 Peter Norvig 学的
  "Call function with args; return the time in seconds and result."
  t0 = time.clock()
  result = fn(*args)
  t1 = time.clock()
  return t1-t0, result, fn.__name__

带记忆功能的递归；
函数调用统计；

3. if-else 是一种根据条件来分派操作或者返回不同值的策略
而dictionary是根据key值的不同来返回不同的值的，而因为value值可以是函数，所以dict也可以用来分派操作。
我们可以使用dictionary来替代多分支的if-else；

前两章描述了两种编程基本要素即函数和数据之间的紧密联系。我们看到可以使用高阶函数将函数当作数据来操纵。
我们也看到通过消息传递（message passing）和对象系统（object system）怎样使得数据被赋予行为。

3+. 实现generic function的四种方法，很典型很有启发。

3++. 《Composing Programs》中，实现class和instance那一节要多看几遍。

4. Lisp中
单元测试例子中，利用词法作用域规则，实现完整路径；（《Practical Common Lisp》）
声明全局变量dpath，每进入一层函数调用，即使用let绑定路径dpath，这样的话，每一层都有自己的dpath。

5. Lisp中使用宏实现词法抽象。

6. 数据生成，过滤，map，累积（《SICP》）
data enumerate
data filter
data map
data accumulate

7. 相互调用的递归
那个分形的三角形嵌套。

8. 数据抽象（rational number）
constructor and selector
抽象屏障，abstraction barrier

9. 典型数据结构
无序表
有序表
二叉树
hashing（python的set即使用此技术）

10. recursive objects（《composing programs chapter2》）






