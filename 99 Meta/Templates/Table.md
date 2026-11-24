<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
-%>
---
type: table
up: "[[<% up %>]]"
---

↑ [[<% up %>]]

<% tp.file.cursor() %>

| d6 | Result |
| --- | --- |
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
