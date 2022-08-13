# [NMRiH/Any?] Tickbase Manipulation Fix

[AlliedModders thread](https://forums.alliedmods.net/showthread.php?t=339058)

Fixes an exploit where players can manipulate game time to perform actions instantly (using progress triggers, detonating grenades, firing, etc.)

## Installation
- Upgrade to Sourcemod 1.11 or higher, else install [DHooks2](https://github.com/peace-maker/DHooks2/releases) 
- Download the latest zip in [releases](https://github.com/dysphie/sm-tickbase-manipulation-fix/releases)
- Extract contents into `addons/sourcemod`
- Refresh your plugin list (`sm plugins refresh` in server console)

## CVars

Cvars should be modified in `cfg/plugin.tickbase-manipulation-fix.cfg`

- `sm_tickbase_shift_max_seconds` (Default: 2)
  - How far ahead from server time a client is allowed to be (don't touch unless you know what you're doing)
  
- `sm_tickbase_shift_log_seconds` (Default: 25)
  - Logs the name and steamID of clients that are ahead of server time by more than this many seconds. 
    
    **Important note: A detection does not mean a client is cheating**. However, repeated offenses in a short period most certainly do 
  
## Game Support
- This fix should be game-agnostic but I can't maintain gamedata for all of them. If you want support for your game please [submit a pull request](https://github.com/dysphie/sm-tickbase-manipulation-fix/pulls) with valid gamedata or [open an issue](https://github.com/dysphie/sm-tickbase-manipulation-fix/issues).

  Currently tested games:
  - No More Room in Hell

## Special thanks
  - [backwards](https://forums.alliedmods.net/member.php?u=246029) for help with coding and testing
