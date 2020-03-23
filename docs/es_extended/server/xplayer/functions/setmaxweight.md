# xPlayer.setMaxWeight

```lua
xPlayer.setMaxWeight(newWeight)
```

This functions sets the max weight that the player can hold in their inventory.

## 参数

| 参数  | 数据类型 | 数据类型 | 默认值 | 说明    |
|-----------|-----------|----------|---------------|----------------|
| newWeight | number    | No       | -             | New max weight |

#### xPlayer.setMaxWeight 示例

```lua
if xPlayer.group ~= 'user' then
	xPlayer.setMaxWeight(ESX.GetConfig().MaxWeight + 30)
end
```
