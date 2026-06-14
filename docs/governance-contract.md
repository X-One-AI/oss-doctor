# Governance Contract

`oss-doctor` is a deferred decision repository. Its job is to preserve useful repository-health facts only when they directly improve MCP risk review.

## Portfolio Role

This repository must strengthen `mcp-risk-index` evidence without becoming a generic OSS scorecard.

Allowed output:

- factual maintenance dimensions for MCP server catalog entries
- evidence-source requirements for repository metadata
- limitation wording for stale, missing, or ambiguous repository signals
- explicit reject decisions for generic health scoring
- review notes that feed `mcp-risk-index` catalog governance

Disallowed output:

- overall OSS health score
- popularity ranking
- contributor quality rating
- generic dependency dashboard
- broad GitHub analytics product
- trusted, safe, unsafe, or abandoned labels based on repository metadata alone

## Absorption Contract

Move an idea out of this repository when it can improve `mcp-risk-index` evidence.

| Candidate Shape | Required Evidence | Destination Artifact |
|---|---|---|
| maintenance fact | public repository metadata and checked date | `mcp-risk-index` catalog field or limitation note |
| provenance fact | repository URL, package source, or maintainer-provided link | catalog governance issue or docs update |
| install evidence | documented command or package metadata | catalog entry or fixture update |
| security reporting fact | public `SECURITY.md` or maintainer policy URL | limitation/evidence note |

Absorbed ideas should leave this repository once a destination issue or PR exists. Keep only the link and decision note.

## Rejection Contract

Reject or delete an idea when any are true:

- it produces a score, rank, or subjective trust label
- it relies on popularity as a proxy for safety
- it cannot name a public evidence source
- it is useful only as broad repository analytics
- it makes `mcp-risk-index` look like a safety certification

Watch-only ideas must name the exact missing public evidence. If no destination field or limitation wording appears after two catalog reviews, delete the idea.

## Review Cadence

Run this governance review before every `mcp-risk-index` catalog release and after every public sample refresh.

Review questions:

1. Which facts should become catalog fields, maintenance notes, or limitation wording?
2. Which facts are too noisy and should be deleted?
3. Does any wording imply a safety, trust, or abandonment label?
4. Are source dates and public evidence links current enough for the release?
5. Did any local constraint or skill need strengthening, rewrite, or deletion?

## Reopen Gate

Reopen standalone repo-health analysis only when the criteria in `docs/defer-decision.md` are met and a new PRD proves the product is narrower and more valuable than `mcp-risk-index` integration.

Until then, this repository ships governance, not OSS health product behavior.
