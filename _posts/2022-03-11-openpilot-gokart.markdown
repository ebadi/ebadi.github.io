---
layout: post
title: OpenPilot on Infotiv Go-Kart Platform
date: 2022-03-11 00:00:00 +0300
description: Adaptation of the OpenPilot open-source driver assistance system to run on Infotiv's go-kart platform, enabling autonomous driving features on the physical vehicle.
img: openpilot.png
tags: [autonomous-driving, robotics, openpilot, machine-learning, simulator]
---

openpilot_gokart is an adaptation of [OpenPilot](http://github.com/commaai/openpilot) — the open source driver assistance system by comma.ai — to run on Infotiv's go-kart platform. This fork enables autonomous driving features on the physical go-kart vehicle.

## OpenPilot in CARLA

Verification and Validation of OpenPilot driver assistance system within the CARLA simulator:

<iframe width="560" height="315" src="https://www.youtube.com/embed/onnVoFoYCOA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What is OpenPilot?

OpenPilot is an open source driver assistance system that provides:

- **Adaptive Cruise Control (ACC)**
- **Automated Lane Centering (ALC)**
- **Forward Collision Warning (FCW)**
- **Lane Departure Warning (LDW)**
- **Driver Monitoring (DM)** — alerts distracted and drowsy drivers

## Running on the Go-Kart

The go-kart fork adapts OpenPilot's software stack to interface with the Infotiv Autonomous Platform hardware. A supported device (e.g. comma three) runs the software, connected to the go-kart via a custom harness.

## Running in Simulation

OpenPilot can also be run in simulation [with the CARLA simulator](https://github.com/commaai/openpilot/tree/master/tools/sim/README.md), which is the basis for development and testing before deployment on the physical platform.

## License

OpenPilot is released under the MIT license.

> **THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT. YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.**

### Links

[openpilot_gokart GitHub repository](https://github.com/ebadi/openpilot_gokart)
