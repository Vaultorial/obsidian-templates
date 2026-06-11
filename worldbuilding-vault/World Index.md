---
type: index
---

# World Index — The Tide Courts

The Shallow Sea drains and returns twice a day, and twice a year the king tides redraw the coast itself. Around its bay stand the Tide Courts: city-states whose law is not about land but about *when* land exists. Tide-law decides who may build, farm and harvest on ground that floods — and tide-law is only as good as the charts it stands on. The charts are drifting. This index is the front door to everything.

## The present situation, in three sentences

The Ebb Court in [[Ostreve]] upholds the old charts, which schedule [[The Drowning of Lowmark]] for this midsummer. The Floodsworn of [[Lowmark]] mean to stop it, by petition or by breaking the dikes. And the Order of the Drowned Bell, whose measurements make the law possible, has quietly discovered that the measurements no longer agree with the sea — see [[The Mirrormoor Blight]].

## Places

- [[Ostreve]] — cliff city, seat of the Ebb Court, keeper of charts and tolls.
- [[Lowmark]] — the port below: stilts, fish-smoke, and the ward scheduled to drown.
- [[The Causeway of Bells]] — the only road between them, passable at low water.
- [[The Mirrormoor]] — tidal flats and pearl-moss beds; wealth you must outrun the sea to harvest.
- [[Hethwick]] — upland market town beyond tide-law; everyone's neutral ground.
- [[The Drowned Abbey]] — half-sunk archive of the Order, reachable on foot only at neap tide.

## Factions

- [[The Ebb Court]] — the law. Seat: Ostreve. Led by Tidemistress [[Elowen Hark]].
- [[The Floodsworn]] — the protest. Seat: Lowmark. Led by [[Bren Callow]].
- [[Order of the Drowned Bell]] — the measurers. Seat: the Drowned Abbey. Led by [[Maud Pell]].

## People

```dataview
TABLE role, home, faction
FROM "Characters"
SORT file.name ASC
```

### By faction

```dataview
TABLE rows.file.link AS "Members", rows.role AS "Role"
FROM "Characters"
GROUP BY faction
```

## Chronology

The full narrated version lives in [[Timeline]].

```dataview
TABLE year, location, status
FROM "Events"
SORT year ASC
```

## Threads to pull

- Will [[Verity Ostreve]]'s secret accord with [[Bren Callow]] hold when the sluice vote comes?
- What happens to tide-law when [[Maud Pell]] publishes that the charts are wrong?
- [[Wick the Ferryman]] has carried every secret in this index at least once. Who does he finally tell?
