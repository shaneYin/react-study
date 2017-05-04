## React 与 DOM

### 1.6.1 ReactDOM

1. findDOMNode

	**DOM真正被添加到HTML中的生命周期方法是componentDidMount和comppponentDidUpdate**
	
	当组件被渲染到DOM中，findDOMNode返回该react组件实例相应的DOM节点，用来获取表单的value

	代码见 *findDOMNode.html*

2. render

	渲染到浏览器的DOM中的方法

### 1.6.2 DOM中的不稳定方法

***

### 1.6.3 refs

refs可以是一个回调函数 代码见 *refs1.html*

也可以是一个字符串，代码见 *refs2.html*

### 1.6.4 React之外的DOM操作