---
<%* const dv = this.app.plugins.plugins["dataview"].api;
let bibliographies = dv.pages('"bibliografia"');
let names = bibliographies.name;
let ids = bibliographies.id;
const selectId = await tp.system.suggester(names, ids);
const selectNameIndex = ids.indexOf(selectId);
const selectName = names[selectNameIndex]; -%>
bibliography_id: <%-* tR += selectId; %>
type: extract
subtype: annotate
date: <% tp.file.creation_date() %>
---

# Annotate ✍
## Título
<% tp.file.title %>
## Origen
[[<%-* tR += selectName; %>]]
## Contenido
