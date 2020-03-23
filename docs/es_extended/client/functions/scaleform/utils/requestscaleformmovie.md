# ESX.Scaleform.Utils.RequestScaleformMovie

```lua
ESX.Scaleform.Utils.RequestScaleformMovie(movie)
```

该函数请求并返回一个已解析的影片scaleform句柄。

## 参数

| 参数      | 数据类型  | 可选项    | 默认值        | 说明                                                                              |
|----------|-----------|----------|---------------|-----------------------------------------------------------------------------------|
| movie    | string    | No       | -             | 影片名称, [可用scaleforms列表](https://scaleform.devtesting.pizza) |

## ESX.Scaleform.Utils.RequestScaleformMovie 示例

```lua
local scaleform = ESX.ScaleForm.Utils.RequestScaleformMovie('MP_BIG_MESSAGE_FREEMODE')
```
