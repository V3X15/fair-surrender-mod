# Surrender Faction Quest Mod

This mod adds a surrender and faction penalty system to S.T.A.L.K.E.R. G.A.M.M.A.

## What it does
- manages a 3-second delay before the local faction attacks after friendly fire
- allows the player to pay a bribe to stop the alarm
- if the player cannot afford it, a forced timed quest is generated
- doubles reputation loss if the player fails or refuses
- integrates support for a local PDA network to alert the faction

## Created files
- `gamedata/scripts/xrs_surrender_handler.script`
- `gamedata/configs/gameplay/dialogs_surrender.xml`
- `gamedata/configs/gameplay/dialogs_stalkers.xml`
- `gamedata/configs/tasks/tm_surrender.ltx`

## Installation
1. Install via Mod Organizer (recommended): add the ZIP `Fair_Surrender.zip` and enable the mod, or
2. Manually copy the entire `gamedata` folder into the S.T.A.L.K.E.R. G.A.M.M.A. mod directory.
3. Make sure the engine loads `xrs_surrender_handler.script` during game startup.

## Structure
- `scripts/xrs_surrender_handler.script`: game logic and friendly-fire behavior management
- `configs/gameplay/dialogs_surrender.xml`: PDA dialog options for resolution choices
- `configs/tasks/tm_surrender.ltx`: definition of the forced timed quest

## Notes
- The task uses `wpn_medkit_advanced` as the target item.
- Quest duration is set to 1800 seconds (30 real minutes).
- Dialog functions reference `xrs_surrender_handler`.

## Check
If you want, I can also add a `mod_description.xml` file or integrate automatic loading of the new script into the mod init system.