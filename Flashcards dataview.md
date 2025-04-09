---
tags:
  - flashcards
---

## Dataview list of notes NOT containing "#flashcards"
``` dataview
TABLE file.name as "Note"
FROM ""
WHERE !contains(tags, "flashcards") OR !contains(file.tags, "flashcards")
```


---

## Dataview List of notes that DO contain "#flashcards"
```dataview
TABLE file.name AS "Note"
FROM ""
WHERE contains(file.tags, "flashcards")
```




