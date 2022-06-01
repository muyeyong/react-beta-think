## 为什么不使用常规的variable
用let const var定义变量和用useState定义变量有什么区别了，我以前也想到过这个问题
1. let const var定义的变量改变不能触发render
2. let const var定义的变量在render的过程中不能保存上一次的值，每次render都会初始化
那么问题来了，以前没有框架之前，用普通变量不也可以保持？ 没有渲染？

## 总结
1. 需要组件有记忆的时候，使用useSate
2. 不能在循环、条件语句中声明hook，因为hook的实现需要严格的顺序，为什么一定要使用数组结构了？
3. state之间是独立的、互不干扰的