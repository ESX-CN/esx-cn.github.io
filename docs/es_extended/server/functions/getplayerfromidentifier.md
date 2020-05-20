# ESX.GetPlayerFromIdentifier

```lua
ESX.GetPlayerFromIdentifier(identifier)
```

次函数将Rockstar标识符返回给ESX玩家。如果未找到玩家则返回`nil`

## ESX.GetPlayerFromIdentifier 示例

```lua
local xPlayer = ESX.GetPlayerFromIdentifier('888452e629a590b9d79245f0030b1f7b9a81d558')

if xPlayer then
	xPlayer.showNotification('Welcome Hawaii!')
else
	print('Hawaii is not in your server, good')
end
```
