---
tags: 
- type/question
- theme/xyz
aliases:
question: +++ Question goes here +++
lead: +++ Lead paragraph goes here +++
visual: "![[image.jpg]]"
created_at: <% tp.file.creation_date("") %>
modified_at: <% tp.file.creation_date("") %>
template_type: Question
template_version: "1.25"
---

# <% tp.file.title %>

<!-- Detailed question from "lead"-key  in properties section -->

> [!Question]
> `= this.question`

<% tp.file.cursor(0) %>

<!-- Answer the detailed question  -->
> [!Answer]
> `= this.lead`


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
- 
