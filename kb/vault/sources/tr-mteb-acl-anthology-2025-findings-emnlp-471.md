---
kb_id: "title:tr mteb acl anthology 2025 findings emnlp 471 huggingface co trmteb leaderboard"
type: "source"
title: "TR-MTEB, ACL Anthology 2025.findings-emnlp.471"
doi: null
hf_repo: null
year: null
topics: ["turkic-pan-models"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:tr mteb acl anthology 2025 findings emnlp 471 huggingface co trmteb leaderboard"]
tags: ["source", "topic/turkic-pan-models"]
---
# TR-MTEB, ACL Anthology 2025.findings-emnlp.471

**Topics:** [[turkic-pan-models]]

## Source URLs
- TR-MTEB, ACL Anthology 2025.findings-emnlp.471
- huggingface.co/trmteb leaderboard

## Findings

> [!note] CLAIM — turkic-pan-models
> [tr] TR-MTEB (EMNLP 2025 Findings) is the first comprehensive Turkish embedding benchmark: 6 tasks, 26 datasets. On the full leaderboard, OpenAI text-embedding-3-small ranks 1st (66.5 avg), the Turkish-specific ytu-ce-cosmos/turkish-e5-large (a fine-tune of intfloat/multilingual-e5-large-instruct) ranks 2nd (66.0), and multilingual-e5-large-instruct itself ranks 3rd (65.9) — i.e. a Turkish-adapted E5 variant essentially TIES/slightly beats its own multilingual-e5 base on its native-language benchmark.
>
> **Numbers:** text-embedding-3-small 66.5 (1st/26); turkish-e5-large 66.0 (2nd/26); mE5-large-instruct 65.9 (3rd/26)
> **Relevance:** Directly answers decision (1)/(3): unlike Kazakh (where kazembed-v5's own mE5 fine-tune only gained +2.1% MRR, KB) and unlike the general TR-MTEB narrative that 'multilingual E5 dominate, Turkish-specific not yet surpassing' (from a broader search summary), the SPECIFIC turkish-e5-large datapoint shows a fine-tuned Turkish E5 variant matching its multilingual base — meaning Turkish embedding adaptation is closer to solved than Kazakh's, and any pan-Turkic embedding benchmark artifact should benchmark against turkish-e5-large as the strongest same-family baseline, not just raw mE5.
> **Source:** TR-MTEB, ACL Anthology 2025.findings-emnlp.471; huggingface.co/trmteb leaderboard · **Sweep:** `turkic-landscape`

[[Home]]
