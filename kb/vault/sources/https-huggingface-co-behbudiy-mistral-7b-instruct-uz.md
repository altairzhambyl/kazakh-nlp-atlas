---
kb_id: "hf:behbudiy/mistral-7b-instruct-uz"
type: "source"
title: "https://huggingface.co/behbudiy/Mistral-7B-Instruct-Uz"
doi: null
hf_repo: "behbudiy/Mistral-7B-Instruct-Uz"
year: null
topics: ["turkic-uzbek-non-kazakh-turkic-nlp-lands"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["hf:behbudiy/mistral-7b-instruct-uz"]
tags: ["source", "topic/turkic-uzbek-non-kazakh-turkic-nlp-lands"]
---
# https://huggingface.co/behbudiy/Mistral-7B-Instruct-Uz

**Topics:** [[turkic-uzbek-non-kazakh-turkic-nlp-lands]]

## Source URLs
- https://huggingface.co/behbudiy/Mistral-7B-Instruct-Uz

## Findings

> [!warning] UNCERTAIN — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz] Behbudiy Labs (2024-2025, HF org 'behbudiy'): continual-pretrained + instruction-tuned Uzbek variants of Mistral-7B-Instruct, Mistral-Nemo-Instruct, and Llama-3.1-8B-Instruct on 'over 5B Uzbek tokens' (mix of public + synthetic data), claiming '2x token efficiency vs global models' (no absolute fertility number given). Mistral-7B-Instruct-Uz vs base Mistral-7B-Instruct: FLORES+ BLEU Uz-En 7.47->29.39, En-Uz 0.67->16.77; COMET Uz-En 68.14->86.91, En-Uz 45.58->88.75; sentiment analysis 62.02%->79.13%; news classification 47.52%->59.38%; but English MMLU regressed 61.07%->55.72% (specialization tax). Apache 2.0.
>
> **Numbers:** BLEU Uz-En 7.47->29.39, En-Uz 0.67->16.77; COMET Uz-En 68.14->86.91, En-Uz 45.58->88.75; sentiment 62.02%->79.13%; news-class 47.52%->59.38%; MMLU-en 61.07%->55.72%
> **Relevance:** Direct evidence of the same generative-target trade-off pattern the lab measures for Kazakh (Kazakh-specialization gains vs general-knowledge tax); no arXiv/technical report found, only HF model card, so the '2x token efficiency' and '5B tokens' claims are unverified beyond the card itself.
> **Source:** https://huggingface.co/behbudiy/Mistral-7B-Instruct-Uz · **Sweep:** `turkic-landscape`

[[Home]]
