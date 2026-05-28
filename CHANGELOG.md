# Changelog

All notable changes to the Fair Surrender Mod will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-05-28

### Added
- Core surrender and bribery system for friendly fire incidents
- PDA network integration for faction alerts and communication
- Dialog system for NPC interaction (`dialogs_surrender.xml`)
- Sample stalker dialogs in English (`dialogs_stalkers.xml`)
- Forced timed quest system for payment alternatives
- Reputation penalty system (double loss on refusal/failure)
- 3-second faction delay before automatic hostility
- Dynamic faction management based on player actions
- Exhaustive dialog method fallback system for engine compatibility
- Debug tips for dialog troubleshooting via PDA notifications

### Changed
- Script uses multiple dialog call signatures for XRAY engine compatibility

### Notes
- Tested with S.T.A.L.K.E.R. G.A.M.M.A
- Requires `xrs_surrender_handler.script` to be loaded at game startup
- Dialog opening method requires engine support; fallback notifications included
