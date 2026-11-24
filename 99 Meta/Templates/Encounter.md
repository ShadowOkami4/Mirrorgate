<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: encounter
up: "[[<% up %>]]"
region: ""
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Setup

## Creatures

## Outcome
