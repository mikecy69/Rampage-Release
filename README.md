# Rampage

Rampage is a creature-centered digital card game featuring a 357-card catalog, five distinctive Biomes, tactical combat, responsive card play, and a simulation-based CPU opponent. The current beta also supports authoritative two-player matches between Windows PCs on the same private local network.

This public repository contains Windows beta installers, release notes, screenshots, and player instructions. It does **not** contain the Rampage source code.

## Install Rampage on Windows

1. Open the repository's **Releases** page
2. Open the newest Rampage release
3. Download the attached Windows installer (`Rampage-Setup.exe` or similarly named `.exe`)
4. Double-click the downloaded installer
5. Follow the installation prompts
6. Leave **Create a desktop shortcut** selected if the installer presents that choice
7. Start Rampage from its desktop icon or its Start Menu entry

The installer is intended to include the Rampage application, its required runtime, card art, audio, maps, and other game assets. Testers should not need to install Node.js, Git, Chrome, or the source project separately. Rampage opens in its own application window rather than an ordinary browser tab.

## Current beta features

- Constructed, Draft, and Randomly-Generated deck formats
- Solo play against Casual, Normal, Challenging, or Expert CPU opponents
- Two-player LAN matches with room codes, authoritative server validation, reconnection, and private player views
- A 357-card catalog across Forest, Mountain, Ocean, Savannah, Swamp, dual-Biome, and Universal card pools
- Stack interaction, priority, seven turn phases, activated and triggered abilities, Items, Enchantments, and persistent creature damage
- Save/load support, resumable Drafts, deck records, a searchable Glossary, card previews, sound, and card-movement animations

Rampage remains a beta. Card balance, CPU decisions, presentation, and edge-case rules interactions are still being playtested and refined.

## Windows SmartScreen notice

Early beta installers may not yet be digitally code-signed. Windows may therefore display a **Windows protected your PC** or **Unknown publisher** warning even when the installer was downloaded from this official repository.

To continue:

1. Verify that you downloaded the installer from this repository's official **Releases** page
2. In the SmartScreen window, click **More info**
3. Click **Run anyway**

Never run an installer received from an unknown person or an unofficial mirror.

## Before playing

Read [Rampage Notes](Rampage%20Notes.md) for controls, action-resolution methods, game modes, Biome flavor descriptions, match options, hand limits, and CPU difficulty information. Card choices from the library, hand, or graveyard use focused legal-choice modals, while casting and battlefield targeting use double-click or click-and-hold meters.

For two-PC room connection instructions and the current human-versus-human beta
status, read the [Rampage LAN Play Guide](LAN%20Play%20Guide.md).

## Beta feedback

Rampage is still being refined. If you encounter a problem or notice card balance issues, please include:

- The Rampage version shown on the release page
- What you were doing immediately before the problem
- The cards and turn phase involved
- A screenshot, if possible
- Whether the problem can be reproduced

## Updates

Installing a newer beta may replace the previous Rampage application. Release notes will identify any special update or saved-game instructions.

## Uninstalling

Use **Settings → Apps → Installed apps → Rampage → Uninstall**, or use the Rampage uninstaller from the Start Menu if one is provided.

Copyright © Rampage project owner. All rights reserved.
