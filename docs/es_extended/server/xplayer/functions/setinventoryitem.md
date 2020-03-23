# xPlayer.setInventoryItem

```lua
xPlayer.setInventoryItem(item, count)
```

This function sets an inventory item count

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明                                                   |
|----------|-----------|----------|---------------|---------------------------------------------------------------|
| item     | string    | No       | -             | Item name, valid items can be found in database table `items` |
| count    | number    | No       | -             | New item count                                                |


!!! warning
      This function will not check if the player weight limit exceeds. Recommended to use in comibation with [xPlayer.canCarryItem(item, count)](cancarryitem.md)
