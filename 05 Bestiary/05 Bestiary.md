---
tags:
  - hub
---

> [!lore] Everything in the house with initiative.
> Statblocks pull from Fantasy Statblocks. Run **Fantasy Statblocks: Import SRD bestiary**
> once from the command palette if they render blank.

```dataview
TABLE WITHOUT ID
  file.link AS "Creature",
  appears_in AS "Appears In",
  count AS "How Many"
FROM "05 Bestiary"
WHERE file.name != "05 Bestiary"
SORT file.name ASC
```

---

## Named

- [[Lorghoth the Decayer]]

## Undead

- [[Ghast]] · [[Ghoul]] · [[Shadow]] · [[Specter]]

## Constructs & Ambushers

- [[Animated Armor]] · [[Broom of Animated Attack]] · [[Mimic]]

## Vermin & Vermin-Adjacent

- [[Grick]] · [[Nothic]] · [[Swarm of Bats]] · [[Swarm of Insects]] · [[Swarm of Rats]]

## People

- [[Cultist]]

---

> [!check] Before the session
> Fill `appears_in` and `count` on each page. Then [[Initiative & Combat]] is a two-minute job.

---
[[00 START HERE|← Dashboard]]
