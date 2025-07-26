---
tags:
  - type/structure
  - structure/journal
aliases:
created: <% tp.date.now(tp.file.title) %>T00:00:00
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: Journal Daily
template_version: "1.2"
---
# <% tp.file.title %>
## Notes
- 

--- 
# Back Matter

**Notes created today**
```dataview
LIST
FROM ""
WHERE striptime(created) = date(this.file.name) AND file.name != this.file.name
SORT file.mtime DESC
```

**Notes modified today**
```dataview
LIST
FROM ""
WHERE striptime(modified) = date(this.file.name) AND file.name != this.file.name
SORT file.mtime DESC
```
