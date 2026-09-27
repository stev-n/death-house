---
floor: Second Floor
tags:
  - floor
  - map
---

> [!lore] Areas 6–10. Library, conservatory, and the room behind the bookcase.
> Click a pin to open that area. Pins are draggable — nudge any that sit wrong and Leaflet remembers.

```leaflet
id: dh-second-floor
image: [[Death House - Second Floor.webp]]
height: 680px
width: 100%
lat: 70
long: 50
minZoom: -2
maxZoom: 6
defaultZoom: 1.5
zoomDelta: 0.5
marker: default,69,47,[[06 Upper Hall]],6 — Upper Hall
marker: default,77,59,[[07 Servants' Room]],7 — Servants' Room
marker: default,82,45,[[08 Library]],8 — Library
marker: default,84,60,[[09 Secret Room]],9 — Secret Room
marker: default,58,50,[[10 Conservatory]],10 — Conservatory
```

> [!lore]- Lights out — same floor, no lamps lit
> ![[Death House - Second Floor (Dark).webp]]

## Prep Tracker

```dataview
TABLE WITHOUT ID
  "**" + area + "**" AS "#",
  link(file.link, room) AS "Area",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE floor = "Second Floor"
SORT area ASC
```

## Floor Notes

-

---
[[Death House (Map Hub)|↑ Map Hub]]  ·  [[Exterior]]  ·  [[First Floor]]  ·  **Second Floor**  ·  [[Third Floor]]  ·  [[Attic]]  ·  [[Dungeon Level]]
