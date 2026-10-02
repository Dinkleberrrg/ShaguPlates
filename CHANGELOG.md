# Changelog OctoWoW – ShaguPlates

> Branch `octowow` = the state from Dinkleberrrg's "OctoWoW – HD Upgrade" install (WoW 1.12). Own changes are marked with `-- [patch]` in the code.

**Base:** shagu/ShaguPlates `9b2ebdf` (2025-06-06)

## Changes

### ShaguPlates.lua – no error message when Blizzard_CombatText is disabled
Blizzard_CombatText is disabled on purpose (otherwise combat numbers show twice next to MikScrollingBattleText). `UIParentLoadAddOn("Blizzard_CombatText")` then printed "Couldn't load Blizzard_CombatText: Disabled" to chat on every reload. It is now checked with `IsAddOnLoadable` first.

### fonts/Prototype.ttf – new
Added the "Prototype" font so it is available UI-wide (also used in MSBT and Bagshui).
