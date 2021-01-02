# Roll20

[Roll20](https://app.roll20.net/)

How-tos and macros and stuff related to Roll20. Issues I've run into and how to fix them.

## Map

Click the _document_ icon at the top to open a listing of all your maps.
- Click on a map title to edit the title.
- Drag-n-drop the _player_ ribbon to indicate which map players should be viewing when they enter the game.

The _cube_ icon let's you select which layer of the map you're working on.

The _clock_ icon will open the Turn Tracker. This is where initiative rolls show up.
- In Settings, you can sort the initiative rolls in descending order before starting combat.
- Hover over an entry in the Turn Tracker to see that token highlighted on the map.

The _cloud_ icon let's you reveal/hide areas of the map (assuming you have Fog Of War turned on).
- Fog Of War is a Setting on the map.

## Journal

The Journal tab holds player character sheets, npc character template sheets, maps, etc.

If you set the _avatar_ on an npc sheet, it will be used as the token for those characters. To add them to the active map, click on the _name_ (not the _icon_) in the Journal and drag-n-drop it onto the map. Make sure you're on the _Objects&Tokens_ layer of the map.

## Macros

The Collection tab includes custom Macros.

**NPC: roll initiative and add them to the Turn Tracker**  
```
@{selected|token_name} rolled initiative: [[1d20+@selected|npc_dexterity_mod}&{tracker}]]
```
To use: select an npc token on the map, click this macro.

