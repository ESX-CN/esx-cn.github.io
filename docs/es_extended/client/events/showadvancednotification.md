# esx:showAdvancedNotification

```lua
TriggerClientEvent('esx:showAdvancedNotification', source, title, subject, msg, icon, iconType)
```

此事件显示指定源的通知。 这是当您要在发送通知时所使用服务端的功能。

#### esx:showAdvancedNotification 示例

```lua
TriggerClientEvent('esx:showAdvancedNotification', source, 'title', 'subject', 'msg', 'CHAR_AMMUNATION', 3)
```

##### 效果

![效果图](https://s2.ax1x.com/2020/02/27/302c8I.png)

###### 注意

请不要在客户端使用此事件，客户端请使用 [ESX.ShowAdvancedNotification](../functions/showadvancednotification.md)
