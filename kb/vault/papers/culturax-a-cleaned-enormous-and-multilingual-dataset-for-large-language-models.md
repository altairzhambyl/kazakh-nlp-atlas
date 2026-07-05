---
kb_id: "arxiv:2309.09400"
type: "paper"
title: "CulturaX: A Cleaned, Enormous, and Multilingual Dataset for Large Language Models in 167 Languages"
arxiv_id: "2309.09400"
doi: null
hf_repo: "uonlp/CulturaX"
year: 2023
topics: ["turkic-turkish", "turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-nlp-landscape-uzbek-monolingual-p"]
claims: 3
uncertain_claims: 1
verdicts: []
aliases: ["CulturaX: A Cleaned, Enormous, and Multilingual Dataset for Large Language Models in 167 Languages", "arXiv:2309.09400", "arxiv:2309.09400"]
tags: ["paper", "topic/turkic-turkish", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-nlp-landscape-uzbek-monolingual-p"]
---
# CulturaX: A Cleaned, Enormous, and Multilingual Dataset for Large Language Models in 167 Languages

[arXiv](https://arxiv.org/abs/2309.09400)
**Topics:** [[turkic-turkish]], [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-nlp-landscape-uzbek-monolingual-p]]

> [!abstract]
> The driving factors behind the development of large language models (LLMs) with impressive learning capabilities are their colossal model sizes and extensive training datasets. Along with the progress in natural language processing, LLMs have been frequently made accessible to the public to foster deeper investigation and applications. However, when it comes to training datasets for these LLMs, es …

## Claims

> [!note] CLAIM — turkic-turkish
> CulturaX's per-language token counts give an exact, checkable resource ratio across the whole Turkic family: [tr] Turkish 64.29B tokens (94.2M docs, 1.02% of the 6.3T-token corpus); [kk] Kazakh 2.80B tokens (2.73M docs, 0.04%); [az] Azerbaijani 3.51B tokens (5.08M docs, 0.06%); [ky] Kyrgyz 501M tokens (0.01%); [ug] Uyghur 77.7M tokens; [uz] Uzbek 75.25M tokens (only 87K docs) — Uzbek is the most under-represented major Turkic language in CulturaX despite ~35M speakers. Turkish is ~23x larger than Kazakh, ~854x larger than Uzbek, ~128x larger than Kyrgyz, ~828x larger than Uyghur in this specific corpus.
>
> **Numbers:** tr 64.29B tok; kk 2.80B tok; az 3.51B tok; ky 501M tok; ug 77.7M tok; uz 75.25M tok (tt/ba/tk/cv/sah lack published token counts, only doc counts: tt 218K docs, ba 72K, tk 14K, cv 22.6K, sah 22.1K)
> **Relevance:** Directly answers decision (2)/resource ratios; flags that Uzbek — the language with a live collaboration offer — is WORSE off than Kazakh in raw web-corpus terms (0.04% vs far under 0.01%), so an Uzbek port cannot assume Kazakh-level pretraining data availability.
> **Source:** huggingface.co/datasets/uonlp/CulturaX (per-language stats table); arXiv:2309.09400 · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [kk][ky][uz] CulturaX per-language token counts for the three Central Asian languages: Kazakh 2,802,485,195 tokens (2,733,982 docs); Kyrgyz 501,442,620 tokens (570,922 docs); Uzbek 75,250,787 tokens (87,219 docs) — i.e. Kazakh has 5.6x Kyrgyz's tokens and 37.2x Uzbek's, in this specific corpus.
>
> **Numbers:** kk 2.80B tok / 2.73M docs; ky 501M tok / 571K docs; uz 75.25M tok / 87.2K docs; kk:ky ratio 5.6x; kk:uz ratio 37.2x
> **Relevance:** Quantifies decision (2) — Kazakh sits clearly ahead of Kyrgyz and (surprisingly) of Uzbek in this specific web-crawl corpus, giving the atlas a concrete resource-ratio number. BUT the Uzbek figure is suspiciously low given Uzbekistan's 34M population and should be checked for script-code artifacts (CulturaX may register only one script variant under 'uz').
> **Source:** huggingface.co/datasets/uonlp/CulturaX language table (arXiv:2309.09400) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-uzbek-monolingual-p
> [uz] CulturaX's Uzbek slice is the smallest of the four candidates: 75,250,787 tokens across 87,219 documents, per the dataset's own per-language statistics table.
>
> **Numbers:** 75,250,787 tokens; 87,219 documents; built from mC4 v3.1.0 + OSCAR 20.19/21.09/22.01/23.01 union with cross-source dedup
> **Relevance:** This is the number an engineer gets by default if they just `datasets.load_dataset('uonlp/CulturaX','uz')` — using it as 'true Uzbek data availability' massively understates reality by 9-16x vs the other sources below; it reflects CulturaX's specific (heavy) dedup/union choices, not raw web availability.
> **Source:** HF dataset card uonlp/CulturaX (README.md language stats table); paper arXiv:2309.09400 (Nguyen et al., CulturaX, LREC-COLING 2024) · **Sweep:** `turkic-landscape`

[[Home]]
