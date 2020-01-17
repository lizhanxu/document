## Vue.js

渐进式框架，所谓渐进式，就是指可以一步一步、有阶段性地来使用Vue.js,不必一开始就使用所有东西。

自底向上逐层应用


声明式渲染——Vue.js 的核心

允许采用简洁的模板语法来声明式地将数据渲染进 DOM

数据和 DOM 已经被建立了关联，所有东西都是**响应式的**



Vue中的渲染是指将Vue的东西解析成原生的HTML文本



计算属性computed和方法methods的区别，只要入参不变computed会缓存计算结果，而methods在每次渲染时都要重新计算



组件化

在 Vue 里，一个组件本质上是一个拥有预定义选项的一个 Vue 实例



每个 Vue 应用都是通过用 `Vue` 函数创建一个新的 **Vue 实例**开始的
```
var vm = new Vue({
// 选项
})
```

Vue没有完全遵循MVVM模受型，但是Vue的设计也受到了它的启发。

所有的 Vue 组件都是 Vue 实例

`Object.freeze()`，会阻止修改现有的属性，也意味着响应系统无法再*追踪*变化。

Vue 实例暴露了一些有用的实例属性与方法。它们都有前缀 `$`，以便与用户定义的属性区分开来。



生命周期钩子

created：一个实例被创建之后执行代码

不要在选项属性或回调上使用箭头函数(娜姆大表达式)



MVVM模型

Model-View-ViewModel

Model用纯粹的JavaScript对象表示

View负责显示

ViewModel连接视图View和数据业务的Model层，ViewModel负责把Model的数据同步到View显示出来，还负责把View的修改同步回Model。

本质上是MVC的改进版。MVVM将其中的View 的状态和行为抽象化，让我们将视图 UI 和业务逻辑分开












JavaScript在head和body中的区别

在head中：被调用才执行。

在body中：页面加载时被执行，通常被用来生成页面的内容。