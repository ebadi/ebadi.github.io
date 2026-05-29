---
layout: post
title: Sim-to-Real Style Transfer
date: 2026-01-04 00:00:00 +0300
description: Converts Gazebo simulator recordings into photorealistic factory footage using a ComfyUI pipeline with AnimateDiff for temporal consistency or per-frame processing with LoRA fine-tuning.
img: # no image in README
tags: [simulation, machine-learning, computer-vision, deep-learning, gazebo]
---

style-transfer converts Gazebo simulator video into photorealistic factory footage using your own factory images as style reference. It uses a ComfyUI pipeline with either AnimateDiff for temporal consistency or per-frame processing with LoRA fine-tuning.

## Two Inference Pipelines

**Video Pipeline** — processes the entire video as one AnimateDiff job in ComfyUI, using temporal attention for smooth output:

```bash
./infer.sh video
```

**Image Pipeline** — extracts frames via ffmpeg, submits each as a separate ComfyUI job, and reassembles with temporal blending, enabling per-frame control:

```bash
./infer.sh frame
```

## System Requirements

- Docker and Docker Compose v2
- NVIDIA Container Toolkit
- NVIDIA GPU with ≥ 8 GB VRAM
- ~20 GB free disk space

## Setup

**1. Organize data**

```
data/
├── input/
│   └── your_video.mp4
└── sample_images/
    └── *.jpg / *.png
```

Update `input.video` in `config.yaml` with your video filename.

**2. Download pretrained models (~11 GB)**

```bash
chmod +x *.sh
./download_models.sh
```

Downloads: Realistic Vision V5.1, ControlNet canny, IP-Adapter Plus, CLIP Vision ViT-H, VAE, AnimateDiff v2.

**3. Train LoRA** (learns factory style from your reference images)

```bash
./train.sh
```

Output: `models/loras/factory_lora.safetensors`

**4. Run inference**

```bash
./infer.sh video    # AnimateDiff pipeline
./infer.sh frame    # Per-frame pipeline
```

Output: `data/output/stylized_video.mp4`

The ComfyUI web interface is accessible at `http://localhost:8188` during inference.

## Parameter Testing

```bash
./test_params.sh
```

Runs four inference jobs with parameter variations, saving results with descriptive filenames for easy comparison.

### Links

[style-transfer GitHub repository](https://github.com/ebadi/style-transfer)
