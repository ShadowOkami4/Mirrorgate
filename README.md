<div align="center">
  <h1>The Mirrored Realms</h1>
  <p><strong>An evolving campaign setting of living reflections, broken time, folded space, and divine scars.</strong></p>
  <p>
    <code>5.5e compatible</code> ·
    <code>SRD 5.2.1</code> ·
    <code>CC BY 4.0</code> ·
    <code>Obsidian vault</code> ·
    <code>Atlas VTT ready</code> ·
    <code>active development</code>
  </p>
  <p>
    <a href="https://shadowokami.com/MirrorGate">Project website</a> ·
    <a href="Home.md">Open the vault</a> ·
    <a href="#getting-started">Getting started</a> ·
    <a href="#release-roadmap">Roadmap</a> ·
    <a href="#contributing">Contributing</a> ·
    <a href="#license-and-attribution">License</a>
  </p>
</div>

---

> [!IMPORTANT]
> **The Mirrored Realms is in early development.** The setting is growing, but it is not yet a complete, ready-to-run campaign. Lore, mechanics, names, maps, and planned releases may change during writing and playtesting.

## Contents

- [About the Setting](#about-the-setting)
- [The Known World](#the-known-world)
- [Getting Started](#getting-started)
- [Repository Layout](#repository-layout)
- [Reading the Vault](#reading-the-vault)
- [Rules and Game Material](#rules-and-game-material)
- [Playing at the Table](#playing-at-the-table)
- [Release Roadmap](#release-roadmap)
- [How This World Is Made](#how-this-world-is-made)
- [Contributing](#contributing)
- [Credits](#credits)
- [License and Attribution](#license-and-attribution)

## About the Setting

**The Mirrored Realms** is both the name of this project and of its fifth-edition campaign setting. Its central world, **Kagameru**, still bears the wounds of an ancient divine war. Roads can arrive in the wrong century, ruins remember histories that never happened, and mirrors sometimes open toward places no map can contain.

The project combines setting lore, characters, factions, creatures, homebrew rules, and playable adventures in one interconnected archive. It supports one-shots, short multishot adventures, and long-form campaigns without requiring every table to follow the same version of history.

| At a glance | |
| --- | --- |
| **World** | Kagameru |
| **Central mystery** | the Mirrorgate and the Scars of the Primordial War |
| **Present age** | the Shattered Hope Era |
| **Main campaign** | Shattered Hope (CF-01) |
| **Rules foundation** | fifth edition, using the System Reference Document 5.2.1 |
| **Format** | Obsidian vault of linked Markdown notes |
| **Virtual tabletop** | Atlas VTT (optional) |
| **License** | CC BY 4.0 for original project material |

## The Known World

<p align="center">
  <img src="90%20Assets/Maps/Kagameru_World_Map.jpg" alt="Physical map of Kagameru, showing Specula, Drychwen, Scáthan, Veidra, Skuggsjá, Tezcatl, and the Southern Ice" width="100%">
</p>

<details>
<summary><strong>View the political map</strong></summary>
<p align="center">
  <img src="90%20Assets/Maps/Kagameru_Political_Map.jpg" alt="Political map of Kagameru, showing its realms and their borders" width="100%">
</p>
</details>

> [!WARNING]
> **This is an early version of the world map.** Coastlines, borders, realms, and the positions of places may still change wherever they do not fit the stories being written. When the map and the stories disagree, the stories decide.

The map previews are made with a self-made AI-assisted simulation. The maps themselves are then generated from a single seed (`27182818`) through procedural generation: terrain, erosion, climate, and biomes are simulated first, and rivers, realms, settlements, roads, and railways are placed on top.

| Property | Value |
| --- | --- |
| Extent | 12,000 × 10,000 km |
| Projection | flat, origin at the north-west corner; x runs east, y runs south |
| Full resolution | 12,000 × 10,000 px (1 px ≈ 1 km) |
| Images in this repository | 2,400 px wide copies in `90 Assets/Maps/` |
| Source files | kept locally, outside the vault; not published, because the full-size renders exceed 20 MB each |

## Getting Started

### Requirements

- [Obsidian](https://obsidian.md/) **1.8.7 or newer**. Reading the vault works on any platform; Atlas VTT and Enhancing Export are desktop-only.
- *Optional:* [Pandoc](https://pandoc.org/), if you want to export notes or books with Enhancing Export.

### Opening the Vault

1. Clone or download the repository.

   ```shell
   git clone https://github.com/ShadowOkami4/Mirrorgate.git
   ```

2. Open the repository folder as a vault in Obsidian.
3. When Obsidian asks, trust the vault's community plugins so that its layout, callouts, and tools work as intended.
4. Open [`Home.md`](Home.md) and follow whichever section catches your attention.

> [!NOTE]
> Internal links such as `[[The Mirrorgate]]` are written for Obsidian and do not resolve on GitHub. The navigation links in this README use relative paths and work in both.

### Included Plugins and Settings

The shared vault settings in `.obsidian/` enable the following community plugins. None of them is required to read the notes as plain Markdown.

| Plugin | Purpose in this vault |
| --- | --- |
| Atlas VTT | battle maps, tokens, fog of war, dice, initiative, and a player view |
| Dice Roller | inline dice rolls in notes |
| Enhancing Export | export of notes and books to PDF, DOCX, and other formats (requires Pandoc) |
| Pixel Banner | banner images at the top of notes |
| Iconize | folder and note icons |
| File Explorer++ | filtering and pinning in the file explorer |
| Templater | note templates that link each new note to its section |
| QuickAdd | *New Place*, *New Character*, *New Secret*, *New Area* … commands that create a note in the right folder |
| Homepage | opens `Home.md` when the vault starts |
| Style Settings | options for the theme and CSS snippets |
| Claudian | the maintainer's AI assistant (see [A Note on AI](#a-note-on-ai)); not needed to read or play |

The tables inside hub notes use Obsidian's core **Bases** plugin. The vault uses its own theme, **[Mirrored Pages](https://github.com/ShadowOkami4/mirrored-pages)** (silver-mirror look, dark and light, also styles Atlas VTT), which also styles the Player info box (`> [!player]`) and GM callouts (`> [!gm]-`). The CSS snippet `mirrored-realms` gives each section card on the hub notes its own icon and colour, matching the graph view.

## Repository Layout

> [!NOTE]
> **The vault is being rebuilt (November 2026).** The folders below are the new skeleton; notes are rewritten section by section. The previous version is in the git history.

The vault is written for **Game Masters**. Every page tells the whole story; text players may read sits in a **Player info** box at the bottom of the page.

| Path | Contents |
| --- | --- |
| `Home.md` | the entrance: the world map, where to start, and every section |
| `01 Atlas/` | places, nested like the map: continent → realm → settlement → site |
| `02 Characters/` | everyone the GM may play or mention |
| `03 Factions/` | houses, orders, guilds, churches, cults |
| `04 History/` | eras and events as they really happened |
| `05 Faiths & Cosmos/` | deities, planes, the Mirrorgate |
| `06 Peoples/` | species and cultures |
| `07 Secrets/` | hidden truths and twists, linked to the pages they explain |
| `08 Adventures/` | ready-to-run adventures, one folder each |
| `09 Rules/` | core rules, character options, bestiary |
| `10 Books/` | compiled book editions |
| `90 Assets/` | maps and art; `90 Assets/Private/` is kept local and not published |
| `99 Meta/` | the World Bible, the GM Toolkit (encounters, tables, sessions), templates and views |
| `.obsidian/` | shared vault settings, plugins, theme |

These paths are excluded from the repository by `.gitignore`:

| Path | Reason |
| --- | --- |
| `atlas-vtt/` | local Atlas VTT data: personal settings, test scenes, and the plugin's third-party starter tokens. The plugin requires this folder at the vault root; never move or rename it. |
| `Private/`, `90 Assets/Private/` | private files and images that are kept local and not published |
| `.obsidian/workspace.json` | personal window layout |
| `.claude/`, `.claudian/` | local AI assistant data |

## Reading the Vault

- **By folder.** Every folder has a hub note with the folder's name (`Atlas.md`, `Characters.md` …). Its *In this section* table lists what is inside.
- **By graph.** Every note's `up` property links to its hub, and every hub links up to [Home](Home.md), so the graph branches out from Home. Each section has its own colour; pages with a finished player box are parchment-coloured.
- **By table.** Each hub's *In this section* table (a Bases view) lists what is in its folder, including the `player` column.

### Player Info

The last block of a lore page is the player box:

```markdown
> [!player] What players know
> Ogledal is the royal capital of Lustro, known for its mirrored bridges.
```

The Mirrored Pages theme draws it with a *Player info* corner ribbon. Set `player: true` in the page's properties once the box is written.

### Note Properties

Every note carries YAML front matter, hidden in the reading view. Templates in `99 Meta/Templates/` fill it in; QuickAdd's *New Place*, *New Character*, *New Secret* … commands create notes in the right folder.

| Property | Meaning |
| --- | --- |
| `type` | `place`, `character`, `faction`, `event`, `faith`, `people`, `secret`, `adventure`, `encounter`, `table`, `session`, `rule`, `creature`, `hub` |
| `up` | the hub (or containing place) the note belongs to |
| `player` | `true` once the page has a finished Player info box |
| `region` | where it is, for places, characters and factions |

## Rules and Game Material

All rules material targets fifth edition and uses the terminology and stat block format of the **System Reference Document 5.2.1**.

- **Character options**, such as the Mirrorbound fighter and Scarborn Sorcery, work in any fifth-edition world. Setting lore is kept in an optional section, *In the Mirrored Realms*.
- **Creatures** use the current stat block layout: AC and Initiative, a combined ability and saving-throw table, `CR x (XP y; PB +z)`, and separate Traits, Actions, Bonus Actions, and Reactions.
- **Rules modules**, such as Scar Hazards, keep mechanics out of the lore entries.

> [!NOTE]
> Subclasses, creatures, and rules modules are **playtest drafts**. Numbers may change.

## Playing at the Table

### Atlas VTT

The vault is set up for **[Atlas VTT](https://github.com/ByteMirror/atlas-vtt)** by **Fabian Urbanek** ([ByteMirror](https://github.com/ByteMirror)), a free and open-source Obsidian plugin that turns the vault into a virtual tabletop. It is optional; every note can be read and run without it.

> [!WARNING]
> Atlas VTT stores its data in an `atlas-vtt` folder at the root of the vault. The plugin requires that exact location: **do not move or rename the folder**, or existing maps will break.

### Soundtrack

Every important place and character has a music recommendation. Some are generic moods; others are specific tracks from these games:

| Franchise | Rights holder |
| --- | --- |
| *Celeste* (music by Lena Raine) | © Maddy Makes Games |
| *The Legend of Zelda* | © Nintendo |
| *Super Mario* | © Nintendo |
| *Professor Layton* | © Level-5 |

> [!IMPORTANT]
> **These are only recommendations.** No music is included in this repository. Every named track belongs to its composer and rights holders. Please listen through official sources.
>
> **Self-made remixes are planned for every track.** Remixes of copyrighted music will only be published where that is permitted, and they are not covered by the project's CC BY 4.0 license.

## Release Roadmap

The planned collection contains **18 journeys**: ten one-shots, five short adventures or multishots, and three campaign frameworks. A title being announced does not mean active development has begun.

| Collection | Planned | Announced | In development |
| --- | ---: | ---: | ---: |
| One-shots | 10 | 2 | 0 |
| Short adventures / multishots | 5 | 3 | 1 |
| Campaigns / campaign frameworks | 3 | 1 | 1 |
| **Total** | **18** | **6** | **2** |

### Current Production

| Release | Kind | State | Progress | Current work |
| --- | --- | --- | ---: | --- |
| The Pact in the Twilight | short adventure | `ACTIVE DRAFT` | **25%** | Prelude and Chapters 1–3 drafted; outlining the rest of the adventure |
| Shattered Hope | main campaign | `FOUNDATION` | **1%** | defining the campaign spine and its major arcs |

<details>
<summary><strong>View current development milestones</strong></summary>

#### The Pact in the Twilight

- [x] Draft the opening premise, forest journey, and meeting with Sandra
- [x] Draft the first chapters: the road north, the temple, and the sanctum behind the mirror
- [ ] **Complete the adventure outline and chapter structure — current work**
- [ ] Add encounters, maps, creature statistics, and consequences
- [ ] Add rewards, scaling, and Game Master guidance
- [ ] Playtest, revise, and prepare the adventure for release

#### Shattered Hope

- [x] Establish the era, tone, and central campaign question
- [ ] **Define the campaign spine and major arcs — current work**
- [ ] Assign factions, antagonists, and major locations to each arc
- [ ] Design the adventure sequence, encounters, and rewards
- [ ] Playtest, revise, and prepare the campaign framework for release

</details>

> [!NOTE]
> Progress percentages are editorial estimates, not release dates. They describe how much of the intended finished work has been drafted, revised, and prepared for playtesting.

<details>
<summary><strong>View the full release catalogue</strong></summary>

#### Status Key

| State | Meaning |
| --- | --- |
| `UNANNOUNCED` | a reserved roadmap slot without a public title |
| `ANNOUNCED` | the title and premise are public, but active development has not begun |
| `FOUNDATION` | core structure and campaign architecture are being established |
| `ACTIVE DRAFT` | playable material is currently being written |

#### One-shots — 10 planned

| ID | Title | State | Notes |
| --- | --- | --- | --- |
| OS-01 | **The Dark Alley** | `ANNOUNCED` | a complete rewrite of an older original one-shot, rebuilt to fit the Mirrored Realms |
| OS-02 | **Mirror and Scars** | `ANNOUNCED` | an episodic series whose episodes can each be played on their own; the series occupies one slot |
| OS-03 – OS-10 | — | `UNANNOUNCED` | |

#### Short Adventures / Multishots — 5 planned

| ID | Title | State | Notes |
| --- | --- | --- | --- |
| SA-01 | **The Pact in the Twilight** | `ACTIVE DRAFT` · **25%** | the first short adventure in active development |
| SA-02 | **Confronting Yourself** | `ANNOUNCED` | development has not begun |
| SA-03 | **The Mysteries of the Phantomhives** | `ANNOUNCED` | development has not begun |
| SA-04 – SA-05 | — | `UNANNOUNCED` | |

#### Campaigns / Campaign Frameworks — 3 planned

| ID | Title | State | Notes |
| --- | --- | --- | --- |
| CF-01 | **Shattered Hope** | `FOUNDATION` · **1%** | the main campaign of the Mirrored Realms |
| CF-02 – CF-03 | — | `UNANNOUNCED` | |

</details>

### Development Principles

- **Playability before volume:** a smaller finished adventure is more valuable than many disconnected drafts.
- **Mystery with usable answers:** players may encounter uncertainty, but Game Masters should receive enough truth to run the setting confidently.
- **Connected, not linear:** records reward curiosity and cross-reference related lore without demanding a fixed reading order.
- **Open by design:** tables may reuse, alter, publish, and build upon original project material under CC BY 4.0.
- **Revision is expected:** early concepts may change when stronger ideas emerge through writing, feedback, and playtesting.

## How This World Is Made

The Mirrored Realms is created by **Okami**. The world has been in the making for about two years, and many earlier versions were written, played with, and scrapped before this one.

**The storytelling is made by human hand, and it will stay that way.** The world's vision, its history, its characters, how the stories unfold, and where they are going are planned and written by Okami.

### A Note on AI

I will not hide or lie about it: I use AI. [Claude](https://claude.ai), an AI assistant by Anthropic, helps me as a tool in a few limited areas:

- checking that the world map and the written lore agree with each other;
- checking grammar and spelling;
- minor help with balancing the game mechanics of subclasses, monsters, and items;
- organizing the vault and rewording existing entries from my own notes and ideas;
- the self-made simulation that helps prepare the world map previews.

What I will not use AI for is the story itself. The plot, the characters, the direction of the adventures, and the vision of the world come from me. This world has taken years and many scrapped versions to grow into what it is, and I don't want that vision replaced by AI. Where AI has helped with wording, the story decisions behind it are still mine, and anything that does not match my vision gets rewritten.

I also do not use AI-generated artwork. Every image in the Mirrored Realms is made by a person.

## Contributing

Corrections, playtest reports, writing, mechanics, and original artwork are welcome through [GitHub Issues](https://github.com/ShadowOkami4/Mirrorgate/issues) and pull requests.

1. Open an issue describing the correction, idea, or playtest report.
2. For changes to the vault, fork the repository, make your edits in Obsidian, and open a pull request.
3. Keep to the style of the existing notes, and give every new note complete front matter (see [Note Properties](#note-properties)).
4. Move or rename notes inside Obsidian so that links update; never move the `atlas-vtt` folder.

By contributing original material, you agree to make it available under the project's [CC BY 4.0 license](LICENSE). You keep authorship and receive credit for accepted work. Submit only material you created or have the right to release under those terms, and do not submit protected text, artwork, characters, or settings from games and fictional universes you do not control.

### Artwork and Artist Contributions

**Artwork contributions are extremely welcome.** The Mirrored Realms has no public artwork yet, and I am actively looking for artists to bring its characters, creatures, places, and maps to life. I am saving up money so that I can commission artists properly.

Artists are invited to propose original character art, creatures, locations, maps, symbols, items, or any other visual interpretation of the Mirrored Realms. Every accepted work will credit its artist.

- **Paid commissions** are planned as soon as the budget allows. Scope, schedule, price, attribution, and usage rights will be agreed in writing before any work begins.
- **Voluntary contributions** are just as welcome.
- Artwork in this repository must be original, and the artist must have the right to release it under [CC BY 4.0](LICENSE). Payment never removes the artist's right to be credited.
- Artwork must be made by the artist without generative AI. AI-generated images are not accepted.

To propose artwork or get in touch about a commission, open an [artwork proposal issue](https://github.com/ShadowOkami4/Mirrorgate/issues) with:

- the subject or part of the setting you want to illustrate;
- a portfolio or relevant examples, if available;
- your preferred artist credit and links;
- whether you are offering voluntary work or a commission; and
- any schedule, format, or accessibility considerations.

## Credits

**The Mirrored Realms** — world, story, and adventures — is created by **Okami**.

**Atlas VTT** — the virtual tabletop plugin this vault is set up for — is created by **Fabian Urbanek** ([ByteMirror](https://github.com/ByteMirror)). It began as part of his bachelor's thesis, with the goal of giving the tabletop community a virtual tabletop that is open source, hackable, and free to use. Many thanks for making it. If you enjoy playing the Mirrored Realms with Atlas VTT, consider starring or supporting the [Atlas VTT project](https://github.com/ByteMirror/atlas-vtt).

## License and Attribution

| Material | License |
| --- | --- |
| Original Mirrored Realms material (text, rules, maps, contributed artwork) | [CC BY 4.0](LICENSE) |
| Material from the System Reference Document 5.2.1 | CC BY 4.0, by Wizards of the Coast LLC |
| Obsidian plugins and themes in `.obsidian/` | their own licenses; Atlas VTT is licensed under the GNU AGPL |
| Recommended music | not included; all rights remain with the rights holders |

Except where stated otherwise, original material created for **The Mirrored Realms** may be copied, adapted, redistributed, published, and used commercially with appropriate credit. A simple attribution names **The Mirrored Realms** and links to the [project website](https://shadowokami.com/MirrorGate) or this repository.

See [NOTICE.md](NOTICE.md) for a ready-to-use attribution statement, the required SRD 5.2.1 notice, and third-party exclusions.

---

<div align="center">
  <p><em>The realm is unfinished. Its possibilities are not.</em></p>
</div>
