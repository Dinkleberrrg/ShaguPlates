# Changelog OctoWoW – ShaguPlates

> Branch `octowow` = Stand aus Henrys Installation „OctoWoW – HD Upgrade“ (WoW 1.12). Eigene Anpassungen sind im Code mit `-- [patch]` markiert.

**Basis:** shagu/ShaguPlates `9b2ebdf` (2025-06-06)

## Änderungen

### ShaguPlates.lua – keine Fehlermeldung bei deaktiviertem Blizzard_CombatText
Blizzard_CombatText ist bewusst abgeschaltet (sonst doppelte Kampfzahlen neben MikScrollingBattleText). `UIParentLoadAddOn("Blizzard_CombatText")` schrieb dann bei jedem Reload „Couldn't load Blizzard_CombatText: Disabled“ in den Chat. Jetzt wird vorher mit `IsAddOnLoadable` geprüft.

### fonts/Prototype.ttf – neu
Schriftart „Prototype“ hinzugefügt, damit sie UI-weit einheitlich verfügbar ist (auch in MSBT und Bagshui).
