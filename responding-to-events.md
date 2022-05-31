https://beta.reactjs.org/learn/responding-to-events
## 疑惑
1. e.preventDefault() 都阻止了浏览器那些默认事件
  点击连接跳转
  表单提交
  鼠标选中文本
  滚轮放大页面
  .....
## 总结：
1. 可以通过props传递处理函数
2. 通常命名习惯 <child onXXX = {handleXXX} /> onXXX接受一个handleXXX的处理函数
3. 传递的是处理函数，而不是处理函数执行的结果 <child onXXX = {handleXXX} /> or <child onXXX = {() => handleXXX()} />
4. 使用 e.stopPropagation() 阻止事件冒泡 e.preventDefault() 阻止浏览器默认事件

