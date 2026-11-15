---
layout: default
title: Getting Started
nav_order: 2
---

# Getting Started

Three ideas explain the whole kit.

## 1. Everything is data

Maps, towers, economy rules, generation parameters — all data files. The systems that run them never change when your content does, and malformed data is reported with an error naming the entry.

## 2. Two engines do the heavy lifting

A **seeded generation core** makes the maps: same seed, same map, guaranteed valid path. An **encounter director** makes the waves: a difficulty curve decides how hard the game gets, a budget decides what each wave is made of. Both are deterministic, so the game you test is the game your players get.

## 3. The loop is already closed

Grid → towers → economy → waves → campaign → meta. You are not assembling a game from parts; you are designing towers and maps inside a game that already plays, wins and loses.

Next: [Installation]({{ site.baseurl }}/docs/installation/), then the [Quick Start]({{ site.baseurl }}/docs/quick-start/).
