---
kb_id: "hf:seroe/qwen3-embedding-0.6b-turkish-triplet-matryoshka-v2"
type: "source"
title: "huggingface.co/seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v…"
doi: null
hf_repo: "seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v2"
year: null
topics: ["turkic-embeddings-retrieval-non-kazakh-t"]
claims: 1
uncertain_claims: 1
verdicts: []
aliases: ["hf:seroe/qwen3-embedding-0.6b-turkish-triplet-matryoshka-v2"]
tags: ["source", "topic/turkic-embeddings-retrieval-non-kazakh-t"]
---
# huggingface.co/seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v…

**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]]

## Source URLs
- huggingface.co/seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v2 (model card, fetched directly)

## Findings

> [!warning] UNCERTAIN — turkic-embeddings-retrieval-non-kazakh-t
> [tr] A community fine-tune of the exact backbone the lab plans to use — seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v2 (HF, Apache-2.0) — already exists: fine-tuned on 215,676 Turkish triplets ('vodex-turkish-triplets-large', telecom domain) with MatryoshkaLoss+CachedMultipleNegativesRankingLoss across 1024/768/512/256 dims, batch 2,048, lr 5e-5, 1 epoch. Reported metrics are only in-domain triplet accuracy (99.8%+ at all dims vs 88.7% base init) — NO TR-MTEB or other standardized benchmark score is published for this checkpoint.
>
> **Relevance:** Existence-proof that Qwen3-Embedding-0.6B (the lab's planned base per KB) is already being independently adapted to a sibling Turkic language by hobbyists, but with an in-domain-only, non-rigorous eval — the lab's rigorous TR-MTEB-style evaluation of a Qwen3-Embedding-0.6B Turkish fine-tune remains an open, unclaimed comparison point relevant to validating that the same recipe transfers across the family.
> **Source:** huggingface.co/seroe/Qwen3-Embedding-0.6B-turkish-triplet-matryoshka-v2 (model card, fetched directly) · **Sweep:** `turkic-landscape`

[[Home]]
