<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: session
up: "[[<% up %>]]"
date: "<% tp.date.now('YYYY-MM-DD') %>"
adventure: ""
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Prep

## Recap

## Next time
