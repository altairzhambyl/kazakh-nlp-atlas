---
kb_id: "title:mteb abstasks retrieval py 690 739 in embeddings benchmark mteb 2 16 3"
type: "source"
title: "mteb/abstasks/retrieval.py:690-739 in embeddings-benchmark/mteb@2.16.3…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb abstasks retrieval py 690 739 in embeddings benchmark mteb 2 16 3"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/abstasks/retrieval.py:690-739 in embeddings-benchmark/mteb@2.16.3…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/abstasks/retrieval.py:690-739 in embeddings-benchmark/mteb@2.16.3 (

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> A retrieval task can be converted, at runtime, into a reranking-style evaluation from a previous model's saved predictions via `AbsTaskRetrieval.convert_to_reranking(top_ranked_path, top_k=10)`, which loads a JSON of a prior run's per-query scored candidates and truncates to top_k per query — an alternative to pre-baking a static top_ranked column into the HF dataset.
> **Source:** mteb/abstasks/retrieval.py:690-739 in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/abstasks/retrieval.py) · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
