---
kb_id: "title:aclanthology org 2025 findings emnlp 471 table 2 and section 4 discussion bitext mining challenge"
type: "source"
title: "aclanthology.org/2025.findings-emnlp.471, Table 2 and Section 4 discus…"
doi: null
hf_repo: null
year: null
topics: ["non-kazakh-turkic-nlp-landscape-embeddin"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:aclanthology org 2025 findings emnlp 471 table 2 and section 4 discussion bitext mining challenge"]
tags: ["source", "topic/non-kazakh-turkic-nlp-landscape-embeddin"]
---
# aclanthology.org/2025.findings-emnlp.471, Table 2 and Section 4 discus…

**Topics:** [[non-kazakh-turkic-nlp-landscape-embeddin]]

## Source URLs
- aclanthology.org/2025.findings-emnlp.471, Table 2 and Section 4 discussion ('Bitext Mining Challenge')

## Findings

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-embeddin
> [tr] TR-MTEB's own specialized Turkish embedding models (contrastively pretrained from BERTurk on 34.2M weakly-supervised Turkish pairs, then supervised fine-tuned) underperform mE5-large on EVERY task category except Pair Classification and are dramatically worse at Bitext Mining (37.7-86.88 vs mE5-large's 99.43), because monolingual training provides no cross-lingual signal — confirming that a from-scratch or single-language-fine-tuned embedder trades away cross-lingual/bitext capability for modest task-specific gains.
>
> **Numbers:** Bitext: turkish-embedding-model-fine-tuned 86.88 / turkish-embedding-model (contrastive only) 37.7 vs mE5-large 99.43 and LaBSE 99.53; overall Mean(Task): mE5-large 66.82 vs turkish-embedding-model-fine-tuned 63.42
> **Relevance:** Directly informs the lab's own architecture choice: if the Kazakh embedding effort ever considers a from-scratch or monolingual-only fine-tune path (vs. Less-is-More's approach of lightly adapting mE5-base while keeping its multilingual backbone), the Turkish precedent shows monolingual specialization sacrifices bitext/cross-lingual retrieval (relevant given heavy kk/ru code-switching) for gains that don't even reach mE5-large's aggregate score.
> **Source:** aclanthology.org/2025.findings-emnlp.471, Table 2 and Section 4 discussion ('Bitext Mining Challenge') · **Sweep:** `turkic-landscape`

[[Home]]
