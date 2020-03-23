# xPlayer.addWeaponComponent

```lua
xPlayer.addWeaponComponent(weaponName, weaponComponent)
```

This function adds a weapon component to a weapon, if the player has it, the available component list can be found in the weapon configuration file.

## 参数

| 参数        | 数据类型 | 数据类型 | 默认值 | 说明      |
|-----------------|-----------|----------|---------------|------------------|
| weaponName      | string    | No       | -             | Weapon name      |
| weaponComponent | string    | No       | -             | Weapon component |

## xPlayer.addWeaponComponent 示例

```lua
xPlayer.addWeapon('WEAPON_ASSAULTRIFLE', 50)
xPlayer.addWeaponComponent('WEAPON_ASSAULTRIFLE', 'clip_drum')
xPlayer.addWeaponComponent('WEAPON_ASSAULTRIFLE', 'flashlight')
```