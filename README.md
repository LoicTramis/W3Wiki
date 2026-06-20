This is a Warcraft 3 campaign encyclopedia/reference app.


<!-- ============================================================= -->
#                              SUMMARY                               #
<!-- ============================================================= -->

1. [Game](#GAME)
2. [Campaigns](#CAMPAIGNS)
   1. [Difficulty](#DIFFICULTY)
   2. [Maps](#MAPS)
   3. [Units](#UNITS)
   4. [Items](#ITEMS)
3. [Application](#APPLICATION)


<!-- ============================================================= -->
#                             OVERVIEW                               #
<!-- ============================================================= -->

Warcraft 3 is RTS (Real-Time Strategy) single or multiplayer game.
The Warcraft 3 campaign is one of the single player experience. The player follows 
a story line of several characters through different campaigns.

This app allows you to see some information about the campaign part of the game.
For each `chapter` of each `campaign` of Warcraft 3:Reforged this app will display inforamtions about maps, players , units, buildings, shops, items, quests and so on...
Warcraft 3:Reforged is a re-imagination of Warcraft 3:Reign of Chaos and Warcraft 3:The Frozen Throne released in 2002 and 2003 respectively.


<!-- ============================================================= -->
#                             CAMPAIGNS                              #
<!-- ============================================================= -->

Campaigns are narrative playstyle. Each campaign focus on one story line with typically one or 2 main protagonist.
There are 4 main campaigns for the classic game 'Reign of Chaos' and 3 additional campaigns for the extension of the game 'The Frozen Throne', they also provided 1 prologue campaign and 1 bonus campaign:
- 1 prologue
- 4 classics
- 3 extensions
- 1 bonus

|       [Title]       |       [Game]        |          [Name]          |  [Race]   |   [Image]   |
| ------------------- | ------------------- | ------------------------ | --------- | ----------- |
| Prologue Campaign   | Reign of Chaos      | Exodus of the Horde      | Orc       | ----------- |
| Human Campaign      | Reign of Chaos      | The Scourge of Lordaeron | Human     | ----------- |
| Undead Campaign     | Reign of Chaos      | Path of the Damned       | Undead    | ----------- |
| Orc Campaign        | Reign of Chaos      | The Invasion of Kalimdor | Orc       | ----------- |
| Night Elf Campaign  | Reign of Chaos      | Eternity's End           | Night Elf | ----------- |
| Sentinel Campaign   | Frozen throne       | Terror of the Tides      | Night Elf | ----------- |
| Alliance Campaign   | Frozen throne       | Curse of the Blood Elves | Human     | ----------- |
| Scourge Campaign    | Frozen throne       | Legacy of the Damned     | Undead    | ----------- |
| Bonus Campaign      | Frozen throne       | The Founding of Durotar  | Orc       | ----------- |

Each campaign has multiple chapters, with one mission each called main quest.

<!-- ------------------------------------------------------------- -->
##                             CHAPTERS                             ##
<!-- ------------------------------------------------------------- -->
Campaign has multiple chapters

<!-- ------------------------------------------------------------- -->
##                              MAPS                                ##
<!-- ------------------------------------------------------------- -->
A map is a define space with a unique terrain disposition.
The goal of every map is to complete all main quests.

Each map has:
- **units** (playable, non-playable, recruitable, neutral, allied, ennemy, building...)
- **items** (either directly visible on the map, consumable, droppable, triggered...)
- **doodads**, non-interactable (rock, some buildings, walls, terrain effects like fire)
- **destructable** (trees, crates, some stones...)
- **critters** (sheep, pig, vultur...)

<!-- ------------------------------------------------------------- -->
##                             UNITS                                ##
<!-- ------------------------------------------------------------- -->
Units are parts of race (human, orc, undead, night elf, demons, naga...).
Units on the map are displayed has only one faction.
A faction represents a player and has one specific color.

There are 3 type of units:
- Basic units
- Hero (stronger unit)
- Building 

Source: _worldeditstrings.txt_

<!-- ------------------------------------------------------------- -->
##                            DIFFICULTY                            ##
<!-- ------------------------------------------------------------- -->
There are 3 levels of difficulty:
- **Story mode**: easy mode, where the game knowledge is not required and the errors
made by the player are not punished. Focus more on the story rather than the gameplay. Has less ennemy units than _normal mode_.
- **Normal mode**: a bit more challenging, some basic game knowledge is required,
errors made by the player are not punish. Has a bit more ennemy units than _story mode_.
- **Hard mode**: deeper understanding of the game knowledge is required, errors
made by the player are punished. Has a lot more ennemy units then _normal mode_.

<!-- ------------------------------------------------------------- -->
##                              ITEMS                               ##
<!-- ------------------------------------------------------------- -->
Items can be permanents or consumables.
One item has only one icon, but a icon can be used for multiple items,
specially for custom items.

<!-- ------------------------------------------------------------- -->
##                              QUESTS                              ##
<!-- ------------------------------------------------------------- -->
Each chapter has one or more main quest. Main quests are sequential and they need to be accomplish in one specific order in order move through the story and complete the chapter.
Optional quests can be avoided but will reward the player with additional units or powerful items if they are completed.

<!-- ------------------------------------------------------------- -->
#                            GAME FILES                              #
<!-- ------------------------------------------------------------- -->
There is a lot of files We need 3 categories of files :
- Game files like SLK, JASS, TXT...
- Chapter file (or campaign file) W3M or W3X
- Map files like W3I, W3T, DOO...

Game files data changes only with patch version.  
SLK files are like CSV, JASS files are scripts.
    
Chapter file is the compressed file that contains all data for one specific chapter (or level).  
Map files contain specific data about the chapter like droppable or quest obtanable items, position of units, triggers...  

Every chapter data file is eitther a .w3x (or .w3m for before reforged).
.w3x files are compressed files that contain multiple specific blizzard format files, we'll call them **map files** (because they generally start with war3map.*).
All the data are in 
- JASS (Just Another Scripting Syntax) files contain all the code, global variables, triggers and basic functions.
- Encoded files like .w3i, .w3t, .w3u, and .doo contain encoded data about the campaign chapter.
- Text files contain text data about the campaign chapter such as hero name, quest name, dialog... 

## FILES NEEDED
All those files are needed for the smooth operation of the application.

### To extract from Ladik's CASC Viewer
_They need to be updated for every patch version._  

10 paths for the data files - `.slk`,  
  1. _war3.w3mod > units >_ `abilitydata.slk`,
  2. _war3.w3mod > units >_ `abilitymetadata.slk` ,
  3. _war3.w3mod > units >_ `destructabledata.slk` ,
  4. _war3.w3mod > units >_ `destructablemetadata.slk` ,
  5. _war3.w3mod > units >_ `itemdata.slk` ,
  6. _war3.w3mod > units >_ `unitdata.slk` ,
  7. _war3.w3mod > units >_ `unitmetadata.slk` ,
  8. _war3.w3mod > doodads >_ `doodadmetadata.slk`,
  9. _war3.w3mod > doodads >_ `doodads.slk`,

9 paths for the text files - `.txt`
  1. _war3.w3mod > \_locales > enus.w3mod > units >_ `campaignunitstrings.txt`,
  2. _war3.w3mod > \_locales > enus.w3mod > units >_ `humanunitstrings.txt`,
  3. _war3.w3mod > \_locales > enus.w3mod > units >_ `itemstrings.txt`,
  4. _war3.w3mod > \_locales > enus.w3mod > units >_ `neutralunitstrings.txt`,
  5. _war3.w3mod > \_locales > enus.w3mod > units >_ `nightelfunitstrings.txt`,
  6. _war3.w3mod > \_locales > enus.w3mod > units >_ `orcunitstrings.txt`,
  7. _war3.w3mod > \_locales > enus.w3mod > units >_ `undeadunitstrings.txt`,
  8. _war3.w3mod > \_locales > enus.w3mod > units >_ `unitskin.txt`,
  9. _war3.w3mod > units >_ `itemfunc.txt`,
  10. _war3.w3mod > units >_ `unitskin.txt`,

1 path for the compressed chapter files - `.w3x`
  1. _war3.w3mod:campaign > reforged > roc >_ [filename].w3x  
  _filename_ is a [race][?expension][level].w3x pattern where:
  - [race] is either `human`, `orc`, `nightelf` or `undead`
  - [extension] a single character to specify Frozen Throne chapters, `x` or nothing.
  - [level] is a range from `01` to `08`
  Some examples: `human03.w3x`, `undeadx02.w3x`,...
_Bonus chapters follow a light different pattern, we'll get into it later._

The last needed file are present in the .w3x file.


### To extract from Ladik's MPQ Editor
_They need to be updated for every chapter._  
In the chapter file there are 6 files for regular data and 1 file for custom item data.

Map files (like .w3i, .w3u, .doo...) can be extracted with a MPQ Editor software.
_More infos about file contents in Application >_
  1. `war3campaign.w3u` 
  2. `war3map.j` 
  3. `war3map.w3i` 
  4. `war3map.w3t` (only for custom items)
  5. `war3map.w3u` 
  6. `war3map.wts` 
  7. `war3mapUnits.doo` 


## HOW TO EXTRACT
### CASC VIEWER
_Disclaimer: This works for Ladik's Casc Viewer only._
**To extract `.w3x` file do the following**
After locating the game app folder path in the disk:
- Open Casc Viewer
- Click `Open storage` (local) > Open `campaign` folder > Open `reforged` folder > Open `roc` folder
- Extract `human01.w3x` or any other chapter file in the `operations` tab
- Choose the path, click on `Extract plain name...` (to avoid generating deep tree folder) and click `OK` to extract.
_Now the chapter file is extracted from the game app._

_Casc viewer is also needed to extract SLK and TXT files._
**To extract SLK files do the following:**

## MPQ EDITOR
_Disclaimer: This works for Ladik's MPQ Editor only._
Now that the extracted .w3x is saved.
- Open MPQ Editor
- Open MPQ(s)
- From the path of the saved extracted .w3x file: select `.w3x` file and click `Open`.
Now every map files is displayed in the app.
- Select every file in the ### Campaign files - .War3Map
_Note that the .w3i file may not be present (used for custom items only)_
- Click on `extract`, choose path and click `OK`



Some file are not present in the
All of the files below are used in the application.



Files:
- `itemstring.txt` (or `war3mapW3T.json` for custom items)
  - itemID       (ex: [rre2])       
  - name         (ex: Rune of Greater Resurrection) 
  - tip          (ex: Purchase Rune of Greater Resurrection) 
  - ubertip      (ex: "Brings <APrr,DataA1> of your nearby dead units back to life.") 
  - description  (ex: Resurrects your dead to fight again.) 
- `itemfunc.txt`
  - item ID (ex: [rre2])
  - path    (ex: ReplaceableTextures\CommandButtons\BTNRune.blp)

## ICONS 
File: [_itemfunc.txt_](##)

<!-- ============================================================= -->
<!-- ============================================================= -->
#                       A P P L I C A T I O N                        #
<!-- ============================================================= -->
<!-- ============================================================= -->

## ARCHITECTURE
ETL Pattern: Extract Transform Load
- Extract -> from .w3x to .slk, .ai, .w3i, .txt, .j... using a third-party app
- Transform -> unitdata.slk to unitdata.json, war3map.w3u to war3mapW3U.json... using a js dependancy
- Load -> war3mapUnit.json + war3mapWTS.json + unitdata.json to JS or JSON using proper algorithm
_I want to retrieve and later display informations about one particular type of data_  
Each domain needs 3 types of classes:
- an entity model class to define the data structure
- an parser class to retrieve data from game files
- an collection class to

| Entity models | Data Parsing Logic | Collection Management |
| ------------- | ------------------ | --------------------- |
| Unit.js       | UnitParser.js      | UnitCollection.js     |
| Item.js       | ItemParser.js      | ItemCollection.js     |
| Player.js     | PlayerParser.js    | PlayerCollection.js   |
| Chapter.js    | ChapterParser.js   |                       |

Same thing for ITEMS, PLAYERS, QUESTS...
Entity models defines constructors with 
## PATTERN

### Extract
Files needed for extraction from the compressed `.w3x`:
 -  __war3map.w3i__       ->  Info displayed at the start of a chapter
 -  __war3map.w3t__       ->  Changes made in the object editor
 -  __\*.slk__            ->  All units, spells and items data (HP, mana, damage...)
 -  __war3campaign.w3u__  ->  Changes made to regular race units
 -  __war3mapUnits.doo__  ->  Definitions and positions of all placed units and items
 -  __war3map.w3u__       ->  Changes made to specific and custom units
 -  __\*.txt__            ->  All units, spells and items description
 -  __war3map.wts__       ->  All texts for a chapter (title, dialogs, names...)

- **Infos** - contains all infos about the map (name, loading screen, players, version...),
- **Items** - contains all custom items,
- **JASS** - contains data about items, units, position, scripts, triggers, quests...
- **Triggers** - contains all the text for this chapter (unit, conversations, quests, player...)
- **Units**
- **Units** and 
- **Units**
### Collection classes

### Item files
- Item data class       _Item.js_           -> define all attributes for data file _items.js (or items.json)_
- Item parser class     _ItemParser.js_     -> retrieves data from JSON and JASS files
- Item collection class _ItemCollection.js  ->


## DESIGN PATTERN
### Factory methods
Using a static factory methods allow me to create an instance of object without the need to specify every parameters.
Example:
For the entity **class Item**, without factory method, creating a new instance for a **drop item** will look like this:
```JS
const item = new Item(id, type, undefined, undefined, undefined, undefined, undefined, unit, prob, group, undefined, undefined)
```
with factory method
```JS
const item = Item.createDropItem(id, type, unit, prob, group)
```
which is less error prone.
## FOLDER STRUCTURE


### Main file

## DEPENDANCIES
 W3MapTranslator dependancies.
<!-- ------------------------------------------------------------- -->
##                         SLK CONVERSION                           ##
<!-- ------------------------------------------------------------- -->
### ABILITY: ability.slk -> ability.json
Contains all data about ability like spells, consumable, aura

<!-- ------------------------------------------------------------- -->
##                        .W3* CONVERSION                           ##
<!-- ------------------------------------------------------------- -->
### DOODADS: war3mapUnits.doo --> war3mapUnitsDOO.json
Includes player units, start location, cinematic unit... on the MAP
Relevant attributes for _Unit_ are:
- type
- hero (with lvl, str, agi, int)
- inventory
- abilities
- player
- ID

### INFOS: war3map.w3i --> war3mapW3I.json
Contains all informations about the map:
- Chapter title
- Chapter number
- Description
- Number of players
- Patch version

### CAMPAIGN UNITS: war3campaign.w3u --> war3campaignW3U.json
File listing all changes to unit properties like icon, abilities...
Relevant for custom unit:

### ITEMS: war3map.w3t --> war3mapW3T.json
Contains all change made to item. Doesn't list all items in the map
- id    ->  itemdata.json (as _itemID_)
- id.id ->  unitmetadata.json (as _iabi_) 

### UNITS: war3map.w3u --> war3mapW3U.json
Contains changes about unit

### MAP CAMPAIGN UNITS: war3mapcampaign.w3u --> war3mapcampaignW3U.json
Keeps consistency between RoC and TFT in reforged

### TRIGGER STRINGS: war3map.wts --> war3mapWTS.json
Contains all the strings like item names, unit names, quest names, dialogs...
- number: _string_
<id,field> -> abilitydata.json

<!-- ------------------------------------------------------------- -->
##                           JASS PARSER                            ##
<!-- ------------------------------------------------------------- -->

### UNIT Search:
- ADD: CreateNUnitsAtLoc
- ADD: CreateNUnitsAtLocFacingLocBJ (usually for cinematics)
- REMOVE: RemoveUnit
- REMOVE: ExplodeUnitBJ (used for mid-cutscene)

### ITEM Search:
- ADD: RandomDistAddItem
- ADD: CreateItemLoc
- REMOVE: RemoveItem

### QUESTS
- CreateQuestItemBJ
- QuestMessageBJ

### Alliance settings
- SetPlayerAllianceStateBJ

## https://867380699.github.io/blog/2019/05/09/W3X_Files_Format#introduction

## The custom units file
| Extension   | Object Type   | Object IDs                  | Mod IDs                        | Uses Optional Ints |
| ----------- | ------------- | --------------------------- | ------------------------------ | ------------------ |
| w3u         | Units         | Units\UnitData.slk          | Units\UnitMetaData.slk         | No                 |
| w3t         | Items         | Units\ItemData.slk          | Units\UnitMetaData.slk         | No (useItem = 1)   |
| w3b         | Destructables | Units\DestructableData.slk  | Units\DestructableMetaData.slk | No                 |
| w3d         | Doodads       | Doodads\Doodads.slk         | Doodads\DoodadMetaData.slk     | Yes                |
| w3a         | Abilities     | Units\AbilityData.slk       | Units\AbilityMetaData.slk      | Yes                |
| w3h         | Buffs         | Units\AbilityBuffData.slk   | Units\AbilityBuffMetaData.slk  | No                 |
| w3q         | Upgrades      | Units\UpgradeData.slk       | Units\UpgradeMetaData.slk      | Yes                |

<!-- ------------------------------------------------------------- -->
##                           TEXT PARSER                            ##
<!-- ------------------------------------------------------------- -->
For item:
- itemfunc.txt --> Icon path (what it looks like in the inventory)
- itemskin.txt --> Skin path (what it looks like on the map)
- itemstrings.txt --> Name, Tip, UberTip, Description

For custom item:


<!-- ------------------------------------------------------------- -->
##                            CONFIG.JS                             ##
<!-- ------------------------------------------------------------- -->
_-> to avoid remplacing every path string by grouping all path in one file_
<!-- ============================================================= -->
<!--                                                               -->
#                      C O D E   E X A M P L E                       #
<!--                                                               -->
<!-- ============================================================= -->
# CODE
<!-- /// NO TODO TURN CODE SAMPLE INTO IMAGES -->
Code sample that I found somewhat interesting.

Parsing through JASS files (Script language created by Blizzard with no public document 'obviously'), trying to find the logic behind the code knowing that it was generated by Warcraft 3's World Editor software that was made by a rocket science engineer about 23 years ago was a challenge.

## RegEx

/^(?!endfunction)\s*function\s+\S*CreateUnitsForPlayer\S*\b/i
--> ensure that the string doesn't have endfunction
--> ensure that the string contains function and CreateUnitsForPlayer

## Data type
- Object -> grouping data into one single entity
- Array -> convenient data storage
- Set -> to eliminate duplicate data

## Binding
Binding the PlayerParser function getPlayerIDByUdgName() on the UnitParser class so I can use it in findUnitsToAdd() function
```JS
/* --------------- index.js --------------- */
const playerParser = new PlayerParser()
const unitParser = new UnitParser(playerParser.getPlayerIDByUdgName.bind(playerParser))
/* --------- ParserPlayer.js CLASS -------- */
getPlayerIDByUdgName(udg_name) {
  return this.players.find(player => player.udg_name === udg_name).id
}
/* ---------- UnitParser.js CLASS --------- */
class UnitParser {
  constructor(getPlayerIDByUdgName) {
  // ...
    this.getPlayerIDByUdgName = getPlayerIDByUdgName
  // ...
  }
  #findUnitsToAdd() {
    // ...
    const player = parts[2].includes("Player") ? 
      parseInt(parts[2].at(-2)) : 
      this.getPlayerIDByUdgName(parts[2].trim().slice(4))
    // ...
  }
}
```

## Parsing logic function

SLK files are a CSV structured-like file, but there is no library to convert them. So I came with
a function to do it.
Except there are a few problems with these files.

For example:
- in unitdata.slk, header indicates 32 columns (;X32;) but there is actually 31 columnss
```SLK
ID;PWXL;N;E
B;X32;Y865;D0
C;X1;Y1;K"unitID"
C;X2;K"sort"
...
C;X31;K"version"
C;X1;Y2;K"Hamg"
C;X2;K"a1"
```
- in itemdata.slk, header indicates 30 columns (;X30;) and there is effectively 31 data columns
```SLK
ID;PWXL;N;E
B;X30;Y284;D0
C;X1;Y1;K"itemID"
C;X2;K"comment"
...
C;X30;K"stackMax"
C;X1;Y2;K"ckng"
C;X2;K"Crown of Kings +5"
```
- but some rows don't have every column (;X9; missing)
```SLK
C;X6;K0
C;X7;K0
C;X8;K"AIfe"
C;X10;K0
C;X11;K"-"
```
A lot of slk files have X columns in header but X-1 field for each row. Naturally, as I test for every files
I've come to an programming issue.
In version 1, I counted the number of rows to determine which column it is. Which led to error for some SLK files.
In version 2, instead of counting, I checked for new columns, which worked for any SLK files.
```JS
const SLKtoJSON_Version_1 = () => {
// ... LOOP THROUGH EVERY LINE OF THE FILES... //
/* Ignore first line                    */ if (index === 0) continue
/* Get n columns (;Xn;) & m rows (;Ym;) */ if (index === 1) getCols, getRows, continue
/* From 0 to n -> field name            */ if ((index - 2) <= cols) field[objectIndex] = field     
/* Otherwise -> field value             */ else values[objectIndex] = value

/* ! PROBLEM HERE: Either one or the other but not both! */
/* After field row && X === n - 1 */
/* After field row && X === n */
if ((index > cols * 2) && parseInt(line.split(";")[1].slice(1)) === cols - 1) dataObject[keys[col]] = values[col]
}

const SLKtoJSON_Version_2 = () => {
// ... LOOP THROUGH EVERY LINE OF THE FILES... //
/* Skip line 1 & 2       */ if (!line.includes("C;")) continue
/* Y1 -> field name      */ if (line.includes(";Y1;")) isFieldName = true
/* Yx & !Y1 -> new line  */ if (line.includes(";Y") && !line.includes(";Y1;")) object[fields[vIndex]] = values[vIndex]  
/* Y1 & X -> field name  */ if (isFieldName && line.includes(";X")) fields[fIndex] = fieldName
/* Yx & X -> field value */ if (!isFieldName && line.includes(";X")) values[vIndex] = value
}
```
## One big array
Read multiple text files and concatenate them into one big array.
Units can be of any race and unit names split into multiple files
```js
const [humanNames, orcNames, undeadNames, nightelfNames, neutralNames] = [
  fs.readFileSync('./extracted/text/humanunitstrings.txt', 'utf-8').split("\n"), // human
  fs.readFileSync('./extracted/text/orcunitstrings.txt', 'utf-8').split("\n"), // orc
  fs.readFileSync('./extracted/text/undeadunitstrings.txt', 'utf-8').split("\n"), // undead
  fs.readFileSync('./extracted/text/nightelfunitstrings.txt', 'utf-8').split("\n"), // night elf
  fs.readFileSync('./extracted/text/neutralunitstrings.txt', 'utf-8').split("\n"), // neutral
]
const allLines = humanNames.concat(orcNames, undeadNames, nightelfNames, neutralNames)
```  
Function: `#retrieveUnitName`  
File: `UnitParser.js`

## DESIGN PATTERN: Factory Methods
_*Builder pattern* is better for much more complex object._
_*Factory classes* need predefined information that I don't have_.

Used in `addUnits` and `updateUnits` from: `UnitParser.js`
I need to create a Unit with multiple parameters combination
So I avoid doing `undefined` parameter for added and updated unit
Potentially, I can more factory method if needed.
```JS
const addedUnit = { type, player, status }
const newUnit = new Unit(
        newID,
        addedUnit.type,
        undefined,
        undefined,
        undefined,
        undefined,
        undefined,
        addedUnit.player,
        undefined,
        undefined,
        undefined,
        undefined,
        addedUnit.status)

const updatedUnit = { type, player, udg_name, status }
const newUnit = new Unit(
        newID,
        addedUnit.type,
        undefined,
        undefined,
        undefined,
        undefined,
        addedUnit.udg_name,
        addedUnit.player,
        undefined,
        undefined,
        undefined,
        undefined,
        addedUnit.status)
```

## STRING MANIPULATION
I want to extract a specific substring from a specific string using another substring.
Example: I want to extract "05_HumanX" from "05_HumanX04secret" using "HumanX04secret"
I used 
``` JS
const result = "05_HumanX04secret".slice(0, "HumanX04secret".indexOf("0") + 3)
```
I get the index of the first "0" to _cut_ (or _slice_) the string at the "0" index, but since it has 3 more characters at the beginning
I add 3 to slice at the correct index and to end up with the substring I want.

<!-- INCORPORATE THIS SOMEWHERE
JASS scripts (war3map.j) - for unit definitions, triggers, etc.
W3I files - map info and player data
WTS files - string tables for text
W3U/W3T/W3A files - unit/item/ability data
MPQ archives - to extract images and models
Object data - custom units, items, abilities
 -->
