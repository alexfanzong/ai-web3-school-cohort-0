# LUO: Legal Uncertainty Oracle

## Summary

LUO is a Bittensor subnet concept for mapping cross-jurisdiction legal risk. It does not try to produce a single legal answer. It identifies where legal certainty is not justified by the evidence.

One-line positioning:

> Chainlink tells you where the price is; LUO tells you where legal uncertainty is.

## Problem

The most dangerous failure mode in legal AI is not "I do not know." It is fabricated certainty: a model invents a non-existent statute, regulatory document, or citation and formats it as if it were authoritative.

For cross-border legal/compliance work, this is especially dangerous because the real answer is often jurisdiction-dependent, contested, or structurally uncertain.

## Intelligence Good

Cross-jurisdiction legal risk topology:

- source-grounded legal claims;
- citation-backed evidence extraction;
- jurisdictional disagreement mapping;
- uncertainty-preserving summaries.

## Miner Task

Miners extract evidence from a legal corpus and bind each legal claim to concrete documents.

## Validator Scoring

Validators score outputs through three dimensions:

- Citation existence: does the cited source actually exist?
- Synthetic trap detection: does the output rely on planted fake materials?
- Evidence boundary discipline: does the conclusion exceed what the evidence supports?

## Demo Case

Tornado Cash:

- United States
- Netherlands
- Switzerland
- Hong Kong

The same protocol can have different legal treatment across jurisdictions. LUO's product value is to preserve and visualize this difference instead of compressing it into one overconfident answer.

## Connection To Programmable Compliance

LUO can become a legal uncertainty layer for Programmable Compliance. Before a product, wallet, DAO, RWA transfer, or Agentic Commerce workflow executes a high-risk action, LUO-like systems can surface:

- which jurisdictional claims are grounded;
- which claims are disputed;
- where citations are missing or fabricated;
- where human legal review is required.

## Open Questions

- How should synthetic traps be generated without making the benchmark too gameable?
- How should validators handle legitimate legal ambiguity?
- What corpus governance process prevents the legal dataset from becoming stale?
- Should the product surface uncertainty as map, score, graph, or workflow gate?
