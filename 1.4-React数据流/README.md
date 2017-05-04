## 1.4 React数据流
> props与state

### 1.4.1 state
在*es6*当中，初始化state在**constructor**函数中`this.state={}`

在*es5*中，初始化state用一个**getinitialstate**方法，返回state对象

react当中 ，通常在**事件处理**方法中更新state的值，通常只在组件内部使用，用于组件**内部**的通信

代码见 *count_Component.html*  

### 1.4.2 props

props一般用于各种组件之间的联系