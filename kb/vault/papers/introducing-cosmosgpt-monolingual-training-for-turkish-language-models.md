---
kb_id: "arxiv:2404.17336"
type: "paper"
title: "Introducing cosmosGPT: Monolingual Training for Turkish Language Models"
arxiv_id: "2404.17336"
doi: null
hf_repo: null
year: 2024
topics: ["turkic-turkish"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["Introducing cosmosGPT: Monolingual Training for Turkish Language Models", "arXiv:2404.17336", "arxiv:2404.17336"]
tags: ["paper", "topic/turkic-turkish"]
---
# Introducing cosmosGPT: Monolingual Training for Turkish Language Models

[arXiv](https://arxiv.org/abs/2404.17336)
**Topics:** [[turkic-turkish]]

> [!abstract]
> The number of open source language models that can produce Turkish is increasing day by day, as in other languages. In order to create the basic versions of such models, the training of multilingual models is usually continued with Turkish corpora. The alternative is to train the model with only Turkish corpora. In this study, we first introduce the cosmosGPT models that we created with this alter …

## Claims

> [!note] CLAIM — turkic-turkish
> [tr] cosmosGPT (YTU COSMOS, Apr 2024) is architecturally near-identical prior art to SozKZ one Turkic step earlier: monolingual from-scratch GPT-2-style models (355M, 774M params), dedicated ByteLevel BPE 50,257-token vocab trained on 100GB, total pretraining corpus 275GB (250GB cleaned/deduped CulturaX + 25GB other Turkish sources), trained on TPUv3-8. In direct ELO-based human-preference comparison it LOSES to the larger adapted Trendyol-LLM-7B (cosmosGPT-Large ELO 969 / 43.19% win-rate vs Trendyol-7B 1194 ELO / 70.34% win-rate) despite matched vocab size and from-scratch monolingual training.
>
> **Numbers:** 355M/774M params; 50,257 BPE vocab (identical size to SozKZ's); 275GB corpus (250GB CulturaX-derived); ELO 969 vs 1194; win-rate 43.19% vs 70.34%
> **Relevance:** Cross-Turkic corroboration of the SozKZ finding already in the Kazakh KB: from-scratch small monolingual Turkic models with a great dedicated tokenizer consistently lose to larger adapted/continual-PT models on the SAME family, strengthening the case that the Kazakh Frontier Lab's architectural differentiation (Engram/memory) rather than 'from-scratch + good tokenizer alone' is the right bet.
> **Source:** arXiv:2404.17336 (cosmosGPT), huggingface.co/ytu-ce-cosmos · **Sweep:** `turkic-landscape`

[[Home]]
