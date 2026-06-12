# oss-doctor

语言： [English](./README.md) | 中文

GitHub repo 健康度分析暂缓，除非直接服务 MCP 风险证据。

## 状态

`v0.1.0` - deferred repo-health decision 和 mcp-risk-index dimension source。

## 目的

Avoid a generic repo health analyzer that weakens the Safe Agent Operations signal.

## 第一生产化表面

Decision log 和可复用 repo-health dimensions，用于 `mcp-risk-index`。

v0.1.0 明确不发布泛 OSS scorecard、dashboard 或 CLI。

## 必要证据

- allowed dimensions
- rejected generic checks
- risk-index mapping
- evidence criteria

## 决策

泛 repository health analysis 暂缓。只保留能直接支持 MCP risk review 的证据型维度。

## 非目标

- not a generic OSS scorecard
- not a dependency dashboard
- not a broad GitHub analytics product

## OPT 运行模型

本项目通过 [ops/opt-overlay.md](./ops/opt-overlay.md) 引用共享 One Person Team 工作流。项目自己的约束放在 [ops/constraints](./ops/constraints)，可演进 skill 放在 [ops/skills](./ops/skills)。

## 暂缺输入

需要用户或真实世界数据补充的内容记录在 `../x-one-skipped-inputs.md`，不阻塞基础建设。

## 文档

- [产品基础](./docs/product-foundation.md)
- [Defer Decision](./docs/defer-decision.md)
- [Risk Index Dimensions](./docs/risk-index-dimensions.md)
- [Review Runbook](./docs/review-runbook.md)
- [OPT Overlay](./ops/opt-overlay.md)
- [生产约束](./ops/constraints/production.md)
- [主入口约束](./ops/constraints/main-entry.md)
- [Skill 演进](./ops/skills/evolution.md)
