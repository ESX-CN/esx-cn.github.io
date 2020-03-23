# ESX.Game.GetPedMugshot

```lua
local mugshot, mugshotStr = ESX.Game.GetPedMugshot(ped)
```

此函数可生成可在各种应用中使用的ped面部照片。

## 参数

| 参数     | 数据类型   | 可选项   | 默认值         | 说明           |
|----------|-----------|----------|---------------|----------------|
| ped      | string    | No       | -             | The ped handle |

## ESX.Game.GetPedMugshot 示例

!!! warning
	使用后请务必使用 `UnregisterPedheadshot(mugshot)` ，因为游戏只允许你使用34张面部照片，如果你不注销它，一旦达到这个限制，你将不被允许使用面部照片。

```lua
ESX = nil

Citizen.CreateThread(function()
	while ESX == nil do
		TriggerEvent('esx:getSharedObject', function(obj) ESX = obj end)
		Citizen.Wait(0)
	end

	while true do
		Citizen.Wait(10)

		if IsControlJustReleased(0, 22) then -- Spacebar Key
			notification('Hello')
		end
	end
end)

function notification(msg)
	local mugshot, mugshotStr = ESX.Game.GetPedMugshot(GetPlayerPed(-1))
	ESX.ShowAdvancedNotification('Test', 'Testing!', msg, mugshotStr, 1)
	UnregisterPedheadshot(mugshot)
end
```

![面部照片效果图](https://s2.ax1x.com/2020/02/28/3rPsBt.jpg)

## 另请参阅

[ESX.ShowAdvancedNotification](../showadvancednotification.md)
