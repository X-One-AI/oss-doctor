# oss-doctor

语言： [English](./README.md) | 中文

GitHub repo 健康度分析暂缓，除非直接服务 MCP 风险证据。

## 状态

`P3` - deferred decision repository。

## 目的

Avoid a generic repo health analyzer that weakens the Safe Agent Operations signal.

## 第一生产化表面

Decision log and reusable repo-health dimensions for mcp-risk-index.

## 必要证据

- allowed dimensions
- rejected generic checks
- risk-index mapping
- evidence criteria

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
- [OPT Overlay](./ops/opt-overlay.md)
- [生产约束](./ops/constraints/production.md)
- [主入口约束](./ops/constraints/main-entry.md)
- [Skill 演进](./ops/skills/evolution.md)
