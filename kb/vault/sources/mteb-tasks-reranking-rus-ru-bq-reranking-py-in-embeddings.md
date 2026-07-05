---
kb_id: "title:mteb tasks reranking rus ru bq reranking py in embeddings benchmark mteb 2 16 3"
type: "source"
title: "mteb/tasks/reranking/rus/ru_bq_reranking.py in embeddings-benchmark/mt…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb tasks reranking rus ru bq reranking py in embeddings benchmark mteb 2 16 3"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/tasks/reranking/rus/ru_bq_reranking.py in embeddings-benchmark/mt…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/tasks/reranking/rus/ru_bq_reranking.py in embeddings-benchmark/mteb@2.16.3 (

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> There is no separate, non-deprecated `AbsTaskReranking` base class anymore. All modern reranking tasks (and all modern retrieval tasks) subclass `AbsTaskRetrieval` directly; `type="Reranking"` in TaskMetadata is what distinguishes them, not the Python base class.
> **Source:** mteb/tasks/reranking/rus/ru_bq_reranking.py in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/tasks/reranking/rus/ru_bq_reranking.py) · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
