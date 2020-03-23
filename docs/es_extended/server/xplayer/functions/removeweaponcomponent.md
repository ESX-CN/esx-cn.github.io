# xPlayer.removeWeaponComponent

```lua
xPlayer.removeWeaponComponent(weaponName, weaponComponent)
```

This function removes a weapon component from a player, if the player has it. The available component list can be found in the weapon configuration file (`config.weapons.lua`).

## 参数

| 参数        | 数据类型 | 数据类型 | 默认值 | 说明      |
|-----------------|-----------|----------|---------------|------------------|
| weaponName      | string    | No       | -             | Weapon name      |
| weaponComponent | string    | No       | -             | Weapon component |

#### xPlayer.removeWeaponComponent 示例

```lua
local weaponName, weaponComponent = 'WEAPON_PISTOL', 'clip_extended'

if xPlayer.hasWeaponComponent(weaponName, weaponComponent) then
	xPlayer.removeWeaponComponent(weaponName, weaponComponent)
end
```
