---
aliases:
  - High Council
location: "[[Asteri District]]"
status: inactive
lore_type: faction
icon: faction
---
## Information
> [!infobox]
> # `=this.file.name`
> ![[insertimage.png|cover hsmall]]
> ###### Information
> |   |  |
> | ---- | ---- |
> | Aliases | `=this.aliases`|
> | Status| `=this.status`|
> | Based in|  `=this.location`|
##### Known for: handling all political matters of the[[Kingdom of United Kippian]]
### Description
##### High Council Seating
Drakon-Aetos-Chtapodhi-Foenyx-King of Kippian-Ankyra-Yvernus-Duospathia-Lykos

## Organization
##### Leader: [[Riordan Kyp|King Riordan]]
### Known Members
```dataview
TABLE WITHOUT ID
  file.link as Name
FROM "NPCs" or "PCs"
WHERE faction = this.file.link
```
## Goals
- [ ] Task 1
## Story log
### Most Recent
```dataview
LIST bullets.text
FROM "Session Log"
FLATTEN file.lists as bullets
WHERE contains(bullets.text, this.file.name)
SORT number(file.name) desc, reverse(bullets) desc
LIMIT 10
SORT number(file.name) asc, reverse(bullets) asc
```
### All Entries
```dataview
LIST bullets.text
FROM "Session Log"
FLATTEN file.lists as bullets
WHERE contains(bullets.text, this.file.name)
SORT number(file.name) asc
```