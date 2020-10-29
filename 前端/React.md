* 1.React是一个组件化的，functional Components的命名必须是首字母大写，采用驼峰命名法MyApp
* 2.React引入css，跟html的写法不一样
html  class=“header”
React className=“header"
* 3.style
Html  字符串   <h1 style="color: #395687;backgrpund-color:black”></h1>
React Object  <h1 style={{color:"#349586”, backgroundColor=“black”, fontSize=“200px”}} ></h1>
因为这个style里是java代码，在js里写的话需要加上{}，外层的代表是java代码，内层的代表是object
* 4.React中functional和Component class的区别是什么？
声明方式不同，可以看代码
functional是一个js函数，不可以使用setState，通过props获取
如果你想让你的component有state，你需要创建Class

* 什么情况下需要用functional component
 - functional component比较容易理解，没有state和life-cycle-hooks
 - 代码量少
 - 使用体验佳，让你去分开容器控件和展示控件
所以展示控件用functional component，容器控件使用class

* React
https://www.youtube.com/watch?v=DLX62G4lc44

Redux
Store
Action
Reducer
Dispatch

使用 connect() 前，需要先定义 mapStateToProps 这个函数来指定如何把当前 Redux store state 映射到展示组件的 props 中。
除了读取 state，容器组件还能分发 action。mapDispatchToProps() 方法接收 dispatch() 方法并返回期望注入到展示组件的 props 中的回调方法
最后，使用 connect() 创建 VisibleTodoList，并传入这两个函数。
