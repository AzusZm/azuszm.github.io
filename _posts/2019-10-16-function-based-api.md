---
layout: post
title:  "Function-based API"
description: Record the key point need to be remember
date:   2019-10-15 20:49:36 +0530
categories: English
---

Function-based API 受 React Hooks 的启发，提供了一个全新的逻辑复用方案，且不存在上述问题。使用基于函数的 API，我们可以将相关联的代码抽取到一个 "composition function"（组合函数）中 —— 该函数封装了相关联的逻辑，并将需要暴露给组件的状态以响应式的数据源的方式返回出来。