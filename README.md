# 类 Manus 智能体平台 · 技术调研与设计文档

本仓库汇总了基于 **Higress + OpenCode + E2B** 构建大模型网关与类 Manus 智能体平台的全套调研与设计文档。

## 文档目录

| 文件 | 说明 |
| :--- | :--- |
| `docs/01_平台架构调研报告.md` | Higress、OpenCode、E2B 三大组件调研及整体平台架构设计 |
| `docs/02_多租户隔离与资源配额管理方案.md` | 多租户隔离机制、资源配额管理、RBAC 权限体系设计 |
| `docs/03_计费系统集成设计方案.md` | 计量数据采集、实时计量引擎、Stripe 计费与账单集成方案 |
| `docs/04_开发计划与人员安排.xlsx` | 2 个月开发计划甘特图、人员安排及里程碑计划 |

## 技术栈概览

- **大模型网关**：[Higress](https://higress.ai) — 基于 Istio/Envoy 的云原生 AI 网关，提供多模型路由、Token 限流、鉴权与可观测性。
- **智能体运行时**：[OpenCode](https://opencode.ai) — 开源 AI 编码 Agent，支持 MCP 工具协议与多模型接入。
- **沙箱执行环境**：[E2B](https://e2b.dev) — 基于 Firecracker microVM 的安全沙箱，为 Agent 提供隔离的代码执行环境。
- **计量引擎**：[OpenMeter](https://openmeter.io) — 开源实时计量平台，基于 Kafka + ClickHouse 架构。
- **支付与账单**：[Stripe Billing](https://stripe.com) — 支持按量计费、阶梯定价与预付费积分。

## 开发周期

**2026-05-01 ~ 2026-06-30（共 8 周）**

## 分支说明

- `main`：稳定版本
- `dev`：开发分支（当前分支）
