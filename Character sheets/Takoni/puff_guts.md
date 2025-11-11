---
SavSTR: 1
toggle2: 1
STR: 12
Dexterity: 10
SavDEX: 1
SavCON: 0
DEX: 16
Prof: 2
SavCHA: 0
SavWIS: 0
SavINT: 0
Acrobatics: 1
Deception: 1
Arcana: 0
Athletics: 1
Survival: 0
Animal: 0
History: 1
Insight: 0
Intimidation: 0
Investigation: 1
Medicine: 0
Nature: 0
Perception: 0
Performance: 0
Persuasion: 0
Religion: 0
Sleight: 0
Stealth: 1
select: 11
armor: 0
Hitpoints: 9
DamageTaken: 40
TEMPHitpoints: 60
Inspiration: 0
DeathS3: 0
CON: 12
someProperty: 14
spellcastingclass: 2
INT: 9
WIS: 15
CHA: 12
DeathF1: 0
DeathF2: 0
DeathS1: 0
---
# THINGS YOU MUST CONFIGURE
## Proficiency
`INPUT[number(class(stat)):Prof]`

## str
`INPUT[number(class(stat)):STR]`

## str mod
+`VIEW[floor(({STR} - 10)/2)]` ^M4RLUFoD

## dex 
`INPUT[number(class(stat)):DEX]` ^o5dlMSSM

## dex mod
+`VIEW[floor(({DEX} - 10)/2)]` ^YWvxWXpL

## con
`INPUT[number(class(stat)):CON]` ^oIkRvtuf

## con mod
+`VIEW[floor(({CON} - 10)/2)]` 
^k1CeDMY8

## int
`INPUT[number(class(stat)):INT]` ^k2n0n7jm

## int mod
`VIEW[floor(({INT} - 10)/2)]` ^DjUxivRx

## wis
`INPUT[number(class(stat)):WIS]` ^7yYhKTGN

## wis mod
+`VIEW[floor(({WIS} - 10)/2)]` ^TEAtDnPd

## cha
`INPUT[number(class(stat)):CHA]` ^Ue19j8Oi

## cha mod
+`VIEW[floor(({CHA} - 10)/2)]` ^Ik8QcCc2

## saving throws
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):SavSTR]` Str: +`VIEW[{SavSTR}<1 ? (floor(({STR} - 10)/2)) : ((floor(({STR} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavDEX]` Dex: +`VIEW[{SavDEX}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavCON]` Con: +`VIEW[{SavCON}<1 ? (floor(({CON} - 10)/2)) : ((floor(({CON} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavINT]` Int: `VIEW[{SavINT}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavWIS]` Wis: +`VIEW[{SavWIS}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavCHA]` Cha: +`VIEW[{SavCHA}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]` ^QofL64D7

## skills
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Acrobatics]` Acrobatics +`VIEW[{Acrobatics}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Animal]` Animal Handling +`VIEW[{Animal}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Arcana]` Arcana `VIEW[{Arcana}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Athletics]` Athletics +`VIEW[{Athletics}<1 ? (floor(({STR} - 10)/2)) : ((floor(({STR} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Deception]` Deception +`VIEW[{Deception}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):History]` History +`VIEW[{History}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Insight]` Insight +`VIEW[{Insight}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Intimidation]` Intimidation +`VIEW[{Intimidation}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Investigation]` Investigation +`VIEW[{Investigation}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Medicine]` Medicine +`VIEW[{Medicine}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Nature]` Nature `VIEW[{Nature}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Perception]` Perception +`VIEW[{Perception}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Performance]` Performance +`VIEW[{Performance}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Persuasion]` Persuasion +`VIEW[{Persuasion}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Religion]` Religion `VIEW[{Religion}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Sleight]` Sleight of Hand +`VIEW[{Sleight}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Stealth]` Stealth +`VIEW[{Stealth}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Survival]` Survival +`VIEW[{Survival}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]` ^XhwOOd0p

## passive perception
`VIEW[{Perception}<1 ? (floor(({WIS} - 10)/2)+10) : ((floor(({WIS} - 10)/2))+{Prof}+10)]`

## armor class
`VIEW[10+(floor(({DEX} - 10)/2))+(floor(({WIS} - 10)/2))]` ^ZXCc6bem

## mod with prof
+`VIEW[floor(({DEX} - 10)/2)+{Prof}]` ^Iesb28FO

## spell save dc
`VIEW[10+(floor(({WIS} - 10)/2)+{Prof})]` 

## death saves
Success: `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS1]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS2]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS3]`
Failure:   `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF1]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF2]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF3]`

