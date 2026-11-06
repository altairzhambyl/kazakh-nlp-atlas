---
kb_id: "title:github com localdoc azerbaijan sts benchmark readme fetched via webfetch"
type: "source"
title: "github.com/LocalDoc-Azerbaijan/STS-Benchmark (README, fetched via WebF…"
doi: null
hf_repo: null
year: null
topics: ["turkic-embeddings-retrieval-non-kazakh-t"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["title:github com localdoc azerbaijan sts benchmark readme fetched via webfetch"]
tags: ["source", "topic/turkic-embeddings-retrieval-non-kazakh-t"]
---
# github.com/LocalDoc-Azerbaijan/STS-Benchmark (README, fetched via WebF…

**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]]

## Source URLs
- github.com/LocalDoc-Azerbaijan/STS-Benchmark (README, fetched via WebFetch)

## Findings

> [!warning] UNCERTAIN — turkic-embeddings-retrieval-non-kazakh-t
> [az] LocalDoc-Azerbaijan/STS-Benchmark (GitHub, LocalDoc AI) benchmarks Azerbaijani-adapted SICK-R + STS12/13/15/16 sets against multilingual encoders. Result INVERTS the usual scaling trend: multilingual-e5-SMALL scores HIGHEST average Pearson (0.7577), beating e5-large-instruct (0.7280), e5-base (0.7242), and e5-large (0.6960) — the largest mE5 variant is the WORST of the four on Azerbaijani STS. Models evaluated: LaBSE, ColBERT-XM, all four mE5 sizes, BGE-M3 (exact BGE-M3 score not extracted). Also LocalDoc/az-en-MiniLM-L6-v2 (a small bilingual az-en model) is reported competitive with/exceeding larger multilingual models on this same benchmark.
>
> **Numbers:** mE5-small 0.7577; mE5-large-instruct 0.7280; mE5-base 0.7242; mE5-large 0.6960 (avg Pearson across SICK-R+STS12/13/15/16-az)
> **Relevance:** A dedicated native Azerbaijani STS test set already exists (unlike Uzbek/Kyrgyz), making Azerbaijani a fast, low-infrastructure-cost second target for the lab's evallab protocols. The large-vs-small inversion is a red flag worth independently re-verifying (possible overfitting/noise/leakage in the small mE5 checkpoint or a broken large-model eval) before quoting — evallab should re-run this under its own pinned protocol rather than trust the GitHub number as-is.
> **Source:** github.com/LocalDoc-Azerbaijan/STS-Benchmark (README, fetched via WebFetch) · **Sweep:** `turkic-landscape`

[[Home]]
