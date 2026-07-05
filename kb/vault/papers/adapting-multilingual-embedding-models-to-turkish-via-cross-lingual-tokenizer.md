---
kb_id: "arxiv:2605.29992"
type: "paper"
title: "Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation"
arxiv_id: "2605.29992"
doi: null
hf_repo: null
year: 2026
topics: ["turkic-turkish", "turkic-other-langs-non-kazakh-turkic-nlp", "turkic-pan-benchmarks-non-kazakh-turkic", "turkic-pan-models", "turkic-nlp-landscape-cheap-tokenizer-sur"]
claims: 9
uncertain_claims: 1
verdicts: []
aliases: ["Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation", "arXiv:2605.29992", "arxiv:2605.29992"]
tags: ["paper", "topic/turkic-turkish", "topic/turkic-other-langs-non-kazakh-turkic-nlp", "topic/turkic-pan-benchmarks-non-kazakh-turkic", "topic/turkic-pan-models", "topic/turkic-nlp-landscape-cheap-tokenizer-sur"]
---
# Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation

[arXiv](https://arxiv.org/abs/2605.29992)
**Topics:** [[turkic-turkish]], [[turkic-other-langs-non-kazakh-turkic-nlp]], [[turkic-pan-benchmarks-non-kazakh-turkic]], [[turkic-pan-models]], [[turkic-nlp-landscape-cheap-tokenizer-sur]]

> [!abstract]
> Sentence embeddings are a foundational component for semantic search, clustering, classification, and retrieval-augmented generation. This paper presents embeddingmagibu-200m, a Turkish-focused sentence embedding model that produces 768-dimensional L2-normalized vectors and supports an 8,192-token context window, far exceeding the 512-token limit of earlier BERT-based Turkish encoders. Instead of …

## Claims

> [!note] CLAIM — turkic-turkish
> [tr] A 2026 paper distills EmbeddingGemma-300M into a 200M Turkish-specialized embedder via tokenizer surgery (build 128K vocab: top-64K Turkish tokens from Cosmos Turkish Corpus + pruned teacher tokens + frequency-selected multilingual Wikipedia tokens) + weight-preserving embedding remapping (mean-composition of teacher embeddings) + offline distillation (cosine-similarity loss on 580K examples: 100K Turkish + 100K English + 10K/language across 40-language Wikipedia). Result: the 200M student BEATS its 300M teacher on Turkish STS (STSbTR Pearson 77.55% vs 73.84%, +3.71pp) at 33% fewer params, for $5-20 / ~4 A100-GPU-hours, but loses slightly on full TR-MTEB average (63.9% vs teacher's 65.2%, -1.3pp; task-specific gains of +4.6pp STS, +7.3pp NLI).
>
> **Numbers:** 128K vocab (64K Turkish + pruned teacher + multilingual); 580K distillation examples; STSbTR 77.55/77.45 (student) vs 73.84/72.92 (teacher); TR-MTEB 63.9% vs 65.2%; cost $5-20, ~4 A100-hrs; 200M vs 300M params
> **Relevance:** A genuinely portable, CHEAPER alternative/complement to the lab's Less-is-More recipe for Kazakh: tokenizer surgery + distillation from a strong multilingual teacher (e.g. EmbeddingGemma or mE5) is untested on Kazakh and could be run as an ablation alongside the 10k-noisy-pairs Less-is-More protocol — same budget class ($5-20).
> **Source:** arXiv:2605.29992 (Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-other-langs-non-kazakh-turkic-nlp
> [tr] The only Turkic-language-validated cheap embedding-adaptation recipe found beyond mE5 fine-tuning is 'tokenizer surgery + offline distillation' (arXiv:2605.29992, embeddingmagibu-200m, Turkish): (1) build a Turkish-optimized 131,072-vocab tokenizer by pruning/extending a multilingual teacher's vocab via frequency analysis on a 40-language corpus, (2) clone the teacher backbone with mean-composition token-embedding initialization for new vocab, (3) offline cosine-similarity distillation from precomputed teacher vectors (no online teacher inference) over a balanced 40-language Wikipedia corpus. Result: a ~200M-param student BEATS its ~300M-param teacher on STSbTR (Pearson/Spearman 77.55/77.45 vs teacher's own 73.84/72.92), trains in ~4 GPU-hours for $5-$20 total, and supports an 8,192-token context (vs 512 for BERT-era Turkish encoders).
>
> **Numbers:** Tokenizer 131,072 vocab, 40-lang frequency analysis; student 200M params vs teacher 300M; STSbTR Pearson/Spearman: student 77.55/77.45 vs teacher 73.84/72.92; training ~4 GPU-hours, $5-$20; context 8,192 tokens
> **Relevance:** Decision (1): this is a CHEAPER (~$5-20 vs Less-is-More's <$20 for data but full-FT compute) and Turkic-in-family-validated alternative/complement to Less-is-More that the lab should benchmark head-to-head for the Kazakh/Uzbek embedding recipe choice, since Less-is-More itself has NEVER been tested on any Turkic language (per KB) while this recipe has.
> **Source:** arXiv:2605.29992, confirmed via search + WebSearch summary of abstract/results · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-benchmarks-non-kazakh-turkic
> A cheap tokenizer-surgery + offline-distillation recipe adapts a large multilingual embedder to a new language for ~$5-20 on a single A100 in ~4 hours: source=EmbeddingGemma-300M (768-dim, 256K vocab), target=embeddingmagibu-200m [tr] (768-dim, 128K vocab, ~200M params) via (1) extracting 64K frequent target-language tokens + merging with existing multilingual tokens = 128K vocab, (2) weight-preserving mean-composition cloning of new token embeddings from teacher, (3) offline distillation on precomputed teacher embeddings (cosine loss) over ~580K balanced 40-language Wikipedia examples. Result: 77.55% Pearson on STSb-tr (vs teacher's 73.84%, i.e. BEATS the teacher) and 63.9% avg on TR-MTEB (26 tasks, ranks 7th/26 models) at 98% of teacher performance with 33% fewer params.
>
> **Numbers:** cost $5-20, ~4h single A100; 580K training examples; STSb-tr 77.55% (student) vs 73.84% (teacher); TR-MTEB avg 63.9%, rank 7/26
> **Relevance:** This is a directly portable, near-zero-cost recipe for the lab's Kazakh embedding track: same tokenizer-surgery + offline-distillation approach applied to EmbeddingGemma-300M or mE5-large with a Kazakh-frequent-token vocabulary could produce a compact Kazakh-specialized embedder for roughly the same $5-20/4h budget — a concrete low-risk alternative or complement to the current mE5 Less-is-More plan, and the paper explicitly notes it has NOT been tested on other Turkic languages (fully open for Kazakh/Uzbek as a first-mover).
> **Source:** arXiv:2605.29992 (Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-pan-models
> [tr] A distinct 2026 paper adapts EmbeddingGemma-300M (teacher, 256K vocab, 768-dim, 2048 ctx) to Turkish via 3-stage recipe: tokenizer surgery (prune/merge to 131,072-token vocab: 64K Turkish tokens from Cosmos Turkish Corpus + frequency-selected multilingual tokens from 40-language Wikipedia), weight-preserving mean-composition embedding init, then offline distillation on ~580K examples (Turkish/English capped at 100K each) with precomputed teacher vectors. Resulting ~200M-param student (embedding table cut from 196.6M to 100.6M params, ctx extended to 8,192) trains in ~4 hours on a single GPU for $5-20 total.
>
> **Numbers:** vocab 256K->131,072 (64K Turkish); student ~200M (embed table 196.6M->100.6M); ctx 2048->8192; ~580K distillation examples; ~4 GPU-hours; $5-20 cost; TR-MTEB: student 63.9 (7th/26) vs teacher 65.2 (4th/26), 33% fewer params for 98% of teacher score; STSbTR Pearson: student 77.55% vs teacher 73.84% (+3.71pp, student BEATS teacher)
> **Relevance:** A second, even cheaper (<$20, 4 GPU-hours) Turkish embedding adaptation recipe than Less-is-More, using tokenizer surgery + distillation rather than noisy-pair fine-tuning — worth comparing against Less-is-More as an alternative cheap adaptation path for Kazakh/Uzbek. Paper explicitly names Finnish/Hungarian/Korean as future generalization targets but NOT other Turkic languages — leaves kk/uz/ky tokenizer-surgery+distillation unclaimed, a possible lab artifact angle for decision (3).
> **Source:** arXiv:2605.29992 (Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation) · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-cheap-tokenizer-sur
> [tr] The tokenizer-surgery + offline-distillation recipe was validated EXCLUSIVELY on Latin-script Turkish (STSb-TR, TR-MTEB-26-tasks); the paper contains zero mention of Kazakh, Russian, or any Cyrillic-script language anywhere in the full text, and zero discussion of code-switching. Cross-script/Cyrillic transfer to Kazakh is entirely unestablished by the source paper itself — the 'transfers to Kazakh' recommendation is pure extrapolation, not evidence.
>
> **Numbers:** 0 mentions of Kazakh/Cyrillic/code-switching in full text; teacher=EmbeddingGemma-300M (256K SentencePiece vocab); student vocab pruned 256K->131,072
> **Relevance:** The Uzbek-collab and pan-Turkic porting decision needs evidence the recipe survives a script change (Cyrillic) plus a code-switching regime (kk/ru); neither exists. Treating this as validated-for-Kazakh would be citing a paper for something it never tested.
> **Source:** arXiv:2605.29992 (Bayram, Diri, Yıldırım, 'Adapting Multilingual Embedding Models to Turkish via Cross-Lingual Tokenizer Surgery and Offline Distillation', submitted 2026-05-28, preprint, CC BY-NC-SA 4.0, no peer-review venue stated); full-text checked at arxiv.org/html/2605.29992 · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-cheap-tokenizer-sur
> [tr] The recipe's teacher is EmbeddingGemma-300M, NOT mE5-base (the lab's canonical Less-is-More base) — so 'replacing Less-is-More with tokenizer-surgery' actually means swapping the base architecture (Gemma3 decoder-derived, 300M, 256K vocab) AND the recipe simultaneously, not a like-for-like recipe substitution on the same backbone.
>
> **Numbers:** Teacher: EmbeddingGemma-300M = 196.6M embedding params + 104.0M backbone, 768-dim output, 2,048-token input cap; Student: ~200M, 131,072 vocab, 8,192-token context
> **Relevance:** Any lab decision to adopt this recipe is really a decision to adopt EmbeddingGemma as teacher, which the lab's own KB already found to be a WEAKER low-resource-language performer than mE5 (see next finding) — this is a compounding risk, not a clean recipe swap.
> **Source:** arXiv:2605.29992 full text (arxiv.org/html/2605.29992), Methodology section · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-cheap-tokenizer-sur
> [tr] Within the surgery paper's own results, the student's gain over teacher is concentrated in STS (+4.6 abs, 77.5 vs 72.9) and NLI (+7.3 abs, 67.9 vs 60.6), but it LOSES to the teacher on Retrieval (72.2 vs 75.9, -3.7 abs) and on the overall TR-MTEB mean (63.9 vs 65.2, achieving only '98.0% of teacher'). Retrieval is precisely the axis the lab's canonical protocols (KazQAD, MTEB-style) are built around.
>
> **Numbers:** TR-MTEB: student 63.9% mean (rank 7/26), Retrieval 72.2%; teacher (EmbeddingGemma-300M) 65.2% mean (rank 4/26), Retrieval 75.9%; STSb-TR student 77.55/77.45 (P/S) vs teacher 73.84/72.92
> **Relevance:** Even in-distribution (Turkish, Latin script, the paper's best case) the recipe's demonstrated strength is semantic similarity/NLI, not retrieval — the wrong axis for the lab's canonical KazQAD-style deliverable.
> **Source:** arXiv:2605.29992 full text, Benchmark Results tables (STSb-TR, TR-MTEB 26 tasks) · **Sweep:** `turkic-landscape`

> [!warning] UNCERTAIN — turkic-nlp-landscape-cheap-tokenizer-sur
> [tr] The surgery paper's own stated limitation directly predicts Kazakh-specific failure: pruning vocab 256K->131,072 tokens 'reduces the model's capacity to represent non-target languages... performance on lower-resource non-target languages may degrade.' A Turkish-optimized 128K vocab was built by extracting the top 64K frequent tokens from a Turkish-only corpus (Cosmos Turkish Corpus) plus multilingual tokens from a 40-language Wikipedia frequency analysis (Kazakh not named as one of the 40). Applying the SAME (Turkish) tokenizer to Kazakh, rather than building a dedicated Kazakh-corpus vocab, would incur exactly this stated degradation; building a dedicated Kazakh version is unverified but architecturally analogous work, not yet done by anyone.
>
> **Numbers:** Vocab: 256K (teacher) -> 131,072 (student); 64K top-frequency Turkish tokens seeded from Cosmos Turkish Corpus; ~580K total distillation training rows (Turkish+English capped 100K each, other 38 languages capped 10K each)
> **Relevance:** For a Kazakh port, this is a build-from-scratch-tokenizer exercise (like SozKZ's from-scratch BPE, already in KB) grafted onto a distillation step — not a drop-in reuse of the published Turkish artifact. Feasibility is plausible given Kazakh/Turkish share Turkic agglutinative typology, but zero empirical evidence exists for the Kipchak branch (Kazakh) vs the paper's Oghuz branch (Turkish) target.
> **Source:** arXiv:2605.29992 full text, Limitations section + Tokenizer Construction section · **Sweep:** `turkic-landscape`

> [!note] CLAIM — turkic-nlp-landscape-cheap-tokenizer-sur
> [pan-turkic] No head-to-head between the tokenizer-surgery recipe and Less-is-More exists in the literature: arXiv:2605.29992 does not cite, benchmark against, or discuss 'Less is More' (arXiv:2603.22290) at all, despite both being 2026 low-cost embedding-adaptation papers. The two recipes are also not directly comparable on compute cost from published numbers: surgery = $5-20 total / ~4 hrs on 1x A100-80GB (fully documented); Less-is-More = <$20 for the translation/generation phase only (10k pairs via Gemini 2.5 Flash) with fine-tuning run on 16x MI250x GPUs but NO GPU-hours or wall-clock time disclosed for the fine-tune itself.
>
> **Numbers:** Surgery: $5-20, ~4 GPU-hrs, 1x A100-80GB. Less-is-More: <$20 (data-gen only, Gemini 2.5 Flash), fine-tune on 16x MI250x GPUs, batch 512, lr 7e-5, 5 epochs, GPU-hours unreported
> **Relevance:** The 'four researchers recommend adopting/benchmarking' claim has no literature support for a comparison — any head-to-head would be a genuinely novel evallab experiment, not a replication of a published result; cost claims used to justify a switch cannot currently be verified as apples-to-apples.
> **Source:** arXiv:2605.29992 full text (no citation of arXiv:2603.22290 found); arXiv:2603.22290 full text (arxiv.org/html/2603.22290), compute/training section · **Sweep:** `turkic-landscape`

**Cited KB notes:** [[less-is-more-adapting-text-embeddings-for-low-resource-languages-with-small]]

[[Home]]
