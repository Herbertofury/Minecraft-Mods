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

The original 17 views and all 159 master observations are preserved in the repository. Seventy-nine master observations are attached to catalogue identities: 37 exact matches to existing records and forty-two newly reviewed identities. The remaining 80 master observations and 168 unmatched companion-view rows remain in review. 183 companion rows are attached to 70 entries; they do not inflate the unique-project or source-record totals.

[Preserved source views](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-source-views.json) · [Master import receipt](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-import.json) · [Companion receipt](https://github.com/Herbertofury/Minecraft-Mods/blob/main/docs/resource-pack-atlas-companion-receipt.json)

Original scores and superlatives remain source opinions. No pack was installed, no source was deleted, and no native compatibility flag was promoted by this consolidation.

## Apotheosis and farming: choose a visual direction

[Pinnacle](https://www.curseforge.com/minecraft/texture-packs/pinnacle) refreshes Apotheosis alone. A 1.20.1 backport exists, while the author’s stated ongoing focus is 1.21.1+. [Excalibur Apotheosis](https://www.curseforge.com/minecraft/texture-packs/excalibur-apotheosis-support) is an alternative medieval treatment for its blocks, items and GUI. Both can target the same resources: choose the intended winner and inspect overlap rather than assuming they combine automatically.

[Excalibur Farmer’s Delight](https://www.curseforge.com/minecraft/texture-packs/excalibur-farmers-delight-support) provides food/block textures; author-reported completion does not cover every third-party Delight addon. Both Excalibur support authors instruct placing their addon above base Excalibur. These are visual integrations, not substitutes for gameplay compatibility tests.

## Connected textures are a renderer feature

[Connected Paths](https://www.curseforge.com/minecraft/texture-packs/connected-paths) requires OptiFine or Continuity according to its author. A pack-format edit alone does not implement connected rendering, and planned support for an ecosystem is not shipped support. The similarly named dynamic-generation mod is a separate project.

[Stay True](https://www.curseforge.com/minecraft/texture-packs/stay-true) has feature-specific renderer requirements and leaf/pack-order guidance. Its base pack is distinct from Stay True Compats Reforged. Verify the actual loader and renderer stack before promising identical leaves or connected surfaces.

[Ars Naturae](https://www.curseforge.com/minecraft/texture-packs/ars-naturae) offers a wood/moss/blue-Source visual direction for Ars Nouveau. The inspected page lists 1.20.1; broad addon support and other releases still need checking. Decide precedence when combining it with other Ars visual packs.

## Excalibur animation-stack cautions

[Clarent](https://www.curseforge.com/minecraft/texture-packs/clarent-excalibur-patch) and [the Fresh Animations Patch](https://modrinth.com/resourcepack/excalibur-fresh-animations) currently name different Excalibur base versions in their instructions. Pin the exact intended combination before testing; do not merge two differing recipes for the stack into an assumed guarantee. The animation patch also lists renderer/animation conflicts and requires its supporting resources and entity-animation tools.

[Supplementaries support](https://www.curseforge.com/minecraft/texture-packs/excalibur-supplementaries-support) still lists presents and flags as missing. [Hearth and Harvest support](https://www.curseforge.com/minecraft/texture-packs/excalibur-hearth-and-harvest-support) has separate Forge and NeoForge file lanes and focuses on crop/block visuals. Both are visual support packs, not replacements for native gameplay testing.

## Food and coaster packs: resolve overlapping assets

[BnC Coaster Compat](https://modrinth.com/resourcepack/bnc-coaster-compat) is the project behind the old opaque atlas link. It supplies selected food-display models and overrides some existing assets. [Excalibur support for Brewin’ and Chewin’](https://modrinth.com/resourcepack/brewin-and-chewin-excalibur-support) also changes coaster visuals. Check exact overlapping model/texture paths and test priority order instead of assuming both can win. Neither is the same project as similarly named Modded Coasters or More Coaster Compat.

[My Nether’s Delight support](https://www.curseforge.com/minecraft/texture-packs/excalibur-my-nethers-delight-support) targets My Nether’s Delight rather than the older Nether’s Delight. [Pixel Perfection’s Farmer’s Delight pack](https://modrinth.com/resourcepack/pixelperfectionxfarmersdelight) describes standalone use in its prose but lists a base Pixel Perfection pack as required; keep this discrepancy visible until the intended exact stack is tested. Its Rustic Delight support is labelled beta.

## Classic packs and naming fixes are distinct tools

[Faithful 32x Modded](https://www.curseforge.com/minecraft/texture-packs/faithful-32x-modded) targets older Minecraft and the Programmer Art style; its main file is for 1.12.2. Do not present it as a native 1.20.1 download. [Create BDCraft](https://www.curseforge.com/minecraft/texture-packs/create-bdcraft) separates Create generations and texture resolutions, so choose the actual game/Create pair before comparing appearance or memory cost.

[The Rename Compat Project](https://modrinth.com/resourcepack/the-rename-compat-project) changes display names rather than merging item identities or recipes. Its language scope and supported-but-not-included list matter. [Fresh Mowzie’s Mobs textures](https://modrinth.com/resourcepack/fresh-mowzies-mobs-textures) lists selected mob retextures; the word Fresh does not establish new animations or complete mob coverage.

## Material effects and partial coverage

[SPBR-Farmer’s Delight](https://modrinth.com/resourcepack/spbr-farmersdelight) provides LabPBR material maps. Its linked [SPBR setup guidance](https://modrinth.com/resourcepack/spbr) requires a shader with LabPBR/parallax support and those settings enabled. These author instructions are not a benchmark or Hari/Vulkan qualification. Test the precise shader, renderer and mod versions before recommending the stack.

[Iron’s Spells ’n Spellbooks Reimagined](https://www.curseforge.com/minecraft/texture-packs/irons-spells-n-spellbooks-reimagined) changes models and selected GUI icons; use the correct Forge 1.20.1 or NeoForge 1.21.1 release. [Bare Bones x The Aether](https://modrinth.com/resourcepack/bare-bones-x-the-aether) lists several Aether add-ons, but Aether Redux and Deep Aether remain planned. [Better Leaves - Hexerei](https://www.curseforge.com/minecraft/texture-packs/better-leaves-hexerei) covers three Hexerei leaf types and does not require Motschen’s Better Leaves.

## Selective crops and biome foliage

[Crops 3D Reploughed](https://www.curseforge.com/minecraft/texture-packs/crops-3d-reploughed) separates crops, flowers and saplings, making selective stacking possible. Its author directs all-in-one users to [Crops 3D Reforged](https://www.curseforge.com/minecraft/texture-packs/crops-3d-reforged). Choose the exact game-version file and inspect overlapping model paths before combining packs; the names do not mean duplicate identities or automatically compatible layers.

[Biomes You’ll Go 3D Flora](https://www.curseforge.com/minecraft/texture-packs/biomes-youll-go-3d-flora) targets vines and mushrooms, not every plant. Confirm the actual BYG/BWG registry names for each file. [Excalibur | Quark Delight Support](https://modrinth.com/resourcepack/quark-delight-excalibur-support) is for that add-on; Quark and Farmer’s Delight have separate support packs.
