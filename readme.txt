=======================================================================================================================
IMPORTANT NOTE: Localization support is in active development. Not all the text is currently available for translation, 
but more and more of it will be added in the future. Refer to this instruction again in future versions.
=======================================================================================================================


CREATING A NEW LOCALIZATION PACKAGE
===================================
To create a localization package, you need to do the following:
- Navigate to the game's installation folder
- From there navigate to Data\Localization
- Create a copy of the "template" folder and rename it appropriately (e.g. "deutsche")
- Inside the newly created folder, open info.txt and replace the existing text with the display name of the localization. This name will appear in the selection box in the options screen (e.g. "Deutsche")



FONT
====
Underrail fonts should support all the European languages at least. For other languages you might need to replate the font files. You'll have to figure out how to do that yourself for now, there is no support for this in the engine.



SPECIAL SYMBOLS
===============
Whenever there are special symbols such as these in the text - "{0}", "{1}", "{2}", they are meant to hold the text that's being inserted programatically (e.g. damage numbers and such). Make sure that all of these that appear in the original text, also appear in the translated version or the translation might fail.



DIALOG FILES
============
When translating dialogs do not change the text keyed under "_original" - these are just for reference and for future comparison. The keys that start with "q" denote the "questions" - that is, text that is spoken by NPCs and interfaces, while "a" detones the "answers" - things that the player says.

Keep in mind that there is some stuff in the game that is still hardcoded in English that's being injected in the dialog - we'll get to that eventually.

Also, there is currently no support for cutscene localization.



KNOWLEDGE FILES
===============
These files hold text that is used in various places in the game, but mostly in the UI. Each text segment has its own key that is unique inside that file. You should only translate the text, not the key, of course. In most files you'll just be translating the already existing entries (in place), but in some, you are expected to add your own.

Here is list of knowledge files and what they are used for:

ABILITYNAMES.TXT - Translates the names of all the various abilities in the games (abilities, attacks, psi, etc). You must add the entries here yourself. The key is original name of the ability and the text is the translated name.
AMMODISPLAYINFO.TXT - Names of different ammo types as they appear in the weapon tooltips and elsewhere. You must add the entries here yourself.
BASEABILITIES.TXT - Base ability descriptions. Do not add keys.
CALTROPS.TXT - Caltrop stuff. Do not add keys.
COMBATLOG.TXT - Combat log stuff. Work in progress. Do not add keys.
COMBATSTATTOOLTIPS.TXT - Combat stat window tooltips. Do not add keys.
CONCEPTS.TXT - Couple of minor stuff. Do not add keys.
DEATHSCREEN.TXT - Not used currently.
DEVICES.TXT - Not used currently.
DYNAMICEFFECTS.TXT - Dynamic effects on items. This is work in progress. Will add more keys in the future. Do not add your own keys, it won't help.
ENTITYNAMES.TXT - Used to translate the names of objects and characters. Add your own keys here.
ENUMS.TXT - Translates various enumarations in the game. Do not add keys.
EXPLOSIVES.TXT - TNT usage. Might merge this with something else later.
FEATNAMES.TXT - Feat names. Add your own keys.
FEATS.TXT - Feat descriptions. Do not add/change keys.
GRENADES.TXT - Grenade stuff. Do not add keys.
HITEFFECTS.TXT - Weapon on hit effects. Will add more keys in the future. Do not add your own keys, it won't help.
ITEMBLUEPRINTS.TXT - Blueprint descriptions and names. Do not add keys.
ITEMNAMES.TXT - Item names. Add your own keys.
ITEMS.TXT - Work in progress.
MAPS.TXT - Global map stuff. Do not add keys.
POWERSTATIONS.TXT - Misc. stuff. Will probably merge later.
PSI.TXT - Psi abilities (descriptions). Do not add keys.
QUESTS.TXT - Quests (notes). Do not add keys.
RULES.TXT - Gameplay settings stuff. Do not add keys.
SECURITYSCOPES.TXT - Misc. stuff. Will probably merge later.
SKILLS.TXT - Skill descriptions. Do not add keys.
SPECIALABILITIES.TXT - Special abilities (descriptions). Do not add keys.
SPECIALATTACKS.TXT - Special attacks (descriptions). Do not add keys.
SPECIALIZATION.TXT - Specializations. Do not add keys.
STATICEFFECTS.TXT - Static effects on items. This is work in progress. Will add more keys in the future. Do not add your own keys, it won't help.
STATUSEFFECTS.TXT - Character buffs/debuffs. Do not add keys.
STATUSEFFECTNAMES.TXT - Display names of status effects. Add your own keys here.
THROWINGKNIVES.TXT - Throwing knives. Do not add keys.
TRAPS.TXT - Traps. Do not add keys.
UI.TXT - Most of the generic UI stuff. Inclused short and long phrases. Do not add your own keys.
VEHICLE.TXT - Will probably merge later.
VEHICLESTATTOOLTIPS.TXT - Vehicle tooltips. Do not add keys.
ZONESECURITY.TXT - Zone settings stuff. Do not add keys.
ITEMS\AMMO.TXT - Custom modifiers for different ammo and weapon types. Do not add keys.
ITEMS\ARMORITEMMODIFIER.TXT - Armor Modifiers. Do not add keys.
ITEMS\ARMORS.TXT - Work in progress. 
ITEMS\CONSUMABLES.TXT - Consumable usage text. Do not add keys.
ITEMS\CUSTOM.TXT - Some custom utilities. Do not add keys.
ITEMS\FOOD.TXT - Food usage. Do not add keys.
ITEMS\MODS.TXT - Some description for item mods. Work in progress. Do not add keys.
ITEMS\REPAIRKITS.TXT - Repair kits. Do not add keys.
ITEMS\SHIELDEMITTERS.TXT - Shield emitter stuff. Will probably get merged later. Do not add keys.
ITEMS\UTILITIES.TXT - Various utility usage. Do not add keys.
ITEMS\VEHICLEPARTS.TXT - Some vehicle part general text. Do not add keys.
ITEMS\WEAPONS.TXT - Crafted/generated weapon text. Work in progress. Do not add keys.
ITEMS\WEAPONSUBTYPES.TXT - Custom weapon stuff. Do not add keys.