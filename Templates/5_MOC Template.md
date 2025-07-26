---
tags:
  - type/structure
  - structure/moc
aliases:
lead: +++ Lead paragraph goes here +++
visual: "![[image.jpg]]"
theme_tag: ""
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: MOC
template_version: "1.2"
---

# <% tp.file.title %>

<!-- Main STRUCTURE of my content -->
## MOC

### Notes

### Readwise Highlights
```dataview
list
from #theme and "Readwise"
where contains(file.etags, this.theme_tag)
sort modified desc
```

### Terms
```dataview
table lead
from #theme and #type/term 
where contains(file.etags, this.theme_tag)
sort file.name
```

## Others with `= this.theme_tag`
```dataview
table join(sort(file.etags), " ") as tags
from #theme and -(#type/term OR "Readwise")
where contains(file.etags, this.theme_tag)
sort modified desc
```

---
# Back Matter

**Source**
<!-- Always keep a link to the source- --> 
- 

**References**
<!-- Links to pages not referenced in the content. -->
- 

**Terms**
<!-- Links to definition pages. -->
- 

**Target**
<!-- Link to project note or externaly published content. -->
- 

**Tasks**
<!-- What remains to be done with this note? --> 
- 

**Questions**
<!-- What remains for you to consider? --> 
- 
