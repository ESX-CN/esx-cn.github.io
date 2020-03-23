# ESX.Game.SpawnLocalObject

```lua
ESX.Game.SpawnLocalObject(modelOrHash, coords, cb)
```

该函数产生一个本地对象，仅本地玩家可见，其他人则看不到。

!!! warning
      这是一个异步函数，因为它正在等待要流式传输的对象模型，下面有一个有关如何正确利用它的示例。

## 参数

| 参数        | 数据类型       | 可选项   | 默认值         | 说明                                                                                                                       |
|-------------|---------------|----------|---------------|----------------------------------------------------------------------------------------------------------------------------|
| modelOrHash | string&number | No       | -             | 你可以指定模型，例如“ prop_cs_cuffs_01”，也可以指定对象哈希值                                                                 |
| coords      | table         | No       | -             | 生成对象的坐标。 您也可以解析向量类型而没有任何问题                                                                            |
| cb          | function      | Yes      | -             | 生成对象时返回的函数。 调用的函数有一个参数，即对象句柄。                                                                       |

## ESX.Game.SpawnLocalObject 示例

```lua
ESX.Game.SpawnLocalObject('prop_cs_cuffs_01', vector3(120.0, -200.0, 30.0), function(object)
	print(DoesEntityExist(object), 'this code is async!')
end)

print('this code is sync!')
```
