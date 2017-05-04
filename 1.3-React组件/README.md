## 构建react组件的三种方式
* React.createClass

```JavaScript
var Buttom = React.createClass({
	getDefaultProps(){
		return{
			color : 'blue',
			text : 'Confirm'
		};
	},
	render(){
		return (
			<button><em>{text}</em></button>
		);
	}
});
```

* ES6 class

详见*index.html*

* 无状态组件

```javascript
function Button({color : 'blue',text : 'Confirm'}){
	return (
		<button className={`btn btn-${color}`}>
			<em>{text}</em>
		</button>
	);
}
```

某些情况下必须要使用无状态组件，无状态组件的好处就是始终是保持一个实例，做到了内部优化
