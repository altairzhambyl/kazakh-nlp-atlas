---
kb_id: "arxiv:2502.11020"
type: "paper"
title: "TUMLU: A Unified and Native Language Understanding Benchmark for Turkic Languages"
arxiv_id: "2502.11020"
doi: null
hf_repo: null
year: 2025
topics: ["sota-slm", "kazakh-turkic-nlp", "turkic-turkish", "turkic-uzbek-non-kazakh-turkic-nlp-lands", "turkic-kyrgyz-non-kazakh-turkic-nlp-land", "turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-benchmarks-non-kazakh-turkic", "turkic-pan-models", "non-kazakh-turkic-nlp-landscape-reconcil"]
claims: 19
uncertain_claims: 7
verdicts: []
aliases: ["TUMLU: A Unified and Native Language Understanding Benchmark for Turkic Languages", "arXiv:2502.11020", "arxiv:2502.11020"]
tags: ["paper", "topic/sota-slm", "topic/kazakh-turkic-nlp", "topic/turkic-turkish", "topic/turkic-uzbek-non-kazakh-turkic-nlp-lands", "topic/turkic-kyrgyz-non-kazakh-turkic-nlp-land", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-benchmarks-non-kazakh-turkic", "topic/turkic-pan-models", "topic/non-kazakh-turkic-nlp-landscape-reconcil"]
---
# TUMLU: A Unified and Native Language Understanding Benchmark for Turkic Languages

[arXiv](https://arxiv.org/abs/2502.11020)
**Topics:** [[sota-slm]], [[kazakh-turkic-nlp]], [[turkic-turkish]], [[turkic-uzbek-non-kazakh-turkic-nlp-lands]], [[turkic-kyrgyz-non-kazakh-turkic-nlp-land]], [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-benchmarks-non-kazakh-turkic]], [[turkic-pan-models]], [[non-kazakh-turkic-nlp-landscape-reconcil]]

> [!abstract]
> Being able to thoroughly assess massive multi-task language understanding (MMLU) capabilities is essential for advancing the applicability of multilingual language models. However, preparing such benchmarks in high quality native language is often costly and therefore limits the representativeness of evaluation datasets. While recent efforts focused on building more inclusive MMLU benchmarks, thes …

## Claims

> [!note] CLAIM — sota-slm
> TUMLU-mini is the right Turkic cross-lingual eval: a natively-authored (not translated) benchmark of 4-choice middle/high-school questions across 8 Turkic languages incl. Kazakh, Azerbaijani, Uzbek, Kyrgyz, Tatar, Uyghur, Karakalpak, Crimean Tatar; 38,139 total questions across 11 subjects.
>
> **Numbers:** 8 Turkic langs, 11 subjects, 38,139 Qs, 4-choice
> **Relevance:** Confirms the paper's secondary eval choice and enables a 'Turkic transfer' story — training on Kazakh + related Turkic data and reporting TUMLU-mini would strengthen the SOTA claim beyond a single language.
> **Source:** arXiv 2502.11020 (TUMLU, ACL 2025); github.com/ceferisbarov/TUMLU · **Sweep:** `slm-architecture-2026-07`

> [!note] CLAIM — kazakh-turkic-nlp
> TUMLU-mini is the Turkic secondary eval: Kazakh subset = 700 Q (7 subjects x 100, Cyrillic). All models score higher on Kazakh in CYRILLIC than Latin. Best small-open on Kazakh: Gemma-2-9B 49.1, Llama-3.1-8B 46.4, Qwen2.5-7B 45.0; frontier Claude-3.5-Sonnet 83.0 (87.1 with 5-shot CoT). No <=1B model was tested. FineWeb-2 has 1.8B Kazakh Cyrillic words and 0 Latin.
>
> **Numbers:** Kazakh TUMLU-mini 700 Q; Gemma-2-9B 49.1 / Llama-3.1-8B 46.4 / Qwen2.5-7B 45.0; Claude-3.5-Sonnet 83.0
> **Relevance:** Train and evaluate in Cyrillic only for now — Latin Kazakh web data is essentially nonexistent, so the 2031 Latin transition is a pure data gap, not something to pre-train on. Handle Latin via deterministic Cyrillic<->Latin transliteration augmentation, not native Latin corpora.
> **Source:** arXiv 2502.11020 (TUMLU), html v2, Table 2 + Appendix B · **Sweep:** `slm-architecture-2026-07`

> [!note] CLAIM — turkic-turkish
> TUMLU is the only native (non-translated) pan-Turkic MMLU-style benchmark and gives a direct, same-protocol Turkish-vs-Kazakh-vs-Uzbek-vs-Azerbaijani-vs-Kyrgyz-vs-Uyghur comparison at 5-shot: [tr] Claude-3.5-Sonnet 85.7%, GPT-4o 83.7%, Qwen2.5-72B 73.9%, Llama-3.1-70B 64.9%; [kk] Claude-3.5-Sonnet 83.0%, GPT-4o 81.0%, Qwen2.5-72B 62.6%, Llama-3.1-70B 56.4%; [az] Claude-3.5-Sonnet 84.4%; [crh] (Crimean Tatar) 81.2%; [ky] 75.7%; [ug] 71.3%; [uz] 69.1% (lowest of the eight). Notably Kazakh trails Turkish by only 2.7pp on the strongest closed model but by 11.3pp on Qwen2.5-72B and 8.5pp on Llama-3.1-70B — the gap is much wider for open-weight models than frontier closed ones.
>
> **Numbers:** 38,139 questions, 8 languages (az, crh, kaa, kk, ky, tr, ug, uz), 11 subjects, TUMLU-mini=100 q/subject; kk 83.0/81.0/62.6/56.4 vs tr 85.7/83.7/73.9/64.9 (Claude-3.5-Sonnet/GPT-4o/Qwen2.5-72B/Llama-3.1-70B)
> **Relevance:** Directly answers decision (2): quantifies where Kazakh sits vs Turkish and siblings on IDENTICAL native (non-MT) questions; shows open-weight-model gap (8-11pp) is the honest number to cite, not the closed-model gap (2.7pp) which flatters resource parity.
> **Source:** arXiv:2502.11020 (TUMLU, ACL 2025 Findings), github.com/ceferisbarov/TUMLU · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-turkish
> No pan-Turkic MTEB-style embedding/retrieval benchmark exists as of mid-2026: TR-MTEB (Turkish-only, 26 datasets) and the lab's planned kk-MTEB are both monolingual efforts; TUMLU (pan-Turkic, 8 languages) covers MMLU-style multiple-choice QA only, not embeddings/retrieval. No search turned up a 'Turkic-MTEB' or equivalent multi-language embedding suite.
>
> **Numbers:** n/a (absence finding)
> **Relevance:** Directly answers decision (3): a pan-Turkic-MTEB (using TR-MTEB's 6-task taxonomy as template, extended to kk/uz/az/ky at minimum) is unclaimed territory and would be a genuinely novel, adoptable lab artifact beyond the Kazakh-only kk-MTEB plan — natural collaboration surface with the live Uzbek offer.
> **Source:** Search synthesis across aclanthology.org/2025.findings-emnlp.471, arXiv:2502.11020, and general web search for 'pan-Turkic MTEB' · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz][kk][az][tr][ky][tt][crh][kaa][ug] TUMLU (arXiv:2502.11020, ACL 2025) is a native (non-translated) MCQ benchmark across 9 Turkic languages with 38,139 total questions; TUMLU-mini per-language subset sizes: Kazakh 700, Uzbek 700, Azerbaijani 700, Turkish 700, Tatar 700, Kyrgyz 598, Uyghur 494, Crimean Tatar 316, Karakalpak 215. 7 core subjects: Biology, Chemistry, Geography, History, Mathematics, Native Language & Literature, Physics. 5-shot accuracy shows Kazakh consistently and substantially ABOVE Uzbek across every model tested: Claude 3.5 Sonnet 83.0% (kk) vs 69.1% (uz); GPT-4o 81.0% vs 65.4%; Gemini 1.5 Pro 78.4% vs 65.1%; Qwen2.5-72B 62.6% vs 50.4%; Llama-3.1-70B 56.4% vs 45.3% — an 11-16 percentage-point Kazakh advantage across all five frontier/large models.
>
> **Numbers:** per-lang Q counts: kk 700, uz 700, az 700, tr 700, tt 700, ky 598, ug 494, crh 316, kaa 215; 5-shot: Claude kk 83.0/uz 69.1, GPT-4o kk 81.0/uz 65.4, Gemini1.5Pro kk 78.4/uz 65.1, Qwen2.5-72B kk 62.6/uz 50.4, Llama3.1-70B kk 56.4/uz 45.3
> **Relevance:** This is the single most direct published cross-Turkic head-to-head for the atlas's Kazakh-vs-family positioning (decision 2): Kazakh is measurably AHEAD of Uzbek on native knowledge MCQ, not behind, contrary to a naive 'Kazakh is the laggard' framing. Extraction came from a tool-summarized HTML pass, not raw text — recommend re-verifying Table 2 exact digits directly from the PDF before citing in a paper.
> **Source:** arXiv:2502.11020 (fetched via WebFetch summarization of HTML version, table numbers reproduced as extracted — not independently cross-checked against raw PDF table) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-uzbek-non-kazakh-turkic-nlp-lands
> [uz][tr][pan-turkic] The TUMLU paper attributes part of the Kazakh-vs-Uzbek/Turkish gap to test-design difficulty, not resource availability: 'Uzbek and Turkish datasets are particularly difficult because those questions are designed specifically to imitate university entrance examinations,' and separately finds 'low-resource languages such as Crimean Tatar, Karakalpak, and Uyghur have comparable performance to middle- and high-resource languages' — i.e. TUMLU scores do not cleanly rank by corpus size.
>
> **Numbers:** n/a (qualitative claim from paper text)
> **Relevance:** Warns against using raw TUMLU-mini rankings alone as a resource-ratio proxy in the atlas; the survey should separate 'test difficulty' from 'model/resource capability' when positioning Kazakh vs Uzbek vs Karakalpak/Uyghur/Crimean Tatar.
> **Source:** arXiv:2502.11020 (WebFetch summarization) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-kyrgyz-non-kazakh-turkic-nlp-land
> [ky][kk][az][uz][tt][ug][kaa] TUMLU-mini (already in KB) covers Kyrgyz among its 8 natively-authored Turkic languages (38,139 4-choice questions, 11 subjects); no ≤1B model has been evaluated on it and the Kazakh subset (700 Q) tops out at Gemma-2-9B 49.1 among small-open models — Kyrgyz-specific per-language scores were not extracted in this sweep and should be pulled from the full leaderboard table before using as a design input.
>
> **Numbers:** 8 Turkic langs, 11 subjects, 38,139 Qs total; Kazakh subset 700 Q, best small-open Gemma-2-9B 49.1
> **Relevance:** TUMLU is the one pan-Turkic knowledge benchmark already claiming cross-lingual generative-eval territory; the lab should check whether its Kyrgyz subset is large/clean enough to reuse instead of building a bespoke Kyrgyz MC-QA set.
> **Source:** arXiv:2502.11020 (TUMLU, 2025) — extending KB entry · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [pan-turkic] TUMLU (ACL Findings/arXiv:2502.11020, native-authored MCQA, 38,139 Qs, 11 subjects, 8 languages: Azerbaijani/aze, Crimean Tatar/crh, Karakalpak/kaa, Kazakh/kaz, Kyrgyz/kir, Tatar/tat, Turkish/tur, Uzbek/uzb) gives the only cross-Turkic ranking with exact per-language scores. 5-shot mean accuracy ranking (Claude 3.5 Sonnet): tur 85.7 > aze 84.4 > tat 84.0 > kaz 83.0 > crh 81.2 > kir 75.7 > kaa 75.3 > uig 71.3 > uzb 69.1 (mean 78.9). For the SMALLEST open model tested (Llama-3.1-8B), Kazakh is the SINGLE HIGHEST-scoring language (46.4, mean 40.3), and Gemma-2-9B also puts Kazakh above its own mean (49.1 vs 47.1) — i.e. Kazakh's relative advantage concentrates in the small/mid model regime, not the frontier regime where Azerbaijani/Turkish/Tatar lead.
>
> **Numbers:** Claude 3.5 Sonnet per-lang: aze 84.4, crh 81.2, kaa 75.3, kaz 83.0, kir 75.7, tat 84.0, tur 85.7, uig 71.3, uzb 69.1 (mean 78.9). Llama-3.1-8B: aze 48.4, crh 35.7, kaa 33.7, kaz 46.4 (HIGHEST), kir 41.8, tat 44.1, tur 47.7, uig 35.0, uzb 29.9 (mean 40.3). Gemma-2-9B: kaz 49.1 vs mean 47.1.
> **Relevance:** Directly answers decision (2): quantifies exactly where Kazakh sits in the Turkic family, and shows its comparative edge is strongest precisely in the ≤~9B open-model regime the lab's ≤600M model is adjacent to — a defensible, sourced atlas claim ('best-learnable mid/small-model Turkic language') rather than a vague ranking.
> **Source:** arXiv:2502.11020v2 (TUMLU), Table 2, fetched directly · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [uz][az][kaz][crh][kaa][ug] FineWeb2 script/word counts per language (as reported inside the TUMLU paper) give a directly comparable resource ladder: Kazakh 1,837,049,585 Cyrillic words / 0 Latin (100% Cyrillic); Uzbek 616,563,348 Latin + 492,264,125 Cyrillic (≈1.109B total, ≈56%/44% split); Crimean Tatar 21,365,608 Latin + 1,934,168 Cyrillic (≈23.3M total, 11:1 Latin:Cyrillic). Uyghur has ~0 presence in FineWeb2 (virtually all Uyghur text is Arabic-script, outside this corpus's script coverage).
>
> **Numbers:** kaz 1.837B (100% Cyr); uzb 616.6M Latin + 492.3M Cyr = 1.109B; crh 21.37M Latin + 1.93M Cyr = 23.3M
> **Relevance:** Decision (2): gives an exact, sourced resource-ratio ladder (kaz ≈1.7x uzb ≈79x crh) for the atlas's 'who is ahead on data volume' axis, using one single corpus so the comparison is apples-to-apples (unlike mixing curated corpora of different provenance).
> **Source:** arXiv:2502.11020v2 (TUMLU), Section 5 body text, citing Penedo et al. 2024 FineWeb2 · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-other-langs-non-kazakh-turkic-nlp
> [uz] Uzbek is the WORST- or near-worst-performing language in TUMLU across nearly every model tested despite having more raw web text (FineWeb2 ≈1.1B words) than Kazakh's dedicated slice methodology would predict, and despite Tahrirchi's TahrirchiBERT being trained on ~5B tokens. This is consistent with Uzbek text being split roughly 56%/44% between Latin and Cyrillic scripts (vs Kazakh's ~100% Cyrillic concentration), which may fragment effective per-script training signal even though total-language volume is large.
>
> **Numbers:** uzb lowest in 3 of 4 models shown in Table 2 mean row context; FineWeb2 Uzbek Latin/Cyrillic split 616.6M/492.3M words
> **Relevance:** Directly informs decision (1): before porting the pinned eval protocols/Less-is-More recipe to Uzbek for the live collaboration, the script-split confound (not code-switching, which is Kazakh's issue) should be isolated — recommend a controlled ablation (Cyrillic-only vs Latin-only vs mixed Uzbek fine-tune) rather than assuming the Kazakh kk/ru code-switch lesson transfers as-is.
> **Source:** arXiv:2502.11020v2 Table 2 (Claude 3.5 Sonnet uzb 69.1, lowest of 8; Qwen2.5-72B uzb 44.1, lowest; Llama-3.1-8B uzb 29.9, lowest); TahrirchiBERT 5B-token claim via web search of Tahrirchi HF/GitHub pages · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [crh] Crimean Tatar's script-performance pattern is the OPPOSITE of Kazakh's and offers the closest available empirical natural-experiment for Kazakh's pending 2031 Latin transition: Crimean Tatar (FineWeb2: 21.37M Latin words vs only 1.93M Cyrillic, 11:1 ratio) scores markedly HIGHER when queried in Latin script (Claude 80.0 vs Cyrillic 66.1, a 13.9pp gap; Qwen2.5-72B 61.8 Latin vs 47.6 Cyrillic, 14.2pp; Gemma-2-27B 49.8 Latin vs 43.5 Cyrillic). Kazakh shows the mirror-image but SMALLER gap favoring Cyrillic (its dominant script today): Claude 82.7 Cyr vs 78.0 Latin (4.7pp); Qwen2.5-72B 64.3 Cyr vs 54.1 Latin (10.2pp); Gemma-2-27B 58.5 Cyr vs 46.3 Latin (12.2pp).
>
> **Numbers:** Crimean Tatar: Claude Latin 80.0/Cyr 66.1; Qwen72B Latin 61.8/Cyr 47.6; Gemma27B Latin 49.8/Cyr 43.5. Kazakh: Claude Cyr 82.7/Latin 78.0; Qwen72B Cyr 64.3/Latin 54.1; Gemma27B Cyr 58.5/Latin 46.3
> **Relevance:** Decision (2)/atlas: quantifies the real accuracy tax Kazakh should expect on Latin-script queries even TODAY (5-12pp, despite near-zero Latin web presence, via generalization/transliteration) and gives a same-family reference point (Crimean Tatar's 14pp Latin-favoring gap) for forecasting how large the transition-era penalty could grow before web corpora rebalance post-2031.
> **Source:** arXiv:2502.11020v2 Table 6, fetched directly · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-other-langs-non-kazakh-turkic-nlp
> [pan-turkic] The TUMLU paper's own text states 'TUMLU covers 8 Turkic languages... some major Turkic languages, such as Turkmen, Kyrgyz and Bashkir are not included' — but Kyrgyz (kir) demonstrably IS one of the 8 languages with full results throughout the paper's tables. This is an internal inconsistency in the source paper (likely a drafting error), not a lab measurement error.
>
> **Numbers:** n/a — textual contradiction: Kyrgyz appears in Table 2 (kir column, e.g. Claude 75.7) despite being listed as excluded
> **Relevance:** Flag so the atlas doesn't propagate this contradiction; Turkmen and Bashkir ARE genuinely absent from TUMLU and remain uncovered by any native MCQA benchmark.
> **Source:** arXiv:2502.11020v2, 'Missing major languages' paragraph vs Table 2/Figure 1 · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [ug] Uyghur shows the same native-script advantage pattern as Kazakh/Crimean Tatar but in Arabic script: TUMLU Table 6 shows Claude 3.5 Sonnet scoring Arabic 70.8 vs Latin 64.5 (Cyrillic not evaluated/used), Qwen2.5-72B Arabic 56.1 vs Latin 53.4, Gemma-2-27B Arabic 42.2 vs Latin 36.0 — the native/majority script consistently wins by 3-8pp across models, mirroring Kazakh's Cyrillic advantage. No dedicated Uyghur generative LLM or embedding/retrieval model was found; the main documented resources are the historical Uyghur-Chinese bilingual corpus (diaspora/historical, not modern web text) and the MC2 corpus used only for language-ID testing.
>
> **Numbers:** Uyghur Claude: Arabic 70.8 / Latin 64.5; Qwen72B: Arabic 56.1 / Latin 53.4; Gemma27B: Arabic 42.2 / Latin 36.0. TUMLU uig subset: 519 questions, low-resource group, mean rank 2nd-lowest of 8 (Claude 71.3)
> **Relevance:** Cross-checks the atlas's script-effect argument across a THIRD script family (Arabic, not just Cyrillic/Latin) — strengthens the general claim that native/majority-script training data drives accuracy regardless of which script it is, useful boilerplate for the Latin-transition risk section.
> **Source:** arXiv:2502.11020v2 Table 6; web search for Uyghur NLP 2025-2026 corpus/model (no modern dedicated LM found) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [kaa] Karakalpak's TUMLU subject breakdown reveals an anomaly not seen in other languages: Claude 3.5 Sonnet scores very high on general knowledge subjects (Biology 78.0, Chemistry 85.7, Physics 95.6) but collapses on Native Language & Literature specifically (42.2, vs 70-90 range for other languages on the same subject) — the opposite pattern from what data-quantity alone would predict, since Karakalpak has the smallest FineWeb2/curated footprint of the low-resource group (~2.2M words, bekan/karakalpak_corpus_v2_m, MIT license, 135,667 docs, Latin script).
>
> **Numbers:** Karakalpak Claude 3.5: Biology 78.0, Chemistry 85.7, Geography 75.0, NL&L 42.2, Physics 95.6 (History/Maths missing entirely — no questions in those subjects for this language); monolingual corpus 135,667 docs, ~2.2M words, 21.4MB, MIT license
> **Relevance:** Decision (3)/atlas: flags that 'general knowledge' MCQA and 'native language & literature' MCQA can diverge sharply within one low-resource language, meaning a single aggregate score (as often reported) can mask subject-specific data gaps — worth noting if the lab designs its own Kazakh subject-wise breakdown for KazMMLU-style reporting.
> **Source:** arXiv:2502.11020v2 Table 3; HF dataset bekan/karakalpak_corpus_v2_m fetched directly · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> TUMLU is the widest native (non-machine-translated) Turkic MMLU-style benchmark: 9 languages [tr][az][uz][kk][ky][tt][crh][ug][kaa], 38,139 MCQs across 11 subjects (Maths, Physics, Chemistry, Biology, Geography, Native Language & Literature, History, + 4 excluded from main experiments for limited coverage: Logic, Philosophy, Religion & Ethics, Human & Society). TUMLU-mini = manually-verified, ~100 Q/subject/language subset. Evaluated 5-shot and 5-shot-CoT.
>
> **Numbers:** 9 langs, 38,139 Q, 11 subjects (7 used), 5-shot / 5-shot-CoT
> **Relevance:** Direct protocol comparator: TUMLU uses 5-shot, the lab's KazMMLU protocol is 3-shot dev-limited — NOT directly comparable without re-running under evallab's pinned shot count. TUMLU-mini's per-language MCQ format is portable to Uzbek/Kyrgyz with the lab's existing KazMMLU harness design.
> **Source:** arXiv:2502.11020 (ACL 2025), https://arxiv.org/html/2502.11020, https://github.com/ceferisbarov/TUMLU · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-pan-benchmarks-non-kazakh-turkic
> TUMLU-mini 5-shot Claude-3.5-Sonnet scores by language rank Kazakh mid-pack, not last: Turkish 85.7% [tr] > Azerbaijani 84.4% [az] > Kazakh 83.0% [kk] > ... > Karakalpak 75.3% [kaa] > Uyghur 71.3% [ug] > Uzbek 69.1% [uz] (worst).
>
> **Numbers:** tr 85.7 / az 84.4 / kk 83.0 / kaa 75.3 / ug 71.3 / uz 69.1 (Claude-3.5-Sonnet, 5-shot)
> **Relevance:** For the atlas's Kazakh-vs-Turkic-family positioning: on a frontier proprietary model, Kazakh is NOT the weak link among Kipchak languages — Uzbek (Karluk) and Uyghur score lower despite Uzbek's larger population, likely reflecting weaker native educational-text digitization; useful counter to a naive 'Kazakh is behind Turkish' narrative.
> **Source:** arXiv:2502.11020 (TUMLU), Table of per-language results · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-models
> [kk][tr][az][crh][kaa][kir][tat][ug] TUMLU-mini per-language results for Claude 3.5 Sonnet (5-shot, native scripts): Turkish 85.7 (highest), Azerbaijani 84.4, Tatar 84.0, Kazakh 83.0, Crimean Tatar 81.2, Karakalpak 75.3, Uyghur 71.3, Uzbek 69.1 (LOWEST) — mean 79.3 across all 9.
>
> **Numbers:** tur 85.7, aze 84.4, tat 84.0, kaz 83.0, crh 81.2, kaa 75.3, uig 71.3, uzb 69.1, mean 79.3
> **Relevance:** Directly answers decision (2): Kazakh ranks 4th of 9 Turkic languages tested (mid-pack, ahead of Karakalpak/Uyghur/Uzbek, behind Turkish/Azerbaijani/Tatar) on a frontier model — gives the atlas a concrete, citable resource/performance ranking. Counter-intuitively Uzbek scores LOWEST despite being classed 'moderately-resourced' by TurkicNLP — worth flagging as an open question (script-transition effects? Latin-script Uzbek tokenization/data scarcity vs Cyrillic peers?) rather than assuming Uzbek is NLP-ready just because it has more monolingual model efforts.
> **Source:** github.com/ceferisbarov/TUMLU (Table 2 data, arXiv:2502.11020) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-reconcil
> [az][kk][tr][uz][ky][uig][kaa][crh(Crimean Tatar)][tt] On TUMLU-mini (native-language-authored, non-translated, 4-choice MCQA across 8 Turkic languages, 5-shot), Azerbaijani BEATS Kazakh on every one of the 5 evaluated models, not the reverse: Claude-3.5-Sonnet az 84.4 vs kk 83.0; GPT-4o az 82.4 vs kk 81.0; Gemma-2-9B az 53.7 vs kk 49.1; Llama-3.1-8B az 48.4 vs kk 46.4; Qwen2.5-7B az 48.0 vs kk 45.0. The paper's own difficulty caveat ('Uzbek and Turkish datasets are particularly difficult because those questions are designed to mirror university entrance examinations') applies to Uzbek/Turkish, NOT to Azerbaijani/Kazakh — both of which the paper says derive from 'community-developed materials with varying rigor' — so the Az>Kk gap is NOT explained away by the paper's stated confound; it stands as a genuine (if modest, 1.4-4.6pp) Azerbaijani edge on the one native-authored shared benchmark that exists.
>
> **Numbers:** Az vs Kk per model: Claude 84.4/83.0; GPT-4o 82.4/81.0; Gemma-2-9B 53.7/49.1; Llama-3.1-8B 48.4/46.4; Qwen2.5-7B 48.0/45.0. TUMLU-mini per-lang Q counts: az 700, kk 700, tr 700, uz 700, ky 698, tt 700, crh 417, kaa 215, uig 494.
> **Relevance:** This directly falsifies the sweep's prior framing that Kazakh is '#1' on curated-task accuracy — on the one benchmark built for genuinely fair cross-Turkic comparison, Azerbaijani is ahead, not Kazakh. The atlas cannot claim Kazakh leads on the accuracy axis.
> **Source:** TUMLU: A Unified and Native Language Understanding Benchmark for Turkic Languages (arXiv:2502.11020 / ACL 2025), Table 2, verified via direct fetch of arxiv.org/html/2502.11020. · **Sweep:** `turkic-landscape`

> [!note] CLAIM — non-kazakh-turkic-nlp-landscape-reconcil
> [uz] Uzbek's raw web footprint is surprisingly SMALL relative to its ~34-35M speaker population (roughly 2.5-2.7x Kazakh's ~13M speakers): FineWeb2 shows Uzbek (uzn_Latn+uzn_Cyrl combined, reflecting the ongoing Latin/Cyrillic script split) at only 2.62M docs/4.05 GB, LESS than Kazakh's 3.38M docs/6.86 GB despite the larger population — and Uzbek scores WORST of the 4 major Turkic languages on TUMLU-mini (69.1-36.1 range across models, below Kazakh/Azerbaijani/Turkish on every model). This is relevant to the live Uzbek collaboration offer: Uzbek is comparably or more resource-constrained than Kazakh on raw web text, meaning KazQAD-style retrieval and the Less-is-More embedding recipe would face an EQUALLY or MORE severe low-resource regime porting to Uzbek, not an easier one.
>
> **Numbers:** uz FineWeb2 combined 2.62M docs/4.05GB vs kk 3.38M docs/6.86GB; uz TUMLU: Claude 69.1, GPT-4o 65.4, Gemma-2-9B 36.1, Qwen2.5-7B 34.6, Llama-3.1-8B 29.9 (lowest of az/kk/tr/uz on every model)
> **Relevance:** Directly informs Decision 1 (which Turkic language to port protocols to first) — Uzbek is not a 'higher-resource, easier port' target; a lab port there inherits comparable data scarcity to Kazakh plus a Latin/Cyrillic script bifurcation the Kazakh work does not have to handle (yet).
> **Source:** HF datasets-server fineweb-2 per-config size query (uzn_Latn, uzn_Cyrl); TUMLU Table 2 (arXiv:2502.11020). · **Sweep:** `turkic-landscape`

## Related
- [[huggingface-co-datasets-mbzuai-kazmmlu-dataset-inspection|huggingface.co/datasets/MBZUAI/KazMMLU (dataset inspection 2026-07-03)]] — KazMMLU and TUMLU are parallel MMLU-style native benchmarks for Turkic languages; TUMLU covers the same regional-knowledge evaluation niche

[[Home]]
