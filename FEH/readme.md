# FEH Static Mod
## What's new
- Added map template
- Most xored values now can be edited directly
- Added FEH_Common.bt.h to store shared functions and structs (please put the .bt files and .h in the same folder)

## File paths
- Skills: Common/SRPG/Skills/
- Heros:Common/SRPG/Persona/
- Decriptions: LANG/Message/Data/
- Maps: Common/SRPGMAP

## Tools
- A modified FEAT (can be found in my repository)
- 010 editor

## Process
- Use FEAT to extract a .bin file from .bin.lz
- Open the .bin file with 010 editor
  - Delete the first 4 bytes
  - Run a corresponded template
  - Mod!
  - Insert the deleted 4 bytes back. (If you forgot, just copy it from the .bin.lz file, they are the same)
- Use FEAT to compress the modded .bin file back into .bin.lz
- Overwrite the original file.

## Some Explanations
- The first 4 bytes of a .bin.lz file are only relevant for decrypt/encrypt and have nothing to do with the file content.
- Most of the values in .bin are xor encrypted, their xor key can be seen in the template file
- Skill timing/ability/limit ids: https://feheroes.gamepedia.com/User:HertzDevil/Skill_effect_tags
