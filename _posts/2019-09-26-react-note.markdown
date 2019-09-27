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

### 环境

“React.js全家桶”，通过create-react-app来一键生成所需要的工程项目。

> 工具地址：https://github.com/facebook/create-react-app

保存文件，浏览器自动更新

> 这个实际上使用了webpack的热更新技术，参考 https://yuque.antfin-inc.com/afx-es/ffb/otnnxb

### JSX

1. JSX 是 JavaScript 语言的一种语法扩展，长得像 HTML，但并不是 HTML。
2. React.js 可以用 JSX 来描述你的组件长什么样的。
3. JSX 在编译的时候会变成相应的 JavaScript 对象描述。
4. `react-dom` 负责把这个用来描述 UI 信息的 JavaScript 对象变成 DOM 元素，并且渲染到页面上。

原因：

1. 跨平台，react-dom react-canvas react-app(RN)
2. 性能，不直接操作页面上的 DOM，可以尽量少的减少浏览器重排

### Method Render

1. React.js 中一切皆组件，一个组件类必须要实现一个 render 方法
2. JSX中class, for属性需要通过className, htmlFor关键字来代替

### 组件的组合、嵌套

1. 在JSX中可以通过标签来引入自定义组件

### 事件监听

1. on*事件只能作用于HTML标签上
2. React.js 会给每个事件监听传入一个 event 对象，这个对象提供的功能和浏览器提供的功能一致，而且它是兼容所有浏览器的。
3. bind方法

### Props

1. 为了使得组件的可定制性更强，在使用组件的时候，可以在标签上加属性来传入配置参数。
2. 组件可以在内部通过 this.props 获取到配置参数，组件可以根据 props 的不同来确定自己的显示形态，达到可配置的效果。
3. 可以通过给组件添加类属性 defaultProps 来配置默认参数。
4. props 一旦传入，你就不可以在组件内部对它进行修改。但是你可以通过父组件主动重新渲染的方式来传入新的 props，从而达到更新的效果。

### State vs Props 

1. State用于组件内部保存、控制、修改自身的状态，外部不能访问修改。
2. Props让组件使用方通过参数来定制组件的样式、行为，对于组件内部只读。
3. 函数式组件的方式来创建无状态组件

### 渲染列表

1. 通过map将数据数组转换成组件
2. 每个页面元素必须得有key作为其唯一标识

## React 进阶

### React生命周期



