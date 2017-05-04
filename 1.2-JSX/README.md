## 1.2.1 jsx由来


## 1.2.2 jsx语法


### xml基本语法：

* 定义标签的时候，只允许被**一个标签**包裹

* 标签一定要**闭合**

	
### 元素类型


* 标签中DOM元素标签为小写开头，组件元素为大写开头

* 注释 
	
    1. jsx中在组件子元素的位置注释是  {/**/}，其余和JS一样
	
    2. 在HTML中条件注释可以使用JavaScript判断浏览器
	
* DOCTYPE 第七章解释
	
### 元素属性
	
DOM属性都是标准规范属性。有两个例外：**class -> className , for -> htmlFor**,组件属性可以是自定义属性

```javascript

	const Header = (title,children) => (
		<h3 title={title}>{children}</h3>
	);
	<Header title="hello world">hello world</Header>

```

* **Boolean**

通常在表单中省略Boolean属性默认为true， *disabled*，*checked*等被视为false

* **展开属性**

在不知道属性是什么的时候可以先不用设置

`const component = <Component />;`

`component.props.name = name;`

`component.props.value = value;`

* **自定义HTML属性**

DOM元素中不能使用自定义属性，可以这样使用：

`<div data-attr="xxx">content</div>`

自定义标签中可以使用任何属性

### JavaScript属性表达式

如果属性值需要使用表达式，就用{ }

### HTML转义
	

			