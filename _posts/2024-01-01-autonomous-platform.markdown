---
layout: post
title: Autonomous Platform Generation 4
date: 2024-01-01 00:00:00 +0300
description: Modular, scalable go-kart robotic platform (Generation 4) for testing autonomous driving algorithms, featuring a three-tier ROS2 software architecture, drive-by-wire, and a Gazebo digital twin.
img: https://img.youtube.com/vi/hyw-hApxQHU/0.jpg
tags: [autonomous-driving, ros2, robotics, simulation, machine-learning]
---

Autonomous Platform (Generation 4) is a platform at Infotiv on which internal and external research projects can be tested — particularly autonomous driving algorithms. The system features a modular mono-repository collecting all software and hardware design components in one place.

## Autonomous Navigation with LiDAR and SLAM

<iframe width="560" height="315" src="https://www.youtube.com/embed/hyw-hApxQHU" title="AP4 Autonomous Driving Navigation/SLAM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Imitation Learning

<iframe width="560" height="315" src="https://www.youtube.com/embed/8izLmmYHW0s" title="AP4 Autonomous Driving — Imitation Learning" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Raw footage:

<iframe width="560" height="315" src="https://www.youtube.com/embed/A2l_nDKsU7g" title="AP4 Imitation Learning raw footage" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## System Architecture

The platform has three software layers:

- **High-level control** — autonomous driving algorithms, Gazebo digital twin, RViz
- **Low-level control** — Raspberry Pi 4b, ROS2 `\cmd_vel` to CAN bus bridge
- **Embedded control** — ECU firmware (Arduino/PlatformIO) for steering and propulsion (SPCU)

## Capabilities

- Drive-by-wire with Xbox 360 controller
- Imitation Learning via Behavioral Cloning (BC) and Human Gated Dataset Aggregation (HG-DAgger)
- LiDAR-based SLAM and autonomous navigation with Nav2
- Gazebo digital twin synchronized with the physical platform
- Fully Dockerized software stack

## Master Theses

- **Spring 2023** (Fredrik Juthe, Erik Magnusson): E/E and software architecture design
- **Spring 2024** (Arvid Petersén, Johan Wellander): Imitation learning pipeline (BC + HG-DAgger)
- **Spring 2025** (David Espedalen, Anton Stigemyr Hill): LiDAR-based SLAM and autonomous navigation

All three theses are supervised by Hamid Ebadi at Infotiv AB.

### Links

[Autonomous Platform GitHub repository](https://github.com/infotiv-research/autonomous_platform)
