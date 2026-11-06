---
kb_id: "doi:10.54287/gujsa.1844025"
type: "source"
title: "Aghalarov et al. 2026, GU J Sci Part A 13(1):334-347, DOI 10.54287/guj…"
doi: "10.54287/gujsa.1844025"
hf_repo: null
year: null
topics: ["non-kazakh-turkic-nlp-landscape-prior-ar"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["doi:10.54287/gujsa.1844025"]
tags: ["source", "topic/non-kazakh-turkic-nlp-landscape-prior-ar"]
---
# Aghalarov et al. 2026, GU J Sci Part A 13(1):334-347, DOI 10.54287/guj…

**Topics:** [[non-kazakh-turkic-nlp-landscape-prior-ar]]

## Source URLs
- Aghalarov et al. 2026, GU J Sci Part A 13(1):334-347, DOI 10.54287/gujsa.1844025 (full PDF read, all 14 pages)

## Findings

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-prior-ar
> [az][pan-turkic] The closest prior-art threat — 'Knowledge Distillation for Embeddings of Low-Resource Turkic Family Languages' (Aghalarov, Mammadov, Huseynova, Baku Higher Oil School) — is confirmed real, published, and its headline 89% figure is a RAG top-1 retrieval accuracy on a 100-question Azerbaijani LEGAL QA set (Jina-v3 Multi-Task model), not a KazQAD/MTEB-style full-corpus retrieval metric. Full numbers from primary source (read all 14 pages of the PDF): BGE-M3 Azerbaijani STS 79.3->85.0 (+5.7pts, new SOTA on local benchmark) while retaining 98.6% of original English MTEB STS score (74.1->73.1). Jina-v3 Multi-Task: AZ-STS 84.8, BeleBele-az 90.3, English-STS 75.6 (vs vanilla Jina-v3 84.0/88.2/77.1). RAG pipeline (LLaMA-3.3-70B, Milvus, 100 legal FAQ questions, 2 human raters, Cohen's kappa 0.82): Jina Multi-Task Top-1 89.0%/Top-3 95.1%, human eval avg score 1.92/2, 94% 'Excellent'; vanilla Jina baseline was already 86.8% Top-1/84% Excellent -- so the KD gain over a strong off-the-shelf baseline is only +2.2pp Top-1 / +10pp Excellent, not a dramatic leap.
>
> **Numbers:** AZ-STS 79.3->85.0 (BGE-M3); English MTEB retention 98.6%; RAG Top-1 89.0%/Top-3 95.1% (Jina MT) vs vanilla Jina 86.8%/89.9%; %Excellent 94 vs 84 vanilla
> **Relevance:** Directly answers the research question: quantifies exactly what the Azerbaijani paper claims and shows the 89% figure is domain-specific (legal RAG), not a general Turkic retrieval SOTA, and the delta over vanilla off-the-shelf embeddings is modest -- weakens (but does not eliminate) the pre-emption risk for a Kazakh/pan-Turkic embedding-distillation claim.
> **Source:** Aghalarov et al. 2026, GU J Sci Part A 13(1):334-347, DOI 10.54287/gujsa.1844025 (full PDF read, all 14 pages) · **Sweep:** `turkic-landscape`

[[Home]]
