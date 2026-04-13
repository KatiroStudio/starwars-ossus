# ✦ Star Wars Ossus

> *"The great library of Ossus once held the accumulated knowledge of a thousand generations of Jedi."*

**Ossus** is an open dataset of Star Wars planets — built as the data backbone of the **Star Wars Space & Time** project.

This repository follows the spirit of its namesake: the ancient Jedi library planet, the greatest repository of galactic knowledge ever assembled.

---

## 👋 Why this exists

I'm a Star Wars fan who wanted to build something precise — a complete, structured database of planets and timeline events. When I started looking, I couldn't find anything complete enough to work with. So I built it myself.

This is fan work, done with care. If you're also obsessed with getting the details right, contributions are welcome.

---

## 📦 Contents

| File | Description |
|------|-------------|
| `data/planets.json` | 1,361 canon planets with coordinates, regions and physical data |
| `data/events.json` | Timeline events *(coming soon)* |
| `SCHEMA.md` | Full field descriptions and data types |
| `CONTRIBUTING.md` | How to suggest corrections or additions |

---

## 🌌 Understanding the Star Wars galaxy

### Coruscant is the center of everything

In Star Wars lore, **Coruscant** — the galaxy's capital planet — serves as the origin point of the galactic coordinate system. Its position is `galactic_x: 0, galactic_y: 0`. All other planet coordinates are expressed in **parsecs** relative to Coruscant.

So if a planet has `galactic_x: 243, galactic_y: -327`, it means it is located 243 parsecs to the right and 327 parsecs below Coruscant on the standard galactic map.

> Coordinates in this dataset were extracted from the [official Star Wars Galaxy Map](https://www.starwars.com/star-wars-galaxy-map) using OCR and coordinate triangulation. They are approximately accurate. The galaxy is big — we did our best.

---

### The grid system

The galaxy is divided into a **grid of named squares**, each identified by a letter (column) and a number (row) — for example `M-10` or `R-16`.

- **Columns** go from `A` (far left) to `S` (far right) — roughly west to east
- **Rows** go from `1` (top) to `27` (bottom) — roughly north to south
- **Coruscant** sits at approximately `L-9`, near the galactic center

The grid is a navigational convention used by pilots, cartographers and the Imperial Navy alike. It appears on the official Star Wars Galaxy Map and in many in-universe documents.

---

### Galactic regions

The galaxy is divided into concentric regions, from the dense core to the wild fringes:

| Region | Description |
|--------|-------------|
| **Deep Core** | The innermost, densely packed star systems. Dangerous to navigate, home to ancient secrets. |
| **Core Worlds** | The political and cultural heart of the galaxy. Birthplace of the Republic and the Empire. Includes Coruscant, Alderaan, Corellia. |
| **Colonies** | The first worlds colonized beyond the Core. Wealthy and heavily populated. |
| **Inner Rim** | A prosperous ring of established worlds, just beyond the Colonies. |
| **Expansion Region** | Heavily industrialized and exploited territories, rich in resources. |
| **Mid Rim** | A vast, diverse band of worlds — from thriving trade hubs to quiet backwaters. |
| **Outer Rim Territories** | The frontier. Most of the galaxy's area, sparsely populated, poorly mapped. Home to Tatooine, Mandalore, and many iconic planets. |
| **Wild Space** | Beyond the Outer Rim. Largely uncharted, dangerous, and full of mysteries. |
| **Unknown Regions** | The far edge of the galaxy. Virtually unexplored. Home of the First Order's origins and ancient threats. |
| **Hutt Space** | A semi-independent region controlled by the Hutt crime syndicates. |
| **Corporate Sector** | A vast region once ceded to private corporations by the Empire. |
| **Chiss Space** | Home of the Chiss Ascendancy, in the Unknown Regions. |

---

## 🌍 Planet data sample

```json
{
  "id": "550e8400-e29b-41d4-a716-446655440000",
  "name": "Tatooine",
  "region": "Outer Rim Territories",
  "sector": "Arkanis sector",
  "grid": "R-16",
  "galactic_x": 243.0,
  "galactic_y": -327.5,
  "suns": 2,
  "moons": 3,
  "diameter": 10465,
  "climate": "Arid",
  "terrain": "Desert",
  "style": "desert"
}
```

---

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) — corrections and additions are welcome via Pull Request or Issue.

---

## ⚠️ Disclaimer

Fan-made project. Star Wars and all related properties are trademarks of Lucasfilm Ltd. / Disney.

**Data sources:**
- [Wookieepedia](https://starwars.fandom.com) — the galaxy's most reliable encyclopedia
- [Star Wars Galaxy Map](https://www.starwars.com/star-wars-galaxy-map) — the official interactive map, from which planet positions were extracted using OCR and coordinate triangulation

Community corrections welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).
