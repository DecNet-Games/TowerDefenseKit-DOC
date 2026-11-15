---
layout: default
title: Home
nav_order: 1
---

# A complete tower-defense game in a box.

![Tower Defense Complete Kit]({{ site.baseurl }}/assets/images/cover.png)

Assembling a tower-defense game the usual way means a grid system from one place, a wave spawner from another, an economy bolted on last — and weeks spent making them agree. The **Tower Defense Complete Kit** is the whole game in one box: grid and paths, towers, economy, campaign and meta systems, playable out of the box.

Two systems make it unlike any standalone kit: its maps **generate from a seed**, and its encounters are **directed** — shaped by a difficulty curve and composed to a budget, with playtest telemetry to prove the pacing.

---

## What it does

- **Grid & path logic** — buildable, blocked and path cells; one or more enemy paths from entry to exit; placement rules enforced (never on the path, never blocking the only route). Grids and paths are data.
- **Towers, targeting, upgrades** — tower types with range, damage, fire rate and cost; targeting modes (first, last, strongest, weakest, closest); upgrade paths with exact stated stat changes; sell/refund with a documented refund fraction. Towers are data files, not code.
- **An exact economy** — currency from kills and wave completion, guarded spending, a lives system, zero rounding drift. Proven winnable and losable by scripted runs in the verification record.
- **Maps that generate** — a seeded generation core produces the grid, paths and cells from a seed; the same seed gives the same map on every machine. Hand-authored maps are fully supported alongside.
- **Waves that are directed** — a built-in encounter director: difficulty curves, budget-fitted wave composition, deterministic waves, per-wave telemetry.
- **A campaign with meta** — a campaign of maps with progression unlocks, difficulty steps, and persistent upgrades and unlocks between runs, preserved through save and load.
- **One locked art set** — towers, enemies, maps and interface in one coherent stylised set, and everything reskinnable without touching behaviour.

![Layered defense, generated map]({{ site.baseurl }}/assets/images/hero-01.png)

---

## The honesty policy

This site's claims are the verification record's claims — scripted runs, recorded hashes, counted content — and the winnable/losable claim is a pair of scripted runs, not a feeling. The kit's art is one locked set judged against a fixed benchmark before listing; what the kit does not do is in [Limitations]({{ site.baseurl }}/docs/limitations/).

---

## Quick links

- [Getting Started]({{ site.baseurl }}/docs/getting-started/) — core concepts in five minutes
- [Installation]({{ site.baseurl }}/docs/installation/) — Asset Store purchase and setup
- [Quick Start]({{ site.baseurl }}/docs/quick-start/) — generate a map, place a tower, survive a directed wave
- [Features]({{ site.baseurl }}/docs/features/) — deep dives on every system
- [API Reference]({{ site.baseurl }}/docs/api/) — data formats and integration contracts
- [The Campaign & Sample Game]({{ site.baseurl }}/docs/samples/)
- [FAQ]({{ site.baseurl }}/docs/faq/)
- [Limitations]({{ site.baseurl }}/docs/limitations/)

---

*Tower Defense Complete Kit is a commercial Unity product by DecNet Games. Verified on Unity 2022.3 LTS and Unity 6. Support: support@decnetgames.com.*
