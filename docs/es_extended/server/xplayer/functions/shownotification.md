# xPlayer.showNotification

```lua
xPlayer.showNotification(msg, flash, saveToBrief, hudColorIndex)
```

该函数显示给玩家一个基本的通知。

## 参数

| 参数          | 数据类型 | 数据类型 | 默认值 | 说明                                                                                   |
|---------------|----------|----------|--------|----------------------------------------------------------------------------------------|
| msg           | string   | No       | -      | 要显示的信息                                                                           |
| flash         | boolean  | Yes      | false  | 闪烁通知？                                                                             |
| saveToBreif   | boolean  | Yes      | true   | 暂时保存？ 暂停菜单>帮助                                                               |
| hudColorIndex | number   | Yes      | nil    | 背景色, 请参阅[该地址](https://gyazo.com/68bd384455fceb0a85a8729e48216e15)了解可用颜色 |

## 支持的颜色语法

* `~r~` --> 红色
* `~b~` --> 蓝色
* `~g~` --> 绿色
* `~y~` --> 黄色
* `~p~` --> 紫色
* `~o~` --> 橙色
* `~c~` --> 灰色
* `~m~` --> 深灰色
* `~u~` --> 黑色
* `~n~` --> 下划线
* `~s~` --> 白色 (默认)
* `~w~` --> 白色
* `~h~` --> 加粗
