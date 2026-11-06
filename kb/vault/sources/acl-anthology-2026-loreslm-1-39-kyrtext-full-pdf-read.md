---
kb_id: "title:acl anthology 2026 loreslm 1 39 kyrtext full pdf read"
type: "source"
title: "ACL Anthology 2026.loreslm-1.39 (KyrText), full PDF read"
doi: null
hf_repo: null
year: null
topics: ["turkic-other-langs-non-kazakh-turkic-nlp"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:acl anthology 2026 loreslm 1 39 kyrtext full pdf read"]
tags: ["source", "topic/turkic-other-langs-non-kazakh-turkic-nlp"]
---
# ACL Anthology 2026.loreslm-1.39 (KyrText), full PDF read

**Topics:** [[turkic-other-langs-non-kazakh-turkic-nlp]]

## Source URLs
- ACL Anthology 2026.loreslm-1.39 (KyrText), full PDF read

## Findings

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [ky] KyrText (ACL LoResLM 2026, arXiv-adjacent, aclanthology 2026.loreslm-1.39) is the largest curated Kyrgyz corpus found: 680.5M words (2,334,281 docs) from news (61.4%, 1.91M docs), court decisions (23.9%), legislation (9.9%), Wikipedia (1.34%), and digitized e-library (3.45%, OCR'd via DeepSeek-OCR). Continual-pretrained xlm-roberta-large-kgz is the best resulting model, beating its own un-adapted xlm-roberta-large baseline by +19pp XNLI (0.76 vs 0.55), +18pp PAWS-X (0.85 vs 0.66), +7pp BoolQ (0.79 vs 0.72). RoBERTa trained FROM SCRATCH on only 680.5M words underperforms continual-pretrained multilingual models on tasks needing cross-lingual knowledge (PAWS-X, XNLI) despite competitive News/SST scores — a from-scratch-vs-adapt datapoint at ~680M-word scale.
>
> **Numbers:** 680.5M words total (Train 672.3M/Test 8.2M); News 1.91M docs/413.7M words (45.6% after upsampling), Courts 172,772 docs/160.8M words, Legal 157,021 docs/66.8M words, Wikipedia 89,657 docs/8.7M words (5x upsampled), E-library 629 docs/22.3M words (10x upsampled); xlm-roberta-large-kgz: BoolQ 0.79±0.006, PAWS-X 0.85±0.009, XNLI 0.76±0.002, News 0.92±0.005 vs base xlm-roberta-large 0.72/0.66/0.55/0.90
> **Relevance:** Decision (1): the paper explicitly documents that OSCAR/mC4/CulturaX Kyrgyz splits are heavily contaminated by misidentified KAZAKH text ('poor performance of language identification libraries for Kyrgyz and Kazakh, which share a large common vocabulary') — a direct, actionable warning for the lab's own Kazakh corpus cleaning pipeline (check for Kyrgyz contamination in the reverse direction) and for any Kyrgyz-Kazakh joint data effort.
> **Source:** ACL Anthology 2026.loreslm-1.39 (KyrText), full PDF read · **Sweep:** `turkic-landscape`

[[Home]]
