# 配置单页调试
```
# 参考文献
https://blog.csdn.net/supermozhe/article/details/84918314
```

# 操作技巧
```
option + B 运行html
```
# $emit 与 $on
```
$on 注册/监听实例内的事件
$emit 触发事件
# 参考文献
https://blog.csdn.net/weixin_41796631/article/details/83551997
```
# directive
```
# directive 注册标签指令 
提供 v- 标签属性使用 <div v-loading="isLoading">{{data}}</div>
参考文献
https://segmentfault.com/a/1190000012827871
```
# component
```
较高层面上，组件是自定义元素
组件注册后不需要显示的触发,只需要按照<Test :msg="message"></Test> 方式访问组件即可
# props
参考文献
https://www.jianshu.com/p/89bd18e44e73
https://segmentfault.com/a/1190000012826671

全局API 方式注册组件 API：Vue.extend()
```
# 获取script 标签的数据
```
参考文献
https://www.jianshu.com/p/bfc7241671c9
```
# extend 01
```
extend api 无法直接完成组件注册
component 无回调函数也无法完成组件注册

extend 方法生成组件需要 $mount 方可

注意$mount 生命周期 也许需要延时才能调用成功
```

# use
```
注册全局插件
如果plugin(Vue.use的第一个参数)传入一个对象，对象中包含install方法，则调用这个plugin的install方法并将整理好的数组当成参数传入install方法中。 =>plugin.install.apply(plugin, args)

参考文献
https://www.jianshu.com/p/0b9d3e3f710f
```