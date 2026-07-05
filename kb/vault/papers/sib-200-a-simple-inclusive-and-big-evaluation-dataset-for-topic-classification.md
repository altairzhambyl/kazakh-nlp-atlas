---
kb_id: "arxiv:2309.07445"
type: "paper"
title: "SIB-200: A Simple, Inclusive, and Big Evaluation Dataset for Topic Classification in 200+ Languages and Dialects"
arxiv_id: "2309.07445"
doi: null
hf_repo: null
year: 2023
topics: ["turkic-kyrgyz-non-kazakh-turkic-nlp-land"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["SIB-200: A Simple, Inclusive, and Big Evaluation Dataset for Topic Classification in 200+ Languages and Dialects", "arXiv:2309.07445", "arxiv:2309.07445"]
tags: ["paper", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land"]
---
# SIB-200: A Simple, Inclusive, and Big Evaluation Dataset for Topic Classification in 200+ Languages and Dialects

[arXiv](https://arxiv.org/abs/2309.07445)
**Topics:** [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]]

> [!abstract]
> Despite the progress we have recorded in the last few years in multilingual natural language processing, evaluation is typically limited to a small set of languages with available datasets which excludes a large number of low-resource languages. In this paper, we created SIB-200 -- a large-scale open-sourced benchmark dataset for topic classification in 200 languages and dialects to address the la …

## Claims

> [!note] CLAIM — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [ky][kk][az][uz][tt][ug][kaa][crh] FLORES-200, SIB-200, and Belebele all include Kyrgyz (kir_Cyrl) natively as one of their 200+/205/122 covered languages/variants, meaning the KazQAD-style retrieval and MTEB-style classification protocols the lab already pins for Kazakh are directly reusable on Kyrgyz text with ZERO additional annotation — the same FLORES-200 passages underlie SIB-200 (topic classification) and Belebele (reading-comprehension MCQ).
>
> **Numbers:** FLORES-200: 842 web articles, 3,001 sentences per language incl. kir_Cyrl; SIB-200: 205 langs/dialects; Belebele: 122 variants
> **Relevance:** This is the concrete evidence for decision (1): Kyrgyz is 'free' to add to the lab's evallab classification/reading-comprehension suite (no new annotation), but retrieval specifically (KazQAD-analog passage-retrieval, not just topic-classification) has NO existing Kyrgyz benchmark — that gap must be built from scratch (e.g. from the 76,170-article Kyrgyz Wikipedia) if Kyrgyz retrieval is prioritized.
> **Source:** SIB-200 (arXiv 2309.07445 / EACL 2024); FLORES-200 GitHub README (facebookresearch/flores); Belebele HF card · **Sweep:** `turkic-landscape`

[[Home]]
