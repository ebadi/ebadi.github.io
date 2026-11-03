---
layout: post
title: AI Course for Engineers
date: 2026-10-29 00:00:00 +0100
description: A one-day workshop at INFOTIV about how AI and large language models work. Engineers learn to use language models and AI agents on real code, and to verify the results.
img: # no image
tags: [machine-learning, llm, ai-agents, teaching]
---

The AI Course for Engineers is a one-day workshop that I teach at INFOTIV. The workshop explains how AI and large language models (LLMs) work. With this knowledge, engineers can use these tools with a plan, not by luck.

The workshop moves the participants from "vibe coding" to agentic engineering. The participants write specifications, set rules and checks, run agents on real code and verify the results. The workshop does not give "magic prompts".

#### Demos

An AI agent wrote all the code for these two demos. Nobody wrote the code by hand.

**3D modelling and video creation**: A robot arm lifts a glass. Code from an agent makes the scene, the motion and the soundtrack.

<video controls preload="metadata" playsinline style="width: 100%; height: auto;">
  <source src="https://infotiv-research.github.io/ai-course/robotarm-glass-liftlow/robotarm_glass_liftlow_audio.mp4" type="video/mp4">
  <a href="https://infotiv-research.github.io/ai-course/robotarm-glass-liftlow/robotarm_glass_liftlow_audio.mp4">Download the robot arm video</a>
</video>

**Super Mario++**: The first level of the classic game, with new features. The new features are weapons (banana boomerang, dynamite and laser beam), wings, an umbrella and a new enemy (bomber planes).

<video controls preload="metadata" playsinline style="width: 100%; height: auto;">
  <source src="https://infotiv-research.github.io/ai-course/mario-game/features.mp4" type="video/mp4">
  <a href="https://infotiv-research.github.io/ai-course/mario-game/features.mp4">Download the Super Mario++ video</a>
</video>

#### Target audience

* Developers
* Testers and quality assurance engineers
* Engineers in safety-critical and regulated domains
* Technical leads and engineering managers

#### Agenda

The workshop is one day, from 09:00 to 16:00. It has ten sessions.

1. **Intro**: What this day is and what it is not.
   *Topics: Mario demonstration, human and AI, from luck to repeatable results, how we work today.*
2. **Inside the box**: AI, machine learning and deep learning. The participants train a small neural network by hand.
   *Topics: machine learning, neural networks, deep learning, CNN, RNN, diffusion, multimodal models.*
3. **Language models**: How a model reads text and writes the next word.
   *Topics: embeddings, tokens, transformers, temperature, context window.*
4. **Working with the model**: Prompts, and how to write a specification that the model can follow.
   *Topics: vibe coding, prompt engineering, chain prompting, goals, boundaries and checks.*
5. **Harness, tools and agents**: How to give the model tools.
   *Topics: agents, tool calling, Claude Code, Model Context Protocol (MCP), skills, command line.*
6. **Context engineering and memory**: What to put in the context of the model and what to leave out.
   *Topics: context rot, memory, retrieval-augmented generation (RAG), OpenRouter.*
7. **Security and brakes**: Sandboxes, credentials and poisoned text.
   *Topics: sandboxes, prompt injection.*
8. **Limits, failures and verification**: False output, bias, tests and review. How to know if the output is good.
   *Topics: hallucination, bias, AI slop, testing, benchmarks.*
9. **Ethics, law and obligations**: Real incidents, the EU AI Act and who is responsible.
   *Topics: misalignment, real incidents, EU AI Act, standards.*
10. **Models, cost and running locally**: What you pay for, and how to run a model on your own computer.
    *Topics: token cost, open and closed models, local models, quantization, fine-tuning.*

The participants answer quiz questions on their phones during the day.

### Links

[AI Course for Engineers](https://infotiv-research.github.io/ai-course/)
