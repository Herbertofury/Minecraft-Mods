# Visual styles and resource-pack stacks

[Browse visual packs](https://herbertofury.github.io/Minecraft-Mods/?category=Visuals%20and%20Resource%20Packs) · [All visual entries](Visuals-and-Resource-Packs) · [Verification guide](Research-and-Verification)

Choose a coherent visual direction first, then add narrowly scoped fixes for the mods that look out of place. A pack's presence in this library means it is worth researching; it does not certify every combination or version.

## Choose a direction

| Direction | Starting point | What to preserve |
|---|---|---|
| Trailer-like simplicity | Bare Bones with mod-specific support | Consistent flat shapes and color grouping rather than mixing unrelated high-detail styles |
| Medieval world | Excalibur and version-matched support packs | Matching material language across Create machinery, magic and buildings |
| Cozy interfaces | Farmer GUI | Readable screens and the exact version-specific supported-mod list |
| Richer foliage | One chosen leaf system, with matching plant/crop layers | Texture-pack adaptation, render cost and overlapping leaf models |
| Magic / enchanted items | Ars Loafers and Bibliophilia where appropriate | Target-mod versions, CIT dependencies and readable item distinctions |

## Author guidance that changes the install plan

### Bare Bones: check priority rather than copying an old stack

The recovered research suggested mod-specific packs above Bare Bones x Mods. The current [Bare Bones x Mods author page](https://modrinth.com/resourcepack/bare-bones-x-mods) instead says to place that pack at the top. Treat this as a conflict to resolve for the exact chosen overlay, rather than claiming that either order works universally. Its published example puts its integrated compatibility layer above the corresponding resource packs and Bare Bones base.

Start with the author's matching-version example, add one overlay at a time, and inspect the affected items/blocks. Record any intentional override. A successful reload is not proof that all textures are taking priority as intended.

### Excalibur + Create: the support pack sits above the base

[Excalibur Create Support](https://www.curseforge.com/minecraft/texture-packs/excalibur-create-support) explicitly places its support pack above Excalibur. Its release list distinguishes Forge 1.20.1 and NeoForge 1.21.1 archives and names the Create generation. Match all three: Minecraft, loader and Create version. Do not treat the latest project file as a universal archive.

### Better Leaves: version 9 changes how texture adaptation works

[Motschen's Better Leaves](https://modrinth.com/resourcepack/better-leaves) says version 9 uses pre-created textures and custom texture packs may need compilation. Version 8.1 and earlier adapted textures dynamically at a stated performance cost. That is a version-dependent tradeoff, not a measured FPS result for this pack. Choose one leaf system and test overlapping models before adding several foliage packs.

### Bibliophilia: a dependency and a reported conflict

[Bibliophilia](https://modrinth.com/resourcepack/bibliophilia) requires CIT Resewn or Forge CIT for 1.18–1.21.1. Its page marks 1.21.2–1.21.4 unsupported and 1.21.5 as vanilla-capable. It also reports incompatibility with Dynamic Trims. The 1.20.1 lane must therefore include an appropriate CIT solution; a newer vanilla-capable version does not remove that older dependency.

### Farmer GUI and Ars Loafers: support is version-scoped

[Farmer GUI](https://modrinth.com/resourcepack/farmergui) separates its supported-mod lists by Minecraft range. Preserve that distinction when checking a large modpack. [Ars Loafers](https://www.curseforge.com/minecraft/texture-packs/ars-loafers) currently describes its 1.21.1 behavior while older files cover 1.20.1. Its Create/Farmer's Delight-inspired styling is visual design, not proof of functional cross-mod integration.

## More stack ideas retained from the research

These are historical starting ideas awaiting full exact-file review, not certified load orders:

- **Vanilla-like large pack:** a broad base plus its compatibility layer, then narrowly selected plant/crop treatments.
- **Flowers and farms:** dedicated Botania/Ars/plant treatments, a chosen crop-model layer and a consistent base. Avoid several packs owning the same crop model by accident.
- **Animated modded creatures:** investigate F.M.R.P, Fresh Animations and the needed extensions together. Verify the relevant model/texture feature dependencies and exact supported entities before adoption.
- **Medieval ecosystem expansion:** investigate Excalibur-specific magic, farming and creature overlays individually. A similarly named addon is not automatically compatible with every Excalibur or mod version.

## Repeatable visual check

1. Record the exact Minecraft version, loader, target-mod versions, renderer/shader and each resource-pack file.
2. Keep a known-good base arrangement, then add one layer at a time.
3. Inspect the actual affected blocks, items, GUI screens and entities in bright and dark scenes. Include inventory icons, held items and animated states.
4. Test resource reload, missing textures/models, transparency, emissive surfaces, connected textures and alternate entity variants where applicable.
5. Compare frame times and memory in the same scene and settings. No FPS gain or no-loss claim is made from screenshots or author descriptions alone.
6. Save the chosen priority order and exact file versions, including intentional overrides and known unsupported cells.

## Import coverage

The original 17 views and all 159 master observations are preserved in the repository. Fifty-three master observations are attached to catalogue identities: 37 exact matches to existing records and sixteen newly reviewed identities. The remaining 106 master observations and 240 unmatched companion-view rows remain in review. Ninety-one companion rows are attached to 36 existing entries; they do not inflate the unique-project or source-record totals.

[Preserved source views](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-source-views.json) · [Master import receipt](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-import.json) · [Companion receipt](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-companion-receipt.json)

Original scores and superlatives remain source opinions. No pack was installed, no source was deleted, and no native compatibility flag was promoted by this consolidation.
