---
kb_id: "title:github com huggingface fineweb 2 blob main fineweb2 language distribution csv rows kaz cyrl vs uzn latn uzn cyrl same source as above"
type: "source"
title: "github.com/huggingface/fineweb-2/blob/main/fineweb2-language-distribut…"
doi: null
hf_repo: null
year: null
topics: ["turkic-nlp-landscape-uzbek-monolingual-p"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:github com huggingface fineweb 2 blob main fineweb2 language distribution csv rows kaz cyrl vs uzn latn uzn cyrl same source as above"]
tags: ["source", "topic/turkic-nlp-landscape-uzbek-monolingual-p"]
---
# github.com/huggingface/fineweb-2/blob/main/fineweb2-language-distribut…

**Topics:** [[turkic-nlp-landscape-uzbek-monolingual-p]]

## Source URLs
- github.com/huggingface/fineweb-2/blob/main/fineweb2-language-distribution.csv (rows kaz_Cyrl vs uzn_Latn/uzn_Cyrl), same source as above

## Findings

> [!note] CLAIM — turkic-nlp-landscape-uzbek-monolingual-p
> [uz][kk] Apples-to-apples same-pipeline comparison (FineWeb2 CSV): Kazakh kaz_Cyrl train = 1,876,843,453 words / 3,344,366 docs / 20.67GB text / 6.33GB parquet. Ratio Kazakh:Uzbek(both scripts combined) = 1.52x; Kazakh:Uzbek(Latin-only) = 2.73x — dramatically smaller than the 3.4-5.2x gaps seen in the older mC4(2020)/CC-100(2018) sources, and far below the '~37x worse than Kazakh' some prior researcher recommendations assumed.
>
> **Numbers:** kk (kaz_Cyrl train): 1,876,843,453 words / 3,344,366 docs / 20.67GB. Ratio kk:uz(combined)=1.52x; kk:uz(Latin only)=2.73x. Prior sources gave kk:uz ratios of 3.4x (mC4 2020) and 5.2x (CC-100 2018).
> **Relevance:** DIRECTLY resolves the port-feasibility disagreement in Decision 1: on the newest, largest, most-filtered public web corpus, Uzbek is only 1.5-2.7x smaller than Kazakh (not 15x-66x). The '~37x worse' claim is only defensible if the port pipeline is restricted to CulturaX specifically (75M tok) vs Kazakh's own CulturaX-scale pool — it is NOT true of the best available raw web data (FineWeb2).
> **Source:** github.com/huggingface/fineweb-2/blob/main/fineweb2-language-distribution.csv (rows kaz_Cyrl vs uzn_Latn/uzn_Cyrl), same source as above · **Sweep:** `turkic-landscape`

[[Home]]
