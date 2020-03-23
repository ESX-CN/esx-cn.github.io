# xPlayer.getCoords

```lua
xPlayer.getCoords(useVector)
```

This function returns the player's current coordinates on the server. The 数据类型 boolean `useVector` 参数 is for returning a `vector3` type. Keep in mind that the coords sync interval can be adjusted in the configuration file in case you want to get precise player coords.

## 参数

| 参数  | 数据类型 | 数据类型 | 默认值 | 说明                                                                          |
|-----------|-----------|----------|---------------|--------------------------------------------------------------------------------------|
| useVector | boolean   | Yes      | -             | Returns an vector3 type if set to `true`, and normally a table with x, y and z pairs |

## xPlayer.getCoords 示例

```lua
local coords = xPlayer.getCoords(true)
local distance = #(coords - vector3(610.0, 120.2, 60.3))

print(distance)
```
