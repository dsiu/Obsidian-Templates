---
tags: 
- type/term
- theme/xyz
aliases: 
lead: +++ Term definition goes here +++
source: +++ source undefined +++
visual: "![[image.jpg]]"
created_at: <% tp.file.creation_date("") %>
modified_at: <% tp.file.creation_date("") %>
template_type: Term
template_version: "1.20"
---

# {{Title}}
<!--  Clear and descriptive title -->

<!-- A supporting visual from front matter if available -->

```dataviewjs 
dv.paragraph(dv.current().visual);
```

# <% tp.file.title %>

<!-- Term definition and source from front matter goes here. Also used for Dataview glossary. -->

> [!Definition]
> `= this.lead`
>  — `= this.source`

<% tp.file.cursor(0) %>

<!-- Additional term description if needed -->



---
# Back Matter

**Source**
<!-- Always keep a link to the source- --> 
- based_on:: `= this.source`

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
