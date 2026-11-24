---
type: guide
up: "[[Meta]]"
tags:
  - guide
---

↑ [[Meta]]

# World Bible

How Kagameru is built. Carried over from the old cartography project when the vault was rebuilt (2026-11-24). **Canon is open:** every rule below is up for review. Mark each one *keep*, *change* or *drop* as the rewrite settles it.

## 1. The world as a planet

### Why v3

v2 simulates a flat 12,000 × 10,000 km rectangle with square 10 km cells and no east–west wrap. On a real globe
that breaks: at Skuggsjá (79° N) a cell would be five times narrower east–west than north–south, so rivers,
borders and distances there would be distorted. Continents in v2 are ellipses ("lobes") around anchors, realm
borders grow from capitals through deliberate noise, railways are built after (and stop at) today's borders,
and sea routes run on an eight-direction grid.

### Decisions (user, 2026-10-17)

- **Full globe rebuild.** Plate tectonics on a sphere; the map shows the whole planet and wraps east–west.
  Continents keep their lore latitude, climate and relative position; their shapes change.
- **Railways: mixed.** An ancient core network that predates today's realms and crosses their borders
  (crossings may be open, controlled or closed), plus newer national branch lines.
- **Railways only on Specula and Veidra.**
- Borders: natural (watersheds, crests, large rivers, lakes), Lustro bounded by mountains like Switzerland;
  far less jagged in Specula.
- Sea routes: proper shipping lanes, not grid staircases.
- Keep all lore names, and the realm and seat names already listed in the Naming Guide.

### Architecture

| Layer | v3 |
| --- | --- |
| Geometry | jittered Fibonacci mesh on a sphere of radius 10,000/π km (pole to pole 10,000 km); ~10 km spacing (≈1.27 M nodes), coarse 20 km mesh for the long erosion run |
| Noise | 3-D value noise sampled on the sphere (no seams, no polar pinching) |
| Terrain | plates as warped spherical Voronoi cells with Euler-pole motion; convergence → belts, arcs; divergence → rifts; continental crust from domain-warped noise around the lore anchors; stream-power erosion, sediment, hillslope and marine diffusion on the mesh graph |
| Climate | latitude–longitude grid (wraps), wind belts and moisture advection with the true metric; sampled onto the mesh |
| Hydro, biomes | on the mesh graph |
| Realms | built from watershed units (sub-catchments split along large rivers); realms grow over the unit graph, so borders follow divides, crests, rivers and lakes |
| Railways | ancient core (gravity model, built before realms) + national branches; 2 % grade, tunnels, gauges, crossings with status |
| Sea routes | lanes on the ocean graph that bundle onto shared trunks, then string-pulled and drawn as smooth curves |
| Maps | world in the Equal Earth projection (whole planet), orthographic globes, Specula and Veidra in Lambert azimuthal equal-area; rendering reuses the v2 cartography (relief, hachures, forests, labels) on rasters projected from the mesh |

### Stages

`sphere → terrain → climate → hydro → biomes → rivers → scars → civ → resources → rail → sea → vector → render → checks`

## 2. Inherited lore rules

Rules the old maps were checked against. **Hard** rules were treated as fixed, **soft** ones as strong preferences. The notes they came from are in git history (commit `4f79149`).

