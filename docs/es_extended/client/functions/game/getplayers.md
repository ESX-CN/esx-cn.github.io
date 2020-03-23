# ESX.Game.GetPlayers

```lua
ESX.Game.GetPlayers()
```

这个函数获取服务器中的所有在线玩家，并返回一个玩家客户端ID表。

## ESX.Game.GetPlayers 示例

```lua
local players = ESX.Game.GetPlayers()

for k,v in ipairs(players) do
	local targetPed = GetPlayerPed(v)
	print(('A player with server id %s found at %s!'):format(GetPlayerServerId(v), GetEntityCoords(targetPed)))
end
```
