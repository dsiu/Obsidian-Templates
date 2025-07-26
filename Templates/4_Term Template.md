---
tags:
  - type/term
  - theme/xyz
aliases:
lead: +++ Term definition goes here +++
source: +++ source undefined +++
visual: "![[image.jpg]]"
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: Term
template_version: "1.22"
---

# <% tp.file.title %>
<!--  Clear and descriptive title -->

<!-- A supporting visual from front matter if available -->

```dataviewjs
dv.paragraph(dv.current().visual);
```


<!-- Term definition and source from front matter goes here. Also used for Dataview glossary. -->

> [!Definition]
> `= this.lead`
>  — `= this.source`

<!-- Additional term description if needed -->




---
# Back Matter

**Source**
<!-- Always keep a link to the source- --> 
- based_on::

**References**
<!-- Links to pages not referenced in the content. see: [[related note]] because <reason> -->
- see:: 

**Terms**
<!-- Links to definition pages. -->
- 

**Target**
<!-- Link to project note or externaly published content. -->
- used_in::

---
**Tasks**
<!-- What remains to be done with this note? --> 
- 

**Questions**
<!-- What remains for you to consider? --> 
- question::
