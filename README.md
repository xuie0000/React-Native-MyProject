### Android React-Native入门

|常用语|描述|
|---|---|
|JSX|看起来像XML的JavaScript语法扩展|
|`flexDirection`|决定布局的主轴横竖，colum(默认) row|
|`justifyContent`|决定其子元素沿着主轴的排列方式，可选项有：flex-start、center、flex-end、space-around、space-between以及space-evenly|
|`alignItems`|决定其子元素沿着次轴（与主轴垂直的轴，比如若主轴方向为row，则次轴方向为column）的排列方式，可选项有：flex-start、center、flex-end以及stretch(延伸)，注意：*要使stretch选项生效的话，子元素在次轴方向上不能有固定的尺寸*|
|ScrollView|通用的可滚动的容器，*适合用来显示数量不多的滚动元素*|
|Fetch|网络API|
|XMLHttpRequest API|网络API|
|WebSocket|单个 TCP 连接上提供全双工的通信信道|


我们使用两种数据来控制一个组件：`props`和`state`。`props`是在父组件中指定，而且一经指定，在被指定的组件的生命周期中则不再改变。 对于需要改变的数据，我们需要使用`state`。

#### State

- 一切界面变化都是`状态state变化`
- `state`的修改必须通过`setState()`方法
    - this.state.likes = 100; // 这样的`直接赋值修改无效！`
    - setState是一个 merge 合并操作，只修改指定属性，不影响其他属性
    - setState是`异步`操作，修改`不会马上生效`

### 参考

https://reactnative.cn/docs/getting-started/