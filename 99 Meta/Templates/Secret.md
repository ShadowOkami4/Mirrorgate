<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: secret
up: "[[<% up %>]]"
reveals: []
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## The truth

## Clues

## When it comes out
