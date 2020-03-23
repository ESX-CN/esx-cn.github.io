# xPlayer.addAccountMoney

```lua
xPlayer.addAccountMoney(account, money)
```

此函数可增加帐户资金。

## 参数

| 参数    | 数据类型 | 数据类型 | 默认值 | 说明                                     |
| ------- | -------- | -------- | ------ | ---------------------------------------- |
| account | string   | No       | -      | 有效帐户，可在配置文件中找到有效帐户列表 |
| money   | number   | No       | -      | 补充的金额                               |

## xPlayer.addAccountMoney 示例

```lua
	local xPlayer = ESX.GetPlayerFromId(playerId)
	xPlayer.addAccountMoney('bank', 1000)
```
