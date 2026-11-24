<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: event
up: "[[<% up %>]]"
era: ""
year: ""
player: false
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## What happened

## Consequences

> [!player] What players know
> *Not written yet. Set `player: true` once this box is filled in.*
