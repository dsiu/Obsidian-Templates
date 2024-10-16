---
tags: 
- type/structure
- structure/xyz
aliases: 
lead: +++ Lead paragraph goes here +++
visual: "![[image.jpg]]"
created_at: <% tp.file.creation_date("") %>
modified_at: <% tp.file.creation_date("") %>
template_type: Structure
template_version: "1.15"
---

# <% tp.file.title %>
<!--  Clear and descriptive title -->

<!-- Visual or sketchnote if available -->

```dataviewjs 
dv.paragraph(dv.current().visual);
```

<!--  Summarized structure from "lead"-key  in properties section -->

> [!Note]
> `= this.lead`

<!-- Main STRUCTURE of my content -->
- 

<% tp.file.cursor(0) %>

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
