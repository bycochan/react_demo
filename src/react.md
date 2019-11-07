## react 学习
在 JavaScript 中，true && expression 总是返回 expression，而 false && expression 总是返回 false。

### 元素渲染
ReactDOM.render()
### 组件
注意： 
* 获取属性的值用的是this.props.属性名
* 创建的组件名称首字母必须大写。
* 为元素添加css的class时，要用className。
* 组件的style属性的设置方式也值得注意，要写成style={{width: this.state.witdh}}

1. 函数组件
   ```
   function Welcome(props) {
    return <h1>Hello, {props.name}</h1>;
   }
   ```
2. class 组件
   ```
   class Welcome extends React.Component {
     render() {
       return <h1>Hello, {this.props.name}</h1>;
     }
   }
   ```
### state 
声明：
```
  constructor(props) {
    super(props);
    this.state = {name: value};
  }
```
修改：
`this.setState({})`
### 事件处理
* React 事件的命名采用小驼峰式（camelCase），而不是纯小写。
* 使用 JSX 语法时你需要传入一个函数作为事件处理函数，而不是一个字符串。
