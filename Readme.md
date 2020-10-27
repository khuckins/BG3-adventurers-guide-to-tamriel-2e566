# Adventurer's Guide to Tamriel (2E566) 0.3.0

## Background
Three years ago, I started creating a setting sourcebook of ~210 pages for d&d 5th edition, set 
in the Elder Scrolls universe. Over the course of a year, I completed it, released it into the 
world, and gained some valuable feedback. With the Early Release of Baldur's Gate 3, I've
decided to return to this setting, and adapt it for play.

This is an early build, and will no doubt be full of bugs. I'm still learning the capabilities
of modding the game pre-mod tools, and I expect that I'll still be finding bugs as the game
is updated and eventually released. This module includes the Human Elven races: Cyrodiils
(Imperials), Breton, Nord, Redguard, Altmer, Bosmer, Dunmer, and Orsimer, including some
subraces.

## Racial Traits/Features
These can be found in the Wiki, under the [Races](https://github.com/khuckins/BG3-adventurers-guide-to-tamriel-2e566/wiki/Races) page.

## Known Issues
- Nord Northern Hide has no Progression Description
- Nord Battlecry Action doesn't list that it may only be used once per long rest
- Redguard Strong Immune System has no Preogression Description
- Redguard Adrenaline Rush Action has no icon
- Bosmer Natural Shapeshifter claims to last until a long rest, but correctly ends after 5 turns
- Dunmer Ashborn has no Progression Description
- Orsimer Berserker Rage has no icon
- A lot of "Not Found" on the Character Creation Menu

## Installation
I recommend using Candor mod manager to install, as the process is highly simplified.
However, you'll want to be sure you're using it to install any other mods you're
using as well.

### Candor
1. Select Baldur's Gate 3 in Candor Mod Manager
2. Select "Add Mods" and choose the .zip file containing this mod
3. Check "AdventurersGuide-RacesModule" and hit "Install Selected Mods"

### Manual
1. Place the included .pak file into \Documents\Larian Studios\Baldur's Gate 3\Mods\
2. Edit \Documents\Larian Studios\Baldur's Gate 3\PlayerProfiles\[Profile Name]\modsettings.lsx:
3. Place this under the ModOrder children node: (This step is technically unnecessary)
```
            <node id="Module">
              <attribute id="UUID" type="FixedString" value="46c59a34-b3b1-40d0-8424-6f59ded3d575"/>
            </node>
```
4. Place this under the Mods Children Node, beneath the Gustav ModuleShortDesc block:
```
            <node id="ModuleShortDesc">
              <attribute id="Folder" type="LSWString" value="AdventurersGuide-RacesModule"/>
              <attribute id="MD5" type="LSString" value=""/>
              <attribute id="Name" type="FixedString" value="AdventurersGuide-RacesModule"/>
              <attribute id="UUID" type="FixedString" value="46c59a34-b3b1-40d0-8424-6f59ded3d575"/>
              <attribute id="Version" type="int32" value="1"/>
            </node>
```

## Other Links
- [GMBinder link](https://www.gmbinder.com/share/-L3u-2oe4GFo8GtXlRHC) to Adventurer's Guide to Tamriel
- [BetterUI](https://github.com/Purlana/BetterUI) makes this mod less of a strain on the Character Creation UI
- [Candor Mod Manager](https://www.nexusmods.com/baldursgate3/mods/22) eases the process of installing mods

## Acknowledgements
- Larion Software, for working on Baldur's Gate 3 and bringing 5th Edition to PC
- Bethesda Softworks, for creating a Sci-fi/Fantasy universe that has eaten over a decade of my life
- The Baldur's Gate 3 Modding Community
- [https://github.com/ShinyHobo](ShinyHobo) for their work easing the process of creating .pak files
