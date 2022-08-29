---
<%* const dv = this.app.plugins.plugins["dataview"].api;
let bibliographies = dv.pages('"bibliografia"');
let names = bibliographies.name;
let ids = bibliographies.id;
const selectId = await tp.system.suggester(names, ids); -%>
bibliography_id: <%-* tR += selectId; %>
type: extract
subtype: image
date: <% tp.file.creation_date() %>
---
# Imágen 🖼
## Título
<% tp.file.title %>
## Origen
[[Fuente_bibliográfica]]
## Contenido
![Mi_Portada](https://c.tenor.com/6YAY7UTOu14AAAAC/awesome-you-are-awesome.gif)