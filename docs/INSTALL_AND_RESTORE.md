# Install And Restore

## Public v1.2.0 Payload

Payload folder:

`release-payloads/restored-female-small-race-pregen-pack-v1.2.0/`

Primary target:

- default GOG install / bundled-UAP baseline

This payload adds:

- `Stella` as female gnome
- `Loretta` as female halfling
- `Dagna Stonebrow` as female dwarf
- final release scale `85` for all three

It does **not** add:

- trader or vendor integration
- Create Character support
- EXE patching
- separate Race Mod dependency
- optional UAP extra content dependency

## Install

1. Back up any loose overrides already present in the target Arcanum install.
2. Open:
   - `release-payloads/restored-female-small-race-pregen-pack-v1.2.0/`
3. Copy the included `data` folder into the Arcanum install root.
4. Start a new game.
5. Open `Single Player -> New Game -> Pick Character`.
6. Choose `Stella`, `Loretta`, or `Dagna Stonebrow`.

## Verified Starter Loadouts

- `Dagna Stonebrow`
  - `8099 Small Leather Armour`
- `Stella`
  - `8137 Small Ladies' Smoking Dress`
- `Loretta`
  - `8140 Small Ladyservant's Dress`

## Included Verified Clothing Names

- `8134 -> Small Ladies' City Dweller Clothes`
- `8137 -> Small Ladies' Smoking Dress`
- `8140 -> Small Ladyservant's Dress`
- `8143 -> Small Ladies' Rustic Finery`

## Rollback

1. Restore the files you backed up before copying the payload.
2. Remove the loose override files copied by this payload if you want to disable the restored female small-race pregens.

## Known Limitations

- `8135 Small Ladies City Dweller Clothes` remains excluded because it is blocked and wrong-size
- trader or vendor distribution is deferred
- Steam or pure-vanilla compatibility is not claimed
- `baseUAPextras` / optional UAP extra content adapter support is deferred
