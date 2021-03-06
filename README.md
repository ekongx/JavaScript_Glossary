## JavaScript 常用名词解释

#### 编程范式
编程范式（Programming Paradigm）是某种编程语言典型的编程风格或者说是编程方式。

#### ECMAScript
是一种由Ecma国际通过ECMA-262标准化的脚本程序设计语言。

#### 变量
变量是对“值”的引用，使用变量等同于引用一个值。每一个变量都有一个变量名。

#### 变量提升
JavaScript引擎的工作方式是，先解析代码，获取所有被声明的变量，然后再一行一行地运行。这造成的结果，就是所有的变量的声明语句，都会被提升到代码的头部，这就叫做变量提升（hoisting）。

#### 标识符
标识符（identifier）是用来识别具体对象的一个名称。最常见的标识符就是变量名，以及后面要提到的函数名。JavaScript语言的标识符对大小写敏感，所以a和A是两个不同的标识符。

#### 保留字
是被js定义过的单词，如：var，function

#### 关键字
目前还没被js定义单词，但是以后肯能会被js定义使用的单词，也就是很有可能在未来版本的js中会成为关键字的单词。所以不能使用保留字做标识符，如果用了，一旦新版本js发布，那么你之前的程序就会报错了。

#### 语句
JavaScript程序的执行单位为行（line），也就是一行一行地执行。一般情况下，每一行就是一个语句。

#### 函数
就是一段预先设置的代码块，可以反复调用，根据输入参数的不同，返回不同的值。

#### 第一等公民
JavaScript语言将函数看作一种值，与其它值（数值、字符串、布尔值等等）地位相同。由于函数与其他数据类型地位平等，所以在JavaScript语言中又称函数为第一等公民。

#### 函数名的提升
JavaScript引擎将函数名视同变量名，所以采用function命令声明函数时，整个函数会像变量声明一样，被提升到代码头部。所以，下面的代码不会报错。

#### 函数作用域
作用域（scope）指的是变量存在的范围。Javascript只有两种作用域：一种是全局作用域，变量在整个程序中一直存在，所有地方都可以读取；另一种是函数作用域，变量只在函数内部存在。

#### 闭包
一个是可以读取函数内部的变量，另一个就是让这些变量始终保持在内存中，即闭包可以使得它诞生环境一直存在。

#### 参数
函数运行的时候，有时需要提供外部数据，不同的外部数据会得到不同的结果，这种外部数据就叫参数。

#### 传值传递
函数参数如果是原始类型的值（数值、字符串、布尔值），传递方式是传值传递（passes by value）。这意味着，在函数体内修改参数值，不会影响到函数外部。

#### 传址传递
如果函数参数是复合类型的值（数组、对象、其他函数），传递方式是传址传递（pass by reference）。也就是说，传入函数的原始值的地址，因此在函数内部修改参数，将会影响到原始值。

#### 对象
就是一种无序的数据集合，由若干个“键值对”（key-value）（属性和方法）构成。

#### 包装对象
所谓“包装对象”，就是分别与数值、字符串、布尔值相对应的Number、String、Boolean三个原生对象。这三个原生对象可以把原始类型的值变成（包装成）对象。

#### 属性
对象的每一个“键名”又称为“属性”（property）

#### 方法
如果一个属性的值为函数，通常把这个属性称为“方法”，它可以像函数那样调用。

#### 数组
数组（array）是按次序排列的一组值。每个值的位置都有编号（从0开始），整个数组用方括号表示。

#### 面向对象编程
核心思想是将真实世界中各种复杂的关系，抽象为一个个对象，然后由对象之间的分工与合作，完成对真实世界的模拟。

#### 构造函数
就是专门用来生成“对象”的函数。它提供模板，描述对象的基本结构。一个构造函数，可以生成多个对象，这些对象都有相同的结构。

#### 原型对象
原型(prototype)对象的作用，就是定义所有实例对象共享的属性和方法，所以它也被称为实例对象的原型，而实例对象可以视作从prototype对象衍生出来的。

#### 原型链
利用原型让一个引用类型集成另一个引用类型的属性和方法。

#### new命令实质
new命令通过构造函数新建实例对象，实质就是将实例对象的原型绑定构造函数的prototype属性，然后在实例对象上执行构造函数。

#### 模块
就是实现特定功能的一组方法。只要把不同的函数（以及记录状态的变量）简单地放在一起，就算是一个模块。

#### 单线程
就是指一次只能完成一件任务。如果有多个任务，就必须排队，前面一个任务完成，再执行后面一个任务，以此类推。

#### 阻塞
所谓阻塞，就是浏览器在加载js时候会阻塞浏览器的渲染操作。

#### 同步模式
就是上一段的模式，后一个任务等待前一个任务结束，然后再执行，程序的执行顺序与任务的排列顺序是一致的、同步的

#### 同步模式
每一个任务有一个或多个回调函数（callback），前一个任务结束后，不是执行后一个任务，而是执行回调函数，后一个任务则是不等前一个任务结束就执行，所以程序的执行顺序与任务的排列顺序是不一致的、异步的。


#### DOM
DOM是文档对象模型（Document Object Model）的简称，它的基本思想是把结构化文档（比如HTML和XML）解析成一系列的节点，再由这些节点组成一个树状结构（DOM Tree）。所有的节点和最终的树状结构，都有规范的对外接口，以达到使用编程语言操作文档的目的（比如增删内容）。所以，DOM可以理解成文档（HTML文档、XML文档和SVG文档）的编程接口。

#### 节点
DOM的最小组成单位叫做节点（node），一个文档的树形结构（DOM树），就是由各种不同类型的节点组成。

#### document节点
document节点是文档的根节点，每张网页都有自己的document节点。window.document属性就指向这个节点。也就是说，只要浏览器开始载入HTML文档，这个节点对象就存在了，可以直接调用。

#### Element对象
Element对象对应网页的HTML标签元素。每一个HTML标签元素，在DOM树上都会转化成一个Element节点对象（以下简称元素节点）。



---
###### 参考：
- [JavaScript 标准参考教程（alpha）--阮一峰](http://javascript.ruanyifeng.com/)
- [JavaScript高级程序设计（第3版）](https://book.douban.com/subject/10546125/)
- [javascript各种专业名词](http://www.cnblogs.com/xiaomou2014/archive/2014/07/24/3864363.html)
