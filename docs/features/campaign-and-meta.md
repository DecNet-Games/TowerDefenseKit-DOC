---
layout: default
title: Campaign & Meta
parent: Features
nav_order: 6
---

# Campaign & Meta

The reason to keep playing — and the leg that makes this a complete game rather than a single-map toy.

- **A campaign of maps**, playable end-to-end: clear each map in order, unlock the next, reach the campaign's end — asserted by a scripted playthrough on both versions.
- **Progression is enforced.** A locked map cannot be entered before its predecessor is cleared; clearing a map unlocks exactly the next one.
- **Difficulty steps across the campaign** — each map's difficulty, enemy roster and generation parameters are recorded in the verification record, and a comparison test asserts the maps' wave compositions genuinely differ.
- **Meta persists.** Tower unlocks and permanent upgrades earned in one run are present in the next, and save/load preserves them — state hash before save equals state hash after load, across a set of save points.
- **Winnable and losable.** The record holds a scripted winning campaign run and a scripted losing run.

The campaign map screen shows the actual campaign state: locked maps display locked, cleared maps display cleared — asserted against the runtime state, not drawn independently.
