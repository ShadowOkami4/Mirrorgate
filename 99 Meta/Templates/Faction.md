<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
const sec = "mr-" + ((tp.file.folder(true).split("/").filter(Boolean)[0] || "home").replace(/^\d+\s+/, "").toLowerCase().replace(/&/g, "").replace(/\s+/g, "-").replace(/-+/g, "-"));
-%>
---
cssclasses:
  - <% sec %>
type: faction
up: "[[<% up %>]]"
region: ""
player: false
---

> [!up] [[<% up %>]]

<% tp.file.cursor() %>

## Overview

## Goals

## Members

## Resources

> [!player] What players know
> *Not written yet. Set `player: true` once this box is filled in.*
