---
kb_id: "title:acl anthology 2026 loreslm 1 39 section 2 1"
type: "source"
title: "ACL Anthology 2026.loreslm-1.39, Section 2.1"
doi: null
hf_repo: null
year: null
topics: ["turkic-kyrgyz-non-kazakh-turkic-nlp-land"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["title:acl anthology 2026 loreslm 1 39 section 2 1"]
tags: ["source", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land"]
---
# ACL Anthology 2026.loreslm-1.39, Section 2.1

**Topics:** [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]]

## Source URLs
- ACL Anthology 2026.loreslm-1.39, Section 2.1

## Findings

> [!warning] UNCERTAIN — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [ky][kk] The KyrText paper explicitly documents that Kazakh/Kyrgyz splits of major multilingual pretraining corpora (OSCAR, mC4, CulturaX) are cross-contaminated: 'a large ratio of the texts included in the Kyrgyz splits of these datasets is actually in other languages — predominantly in Kazakh,' attributed to poor langID performance on the two languages, which 'share a large common vocabulary.'
>
> **Numbers:** qualitative finding, no contamination % given [UNVERIFIED extent]
> **Relevance:** DIRECT actionable risk for the lab's own Kazakh corpus: any CulturaX/mC4/OSCAR-derived Kazakh training data likely contains uncounted Kyrgyz contamination, which would corrupt vocabulary/perplexity and dilute the from-scratch tokenizer's fertility advantage. Recommend adding an explicit kk-vs-ky binary classifier pass (not generic langID) to the lab's own data-cleaning pipeline.
> **Source:** ACL Anthology 2026.loreslm-1.39, Section 2.1 · **Sweep:** `turkic-landscape`

[[Home]]
