## 缓存组件的作用：保留当前组件的状态

### 应用场景：从当前组件跳转到另一个组件，缓存当前组件的状态

### 需要注意的是：如果父组件设置为缓存组件后，父组件中的子组件也会被缓存，也就y意味着父组件中的mounted和子组件中的mounted都只会执行一次

* 使用keep-alive缓存组件，当前组件的mounted不能多次触发，即不能多次请求数据
    解决方法是：将mounted换为activated()，activated()是keep-alive组件激活时调用， deactivated() 则是 keep-alive 组件停用时调用