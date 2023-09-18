# ET.AIDispatcherComponent

## 描述

AI节点逻辑的分发器

## 变量

| Instance   | 单例入口         |
| ---------- | ------------ |
| AIHandlers | 存储和查找所有的节点逻辑 |

## 方法

| Awake   | 初始化单例，加载所有节点逻辑存入AIHandlers字典 |
| ------- | ---------------------------- |
| Load    | 热重载时重新加载所有节点逻辑存入AIHandlers字典 |
| Destroy | 数据恢复默认值                      |
