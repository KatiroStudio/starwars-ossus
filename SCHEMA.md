# Data Schema

## `data/planets.json`

| Field | Type | Description |
|-------|------|-------------|
| `id` | string | Unique UUID |
| `name` | string | Official planet name |
| `region` | string | Galactic region (see regions below) |
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
| `type` | string | Planet style (see types below) |
| `canonicity` | string | Canon status (see values below) |
| `appearances` | array | List of media appearances |
| `description_fr` | string | Description in French |

> Fields with no data are omitted (not set to null).

---

## Galactic regions

`Deep Core` · `Core Worlds` · `Colonies` · `Inner Rim` · `Expansion Region` · `Mid Rim` · `Outer Rim Territories` · `Wild Space` · `Unknown Regions` · `Hutt Space` · `Corporate Sector` · `Chiss Space`

## Planet types

`desert` · `ice` · `lava` · `ocean` · `forest` · `city` · `gas` · `barren` · `temperate` · `swamp` · `rocky` · `tropical` · `crystal`

## Canonicity values

| Value | Meaning |
|-------|---------|
| `canon` | Disney-era canon only |
| `legends` | Legends / pre-Disney only |
| `canon_and_legends` | Appears in both |

## Appearances object

```json
{
  "title": "A New Hope",
  "type": "film",
  "year": 1977
}
```

| Field | Values |
|-------|--------|
| `type` | `film` · `serie` · `roman` · `comic` · `anime` · `jeu` |