| ID | Type | Subject | Rule | Review |
| --- | --- | --- | --- | --- |
| H01 | hard | world | The world is named Kagameru. | |
| H02 | hard | continents | Exactly six named great landmasses: Specula, Drychwen, Scathan, Veidra, Skuggsja, Tezcatl. | |
| H03 | hard | Skuggsja | Lies in the far north; cold seas and hard winters (cold biomes dominate, coast on a cold sea). | |
| H04 | hard | Tezcatl | The sun-scorched south: southernmost continent, hot climate (desert/savanna/tropical dominant). | |
| H05 | hard | Specula | The heartland of Kagameru: the continent nearest the centre of the known world. | |
| H06 | hard | Lustro | A kingdom on Specula; the central kingdom of Kagameru (central within Specula). | |
| H07 | hard | Ogledal | Royal capital of Lustro, inside Lustro. | |
| H08 | hard | Hansha | A homeland region of familiar hills (hilly terrain) containing the town Utsushi. | |
| H09 | hard | Utsushi | An academy-town (town tier) located in Hansha. | |
| H10 | hard | Forest of Thieves | One bounded, dense, badly roaded wood about 90-130 km across (8 000-15 000 km²); the oldest part of a larger woodland, which keeps its own common-tongue name (the Southern Weald). | |
| H11 | hard | To the Eternal Lady | Current site in the southern third of the Forest of Thieves, 10-20 km inside its southern edge, 2-4 km off the Old Road in a sheltered hollow, reached by an unmarked side path; not on the road network. | |
| H12 | hard | Temple of the Moon in Water | In the northern third of the Forest of Thieves, 25-35 km north (N to NNW) of To the Eternal Lady, with no settlement between them. | |
| H13 | hard | Temple of the Moon in Water | Stands in forest; a spring or stream within 1 km feeds its still courtyard pool; slightly higher ground than the inn is welcome. | |
| H14 | hard | naming | World, continents, countries, kingdoms, and major cities take names inspired by (never identical to) real-world words for mirror, reflection, time, or space; 2-4 syllables; no diacritics or apostrophes; one language flavour per region. | |
| H15 | hard | naming | Forests, inns, roads, rivers, seas, ranges and other landmarks use common-tongue descriptive names. | |
| H16 | hard | naming | Existing lore names are used exactly as written (Specula, Drychwen, Scáthan, Veidra, Skuggsjá, Tezcatl, Lustro, Hansha, Ogledal, Utsushi). | |
| H17 | hard | naming | No names of real deities, sacred figures, or sacred objects. | |
| H18 | hard | Forest of Thieves | Lawless frontier at the edge of Spazienza: claimed by no realm, so no realm polices its road. | |
| H19 | hard | Forest of Thieves | No settlement inside the forest; two or three small villages on its southern edge as the last outposts, Glasscombe among them. | |
| H20 | hard | Forest of Thieves | Exactly one old road crosses the forest, roughly north to south; thieves ambush travellers on it. | |
| H21 | hard | Forest of Thieves | At least one stream crossing (a ford) a short walk north of the inn on the way to the temple. | |
| H22 | hard | Forest of Thieves | The region map shows the whole forest, its edge villages, the Old Road, the inn, the temple and the nearest town on its southern side, all labelled. | |
| S01 | soft | Drychwen | Old forests dominate. | |
| S02 | soft | Veidra | Green realms and ancient groves: wet, forested. | |
| S03 | soft | Scathan | Long nights (high latitude) and long, shadowed coasts. | |
| S04 | soft | Scathan | Lies at the edge of the known world as drawn on most maps. | |
| S05 | soft | Tezcatl | Volcanic glass (obsidian) is available: a volcanic arc on Tezcatl. | |
| S06 | soft | Tezcatl | Stone cities and great temples: several large settlements. | |
| S07 | soft | Specula | Several old kingdoms with knightly houses (more than one realm). | |
| S08 | soft | Skuggsja | Isolated holds: sparse settlement. | |
| S09 | soft | world | Kingdoms keep border forts; borderlands hold impossible ruins. | |
| S10 | soft | Scars of the Primordial War | War-scars exist as sites (glasslike craters, ruined battlefields); shown as ruin sites. | |
| S11 | soft | Dwarves | Mountain holds and fortified settlements in mountains. | |
| S12 | soft | Lustro | Lustro has disputed borderlands and border conflicts over ruins. | |
| S13 | soft | Hansha | Hansha is distinct from Lustro (its status is open; a separate realm is one listed option). | |
| S14 | soft | archive | Superseded draft placed the Blackwoods on 'Avaloria' and the Phantomhives on 'Noctheris'. Informational only; not applied. | |
