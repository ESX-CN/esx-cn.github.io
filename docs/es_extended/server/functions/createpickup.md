# ESX.CreatePickup

```lua
ESX.CreatePickup(type, name, count, label, playerId, components)
```

该函数创建一个可供拾取的物品。

## 参数

| 参数       | 数据类型 | 数据类型 | 默认值 | 说明                                                                                                                                         |
|------------|----------|----------|--------|----------------------------------------------------------------------------------------------------------------------------------------------|
| type       | string   | No       | -      | The pickup type, valid inputs: `item_standard` for items, `item_money` for cash, `item_account` for an account and `item_weapon` for weapons |
| name       | string   | No       | -      | 物品，帐户或武器的名称                                                                                                                       |
| count      | number   | No       | -      | 物品，现金，帐户或武器弹药的数量                                                                                                             |
| label      | string   | No       | -      | The pickup label drawn                                                                                                                       |
| playerId   | number   | No       | -      | The player server id who created the pickup, used to determine pickup spawn point                                                            |
| components | table    | Yes      | -      | 仅在`type`为`item_weapon`（包含组件的 ipairs 表）时使用                                                                                      |
