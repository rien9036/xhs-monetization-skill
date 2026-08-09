---
name: xhs-monetization-skill
description: 将小红书商业目标转换为定位、需求选题、有效内容、流量增长、变现设计、运营诊断与 AI 内容工作流的一体化 Skill；涉及平台规则、产品入口、限制与价格时要求核验当前状态。
---

# XHS Monetization Skill

## Purpose

把“做小红书”转换为一条有商业目标、有需求承接、有内容转化、有交易闭环、可持续复盘的运营流程。

本 Skill 会先判断用户当前处于哪一环，再在内部选择所需方法完成任务。

## Core operating model

先理解业务目标、目标用户和交易路径，再以商业定位为起点，以需求和选题为核心，用内容完成“被看见 → 被点击 → 被互动 → 被咨询 → 成交”的转化链路，最后用数据复盘提升结果。

## Single-skill model

这是一个**单一 Skill**。用户只安装、调用根目录的 `SKILL.md`。原先拆分的能力已变成本 Skill 的内部方法，并放在 `references/methods/` 中供按需读取。

不要要求用户记忆或手动调用内部方法。根据任务自动选择最小必要方法；复杂任务可以组合多个方法。

## Internal method routing

- **Strategy & Positioning** (`strategy-positioning`)：不知道做什么账号、卖什么、商业目标或定位不清 → 读取 `references/methods/strategy-positioning.md`
- **Demand & Topic Map** (`demand-topic-map`)：不知道写什么、用户需求/关键词/长尾词不清 → 读取 `references/methods/demand-topic-map.md`
- **Effective Note** (`effective-note`)：要写或改标题、封面、正文、评论区与交易型笔记 → 读取 `references/methods/effective-note.md`
- **Traffic & Growth** (`traffic-growth`)：流量、搜索、点击、互动或涨粉不理想 → 读取 `references/methods/traffic-growth.md`
- **Monetization Design** (`monetization-design`)：有流量但不赚钱，或要设计服务/广告/电商路径 → 读取 `references/methods/monetization-design.md`
- **Operations Diagnostics** (`operations-diagnostics`)：要诊断账号、做日控/周复盘或找漏斗卡点 → 读取 `references/methods/operations-diagnostics.md`
- **AI Content Workflow** (`ai-content-workflow`)：要用 AI 辅助需求分析、选题、标题或内容生产 → 读取 `references/methods/ai-content-workflow.md`

### Reference loading rule

- 单点任务只读取直接相关的 1–2 个方法文件。
- 端到端规划按工作流逐步读取所需方法，不一次性加载全部 references。
- `references/` 中的框架、检查清单、案例模式、指标和平台时效性说明，只在任务需要时读取。

## End-to-end workflow

**目的 → 量化目标 → 交易路径 → 商业定位 → 账号表达 → 需求图谱 → 选题库 → 笔记生产 → 流量与互动 → 变现承接 → 数据复盘**

## Task selection rules

- 单点问题：只执行完成任务所需的最小内部方法。
- 从 0 到 1：按端到端工作流推进。
- 前置条件未成立：优先修复前置问题，不机械执行后续增长动作。
- 涉及当前平台功能、门槛、费用、权限或审核规则：先核验当前官方状态。

## Required outputs

完整规划至少输出：

- 商业目标与期限
- 目标人群与核心需求
- 产品/服务与交付方式
- 账号定位表达
- 对标研究方向
- 需求关键词地图
- 选题优先级
- 代表性笔记结构
- 从流量到交易的转化路径
- 核心数据指标与复盘规则
- 风险与需要核验的当前平台规则

## Guardrails

- 平台规则、流量机制、账号门槛、投放产品、私信限制、认证/店铺费用等可能变化，不能把历史经验直接当作当前事实。
- 不把规避平台检测、伪造互动、刷量、虚构身份或诱导欺骗作为推荐动作。
- 案例中的收入、转化率、粉丝增长或投放结果仅用于理解模式，不构成结果保证。
- 经验性概率判断只能作为启发，不能包装成平台算法或统计定律。

## References

- `references/capability-map.md` — 内部能力地图与对应方法文件。
- `references/methods/` — 各内部方法的详细执行流程；不是独立 Skills。
- `references/case-patterns.md`
- `references/checklists.md`
- `references/frameworks.md`
- `references/versioning-and-compliance.md`
