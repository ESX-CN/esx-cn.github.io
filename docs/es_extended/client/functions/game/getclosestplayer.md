# ESX.Game.GetClosestPlayer

```lua
ESX.Game.GetClosestPlayer(coords)
```

此函数获取最近的玩家。

## 参数

| 参数     | 数据类型   | 可选项    | 默认值            | 说明                      |
|----------|-----------|----------|-------------------|---------------------------|
| coords   | vector3   | Yes      | (玩家坐标值)       | 要搜索的坐标               |

## ESX.Game.GetClosestPlayer 示例

```lua
local closestPlayer, closestDistance = ESX.Game.GetClosestPlayer()

if closestPlayer == -1 or closestDistance > 3.0 then
	ESX.ShowNotification('There\'s no players nearby you!')
else
	ESX.ShowNotification(('Found %s, they are %s unit(s) away'):format(GetPlayerName(closestPlayer), closestDistance))
end
```
