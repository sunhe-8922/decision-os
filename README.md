# Decision OS

> 高质量决策不是寻找正确答案，而是在约束条件下，构造更好的选项，并用最小代价验证关键假设。

Universal decision-making framework — 7-layer process with plugin routing for investment, real estate, career, and life decisions.

## Architecture

```
Decision OS (Unified Decision Core)
├── Investment Plugin    → ge-weidong-invest
├── Real Estate Plugin   → land-valuator
├── Sector Research       → sector-overview
├── Consulting Plugin     → TBD
├── Business Plugin       → TBD
├── Career Plugin        → TBD
└── Life Plugin          → TBD
```

## 7-Layer Decision Process

```
Step 1: Problem Reframe    → 多数人解决的是假问题
Step 2: Goal + Constraint  → 目标硬排序 + 约束优化
Step 3: Option Generation  → 强制5选项，扩展选项空间
Step 4: Variable + Scenario → 关键变量 + Bull/Base/Bear
Step 5: Red Team Challenge  → 强制反驳，三层攻击
Step 6: Decision Scoring    → 4维加权打分
Step 7: Action + Verify     → 7/30/90天计划 + 止损条件
```

## Key Features

- **Plugin Routing**: Auto-detects decision domain and routes to specialized skills
- **Three Option Strategies**: 要不要型 / 比较型 / 组合配置型
- **Domain Memo Variants**: Investment / Real Estate / Career / Cross-domain templates
- **Scoring Anchors**: Concrete 1-10 rubric for each scoring dimension
- **Red Team Protocol**: Structured adversarial analysis with anti-pattern warnings
- **Cognitive Bias Check**: Anchoring, sunk cost, confirmation bias, framing, loss aversion
- **Decision Speed Guide**: Fast vs slow decision criteria
- **Review → Skill Update Loop**: Decision reviews drive framework evolution
- **Data Integration**: neodata-financial-search + westock-data + WebSearch
- **Source Citation Protocol**: Mandatory hyperlinks, cross-verification, date stamps, output checklist

## Version History

| Version | Date | Change | Trigger |
|---------|------|--------|---------|
| v1.0 | 2026-06-04 | Initial 7-layer framework | User design document |
| v1.1 | 2026-06-04 | Trigger refinement + Plugin injection + Data protocols | Auto-optimization: 63.75%→80% |
| v1.2 | 2026-06-04 | Review trigger rules + Archiving | Auto-optimization: iteration dimension |
| v1.3 | 2026-06-04 | Routing decision tree + Domain Memo variants + Red team anti-patterns + Review→Skill loop | Auto-optimization: 83.75%→90%+ |
| v1.4 | 2026-06-04 | Three option strategies + Scoring anchors + Intent inference + Cross-domain merge + Cognitive bias check + Decision speed guide | Auto-optimization: 73.75%→92.5% |
| v1.5 | 2026-06-04 | Source citation protocol (hyperlinks + cross-verification + output checklist) + Memo template "Data Sources" section | User data provenance standards built-in |

## Usage

This is a [WorkBuddy](https://www.codebuddy.cn) skill. Install by placing the `decision-os/` directory under `~/.workbuddy/skills/`.

Trigger words: 决策、抉择、怎么选、选哪个、decision、该选A还是B

## License

MIT
