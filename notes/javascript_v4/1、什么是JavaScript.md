## 第一章：什么是 JavaScript

- ## 历史回顾

完整的 JavaScript 分为三部分：ecmascript + DOM + BOM

- ### ecmascript

```js
=> 讲了 JavaScript 的发展历程，JavaScript 由网景的工程师 Brendan Eich 推出了 js1.0 版本。
=> 随后 tc39 推出了 es1，作为 JavaScript 的实现依据，跟 js1.1 版本差不多。
=> 后面的 es2 和 es3 没有大的改动。但到了 es4 改动太大，被否。
=> 在 09 年时，推出了 es5。
=> 在 15 年，推出了 es6，增加了很多重要的改动。比如：类、模块、迭代器、生成器、箭头函数、promise、reflect、proxy 等等。 之后的 js 保持了一年一个版本迭代。
=> 16 年的 es7。
=> 17 年的 es8，增加了异步函数 async/await。
=> 18 年推出了 es9。
=> 19 年推出 es10。
```

- ### DOM
  文档对象模型（document object model）是一个应用编程接口。DOM 将页面抽象成一组分层节点。HTML、XML 页面都是右一个个节点组成。使用 DOM API 可以轻松增加、删除、修改、查询节点，主要是跟网页内容交互。

* #### DOM 级别
* DOM1 级，由两个部分组成，目标是映射文档结构：  
  DOM Core：映射 XML 文档，方便访问和操作
  DOM HTML：前者的扩展，增加了一些对象和方法

* DOM2 级，增加了一些新的模块
  DOM 视图：追踪文档不同的视图  
  DOM 事件：描述事件和处理事件接口  
  DOM 样式：处理元素 CSS 样式  
  DOM 遍历和范围：遍历和操作 DOM 树

* ### BOM
  BOM 浏览器对象模型，用于支持访问和操作浏览器的窗口，主要是跟浏览器进行交互。
  如：window、navigation、location、screen 等
