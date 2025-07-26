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
categories: {{categories}}
description:
publisher: {{publisher}}
total_page: {{totalPage}}
cover_url: {{coverUrl}}
cover_small_url: {{coverSmallUrl}}
publish_date: {{publishDate}}
isbn: {{isbn10}} {{isbn13}}
link: {{link}}
preview_link: {{preview_link}}
bibliography: +++ Copy and paste citation from Zotero +++
rating:
date:
read:
status: undefined
created: {{DATE:YYYY-MM-DDTHH:mm:ss}}
modified: {{DATE:YYYY-MM-DDTHH:mm:ss}}
template_type: Book
template_version: "1.21"
---
<!-- 
rating: ⭐️⭐️⭐️    // 1 to 3 stars
date: 2023             // when started reading
read: 2023             // when finished reading
status: undefined, backlog, to read, reading, completed, stopped
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
