---
type: guide
status: active
audience: gm
canon: current
parent: "[[Vault Guide]]"
---
# Atlas VTT Guide

The Mirrored Realms is set up to be played inside Obsidian with **[Atlas VTT](https://github.com/ByteMirror/atlas-vtt)** by Fabian Urbanek (ByteMirror), a community plugin that turns the vault into a virtual tabletop: battle maps, grids, tokens, fog of war, dice, initiative, and a separate player window for a second screen.

Atlas VTT is optional. Every note in the vault can be read and run without it.

## Requirements

- Obsidian **1.8.7** or newer, on **desktop**. Atlas VTT does not run on mobile.
- The **Atlas VTT** community plugin, installed and enabled.
- *Optional:* the **Fantasy Statblocks** plugin, which Atlas uses to link creature notes to tokens.

## The `atlas-vtt` Folder

Atlas VTT keeps all of its data in a folder named `atlas-vtt` at the root of the vault.

> [!warning] Do not move or rename this folder
> The plugin expects the folder at exactly `atlas-vtt/` in the vault root. Its location is built into the plugin and cannot be configured, and saved scenes store paths that begin with `atlas-vtt/`. Moving or renaming the folder breaks existing maps and makes the plugin create a fresh, empty one.

| Path | Contents |
| --- | --- |
| `atlas-vtt/collections/` | one folder per collection, with its scenes, maps, encounters, tokens, characters, players, notes, and stat blocks |
| `atlas-vtt/assets/` | images imported into Atlas, such as maps and token art, plus generated thumbnails |
| `atlas-vtt/.atlas-data/` | hidden plugin data: settings, collection metadata, and asset tags |

Scenes are saved as `.atlasmap` files inside their collection.

## Conventions for This Project

- **One collection per release.** Name each collection after the release it serves, using its ID and title—for example, `SA-01 The Pact in the Twilight`. Shared material, such as generic Shardkin tokens, can live in a collection named `Mirrored Realms`.
- **Pin notes instead of copying them.** Atlas can pin a Markdown note, or another map, to a location on a scene. Pin the existing location, NPC, and creature notes from the library rather than writing new text inside Atlas.
- **Keep the player view clean.** The player window is meant for a second screen. Check its settings before play so that note previews, token hit points, and other GM information stay hidden. Many library entries contain collapsed GM callouts; pinned notes should not be shown to players without checking them first.
- **Use the fifth-edition conditions.** Collections can carry a list of conditions; use the SRD 5.2.1 conditions so they match the stat blocks.
- **Record artwork.** Map and token images imported into Atlas are copied into `atlas-vtt/assets/`. Record original project artwork in the [[Asset Register]] like any other image.

## Linking Creatures to Tokens

Atlas links tokens to creature notes through the optional Fantasy Statblocks plugin. It recognizes a creature note when:

- the note's properties contain `statblock: true`, together with the creature's statistics in the Fantasy Statblocks format, or
- the note contains a `statblock` code block.

A token image can be set with an `image` or `token-image` property.

> [!note] Planned
> The creature notes in the [[Mirrorgate Bestiary]] currently use readable Markdown stat blocks, which Atlas cannot read. Adding Fantasy Statblocks properties to them, while keeping the readable stat blocks for the library and the books, is planned.

## Atlas VTT and the Repository

The plugin itself is included in the vault's shared settings. The `atlas-vtt/` data folder is **not** published to the repository yet:

- it contains personal settings and test scenes;
- the starter tokens supplied by the plugin are third-party artwork, not project material, and are not covered by the project license.

When a release receives official maps, its collection will be published deliberately, along with the artwork it needs.

---

Related: [[Vault Guide]], [[Style Guide]], [[Game Master's Codex]], [[Mirrorgate Bestiary]]
