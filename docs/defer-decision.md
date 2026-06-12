# Defer Decision

## Status

Accepted for v0.1.0.

## Decision

Do not build `oss-doctor` as a generic repository health scorecard or GitHub analytics product.

Keep only repository-health dimensions that directly support MCP risk evidence in `mcp-risk-index`.

## Why

Generic OSS health analysis is useful but too broad for X-One's market signal. It can easily become a repo-quality dashboard unrelated to Safe Agent Operations.

The useful wedge is:

> factual maintenance and provenance signals that help reviewers reason about MCP server adoption.

## Allowed Scope

Allowed dimensions must be factual, evidence-backed, and useful to `mcp-risk-index`:

- repository URL
- source checked date
- archived status
- recent push date
- release or package pinning notes
- maintainer-provided security policy link
- license presence
- documented install command

## Rejected Scope

- overall OSS health score
- popularity ranking
- contributor quality rating
- generic dependency dashboard
- broad GitHub analytics
- subjective trust label

## Reopen Criteria

Reconsider a standalone `oss-doctor` only if:

- 5 or more target users ask for repo-health evidence independent of MCP adoption.
- The requested dimensions are still evidence-backed and not a subjective score.
- The product creates a stronger Agentic DevSecOps signal than `mcp-risk-index` integration.
- A narrow CLI/report can be validated with real repository fixtures.

## Current Outcome

`oss-doctor` remains a decision repository. Useful facts should be added to `mcp-risk-index` catalog governance or entries.
