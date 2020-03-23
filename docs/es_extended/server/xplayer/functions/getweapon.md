# xPlayer.getWeapon

```lua
xPlayer.getWeapon(weaponName)
```

This functions returns the `loadoutNum` and a weapon object for the weapon if the player has it.

## 参数

| 参数   | 数据类型 | 数据类型 | 默认值 | 说明 |
|------------|-----------|----------|---------------|-------------|
| weaponName | string    | No       | -             | Weapon name |

## xPlayer.getWeapon 示例

```lua
	local loadoutNum, weapon = xPlayer.getWeapon('WEAPON_PISTOL')

	if weapon then
		print(xPlayer.loadout[loadoutNum].label)
	else
		print('weapon not found!')
	end
```
