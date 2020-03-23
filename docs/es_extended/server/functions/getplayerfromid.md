# ESX.GetPlayerFromId

```lua
ESX.GetPlayerFromId(playerId)
```

此函数从服务器 ID 获取 ESX 玩家对象。对于不在线玩家返回`nil`。

## 参数

| 参数     | 数据类型 | 数据类型 | 默认值 | 说明          |
| -------- | -------- | -------- | ------ | ------------- |
| playerId | number   | No       | -      | 玩家服务器 ID |

## ESX.GetPlayerFromId 示例

```lua
RegisterNetEvent('esx_ambulancejob:healMe')
AddEventHandler('esx_ambulancejob:healMe', function()
	local xPlayer = ESX.GetPlayerFromId(source)

	if xPlayer.job.name == 'ambulance' then
		xPlayer.triggerEvent('esx_basicneeds:healPlayer')
	end
end)
```
