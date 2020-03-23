# ESX.RegisterServerCallback

```lua
ESX.RegisterServerCallback(name, cb)
```

此函数注册服务回调。

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明                                                                 |
| ---- | -------- | -------- | ------ | -------------------------------------------------------------------- |
| name | string   | No       | -      | 服务回调名称                                                         |
| cb   | function | No       | -      | 回调函数，它包含不同大小的参数，具体大小取决于从客户端解析的参数数量 |

## ESX.RegisterServerCallback 示例

```lua
ESX.RegisterServerCallback('esx_myscript:setNewName', function(playerId, newName, cb))
	local xPlayer = ESX.GetPlayerFromId(playerId)
	xPlayer.setName(newName)

	cb(true)
```
