# react

    因为工作需要，开始学习react整个庞大是生态圈。开始记录自己的学习过程 （脚手架，真的很难理解）
 
推荐阮一峰大师的[React 入门实例教程](http://www.ruanyifeng.com/blog/2015/03/react.html)

## react

###  我想要的效果：对react的基本操作，先写出一个基本的组件
###  简介：
###### 特点：

     仅仅只是 UI
     虚拟 DOM：最大限度减少与 DOM 的交互（类似于使用 jQuery 操作 DOM）
     单向数据流：很大程度减少了重复代码的使用
     
###### 组件化：

     可组合（Composeable）：一个组件易于和其它组件一起使用，或者嵌套在另一个组件内部。如果一个组件内部创建了另一个组件，那么说父组件拥有（own）它创建的子组件，通过这个特性，一个复杂的UI可以拆分成多个简单的UI组件
     可重用（Reusable）：每个组件都是具有独立功能的，它可以被使用在多个UI场景
     可维护（Maintainable）：每个小的组件仅仅包含自身的逻辑，更容易被理解和维护

###### 生命周期：

     Mounting：已插入真实 DOM
     Updating：正在被重新渲染
     Unmounting：已移出真实 DOM

React 为每个状态都提供了两种处理函数，will 函数在进入状态之前调用，did 函数在进入状态之后调用，三种状态共计五种处理函数。

    componentWillMount()
    componentDidMount()
    componentWillUpdate(object nextProps, object nextState)
    componentDidUpdate(object prevProps, object prevState)
    componentWillUnmount()

此外，React 还提供两种特殊状态的处理函数。

    componentWillReceiveProps(object nextProps)：已加载组件收到新的参数时调用
    shouldComponentUpdate(object nextProps, object nextState)：组件判断是否重新渲染时调用

