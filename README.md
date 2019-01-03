虽然目前部分浏览器和 Node.js 已经支持 ES6，但由于它们对 ES6 所有的标准支持不全，这导致在开发中不敢全面地使用 ES6。

接入Babel将 ES6 编写的代码转换成目前已经支持良好的 ES5 代码。

由于 Babel 所做的事情是转换代码，所以应该通过 Loader 去接入 Babel，通过 babel-loader 去调用 Babel 完成转换工作。 在重新执行构建前，需要先安装新引入的依赖：

```
# Webpack 接入 Babel 必须依赖的模块
npm i -D babel-core babel-loader 
# 根据你的需求选择不同的 Plugins 或 Presets
npm i -D babel-preset-env
```