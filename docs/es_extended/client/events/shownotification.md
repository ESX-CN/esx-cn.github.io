# esx:showNotification

```lua
TriggerClientEvent('esx:showNotification', source, '~y~Hello ~b~world~s~!')
```

这个事件向玩家显示一个基本的通知。这是您希望在发送通知时使用的服务器端代码。

#### 支持的颜色语法

* `~r~` --> <font color=red>红色</font>
* `~b~` --> <font color=blue>蓝色</font>
* `~g~` --> <font color=greenm>绿色</font>
* `~y~` --> <font color=yellow>黄色</font>
* `~p~` --> <font color=purple>紫色</font>
* `~o~` --> <font color=orange>橙色</font>
* `~c~` --> <font color=grey>灰色</font>
* `~m~` --> <font color=darkgrey>深灰色</font>
* `~u~` --> <font color=blank>黑色</font>
* `~n~` --> <u>下划线</u>
* `~s~` --> <font color=white>白色</font> (**默认**)
* `~w~` --> <font color=white>白色</font>
* `~h~` --> **粗体**
* `~nrt~` --> ?

###### Note

请不要在客户端使用此事件，客户端请使用 [ESX.ShowNotification](../functions/shownotification.md)
