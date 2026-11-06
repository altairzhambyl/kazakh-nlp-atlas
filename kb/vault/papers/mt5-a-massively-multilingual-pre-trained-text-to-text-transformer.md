---
kb_id: "arxiv:2010.11934"
type: "paper"
title: "mT5: A massively multilingual pre-trained text-to-text transformer"
arxiv_id: "2010.11934"
doi: null
hf_repo: null
year: 2020
topics: ["turkic-nlp-landscape-uzbek-monolingual-p"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["mT5: A massively multilingual pre-trained text-to-text transformer", "arXiv:2010.11934", "arxiv:2010.11934"]
tags: ["paper", "topic/turkic-nlp-landscape-uzbek-monolingual-p"]
---
# mT5: A massively multilingual pre-trained text-to-text transformer

[arXiv](https://arxiv.org/abs/2010.11934)
**Topics:** [[turkic-nlp-landscape-uzbek-monolingual-p]]

> [!abstract]
> The recent "Text-to-Text Transfer Transformer" (T5) leveraged a unified text-to-text format and scale to attain state-of-the-art results on a wide variety of English-language NLP tasks. In this paper, we introduce mT5, a multilingual variant of T5 that was pre-trained on a new Common Crawl-based dataset covering 101 languages. We detail the design and modified training of mT5 and demonstrate its s …

## Claims

> [!note] CLAIM — turkic-nlp-landscape-uzbek-monolingual-p
> [uz][kk][ky][az] The original mT5-era mC4 (2020, pre-CulturaX, single-snapshot generation) reports Uzbek = 0.9B tokens / 0.8M pages (0.46% of mT5 mixture) vs Kazakh 3.1B tokens / 2.4M pages (0.65%), Kyrgyz 1.0B tokens / 1.0M pages (0.50%), Azerbaijani 4.4B tokens / 5.3M pages (0.82%), Turkish 71B tokens / 88M pages (1.93%).
>
> **Numbers:** uz 0.9B tok/0.8M pages; kk 3.1B tok/2.4M pages; ky 1.0B tok/1.0M pages; az 4.4B tok/5.3M pages; tr 71B tok/88M pages
> **Relevance:** Shows Uzbek and Kyrgyz sit in the same low-resource tier (~0.9-1.0B mC4 tokens each), both well below Kazakh/Azerbaijani and far below Turkish — useful for Decision 1 ranking of port order if FineWeb2-scale corpora are unavailable for some candidate language and mC4/CulturaX-class resources must be used instead.
> **Source:** Xue et al. 2020, 'mT5: A Massively Multilingual Pre-trained Text-to-Text Transformer', arXiv:2010.11934, Table 6 (fetched PDF directly, verified row values) · **Sweep:** `turkic-landscape`

[[Home]]
