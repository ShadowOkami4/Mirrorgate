---
type: guide
status: active
audience: shared
canon: current
parent: "[[Vault Guide]]"
---
# Style Guide

These rules keep the vault readable in Obsidian, on GitHub, and for future contributors.

## Notes and Links

- Give every active note a unique filename so internal links resolve predictably.
- Link the first meaningful mention of an existing person, place, faction, release, or concept.
- Use a hub note for navigation instead of copying the same lore into several folders.
- Add a linked `parent` property, such as `parent: "[[Welcome]]"`, to connect a note to its principal area.
- Preserve established note names when moving files; Obsidian links depend on the note target, not the folder alone.

## Editorial State

- `concept` — an idea recorded for later development; details may change freely
- `announced` — publicly named, but active writing has not begun
- `draft` — written material that remains incomplete or untested
- `active-draft` — currently being developed
- `foundation` — worldbuilding or structural work for a future release
- `active` — maintained navigation or reference material

## Library and Books

- The vault is read two ways: as a **library** of short, linked entries, and as **books** that arrange those entries in a fixed order.
- Write each piece of content once, as a library entry or adventure chapter. Books are table-of-contents notes in `04 Books` that link to entries; they never copy text.
- Adventures are books of their own: an overview note with a Contents section, chapter notes, and appendices that link to characters, locations, and creatures.
- End each adventure chapter with a navigation line: **Contents** · **Previous** · **Next**.
- Use the templates for new entries, chapters, rules modules, locations, and stat blocks.

## Audience and Canon

- Use `audience: shared` for spoiler-light material suitable for general readers.
- Use `audience: gm` for adventure content, secrets, stat blocks, and other GM-facing notes.
- Use `canon: current` for the active version of the setting.
- Move superseded material to `99 Archive` instead of maintaining two competing active versions.
- In a `shared` entry, place GM-only material—secrets, adventure hooks, checks—inside a collapsed GM callout: `> [!gm]- Adventure Use`. Players can read the entry without opening it.

## Atlas VTT

- Never move or rename the `atlas-vtt` folder; the plugin requires it at the vault root.
- Create one Atlas collection per release, named with its ID and title, such as `SA-01 The Pact in the Twilight`.
- Pin library notes to scenes instead of writing new text inside Atlas.
- See the [[Atlas VTT Guide]].

## Music

- Every important place and character gets a music recommendation on the [[Soundtrack]] page: either a generic mood or a specific track.
- Credit specific tracks with their title, franchise or work, composer, and rights holder. Never add music files to the vault.

## Names

- **The world, continents, countries, and cities** take names inspired by real-world words for *mirror*, *reflection*, *time*, and *space*, bent so they sound like places rather than dictionary words. The full rules, regional language flavours, and checks are in the [[Naming Guide]].
- **Local places**—forests, inns, roads, temples—use descriptive common-tongue names: Forest of Thieves, To the Eternal Lady, Temple of the Moon in Water.
- **Personal names** follow no fixed rule.
- Record every new name, its pronunciation, and its meaning in the [[Pronunciation Guide]] and in a short "The Name" section of its entry.
- Borrow ordinary words respectfully. Do not use the names of real deities, sacred figures, or sacred objects.

## Rules and Stat Blocks

- Rules material uses the SRD 5.2.1 and its terminology: *Melee Attack Roll*, *Saving Throw* effects with *Failure* and *Success*, capitalized conditions such as Blinded or Frightened, and Emanations for areas centred on a creature.
- Stat blocks follow the [[Stat Block]] template: AC and Initiative, a combined ability and saving-throw table, a single Immunities line, `CR x (XP y; PB +z)`, and sections for Traits, Actions, Bonus Actions, and Reactions.
- **Character options must work in any fifth-edition world.** Subclasses, feats, spells, and similar player options may not depend on setting concepts such as the Mirrorgate or the war-scars in their rules. Put setting lore in a clearly marked optional section titled *In the Mirrored Realms*.
- Keep mechanics in rules modules and stat blocks. Lore entries link to them instead of repeating DCs and effects.

## Writing

- Use clear international English for public project material.
- Distinguish established facts from rumors, open questions, and design notes.
- Do not present announced titles as ready-to-play releases.
- Avoid invented completion dates; production percentages are estimates, not promises.

---

Return to the [[Vault Guide]].
