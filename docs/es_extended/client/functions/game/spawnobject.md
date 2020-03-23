# ESX.Game.SpawnObject

```lua
ESX.Game.SpawnObject(modelOrHash, coords, cb)
```

该函数生成一个服务器上所有人可见的对象。

!!! warning
      这是一个异步函数，因为它正在等待要流式传输的对象模型，下面有一个有关如何正确利用它的示例。

## 参数

| 参数        |数据类型        | 可选项    | 默认值        | 说明                                                                                                                       |
|-------------|---------------|----------|---------------|----------------------------------------------------------------------------------------------------------------------------|
| modelOrHash | string&number | No       | -             | 您可以指定模型，例如 `prop_cs_cuffs_01`，也可以指定对象哈希值                                                                 |
| coords      | table         | No       | -             | 生成对象的坐标值，你也可以解析向量(`vector`)类型而没有任何问题                                                                 |
| cb          | function      | Yes      | -             | 生成对象时返回的函数。被调用的函数有一个参数，它是对象句柄。                                                                    |

## ESX.Game.SpawnObject 示例

```lua
ESX.Game.SpawnObject('prop_cs_cuffs_01', vector3(120.0, -200.0, 30.0), function(object)
	print(DoesEntityExist(object), 'this code is async!')
end)

print('this code is sync!')
```
