# ESX.Game.GetVehicleProperties

```lua
ESX.Game.GetVehicleProperties(vehicle)
```

这个函数获取的车辆的性能。

## 返回值

| Child             | 数据类型   | 说明                                                                |
|-------------------|-----------|---------------------------------------------------------------------|
| model             | number    | 载具哈希值                                                           |
| plate             | number    | 车牌，最多8个字符                                                    |
| plateIndex        | number    | 车牌风格                                                             |
| bodyHealth        | number    | 车身健康度                                                           |
| engineHealth      | number    | 引擎健康度                                                           |
| fuelLevel         | number    | 燃油油位                                                             |
| dirtLevel         | number    | 肮脏程度                                                             |
| color1            | number    | 车漆主色调                                                           |
| color2            | number    | 车漆副色调                                                           |
| pearlescentColor  | number    | Pearlescent color                                                   |
| wheelColor        | number    | 轮毂颜色                                                             |
| wheels            | number    | 轮毂类型                                                             |
| windowTint        | number    |                                                                     |
| neonEnabled       | table     | Table with hardcoded four childs for left, back, front & back neons |
| neonColor         | table     | Packed table with three childs for r,g,b                            |
| extras            | table     | Pair table with id as index, and state as value                     |
| tyreSmokeColor    | table     | Packed table with three childs for r,g,b                            |
| modSpoilers       | number    |                                                                     |
| modFrontBumper    | number    |                                                                     |
| modRearBumper     | number    |                                                                     |
| modSideSkirt      | number    |                                                                     |
| modExhaust        | number    |                                                                     |
| modFrame          | number    |                                                                     |
| modGrille         | number    |                                                                     |
| modHood           | number    |                                                                     |
| modFender         | number    |                                                                     |
| modRightFender    | number    |                                                                     |
| modRoof           | number    |                                                                     |
| modEngine         | number    |                                                                     |
| modBrakes         | number    |                                                                     |
| modTransmission   | number    |                                                                     |
| modHorns          | number    |                                                                     |
| modSuspension     | number    |                                                                     |
| modArmor          | number    |                                                                     |
| modTurbo          | boolean   |                                                                     |
| modSmokeEnabled   | boolean   |                                                                     |
| modXenon          | boolean   |                                                                     |
| modFrontWheels    | number    |                                                                     |
| modBackWheels     | number    |                                                                     |
| modPlateHolder    | number    |                                                                     |
| modVanityPlate    | number    |                                                                     |
| modTrimA          | number    |                                                                     |
| modOrnaments      | number    |                                                                     |
| modDashboard      | number    |                                                                     |
| modDial           | number    |                                                                     |
| modDoorSpeaker    | number    |                                                                     |
| modSeats          | number    |                                                                     |
| modSteeringWheel  | number    |                                                                     |
| modShifterLeavers | number    |                                                                     |
| modAPlate         | number    |                                                                     |
| modSpeakers       | number    |                                                                     |
| modTrunk          | number    |                                                                     |
| modHydrolic       | number    |                                                                     |
| modEngineBlock    | number    |                                                                     |
| modAirFilter      | number    |                                                                     |
| modStruts         | number    |                                                                     |
| modArchCover      | number    |                                                                     |
| modAerials        | number    |                                                                     |
| modTrimB          | number    |                                                                     |
| modTank           | number    |                                                                     |
| modWindows        | number    |                                                                     |
| modLivery         | number    |                                                                     |
