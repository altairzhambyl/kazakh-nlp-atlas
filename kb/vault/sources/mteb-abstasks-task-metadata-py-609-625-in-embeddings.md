---
kb_id: "title:mteb abstasks task metadata py 609 625 in embeddings benchmark mteb 2 16 3 example file mteb descriptive stats retrieval rubqretrieval json"
type: "source"
title: "mteb/abstasks/task_metadata.py:609-625 in embeddings-benchmark/mteb@2.…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:mteb abstasks task metadata py 609 625 in embeddings benchmark mteb 2 16 3 example file mteb descriptive stats retrieval rubqretrieval json"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# mteb/abstasks/task_metadata.py:609-625 in embeddings-benchmark/mteb@2.…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- mteb/abstasks/task_metadata.py:609-625 in embeddings-benchmark/mteb@2.16.3 (  example file mteb/descriptive_stats/Retrieval/RuBQRetrieval.json

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> There is NO `descriptive_stats` (or `n_samples`) field passed into `TaskMetadata(...)` at all in current mteb — this is a change from older mteb versions. Instead `descriptive_stats` and `n_samples` are read-only `@property`s that lazily load a separate auto-generated JSON file at `mteb/descriptive_stats/{TaskType}/{TaskName}.json` (or under an `Image/` subfolder for MIEB task types). The JSON is produced by calling `task.calculate_descriptive_statistics()` on an instantiated, loaded task, which writes stats per split (num_samples, character-length stats for docs/queries, relevant_docs_statistics, top_ranked_statistics, num_documents, num_queries).
> **Source:** mteb/abstasks/task_metadata.py:609-625 in embeddings-benchmark/mteb@2.16.3 (https://github.com/embeddings-benchmark/mteb/blob/2.16.3/mteb/abstasks/task_metadata.py); example file mteb/descriptive_stats/Retrieval/RuBQRetrieval.json · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
