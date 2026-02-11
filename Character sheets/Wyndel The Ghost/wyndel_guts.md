---
STR: 12
Dexterity: 10
SavDEX: 0
SavCON: 1
DEX: 14
Prof: 3
SavCHA: 1
SavWIS: 0
SavINT: 0
Acrobatics: 0
Deception: 0
Arcana: 1
Athletics: 1
Survival: 0
Animal: 0
History: 0
Insight: 0
Intimidation: 1
Investigation: 0
Medicine: 0
Nature: 0
Perception: 1
Performance: 0
Persuasion: 0
Religion: 0
Sleight: 0
Stealth: 0
CON: 16
INT: 10
WIS: 13
CHA: 18
DeathF1: 0
DeathS1: 0
---
# THINGS YOU MUST CONFIGURE
## Proficiency
`INPUT[number(class(stat)):Prof]`

## str
`INPUT[number(class(stat)):STR]`

## str mod
+`VIEW[floor(({STR} - 10)/2)]` 

## dex 
`INPUT[number(class(stat)):DEX]` 

## dex mod
+`VIEW[floor(({DEX} - 10)/2)]` 

## con
`INPUT[number(class(stat)):CON]` 

## con mod
+`VIEW[floor(({CON} - 10)/2)]` 


## int
`INPUT[number(class(stat)):INT]` 

## int mod
`VIEW[floor(({INT} - 10)/2)]` 

## wis
`INPUT[number(class(stat)):WIS]` 

## wis mod
+`VIEW[floor(({WIS} - 10)/2)]` 

## cha
`INPUT[number(class(stat)):CHA]` 

## cha mod
+`VIEW[floor(({CHA} - 10)/2)]` 

## saving throws
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):SavSTR]` Str: +`VIEW[{SavSTR}<1 ? (floor(({STR} - 10)/2)) : ((floor(({STR} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavDEX]` Dex: +`VIEW[{SavDEX}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavCON]` Con: +`VIEW[{SavCON}<1 ? (floor(({CON} - 10)/2)) : ((floor(({CON} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavINT]` Int: `VIEW[{SavINT}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavWIS]` Wis: +`VIEW[{SavWIS}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(showcase, onValue(1), offValue(0), defaultValue(1)):SavCHA]` Cha: +`VIEW[{SavCHA}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]` 

## skills
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Acrobatics]` Acrobatics +`VIEW[{Acrobatics}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Animal]` Animal Handling +`VIEW[{Animal}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Arcana]` Arcana +`VIEW[{Arcana}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Athletics]` Athletics +`VIEW[{Athletics}<1 ? (floor(({STR} - 10)/2)) : ((floor(({STR} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Deception]` Deception +`VIEW[{Deception}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):History]` History +`VIEW[{History}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Insight]` Insight +`VIEW[{Insight}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Intimidation]` Intimidation +`VIEW[{Intimidation}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Investigation]` Investigation +`VIEW[{Investigation}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Medicine]` Medicine +`VIEW[{Medicine}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Nature]` Nature +`VIEW[{Nature}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Perception]` Perception +`VIEW[{Perception}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Performance]` Performance +`VIEW[{Performance}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Persuasion]` Persuasion +`VIEW[{Persuasion}<1 ? (floor(({CHA} - 10)/2)) : ((floor(({CHA} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Religion]` Religion +`VIEW[{Religion}<1 ? (floor(({INT} - 10)/2)) : ((floor(({INT} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Sleight]` Sleight of Hand +`VIEW[{Sleight}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Stealth]` Stealth +`VIEW[{Stealth}<1 ? (floor(({DEX} - 10)/2)) : ((floor(({DEX} - 10)/2))+{Prof})]`
`INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):Survival]` Survival +`VIEW[{Survival}<1 ? (floor(({WIS} - 10)/2)) : ((floor(({WIS} - 10)/2))+{Prof})]` 

## passive perception
`VIEW[{Perception}<1 ? (floor(({WIS} - 10)/2)+10) : ((floor(({WIS} - 10)/2))+{Prof}+10)]`

## armor class
`VIEW[12+(floor(({DEX} - 10)/2))]` 

## spell atk mod
+`VIEW[floor(({CHA} - 10)/2)+{Prof}]` 

## spell save dc
`VIEW[8+(floor(({CHA} - 10)/2)+{Prof})]` 

## death saves
Suc: `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS1]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS2]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathS3]`
 Fail  :  `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF1]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF2]` `INPUT[toggle(onValue(1), offValue(0), defaultValue(0)):DeathF3]`