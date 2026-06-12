# oss-doctor

Languages: English | [中文](./README.zh-CN.md)

GitHub repository health analysis is deferred unless it directly supports MCP risk evidence.

## Status

`P3` - deferred decision repository.

## Purpose

Avoid a generic repo health analyzer that weakens the Safe Agent Operations signal.

## First Production Surface

Decision log and reusable repo-health dimensions for mcp-risk-index.

## Required Evidence

- allowed dimensions
- rejected generic checks
- risk-index mapping
- evidence criteria

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
- [OPT Overlay](./ops/opt-overlay.md)
- [Production Constraints](./ops/constraints/production.md)
- [Main Entry Constraints](./ops/constraints/main-entry.md)
- [Skill Evolution](./ops/skills/evolution.md)
