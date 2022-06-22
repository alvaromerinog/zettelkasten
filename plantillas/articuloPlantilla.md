---
<%-* const year = await tp.system.prompt("Año de creación"); %>
<%-* const keyword = await tp.system.prompt("Palabra clave"); %>
<%-* const author = await tp.system.prompt("Autor"); %>
<%-* const firstSurnameAuthor = tp.user.utils(author); %>
id: <% firstSurnameAuthor + "_" + keyword + "_" + year%>
type: bibliography
subtype: article
date: <% tp.file.creation_date() %>
author: <% tp.file.author %>
keyword: <%* tR += keyword %>
status: <%tp.system.suggester(["Sin empezar", "En Progreso", " Completado"], ["Not Started", "In Progress", " Completed"])%>
year: <%* tR += year %>
---
# Artículo 👩‍🏫
## Nombre
<% tp.file.title %>
## Autor
[Mi_autor](https://www.google.es)
## Enlace
[<% tp.file.title %>](https://www.google.es)
