---
kb_id: "arxiv:2407.02337"
type: "paper"
title: "Open foundation models for Azerbaijani language"
arxiv_id: "2407.02337"
doi: null
hf_repo: null
year: 2024
topics: ["turkic-other-langs-non-kazakh-turkic-nlp"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["Open foundation models for Azerbaijani language", "arXiv:2407.02337", "arxiv:2407.02337"]
tags: ["paper", "topic/turkic-other-langs-non-kazakh-turkic-nlp"]
---
# Open foundation models for Azerbaijani language

[arXiv](https://arxiv.org/abs/2407.02337)
**Topics:** [[turkic-other-langs-non-kazakh-turkic-nlp]]

> [!abstract]
> The emergence of multilingual large language models has enabled the development of language understanding and generation systems in Azerbaijani. However, most of the production-grade systems rely on cloud solutions, such as GPT-4. While there have been several attempts to develop open foundation models for Azerbaijani, these works have not found their way into common use due to a lack of systemic …

## Claims

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [uz] Azerbaijani has the strongest published from-scratch encoder foundation of any non-Kazakh Turkic language found in this sweep, but has NO generative sub-1B LLM and NO embedding/retrieval benchmark: aLLMA family (45.9M/135.2M/369.5M params, WordPiece 64k vocab) trained on DOLLMA (651.1M whitespace-tokenized words: Wikipedia, translated Wikipedia, news, blogs, books, legal). aLLMA-BASE (135.2M) beats same-size and larger multilingual models on 4/6 created benchmarks (AZE-SCI 90.84 F1, WikiANN 91.26, LDQuAd 86.26) despite far less pretraining data than XLM-R-Large (560M, wins WikiANN 92.35/SQuAD 75.70) or mDeBERTa-v3-base (279M, wins MRPC 83.71/AZE-NSP 78.84).
>
> **Numbers:** DOLLMA 651.1M words; aLLMA-SMALL 45.9M/BASE 135.2M/LARGE 369.5M; aLLMA-BASE: AZE-SCI 90.84, MRPC 79.74, WikiANN 91.26, SQuAD 71.30, AZE-NSP 75.95, LDQuAd 86.26; vs XLM-R-Large 560M (89.76/82.41/92.35/75.70/33.46/83.48) and mDeBERTa-v3-base 279M (87.13/83.71/91.87/72.27/78.84/85.29)
> **Relevance:** Decision (1)/(3): Azerbaijani is a genetically distant (Oghuz, not Kipchak) contrast language with a real but encoder-only foundation and zero embedding-benchmark coverage — a candidate second/alternate port target for the pinned retrieval protocol that would avoid the Kazakh-Uzbek same-branch (Kipchak/mixed) confound.
> **Source:** arXiv:2407.02337 (Isbarov et al., SIGTURK 2024, 'Open foundation models for Azerbaijani language') · **Sweep:** `turkic-landscape`

[[Home]]
