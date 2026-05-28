# Fair Surrender Mod

**Version:** 1.0.0  
**Game:** S.T.A.L.K.E.R. G.A.M.M.A  
**Last Updated:** 2026-05-28

Adds a surrender and faction penalty system for friendly fire incidents with PDA network integration.

**Note:** Dialog and bribe options are currently a work in progress (TODO). For now, only pacification and reputation penalty are fully functional.

## Features
- 3-second faction delay before automatic hostility
- Local PDA network faction coordination
- Dynamic NPC behavior management
    - Bribery system to stop faction alerts (**TODO: not yet functional**)
    - Forced timed quest alternative for broke players (**TODO: not yet functional**)
    - Double reputation loss on failure/refusal

## Created Files
- `gamedata/scripts/xrs_surrender_handler.script`
- `gamedata/configs/gameplay/dialogs_surrender.xml`
- `gamedata/configs/tasks/tm_surrender.ltx`

## Installation
1. Install via Mod Organizer (recommended): add the ZIP `Fair_Surrender.zip` and enable the mod, or
2. Manually copy the entire `gamedata` folder into the S.T.A.L.K.E.R. G.A.M.M.A. mod directory.
3. Make sure the engine loads `xrs_surrender_handler.script` during game startup.

## Structure
- `scripts/xrs_surrender_handler.script`: game logic and friendly-fire behavior management
- `configs/gameplay/dialogs_surrender.xml`: PDA dialog options for resolution choices
- `configs/tasks/tm_surrender.ltx`: definition of the forced timed quest
- `configs/gameplay/dialogs_stalkers.xml`: sample stalker dialogues in English

## Notes
- Quest uses `wpn_medkit_advanced` as the target item (30 min duration)
See `CHANGELOG.md` for version history and `VERSION.txt` for current version.

## Support & Issues
For compatibility issues or feature requests, check the debug PDA notifications in-game.

## Repository
The source code and updates for this mod can be found on GitHub:  
[Fair Surrender Mod GitHub Repository](https://github.com/V3X15/fair-surrender-mod)