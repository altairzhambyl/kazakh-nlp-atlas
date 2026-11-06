---
kb_id: "arxiv:2108.09814"
type: "paper"
title: "UzBERT: pretraining a BERT model for Uzbek"
arxiv_id: "2108.09814"
doi: null
hf_repo: null
year: 2021
topics: ["turkic-uzbek-non-kazakh-turkic-nlp-lands", "turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-pan-models"]
claims: 6
uncertain_claims: 3
verdicts: []
aliases: ["UzBERT: pretraining a BERT model for Uzbek", "arXiv:2108.09814", "arxiv:2108.09814"]
tags: ["paper", "topic/turkic-uzbek-non-kazakh-turkic-nlp-lands", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-pan-models"]
---
# UzBERT: pretraining a BERT model for Uzbek

[arXiv](https://arxiv.org/abs/2108.09814)
**Topics:** [[turkic-uzbek-non-kazakh-turkic-nlp-lands]], [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-pan-models]]

> [!abstract]
> Pretrained language models based on the Transformer architecture have achieved state-of-the-art results in various natural language processing tasks such as part-of-speech tagging, named entity recognition, and question answering. However, no such monolingual model for the Uzbek language is publicly available. In this paper, we introduce UzBERT, a pretrained Uzbek language model based on the BERT …

## Claims

> [!note] CLAIM — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz] UzBERT (Mansurov & Mansurov, arXiv:2108.09814, 2021): 110M BERT-base (12 layers, 768 hidden, 12 heads), 30K WordPiece vocab, trained on Cyrillic-only news corpus of ~142M words (~1.9GB), MIT license. Massively outperforms mBERT on masked-LM accuracy: Top-1 match 64.06% vs 14.52% (news set), 32.25% vs 14.33% (encyclopedia set). No downstream task (NER/POS/QA) evaluation was possible at publication time because NO labeled Uzbek datasets existed at all.
>
> **Numbers:** 110M params, 12L/768d/12h, vocab 30K, corpus 142M words / 1.9GB; MLM Top-1: UzBERT 64.06% vs mBERT 14.52% (news), 32.25% vs 14.33% (encyclopedia)
> **Relevance:** Confirms Uzbek in 2021 had ZERO labeled downstream benchmarks (a starker starting point than Kazakh, which already had some NER/sentiment sets by then) — the resource gap direction (Uzbek behind Kazakh at t=2021) reverses somewhat by 2024-26 per TUMLU exam-difficulty findings below.
> **Source:** arXiv:2108.09814 (fetched PDF text directly) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz] UzBERT paper explicitly documents Uzbek's dual-script reality: Cyrillic introduced 1956, Latin (re-)introduced 1995, both still coexist in real text; a dedicated ML-based Cyrillic-Latin-Cyrillic transliterator was built separately (Mansurov & Mansurov 2021, arXiv:2101.05162) precisely to bridge the script split for corpus building.
>
> **Numbers:** Cyrillic since 1956; Latin since 1995
> **Relevance:** Kazakh's Latin transition (~2031) is a future, planned, top-down event; Uzbek already lives the bi-script reality today and has a working transliteration tool as prior art the lab could adapt/cite when the kk Latin transition analysis is done.
> **Source:** arXiv:2108.09814 (fetched PDF text directly); arXiv:2101.05162 (cited, not independently fetched) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz] Uzbek agglutination is demonstrated in the UzBERT paper as unbounded suffix chaining (e.g. уйдагилар -> уйдагилардигилар -> уйдагилардигилардагилар, each adding suffix -дагилар), explicitly flagged by the authors as harder than what a plain WordPiece/BPE tokenizer captures (e.g. менинг is kept as one token instead of stem мен + suffix нинг).
>
> **Numbers:** n/a (qualitative, but load-bearing for tokenizer design)
> **Relevance:** Same morphology class as Kazakh (agglutinative Turkic); no modern (2024-26) Uzbek tokenizer fertility number was found anywhere in this sweep — a genuine measurement gap the lab could fill with a joint kk/uz fertility comparison in the survey.
> **Source:** arXiv:2108.09814 (fetched PDF text directly) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz] Historically (2021, arXiv:2108.09814): Uzbek Wikipedia was only ~12.2M words and 'suffers from low quality articles' (bulk-imported from a print encyclopedia with heavy abbreviation use); the CC-100 Uzbek subset used by XLM-R was only ~91M words. By the FineWeb2 era (2024+) Uzbek's combined web corpus reached ~1.109B words — roughly a 10x+ growth in available web text over ~3 years, but still ~40% smaller than Kazakh's FineWeb2 total.
>
> **Numbers:** 2021: uz Wikipedia 12.2M words, CC-100 uz ~91M words; 2024+: FineWeb2 uz ~1.109B words combined
> **Relevance:** Shows Uzbek's raw-data growth trajectory is fast but Uzbek still trails Kazakh in absolute FineWeb2 scale — useful trend line for the atlas's resource-ratio section.
> **Source:** arXiv:2108.09814 (2021 numbers, fetched PDF); web search aggregation (2024+ FineWeb2 numbers, not independently re-verified against primary FineWeb2 source) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [uz] Uzbek has a comparatively mature encoder-model ecosystem: UzBERT (2021, MIT license, outperforms mBERT on Uzbek MLM accuracy), UzRoBERTa (pretrained on ~2M Uzbek news articles), BERTbek (2024, Latin-script-focused, improves on UzBERT; BERTbek-News-Big reaches 92.25% F1 on sentiment, beating both mBERT and UzBERT), plus UzLiB (Uzbek Linguistic Benchmark, sourced from Telegram grammar-quiz channels, manually verified) from the Tahrirchi/uzlm commercial AI ecosystem.
>
> **Numbers:** BERTbek-News-Big sentiment F1 92.25%; UzRoBERTa ~2M news articles pretraining
> **Relevance:** Directly informs decision (1): despite CulturaX showing Uzbek with the LOWEST raw token count of the three (75.25M, likely undercounted), Uzbek has the MOST mature applied ecosystem (multiple BERT variants, a commercial AI company (Tahrirchi) actively building tools, its own linguistic benchmark) — resource maturity and raw corpus size diverge for Uzbek, unlike Kyrgyz where both are low. This supports prioritizing the live Uzbek collaboration for embedding-recipe porting on ecosystem-readiness grounds, not corpus-size grounds.
> **Source:** arXiv:2108.09814 (UzBERT); aclanthology.org/2024.sigul-1.5 (BERTbek); github.com/tahrirchi/uzlib; huggingface.co/uzlm · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-pan-models
> [uz] Uzbek has an active from-scratch monolingual model lineage (UzBERT 2021, UzRoBERTa 2023, BERTbek LREC-COLING-2024) that 'consistently outperformed multilingual models on downstream tasks like text classification and NER', plus a 2025 knowledge-distillation sentence-embedding effort described as 'the first study of its kind' for Uzbek, and SimRelUz (a word-level semantic similarity/relatedness benchmark).
>
> **Numbers:** [UNVERIFIED — exact benchmark deltas not extracted from primary source]
> **Relevance:** Uzbek already has monolingual BERT-family models AND a first embedding attempt — meaning the Uzbek collaboration offer would NOT be greenfield; the lab's Less-is-More recipe should be pitched as complementary (adapting mE5/EmbeddingGemma cheaply) rather than competing with from-scratch efforts.
> **Source:** arXiv:2108.09814 (UzBERT); BERTbek (LREC-COLING 2024 SIGUL workshop); SimRelUz benchmark (cited via search, not directly fetched) · **Sweep:** `turkic-landscape`

[[Home]]
