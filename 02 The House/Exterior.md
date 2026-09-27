---
floor: Exterior
tags:
  - floor
  - map
---

> [!lore] The street, the gate, the portico. Where the mists close in.
> Click a pin to open that area. Pins are draggable — nudge any that sit wrong and Leaflet remembers.

```leaflet
id: dh-exterior
image: [[Death House - Exterior.webp]]
height: 680px
width: 100%
lat: 60
long: 46
minZoom: -2
maxZoom: 6
defaultZoom: 1
zoomDelta: 0.5
marker: default,51,43,[[01 Entrance]],1 — Entrance
```

> [!lore]- Lights out — same floor, no lamps lit
> ![[Death House - Exterior (Dark).webp]]

## Prep Tracker

```dataview
TABLE WITHOUT ID
  "**" + area + "**" AS "#",
  link(file.link, room) AS "Area",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE floor = "Exterior"
SORT area ASC
```

## Floor Notes

-

---
[[Death House (Map Hub)|↑ Map Hub]]  ·  **Exterior**  ·  [[First Floor]]  ·  [[Second Floor]]  ·  [[Third Floor]]  ·  [[Attic]]  ·  [[Dungeon Level]]
