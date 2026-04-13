# ✦ Starwars Ossus

> *"The great library of Ossus once held the accumulated knowledge of a thousand generations of Jedi."*

**Ossus** is an open dataset of Star Wars planets, timeline events and media appearances — built as the data backbone of the **Star Wars Space & Time** project.

This repository follows the spirit of its namesake: the ancient Jedi library planet, the greatest repository of galactic knowledge ever assembled.

---

## 📦 Contents

| File | Description |
|------|-------------|
| `data/planets.json` | 1,361 planets with coordinates, regions, physical data & appearances |
| `data/events.json` | Timeline events *(coming soon)* |
| `SCHEMA.md` | Full field descriptions and data types |
| `CONTRIBUTING.md` | How to suggest corrections or additions |

---

## 🌌 Planet data sample

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
  "type": "desert",
  "canonicity": "canon",
  "appearances": [
    { "title": "A New Hope", "type": "film", "year": 1977 }
  ]
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
- [Star Wars Galaxy Map](https://www.starwars.com/star-wars-galaxy-map) — the official interactive map, from which planet positions were extracted using OCR and coordinate triangulation. Results are approximately accurate. The galaxy is big, we did our best.

Community corrections welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).
