---
type: guide
status: active
audience: shared
canon: current
parent: "[[Welcome]]"
---
# Vault Guide

The vault is organized for Obsidian. Folders describe broad layers of the project; links, properties, and hub notes describe how the ideas relate.

## How to Navigate

- Begin at [[Welcome]], then follow whichever subject interests you.
- Hub notes—also called maps of content—collect the most useful entry points for an area.
- Use local graph view on a hub or release page to inspect its immediate context.
- Use backlinks to find where a character, place, faction, or concept is used elsewhere.
- Prefer following internal links over browsing folders as if they were a book index.

## Vault Layers

| Folder | Purpose |
| --- | --- |
| `00 Project` | navigation, roadmap, conventions, and templates |
| `01 Setting` | world lore, geography, history, cultures, and religion |
| `02 People & Powers` | factions, lineages, and NPCs |
| `03 Game Material` | creatures and other rules-facing resources |
| `04 Adventures` | one-shots, multishots, and campaigns |
| `05 Player Guide` | spoiler-light player entry points |
| `06 GM Reference` | GM-facing navigation and preparation |
| `z_Assets` | images and their provenance register |
| `99 Archive` | preserved superseded material, excluded from the active graph |

Visual files and their provenance are tracked in the [[Asset Register]].

## Core Properties

| Property | Meaning |
| --- | --- |
| `type` | what kind of note this is, such as `npc`, `location`, `moc`, or `multishot` |
| `status` | its editorial state, such as `announced`, `draft`, `active-draft`, or `foundation` |
| `audience` | `shared` for generally safe material or `gm` for GM-facing material |
| `canon` | whether the note belongs to the current setting |
| `parent` | the main hub connected to this note |
| `id` | a stable release identifier such as `SA-01` |
| `progress` | a whole-number production estimate from 0 to 100 |
| `release` | the adventure in which a note is currently used |
| `campaign` | the campaign framework connected to a setting concept |

Property links are written in quotes, for example `parent: "[[NPCs]]"`, so Obsidian treats them as links without breaking YAML.

## Graph View

Useful graph groups can be created with these searches:

- `path:"00 Project"`
- `path:"01 Setting"`
- `path:"02 People & Powers"`
- `path:"03 Game Material"`
- `path:"04 Adventures"`

The templates, archive, and repository-only documents are excluded in the shared vault settings so that scaffolding and superseded notes do not overwhelm the active graph. Personal graph colors and layout remain user-specific.

## Editing Rules

See the [[Style Guide]] before adding or reorganizing material. For current priorities, use the [[Roadmap]].

---

Return to the [[Welcome|Library of Kagami]].
