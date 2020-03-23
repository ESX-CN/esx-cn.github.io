# ESX.Math.Round

```lua
ESX.Math.Round(value, numDecimalPlaces)
```

此函数将数字四舍五入，并且可以选择解析多少小数位数（默认为0）

#### ESX.Math.Round 示例

```lua
local value - 5.444

print('value: ' .. value) -- returns 5.444
print('value rounded: ' .. ESX.Math.Round(value)) -- returns 5
print('value rounded: ' .. ESX.Math.Round(value, 1)) -- returns 5.4
```
