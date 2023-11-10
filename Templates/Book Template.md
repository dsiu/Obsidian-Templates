---
tags: type/book
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
created_at: {{DATE:YYYY-MM-DDTHH:mm:ss}}
modified_at: {{DATE:YYYY-MM-DDTHH:mm:ss}}
template-type: Book
template-version: "1.11"
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

## Summary
<!-- No more than a couple paragraphs summarizing this BOOK -->

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

## Source
<!-- Always keep a link to the source- --> 
-  

## Tasks
<!-- What remains to be done with this note? --> 
- 

## Questions
<!-- What remains for you to consider? -->
- 

## References
<!-- Links to pages not referenced in the content -->
- 
