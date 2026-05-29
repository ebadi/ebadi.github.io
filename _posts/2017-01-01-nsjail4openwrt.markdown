---
layout: post
title: nsjail4openwrt — Process Isolation for OpenWrt
date: 2017-01-01 00:00:00 +0300
description: Tooling and patches to cross-compile nsjail (process isolation/sandboxing tool) for OpenWrt embedded Linux devices.
img: # no README image
tags: [security, embedded, openwrt, sandboxing]
---

nsjail4openwrt provides tooling and patches to cross-compile [nsjail](https://github.com/google/nsjail) — Google's process isolation and sandboxing tool — for OpenWrt embedded Linux devices.

nsjail uses Linux namespaces, cgroups, and seccomp-bpf to provide lightweight process sandboxing. This project adapts it to run on resource-constrained OpenWrt routers and embedded systems.

The repository contains a Makefile and a series of patches (`001.patch` through `004.patch`) needed to build nsjail for the OpenWrt toolchain.

### Links

[nsjail4openwrt GitHub repository](https://github.com/ebadi/nsjail4openwrt)

[Google nsjail](https://github.com/google/nsjail)
