---
kb_id: "arxiv:2407.12402"
type: "paper"
title: "TurkishMMLU: Measuring Massive Multitask Language Understanding in Turkish"
arxiv_id: "2407.12402"
doi: null
hf_repo: null
year: 2024
topics: ["turkic-turkish"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["TurkishMMLU: Measuring Massive Multitask Language Understanding in Turkish", "arXiv:2407.12402", "arxiv:2407.12402"]
tags: ["paper", "topic/turkic-turkish"]
---
# TurkishMMLU: Measuring Massive Multitask Language Understanding in Turkish

[arXiv](https://arxiv.org/abs/2407.12402)
**Topics:** [[turkic-turkish]]

> [!abstract]
> Multiple choice question answering tasks evaluate the reasoning, comprehension, and mathematical abilities of Large Language Models (LLMs). While existing benchmarks employ automatic translation for multilingual evaluation, this approach is error-prone and potentially introduces culturally biased questions, especially in social sciences. We introduce the first multitask, multiple-choice Turkish QA …

## Claims

> [!note] CLAIM — turkic-turkish
> [tr] TurkishMMLU (KUIS AI, ACL 2024 Findings) is the flagship Turkish knowledge benchmark: 10,032 questions (9,807 test + 225 dev), 9 subjects from Turkish high-school curricula. On the 900-question sub-benchmark at 5-shot: GPT-4o 83.1%, Claude-3 Opus 79.1%, Llama-3-70B-IT 67.3%, and the Turkish-adapted Trendyol-LLM-7B-chat-v1 only 34.1% — the weakest model tested, well below even much smaller general multilingual models like Aya-23-35B (55.6%).
>
> **Numbers:** 10,032 total (9,807 test/225 dev); 9 subjects; 5-shot 900-q subset: GPT-4o 83.1%, Claude-3-Opus 79.1%, Llama-3-70B-IT 67.3%, Trendyol-LLM-7B-C 34.1%, Aya-23-35B 55.6%
> **Relevance:** Turkey's own dedicated 7B Turkish-tuned model (Trendyol) scoring worse than models 5-10x smaller (Aya-23 in relative terms) reinforces that instruction-tuning a strong multilingual base on Turkish text alone, without deeper adaptation (vocab extension, larger corpus), underperforms — informs the lab's Sherkala-style (vocab-extension) preference over naive fine-tuning.
> **Source:** arXiv:2407.12402 (TurkishMMLU) · **Sweep:** `turkic-landscape`

[[Home]]
