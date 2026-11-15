---
layout: default
title: Grid & Paths
parent: Features
nav_order: 1
---

# Grid & Paths

The board the game is played on: a build grid of placeable, blocked and path cells; one or more enemy paths from entry to exit per map; pathfinding along the path; and placement rules that keep the game honest.

## Guarantees (asserted across the shipped and generated map sets)

- **Every map has a valid path.** At least one connected route from entry to exit, no dead ends — on shipped maps and across a generated-map set alike.
- **Placement rules hold.** A tower cannot be placed on a path cell, a blocked cell or an occupied cell — and a placement that would block the only remaining path is refused with a clear reason.
- **Pathfinding is deterministic.** The same map and entry produce the same enemy route on both Unity versions, asserted by route hashes across a fixed map set.
- **Maps are data.** Add a test map as a data file only — no code change — and it plays. Malformed map data (no entry, no exit, a disconnected path, a path through a blocked cell) is reported naming the map.
- **Multi-path maps stay independent.** Where a map ships with more than one path, enemies on path A never route onto path B.
