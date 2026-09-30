---
type: guide
status: active
audience: shared
canon: current
parent: "[[Welcome]]"
---
# Vault Guide

The vault is organized for Obsidian. Folders describe broad layers of the project; links, properties, and hub notes describe how the ideas relate.

## Two Ways to Read

The vault works both as a **library** and as a set of **books**.

- **As a library:** begin at [[Welcome]] and follow whatever interests you. Hub notes collect the entry points for each area, backlinks show where a person, place, or concept is used, and local graph view reveals its immediate context.
- **As books:** open the [[Bookshelf]]. Each book is a table of contents that arranges library entries into a fixed reading order—[[Encyclopedia Kagami]], [[Player's Companion]], [[Game Master's Codex]], and [[Mirrorgate Bestiary]]. Every adventure is also a book: its overview note contains the contents, chapters, and appendices.

Nothing is written twice. Books link to entries instead of copying them.

## Vault Layers

| Folder | Purpose |
| --- | --- |
| `00 Library of Kagami` | the entrance to the library |
| `01 Encyclopedia` | the library itself: cosmology, history, atlas, peoples, faiths, powers, and figures |
| `02 Rules Compendium` | homebrew rules: rules modules, bestiary, and future character options, spells, and relics |
| `03 Adventures` | one-shots, multishots, and campaigns, each laid out as a book |
| `04 Books` | the bookshelf and the table of contents for each book |
| `90 Scriptorium` | the project office: roadmap, conventions, templates, and the asset register |
| `z_Assets` | images |
| `99 Archive` | preserved superseded material, excluded from the active graph |

Visual files and their provenance are tracked in the [[Asset Register]].

## Player and GM Material

Notes marked `audience: shared` are safe for players. Inside them, GM-only material—secrets, adventure hooks, and checks—sits in collapsed callouts marked **GM**, so players can read an entry without opening them. Notes marked `audience: gm` are entirely GM-facing.

## Core Properties

Properties are hidden inside notes by default so that lore and adventure text stays visually clean. They remain available to Obsidian for links, search, filters, and graph relationships. To inspect or edit them, use the **Properties view** in the sidebar or switch the note to **Source mode**.

| Property | Meaning |
| --- | --- |
| `type` | what kind of note this is, such as `npc`, `location`, `moc`, or `multishot` |
| `status` | its editorial state, such as `announced`, `draft`, `active-draft`, or `foundation` |
| `audience` | `shared` for generally safe material or `gm` for GM-facing material |
| `canon` | whether the note belongs to the current setting |
| `parent` | the main hub connected to this note |
| `id` | a stable release identifier such as `SA-01` |
| `progress` | a whole-number production estimate from 0 to 100 |
| `level` | the starting character level of an adventure |
| `located-in` | the place that contains this one, such as a continent, realm, or region |
| `cr` | the challenge rating of a creature |
| `release` | the adventure in which a note is currently used |
| `campaign` | the campaign framework connected to a setting concept |

Property links are written in quotes, for example `parent: "[[NPCs]]"`, so Obsidian treats them as links without breaking YAML.

## Graph View

Useful graph groups can be created with these searches:

- `path:"00 Library of Kagami"`
- `path:"01 Encyclopedia"`
- `path:"02 Rules Compendium"`
- `path:"03 Adventures"`
- `path:"04 Books"`
- `path:"90 Scriptorium"`

The templates, archive, and repository-only documents are excluded in the shared vault settings so that scaffolding and superseded notes do not overwhelm the active graph. Personal graph colors and layout remain user-specific.

## Editing Rules

See the [[Style Guide]] before adding or reorganizing material. For current priorities, use the [[Roadmap]].

---

Return to the [[Welcome|Library of Kagami]].
