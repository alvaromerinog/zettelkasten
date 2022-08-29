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
subtype: document
date: <% tp.file.creation_date() %>
---
# Documento 📄
## Título
<% tp.file.title %>
## Origen
[[<%-* tR += selectName; %>]]
## Contenido
[Mi_document](https://www.google.es)