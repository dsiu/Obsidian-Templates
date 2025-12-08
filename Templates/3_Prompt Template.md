---
tags:
- type/prompt
- theme/xyz
- source/ai
aliases:
question: +++ Question goes here +++
lead: +++ Lead paragraph goes here +++
visual: "![[image.jpg]]"
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: Prompt
template_version: "1.17"
---

# <% tp.file.title %>

<!-- Detailed question from short title in front matter -->

> [!Note]
> `= this.lead`

> [!Prompt]
> `Q: <question>` 
> `A: <answer>`

<!-- Detailed response or dialog  -->



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
