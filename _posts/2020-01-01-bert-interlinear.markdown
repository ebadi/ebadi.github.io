---
layout: post
title: BertInterlinear — BERT for Interlinear Analysis
date: 2020-01-01 00:00:00 +0300
description: Applies BERT to interlinear analysis tasks through multiple Python scripts demonstrating various BERT applications, all Dockerized for easy deployment.
img: # no image in README
tags: [nlp, machine-learning, bert, docker]
---

BertInterlinear applies BERT (Bidirectional Encoder Representations from Transformers) to interlinear analysis tasks. It includes multiple Python scripts demonstrating various BERT applications such as active fill-in-the-blank, masked language modeling, and next-word prediction — all fully Dockerized for easy deployment.

## Usage

```bash
git clone https://github.com/ebadi/fitbert.git

docker build -f Dockerfile -t bertinterlinear:latest .
docker run -v=$PWD:/data/ bertinterlinear:latest /bin/bash -c "python3 /data/activebert.py"
docker run -v=$PWD:/data/ bertinterlinear:latest /bin/bash -c "python3 /data/fitbertx.py"
docker run -v=$PWD:/data/ bertinterlinear:latest /bin/bash -c "python3 /data/betterfitbert.py"
```

The Docker image installs the BERT models during build, so no separate download step is needed.

### Links

[BertInterlinear GitHub repository](https://github.com/ebadi/BertInterlinear)
