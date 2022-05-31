## 为什么不使用常规的variable
用let const var定义变量和用useState定义变量有什么区别了，我以前也想到过这个问题
1. let const var定义的变量改变不能触发render
2. let const var定义的变量在render的过程中不能保存上一次的值，每次render都会初始化