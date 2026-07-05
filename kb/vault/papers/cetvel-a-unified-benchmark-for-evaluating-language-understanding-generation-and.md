---
kb_id: "arxiv:2508.16431"
type: "paper"
title: "Cetvel: A Unified Benchmark for Evaluating Language Understanding, Generation and Cultural Capacity of LLMs for Turkish"
arxiv_id: "2508.16431"
doi: null
hf_repo: "boun-tabi-LMG/TURNA"
year: 2025
topics: ["turkic-turkish"]
claims: 2
uncertain_claims: 0
verdicts: []
aliases: ["Cetvel: A Unified Benchmark for Evaluating Language Understanding, Generation and Cultural Capacity of LLMs for Turkish", "arXiv:2508.16431", "arxiv:2508.16431"]
tags: ["paper", "topic/turkic-turkish"]
---
# Cetvel: A Unified Benchmark for Evaluating Language Understanding, Generation and Cultural Capacity of LLMs for Turkish

[arXiv](https://arxiv.org/abs/2508.16431)
**Topics:** [[turkic-turkish]]

> [!abstract]
> We introduce Cetvel, a comprehensive benchmark designed to evaluate large language models (LLMs) in Turkish. Existing Turkish benchmarks often lack either task diversity or culturally relevant content, or both. Cetvel addresses these gaps by combining a broad range of both discriminative and generative tasks ensuring content that reflects the linguistic and cultural richness of Turkish language. C …

## Claims

> [!note] CLAIM — turkic-turkish
> [tr] Cetvel (KUIS AI / Koç University, EACL 2026, arXiv Aug 2025) tested 33 open-weight Turkish-capable LLMs (up to 70B) across 23 tasks / 7 categories built from 22 Turkish datasets and found that Turkish-centric instruction-tuned models GENERALLY UNDERPERFORM general multilingual models (Llama-3, Mistral) despite language-specific tuning; grammatical error correction and extractive QA were the most discriminative tasks.
>
> **Numbers:** 23 tasks / 7 categories / 22 datasets; 33 models up to 70B; CC BY-SA 4.0
> **Relevance:** Directly parallels the Kazakh finding that SozKZ/from-scratch loses to general Qwen/Llama baselines — this is now a TWO-language pattern (Turkish AND Kazakh), making 'language-specific tuning alone underperforms general multilingual scale' a family-wide phenomenon worth citing in the atlas, not a Kazakh-specific anomaly.
> **Source:** arXiv:2508.16431 (Cetvel), github.com/KUIS-AI/cetvel · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-turkish
> Turkish NLP has four distinct institutional players with different strategies: KUIS AI (Koç University) builds EVALUATION infrastructure (Cetvel, TurkishMMLU) rather than models; Boğaziçi TABILAB builds both encoder (TabiBERT, ModernBERT-based, Dec 2025) and encoder-decoder (TURNA, 1.1B UL2/mT5-style, 43B tokens) foundation models; YTU COSMOS (TUBITAK-funded) builds from-scratch decoder SLMs (cosmosGPT 355M/774M) with rapid iteration (founded Jan 2024, shipped model within 2 months); VNGRS is a private company shipping the most resourced from-scratch efforts (VBART, Kumru-2B/300B tokens) with full open-sourcing including training corpora; Trendyol (e-commerce) does continual-PT of strong bases (Qwen2.5/Qwen3/Gemma3) for commercial chat/domain use, never from scratch.
>
> **Numbers:** TURNA 1.1B/43B tokens; TabiBERT (ModernBERT-based); cosmosGPT 355M/774M; Kumru-2B/300B tokens; Trendyol-LLM-8B-T1 on Qwen3-8B, 32K ctx
> **Relevance:** Maps who to approach/cite for Uzbek-style collaboration playbooks: KUIS AI is the natural counterpart for Kazakh EVAL-protocol design (their Cetvel/TurkishMMLU methodology is directly reusable), VNGRS is the counterpart for from-scratch-SLM data-engineering practices (corpus release transparency), YTU COSMOS is the closest peer in team size/funding model to the lab itself.
> **Source:** Synthesis of arXiv:2508.16431, huggingface.co/boun-tabi-LMG/TURNA, arXiv:2512.23065, arXiv:2404.17336, huggingface.co/vngrs-ai, huggingface.co/Trendyol · **Sweep:** `turkic-landscape`

**Cited KB notes:** [[tabibert-a-large-scale-modernbert-foundation-model-and-a-unified-benchmark-for]], [[introducing-cosmosgpt-monolingual-training-for-turkish-language-models]]

[[Home]]
