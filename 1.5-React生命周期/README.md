### 1.5.1 挂载与卸载
* 挂载

```
class App extends React.Component{
	constructor(props){
		super(props);
		this.state = {};
	}			
	componentWillMount(){
		//...
	}
	componentDidMount(){
		//...
	}
	render() {
		//...
	}
}
```

`App.defaultProps = {}`

`App.propType = {}`

App组件中的 *defaultProps* 和 *propType* 都是静态方法，所以可以在组件外部定义。
*componentWillMount*表示渲染之前，*componentDidMount*表示渲染之后

* 卸载

*componentWillUnmount*方法

### 1.5.2 数据更新过程

*conponentWillReceiveProps() { }* 
如果组件的props是由父组件传入，那么就可以调用此方法 

*shouldComponentUpdate() { }*
此方法判断组件是否更新，返回true就会继续向下执行，返回false就会停止执行

*componentWillUpdate() { }*

*componentDidUpdate() { }*

### 1.5.3 整体流程
![React 生命周期整体流程图](http://static.open-open.com/lib/uploadImg/20151028/20151028165606_134.jpg)


