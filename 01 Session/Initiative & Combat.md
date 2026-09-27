---
tags:
  - session
  - combat
---

> [!lore] Encounters staged ahead of time, so you never build one mid-fight.
> Click **Launch Encounter** on any block below to push it straight into the Initiative Tracker.

## Party

Add your five characters once, in the Initiative Tracker's settings
(**Settings → Initiative Tracker → Players**). They'll be available to every encounter.

---

## Staged Encounters

Copy the block, rename it, change the creatures. Format is `count: Creature Name`.

```encounter
name: Example — rename me
party: The Party
creatures:
 - 2: Specter
 - 1: Animated Armor
```

### 

```encounter
name: 
creatures:
 - 
```

### 

```encounter
name: 
creatures:
 - 
```

### 

```encounter
name: 
creatures:
 - 
```

---

## Quick Rolls

| | |
|---|---|
| Initiative | `dice: 1d20` |
| Perception (passive check) | see [[Party Overview]] |
| Damage, generic | `dice: 1d6` |
| Wild swing | `dice: 1d20+4` |

---

## Combat Reminders

- **Surprise:** only if *nobody* in the group noticed the threat
- **Held actions** trigger before the triggering creature finishes its turn
- **Two death saves failed?** Say it out loud. Tension is the point.
- **Round timer:** if a player takes more than 30 seconds, they Dodge

---
[[00 START HERE|← Dashboard]]
