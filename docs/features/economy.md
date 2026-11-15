---
layout: default
title: Economy
parent: Features
nav_order: 3
---

# Economy

The loop that pays for the towers — and the game's second pacing spine, alongside the director.

- **Exact arithmetic.** A scripted run with a fixed kill set awards exactly the documented currency from kills, wave completion and bonus rules — no rounding drift, on either Unity version.
- **Guarded spending.** Building or upgrading without sufficient currency is refused with no state change: no negative balance, no free tower.
- **Lives leak correctly.** Each enemy reaching the exit removes exactly the documented lives; reaching zero ends the run with the lose condition.
- **Rules are data.** Change the kill reward or the wave bonus in a data file only, and the awarded currency changes — no code.
- **Winnable and losable, by evidence.** The verification record holds at least one scripted winning run and one scripted losing run under the frozen economy definitions. A game that cannot lose is not shipped.
