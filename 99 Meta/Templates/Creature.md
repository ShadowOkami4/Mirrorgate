<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: creature
up: "[[<% up %>]]"
cr: ""
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Description

## Statblock
