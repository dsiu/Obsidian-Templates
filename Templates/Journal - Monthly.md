---
tags:
  - type/structure
  - structure/journal
aliases:
created: <% tp.date.now(tp.file.title + "-01T00:00:00Z") %>
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: Journal Monthly
template_version: "1.0"
---
# <% tp.file.title %>
```dataview 
LIST flat(rows.file.lists.text)
from #structure/journal
where contains(file.name, this.file.name) AND file.name != this.file.name
GROUP BY file.link
```
