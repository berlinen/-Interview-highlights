## React supported libraries & Integration

### 什么是 Reselect 以及它是如何工作的?

Reselect是一个选择器库（用于 Redux ），它使用memoization概念。它最初编写用于计算类似 Redux 的应用程序状态的派生数据，但它不能绑定到任何体系结构或库。

Reselect 保留最后一次调用的最后输入/输出的副本，并仅在其中一个输入发生更改时重新计算结果。如果连续两次提供相同的输入，则 Reselect 将返回缓存的输出。它的 memoization 和缓存是完全可定制的。

### 什么是 Flow?

Flow 是一个静态类型检查器，旨在查找 JavaScript 中的类型错误。与传统类型系统相比，Flow 类型可以表达更细粒度的区别。例如，与大多数类型系统不同，Flow 能帮助你捕获涉及 null 的错误。

### Flow 和 PropTypes 有什么区别?

Flow 是一个静态分析工具（静态检查器），它使用该语言的超集，允许你在所有代码中添加类型注释，并在编译时捕获整个类的错误。PropTypes 是一个基本类型检查器（运行时检查器），已经被添加到 React 中。除了检查传递给给定组件的属性类型外，它不能检查其他任何内容。如果你希望对整个项目进行更灵活的类型检查，那么 Flow/TypeScript 是更合适的选择。

### 在 React 中如何使用 Font Awesome 图标?

接下来的步骤将在 React 中引入 Font Awesome：

安装 font-awesome:

```js
$ npm install --save font-awesome
```

在 index.js 文件中导入 font-awesome:

```js
import 'font-awesome/css/font-awesome.min.css'
```

在 className 中添加 Font Awesome 类:
```js
render() {
  return <div><i className={'fa fa-spinner'} /></div>
}
```

### 什么 是 React 开发者工具?

React Developer Tools 允许您检查组件层次结构，包括组件属性和状态。它既可以作为浏览器扩展（用于 Chrome 和 Firefox ），也可以作为独立的应用程序（用于其他环境，包括 Safari、IE 和 React Native）。

可用于不同浏览器或环境的官方扩展。

Chrome插件

Firefox插件

独立应用 （ Safari，React Native 等）

### 在 Chrome 中为什么 DevTools 没有加载本地文件?

如果您在浏览器中打开了本地 HTML 文件（file://...），则必须先打开Chrome Extensions并选中“允许访问文件URL”。

### 如何在 React 中使用 Polymer?

创建 Polymer 元素：

```html
<link rel='import' href='../../bower_components/polymer/polymer.html' />
```
```js
Polymer({
  is: 'calender-element',
  ready: function() {
    this.textContent = 'I am a calender'
  }
})
```

通过在 HTML 文档中导入 Polymer 组件，来创建该组件对应的标签。例如，在 React 应用程序的 index.html 文件中导入。

```html
<link rel='import' href='./src/polymer-components/calender-element.html'>
```

在 JSX 文件中使用该元素：

```js
import React from 'react'

class MyComponent extends React.Component {
  render() {
    return (
      <calender-element />
    )
  }
}

export default MyComponent

```