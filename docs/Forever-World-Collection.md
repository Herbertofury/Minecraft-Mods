# Forever World Collection

[Home](https://github.com/Herbertofury/Minecraft-Mods/wiki/Minecraft-Mods) · [Favorites](https://github.com/Herbertofury/Minecraft-Mods/wiki/Favorites) · [AoA compatibility implementation backlog](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Compatibility-Targets)

**The long-term compatibility collection for every future mod and modpack we make.** These are the owner's favorite ecosystems to preserve, build with and test together. Requested 2026-10-18. This collection carries forward across projects; it is not just an AoA checklist.

## The foundation

**Butchery · Farmer’s Delight · Born in Chaos · The Aether · Advent of Ascension.** All five are explicitly requested favorites. AoA is both a favorite content mod and the current integration project. The broader roster below carries forward the existing AoA targets as requested.

Favorite membership does not make every entry a mandatory dependency. Optional bridges stay optional, historical/version-gated projects stay visible, and unsupported combinations must be labeled clearly. A target is not a tested-support badge.

## Gameplay, combat, magic and infrastructure

| Favorite ecosystem / integration target | Why keep it in the collection | Acceptance focus |
|---|---|---|
| Advent of Ascension | Core dimensions, creatures, skills and distinctive weapons | Preserve native progression, resource costs, saved item identity and world content |
| L_Ender's Cataclysm | Explicit owner target; boss combat, equipment and progression must coexist with AoA | Native boss mechanics, damage ownership, rewards and progression remain correct |
| Apotheosis | Explicit owner target; affixes, sockets, enchanting and combat progression | No duplicated procs, corrupted equipment or unintended damage multiplication |
| Timeless and Classics Zero (TaCZ) | Explicit owner target; optional premium animated AoA weapon presentation | Original AoA costs/effects and item identity survive; premium presentation and optional reloads work correctly |
| Curios | Already named in the owner's published runtime acceptance checklist | Equip/unequip, death, reconnect and removal remain safe |
| Ars Nouveau | Explicit owner compatibility target; spells, resources and magical progression | Correct spell/resource accounting, ownership, progression and optional dependency handling |
| Iron's Spells 'n Spellbooks + IronsArms | Owner-selected magic-through-firearms research / optional integration candidate | Matching release, spell storage, resource accounting and persistence demonstrated |
| Butchery | Explicit owner target; AoA creature processing and rewards | No lost progression drops or duplicated carcass/reward paths |
| Alex's Mobs | Explicit owner target; creature behavior, combat and progression | Native AI, tame/owner state, drops and AoA rewards remain correct |
| Farmer's Delight | Explicit owner target; AoA ingredients, crops and cooking | Correct ingredients, yields, containers and effects without recipe loops |
| Kaleidoscope Cookery | Explicit owner target; complementary food and cooking integrations | Compatible recipes and food effects without duplication or silent overrides |
| Create | Explicit owner target; mechanical production and expedition logistics | Preserve costs, stack data and progression; no duplication loops |
| Botania | Explicit owner target; magical crafting and optional presentation | Keep Mana and AoA resources distinct; no free-casting loops |
| Applied Energistics 2 | Explicit owner target; storage, crafting and supply preparation | No duplicated withdrawals, lost data or unauthorized remote resupply |
| Gateways to Eternity | Explicit owner target; one themed challenge per accepted dimension | Correct waves, progression gates, rewards, cleanup and performance |
| Scorched Guns | Explicit owner target; appropriate shared ammo and AoA participation | Preserve native weapon behavior and debit resources exactly once |
| Terramity | Explicit owner target; appropriate shared ammo and AoA participation | Preserve native weapon behavior and debit resources exactly once |
| Malum | Explicit owner target; spirit/magic progression and combat | Keep each mod's spirits/resources distinct and avoid duplicated harvest rewards |
| Born in Chaos | Explicit owner target; creature combat, rewards and themed challenges | Preserve special mob mechanics, attribution and progression rewards |
| TaCZ Turrets | Explicit owner target; mount every supported AoA TaCZ weapon | Correct costs, special effects, aiming/ownership, automation policy and safe fallback |

## Dimensions worth keeping connected

These are the existing dimension compatibility targets, carried into Favorites with their original version caveats. The Aether is an explicitly named core favorite. Other rows include historical and discovery lanes; an unavailable release is a documented gap, never an excuse to pretend it is supported.

| Favorite / target | Existing lane | What must remain correct |
|---|---|---|
| The Twilight Forest | Predecessor + priority | Preserve entry conditions and boss progression; distinguish access from progression unlocks |
| The Aether | Priority | Resolve its native entry/exit contract and safe floating-island arrival; check relevant installed addons separately |
| Blue Skies | Predecessor + priority | Separate Everbright and Everdawn destinations and unlocks; preserve the pinned release's entry flow |
| The Bumblezone | Predecessor + priority | Preserve native entry/return behavior and destination context; avoid return loops |
| The Undergarden | Predecessor + priority | Check native activation, destination placement, hazards and return context |
| The Midnight | Priority discovery | Pin a supported release before selecting a rift/travel adapter; do not guess a modern port |
| The Betweenlands | Priority discovery | Pin a supported release and preserve its dimension-specific survival and progression rules |
| Ad Astra | Priority discovery | Treat each planet separately; never silently bypass travel unlocks or life-support requirements |
| Dimensional Doors | Priority discovery | Dynamic pockets require destination identity and ownership checks, not one hard-coded dimension key |
| Eternal Starlight | Priority discovery | Check matching loader/version and native entry/progression contract |
| AbyssalCraft | Historical / version-gated | Preserve separate realm unlocks; no invented target-build support |
| Atum | Predecessor / version-gated | Verify the actual compatible release and native travel rules |
| DivineRPG | Predecessor | One qualified adapter record per dimension; retain progression ordering |
| Eternal Tales | Predecessor | Audit each destination and reward mapping against its exact release |
| Aerial Hell | Predecessor / version-gated | Verify destination, entry and safe-return contracts before enabling |
| [Deeper and Darker](https://www.curseforge.com/minecraft/mc-mods/deeperdarker) | Popular-dimension priority | Preserve the Otherside entry/unlock contract; distinguish release branches and matching loaders |
| [The Lost Cities](https://www.curseforge.com/minecraft/mc-mods/the-lost-cities) | Worldgen / configured-dimension target | Detect the actual world profile; do not invent a separate destination when it modifies the Overworld |
| [RFTools Dimensions](https://www.curseforge.com/minecraft/mc-mods/rftools-dimensions) | Dynamic-dimension target | Preserve dimension identity, ownership and power/availability rules; handle removed or unavailable generated worlds |
| [Tropicraft](https://www.curseforge.com/minecraft/mc-mods/tropicraft) | Established dimension target | Pin the matching release and retain native entry ritual, return and environmental rules |

[Extra Realmstones and dimension adapter plan](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Extra-Realmstones-and-Dimension-Compatibility) records the concrete AoA travel work. More Gateways, ArsArms and IronsArms are supporting addon/bridge lanes, rather than replacements for their parent ecosystems.

## Every new project inherits this checklist

- [ ] Map applicable collection members to the project's exact Minecraft version, loader and feature set.
- [ ] Record each exact release, dependency and archive hash. Keep unavailable lanes explicit.
- [ ] Test each mod alone, the pair, and the supported combined pack, on client and dedicated server where applicable.
- [ ] Preserve existing saves, block/item/entity identity, inventories, ownership, progression and dimension return paths.
- [ ] Test recipes, tags, loot, damage attribution, resources, automation and optional-mod absence. No duplicate rewards or silent overwrites.
- [ ] Check animations, renderers, shaders and graphics-backend interactions without sacrificing features to inflate FPS.
- [ ] Measure cold/warm startup, memory, frame-time lows and server tick time against reproducible baselines. Improve speed in parallel with features; regressions need fixing or explicit explanation.
- [ ] Record compatibility evidence in the relevant project repository and link the result here.

## Per-project evidence record

Use one record per exact configuration: project, Minecraft version, loader, collection member and release/hash, dependencies, config, test scene, result, measured startup/frame/tick times, save-migration result, issue/fix link and verification date. Statuses: **target → files inspected → adapter implemented → native pair tested → combined pack qualified**. A static check cannot skip the runtime gates.

## Keeping a forever world safe

Updates should include migration notes and a reversible test on a copy of the world. Do not remove dimensions or content mods from a living save without a documented recovery plan. Keep the original known-working configuration until the replacement is verified. This page is a collection and compatibility policy, not an automatic installer.
