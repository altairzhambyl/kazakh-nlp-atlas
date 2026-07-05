---
kb_id: "arxiv:2511.08376"
type: "paper"
title: "TurkEmbed: Turkish Embedding Model on NLI & STS Tasks"
arxiv_id: "2511.08376"
doi: null
hf_repo: null
year: 2025
topics: ["embeddings-training", "turkic-turkish", "turkic-pan-benchmarks-non-kazakh-turkic"]
claims: 3
uncertain_claims: 0
verdicts: []
aliases: ["TurkEmbed: Turkish Embedding Model on NLI & STS Tasks", "arXiv:2511.08376", "arxiv:2511.08376"]
tags: ["paper", "topic/embeddings-training", "topic/turkic-turkish", "topic/turkic-pan-benchmarks-non-kazakh-turkic"]
---
# TurkEmbed: Turkish Embedding Model on NLI & STS Tasks

[arXiv](https://arxiv.org/abs/2511.08376)
**Topics:** [[embeddings-training]], [[turkic-turkish]], [[turkic-pan-benchmarks-non-kazakh-turkic]]

> [!abstract]
> This paper introduces TurkEmbed, a novel Turkish language embedding model designed to outperform existing models, particularly in Natural Language Inference (NLI) and Semantic Textual Similarity (STS) tasks. Current Turkish embedding models often rely on machine-translated datasets, potentially limiting their accuracy and semantic understanding. TurkEmbed utilizes a combination of diverse datasets …

## Claims

> [!note] CLAIM — embeddings-training
> Turkic evidence (closest family to Kazakh) says beating mE5 is HARD even with a dedicated effort: TR-MTEB built 34.2M weakly-supervised Turkish pairs and trained Turkish-specific models with Matryoshka + two-stage NLI/STS fine-tuning, yet multilingual-E5 variants still LEAD the benchmark; Turkish-specific models are 'improving but not yet surpassing' mE5.
>
> **Numbers:** 34.2M weak Turkish pairs; Matryoshka + MNRL (All-NLI-TR) then CoSENT (STSB-TR); mE5 still #1 on TR-MTEB retrieval
> **Relevance:** TESTED-ON-TURKIC. Sober calibration for the lab's 'beat mE5-large' target: a 34.2M-pair Turkish program did not dethrone mE5 on a same-family agglutinative language. Implies qymyz-embed must lean on (a) KazQAD-domain specialization and (b) distillation/model-soup, not raw pair volume, to win on KazQAD specifically.
> **Source:** TR-MTEB (ACL Findings EMNLP 2025, aclanthology 2025.findings-emnlp.471); TurkEmbed arXiv:2511.08376; TurkEmbed4Retrieval arXiv:2511.07595 · **Sweep:** `slm-arch-for-kazakh`

> [!note] CLAIM — turkic-turkish
> [tr] TR-MTEB (EMNLP 2025 Findings, aclanthology 2025.findings-emnlp.471) built 34.2M weakly-supervised Turkish pairs across 26 datasets/6 task types (classification, clustering, pair-classification, retrieval, bitext-mining, STS) and confirms multilingual-e5-large remains the overall leader (highest Mean-Task/Mean-Type scores), while a narrower specialized model, TurkEmbed, reaches Turkish-specific SOTA on semantic tasks (STS Pearson 0.845 / Spearman 0.853) using roughly half the parameters of multilingual-e5-large-instruct — i.e. mE5 wins in aggregate but a lean specialized model can beat it on a task subset.
>
> **Numbers:** 26 datasets, 6 task types, 34.2M weak pairs; TurkEmbed STS Pearson 0.845/Spearman 0.853 at ~half mE5-large-instruct's params; mE5-large leads TR-MTEB overall Mean(Task)/Mean(Type)
> **Relevance:** Refines the KB's existing 'TR-MTEB: mE5 not surpassed' claim — it IS surpassed on STS specifically by a half-sized specialized model, so the lab's 'beat mE5-large on KazQAD' target should specify which task(s), since full-suite parity is the harder (and per Turkish evidence, still unbeaten) bar.
> **Source:** aclanthology.org/2025.findings-emnlp.471 (TR-MTEB); arXiv:2511.08376 (TurkEmbed) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> TurkEmbed [tr] (2025 IEEE ASYU conference, arXiv:2511.08376) is a separate, smaller Turkish embedding model claiming SOTA on Turkish STSb/STS22 semantic similarity — evaluated on STS only, not the full TR-MTEB 6-task suite; a second independent 'MTEB-TR' effort (github.com/selmanbaysan/mteb_tr) also exists in parallel to the ACL-published TR-MTEB (trmteb), indicating some naming/effort fragmentation within Turkish embedding benchmarking itself.
>
> **Numbers:** n/a
> **Relevance:** Even Turkish, the best-resourced Turkic language, has fragmented/competing embedding benchmarks (TR-MTEB vs MTEB-TR vs TurkEmbed's own STS claim) — a cautionary note for the lab: naming a Kazakh benchmark 'kk-MTEB' should check for any parallel community effort before the upstream MTEB PR to avoid the same duplication Turkish now has.
> **Source:** arXiv:2511.08376; github.com/selmanbaysan/mteb_tr; aclanthology.org/2025.findings-emnlp.471 · **Sweep:** `turkic-landscape`

## Related
- [[xnli-evaluating-cross-lingual-sentence-representations|XNLI: Evaluating Cross-lingual Sentence Representations]] — Turkish (sister Turkic) has NLI+STS enabling TurkEmbed; Kazakh has neither, so an equivalent kk supervised-STS embedder is blocked
- [[the-russian-focused-embedders-exploration-rumteb-benchmark-and-russian|The Russian-focused embedders' exploration: ruMTEB benchmark and Russian embedding model d…]] — ruMTEB is the kkMTEB construction template; TurkEmbed is the Turkic-family analogue — both test whether monolingual specialization beats mE5
- [[less-is-more-adapting-text-embeddings-for-low-resource-languages-with-small|Less is More: Adapting Text Embeddings for Low-Resource Languages with Small Scale Noisy S…]] — Turkic sibling: TurkEmbed's 34.2M pairs fail to beat mE5, tempering Less-is-More's claim of cheaply winning on a Kazakh-family LRL
- [[aclanthology-org-2025-findings-emnlp-471-tr-mteb-emnlp-2025-b28b6536|aclanthology.org/2025.findings-emnlp.471 (TR-MTEB, EMNLP 2025 Findings…]] — TurkEmbed is evaluated on TR-MTEB, where mE5 variants still lead retrieval
- [[huggingface-co-nurlykhan-kazembed-v5-apache-2-0|huggingface.co/Nurlykhan/kazembed-v5 (apache-2.0)]] — Turkic-sibling target: TurkEmbed is a Turkish embedding model, closest-language comparator for Kazakh

[[Home]]
