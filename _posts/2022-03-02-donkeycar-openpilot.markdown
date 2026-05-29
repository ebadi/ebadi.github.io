---
layout: post
title: DonkeyCar + OpenPilot Integration
date: 2022-03-02 00:00:00 +0300
description: Integrates OpenPilot with the DonkeyCar simulator, allowing testing and experimentation with autonomous driving capabilities in a virtual environment without physical hardware.
img: donkey.png
tags: [simulator, autonomous-driving, machine-learning, openpilot]
---

donkeycar-openpilot integrates [OpenPilot](http://github.com/commaai/openpilot) — the open source driver assistance system by comma.ai — with the [DonkeyCar](https://www.donkeycar.com/) simulator. This allows testing and experimenting with autonomous driving capabilities in a virtual environment without requiring physical hardware.

## DonkeyCar in Self Driving Car Sandbox

Verification and validation of DonkeyCar within the [Self Driving Car Sandbox simulator](https://github.com/tawnkramer/sdsandbox):

<iframe width="560" height="315" src="https://www.youtube.com/embed/tcwXxLMq950" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What is OpenPilot?

OpenPilot is an open source driver assistance system that performs:

- **Adaptive Cruise Control (ACC)**
- **Automated Lane Centering (ALC)**
- **Forward Collision Warning (FCW)**
- **Lane Departure Warning (LDW)**
- **Driver Monitoring (DM)** — alerts distracted and drowsy drivers

## Running on PC

All of OpenPilot's services can run as normal on a PC without special hardware or a car. You can run OpenPilot on recorded or simulated data, plot logs, replay drives, and watch full-resolution camera streams.

OpenPilot can also run in simulation [with the CARLA simulator](https://github.com/commaai/openpilot/tree/master/tools/sim/README.md), allowing the system to drive in a virtual environment on Ubuntu with a GPU.

## License

OpenPilot is released under the MIT license.

> **THIS IS ALPHA QUALITY SOFTWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT. YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.**

### Links

[donkeycar-openpilot GitHub repository](https://github.com/ebadi/donkeycar-openpilot)
