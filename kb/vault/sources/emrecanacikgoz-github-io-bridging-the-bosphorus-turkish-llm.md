---
kb_id: "title:emrecanacikgoz github io bridging the bosphorus turkish llm adaptation and benchmarking study"
type: "source"
title: "emrecanacikgoz.github.io/Bridging-the-Bosphorus/ (Turkish LLM adaptati…"
doi: null
hf_repo: null
year: null
topics: ["turkic-pan-models"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:emrecanacikgoz github io bridging the bosphorus turkish llm adaptation and benchmarking study"]
tags: ["source", "topic/turkic-pan-models"]
---
# emrecanacikgoz.github.io/Bridging-the-Bosphorus/ (Turkish LLM adaptati…

**Topics:** [[turkic-pan-models]]

## Source URLs
- emrecanacikgoz.github.io/Bridging-the-Bosphorus/ (Turkish LLM adaptation and benchmarking study)

## Findings

> [!note] CLAIM — turkic-pan-models
> [tr] 'Bridging the Bosphorus' (Turkish LLM adaptation study) directly tests continual-pretraining-on-strong-base vs from-scratch-pretraining vs LoRA-continual-PT-on-weak-base for Turkish: from-scratch Hamza models (GPT-2 arch, 124M/354M/772M/1.3B, 179.2GB / 130B Turkish tokens) beat continued pretraining of a weak base (GPT2-xlarge) at the SAME architecture, but continual pretraining of a STRONG base (Mistral-7B) beats BOTH the from-scratch Hamza models and the weak-base continual-PT on Turkish QA. Continual pretraining also caused catastrophic forgetting on English benchmarks proportional to Turkish sample count.
>
> **Numbers:** Hamza: 124M/354M/772M/1.3B, 130B tokens, 179.2GB corpus; ARC-TR: Gemma-7B 46.16% (best), range 24-47%; TruthfulQA-TR: Trendyol-DPO 50.11% (best), range 33-50%
> **Relevance:** Cross-validates the lab's own from-scratch-vs-adapted debate (SozKZ vs Qwen3-0.6B, KB) with an independent Turkic-family case: 'from-scratch beats a WEAK continually-pretrained base, but continual-PT-on-a-STRONG-base beats from-scratch' — reinforces that QymyzLM's QLoRA-CPT-on-Qwen3-0.6B-Base strategy (strong base + continual PT) is the empirically-favored path across at least two Turkic languages now, not just an isolated Kazakh finding.
> **Source:** emrecanacikgoz.github.io/Bridging-the-Bosphorus/ (Turkish LLM adaptation and benchmarking study) · **Sweep:** `turkic-landscape`

[[Home]]
