<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: rule
up: "[[<% up %>]]"
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

## Rule
