---
kb_id: "arxiv:2506.20920"
type: "paper"
title: "FineWeb2: One Pipeline to Scale Them All -- Adapting Pre-Training Data Processing to Every Language"
arxiv_id: "2506.20920"
doi: null
hf_repo: null
year: 2025
topics: ["data-efficiency-10b-kazakh-10b-token-pre", "turkic-nlp-landscape-uzbek-monolingual-p", "non-kazakh-turkic-nlp-landscape-reconcil"]
claims: 4
uncertain_claims: 1
verdicts: []
aliases: ["FineWeb2: One Pipeline to Scale Them All -- Adapting Pre-Training Data Processing to Every Language", "arXiv:2506.20920", "arxiv:2506.20920"]
tags: ["paper", "topic/data-efficiency-10b-kazakh-10b-token-pre", "topic/turkic-nlp-landscape-uzbek-monolingual-p", "topic/non-kazakh-turkic-nlp-landscape-reconcil"]
---
# FineWeb2: One Pipeline to Scale Them All -- Adapting Pre-Training Data Processing to Every Language

[arXiv](https://arxiv.org/abs/2506.20920)
**Topics:** [[data-efficiency-10b-kazakh-10b-token-pre]], [[turkic-nlp-landscape-uzbek-monolingual-p]], [[non-kazakh-turkic-nlp-landscape-reconcil]]

> [!abstract]
> Pre-training state-of-the-art large language models (LLMs) requires vast amounts of clean and diverse text data. While the open development of large high-quality English pre-training datasets has seen substantial recent progress, training performant multilingual LLMs remains a challenge, in large part due to the inherent difficulty of tailoring filtering and deduplication pipelines to a large numb …

## Claims

> [!note] CLAIM — data-efficiency-10b-kazakh-10b-token-pre
> FineWeb-2 uses per-language dedup with 'rehydration': it keeps one doc per MinHash cluster but stores minhash_cluster_size, then UPSAMPLES documents by cluster size (per-language weights tuned to each language's cluster-filtering rate) rather than discarding duplicates — shown to improve downstream performance over both keep-all and drop-all-duplicates.
>
> **Numbers:** FineWeb-2: ~20TB/5B docs/1000+ langs; per-language MinHash dedup + cluster-size rehydration/upsampling
> **Relevance:** transferable-untested at Kazakh scale. Concrete upgrade over SozKZ's MD5-exact dedup: adopt MinHash + cluster-size rehydration for the kk pool so the highest-cluster (most-duplicated, often canonical/clean) docs are upsampled — a principled alternative to blind Wikipedia 3x/multidomain 2x upsampling in the KB.
> **Source:** arXiv:2506.20920 (FineWeb2) + HF fineweb-2 README (minhash_cluster_size field, rehydration code on GitHub) · **Sweep:** `slm-arch-for-kazakh`

> [!warning] UNCERTAIN — data-efficiency-10b-kazakh-10b-token-pre
> FineWeb2 (single multilingual pipeline) is reported to outperform CC-100, mC4, CulturaX and HPLT on downstream evals across languages while being substantially larger, and CulturaX<->FineWeb-2 share the most cross-corpus duplication (25.8B tokens overlap globally; C4<->CulturaX 25.5B).
>
> **Numbers:** CulturaX∩FineWeb-2 = 25.8B tok overlap (global); FineWeb2 > CulturaX/HPLT/mC4 on downstream (per-language ablations)
> **Relevance:** transferable-untested for kk specifically. Justifies making FineWeb-2 kk the QUALITY-primary web source and treating CulturaX kk as largely redundant with it (heavy overlap) — dedup CulturaX AGAINST FineWeb-2 rather than adding both naively.
> **Source:** arXiv:2506.20920 (FineWeb2) / HF FineWeb2 card / MarkTechPost summary · **Sweep:** `slm-arch-for-kazakh`

> [!note] CLAIM — turkic-nlp-landscape-uzbek-monolingual-p
> [uz][kk] FineWeb2 (2025, 96 CommonCrawl snapshots 2013-2024, per-language-tuned filtering+global dedup) is the largest and most current CC-derived source, and gives EXACT per-script counts: uzn_Latn train = 687,002,994 words / 1,233,463 docs / 4.45GB raw text (1.90GB parquet); uzn_Cyrl train = 544,866,919 words / 1,357,811 docs / 6.12GB raw text (1.83GB parquet). Combined both scripts = 1,231,869,913 words (~1.23B) / 2,591,274 docs / 10.57GB text — this is the true source of the '~1.109B' figure in the question (a rounding/earlier-commit variant of the current combined-script sum, or possibly Latin-only-plus-test).
>
> **Numbers:** uzn_Latn train: 687,002,994 words, 1,233,463 docs, 4.45GB text, 1.90GB parquet. uzn_Cyrl train: 544,866,919 words, 1,357,811 docs, 6.12GB text, 1.83GB parquet. Combined: ~1.232B words / 2.59M docs / 10.57GB.
> **Relevance:** This is the number the lab should treat as ground truth for 'realistic Uzbek web-text budget' if porting the FineWeb2/pinned-protocol pipeline — reported 'words' (whitespace tokens), NOT subword/BPE tokens, so expect ~1.2-1.6x more actual training tokens after tokenization (not directly measured for Uzbek; flagged uncertain by extrapolation only).
> **Source:** Penedo et al. 2025, 'FineWeb2: One Pipeline to Scale Them All', arXiv:2506.20920; official per-language CSV github.com/huggingface/fineweb-2/blob/main/fineweb2-language-distribution.csv (fetched raw, rows for uzn_Latn/uzn_Cyrl train+test+removed); dataset ODC-By license · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-reconcil
> [az][kk][uz][ky][tt][ba][tk][cv][sah][uig][kaa] On FineWeb-2 (HuggingFaceFW/fineweb-2, built from ~100 Common Crawl snapshots spanning summer 2013 to April 2024 — a far more current and better-deduplicated corpus than CC-100), Azerbaijani (azj_Latn + azj_Cyrl combined) has 7,320,970 documents / 11.31 GB, vs Kazakh (kaz_Cyrl) 3,375,998 documents / 6.86 GB — Azerbaijani leads by 2.17x docs / 1.65x bytes, essentially confirming the CC-100-era ratio persists in a 2024-snapshot corpus. Other Turkic figures (docs/GB): Uzbek uzn_Latn+uzn_Cyrl combined = 2,618,356 docs/4.05 GB (SMALLER than Kazakh alone despite ~2.7x Kazakh's population); Kyrgyz kir_Cyrl 1,079,913/1.48 GB; Tatar tat_Cyrl 163,098/0.52 GB; Bashkir bak_Cyrl 185,008/0.29 GB; Turkmen tuk_Latn 240,424/0.31 GB; Chuvash chv_Cyrl 82,246/0.14 GB; Sakha sah_Cyrl 73,475/0.16 GB; Uyghur uig_Arab 167,459/0.33 GB; Karakalpak kaa_Cyrl+kaa_Latn 14,214/0.019 GB (near-zero — confirms Karakalpak is web-absent).
>
> **Numbers:** az(combined) 7.32M docs/11.31GB; kk 3.38M docs/6.86GB; uz(combined) 2.62M docs/4.05GB; ky 1.08M/1.48GB; tt 0.16M/0.52GB; ba 0.19M/0.29GB; tk 0.24M/0.31GB; cv 82K/0.14GB; sah 73K/0.16GB; ug 167K/0.33GB; kaa 14K/0.019GB
> **Relevance:** This is the current (2024-snapshot) reconciliation of the raw-web-volume axis, independently confirming CC-100's direction with a fresh source — Azerbaijani beats Kazakh by a stable ~1.6-2.2x margin across two independently-built corpora six years apart, so this is not a stale-data artifact.
> **Source:** HuggingFace datasets-server /size endpoint queried live against HuggingFaceFW/fineweb-2 per-config, cross-checked with Penedo et al. 2025 'FineWeb2: One Pipeline to Scale Them All' (arXiv:2506.20920) for corpus methodology. · **Sweep:** `turkic-landscape`

## Related
- [[an-expanded-massive-multilingual-dataset-for-high-performance-language|An Expanded Massive Multilingual Dataset for High-Performance Language Technologies (HPLT)]] — FineWeb2 reports outperforming HPLT/CulturaX downstream and adds per-language rehydration over HPLT's raw Kazakh counts
- [[hplt-3-0-very-large-scale-multilingual-resources-for-llms-and-mt-mono-and-bi|HPLT 3.0: Very Large-Scale Multilingual Resources for LLMs and MT. Mono- and Bi-lingual Da…]] — Overlapping Kazakh web corpora: HPLT notes heavy dedup overlap with FineWeb-2, so naive concatenation double-counts tokens
- [[estllm-enhancing-estonian-capabilities-in-multilingual-llms-via-continued|EstLLM: Enhancing Estonian Capabilities in Multilingual LLMs via Continued Pretraining and…]] — EstLLM refutes FineWeb-2 quality for discriminative tasks — found it full of machine-translated spam by inspection
- [[wiki-apertium-org-wiki-apertium-kaz-apertium-kaz-transducer|wiki.apertium.org/wiki/Apertium-kaz (apertium-kaz transducer stats pag…]] — apertium-kaz FST coverage drops on Wikipedia and is untested on FineWeb2-style crawl — the very noisy pipeline QymyzLM would ingest

[[Home]]
