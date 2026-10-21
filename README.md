# IntrovertVillagers

> Make villagers introverted (silent)

A Minecraft Java Edition resource pack that fully mutes all villager sounds — idle mumbles, hurt noises, trade jingles, death screams, everything. They still function normally, they just shut up.

---

## What it silences

| Sound Event | Description |
|---|---|
| `entity.villager.ambient` | Idle mumbling |
| `entity.villager.hurt` | Damage sounds |
| `entity.villager.death` | Death sound |
| `entity.villager.trade` | Trade accepted |
| `entity.villager.yes` | Villager agrees |
| `entity.villager.no` | Villager disagrees |
| `entity.villager.celebrate` | Raid celebration |

---

## Installation

1. Download the `.zip`
2. Place it in `.minecraft/resourcepacks/`
3. Launch Minecraft → **Options → Resource Packs**
4. Move **IntrovertVillagers** to the active side
5. Click **Done**

---

## Compatibility

- **Java Edition 26.3** (Wilderness Bound) and up
- `pack_format: 46` with open `max_inclusive: 255` — should work across future versions without changes

---

## How it works

`sounds.json` overrides every villager sound event with Minecraft's built-in `silent` sound using `"replace": true`, which wipes the vanilla pool entirely.

```json
{
  "entity.villager.ambient": {
    "sounds": [ { "name": "silent", "volume": 1.0, "pitch": 1.0 } ],
    "replace": true
  },
  ...
}
```

---

## Pack meta

```json
{
  "pack": {
    "pack_format": 46,
    "supported_formats": {
      "min_inclusive": 46,
      "max_inclusive": 255
    },
    "description": "§e• Make villagers introverted\n§6• by Modder Brothers N"
  }
}
```

---

*by Modder Brothers N*
