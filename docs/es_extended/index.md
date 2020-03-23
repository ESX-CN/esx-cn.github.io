# 概述

该文档指导说明如何下载和安装 **ESX** 框架。

## 要求

- [mysql-async](https://github.com/brouznouf/fivem-mysql-async)
- [async](https://github.com/ESX-Org/async)

## 下载 & 安装

### 使用 [fvm](https://github.com/qlaffont/fvm-installer) 安装

```
fvm install --save --folder=essential esx-CN/es_extended
fvm install --save --folder=esx esx-CN/esx_menu_default
fvm install --save --folder=esx esx-CN/esx_menu_dialog
fvm install --save --folder=esx esx-CN/esx_menu_list
```

### 使用 Git 安装

```
cd resources
git clone https://github.com/ESX-CN/es_extended [essential]/es_extended
git clone https://github.com/ESX-CN/esx_menu_default [esx]/[ui]/esx_menu_default
git clone https://github.com/ESX-CN/esx_menu_dialog [esx]/[ui]/esx_menu_dialog
git clone https://github.com/ESX-CN/esx_menu_list [esx]/[ui]/esx_menu_list
```

### 手动安装

- 下载 https://github.com/ESX-CN/es_extended/releases/latest
- 解压至 `resource/[essential]` 文件夹
- 下载 https://github.com/ESX-CN/esx_menu_default/releases/latest
- 解压至 `resource/[esx]/[ui]` 文件夹
- 下载 https://github.com/ESX-CN/esx_menu_dialog/releases/latest
- 解压至 `resource/[esx]/[ui]` 文件夹
- 下载 https://github.com/ESX-CN/esx_menu_list/releases/latest
- 解压至 `resource/[esx]/[ui]` 文件夹

### 安装

- 导入 `es_extended.sql` 文件至你的数据库
- 配置 `server.cfg` 文件如下

```
add_principal group.admin group.user
add_ace resource.es_extended command.add_ace allow
add_ace resource.es_extended command.add_principal allow
add_ace resource.es_extended command.remove_principal allow

start mysql-async
start es_extended

start esx_menu_default
start esx_menu_list
start esx_menu_dialog
```
