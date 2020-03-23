# xPlayer.getInventory

```lua
xPlayer.getInventory(minimal)
```

该函数返回玩家库存信息。

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明                                                                                                       |
|----------|-----------|----------|---------------|-------------------------------------------------------------------------------------------------------------------|
| minimal  | boolean   | Yes      | -             | Return inventory in a key-value table where key is item name, and only add items with count over 0 to that table. |

## Returned Table Content

The returned table contains an index-value table, and for each child there is a key-value table with the following content:

| Child     | 数据类型 | 说明                           |
|-----------|-----------|---------------------------------------|
| name      | string    | Item name                             |
| count     | number    | Item count                            |
| label     | string    | Item label                            |
| weight    | number    | Item weight                           |
| usable    | boolean   | Whether or not the item is usable     |
| rare      | boolean   | Whether or not the item is rare       |
| canRemove | boolean   | Whether or not the item can be thrown |
