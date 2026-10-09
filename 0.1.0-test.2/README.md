# NeepShroom 0.1.0-test.2

Test build for Minecraft 1.20.1 (Fabric), commit e49a9f8. Download: **neepshroom-0.1.0-test.2.jar** in this folder.

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

First balancing pass. NeepShroom now sits in NEEPMeat's late midgame to late game, and it no longer hands out NEEPMeat resources early or cheap.

**Things that work differently now**
- **Mycelium Substrate:** feed the mushroom on dirt with **Gland Potatoes** instead of raw meat.
- **Substrate Feeder:** needs **Eldritch Enzymes** as well as Mycelium Growth to spread. A supplied field also costs a little Growth every minute. Feeders placed in older worlds stop spreading until you fill in Eldritch Enzymes.
- **Incubator (Tier 1):** now has a crafting recipe (Machine Block, Mixer, Motor Unit, Meat Steel, Substrate), so you need Internal Components first. If its motor stops in the middle of a batch, the batch spoils and drops 1–2 Mycelial Residue. That is how you get your first Residue.
- **Mycelial Residue:** now comes only from the **Decomposer** (and from spoiled or failed batches). The trommel and the Enlightening Mushroom no longer make it.
- **Decomposer:** is now a recycler. It takes plants, seeds, mob drops, NEEPMeat by-products and NeepShroom leftovers. It gives a little Tissue Slurry and, by chance, Residue. It no longer turns bricks or brains into Meat.
- **Whisper Broth:** made from Whisper Flour instead of Whisper Wheat Seeds.
- **Enlightened Mushroom:** costs 1024 data (like NEEPMeat's own enlightenments).
- **Enlightening Mushroom:** at most 3× as fast as before (was 6×). NEEPMeat's recipes cost 1.5× to 2× the data there.
- **New recipes:** Heart Casing, Incubator Heart, Great Heart Casing, Feeder, Decomposer, Great Heart, Mycelium Seed, Side Node, Station and Mycelial Implant need later NEEPMeat items: Internal Components, Bioelectric Organs, Rough Brains, Open Eye, Reanimated Heart, Divine Organ, Control Unit. EMI or REI show all of them.
- **Brains:** the network uses much less Brain Supply (about 20 Enlightened Brains per hour for a full core instead of about 86). The 8-component limit is gone: every bucket of Brain Supply stored in Side Nodes or Brain Storage adds a component slot.

**New**
- **Brain Storage:** Tier 3 breeding target that holds 16 buckets of Brain Supply for the network.

**Fixes**
- The Incubator Heart could not be made in survival: its old recipe needed NEEPMeat's Animal Heart, which cannot be obtained.
- Config values are range-checked. A 0 for an interval no longer crashes the server.
- NeepShroom now requires NEEPMeat 0.34.x and refuses to start with a different version.

## Installation

1. Install Fabric Loader for Minecraft 1.20.1.
2. Put all jars from the tables and **neepshroom-0.1.0-test.2.jar** into your `mods` folder.
3. Start the game. NEEPMeat's Guide Projector has a **NeepShroom Testing** section with test tools and a checklist.

## Feedback

Send it to whoever gave you the link. Screenshots help; for errors, please include `logs/latest.log`.
