---
layout: post
title: Swedish Text-to-Speech
date: 2026-01-03 00:00:00 +0300
description: Dockerized Swedish text-to-speech (TTS) solution that converts written Swedish text into spoken audio using KBLab models.
img: # no image in README
tags: [nlp, tts, swedish, docker]
---

swedish-text-to-speech is a Dockerized Swedish text-to-speech (TTS) solution that converts written Swedish text into spoken audio. It uses KBLab's Swedish TTS model and packages everything in Docker for easy, dependency-free deployment.

## Quick Start

```bash
docker build -t kblab-tts .
docker run --rm -v $(pwd)/output:/app/output kblab-tts \
  "Wikipedia är en fri encyklopedi, ett uppslagsverk med öppet innehåll."
```

The generated audio is written to the `output/` directory mounted from the host.

### Links

[swedish-text-to-speech GitHub repository](https://github.com/ebadi/swedish-text-to-speech)
