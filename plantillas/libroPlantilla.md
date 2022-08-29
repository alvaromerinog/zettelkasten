---
<%-* const year = await tp.system.prompt("Año de creación"); %>
<%-* const keyword = await tp.system.prompt("Palabra clave"); %>
<%-* const author = await tp.system.prompt("Autor"); %>
<%-* const firstSurnameAuthor = tp.user.utils(author); %>
id: <% firstSurnameAuthor + "_" + keyword + "_" + year%>
name: <% tp.file.title %>
type: bibliography
subtype: book
date: <% tp.file.creation_date() %>
author: <% tp.file.author %>
keyword: <%* tR += keyword %>
status: <%tp.system.suggester(["Sin empezar", "En Progreso", " Completado"], ["Not Started", "In Progress", " Completed"])%>
year: <%* tR += year %>
---
# Libro 📗
## Título
<% tp.file.title %>
## Autor
[Mi_autor](https://www.google.es)
## Portada
![Mi_Portada](https://c.tenor.com/6YAY7UTOu14AAAAC/awesome-you-are-awesome.gif)
## Url
[<% tp.file.title %>](https://www.google.es)
