---
floor: First Floor
tags:
  - floor
  - map
---

> [!lore] Areas 1–5. Entrance, main hall, and the rooms the house keeps clean.
> Click a pin to open that area. Pins are draggable — nudge any that sit wrong and Leaflet remembers.

```leaflet
id: dh-first-floor
image: [[Death House - First Floor.webp]]
height: 680px
width: 100%
lat: 66
long: 50
minZoom: -2
maxZoom: 6
defaultZoom: 1.5
zoomDelta: 0.5
marker: default,51,43,[[01 Entrance]],1 — Entrance
marker: default,69,48,[[02 Main Hall]],2 — Main Hall
marker: default,58,57,[[03 Den of Wolves]],3 — Den of Wolves
marker: default,80,59,[[04 Kitchen and Pantry]],4 — Kitchen and Pantry
marker: default,82,45,[[05 Dining Room]],5 — Dining Room
```

> [!lore]- Lights out — same floor, no lamps lit
> ![[Death House - First Floor (Dark).webp]]

## Prep Tracker

```dataview
TABLE WITHOUT ID
  "**" + area + "**" AS "#",
  link(file.link, room) AS "Area",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE floor = "First Floor"
SORT area ASC
```

## Floor Notes

-

---
[[Death House (Map Hub)|↑ Map Hub]]  ·  [[Exterior]]  ·  **First Floor**  ·  [[Second Floor]]  ·  [[Third Floor]]  ·  [[Attic]]  ·  [[Dungeon Level]]
