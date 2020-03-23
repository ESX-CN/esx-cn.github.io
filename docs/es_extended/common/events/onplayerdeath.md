# esx:onPlayerDeath

```lua
AddEventHandler('esx:onPlayerDeath', function(data)

end)
```

#### `data` Table Information

| child          | 类型    | 说明                                                                                        |
|----------------|---------|----------------------------------------------------------------------------------------------------|
| victimCoords   | table   |                                                                                                    |
| killerCoords   | table   |                                                                                                    |
| deathCause     | string  | 返回杀死受害者的武器/模型/对象的哈希值。                                                               |
| killedByPlayer | boolean | 玩家被其他玩家杀死了吗?下面的数据只有在玩家被杀死时才会生成。                                            |
| distance       | number  | 死者与杀手之间的距离(GTA游戏内单位)                                                                   |
| killerServerId | number  | 杀手的服务器id                                                                                       |
| killerClientId | number  | 杀手的客户端id                                                                                       |

#### 服务端调用示例

一个简单的击杀通知

```lua
RegisterServerEvent('esx:onPlayerDeath')
AddEventHandler('esx:onPlayerDeath', function(data)
	data.victim = source

	if data.killedByPlayer then
		TriggerClientEvent('esx:showNotification', -1, GetPlayerName(data.victim) .. 'was killed by ' .. GetPlayerName(data.killerServerId) .. ' from ' .. data.distance .. ' units')
	else
		TriggerClientEvent('esx:showNotification', -1, GetPlayerName(data.victim) .. ' died')
	end
end)
```

#### 客户端调用示例

这是一个检查玩家(客户端)是否死亡的完美例子，这对很多事情都很有用，例如只允许菜单在活着的时候打开。

```lua
local IsDead = false

AddEventHandler('esx:onPlayerDeath', function(data)
	IsDead = true
end)

AddEventHandler('playerSpawned', function(spawn)
	IsDead = false
end)
```
