# ESX.RegisterUsableItem

```lua
ESX.RegisterUsableItem(item, cb)
```

该函数注册一个可供使用的物品。

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明             |
| ---- | -------- | -------- | ------ | ---------------- |
| item | string   | No       | -      | 要注册的物品名称 |
| cb   | function | No       | -      | 回调函数         |

## ESX.RegisterUsableItem 示例

```lua
ESX.RegisterUsableItem('bread', function(playerId)
	local xPlayer = ESX.GetPlayerFromId(playerId)
	xPlayer.removeInventoryItem('bread', 1)
	xPlayer.showNotification('That was delicious.. right?')
end)
```
