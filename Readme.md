# Adventurer's Guide to Tamriel (2E566)

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

## Race/Subrace Traits

#### Cyrodiil
##### Colovian
- Light Armor Proficiency
- Martial Weapon Proficiency
- Charisma +1
- Constitution +1
- Action: Star of the West
  - When you are reduced to 0HP, but not killed outright. you instead drop to 1HP
  - Bonus Action
  - Once per Long Rest

##### Nibenese
- Performance Proficiency
- Persuasion Proficiency
- Charisma +2

#### Breton
- 1 Cantrip from the Wizard Spell List (to cbe updated once the Spells Module is complete)
- Charisma +1
- Intelligence +1
- Passive: Dragon Skin (Still not sure if this one works)
  - You have advantage on saving throws against Magic

#### Nord
- Constitution +2
- Passive: Northern Hide
  - Cold Resistance
- Action: Battlecry
  - All enemies within 9m(30ft) that can hear you must succeed on a Wisdom saving throw against
your Strength score, or become Stunned for two turns, ending at the start of their second
turn
  - Action

#### Redguard
- Scimitar Proficiency
- Strength +1
- Dexterity +1
- Passive: Strong Immune System
  - Poison Resistance
- Action: Adrenaline Rush
  - You pump yourself up for combat, gaining a number of temporary hit points equal to your
level + your Constitution modifier, and gaining an additional 3m(10 ft) of movement speed
for 3 turns.
  - Action
  
#### Altmer
- Intelligence +2
- Passive: Highborne
  - Disadvantage against Magical attacks (May or may not work)
  - Immunity to Poison
- One cantrip from the Wizard spells list (To be updated upon completing the Spells Module)
- Three level 1 spells from the Wizard spells list (To be updated upon completing the Spells Module)

#### Bosmer
- Dexterity +2
- Shortbow Proficiency
- Longbow Proficiency
- Beast Tongue Passive
  - Speak to animals without casting a spell! (Untested)
- Action: Natural Shapeshifter
  - Transform into a Boar for 5 turns, once per long rest (Status will say you are transformed until you rest. It is lying)

#### Dunmer
- Wisdom +1
- Ashborn Passive
  - Resistance to Fire
##### Dunmer
- Dexterity +1
- Bonus Action: Ancestral Protection
  - Once per long rest, add +3 to your AC for 1 turn

##### Hlaalu
- Charisma +1
Persuasion Proficiency

##### Redoran
- Strength +1
- Martial Weapon Proficiency

##### Telvanni
- Intelligence +1
- One cantrip from the Wizard spells list (To be updated upon completing the Spells Module)

##### Indoril
- Wisdom +1
- One cantrip, chosen between Light, Dancing Lights, Spare the Dying, Mending, and Shillelagh (To be updated upon completing the Spells Module)

##### Dres
- Constitution +1
- Animal Handling Proficiency

#### Orsimer
- Action: Berserker Rage
  - 5 turns
  - Gain temporary HP equal to Constitution Modifier + Level
  - Gain advantage on all melee attacks
  - Lose 3AC
  - Unable to cast spells
##### Iron Orsimer
- Strength +2
- Survival Proficiency

##### Wood Orsimer
- Dexterity +2
- Nature Proficiency

## Known Issues
- Nord Northern Hide has no Progression Description
- Nord Battlecry Action doesn't list that it may only be used once per long rest
- Redguard Strong Immune System has no Preogression Description
- Redguard Adrenaline Rush Action has no icon
- Bosmer Natural Shapeshifter claims to last until a long rest, but correctly ends after 5 turns
- Dunmer Ashborn has no Progression Description
- Orsimer Berserker Rage has no icon

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