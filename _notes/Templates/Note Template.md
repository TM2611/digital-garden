---
---

Created: <% tp.file.creation_date("dddd Do MMMM YYYY HH:mm:ss") %>
<%\*
let title = tp.file.title
if (title.startsWith("Untitled") ) {
title = await tp.system.prompt("Title: ")
await tp.file.rename("F - " + title);
}%>

# Topic/Concept/Idea


# Context


# Thoughts/Questions


# Connections


