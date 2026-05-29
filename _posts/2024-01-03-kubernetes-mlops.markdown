---
layout: post
title: Kubernetes MLOps Platform
date: 2024-01-03 00:00:00 +0300
description: Kubernetes-based MLOps platform providing scripts and documentation to set up a cluster with local image registry, containerized model training, and distributed GPU training for object detection and other ML tasks.
img: https://raw.githubusercontent.com/ebadi/Kubernetes-MLOps/master/resources/cluster-forklift.png
tags: [mlops, kubernetes, machine-learning, docker]
---

Kubernetes-MLOps contains the results from a master thesis on "Automation and Orchestration for Machine Learning Pipelines" by Filip Melberg and Vasiliki Kostara, supervised by Hamid Ebadi at Infotiv AB. It provides scripts and documentation to set up a fully reproducible Kubernetes-based ML training cluster.

## High-Level Design

Two ML projects are supported:

### Object Detection (YOLOv5)
Containerized training of a forklift/people object detector on a Kubernetes cluster.

### Distributed Data Parallel (DDP) Training
Introduces distributed GPU training, extending the cluster with additional worker nodes.

## High-Level Requirements

1. Automated and reproducible (Docker, scripts, config files)
2. Open-source / free solution
3. Use of cluster for training and load balancing
4. Version controlling for code, data, and models

## Infrastructure

The setup includes:
- Kubernetes control plane and worker nodes on VirtualBox VMs (Ubuntu 22.04)
- Local image registry and Samba storage
- Kubernetes Dashboard
- Networked via Bridged Adapter (all nodes on the same LAN)

## Funding

Research carried out within the [SMILE IV](https://www.vinnova.se/p/smile-iv/) project, financed by Vinnova, FFI under grant number 2023-00789.

### Links

[Kubernetes-MLOps GitHub repository](https://github.com/ebadi/Kubernetes-MLOps)
