# XHS Monetization Skill

面向小红书商业化、内容增长与交易转化的一体化 AI Skill。

**这是一个单一 Skill。** 安装后只需要调用根目录 `SKILL.md`；所有专业能力都由它在内部自动选择，不需要分别安装或调用多个 Skills。

## Core Workflow

**目的 → 量化目标 → 交易路径 → 商业定位 → 账号表达 → 需求图谱 → 选题库 → 笔记生产 → 流量与互动 → 变现承接 → 数据复盘**

## Capabilities

- `strategy-positioning`：商业目标、交易路径、账号定位与对标研究
- `demand-topic-map`：需求图谱、关键词、长尾词与选题池
- `effective-note`：标题、封面、正文、评论区与交易型内容
- `traffic-growth`：搜索、推荐、互动、涨粉与付费放大判断
- `monetization-design`：服务、广告、电商等变现路径与单位经济
- `operations-diagnostics`：账号诊断、日控、复盘与实验设计
- `ai-content-workflow`：AI 辅助需求分析、选题与内容生产

以上名称只是内部能力模块。详细方法放在 `references/methods/`，用于按需加载，不是独立 Skills。

## Structure

```text
.
├── README.md
├── SKILL.md
└── references/
    ├── capability-map.md
    ├── case-patterns.md
    ├── checklists.md
    ├── frameworks.md
    ├── versioning-and-compliance.md
    └── methods/
        ├── strategy-positioning.md
        ├── demand-topic-map.md
        ├── effective-note.md
        ├── traffic-growth.md
        ├── monetization-design.md
        ├── operations-diagnostics.md
        └── ai-content-workflow.md
```

- `SKILL.md`：唯一 Skill 入口，负责理解任务、选择内部方法和组合完整工作流。
- `references/methods/`：详细方法库，仅供本 Skill 内部按需读取。
- 其他 `references/`：框架、检查清单、指标、案例模式与平台时效性资料。

# Installation

## Codex — Skill Installer

在 Codex 中可以让内置的 `$skill-installer` 安装该 GitHub 仓库根目录的 Skill：

```text
$skill-installer install the skill at the repository root from https://github.com/rien9036/xhs-monetization-skill
```

安装完成后，重新启动 Codex 或开启新的会话。

## Codex — Manual Install

macOS / Linux：

```bash
git clone https://github.com/rien9036/xhs-monetization-skill.git ~/.codex/skills/xhs-monetization-skill
```

安装后的核心结构：

```text
~/.codex/skills/xhs-monetization-skill/
├── SKILL.md
└── references/
```

## ChatGPT

如果你的 ChatGPT 账号或工作区支持 Skills：

1. 点击本仓库右上角 **Code → Download ZIP**。
2. 在 ChatGPT 的 Skills 页面选择 **Create → Upload from your computer**。
3. 上传下载的 Skill 包。

> Skills 的具体可用范围取决于当前账号、工作区权限和管理员设置。

## Other Agent Skills Clients

如果其他 Agent 支持以 `SKILL.md` 为入口的 Agent Skills，可以克隆整个仓库，并把根目录 `SKILL.md` 作为唯一入口：

```bash
git clone https://github.com/rien9036/xhs-monetization-skill.git
```

# Quick Start

安装后直接描述任务即可，不需要记忆内部方法名称。

```text
帮我从 0 到 1 规划一个以获客和成交为目标的小红书账号。
```

```text
根据我的产品和目标客户，建立需求关键词地图和 30 个优先选题。
```

```text
帮我优化这篇笔记，让它更接近咨询和成交目标。
```

```text
我的笔记有互动但没有咨询，帮我诊断漏斗卡点。
```

```text
帮我比较服务、广告和电商三种变现方式，并给出单位经济判断。
```

# How It Works

`SKILL.md` 会先判断当前问题属于哪个环节，只读取必要的内部方法。例如：

- 定位未明确时，不会直接跳到投流或规模化。
- 流量异常时，会先区分需求、包装、内容、分发还是承接问题。
- 有流量但商业结果弱时，会进入转化/交易诊断，而不是继续只追求曝光。
- 从 0 到 1 的复杂任务会按端到端工作流组合多个内部方法。

# Platform Freshness

小红书的平台规则、账号权限、广告产品、店铺能力、认证条件、私信/留资方式、费用和流量产品可能随时间变化。稳定的方法论可以直接执行；涉及当前平台功能、门槛、费用和限制时，应先核验当前官方规则。历史经验、案例数据和经验阈值不能包装成当前平台算法。

# Compliance

本 Skill 不建议或鼓励刷量、刷粉、伪造互动、虚构身份、内容搬运、规避平台风控或绕过平台规则的引流方式。优先使用真实内容、真实用户反馈、合规商业表达、官方商业工具以及可持续的交易模型。

# Contributing

欢迎通过 Issue 或 Pull Request 改进工作流、判断规则、Prompt、输出模板、数据诊断框架、平台时效性与合规说明。

# Disclaimer

本项目提供内容运营、商业分析和 AI 工作流辅助，不构成收益保证。涉及平台规则、广告、店铺、认证、线索工具和其他平台功能时，请以当前官方规则为准。
