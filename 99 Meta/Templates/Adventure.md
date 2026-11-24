<%*
const strip = s => s.replace(/^\d+\s+/, "");
const name = tp.file.title;
const parts = tp.file.folder(true).split("/").filter(Boolean);
if (parts[parts.length - 1] !== name) {
  await tp.file.move([...parts, name, name].join("/"));
  parts.push(name);
}
const up = parts.length > 1 ? strip(parts[parts.length - 2]) : "Home";
const sec = "mr-" + ((tp.file.folder(true).split("/").filter(Boolean)[0] || "home").replace(/^\d+\s+/, "").toLowerCase().replace(/&/g, "").replace(/\s+/g, "-").replace(/-+/g, "-"));
-%>
---
cssclasses:
  - <% sec %>
type: adventure
up: "[[<% up %>]]"
level: ""
players: ""
---

> [!up] [[<% up %>]]

<% tp.file.cursor() %>

## Summary

## Locations

## Characters

## Chapters

## In this adventure

![[Folder Contents.base]]
