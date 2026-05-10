# Arcanum Portrait Maker

Arcanum Portrait Maker is the public-facing release and documentation home for Arcanum portrait and pregen packaging work.

Current public update target: `v1.2.0`



## What v1.2.0 Adds
I have officialy restored all of the small female characters that were cut from the game. I also found some hidden small ladies clothes 
that were under the name "No Good". I have gotten all of these clothes working now but have not implemented them into the trader, that is 
the next version. If anyone can help me redraw Dagnas portrait that would be appreciated. Hope you all enjoy! 
- `Stella` as a female gnome pregen
- `Loretta` as a female halfling pregen
- `Dagna Stonebrow` as a female dwarf pregen
- `Dagna` unique portrait route through `gameport.mes#1098 -> DWF1`
- final release scale `85` for Stella, Loretta, and Dagna
- verified restored small-female clothing names and starter outfits
- confirmed small armor compatibility
- no separate Race Mod required

## Verified Wardrobe

- `8102 Small Robes`
- `8134 Small Ladies' City Dweller Clothes`
- `8137 Small Ladies' Smoking Dress`
- `8140 Small Ladyservant's Dress`
- `8143 Small Ladies' Rustic Finery`

## Confirmed Small Armor

- `8099 Small Leather Armour`
- `8119 Small Studded Leather`
- `8120 Small Guard Chainmail`
- `8121 Small Guard Plate`

## Explicit Exclusions

- trader or vendor integration
- Create Character support
- EXE patching
- Steam or pure-vanilla compatibility claims

## Public Payload

Staged public payload folder:

`release-payloads/restored-female-small-race-pregen-pack-v1.2.0/`

That folder contains only the verified loose overrides for:

- `data/proto/016090 - PC.pro`
- `data/proto/016091 - PC.pro`
- `data/proto/016094 - PC.pro`
- `data/portrait/HUF4.bmp`
- `data/portrait/HUF4_b.bmp`
- `data/portrait/HUF3.bmp`
- `data/portrait/HUF3_b.bmp`
- `data/portrait/DWF1.bmp`
- `data/portrait/DWF1_b.bmp`
- `data/portrait/gameport.mes`
- `data/mes/gameback.mes`
- `data/mes/description.mes`
- `data/Rules/InvenSource.mes`

No EXEs, DATs, vendor routes, internal reports, or unrelated binaries are part of this payload folder.

## Install Target

- default GOG install / bundled-UAP baseline
- no separate Race Mod required
- no optional UAP extra content required

## Install

1. Back up any loose overrides you may already have in the target Arcanum install.
2. Copy the `data` folder from `release-payloads/restored-female-small-race-pregen-pack-v1.2.0/` into the Arcanum install root.
3. Start a new game and use `Single Player -> New Game -> Pick Character`.
4. Choose `Stella`, `Loretta`, or `Dagna Stonebrow`.

## Rollback

1. Restore the loose files you backed up before install.
2. Remove the copied loose overrides if you want to disable the restored female small-race pregens.

## Compatibility Notes

- tested against the default GOG install or bundled-UAP baseline
- other mods that replace the same pregenerated character files or the same `.mes` records may conflict
- trader or vendor integration is intentionally deferred from `v1.2.0`
- Create Character support is not included
- no DAT patching is used
- no `data/Players` payload is used
- no scripts are installed by this payload

## Historical Note

This `v1.2.0` update focuses on the verified **Restored Female Small-Race Pregen Pack** payload for the default GOG install / bundled-UAP baseline. It restores Stella, Loretta, and Dagna Stonebrow as playable female small-race pregens. It is a loose-file payload update, not a Create Character unlock.
