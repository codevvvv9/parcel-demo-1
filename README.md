# parcel 来啦～
## 新的挑战者parcel

吐槽webpack大概是没有经历过以前更蛋疼的日子吧，幸好有了新的后起之秀---[parcel](https://parceljs.org/)，它的官网老厉害了，智能提示我用了中文，真是贴心。

回顾一下`webpack`的首页

![webpack](http://p3tha6q4v.bkt.clouddn.com/18-2-13/60817621.jpg)

在对比一下`parcel`的首页

![parcel](http://p3tha6q4v.bkt.clouddn.com/18-2-13/90577657.jpg)

两者的目的是一样的，不过parcel不需要插件，而且速度快。

### 快速开始是真的快

[快速开始](https://parceljs.org/getting_started.html)

没有配置，最好以html或者js为入口，直接`npm init -y , parcel index.html`，可以实现index.js。

它会自动帮你打包到dist目录下的一个js文件里面，并复制index.html过去，而这一切只需要上面的一行代码。

![自动](http://p3tha6q4v.bkt.clouddn.com/18-2-13/25647271.jpg)

1. 一开始我的项目的目录结构
2. 执行`parcel index.html`的目录结构

而我当时搞webpack的时候的快速开始至少需要安装webpack、webpack.config.js、修改配置内容、安装插件才能实现上述的功能。

![快速开始](http://p3tha6q4v.bkt.clouddn.com/18-2-13/44326202.jpg)

### 模块化和scss的解析很方便

当我在`parcel-demo`目录下使用`parcel index.html`的时候，它自动发现我引入了`index.js。`

```html
<body>
  <script src="./index.js"></script>
</body>
```

![模块化](http://p3tha6q4v.bkt.clouddn.com/18-2-13/28380182.jpg)

1. 里面的内容是模块化的内容，它自动帮我转成了`dist/parcel-demo.js`，我在webpack的时候需要babel-loader
2. 我用的是scss,它也会自动发现，并且竟然

***

**还帮我自动下载了node-sass**

![自动下载](http://p3tha6q4v.bkt.clouddn.com/18-2-13/61347334.jpg)

其他的特点都在官网去发掘吧～希望日后`parcel`快速崛起吧

***



而现在我还是要用`webpack`的……

![](http://p3tha6q4v.bkt.clouddn.com/18-2-13/45605477.jpg)
