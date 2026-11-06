---
kb_id: "title:directory listing of embeddings benchmark mteb 2 16 3 mteb tasks retrieval and mteb tasks reranking and local find returned no kaz named files"
type: "source"
title: "directory listing of embeddings-benchmark/mteb@2.16.3 mteb/tasks/retri…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-task-api"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:directory listing of embeddings benchmark mteb 2 16 3 mteb tasks retrieval and mteb tasks reranking and local find returned no kaz named files"]
tags: ["source", "topic/mteb-upstream-task-api"]
---
# directory listing of embeddings-benchmark/mteb@2.16.3 mteb/tasks/retri…

**Topics:** [[mteb-upstream-task-api]]

## Source URLs
- directory listing of embeddings-benchmark/mteb@2.16.3 mteb/tasks/retrieval/ and mteb/tasks/reranking/ (  and   local `find` returned no kaz-named files

## Findings

> [!note] CLAIM — mteb-upstream-task-api
> Retrieval tasks live at mteb/tasks/retrieval/<iso639-3-lang-or-'multilingual'>/*.py (e.g. eng/, rus/, ara/, code/, dan/, deu/...), and reranking tasks live in the sibling tree mteb/tasks/reranking/<lang>/*.py, but reranking task Python classes still subclass AbsTaskRetrieval (see finding above) — the directory split (retrieval/ vs reranking/) is purely organizational, not a base-class split. There is currently NO Kazakh (kaz) directory or task file anywhere under mteb/tasks/ (retrieval, reranking, or otherwise) — a Kazakh contribution would be a net-new `mteb/tasks/retrieval/kaz/` (and optionally `mteb/tasks/reranking/kaz/`) directory.
> **Source:** directory listing of embeddings-benchmark/mteb@2.16.3 mteb/tasks/retrieval/ and mteb/tasks/reranking/ (https://github.com/embeddings-benchmark/mteb/tree/2.16.3/mteb/tasks/retrieval and https://github.com/embeddings-benchmark/mteb/tree/2.16.3/mteb/tasks/reranking); local `find` returned no kaz-named files · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
