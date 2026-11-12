---
title: "Probing Token Spaces under Generator Shift in AI-Generated Music Detection"
short_title: "CoMoE"
collection: "publications"
category: "conferences"
permalink: "/publication/2026-06-10-probing-token-spaces"
date: 2026-06-10
spotlight: 7
authors: "Joonyong Park, Jungwoo Kim, Junyoung Koh, Yuki Saito"
venue: "ICML 2026 Workshop on Machine Learning for Audio"
venue_short: "ICML 2026 Workshop · ML for Audio"
paperurl: "https://arxiv.org/abs/2606.08663"
codeurl: "https://github.com/MAAP-LAB/CoMoE"
image: "/images/publications/probing-token-spaces.png"
image_alt: "CoMoE architecture: audio is tokenized (EnCodec, DAC, MERT k-means, X-Codec); lower- and higher-level token streams go through Transformer branches whose pooled outputs are averaged for real/fake prediction."
highlights:
  - "Keeps a compact (~10M-parameter) detector, CoMoE, fixed and swaps only its input token space: EnCodec, DAC, X-Codec mini, MERT k-means, and continuous MERT."
  - "Standard splits are nearly saturated, but restricting the fake sources (generator shift) exposes large gaps between token spaces."
  - "Argues that the discrete token space should be treated as a primary experimental variable in AI-generated music detection."
citation: "Joonyong Park, Jungwoo Kim, Junyoung Koh, Yuki Saito. \"Probing Token Spaces under Generator Shift in AI-Generated Music Detection.\" <i>ICML 2026 Workshop on Machine Learning for Audio</i>."
---
