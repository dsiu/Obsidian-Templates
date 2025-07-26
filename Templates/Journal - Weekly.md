---
tags:
  - type/structure
  - structure/journal
aliases:
created: {{monday:YYYY-MM-DDTHH:mm:ssZ}}
modified: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
template_type: Journal Weekly
template_version: "1.4"
---
# <% tp.file.title %>
## Summary

-  [[{{monday:gggg-MM-DD}}|Mon | {{monday:gggg-MM-DD}}]] ![[{{monday:gggg-MM-DD}}#{{monday:gggg-MM-DD}}]]
-  [[{{tuesday:gggg-MM-DD}}|Tue | {{tuesday:gggg-MM-DD}}]] ![[{{tuesday:gggg-MM-DD}}#{{tuesday:gggg-MM-DD}}]]
-  [[{{wednesday:gggg-MM-DD}}|Wed | {{wednesday:gggg-MM-DD}}]] ![[{{wednesday:gggg-MM-DD}}#{{wednesday:gggg-MM-DD}}]]
-  [[{{thursday:gggg-MM-DD}}|Thu | {{thursday:gggg-MM-DD}}]] ![[{{thursday:gggg-MM-DD}}#{{thursday:gggg-MM-DD}}]]
-  [[{{friday:gggg-MM-DD}}|Fri | {{friday:gggg-MM-DD}}]] ![[{{friday:gggg-MM-DD}}#{{friday:gggg-MM-DD}}]]
-  [[{{saturday:gggg-MM-DD}}|Sat | {{saturday:gggg-MM-DD}}]] ![[{{saturday:gggg-MM-DD}}#{{saturday:gggg-MM-DD}}]]
-  [[{{sunday:gggg-MM-DD}}|Sun | {{sunday:gggg-MM-DD}}]] ![[{{sunday:gggg-MM-DD}}#{{sunday:gggg-MM-DD}}]]

--- 
# Back Matter

**Notes created this week**
```dataview
LIST rows.file.link
FROM -"0_Journal"
WHERE created.year = number(substring(this.file.name,0,4)) AND created.weekyear =  number(substring(this.file.name,6,8))
FLATTEN dateformat(striptime(created), "ccc | yyyy-MM-dd") as G
GROUP BY G
SORT default(((x) => {
	"Mon":1,
	"Tue":2,
	"Wed":3,
	"Thu":4,
	"Fri":5,
	"Sat":6,
	"Sun":7
}[split(x," | ")[0]])(G), "99" ) ASC
```

**Notes modified this week**
```dataview
LIST rows.file.link
FROM -"0_Journal"
WHERE modified.year = number(substring(this.file.name,0,4)) AND modified.weekyear =  number(substring(this.file.name,6,8))
FLATTEN dateformat(striptime(modified), "ccc | yyyy-MM-dd") as G
GROUP BY G
SORT default(((x) => {
	"Mon":1,
	"Tue":2,
	"Wed":3,
	"Thu":4,
	"Fri":5,
	"Sat":6,
	"Sun":7
}[split(x," | ")[0]])(G), "99" ) ASC
```

