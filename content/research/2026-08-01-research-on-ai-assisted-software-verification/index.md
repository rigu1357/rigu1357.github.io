---
title: Research on AI-assisted software verification
slug: research-on-ai-assisted-software-verification
date: 2026-08-01
start: 2026-08-01
ongoing: true
org: UTEP, Dr. Marcelo Frias
role: Undergraduate Research Assistant
folio_id: 2026-08-01-research-on-ai-assisted-software-verification
summary: Building multi-agent AI pipelines to write and test specifications for the TACO verifier
---

I'm an undergraduate research assistant at UTEP working with Dr. Marcelo Frias on AI-assisted software verification. I design and run multi-agent AI pipelines for TACO, a SAT-based bounded bug-finding tool for Java. Each agent has a role: one checks that code is analyzable, one writes JML specifications, one generates mutants to expose weak specifications, and one audits the results.

I compare the pipeline against a single-prompt baseline on real open-source code (Apache Commons Collections), measuring correctness, cost, and runtime. A specification counts as correct only when TACO confirms it. To keep the results trustworthy and reproducible, I sandbox the agents away from answer keys, pin toolchain versions, and log every run.

Along the way I built TACO and its toolchain (DynAlloy, Alloy) from source and found problems in the tools themselves:

- Identified and reported 31 bugs, 8 of them soundness defects that could let real bugs go undetected
- Traced each bug to its root cause
- Wrote and validated fixes for 16, one of which was merged upstream
