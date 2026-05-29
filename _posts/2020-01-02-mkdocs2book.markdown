---
layout: post
title: mkdocs2book — Convert MkDocs Documentation to Books
date: 2020-01-02 00:00:00 +0300
description: Converts MkDocs documentation projects into formatted books by combining all Markdown files and using Pandoc to generate PDF, EPUB, and HTML output with custom LaTeX templates.
img: # no image in README
tags: [documentation, tooling, pandoc, mkdocs]
---

mkdocs2book converts documentation written in [MkDocs](https://www.mkdocs.org/) format into readable books in multiple formats (PDF, EPUB, HTML). It uses a modified version of mkdocscombine to merge all `.md` files into a single Pandoc source, then applies custom LaTeX templates to produce well-formatted output.

## How It Works

1. Uses a modified [mkdocscombine](https://github.com/twardoch/mkdocs-combine) to combine all `*.md` files into a single Pandoc file (`book.pd`), following the order defined in `mkdocs.yml`
2. Applies a modified LaTeX template from [pandoc-book-template](https://github.com/wikiti/pandoc-book-template) with proper code block wrapping
3. Uses [Pandoc](https://pandoc.org/) to generate `.PDF` and `.EPUB` output

## Usage

```bash
sudo docker build -f Dockerfile -t mkdocs2book:latest .

git clone https://github.com/ebadi/carla.git
sudo docker run -v=$PWD:/data/ mkdocs2book:latest /data/build.sh carla

git clone https://github.com/ebadi/scenario_runner.git
sudo docker run -v=$PWD:/data/ mkdocs2book:latest /data/build.sh scenario_runner
```

Example outputs: [Carla Simulator PDF](https://github.com/ebadi/mkdocs2book/raw/main/carla0.9.11.pdf) and [Scenario Runner PDF](https://github.com/ebadi/mkdocs2book/raw/main/scenario_runner.pdf).

### Links

[mkdocs2book GitHub repository](https://github.com/ebadi/mkdocs2book)
