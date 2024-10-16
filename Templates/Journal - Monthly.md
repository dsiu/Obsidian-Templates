---
tags:
  - type/structure
  - structure/journal
aliases: 
created_at: <% tp.date.now(tp.file.title) %>
modified_at: <% tp.file.creation_date("") %>
template-type: Journal Monthly
template-version: "1.0"
---
# <% tp.file.title %>
```dataview 
LIST flat(rows.file.lists.text)
from #structure/journal
where contains(file.name, this.file.name) AND file.name != this.file.name
GROUP BY file.link
```
