# ESX.GetPlayerFromIdentifier

```lua
ESX.GetPlayerFromIdentifier(identifier)
```

此函数从（STEAM）标识符返回ESX玩家对象。 如果找不到玩家，则返回`nil`。

## ESX.GetPlayerFromIdentifier 示例

```lua
local xPlayer = ESX.GetPlayerFromIdentifier('steam:110000104ed291c')

if xPlayer then
	xPlayer.showNotification('Hello Hawaii!')
else
	print('Hawaii is not in your server')
end
```
