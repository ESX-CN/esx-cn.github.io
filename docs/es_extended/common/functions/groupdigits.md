# ESX.Math.GroupDigits

```lua
ESX.Math.GroupDigits(value)
```

此函数将数字分组，使人们更容易理解它们。在有钱显示时（例如在汽车商店购买新车时）在大多数通知中使用。

#### ESX.Math.Round 示例

```lua
local value = 5555
local valueGrouped = ESX.Math.GroupDigits(5555)

print(value, valueGrouped) -- returns 5555, 5,555
```
