---
tags:
  - type/structure
  - structure/journal
aliases: 
created_at: <% tp.date.now(tp.file.title) %>
modified_at: <% tp.file.creation_date("") %>
template-type: Journal Daily
template-version: "1.2"
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
WHERE striptime(created_at) = date(this.file.name) AND file.name != this.file.name
SORT file.mtime DESC
```

**Notes modified today**
```dataview
LIST
FROM ""
WHERE striptime(modified_at) = date(this.file.name) AND file.name != this.file.name
SORT file.mtime DESC
```