<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
const sec = "mr-" + ((tp.file.folder(true).split("/").filter(Boolean)[0] || "home").replace(/^\d+\s+/, "").toLowerCase().replace(/&/g, "").replace(/\s+/g, "-").replace(/-+/g, "-"));
-%>
---
cssclasses:
  - <% sec %>
type: session
up: "[[<% up %>]]"
date: "<% tp.date.now('YYYY-MM-DD') %>"
adventure: ""
---

> [!up] [[<% up %>]]

# <% tp.file.title %>

<% tp.file.cursor() %>

## Prep

## Recap

## Next time
