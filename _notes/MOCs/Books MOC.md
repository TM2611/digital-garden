---
---

tags:: #MOC
up:: [[Cerebellum 🧠]]

## List of all books

```dataview
TABLE WITHOUT ID
	"![|60](" + coverUrl + ")" as Cover,
	link(file.link, title) as Title,
	author as Author,
	join(list(publisher, publish)) as Publisher
FROM [[Books MOC]] AND #book
WHERE !contains(file.path, "Templates")
SORT status DESC, file.ctime ASC
```