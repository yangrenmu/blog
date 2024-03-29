## HTML 中的 JavaScript

- ### script 元素
  script 有 8 个属性：

```js
1、async: 异步下载执行脚本。（立即开始下载脚本，且不能阻止页面其他动作，比如加载其他脚本。只对外部脚本有效）
2、defer: 立即下载，延迟执行。只对外部文件有效。文档被完全解析和显示之后，才执行脚本。
3、src: 文档来源。当使用这个属性时，会下载并执行脚本，但不会执行标签内的代码。
4、type: 脚本语言类型，type='module'时，可以使用，es6 的export和import。
其他的是：charset、crossorigin、integrity、language
```

- 手动创建 script 标签，并添加到文档中时，相当于给 script 标签添加了 async 属性，由于 async 属性具有兼容性问题，不同浏览器可能会表现不一。

* ### 小结
* 要包含外部 JavaScript 文件，必须将 src 属性设置为要包含文件的 URL。文件可以跟网页在同一台服务器上，也可以位于完全不同的域。

- 所有 script 元素会依照它们在网页中出现的次序被解释。在不使用 defer 和 async 属性的情况下，包含在 script 元素中的代码必须严格按次序解释。

* 对不推迟执行的脚本，浏览器必须解释完位于 script 元素中的代码，然后才能继续渲染页面的剩余部分。为此，通常应该把 script 元素放到页面末尾，介于主内容之后及 /body 标签之前。
* 可以使用 defer 属性把脚本推迟到文档渲染完毕后再执行。推迟的脚本原则上按照它们被列出的次序执行。
* 可以使用 async 属性表示脚本不需要等待其他脚本，同时也不阻塞文档渲染，即异步加载。异步脚本不能保证按照它们在页面中出现的次序执行。
* 不支持 script 标签的浏览器，使用 noscript 标签显示内容。
