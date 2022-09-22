---
test : test
---

[[글쓰기 테스트]]

![[profile.gif]]


```dataview
TABLE WITHOUT ID file.link AS "최신 글"
WHERE date(today) - file.mtime
WHERE file.name != this.file.name
SORT file.mtime DESC
LIMIT 5
```
