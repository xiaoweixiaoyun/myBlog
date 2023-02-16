---
title: 什么是PromiseLike
date: 2023/02/06
tags: 面试、问答
categories: 每日一问
description: 在手机的迭代更新中越来越多的手机不断的更新出世，各种样式层出不起。
keywords: Promise、Primise/A+
cover: /img/md/js.jpg
---

# 问题描述
>如何判断一个值是不是PromiseLike？

# 代码实现
```javascript
/**
 * 判断一个值是不是PromiseLike
 */
function isPromiseLike(value) {
  return (value !== null 
  && (typeof value === 'object' || typeof value === 'function') 
  && typeof value.then === 'function')
}
```
