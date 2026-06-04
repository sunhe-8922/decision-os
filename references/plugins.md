# Decision OS — 通用决策系统插件映射

本文件定义 Decision OS 如何路由到各领域 Plugin skill。

## Plugin 注册表

| Plugin | Skill 名称 | 触发条件 | 状态 |
|--------|-----------|---------|------|
| Investment | `ge-weidong-invest` | 投资决策、股票买卖、仓位管理、硬科技赛道 | ✅ 已有 |
| Real Estate | `land-valuator` | 土地估价、宗地评估、地价测算、抵押评估 | ✅ 已有 |
| Sector Research | `sector-overview` | 行业研究、竞争格局、行业全景、赛道分析 | ✅ 已有 |
| Consulting | 待建 | 咨询项目、客户方案、战略建议 | 🔲 待建 |
| Business | 待建 | 创业、商业模式、公司运营 | 🔲 待建 |
| Career | 待建 | 跳槽、职业规划、城市选择 | 🔲 待建 |
| Life | 待建 | 买房自住、婚姻、教育、移民 | 🔲 待建 |

## 路由规则

1. **精确匹配优先**：如果用户问题明确属于某个 Plugin 的触发条件，直接路由到该 skill
2. **多 Plugin 情况**：如果问题跨领域（如"在珠海买房投资"同时涉及 Real Estate + Investment），主 skill 负责，辅 skill 提供数据支持
3. **无匹配 Plugin**：使用 Decision OS 通用 7 层流程处理
4. **Plugin 内部仍遵循 Decision OS 内核**：目标→约束→选项→概率→赔率→风险→行动

## 每个 Plugin 必须实现的接口

所有 Plugin skill 在其 SKILL.md 中必须包含以下结构，以确保与 Decision OS 对齐：

```markdown
## Decision OS 接口

### 问题重构模板
原问题：___
真正问题：___
决策时限：___
成功标准：___

### 目标排序
1. [必须满足] ___
2. [最好满足] ___
3. [可放弃] ___

### 约束清单
资金：___ | 时间：___ | 能力：___ | 法律：___ | 心理：___

### 选项空间（至少5个）
Option A：___
Option B：___
Option C：___
Option D：___
Option E：___

### Decision Memo 输出
问题：___
目标：___
约束：___
选项：___
关键变量：___
情景推演：___
红队观点：___
最终决策：___
置信度：___ / 10
执行计划：___
观察指标：___
```
