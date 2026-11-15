---
layout: default
title: Towers & Upgrades
parent: Features
nav_order: 2
---

# Towers & Upgrades

The verbs of the game — data-driven, so a new tower type is a file, not a code change.

- **Tower types** — damage, slow, splash, sniper and support families, each with range, damage, fire rate and cost. Every shipped type is proven headless: it fires, it damages, it respects its range, and its fire-rate timing holds within the documented tolerance.
- **Targeting modes** — first, last, strongest, weakest, closest, each behaving per its documented definition (for example, "first" picks the enemy furthest along the path), asserted across a fixed combat set.
- **Upgrades** — per-tower upgrade paths with exact costs and stat changes: upgrading changes the stats by the stated amounts and deducts the stated cost, and a max-level tower refuses further upgrades.
- **Sell / refund** — returns the documented fraction of the invested cost and frees the cell for re-placement.
- **Bad data fails loudly** — negative damage, zero range or an upgrade pointing nowhere is reported naming the tower.
