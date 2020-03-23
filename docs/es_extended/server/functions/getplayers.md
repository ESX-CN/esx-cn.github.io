# ESX.GetPlayers

```lua
ESX.GetPlayers()
```

此函数返回所有在线玩家ID的数组。

您可以使用它来访问每个玩家数据。

## ESX.GetPlayers 示例

```lua
local xPlayers = ESX.GetPlayers()

for i=1, #xPlayers, 1 do
	local xPlayer = ESX.GetPlayerFromId(xPlayers[i])

	xPlayer.addMoney(100)
	xPlayer.showNotification('Here, take ~g~$100~s~ for free!')
end
```
