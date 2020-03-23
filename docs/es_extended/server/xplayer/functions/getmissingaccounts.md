# xPlayer.getMissingAccounts

```lua
xPlayer.getMissingAccounts(cb)
```

This function gets missing accounts. It's an internal function used when saving player data to database and should not be used.

## 参数

| 参数 | 数据类型 | 数据类型 | 默认值 | 说明                                                              |
|----------|-----------|----------|---------------|--------------------------------------------------------------------------|
| cb       | function  | No       | -             | Callback function with `missingAccounts` (index-value table) as 参数 |

## Returned Table Content

The returned table contains an index-value table, and for each child there is a key-value table with the following content:

| Key          | Value         |
|--------------|---------------|
| Account name | Account label |
