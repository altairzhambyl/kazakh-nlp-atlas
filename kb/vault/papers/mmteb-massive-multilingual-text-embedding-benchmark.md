---
kb_id: "arxiv:2502.13595"
type: "paper"
title: "MMTEB: Massive Multilingual Text Embedding Benchmark"
arxiv_id: "2502.13595"
doi: null
hf_repo: null
year: 2025
topics: ["embed-kazakh", "decoder-to-embedder", "mteb-upstream-kazqad-upstream-status", "turkic-pan-models"]
claims: 4
uncertain_claims: 0
verdicts: []
aliases: ["MMTEB: Massive Multilingual Text Embedding Benchmark", "arXiv:2502.13595", "arxiv:2502.13595"]
tags: ["paper", "topic/embed-kazakh", "topic/decoder-to-embedder", "topic/mteb-upstream-kazqad-upstream-status", "topic/turkic-pan-models"]
---
# MMTEB: Massive Multilingual Text Embedding Benchmark

[arXiv](https://arxiv.org/abs/2502.13595)
**Topics:** [[embed-kazakh]], [[decoder-to-embedder]], [[mteb-upstream-kazqad-upstream-status]], [[turkic-pan-models]]

> [!abstract]
> Text embeddings are typically evaluated on a limited set of tasks, which are constrained by language, domain, and task diversity. To address these limitations and provide a more comprehensive evaluation, we introduce the Massive Multilingual Text Embedding Benchmark (MMTEB) - a large-scale, community-driven expansion of MTEB, covering over 500 quality-controlled evaluation tasks across 250+ langua …

## Claims

> [!note] CLAIM — embed-kazakh
> MTEB/MMTEB contains NO dedicated Kazakh task: no Kazakh STS, no NLI/pair-classification, no reranking, no KazQAD, and MASSIVE (MassiveIntent/MassiveScenario) has no kk subset. Kazakh appears only inside multilingual tasks: BelebeleRetrieval (kaz_Cyrl), WebFAQRetrieval (kaz-Cyrl), SIB200Classification + SIB200ClusteringS2S (kaz_Cyrl), TurkicClassification (kk news), CyrillicTurkicLangClassification, and bitext-mining tasks (FLORES, NTREX, Tatoeba, WebFAQ).
>
> **Numbers:** grep of mteb main branch (July 2026): 13 task files mention kaz; 0 files mention KazQAD; 0 hits for kk in massive_intent_classification.py
> **Relevance:** The paper can claim 'first Kazakh-native MTEB benchmark suite' as a deliverable; every missing task type is a concrete milestone.
> **Source:** github.com/embeddings-benchmark/mteb (cloned & grepped 2026-07-03); MMTEB arXiv:2502.13595 · **Sweep:** `embeddings-2026-07`

> [!note] CLAIM — decoder-to-embedder
> Kazakh is essentially ABSENT from MTEB/MMTEB as a first-class language: a code search of the mteb repository finds no KazQAD task and no Kazakh-native retrieval/STS/reranking task — Kazakh appears only via multilingual spillover (SIB-200 classification/clustering, FLEURS, Common Voice, Tatoeba bitext, WebFAQ, Turkic/Cyrillic-Turkic language-ID classification). There is no Kazakh STS dataset at all (SemRel2024's 14 languages exclude Kazakh; no KazSTS exists).
>
> **Numbers:** 0 Kazakh-native retrieval, STS, or reranking tasks in mteb as of 2026-07.
> **Relevance:** THE critical bottleneck: 'best Kazakh embedder' is currently unfalsifiable. Building kkMTEB is a mandatory milestone and a citable contribution in itself.
> **Source:** gh code search of github.com/embeddings-benchmark/mteb (kaz-Cyrl, KazQAD); arXiv 2502.13595 (MMTEB); arXiv 2402.08638 (SemRel2024) · **Sweep:** `embeddings-2026-07`

> [!note] CLAIM — mteb-upstream-kazqad-upstream-status
> The MMTEB paper (arXiv:2502.13595) itself, as fetched, contains no explicit mention of 'Kazakh', 'kaz', 'kk', KazQAD, ISSAI, or a Turkic/Central Asian task grouping in the sections retrievable via WebFetch.
> **Source:** https://arxiv.org/abs/2502.13595 and https://arxiv.org/html/2502.13595v2 (fetched via WebFetch) · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — turkic-pan-models
> [pan-turkic][kk] MMTEB/MTEB (KB, re-confirmed) has NO dedicated Kazakh, Uzbek, Kyrgyz, Azerbaijani, Tatar, or any other Turkic-language-native STS/retrieval/reranking task; Turkic languages appear only via multilingual spillover tasks (SIB-200, BelebeleRetrieval, WebFAQRetrieval, FLORES/NTREX/Tatoeba bitext, TurkicClassification, CyrillicTurkicLangClassification). TR-MTEB (Turkish-only, 26 datasets) is the ONLY native-language MTEB-style benchmark that exists for any Turkic language.
>
> **Numbers:** 0 native Turkic-language MTEB tasks except Turkish's separate TR-MTEB (26 datasets, 6 task types)
> **Relevance:** Directly answers decision (3): a pan-Turkic MTEB extension (kk-MTEB + uz-MTEB + ky-MTEB etc., unified under one leaderboard) is genuinely unclaimed territory — Turkish solved this alone via a standalone benchmark, no one has done it family-wide. This is the single clearest 'unclaimed pan-Turkic artifact' finding of the sweep, directly actionable for the lab's planned kk-MTEB upstream PR (project CLAUDE.md).
> **Source:** KB (arXiv:2502.13595 MMTEB) + this sweep's TR-MTEB findings (2025.findings-emnlp.471) · **Sweep:** `turkic-landscape`

## Related
- [[kazqad-kazakh-open-domain-question-answering-dataset|KazQAD: Kazakh Open-Domain Question Answering Dataset]] — KazQAD is NOT integrated into MMTEB — the retrieval gap the lab's kkMTEB upstream PR is meant to fill
- [[afrimteb-and-afrie5-benchmarking-and-adapting-text-embedding-models-for-african|AfriMTEB and AfriE5: Benchmarking and Adapting Text Embedding Models for African Languages]] — AfriMTEB is the regional-MTEB template proving a kk-MTEB is buildable; MMTEB itself currently has zero native kk tasks
- [[huggingface-co-datasets-mteb-webfaqretrieval|huggingface.co/datasets/mteb/WebFAQRetrieval]] — WebFAQRetrieval is an MMTEB task; MMTEB is the benchmark whose kaz coverage is too thin for a headline eval

[[Home]]
