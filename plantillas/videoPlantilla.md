---
<%-* const year = await tp.system.prompt("Año de creación"); %>
<%-* const keyword = await tp.system.prompt("Palabra clave"); %>
<%-* const author = await tp.system.prompt("Autor"); %>
<%-* const firstSurnameAuthor = tp.user.utils(author); %>
id: <% firstSurnameAuthor + "_" + keyword + "_" + year%>
name: <% tp.file.title %>
type: bibliography
subtype: video
date: <% tp.file.creation_date() %>
author: <% tp.file.author %>
keyword: <%* tR += keyword %>
status: <%tp.system.suggester(["Sin empezar", "En Progreso", " Completado"], ["Not Started", "In Progress", " Completed"])%>
year: <%* tR += year %>
---
# Video ▶
## Nombre
<% tp.file.title %>
## Enlace
[Video](https://www.youtube.es)
## Autor
[Mi_autor](https://www.google.es)
