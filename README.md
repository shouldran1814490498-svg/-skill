# 药品社媒外投全流程技能合集

一站式药品社交媒体投放技能包，涵盖策略生成、达人筛选、内容生成&审核、比价核验全链路，支持单独使用或流水线自动编排。

## 技能清单

| 技能 | 触发命令 | 功能 |
|------|----------|------|
| 策略生成 | `/strategy {药品名}` | 输入药品名，输出完整社媒投放策略报告 |
| 达人筛选 | `/kol-screen {参数}` | 根据策略和预算自动筛选达人、生成看板 |
| 内容生成&审核 | `/xhs {达人表} {策略报告}` | 为每位达人生成个性化笔记并合规审核 |
| 比价核验 | `/quote-audit {PO单} {基准库}` | 对比供应商报价与基准价格，输出风险报告 |
| 全流程编排 | `/pipeline full {参数}` | 一键串联以上技能，自动传递数据 |

## 数据流

```
策略生成 ──→ 达人筛选 ──→ 内容生成&审核
                │
                └──→ 比价核验（可选）
```

## 安装方式

### 整体安装（推荐）

```
/plugin marketplace add Alvinxie323716/team-plugins
/plugin install pharma-marketing-skills@team-plugins
```

### 按需安装

```
/plugin install drug-strategy-generator@team-plugins    # 策略生成
/plugin install kol-screening-dashboard@team-plugins    # 达人筛选
/plugin install xhs-content-generator@team-plugins      # 内容生成&审核
/plugin install external-quote-audit@team-plugins       # 比价核验
/plugin install pharma-pipeline@team-plugins            # 仅流水线编排
```

## 更新

安装后开启 auto-update，作者推送更新后自动同步，无需手动操作。

## 目录结构

```
├── .claude-plugin/
│   └── plugin.json
├── 外投策略生成skill/
│   ├── SKILL.md
│   ├── README.md
│   └── scripts/
├── 外投达人筛选skill/
│   └── 医生达人筛选看板_Skill.md
├── 外投小红书内容生成&审核skill/
│   ├── xhs.md
│   └── README.md
├── 外投比价skill/
│   ├── po单检验工具.md
│   └── README.md
├── pipeline/
│   └── pipeline.md
└── README.md
```

## 作者

[@shouldran1814490498-svg](https://github.com/shouldran1814490498-svg)
