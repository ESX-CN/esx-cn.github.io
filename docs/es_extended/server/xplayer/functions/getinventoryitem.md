# xPlayer.getInventoryItem

```lua
xPlayer.getInventoryItem(item)
```

This function gets an inventory item.

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明 |
|----------|-----------|----------|---------------|-------------|
| item     | string    | No       | -             | Item name   |

## Returned Table Content

| Child     | 数据类型 | 说明                           |
|-----------|-----------|---------------------------------------|
| name      | string    | Item name                             |
| count     | number    | Item count                            |
| label     | string    | Item label                            |
| weight    | number    | Item weight                           |
| usable    | boolean   | Whether or not the item is usable     |
| rare      | boolean   | Whether or not the item is rare       |
| canRemove | boolean   | Whether or not the item can be thrown |
