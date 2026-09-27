---
floor: Dungeon Level
tags:
  - floor
  - map
---

> [!lore] Areas 22–38. Not part of the house — it does not repair itself.
> Click a pin to open that area. Pins are draggable — nudge any that sit wrong and Leaflet remembers.

```leaflet
id: dh-dungeon
image: [[Death House - Dungeon Level.webp]]
height: 680px
width: 100%
lat: 55
long: 48
minZoom: -2
maxZoom: 6
defaultZoom: 0.5
zoomDelta: 0.5
marker: default,89,57,[[22 Dungeon Level Access]],22 — Dungeon Level Access
marker: default,83,76,[[23 Family Crypts]],23 — Family Crypts
marker: default,92,42,[[24 Cult Initiates' Quarters]],24 — Cult Initiates' Quarters
marker: default,78,23,[[25 Well and Cultist Quarters]],25 — Well and Cultist Quarters
marker: default,67,35,[[26 Hidden Spiked Pit]],26 — Hidden Spiked Pit
marker: default,72,61,[[27 Dining Hall]],27 — Dining Hall
marker: default,73,72,[[28 Larder]],28 — Larder
marker: default,64,60,[[29 Ghoulish Encounter]],29 — Ghoulish Encounter
marker: default,40,10,[[30 Stairs Down]],30 — Stairs Down
marker: default,48,79,[[31 Darklord's Shrine]],31 — Darklord's Shrine
marker: default,60,75,[[32 Hidden Trapdoor]],32 — Hidden Trapdoor
marker: default,46,63,[[33 Cult Leaders' Den]],33 — Cult Leaders' Den
marker: default,46,46,[[34 Cult Leaders' Quarters]],34 — Cult Leaders' Quarters
marker: default,36,25,[[35 Reliquary]],35 — Reliquary
marker: default,18,23,[[36 Prison]],36 — Prison
marker: default,28,36,[[37 Portcullis]],37 — Portcullis
marker: default,18,42,[[38 Ritual Chamber]],38 — Ritual Chamber
```

> [!lore]- Lights out — same floor, no lamps lit
> ![[Death House - Dungeon Level (Dark).webp]]

## Prep Tracker

```dataview
TABLE WITHOUT ID
  "**" + area + "**" AS "#",
  link(file.link, room) AS "Area",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE floor = "Dungeon Level"
SORT area ASC
```

## Floor Notes

-

---
[[Death House (Map Hub)|↑ Map Hub]]  ·  [[Exterior]]  ·  [[First Floor]]  ·  [[Second Floor]]  ·  [[Third Floor]]  ·  [[Attic]]  ·  **Dungeon Level**
