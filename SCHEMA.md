# Data Schema

## `data/planets.json`

| Field | Type | Description |
|-------|------|-------------|
| `id` | string | Unique UUID |
| `name` | string | Official planet name |
| `region` | string | Galactic region |
| `sector` | string | Sector name |
| `grid` | string | Grid square (ex: `M-10`) |
| `galactic_x` | number | X coordinate in parsecs from Coruscant |
| `galactic_y` | number | Y coordinate in parsecs from Coruscant |
| `galactic_z` | number | Z coordinate in parsecs from Coruscant |
| `suns` | number | Number of suns |
| `moons` | number | Number of moons |
| `diameter` | number | Diameter in km |
| `climate` | string | Climate description |
| `terrain` | string | Terrain type |
| `atmosphere` | string | Atmosphere classification |
| `style` | string | Visual type (see values below) |

> Fields with no data are omitted rather than set to null.

---

## Galactic regions

`Deep Core` · `Core Worlds` · `Colonies` · `Inner Rim` · `Expansion Region` · `Mid Rim` · `Outer Rim Territories` · `Wild Space` · `Unknown Regions` · `Hutt Space` · `Corporate Sector` · `Chiss Space`

## Planet style values

`desert` · `ice` · `lava` · `ocean` · `forest` · `city` · `gas` · `barren` · `temperate` · `swamp` · `rocky` · `tropical` · `crystal`
