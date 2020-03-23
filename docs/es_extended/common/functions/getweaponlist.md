# ESX.GetWeaponList

```lua
ESX.GetWeaponList()
```

该函数获得完整的武器列表和标签。

#### ESX.GetWeaponList 示例

```lua
local list = ESX.GetWeaponList()

for i=1, #list, 1 do
	print(list[i].name .. ' => ' .. list[i].label)
end
```
