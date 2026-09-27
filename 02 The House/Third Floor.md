---
floor: Third Floor
tags:
  - floor
  - map
---

> [!lore] Areas 11–15. Dust starts here. Two balconies, one nursemaid.
> Click a pin to open that area. Pins are draggable — nudge any that sit wrong and Leaflet remembers.

```leaflet
id: dh-third-floor
image: [[Death House - Third Floor.webp]]
height: 680px
width: 100%
lat: 68
long: 48
minZoom: -2
maxZoom: 6
defaultZoom: 1.5
zoomDelta: 0.5
marker: default,68,51,[[11 Balcony]],11 — Balcony
marker: default,82,47,[[12 Master Suite]],12 — Master Suite
marker: default,69,42,[[13 Bathroom]],13 — Bathroom
marker: default,62,42,[[14 Storage Room]],14 — Storage Room
marker: default,56,53,[[15 Nursemaid's Suite]],15 — Nursemaid's Suite
```

> [!lore]- Lights out — same floor, no lamps lit
> ![[Death House - Third Floor (Dark).webp]]

## Prep Tracker

```dataview
TABLE WITHOUT ID
  "**" + area + "**" AS "#",
  link(file.link, room) AS "Area",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE floor = "Third Floor"
SORT area ASC
```

## Floor Notes

-

---
[[Death House (Map Hub)|↑ Map Hub]]  ·  [[Exterior]]  ·  [[First Floor]]  ·  [[Second Floor]]  ·  **Third Floor**  ·  [[Attic]]  ·  [[Dungeon Level]]
