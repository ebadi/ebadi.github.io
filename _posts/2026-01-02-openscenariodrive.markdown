---
layout: post
title: OpenScenarioDrive — PyQt6 Editor for OpenSCENARIO and OpenDRIVE
date: 2026-01-02 00:00:00 +0300
description: PyQt6-based graphical editor for OpenSCENARIO (.xosc) and OpenDRIVE (.xodr) files with real-time simulation control, syntax highlighting, undo/redo, and dynamic element highlighting synchronized to simulation events.
img: https://img.youtube.com/vi/66SUEqmxTLk/0.jpg
tags: [simulator, autonomous-driving, openscenario]
---

OpenScenarioDrive is a PyQt6-based graphical controller and editor for OpenSCENARIO `.xosc` files. It provides a real-time simulation control interface with integrated XML editors for both `.xosc` and `.xodr` files.

## Demo

<iframe width="560" height="315" src="https://www.youtube.com/embed/66SUEqmxTLk" title="OpenScenarioDrive Editor for OpenSCENARIO .xosc files" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Features

### Simulation Control

- **Play / Pause / Restart / single-step** — scenario control
- **Rewind** — scrub through recorded frame history without re-running the simulation
- **Configurable time step** — adjust simulation `dt` from 0.001 s to 1.0 s
- **Pause on event** — automatically pause when a storyboard event or condition fires

### Object Inspection

- Live list of all active actors in the scenario
- Select any actor to view and edit 3D position (X, Y, Z) and orientation (heading, pitch, roll)
- Apply position changes to the running simulation

### OpenScenario Editor

- XML syntax highlighting (tags, attributes, values)
- Line-number gutter with indent-based code folding
- **Auto-save** — flushes edits to a temporary file every 500 ms
- **Undo / Redo** — full document history
- **Search** — incremental find with forward/backward navigation
- **Dynamic highlighting** — on storyboard event trigger, the relevant XML element is automatically scrolled to and highlighted

### OpenDrive Editor

- Same XML editor features as the OpenScenario editor
- Road ID cross-highlighting: selecting an actor highlights the matching `<road>` element

## Installation

Pre-built installers for Windows, macOS, and Linux are available on the [GitHub Releases page](https://github.com/ebadi/OpenScenarioDrive/releases/latest).

### Links

[OpenScenarioDrive GitHub repository](https://github.com/ebadi/OpenScenarioDrive)
