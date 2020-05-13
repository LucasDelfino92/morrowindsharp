# CONFLICTS

## INDEX

- [Back to main page](https://github.com/Sigourn/morrowind-improved/blob/master/readme.md)

## CONFLICT REPORT

The following conflicts have been noted down after running the plugins with TES3Merge and TESTool's Leveled Lists. As such, only conflicts not solved by these two mods will be reported.

Bear in mind that not every conflict is a bad thing. In many ocassions, a mod will overwrite Patch for Purist's fixes for different reasons, such as typos when it comes to rewriting an entire dialog topic, or additional changes to quests. As such, only the *actual*, non-intended conflicts, will be listed here.

**Unofficial Morrowind Official Plugins Patch.esp**
- Container
  - de_p_chest_02_aryne: Domina Armor is overwritten by Area Effect Arrows Integrated.esp projectiles.
- Dialog Topic
  - latest rumours: overwritten by Balmora Rumours Fix.esp.

**FMI_Nice_to_Meet_You_1.1.esp**
- Dialog Topic
  - Hello: overwrites Patch for Purists.esm **SNAM - Sound filename** fixes.

**FMI_ServiceRefusal_Contraband.esp**
- Dialog Topic
  - BM_Rumors: overwrites Patch for Purists.esm **NAME - ID** typo fixes.

**LDM - Vampire Talk.esp**
- Dialog Topic
  - MS_VampireCure: overwrites Patch for Purists.esm **NNAM - Next info ID** fixes.
  
**Redaynia Restored.esp**
- Dialog Topic
  - little secret: overwrites Patch for Purists.esm **NNAM - Next info ID** fixes and **NAME - ID** typo fixes.
  - Greeting 9:
    - **NNAM - Next info ID** is overwrriten by Greetings for No Lore.esp
    - Overwrites Patch for Purists.esm **NAME - ID** typo fixes.

**Melchior's Mudcrab Merchant.esp**
- Creature
  - mudcrab_unique: **AI_W - AI Wander** is overwritten by Morrowind Anti-Cheese.esp. Load after Morrowind Anti-Cheese.esp.

**WhiteSuran2_MD_Edition.esp**
- Cell
  - Suran < 6, -7>: overwrites Patch for Purists.esm **DATA - Reference Position Data** fixes.
  - Suran < 6, -6>: overwrites Patch for Purists.esm **DATA - Reference Position Data** fixes.

**Yet Another Guard Diversity - Regular.esp**
- Cell
  - Ald Velothi: overwrites Patch for Purists.esm **Illegal to Sleep here** fix.
  - Molag Mar < 13, -8>: guard deleted by No-Frills Closed Molag Mar.esp.
  - Wolverine Hall < 18, 3>: guard overwritten by Wolverine Hall Overhaul.esp.
  - Vivec, Foreign Quarter Plaza: guard deleted by No-Frills Open Vivec (Vanilla Placement) v1.1.esp.
  - Vivec, Hlaalu Plaza: guard deleted by No-Frills Open Vivec (Vanilla Placement) v1.1.esp.
  - Vivec, Redoran Plaza: guard deleted by No-Frills Open Vivec (Vanilla Placement) v1.1.esp.
  - Vivec, St. Delyn Plaza: guard deleted by No-Frills Open Vivec (Vanilla Placement) v1.1.esp.
  - Vivec, St. Olms Plaza: guard deleted by No-Frills Open Vivec (Vanilla Placement) v1.1.esp.
  
**No-Frills Closed Molag Mar.esp**
- Cell
  - Molag Mar < 13, -8>: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.
  
**No-Frills Open Vivec (Vanilla Placement) v1.1.esp**
- Cell
  - Vivec, Foreign Quarter Plaza: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.
  - Vivec, Hlaalu Plaza: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.
  - Vivec, Redoran Plaza: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.
  - Vivec, St. Delyn Plaza: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.
  - Vivec, St. Olms Plaza: deletes guard replaced by **Yet Another Guard Diversity - Regular.esp**.

**QL_SevenGracesShrines.esp**
- Cell
  - Koal Cave: overwrites Patch for Purists.esm **Illegal to Sleep here** fix.

**Wolverine Hall Overhaul.esp**
- Cell
  - Wolverine Hall < 18, 3>: overwrites guard replaced by **Yet Another Guard Diversity - Regular.esp**.
- Dialog Topic
  - Greeting 7: overwrites Patch for Purists.esm **NAME - ID** typo fixes.

**Descriptive Shrines.esp**
- Script
  - Overwrites Patch for Purists.esm 0 gold fixes to the shrine scripts.
  
**FMI_SaneOrdinators.esp**
- Dialog Topic
  - Greeting 0: overwrites Patch for Purists.esm **NNAM - Next info ID** fixes, **NAME - ID** typo fixes, and **BNAM - Result text (not compiled)** fixes.
