# ESX.Game.GetVehicleInDirection.md

```lua
ESX.Game.GetVehicleInDirection()
```

该函数获取在玩家5个单位内载具的方向，并使用射线投射

## ESX.Game.GetVehicleInDirection 示例

```lua
local vehicle = ESX.Game.GetVehicleInDirection()

if DoesEntityExist(vehicle) then
	ESX.ShowNotification('yep there is a vehicle here!')
end
```
