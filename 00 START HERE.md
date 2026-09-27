---
tags:
  - dashboard
cssclasses:
  - dh-dropcap
---

# Death House

A Halloween one-shot for five characters, levels 1–3. Two young ghosts point at a
tall brick row house and tell you there's a monster inside. There is. It isn't the
one they mean.

---

## At the Table

<div class="dh-grid">

- [[Run Sheet]]
- [[Death House (Map Hub)]]
- [[Initiative & Combat]]
- [[Party Overview]]
- [[Session Notes]]
- [[Rules Quick Reference]]

</div>

## Before the Table

<div class="dh-grid">

- [[Session Prep Checklist]]
- [[Atmosphere & Pacing]]
- [[04 NPCs]]
- [[05 Bestiary]]

</div>

---

## The House, Level by Level

<div class="dh-grid">

- [[Exterior]]
- [[First Floor]]
- [[Second Floor]]
- [[Third Floor]]
- [[Attic]]
- [[Dungeon Level]]

</div>

---

## Prep Progress

How much of the house still has empty notes.

```dataview
TABLE WITHOUT ID
  floor AS "Level",
  length(rows) AS "Areas",
  length(filter(rows, (r) => r.status != "unexplored")) AS "Touched"
FROM "02 The House/Rooms"
GROUP BY floor
```

## Rooms Flagged for Attention

Set a room's `status` to anything other than `unexplored` and it shows up here.

```dataview
TABLE WITHOUT ID
  link(file.link, room) AS "Area",
  floor AS "Level",
  status AS "Status"
FROM "02 The House/Rooms"
WHERE status != "unexplored"
SORT area ASC
```

---

## Cast

```dataview
TABLE WITHOUT ID
  file.link AS "Who",
  role AS "Role",
  location AS "Found"
FROM "04 NPCs"
SORT file.name ASC
```

---

> [!secret]- Setup — read this once, then delete it
> Everything below is already done unless noted.
>
> **Plugins** are pre-installed and pre-enabled: Leaflet, Dataview, Initiative Tracker,
> Dice Roller, Fantasy Statblocks, Admonitions, Templater. On first launch Obsidian will
> ask you to trust the vault — choose **Trust author and enable plugins**. If anything
> looks like raw code instead of a map or table, that's the only thing that went wrong.
>
> **Theme** is a CSS snippet, already enabled: *Settings → Appearance → CSS snippets → death-house*.
>
> **One manual step:** open the command palette and run
> **Fantasy Statblocks: Import SRD bestiary** so the [[05 Bestiary]] statblocks render.
>
> **Custom callouts** available to you anywhere:
> `> [!read-aloud]` · `> [!secret]` · `> [!trap]` · `> [!treasure]` · `> [!creature]` · `> [!lore]` · `> [!check]`
> Add a `-` after the type (`[!lore]-`) to make it start collapsed.
>
> **Dice** work inline: `` `dice: 1d20+3` `` renders a clickable roll.
