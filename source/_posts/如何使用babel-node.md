---
title: 如何使用babel-node
date: 2017-06-10 15:39:55
tags:
---
在编写完一个node程序后，假如这个程序的文件是index.js，我们一般输入以下命令运行这个程序：
node index.js

使用node执行一个程序的前提条件包括：
1）这个程序必须遵循CommonJS模块规范，即用require而不是import引用模块，用module.exports或者exports而不是export语句导出内容。
2）这个程序不能使用node不支持的ES6及以上规范支持的特性。

ES6的模块系统由于其语义丰富而又简洁的语法得到越来越广泛的应用。由于node目前不支持ES6模块系统，所以在执行程序之前，我们必须用babel将程序
编译成node理解的程序。

这样我们的工作流程就是：
1）编写程序
2）用babel编译程序
3）运行程序

bable-node是babel-cli的一部分，是一个用来运行node程序的工具。它会自动加载babel-polyfil, 编译程序。

如何使用？
1）安装babel-cli
npm install babel-cli --save-dev
2) 安装babel-preset-env
npm install babel-preset-env --save-dev
3) 配置.babelrc
{
    "presets": ["env"]
}
4）运行node_modules/.bin/babel-node index.js