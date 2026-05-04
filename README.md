# Clowder RPG

A Hytale mod that turns the base game into a richer RPG experience. Built around levelling, classes, combat depth and quality-of-life conveniences, with a few experimental systems that aren't yet part of vanilla Hytale.

The mod is designed for servers and works alongside the standard Hytale game flow — most features can be tuned or disabled via configuration.

## Download and installation

The latest build is always on the [Releases page](https://github.com/cathalsan/ClowderRPG-Release/releases). Each release includes a single `.jar` file.

To install:
1. Stop your Hytale server.
2. Drop the `.jar` into the server's `mods/` directory.
3. Start the server. On first run the mod creates a `mods/Clowder_RPG/` folder with all of its configuration files.

To update, replace the `.jar` with the newer one — configuration defaults are regenerated from the JAR on every restart, so there are no leftover stale files to clean up.

## What's inside

A non-exhaustive overview — features are added and refined release by release.

### RPG progression
- Player levels with an XP HUD and stat point allocation.
- Class system with multiple classes, tiers and passive effects.
- Class-specific combat behaviours and crafting interactions.
- Leaderboards and reward tracks.
- Stats GUI with multiple tabs (Profile, Stats, Classes, Vocation, Contract Board, Rewards, Leaderboard, Commands, Settings, About) — available via `/menu`.

### Combat
- Mob HP and damage scaled to player level, with smooth curves rather than sudden jumps.
- Kill XP scaled to the mob's actual difficulty, not just its level.
- Class-based combat passives (marks, last stands, riposte, focused-target buffs, brews, etc.).
- Optional gap-level penalties so under-levelled and over-levelled players feel the difference.
- Anti-grief friendly — combat state is tracked per player for downstream features.

### Teleport
- Personal homes (`/sethome`, `/home`, `/back`).
- World spawn (`/spawn`) and public admin-defined warps (`/warp`, `/warps`).
- Player-to-player requests (`/tpa`, `/tpaccept`, `/tpdeny`, `/tpcancel`).
- Admin teleport tools (`/tp`, `/tphere`, `/setwarp`, `/delwarp`).
- Configurable warmup, cooldown, anti-combat block, anti-movement and post-death lockout.

### Crafting and items
- Several new recipes added on top of the vanilla crafting tables.
- A handful of vanilla items had recipes or behaviour adjusted so they fit the RPG progression.
- Custom shards available on top of the vanilla ones.

### Quality of life
- Light source blocks for decoration.
- Helipack flight system.
- Localised, concise notifications for in-world events.
- Optional database sync for player data persistence beyond the world files.

## Configuration

All configuration lives under `mods/Clowder_RPG/` and is regenerated from the JAR on every startup. To customise values, edit the relevant JSON file in the JAR's source — file edits in the live folder are overwritten on the next restart by design, so updates roll out cleanly.

## Notes

- This repository only hosts public builds and the README. The source code is kept private.
- For a list of changes per version, see the description on each release.
- For questions, suggestions or feedback, reach out via Discord — the link is on my [GitHub profile](https://github.com/cathalsan).
