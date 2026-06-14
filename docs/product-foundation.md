# oss-doctor Product Foundation

## Intake

- Priority: P3
- Status: v0.1.0 deferred repo-health decision and mcp-risk-index dimension source
- Positioning: GitHub repository health analysis is deferred unless it directly supports MCP risk evidence.
- Primary route: Product -> Architecture -> Expert/Security -> QA -> Implementation -> Completion readiness

## PRD

### Problem

Avoid a generic repo health analyzer that weakens the Safe Agent Operations signal.

### Users

- Developers adopting AI agents or MCP tools
- Platform, DevTools, Security, and AI infrastructure teams
- Maintainers who need reviewable evidence rather than vague AI automation claims

### Goals

- allowed dimensions
- rejected generic checks
- risk-index mapping
- evidence criteria

### Non-Goals

- not a generic OSS scorecard
- not a dependency dashboard
- not a broad GitHub analytics product

### Acceptance Criteria

- The project can explain its place in Safe Agent Operations in one sentence.
- The first production surface is local-first or review-first, not a hosted dashboard by default.
- Reports, packets, indexes, or labs must be redaction-safe by design.
- Every risky claim links to evidence, rule logic, or an explicit limitation.
- The repository explicitly defers generic OSS scorecards.
- Allowed repo-health dimensions map to `mcp-risk-index` evidence fields.
- Governance defines how repository-health facts are absorbed, rejected, watched, or reconsidered without creating scores.

## Architecture Brief

### Boundaries

- Keep shared workflow knowledge in OPT; keep project-specific decisions in this repository.
- Keep the main entrypoint small and explicit.
- Prefer file-based artifacts over hidden services for the first production surface.

### Data Flow

```text
repo-health idea -> evidence-backed dimension check -> move to mcp-risk-index / watch / reject / reopen
```

### Risks

- Overclaiming safety guarantees.
- Creating generic tooling that weakens the Agentic DevSecOps signal.
- Accepting real secrets or private user data into fixtures.

## QA Plan

- Verify no docs imply a generic scorecard exists.
- Verify every kept dimension has evidence source and destination.
- Verify dimensions do not create unsupported trust or safety labels.
- Keep bilingual README guidance aligned.

## Implementation Plan

1. Keep this as a decision repository until reopen criteria are met.
2. Move useful dimensions into `mcp-risk-index`.
3. Reject generic repo-health scoring ideas.
4. Run the governance contract before each `mcp-risk-index` catalog release.
5. Use feature branches named `docs/<scope>`.
6. Use Conventional/Angular commits such as `docs: define risk index dimensions`.
7. Never push directly to `main`; open a pull request from the feature branch.

## Skipped Inputs

- mcp-risk-index need for repo-health dimensions
