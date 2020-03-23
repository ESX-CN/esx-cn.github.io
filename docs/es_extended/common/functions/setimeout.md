# ESX.SetTimeout

```lua
ESX.SetTimeout(msec, cb)
```

此函数设置一个超时，该超时需要两个参数：毫秒（毫秒）和cb（回调）。

#### ESX.SetTimeout 示例

```lua
local id = ESX.SetTimeout(5000, function()
	print('foo')
end)
```
