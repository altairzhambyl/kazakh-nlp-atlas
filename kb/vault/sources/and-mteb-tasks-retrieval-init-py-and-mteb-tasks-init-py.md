---
kb_id: "title:and mteb tasks retrieval   init   py and mteb tasks   init   py"
type: "source"
title: "and mteb/tasks/retrieval/__init__.py and mteb/tasks/__init__.py"
doi: null
hf_repo: null
year: null
topics: ["mteb-upstream-contrib-process"]
claims: 1
uncertain_claims: 0
verdicts: []
aliases: ["title:and mteb tasks retrieval   init   py and mteb tasks   init   py"]
tags: ["source", "topic/mteb-upstream-contrib-process"]
---
# and mteb/tasks/retrieval/__init__.py and mteb/tasks/__init__.py

**Topics:** [[mteb-upstream-contrib-process]]

## Source URLs
- and mteb/tasks/retrieval/__init__.py and mteb/tasks/__init__.py

## Findings

> [!note] CLAIM — mteb-upstream-contrib-process
> Package __init__.py registration pattern: explicit re-export of every class name via __all__ list, then the parent mteb/tasks/retrieval/__init__.py does `from .rus import *` etc, and mteb/tasks/__init__.py does `from .retrieval import *`.
> **Source:** https://raw.githubusercontent.com/embeddings-benchmark/mteb/main/mteb/tasks/retrieval/rus/__init__.py and mteb/tasks/retrieval/__init__.py and mteb/tasks/__init__.py · **Sweep:** `2026-07-mteb-upstream-recon`

[[Home]]
