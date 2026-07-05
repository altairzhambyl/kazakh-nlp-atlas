---
kb_id: "title:scientists uz fileview id 9807 pdf read directly full paper"
type: "source"
title: "scientists.uz/fileView?id=9807 (PDF, read directly, full paper)"
doi: null
hf_repo: null
year: null
topics: ["turkic-embeddings-retrieval-non-kazakh-t"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:scientists uz fileview id 9807 pdf read directly full paper"]
tags: ["source", "topic/turkic-embeddings-retrieval-non-kazakh-t"]
---
# scientists.uz/fileView?id=9807 (PDF, read directly, full paper)

**Topics:** [[turkic-embeddings-retrieval-non-kazakh-t]]

## Source URLs
- scientists.uz/fileView?id=9807 (PDF, read directly, full paper)

## Findings

> [!note] CLAIM — turkic-embeddings-retrieval-non-kazakh-t
> [uz] AugSBERT-Uz (Muminov & Allaberganova, Tashkent Univ. of Economics/TUIT, Science and Innovation journal, Nov 2025, DOI 10.5281/zenodo.17693973) is the FIRST sentence-level Uzbek embedding model, built via teacher(cross-encoder)-student(bi-encoder) distillation from monolingual BERTbek: teacher fine-tuned on ~5,000 human 'gold' pairs (positives from Uzbek-Kazakh parallel corpus + Uzbek-English translation pairs treated as equivalent, negatives random-sampled) reaches Spearman 85.0; BM25 top-50 candidate mining over a >150M-word unlabeled corpus (Uzbek CC-100 + uzWaC + BERTbek pretrain news) generates a silver set the teacher pseudo-labels; student bi-encoder (BERTbek + mean pooling + MNRL) trained on gold+silver reaches Spearman 83.2 (97.9% of teacher) in ~5s vs teacher's 65h for a 10k-sentence corpus (47,000x faster). Evaluated ONLY on SimRelUz (word-level test, adapted to sentence pairs) — NO mE5/BGE-M3 baseline was run; the only multilingual comparison point is zero-shot distiluse-base-multilingual at Spearman 61.0 (an older, weaker sentence-transformer, not mE5).
>
> **Numbers:** TF-IDF 35.0; avg FastText 42.5; distiluse-base-multilingual (zero-shot) 61.0; SBERT-Gold (gold-only, ~5k pairs) 70.5; AugSBERT-Uz (gold+silver) 83.2; BERTbek cross-encoder teacher (upper bound) 85.0; inference 5s (student) vs 65h (teacher) per 10k-sentence corpus
> **Relevance:** Critical for the live Uzbek collaboration (decision 1): Uzbek has ZERO published mE5-large/BGE-M3 baseline number on its only STS set (SimRelUz) — the exact same gap kazembed-v5 filled for Kazakh on KazQAD. Any port of the lab's Less-is-More recipe to Uzbek must FIRST measure mE5-large on SimRelUz before claiming any beat-mE5 target. Also: Uzbek has no retrieval/QA dataset at all (STS only, word-level-derived) — porting KazQAD-style retrieval means building the eval set from scratch, unlike Kazakh where KazQAD already existed. The teacher-student BM25-mining recipe is a concrete, reusable bootstrap method for generating Uzbek training pairs cheaply.
> **Source:** scientists.uz/fileView?id=9807 (PDF, read directly, full paper) · **Sweep:** `turkic-landscape`

[[Home]]
