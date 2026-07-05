---
kb_id: "title:https raw githubusercontent com embeddings benchmark mteb main mteb  hf integration hf hub utils py"
type: "source"
title: "https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/mteb/…"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-pr-precedents"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:https raw githubusercontent com embeddings benchmark mteb main mteb  hf integration hf hub utils py"]
tags: ["source", "topic/mteb-upstream-pr-precedents"]
---
# https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/mteb/…

**Topics:** [[mteb-upstream-pr-precedents]]

## Source URLs
- https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/mteb/_hf_integration/hf_hub_utils.py

## Findings

> [!note] CLAIM — mteb-upstream-pr-precedents
> mteb's own hub-integration code explicitly imports and handles huggingface_hub's GatedRepoError as an expected condition when checking commits/files on the Hub (logs a warning and returns None rather than crashing), i.e. the library is written to tolerate encountering gated repos gracefully, though this is a defensive fallback, not evidence that gated repos pass the CI dataset-loading test.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/mteb/_hf_integration/hf_hub_utils.py · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
