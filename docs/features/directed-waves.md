---
layout: default
title: Directed Waves
parent: Features
nav_order: 5
---

# Directed Waves

Waves in this kit are not hand-written tables. A built-in encounter director runs them:

- **A difficulty curve** shapes how hard the game gets across the campaign.
- **A budget composes each wave.** Every composed wave's total enemy cost fits its budget with the documented minimum utilisation — asserted across a fixed wave set on both versions.
- **Waves are deterministic.** Given (curve, wave index, seed), replaying reproduces the same wave-composition hash.
- **The director drives real waves.** In a scripted run, waves start on the director's schedule, spawn points receive exactly the composed wave, and the wave-end event fires when the wave clears.
- **Telemetry is recorded per wave.** A scripted playtest produces a complete per-wave record, saved as an artifact — so the campaign's pacing is something you can inspect, not guess.

The director inside this kit is a shipped, versioned system — recorded in the verification record, not a private fork.
