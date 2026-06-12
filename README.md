# oss-doctor

Languages: English | [中文](./README.zh-CN.md)

GitHub repository health analysis is deferred unless it directly supports MCP risk evidence.

## Status

`v0.1.0` - deferred repo-health decision and mcp-risk-index dimension source.

## Purpose

Avoid a generic repo health analyzer that weakens the Safe Agent Operations signal.

## First Production Surface

Decision log and reusable repo-health dimensions for `mcp-risk-index`.

This repository intentionally does not ship a generic OSS scorecard, dashboard, or CLI in v0.1.0.

## Required Evidence

- allowed dimensions
- rejected generic checks
- risk-index mapping
- evidence criteria

## Decision

Generic repository health analysis is deferred. Only evidence-backed dimensions that directly support MCP risk review remain in scope.

## Non-Goals

- not a generic OSS scorecard
- not a dependency dashboard
- not a broad GitHub analytics product

## OPT Operating Model

This project references the shared One Person Team workflow through [ops/opt-overlay.md](./ops/opt-overlay.md). Project-specific constraints live under [ops/constraints](./ops/constraints), and evolvable local skills live under [ops/skills](./ops/skills).

## Blocked Inputs

Inputs that require user or real-world data are recorded in `../x-one-skipped-inputs.md` and should not block foundation work.

## Docs

- [Product Foundation](./docs/product-foundation.md)
- [Defer Decision](./docs/defer-decision.md)
- [Risk Index Dimensions](./docs/risk-index-dimensions.md)
- [Review Runbook](./docs/review-runbook.md)
- [OPT Overlay](./ops/opt-overlay.md)
- [Production Constraints](./ops/constraints/production.md)
- [Main Entry Constraints](./ops/constraints/main-entry.md)
- [Skill Evolution](./ops/skills/evolution.md)
