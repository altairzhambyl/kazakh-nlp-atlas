---
kb_id: "hf:vngrs-ai/kumru-2b"
type: "source"
title: "huggingface.co/vngrs-ai/Kumru-2B, huggingface.co/vngrs-ai/Kumru-2B-Bas…"
doi: null
hf_repo: "vngrs-ai/Kumru-2B"
year: null
topics: ["turkic-turkish"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["hf:vngrs-ai/kumru-2b"]
tags: ["source", "topic/turkic-turkish"]
---
# huggingface.co/vngrs-ai/Kumru-2B, huggingface.co/vngrs-ai/Kumru-2B-Bas…

**Topics:** [[turkic-turkish]]

## Source URLs
- huggingface.co/vngrs-ai/Kumru-2B, huggingface.co/vngrs-ai/Kumru-2B-Base, erkansaka.net/2025/10/14 launch coverage

## Findings

> [!note] CLAIM — turkic-turkish
> [tr] Kumru-2B (VNGRS, Sept 2025) is the best-executed from-scratch Turkish SLM and dwarfs SozKZ's data scale: 500GB deduplicated corpus, 300B training tokens for a 2B model (150:1 tokens/param) vs SozKZ's 9B tokens for 600M (15.3:1) — a 10x higher data:param ratio. Base+instruct+the full training corpus were open-sourced (transparency move). Runs on 16GB VRAM (RTX A4000/3090) or on-device at 4.8GB unquantized. Context 8,192 tokens; other open-source models spend 38-98% more tokens than Kumru's custom tokenizer while having larger vocabularies.
>
> **Numbers:** 500GB corpus, 300B tokens, 2B params (150:1 tok/param); context 8,192; 4.8GB device footprint; 38-98% tokenizer efficiency vs peers
> **Relevance:** Sets the honest 'what a well-resourced from-scratch Turkic SLM looks like' bar — SozKZ's 9B-token/600M-param Kazakh effort is 10x less data-intensive per param than the best Turkish from-scratch precedent, partly explaining its weaker knowledge scores (30.3% MC-QA) relative to Kumru's reported quality.
> **Source:** huggingface.co/vngrs-ai/Kumru-2B, huggingface.co/vngrs-ai/Kumru-2B-Base, erkansaka.net/2025/10/14 launch coverage · **Sweep:** `turkic-landscape`

[[Home]]
