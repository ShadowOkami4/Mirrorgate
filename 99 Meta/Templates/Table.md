<%*
const strip = s => s.replace(/^\d+\s+/, "");
const f = tp.file.folder(false);
const up = (!f || f === "/") ? "Home" : strip(f);
const sec = "mr-" + ((tp.file.folder(true).split("/").filter(Boolean)[0] || "home").replace(/^\d+\s+/, "").toLowerCase().replace(/&/g, "").replace(/\s+/g, "-").replace(/-+/g, "-"));
-%>
---
cssclasses:
  - <% sec %>
type: table
up: "[[<% up %>]]"
---

> [!up] [[<% up %>]]

# <% tp.file.title %>

<% tp.file.cursor() %>

| d6 | Result |
| --- | --- |
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
