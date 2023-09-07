---
tags:
  - discord
  - toc
---
```dataviewjs
let pages = dv.pages("#sample");
for (let p of pages) { // Loop through pages 
	//dv.el("h2",p.file.name) 
	dv.el("article", await dv.io.load(p.file.path))
} 
```
