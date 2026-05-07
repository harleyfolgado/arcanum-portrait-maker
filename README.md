# Arcanum Portrait Maker

Arcanum Portrait Maker is a Windows desktop utility for installing custom portraits and a curated Starter Character Pack for Arcanum: Of Steamworks and Magick Obscura.

Validated public release: `v1.0.0` on GitHub Release tag `v1.0.0-starter-pack`.

The Starter Character Pack replaces the 12 stock pregenerated Pick Character characters with new starter characters. It is separate from the Create Character portrait tool. Installing the Starter Character Pack does not add the 12 starter portraits to `userport.mes`.

I have not seen a polished full stock pregen replacement pack for Arcanum before, so this project attempts to provide one. All characters come with a bio/story and some even a unique starting item. Perhaps you will help figure out the curse of Sir Rogers? 

## Screenshots

![Create Portrait workflow](screenshots/1-create-portrait.png)
![Starter Character Pack screen](screenshots/2-starter-character-pack.png)
![Manage Installed Portraits screen](screenshots/3-manage-installed-portraits.png)
![In-game character sheet](screenshots/4-in-game-character-sheet.png)

The full 12-character portrait set is included in [screenshots/](screenshots/).

## Download

Download the app from the GitHub Release asset, not the green `Code` button. The repository ZIP only contains public project files and documentation.

Release page:
`https://github.com/HarleyFolgado/arcanum-portrait-maker/releases/tag/v1.0.0-starter-pack`

Release asset:
`ArcanumPortraitMaker-v1.0.0-win32-x64.zip`

Validated SHA256:
`5B2EAD1756679BC14CE6DDC43F69560A7246CA47AFDF528E89051466DEB91984`

1. Open the GitHub Release page for tag `v1.0.0-starter-pack`.
2. Download `ArcanumPortraitMaker-v1.0.0-win32-x64.zip`.
3. Extract the ZIP to a normal folder.
4. Run `ArcanumPortraitMaker.exe`.
5. Choose your Arcanum install folder inside the app.

Arcanum must be installed separately. This repository and its releases do not include the game itself.

## What It Does

- Installs a 12-character replacement roster for Single Player -> New Game -> Pick Character.
- Keeps Create Character custom portrait installation separate.
- Creates a timestamped restore point before replacing Starter Character Pack files.
- Restores stock characters from the app-created restore point.
- Detects old Create Character starter portrait entries without removing them automatically.

## Validated v1.0.0 Status

- 12 validated starter characters ship in the Starter Character Pack.
- Install and uninstall support are included through the app preview, install, backup, and restore flow.
- Clean GOG/base install testing is the supported `v1.0.0` baseline.
- No Starter Character Pack leakage into Create Character was confirmed in validation.
- Starting gear was confirmed working for the validated roster.
- Optional UAP extra content is not part of `v1.0.0` support.

## Requirements

- Windows.
- A legally installed copy of Arcanum.
- A writable copy of the Arcanum install folder. A throwaway copy is recommended for first-time testing.

This project does not include Arcanum, an Arcanum executable, DAT archives, official game assets, WorldEd, Factory tools, or patch archives.

## Install Starter Character Pack

1. Download `ArcanumPortraitMaker-v1.0.0-win32-x64.zip` from the GitHub Release tag `v1.0.0-starter-pack`.
2. Extract the app folder.
3. Run `ArcanumPortraitMaker.exe`.
4. Open `Starter Character Pack`.
5. Choose your Arcanum install folder.
6. Preview the install.
7. Click `Install Starter Character Pack`.
8. Open Arcanum manually and go to Single Player -> New Game -> Pick Character.

## Restore Stock Characters

1. Open `Manage Installed Portraits`.
2. Choose the same Arcanum install folder.
3. Scan.
4. Use `Restore Stock Characters`.

Restore uses backups created by this app. It does not reconstruct stock files from DAT archives.

## Create Character Portraits

The Create Custom Portrait workflow still writes custom portraits through `data/portrait/userport.mes`. This is separate from the Starter Character Pack.

Manage Installed Portraits treats these as different systems:

- Create Character custom portraits use `userport.mes`.
- Starter Character Pack status uses the starter-pack manifest and installed replacement files.

## Compatibility Notes

- Tested against a clean GOG/base Arcanum install workflow.
- Other mods that replace the same pregenerated character files or the same `.mes` records may conflict.
- Optional UAP Race Mod / extra content support is not part of `v1.0.0`.
- Always test on a copied install before using a long-term play install.
