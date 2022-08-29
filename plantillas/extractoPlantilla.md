---
<%* const dv = this.app.plugins.plugins["dataview"].api;
let bibliographies = dv.pages('"bibliografia"');
let names = bibliographies.name;
let ids = bibliographies.id;
const selectId = await tp.system.suggester(names, ids); -%>
bibliography_id: <%-* tR += selectId; %>
type: extract
subtype: extract
date: <% tp.file.creation_date() %>
---
# Extracto 📃
## Origen
[[Fuente_bibliográfica]]
## Contenido
