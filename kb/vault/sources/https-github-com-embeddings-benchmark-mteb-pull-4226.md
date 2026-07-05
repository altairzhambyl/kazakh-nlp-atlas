---
kb_id: "title:https github com embeddings benchmark mteb pull 4226"
type: "source"
title: "https://github.com/embeddings-benchmark/mteb/pull/4226"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-pr-precedents"]
claims: 2
uncertain_claims: 0
verdicts: []
aliases: ["title:https github com embeddings benchmark mteb pull 4226"]
tags: ["source", "topic/mteb-upstream-pr-precedents"]
---
# https://github.com/embeddings-benchmark/mteb/pull/4226

**Topics:** [[mteb-upstream-pr-precedents]]

## Source URLs
- https://github.com/embeddings-benchmark/mteb/pull/4226

## Findings

> [!note] CLAIM — mteb-upstream-pr-precedents
> PR #4226 'dataset: add BrowseComp-Plus' — a retrieval task built on a dataset that is XOR-obfuscated at rest for anti-scraping reasons (analogous to a gating concern). Created 2026-03-11, merged 2026-04-13 (~33 days) — the slowest of the sample, stalled mainly on the maintainer needing compute to run Qwen3-Embedding-0.6B as a required baseline (hit a github-actions stale-bot warning at day 25 for inactivity).
> **Source:** https://github.com/embeddings-benchmark/mteb/pull/4226 · **Sweep:** `2026-07-mteb-upstream-recon`

> [!note] CLAIM — mteb-upstream-pr-precedents
> On handling of datasets that must not appear as public plaintext (closest documented analogue to a 'gated' HF dataset), maintainer KennethEnevoldsen's stated preference order was: (1) re-upload to a proper mteb-controlled HF repo, (2) if that would expose sensitive content via HF's dataset viewer, make the mteb-controlled re-upload GATED rather than leave the original arrangement — explicitly calling gating 'not ideal, but better' than exposing content — and separately explored disabling the HF datasets-viewer as an alternative to gating. In the event, the maintainer ultimately re-uploaded it as a fully PUBLIC ungated dataset under the official mteb HF org and removed the custom load_data entirely.
> **Source:** https://github.com/embeddings-benchmark/mteb/pull/4226 · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
