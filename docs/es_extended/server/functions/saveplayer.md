# ESX.SavePlayer

```lua
ESX.SavePlayer(xPlayer, cb)
```

该函数保存玩家信息至数据库，它是异步保存的，保存完成后，将调用一个函数(数据类型)。

## 参数

| 参数    | 数据类型 | 数据类型 | 默认值 | 说明          |
| ------- | -------- | -------- | ------ | ------------- |
| xPlayer | number   | No       | -      | 一个 ESX 玩家 |
| cb      | function | Yes      | -      | 回调函数      |
