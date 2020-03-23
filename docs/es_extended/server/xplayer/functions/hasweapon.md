# xPlayer.hasWeapon

```lua
xPlayer.hasWeapon(weaponName)
```

该函数返回如果玩家拥有指定的武器。

## 参数

| 参数       | 数据类型 | 数据类型 | 默认值 | 说明        |
| ---------- | -------- | -------- | ------ | ----------- |
| weaponName | string   | No       | -      | Weapon name |

## xPlayer.hasWeapon 示例

```lua
	if xPlayer.hasWeapon('WEAPON_PISTOL') then
		print('found weapon')
	else
		print('weapon not found!')
	end
```
