# Pavlov_KillConfirmed_Gamemode by Golden


## Installation
1. Drag and drop the **Content** folder inside your Unreal Engine 4 project. 
Then open your project, and move the **KILLCONFIRMED** folder inside your UGC. Do not move the Gameplay folder!
2. Remove any Pavlov Gamelogic in your level. Then put the GL_KillConfirmed gamelogic in your level.
3. Link the definition to it.
4. Place the BP_KC_PlayerProxy in your level.
5 .If you want to add BOTS to your game, place the BP_AutoBotsSpawner inside your level. Edit the variable "Needed Bots" to change the bots count. ***Note**: You can manage bots ingame, but if you don't want players to use it, place it under the map or somewhere hidden.
6. Click on the GL_KillConfirmed blueprints, and edit the defaults variables as you want (Weapons, skins, match length etc)
7. If you have a Custom Item Table or a custom Skin table, replace them inside the CMP_KC_GlobalInfo
8. Set the gamemode to CUSTOM in your server to enable the KillConfirmed Gamemode.
**Note**: You can play all vanilla gamemode even with this custom gamelogic. But you can't have two custom gamelogics in your level!

## Settings


In the GL_KillConfirmed gamelogic, you will find multiples variables:
* **No Team** = Free for all, no team. Change the win score by adjusting the DMWin Score variable.
* If **No Team** is unticked, it will be a team deathmatch, change the win score by adjusting the TDMWin Score variable.
* **Round Duration** is the max match length in seconds.
* By default, the first spawn will give you a random loot, with all weapons available in Pavlov, including the WWII stuff. You can edit it.

## Features


* DogTag spawn when a player is killed. The color is adjusted by the dead player's team. If it's a deathmatch, it's color will be green.
* Dogtags are visible through walls.
* Teams are balanced at runtime!
