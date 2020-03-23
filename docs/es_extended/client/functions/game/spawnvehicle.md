# ESX.Game.SpawnVehicle

```lua
ESX.Game.SpawnVehicle(modelOrHash, coords, heading, cb)
```

该函数生成一个服务器上所有玩家都可以看到的载具。

!!! warning
      这是一个异步函数，因为需要等待车辆模型流式传输，下面有一个有关如何正确利用它的示例。

## 参数

| 参数        | 数据类型       | 可选项   | 默认值         | 说明                                                                                                                        |
|-------------|---------------|----------|---------------|-----------------------------------------------------------------------------------------------------------------------------|
| modelOrHash | string&number | No       | -             | 您可以指定模型（例如 `blista`）或载具哈希值。                                                                                  |
| coords      | table         | No       | -             | 载具生成的坐标值，你也可以解析向量类型而没有任何问题                                                                            |
| heading     | number        | No       | -             | 在生成载具的前进方向，必须包含一个小数位                                                                                       |
| cb          | function      | Yes      | -             | 生成载具后返回的函数。调用的函数有一个参数，即载具句柄                                                                          |

## ESX.Game.SpawnVehicle 示例

```lua
ESX.Game.SpawnVehicle('blista', vector3(120.0, -200.0, 30.0), 100.0, function(vehicle)
	print(DoesEntityExist(vehicle), 'this code is async!')
end)

print('this code is sync!')
```
