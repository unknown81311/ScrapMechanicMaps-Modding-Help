---
sidebar_position: 4
title: Script Loading and Execution Order
hide_title: true
sidebar-label: 'Script Loading and Execution Order'
---

### Script Loading and Execution Order

This is an incomplete list of the loading and execution order of scripts and the respective objects for a Custom Game mode.

```
Load Character.lua
Load Unit.lua
Load Tool.lua
Load Game.lua
Call Game:server_onCreate()
Load World.lua
Call Game:client_onCreate()
Load Player.lua
Call Game:server_onPlayerJoined()
Call World:server_onCreate()
Call World:client_onCreate()
Call Player:server_onCreate()
Call Player:client_onCreate()
Call Game:client_onLoadingScreenLifted()
```