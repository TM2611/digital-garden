---
---

Created: <% tp.file.creation_date("dddd Do MMMM YYYY HH:mm:ss") %>
<%*
let title = tp.file.title
if (title.startsWith("Untitled") ) {
title = await tp.system.prompt("Title: ")
await tp.file.rename(title + ' MOC');
}%>
tags:: #MOC

up:: [[Cerebellum 🧠]]

  

```dataview

TABLE WITHOUT ID

file.link As "Incoming Links"

FROM [[]]

```

```dataview

TABLE WITHOUT ID

file.link As "Outgoing Links"

FROM outgoing([[]])

WHERE !contains(file.tags, "#home")

```