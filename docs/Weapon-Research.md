# Weapon research

[Weapons and Combat](https://github.com/Herbertofury/Minecraft-Mods/wiki/Weapons-and-Combat) · [AoA implementation backlog](https://github.com/Herbertofury/Advent-of-Ascension/wiki/Weapon-Upgrade-Backlog)

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
