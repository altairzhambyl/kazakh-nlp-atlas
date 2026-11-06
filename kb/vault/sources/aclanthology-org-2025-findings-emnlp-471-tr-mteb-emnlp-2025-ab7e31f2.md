---
kb_id: "title:aclanthology org 2025 findings emnlp 471 tr mteb emnlp 2025 findings baysan gungor table 2"
type: "source"
title: "aclanthology.org/2025.findings-emnlp.471 (TR-MTEB, EMNLP 2025 Findings…"
doi: null
hf_repo: null
year: null
topics: ["non-kazakh-turkic-nlp-landscape-embeddin"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:aclanthology org 2025 findings emnlp 471 tr mteb emnlp 2025 findings baysan gungor table 2"]
tags: ["source", "topic/non-kazakh-turkic-nlp-landscape-embeddin"]
---
# aclanthology.org/2025.findings-emnlp.471 (TR-MTEB, EMNLP 2025 Findings…

**Topics:** [[non-kazakh-turkic-nlp-landscape-embeddin]]

## Source URLs
- aclanthology.org/2025.findings-emnlp.471 (TR-MTEB, EMNLP 2025 Findings, Baysan & Gungor), Table 2

## Findings

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-embeddin
> [tr] On TR-MTEB's RETRIEVAL-SPECIFIC column (not aggregate), multilingual-e5-large IS beaten — but only by OpenAI's proprietary text-embedding-3-small, not by any dedicated Turkish/Turkic model. Full retrieval column from the paper's own Table 2: mE5-large 63.74, text-embedding-3-small 64.99 (+1.25), mE5-base 58.29, gte-multilingual-base 57.51, mE5-large-instruct 57.21, mE5-small 56.53. TR-MTEB's own purpose-built Turkish embedder (BERTurk-base 110M, contrastively pretrained on 34.2M Turkish pairs + supervised fine-tuned) scores only 52.75 retrieval — LOSES to mE5-large by 10.99 points despite winning Pair-Classification (71.03 vs 65.01) and STS (78.44 vs 81.18 is close).
>
> **Numbers:** Retr. column: mE5-large 63.74; text-embedding-3-small 64.99; mE5-base 58.29; gte-multilingual-base 57.51; mE5-large-instruct 57.21; mE5-small 56.53; turkish-embedding-model-fine-tuned (110M) 52.75; turkish-embedding-model (contrastive-only) 52.54; paraphrase-multilingual-mpnet-base-v2 49.27
> **Relevance:** Directly answers the sweep question with a primary source: mE5-large's retrieval crown in the Turkic family is NOT unbroken in absolute terms, but the only challenger is a general-purpose SOTA proprietary model, not a Turkic-specialized one — so the lab's 'beat mE5-large on KazQAD' target remains meaningfully hard and unclaimed by any dedicated-Turkic effort so far.
> **Source:** aclanthology.org/2025.findings-emnlp.471 (TR-MTEB, EMNLP 2025 Findings, Baysan & Gungor), Table 2 — fetched and OCR'd directly from PDF · **Sweep:** `turkic-landscape`

[[Home]]
