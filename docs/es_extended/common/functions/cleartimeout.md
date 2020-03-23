# ESX.ClearTimeout

```lua
ESX.ClearTimeout(id)
```

该函数清除`ESX.SetTimeout`函数中的超时。

#### ESX.ClearTimeout 示例

```lua
local id = ESX.SetTimeout(5000, function()
	print('foo')
end)

ESX.ClearTimeout(id)
```
