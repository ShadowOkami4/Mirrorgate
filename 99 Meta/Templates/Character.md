<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: character
up: "[[<% up %>]]"
region: ""
role: ""
status: alive
player: false
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Role

## Wants

## Secret

## Stats

> [!player] What players know
> *Not written yet. Set `player: true` once this box is filled in.*
