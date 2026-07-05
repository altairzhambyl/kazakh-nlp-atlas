---
kb_id: "title:mteb abstasks retrieval dataset loaders py 79 249 in embeddings benchmark mteb 2 16 3"
type: "source"
title: "mteb/abstasks/retrieval_dataset_loaders.py:79-249 in embeddings-benchm…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb abstasks retrieval dataset loaders py 79 249 in embeddings benchmark mteb 2 16 3"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/abstasks/retrieval_dataset_loaders.py:79-249 in embeddings-benchm…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/abstasks/retrieval_dataset_loaders.py:79-249 in embeddings-benchmark/mteb@2.16.3 (

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> `RetrievalDatasetLoader` expects the HF dataset repo to expose specific HF 'config' names it auto-discovers via get_dataset_config_names: `{subset}-corpus` (or plain `corpus` for non-multilingual), `{subset}-queries` (or `queries`), a qrels config (`qrels` if not subset-specific), and OPTIONALLY `{subset}-top_ranked` (or plain `top_ranked`) which, if present, is loaded and used to populate the RetrievalSplitData's `top_ranked` field for reranking-style evaluation.
> **Source:** mteb/abstasks/retrieval_dataset_loaders.py:79-249 in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/abstasks/retrieval_dataset_loaders.py) · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
