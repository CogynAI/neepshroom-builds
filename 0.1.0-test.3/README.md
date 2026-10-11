# NeepShroom 0.1.0-test.3

Test build for Minecraft 1.20.1 (Fabric), commit f1fe7a4. Download: **neepshroom-0.1.0-test.3.jar** in this folder.

## Required

| Mod | Version | Download |
|---|---|---|
| Fabric Loader | 0.16.14 or newer | https://fabricmc.net/use/installer/ |
| Fabric API | 0.92.12+1.20.1 or newer | https://modrinth.com/mod/fabric-api |
| NEEPMeat | 0.34.0-beta | https://modrinth.com/mod/neepmeat |
| GeckoLib | 4.8.4 or newer | https://modrinth.com/mod/geckolib |

Recommended (recipe viewer, pick one):

| Mod | Version | Download |
|---|---|---|
| EMI | 1.1.24+1.20.1 | https://modrinth.com/mod/emi |
| REI | 12.1.785 (needs Architectury and Cloth Config) | https://modrinth.com/mod/rei |

## What's new

Fixes from tester feedback.

- **Podzol without Silk Touch:** a NEEPMeat PLC turns dirt on a workbench into 4 podzol (COMBINE a Gland Potato, then INJECT blood). Reminder: on plain dirt or grass, mushrooms only stay in the dark (light level 12 or less); on podzol or mycelium they grow in any light. The guide and EMI now say this.
- **Breathing Mask** now sits on the face when worn (goggles, filter, straps), instead of floating above the head.
- **Config follows balance updates:** `config/neepshroom.json5` from an older test build is reset to the current defaults once (the old file is kept as `neepshroom.json5.old`). Before this, older configs kept the pre-balancing numbers. From now on, values you never changed follow new defaults automatically, and your own changes are kept.
- **Flickering models fixed:** surfaces that lay exactly on top of each other flickered on held items (Heart Casing and 36 more) and on the Core Controller and Enlightening Mushroom in the world.

## Installation

1. Install Fabric Loader for Minecraft 1.20.1.
2. Put all jars from the tables and **neepshroom-0.1.0-test.3.jar** into your `mods` folder.
3. Start the game. NEEPMeat's Guide Projector has a **NeepShroom Testing** section with test tools and a checklist.

## Feedback

Send it to whoever gave you the link. Screenshots help; for errors, please include `logs/latest.log`.
