---
layout: default
title: Generated Maps
parent: Features
nav_order: 4
---

# Generated Maps

Maps that generate, on a seeded generation core — the differentiator no standalone tower-defense kit ships.

- **Deterministic.** The same seed produces the same map (grid, paths, difficulty parameters) on both Unity versions, asserted across a fixed seed set by map hashes.
- **Always valid.** Every generated map satisfies the grid rules: a valid connected path, placement rules intact — the grid test set re-run against the generated set, zero failures.
- **Measurably varied.** Across the seed set, path shapes and buildable-cell layouts are not copies of one another — asserted by a comparison test over path hashes.
- **Parameters are data.** Map size and path complexity change in data files only; the generated maps follow, with no code change.
- **Shareable.** A map is a seed: send the seed, and the other side generates your exact map. Hand-authored maps remain fully supported for hand-tuned campaign entries.

The generation core inside this kit is a shipped, versioned core — recorded in the verification record, not a private fork.

![A seeded canyon map]({{ site.baseurl }}/assets/images/hero-02.png)
