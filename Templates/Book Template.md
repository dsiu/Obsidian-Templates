---
tags: 
- type/book
- theme/xyz
aliases: 
lead: +++ Lead paragraph goes here +++
visual: "![[image.jpg]]"
title: "{{title}}"
subtitle: {{subtitle}}
author: "[[{{author}}]]"
authors: <%=book.authors.map(author=>`\n  - "[[${author}]]"`).join('')%>
category: {{category}}
publisher: {{publisher}}
publish_date: {{publishDate}}
total_page: {{totalPage}}
isbn: {{isbn10}} {{isbn13}}
cover_url: {{coverUrl}}
cover_small_url: {{cover_small_url}}
description:
link: {{link}}
preview_link: {{preview_link}}
bibliography: +++ Copy here from Zotero +++
rating: 
date:
read: 
status: undefined
created: {{DATE:YYYY-MM-DDTHH:mm:ss}}
modified: {{DATE:YYYY-MM-DDTHH:mm:ss}}
template_type: Book
template_version: "1.17"
---
<!-- 
rating: ⭐️⭐️⭐️    // 1 to 3 stars
date: 2023             // when started reading
read: 2023             // when finished reading
status: undefined, backlog, to read, reading, completed, stopped
*** See "Template Help" below for using properties ***
-->

![cover|150]({{coverUrl}})

# <% tp.file.title %>

by [[{{author}}]]

<!-- No more than a couple paragraphs summarizing this BOOK -->

> [!summary]
{{description}}

## Table of Contents
<!--Link to table of contents (TOC) -->
- 

## Notes
<!-- The main content of my thoughts really -->
- 


## Quotes
<!-- Notable quotes with reference to their page or location -->

## Bibliography

> `= this.bibliography`

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
