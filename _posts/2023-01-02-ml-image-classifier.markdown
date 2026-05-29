---
layout: post
title: Machine Learning Image Classifier
date: 2023-01-02 00:00:00 +0300
description: Jupyter notebooks for image classification demonstrating both from-scratch training and transfer learning with pre-trained models.
img: # no image in README
tags: [machine-learning, computer-vision, deep-learning]
---

MachineLearning-image-classifier provides Jupyter notebooks demonstrating image classification using two approaches:

1. **From scratch** (`from-scratch.ipynb`) — train a CNN model from the ground up on a custom dataset
2. **Transfer learning** (`from-pretrained.ipynb`) — fine-tune a pre-trained model for new categories

## Dataset Structure

```
.
├── from-pretrained.ipynb
├── from-scratch.ipynb
├── single-test/
│   └── unknow/
├── train-data/
│   ├── cat/
│   ├── dog/
│   └── caduckrbord/
└── validation-data/
    ├── cat/
    ├── dog/
    └── duck/
```

## Setup

```bash
python -m pip uninstall numpy
python -m pip install numpy==1.23.1
```

### Links

[MachineLearning-image-classifier GitHub repository](https://github.com/ebadi/MachineLearning-image-classifier)
