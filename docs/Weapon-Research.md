# Weapon research

[Weapons and Combat](Weapons-and-Combat) · [AoA implementation backlog](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Upgrade-Backlog)

## Actual downloads and source studies

- [Ars Armorer direct gallery and file study](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Ars-Armorer-Direct-Study): eight weapon display/animation definitions, 36 attachments and selected Lua logic. Effect/delivery/modifier/capacity roles and magical resource presentation.
- [ArsArms and IronsArms source plus released JAR study](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Spell-Adapter-Source-and-Release-Study): 17 released classes, pinned source, charging/impact/workbench patterns and preventive QA requirements.
- [Create Armorer, Immersive Armorer and Helldivers reference inspection](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Mechanism-and-Animation-QA): selected actual reload rigs, independent barrel actions, hand ownership and state-machine behavior. Scoped inspection, not a claim that every asset was tested.
- [Modular armory and effect salvage](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Modular-Armory-and-Effect-Salvage): Fallout-inspired component swaps, detachable effects, resource-preserving adapters and transaction requirements.

## Findings to carry into every weapon project

- [Create Armorer actual-file study](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Create-Armorer-Direct-Study): layered animation/state logic and frame planes. Audit the exact declared LOD paths rather than assuming that a LOD setting points to existing files. Missing declarations are not automatically a reproduced crash.
- [Helldivers actual-file study](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Helldivers-Gunpack-Direct-Study): the selected Quasar logic uses an ammo field for a cooling timestamp. Generic refill/salvage code must respect field meaning and active script routing. This is why adapters need typed state ownership.
- [Versioned AoA native adapters](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Versioned-Weapon-Adapters): current 1.21.1 AoA already exposes per-stack weapon components. Reuse native support where available, keep the 1.20.1 adapter separate, and preserve unknown fields and customized ammo.
- [TaCZ isolated model/animation parser checks](https://github.com/Herbertofury/Advent-of-Ascension/wiki/TaCZ-Isolated-Model-Parser-Check): useful early format checks with explicitly documented harness stand-ins. Passing them does not prove renderer, hands, animation playback or native compatibility.
- [Presentation core and visibility](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Presentation-Core): game-time cosmetic scheduling, duplicate-event control and frame-part visibility. Zero scale is not evidence that geometry submission is skipped, and an exporter label is not proof the native interpolation mode exists.
- [Pinned 1.20.1 ammunition desk](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Ammunition-1.20.1): 172 conventional weapon identities, with seed-tag, daylight and valuable-equipment exceptions. Base ammo identity and actual spending are different questions.

## Mastercraft reference collection

[Owner-selected cross-game playlist index](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Mastercraft-Playlist-Index) groups the BO6/BO7, COD Mobile and other references by study purpose, retaining duplicate positions without inflating unique video counts. Link/title verification is complete for the indexed snapshot; detailed visual sequence review remains separate and is not inferred from thumbnails or comments.

## Apply the findings

Preserve AoA item/resource identity. Keep optional reloads. Validate believable resource pathways, full hand clearance, moving attachments, interruption blends, sound/VFX timing and native multiplayer behavior. A preview or static parser pass does not certify a finished weapon.

## Research still to deepen

The imported catalogue contains many additional frameworks, packs, bridges and historical routes. Their presence is a research lead, not proof of actual-file study. Prioritize owner-selected references, exact matching versions, source hubs, license boundaries and findings that improve the AoA implementation.

## Choose a reference by the problem you are solving

| Design or implementation problem | Start here | Evidence to carry forward |
|---|---|---|
| Magical attachments and visible resource delivery | [Ars Armorer](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Ars-Armorer-Direct-Study) | Separate delivery, modifier and capacity roles; do not turn every magical weapon into a magazine-fed gun |
| Mechanical reloads and independent moving parts | [Create Armorer](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Create-Armorer-Direct-Study) | Real animation/state paths, clear hand ownership, verify declared assets exist |
| Charge, cooling and unusual firing state | [Helldivers gunpack](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Helldivers-Gunpack-Direct-Study) | Preserve the meaning of script fields rather than treating every ammo field as a count |
| Spell integration and crafting bridges | [ArsArms / IronsArms](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Spell-Adapter-Source-and-Release-Study) | Exact released classes, resource accounting and optional dependency behavior |
| Hand or grip clipping | [Pinned TaCZ native hand contract](https://github.com/Herbertofury/Advent-of-Ascension/blob/main/docs/TaCZ-Native-Hand-Contract.md) | Runtime player arms matter; fallback cubes alone cannot certify wide/slim skin hand fit |
| Original identity versus premium redesign | [AoA original-to-concept gallery](https://herbertofury.github.io/Advent-of-Ascension/weapon-concepts.html) | Compare the released sprite, verified behavior and concept before modeling |

### Keep the collection useful

Frameworks, content packs, bridges and compatibility targets remain separate in [Weapons and Combat](Weapons-and-Combat). Favorites belong in [Forever World Collection](Forever-World-Collection); being a favorite does not establish tested compatibility. Record exact versions, source or file pins, inspected features, remaining gaps and the relevant study together. A pack title or showcase is a discovery lead until its actual files are examined.

## Reopen a focused research view

- [TaCZ content packs with actual-file/source studies](https://herbertofury.github.io/Minecraft-Mods/?q=TaCZ&category=Weapons%20and%20Combat&type=content_pack&evidence=study&sort=research): the current view returns Ars Armorer, Create Armorer and Helldivers.
- [Favorite combat entries](https://herbertofury.github.io/Minecraft-Mods/?category=Weapons%20and%20Combat&favorites=1&sort=research): keep favorite ecosystems distinct from tested support.
- [All weapon content-pack research](https://herbertofury.github.io/Minecraft-Mods/?category=Weapons%20and%20Combat&type=content_pack&sort=name): includes imported leads that still need exact-build review.

The catalogue’s **Link to these filters** preserves search, purpose, type, edition, evidence, order, favorites and discovery-route settings. Bookmark it to return to the same research view without rebuilding filters. Individual entry links and comparisons remain available.

## Documented Bedrock roles to evaluate for original designs

Pixelusion's [official Blasters guide](https://wiki.pixelusion.net/en/add-ons/blasters/blasters) describes sustained electrical attacks, healing, three-shot bursts, six-way scatter, charged release, displacement and ammunition-dependent variants. These are documentation-level references, not an actual-file or runtime study of this commercial pack. Other similarly named Blasters packs are separate projects.

For AoA, turn those role distinctions into explicit original design tests:

- **Burst versus scatter:** separate accepted shots, projectiles within a shot and cosmetic emitter selection. Do not multiply resource spending by the number of visual flashes.
- **Sustained effects:** make server timing authoritative, with bounded targets, duration and cleanup. A faster client frame rate must not increase damage or healing.
- **Charge/release:** define cancellation on swap, death, disconnect and interrupted aim. Cancelled attempts must not create a late ghost shot.
- **Movement effects:** define who is pushed, when landing damage applies and how other movement controllers coexist. Test mounts and dimension transitions.
- **Healing and rewards:** specify target eligibility and confirmed outcomes. Visual feedback cannot independently reroll loot or restore resources.
- **Variant identity:** communicate changed role through silhouette, sound and projectile behavior while preserving the original-mode contract. A skin alone is not evidence of a functional conversion.

These are proposed QA/design requirements, not claims of implemented AoA mechanics. Use the [confirmed-shot event audit](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Confirmed-Shot-Presentation) and [complete weapon standard](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Completeness-Standard) when applying them.
