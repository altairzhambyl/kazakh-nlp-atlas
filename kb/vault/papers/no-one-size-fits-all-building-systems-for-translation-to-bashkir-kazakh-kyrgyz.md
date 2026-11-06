---
kb_id: "arxiv:2602.04442"
type: "paper"
title: "No One-Size-Fits-All: Building Systems For Translation to Bashkir, Kazakh, Kyrgyz, Tatar and Chuvash Using Synthetic And Original Data"
arxiv_id: "2602.04442"
doi: null
hf_repo: null
year: 2026
topics: ["turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-benchmarks-non-kazakh-turkic", "non-kazakh-turkic-nlp-landscape-prior-ar"]
claims: 6
uncertain_claims: 3
verdicts: []
aliases: ["No One-Size-Fits-All: Building Systems For Translation to Bashkir, Kazakh, Kyrgyz, Tatar and Chuvash Using Synthetic And Original Data", "arXiv:2602.04442", "arxiv:2602.04442"]
tags: ["paper", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-benchmarks-non-kazakh-turkic", "topic/non-kazakh-turkic-nlp-landscape-prior-ar"]
---
# No One-Size-Fits-All: Building Systems For Translation to Bashkir, Kazakh, Kyrgyz, Tatar and Chuvash Using Synthetic And Original Data

[arXiv](https://arxiv.org/abs/2602.04442)
**Topics:** [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-benchmarks-non-kazakh-turkic]], [[non-kazakh-turkic-nlp-landscape-prior-ar]]

> [!abstract]
> We explore machine translation for five Turkic language pairs: Russian-Bashkir, Russian-Kazakh, Russian-Kyrgyz, English-Tatar, English-Chuvash. Fine-tuning nllb-200-distilled-600M with LoRA on synthetic data achieved chrF++ 49.71 for Kazakh and 46.94 for Bashkir. Prompting DeepSeek-V3.2 with retrieved similar examples achieved chrF++ 39.47 for Chuvash. For Tatar, zero-shot or retrieval-based appro …

## Claims

> [!note] CLAIM — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [kk][ky][ba] In a 2026 Turkic MT shared-task paper, ORIGINAL (non-synthetic) parallel training data sizes were: Russian-Kazakh 367,095 samples, Russian-Kyrgyz 35,429 samples, Russian-Bashkir 1,190,773 samples — i.e. Kazakh has 10.4x more original RU-parallel data than Kyrgyz, and Bashkir (a non-state, autonomous-republic language) has 33.6x more than Kyrgyz and 3.2x more than Kazakh.
>
> **Numbers:** ru-kk 367,095 train / 9,845 val; ru-ky 35,429 train / 4,845 val; ru-ba 1,190,773 train / 9,997 val; kk:ky ratio 10.4x
> **Relevance:** Gives a second, independent-of-CulturaX resource-ratio datapoint (parallel-corpus axis rather than monolingual-web axis) confirming Kazakh's mid-tier lead over Kyrgyz among Kipchak Turkic languages — useful cross-check for the atlas's 'who is ahead on what axis' table.
> **Source:** arXiv:2602.04442 (Karpov, 'No One-Size-Fits-All', Feb 2026) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [kk][ky][ba][tt][cv] Same paper: for the better-resourced languages (Kazakh, Bashkir) fine-tuning NLLB-200-distilled-600M with LoRA/DoRA beat zero-shot LLM prompting (Kazakh chrF++ 49.93 LoRA vs 47.54 best zero-shot MiMoV2; Bashkir 49.53 LoRA vs 41.59 zero-shot). For Kyrgyz, the pattern INVERTS: zero-shot LLM prompting (MiMoV2 46.61, submitted result 45.61 chrF++) beat NLLB fine-tuning (LoRA only 36.29, single-task fine-tune 27.04) — fine-tuning on Kyrgyz's smaller pretraining allocation could not catch up to a frontier LLM's zero-shot multilingual knowledge.
>
> **Numbers:** Kazakh: LoRA 49.93 > zero-shot best 47.54; Bashkir: LoRA 49.53 > zero-shot 41.59. Kyrgyz: LoRA 36.29 < zero-shot MiMoV2 46.61 (final submission chrF++ 45.61)
> **Relevance:** Signals a resource-crossover threshold: below some pretraining-data floor, adapting a dedicated MT model underperforms just prompting a frontier LLM — evidence that Kyrgyz sits below that floor while Kazakh sits above it. Relevant when the lab decides whether a from-scratch/continual-PT strategy is even worth it for a target language before porting the recipe.
> **Source:** arXiv:2602.04442, Table 1 & Table 2 · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [kk][ky] LaBSE nominally supports both Kazakh and Kyrgyz, but the same paper notes that stacking translations by LaBSE cosine-similarity 'led to a minor deterioration' and cites prior work that 'the quality of the multilingual BERT on any given language is strongly correlated with the size of the pretraining data' — i.e. LaBSE's Kyrgyz embeddings are lower-fidelity than its Kazakh embeddings purely due to pretraining-data imbalance, not architecture.
>
> **Numbers:** qualitative; LaBSE-based reranking underperformed single-model baseline for both kk and ky [UNVERIFIED exact delta]
> **Relevance:** Warns that reusing an off-the-shelf multilingual embedder (LaBSE, mE5, BGE-M3) for a Kyrgyz-analog retrieval eval will likely show a bigger multilingual-vs-dedicated gap than the lab already measured for Kazakh (mE5-large on KazQAD), because Kyrgyz's pretraining allocation in these encoders is smaller still.
> **Source:** arXiv:2602.04442, Section 6 (citing Karpov & Burtsev 2023) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-other-langs-non-kazakh-turkic-nlp
> [ba][cv][kaz] 'No One-Size-Fits-All' (arXiv:2602.04442) trains MT systems (LoRA/DoRA + 8-bit quant, DeepSeek/Gemma/mGPT bases) for Bashkir, Kazakh, Kyrgyz, Tatar, Chuvash and reports chrF++ scores that rank Kazakh transfer BEST and Chuvash WORST of the three languages with numbers surfaced: Kazakh 49.71, Bashkir 46.94, Chuvash 39.47. Chuvash is the outlier as the sole Oghur-branch language in the set (vs the other four's Kipchak branch), consistent with genetic distance — not just resource size — mattering for MT transfer specifically (unlike KB's byte-premium finding for knowledge tasks).
>
> **Numbers:** chrF++: Kazakh 49.71, Bashkir 46.94, Chuvash 39.47 (Russian-X pairs)
> **Relevance:** Decision (2): gives one more sourced axis (MT transfer quality) where Kazakh leads its Kipchak/Oghur neighbors, and flags Chuvash as the family's genetic outlier — relevant if the atlas wants a 'who transfers best' ranking distinct from the TUMLU knowledge-QA ranking.
> **Source:** arXiv:2602.04442 (fetched, partial extraction — exact per-language corpus sizes were embedded in unreadable PDF streams) + web search snippet corroboration · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> A 5-language MT resource-tier study (Bashkir, Kazakh, Kyrgyz, Tatar, Chuvash) [ba][kk][ky][tt][cv] found original parallel-data sizes vary by >30x: Russian-Bashkir 1,190,773 pairs, Russian-Kazakh 367,095, Russian-Kyrgyz 35,429, English-Tatar 106,777, English-Chuvash 193,826. Best chrF++ after LoRA fine-tuning + synthetic back-translation augmentation (to 2,457,344 pairs/language): Kazakh 49.71, Bashkir 46.94, Kyrgyz 45.6 (zero-shot), Tatar 41.6, Chuvash 39.47 (worst, base model wasn't even pretrained on Chuvash).
>
> **Numbers:** chrF++: kk 49.71 > ba 46.94 > ky 45.6 > tt 41.6 > cv 39.47; original pairs ba 1.19M > cv 193.8K > tt 106.8K > kk 367.1K(!) > ky 35.4K
> **Relevance:** Counter-intuitive resource/performance mismatch: Bashkir has MORE raw parallel data than Kazakh (1.19M vs 367K pairs) yet still trails Kazakh on final chrF++ (46.94 vs 49.71), suggesting Kazakh benefits from stronger base-model language coverage, not just data volume — relevant caveat for the atlas's resource-ratio claims (raw corpus size alone doesn't predict downstream Turkic NLP quality).
> **Source:** arXiv:2602.04442 (No One-Size-Fits-All: Building Systems For Translation to Bashkir, Kazakh, Kyrgyz, Tatar and Chuvash Using Synthetic And Original Data) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — non-kazakh-turkic-nlp-landscape-prior-ar
> [kk][ky][tt][ba][cv] A February 2026 machine-translation paper, 'No One-Size-Fits-All: Building Systems For Translation to Bashkir, Kazakh, Kyrgyz, Tatar and Chuvash Using Synthetic And Original Data' (arXiv:2602.04442, Kunafin & Shakirov), builds translation systems (tested with DeepSeek-V3.2, MiMoV2, Gemma3) across five Kipchak/Turkic languages including Kazakh -- but this is an MT paper, not an embedding paper, and does not build or claim any retrieval/embedding benchmark.
>
> **Numbers:** 5 languages: ba, kk, ky, tt, cv; models used: DeepSeek-V3.2, MiMoV2, Gemma3
> **Relevance:** Relevant to Decision 1 only as a potential source of fresh parallel-corpus/synthetic-data infrastructure across Kipchak Turkic languages (useful for building the KD teacher-student pairs the Less-is-More recipe needs) -- it is NOT competing embedding prior art and does not affect the novelty claim.
> **Source:** arXiv:2602.04442 (search snippet; abstract page) · **Sweep:** `turkic-landscape`

[[Home]]
