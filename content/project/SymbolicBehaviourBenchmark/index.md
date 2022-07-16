---
title: Symbolic Behaviour Benchmark (S2B)
summary: "Suite of OpenAI Gym-compatible multi-agent reinforcement learning environment to benchmark for behavioral traits pertaining to symbolic behaviours (primarily: being receptive, constructive, malleable, and separable) using referential games."
tags:
- Symbolic Behaviours
- Language
- Multi-Agent
- Reinforcement Learning
- Meta-Learning
date: "2022-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/Near32/SymbolicBehaviourBenchmark"

image:
  caption: A Meta-Referential Game.
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/KeviDenam
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Suite of OpenAI Gym-compatible multi-agent reinforcement learning environment centered around referntial games to benchmark for behavioral traits pertaining to symbolic behaviours, as described in [Santoro et al., 2021, "Symbolic Behaviours in Artificial Intelligence"](https://arxiv.org/abs/2102.03406), primarily: exhibiting receptive, constructive, malleable, and separable behaviours.

## Usage

`gym` must be installed. Environments can be created as follows, for instance, in order to test for receptivity and constructivity:

```python
>>> import gym
>>> import symbolic_behaviour_benchmark
>>> env = gym.make(
        "SymbolicBehaviourBenchmark-ReceptiveConstructiveTestEnv-v0", 
        vocab_size=10,
        max_sentence_length=5,
        nbr_latents=5,
        min_nbr_values_per_latent=3,
        max_nbr_values_per_latent=5,
        nbr_object_centric_samples=1,
        nbr_distractors=3,
        use_communication_channel_permutations=True,
        allow_listener_query=False,
    )
```

## Installation

### Installing via pip

This package is available in PyPi as `symbolic_behaviour_benchmark`

```bash
pip install symbolic_behaviour_benchmark
```

### Installing via cloning this repository

```bash
git clone https://www.github.com/Near32/SymbolicBehaviourBenchmark
cd SymbolicBehaviourBenchmark
pip install -e .
```
