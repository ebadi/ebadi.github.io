---
layout: post
title: Swedish Topic Modeling with BERTopic
date: 2024-01-02 00:00:00 +0300
description: Parses Swedish media archive data (Markivet) and applies BERTopic to automatically identify and extract underlying topics from Swedish-language texts.
img: # no image in README
tags: [nlp, machine-learning, swedish, topic-modeling]
---

Swedish-topic-modeling is a simple Markivet parser and topic analyser using [BERTopic](https://maartengr.github.io/BERTopic/). It parses Swedish media archive data from [Markivet](https://github.com/peterdalle/markivet) and automatically identifies and extracts underlying topics from Swedish-language texts.

## Features

- Parser for the Markivet Swedish media archive format
- BERTopic-based topic extraction
- Stop word support via [stopwords-iso](https://github.com/stopwords-iso)
- Tested against Stack Overflow Q&A datasets for benchmarking

## References

- Stop words: [stopwords-iso](https://github.com/stopwords-iso)
- Test files from [Markivet](https://github.com/peterdalle/markivet)

### Links

[Swedish-topic-modeling GitHub repository](https://github.com/ebadi/Swedish-topic-modeling)
