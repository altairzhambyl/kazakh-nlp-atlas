---
kb_id: "title:mteb abstasks retrieval py 228 277 in embeddings benchmark mteb 2 16 3"
type: "source"
title: "mteb/abstasks/retrieval.py:228-277 in embeddings-benchmark/mteb@2.16.3…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb abstasks retrieval py 228 277 in embeddings benchmark mteb 2 16 3"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/abstasks/retrieval.py:228-277 in embeddings-benchmark/mteb@2.16.3…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/abstasks/retrieval.py:228-277 in embeddings-benchmark/mteb@2.16.3 (

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> `AbsTaskRetrieval.load_data()` reads `self.metadata.dataset['path']`, `['revision']`, and optional `.get('trust_remote_code', False)`, then for each eval split (and each hf_subset if multilingual) instantiates `RetrievalDatasetLoader(hf_repo=..., revision=..., trust_remote_code=..., split=..., config=hf_subset).load(num_proc=...)`, storing results in `self.dataset[hf_subset][split]` as a `RetrievalSplitData`. Finally it calls `self.dataset_transform()` and sets `self.data_loaded = True`.
> **Source:** mteb/abstasks/retrieval.py:228-277 in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/abstasks/retrieval.py) · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
