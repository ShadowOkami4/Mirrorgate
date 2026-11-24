<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: faith
up: "[[<% up %>]]"
player: false
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Overview

## Worship

## The truth

> [!player] What players know
> *Not written yet. Set `player: true` once this box is filled in.*
