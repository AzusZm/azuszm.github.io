---
layout: post
title:  "React Learning Note"
description: Record the key point need to be remember
date:   2019-09-26 17:49:36 +0530
categories: Javascript React
---
## React 初见

**根据属性来改变组件的样式、行为等**

**原子设计：**

1. *Atoms原子*。 为网页构成的基本元素。例如标签、输入，或是一个按钮，也可以为抽象的概念，例如字体、色调等。
2. *Molecules分子*。 由原子构成的简单UI组件。例如，一个表单标签，搜索框和按钮共同打造了一个搜索表单分子。
3. *Organisms组织*。 由原子及分子组成的相对复杂的UI构成物
4. *Templates模版*。 将以上元素进行排版，显示设计的底层内容结构。
5. *Pages页面*。 将实际内容（图片、文章等）套件在特定模板，页面是模板的具体实例



## React 快速入门

### L1

“React.js全家桶”，通过create-react-app来一键生成所需要的工程项目。

> 工具地址：https://github.com/facebook/create-react-app

保存文件，浏览器自动更新

> 这个实际上使用了webpack的热更新技术，参考 https://yuque.antfin-inc.com/afx-es/ffb/otnnxb

### L2

1. JSX 是 JavaScript 语言的一种语法扩展，长得像 HTML，但并不是 HTML。
2. React.js 可以用 JSX 来描述你的组件长什么样的。
3. JSX 在编译的时候会变成相应的 JavaScript 对象描述。
4. `react-dom` 负责把这个用来描述 UI 信息的 JavaScript 对象变成 DOM 元素，并且渲染到页面上。

原因：

1. 跨平台，react-dom react-canvas react-app(RN)
2. 性能，不直接操作页面上的 DOM，可以尽量少的减少浏览器重排