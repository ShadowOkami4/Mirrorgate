<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: faction
up: "[[<% up %>]]"
region: ""
player: false
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Overview

## Goals

## Members

## Resources

> [!player] What players know
> *Not written yet. Set `player: true` once this box is filled in.*
