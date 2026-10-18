![Official project icon](https://cdn.modrinth.com/data/8aoMKplv/a9171ec026d659ccad5c3dff6fdfc80259d63e09.gif)

# Punchy!

[Favorite library](https://github.com/Herbertofury/Minecraft-Mods/wiki/Favorites) · [Official project](https://modrinth.com/mod/punchy-fpa) · [Exact Forge 1.20.1 release](https://modrinth.com/mod/punchy-fpa/version/vbMU3NlS)

## Why it belongs here

Explicitly marked as a favorite in the user's catalogue. A mod that adds various first person animations and visible hands with held items!

## Verified release lane

- Checked: 2026-10-18 using the official Modrinth project/version API.
- Forge 1.20.1: **2.8f**, published 2026-10-14.
- Release ID: `vbMU3NlS`. Project metadata lists client required and server unsupported.
- This is a version-specific metadata check, not a native modpack test. Other Minecraft/loader branches must be checked separately.
- Declared license: All Rights Reserved. Reference and compatibility study do not grant asset redistribution rights.

## Compatibility and quality checklist

First-person arm ownership, rapid animation interruptions, FOV, handedness, TaCZ and other animation systems.

- [ ] Test the exact build in the actual pack, including startup and low-percentile frame times.
- [ ] Exercise setting changes, world changes and resource reloads.
- [ ] Preserve the known-working configuration and compare before upgrading.
- [ ] Record real conflicts and their exact versions; distinguish reports from reproduced defects.

## Relevant to our weapon animation work

The 2.8f changelog describes improved continuity when actions are interrupted or retriggered, including bow/crossbow, eating and swimming transitions. It also addresses Spatial GUI interaction and arm-offset behavior. Our weapon work should preserve current poses and timeline progress through blends, keep hand/item alignment, and avoid replaying earlier sound cues. These are research lessons; a native AoA/Punchy integration is not yet tested.

The imported catalogue pointed to 2.8c. This profile now links the independently checked 2.8f Forge 1.20.1 release while retaining the old source note in the detailed catalogue history.
