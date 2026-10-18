# NeepShroom 0.1.0-test.4

Test build for Minecraft 1.20.1 (Fabric), commit d816b39. Download: **neepshroom-0.1.0-test.4.jar** in this folder.

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

Tester feedback and checks before the first release.

**Things that work differently now**
- **Incubator Heart:** needs a real heart now: a NEEPMeat **Reanimated Heart** (vivisect a zombie) instead of the two Bioelectric Organs.
- **Incubator output:** items the incubator makes (Great Incubator Heart, Mycelium Seed, Mycelial Implant) and the Residue of a failed breed no longer drop out of the top. They go into a 9-slot **output** in the heart's terminal; click a stack to take it. An Item Output Port at one of the port places takes them out automatically. While the output is full, a finished item waits in the ceiling.
- **Incubator Cooler:** no longer needs Packed Ice. It takes 8 Snow Blocks (farmable anywhere with a snow golem) or 4 Ice instead.
- **Mycelial Implant:** no longer crafted. It is now a chain: Mycelium Block → **Ball Mill** → 2 Mycelial Fibers; 4 Fibers + 1 Residue + 1 bucket of NEEPMeat **Fat** → **Mycelium Reactor** → Nerve Strand; 2 Nerve Strands + Control Unit + Enlightened Brain → **Tier 3 Incubator** → implant.
- **Higher costs (first step):** machine and breeding recipes need about 1.5× the ingredients. Breeding fluids, growing machines, spreading substrate, growing the network and the brain upkeep cost about 1.25× as much. More processing chains to make this easier will follow in later versions.

**New**
- Server option `NETWORK_TRAVEL_BLOCK_IN_COMBAT` (off by default): players who were just hit by or hit a living thing cannot dive into the network for `NETWORK_TRAVEL_COMBAT_SECONDS`.

**Server and security**
- Spectators can no longer change network settings or rename stations.
- Network terminal updates are sent at most once per tick, and the terminal no longer loads chunks of far-away components. Spamming the implant key is ignored.
- Station names can no longer contain formatting codes.
- The creative "build whole incubator" use of the blueprint needs operator rights.
- **Known limitation:** networks have no owner yet. Anyone with an implant can open and change any network up close and travel through it. Keep that in mind on public servers.

## Installation

1. Install Fabric Loader for Minecraft 1.20.1.
2. Put all jars from the tables and **neepshroom-0.1.0-test.4.jar** into your `mods` folder.
3. Start the game. NEEPMeat's Guide Projector has a **NeepShroom Testing** section with test tools and a checklist.

## Feedback

Send it to whoever gave you the link. Screenshots help; for errors, please include `logs/latest.log`.
