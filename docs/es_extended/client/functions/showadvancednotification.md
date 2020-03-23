# ESX.ShowAdvancedNotification

```lua
ESX.ShowAdvancedNotification(sender, subject, msg, textureDict, iconType, flash, saveToBrief, hudColorIndex)
```

这个函数显示一个高级通知。

## 参数

| 参数          | 数据类型   | 可选的   | 默认值         | 说明                                                                                        		  |
|---------------|-----------|----------|---------------|---------------------------------------------------------------------------------------------------|
| sender        | string    | No       | -             | 消息通知标题																						|
| subject       | string    | No       | -             | 消息通知主题                                                                                       |
| msg           | string    | No       | -             | 消息通知内容                                                                                       |
| textureDict   | string    | No       | -             | 纹理目录, 有关可接受的值，请参见[纹理目录](#Texture_Directory)                                        |
| iconType      | number    | No       | -             | 图标类型，有关可接受的值，请参见[图标类型](#Icon_Types)                                               |
| flash         | boolean   | Yes      | false         | 闪烁通知？                                                                                         |
| savetoBreif   | boolean   | Yes      | true          | 暂时保存通知？路径：暂停菜单 > 帮助                                                                  |
| hudColorIndex | number    | Yes      | nil           | 背景颜色， 请参阅 [此视频](https://gyazo.com/68bd384455fceb0a85a8729e48216e15)以了解可用颜色          |

## ESX.ShowAdvancedNotification 示例

```lua
function notification(msg)
	local mugshot, mugshotStr = ESX.Game.GetPedMugshot(PlayerPedId())
	ESX.ShowAdvancedNotification('title', 'subject', 'msg', mugshotStr, 1)
	UnregisterPedheadshot(mugshot)
end
```

![高级同志示例效果图](https://s2.ax1x.com/2020/02/27/30hmoF.png)

## 纹理目录

要指定一个纹理目录，您可以简单地解析一个已经存在的通知图像，或者您可以使用ESX创建一个玩家面部照片。

* [现有图像](https://wiki.gtanet.work/index.php?title=Notification_Pictures)
* [玩家面部照片](game/getpedmugshot.md)

## 图标类型

| 图标类型   | 说明                |
|-----------|---------------------|
| 1         | 聊天框               |
| 2         | 电子邮件             |
| 3         | 添加好友请求         |
| 7         | 右跳箭头             |
| 8         | RP 图标              |
| 9         | $ 图标               |
