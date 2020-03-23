# ESX.Game.Teleport

```lua
ESX.Game.Teleport(entity, coords, cb)
```

该函数传送一个实体。

!!! warning
      这是一个异步函数，因为它等待加载冲突，下面有一个有关如何正确利用它的示例。

## 参数

| 参数     | 数据类型       | 可选项    | 默认值        | 说明                                                                                                                                                                        |
|----------|---------------|----------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| entity   | string        | No       | -             | 要传送的实体                                                                                                                                                                         |
| coords   | table&vector3 | No       | -             | 要传送到的坐标。 同时支持vector3和表格类型。 如果使用表格类型，您还可以指定`heading`来设置传送时的实体方向                                                                                                                           |
| cb       | function      | Yes      | -             | 实体被传送后返回的函数                                                                                                                               |

## ESX.Game.Teleport 示例

```lua
local playerPed = PlayerPedId()

ESX.Game.Teleport(playerPed, {x = 120.0, y = -200.0, z = 30.0, heading = 100.0}, function()
	print('this code is async!')
end)

print('this code is sync!')
```
