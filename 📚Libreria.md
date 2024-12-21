---
cssclasses:
  - cards
---

## In Lettura
```dataview
table ("![](" + cover +")") as Copertina, title as "Titolo",  author as "Autore", start as "Data Inizio", finished as "Data Fine"
from "5. Libreria/NuovaLibreria/Libri"
where status = "reading"
```



## Letti
```dataview
table ("![](" + cover +")") as Copertina, title as "Titolo",  author as "Autore"
from "5. Libreria/NuovaLibreria/Libri"
where status = "read"
```


## Da leggere
```dataview
table ("![|100](" + cover + ")") as Copertina, title as "Titolo",  author as "Autore", start as "Data Inizio", finished as "Data Fine"
from "5. Libreria/NuovaLibreria/Libri"
where status = "unread"
```


## Incompleti
```dataview
table ("![|100](" + cover + ")") as Copertina, title as "Titolo",  author as "Autore", start as "Data Inizio", finished as "Data Fine"
from "5. Libreria/NuovaLibreria/Libri"
where status = "incomplete"
```