# xPlayer.addInventoryItem

```lua
xPlayer.addInventoryItem(item, count)
```

此功能添加库存物品。

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明          |
|----------|-----------|----------|---------------|----------------------|
| item     | string    | No       | -             | 物品名称            |
| count    | number    | No       | -             | 要添加的数目 |

!!! warning
      This function will not check if the player weight limit exceeds. Recommended to use in comibation with [xPlayer.canCarryItem(item, count)](cancarryitem.md)

## xPlayer.addInventoryItem 示例

```lua
if targetXPlayer.canCarryItem(itemName, itemCount) then
	sourceXPlayer.removeInventoryItem(itemName, itemCount)
	targetXPlayer.addInventoryItem   (itemName, itemCount)
else
	sourceXPlayer.showNotification('Target player could not hold all of that.')
end
```
