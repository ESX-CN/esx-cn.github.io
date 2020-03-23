# ESX.DumpTable

```lua
ESX.DumpTable(table)
```

此函数将给定的表转储到具有树结构的可读字符串中。

## ESX.DumpTable 示例

```lua
local myTable = { {esx = 'awesome'} }
local dumpedTable = ESX.DumpTable(myTable)

print(dumpedTable)

-- print below
{

  [1] = {

    ["esx"] = awesome,

  }

}
```
