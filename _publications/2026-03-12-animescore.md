---
title: "AnimeScore: A Preference-Based Dataset and Framework for Evaluating Anime-Like Speech Style"
short_title: "AnimeScore"
collection: "publications"
category: "conferences"
permalink: "/publication/2026-03-12-animescore"
date: 2026-03-12
spotlight: 8
authors: "Joonyong Park, Jerry Li"
venue: "Proceedings of INTERSPEECH 2026"
venue_short: "INTERSPEECH 2026"
paperurl: "https://arxiv.org/abs/2603.11482"
codeurl: "https://github.com/sizigi/animescore"
demourl: "https://huggingface.co/spaces/spellbrush/animescore-demo"
modelurl: "https://huggingface.co/spellbrush/animescore"
image: "/images/publications/animescore.png"
image_alt: "AnimeScore model: a frozen SSL encoder, BiLSTM, mean pooling and an MLP predict a score s(x), trained with a pairwise RankNet loss on A/B preferences."
highlights:
  - "A preference-based metric for *anime-likeness* in Japanese speech, a style that has no shared absolute scale for MOS-style rating."
  - "Collects 15,000 pairwise A/B judgments from 187 evaluators over 3,000 utterances, and trains a RankNet scorer on frozen SSL features anchored to a MOS-like scale."
  - "SSL-based rankers reach up to 90.8% AUC, against a 69.3% ceiling for handcrafted acoustic features; the scorer serves as an automatic metric or an RL reward."
citation: "Joonyong Park, Jerry Li. \"AnimeScore: A Preference-Based Dataset and Framework for Evaluating Anime-Like Speech Style.\" <i>Proceedings of INTERSPEECH 2026</i>."
---
