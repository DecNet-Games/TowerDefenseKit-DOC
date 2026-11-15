---
layout: default
title: API Reference
nav_order: 6
---

# API Reference

This page covers the kit's public contract: the data formats you author in, and the determinism guarantees you can rely on. The offline API reference inside the package documents every public method signature and matches this site's version.

## Data formats

- **Maps** — grid cells (buildable / blocked / path), entries and exits, one or more paths. Hand-authored as data, or produced by the generator from a seed + generation parameters.
- **Towers** — type, range, damage, fire rate, cost, targeting modes, upgrade chain (per-level costs and stat changes), sell fraction. Validated on load, with errors naming the tower.
- **Economy** — kill rewards, wave-clear bonuses, build/upgrade costs, lives per leaked enemy. Change a value in data and the awarded currency follows.
- **Generation parameters** — map size, path complexity and difficulty parameters for seeded maps.
- **Director configuration** — difficulty curve, enemy costs and composition rules for directed waves.

## Determinism contracts

- **Routes:** same map + entry → same enemy route, both versions (route hashes).
- **Maps:** same seed → same map, both versions (map hashes).
- **Waves:** same (curve, wave index, seed) → same composition, both versions (composition hashes).
- **Saves:** run and meta state round-trip exactly (state hash before save = after load).

## Reuse, recorded honestly

Two components inside this kit are versioned systems in their own right — the seeded generation core and the encounter director. The verification record names the exact core/director versions this kit ships, and if either core changes, the affected acceptance tests are re-run against the new version and the result recorded.
