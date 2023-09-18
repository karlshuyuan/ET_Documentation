# ET.AIComponent

## 描述

AI的控制器，管理父实体需要的一类AI，负责AI节点协程的切换。

挂载到需要使用AI的Entity上。

## 变量

| AIConfigId        | 表格中AIConfig数据，相当于AI的种类 |
|:-----------------:| ---------------------- |
| CancellationToken | 取消当前协程的入口              |
| Timer             | 重新选择节点的计时器             |
| Current           | 此类AI中当前的节点Id           |

## 方法

| AITimer | 重新选择节点的计时器的回调函数      |
| ------- | -------------------- |
| Awake   | 指定AI的种类，开启重新选择节点的计时器 |
| Destroy | 销毁此组件，恢复默认值          |
| Check   | 遍历此类AI的节点，选择合适的节点切换  |
| Cancel  | 取消当前的协程              |
