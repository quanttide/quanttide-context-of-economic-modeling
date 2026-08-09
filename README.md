# 量潮经济建模工作语境

## 领域定位

量潮经济云（qtcloud-econ）以**博弈论**为基础建立对经济体系的认知：通过**机制设计**（Mechanism Design）设计博弈规则，让参与者的自利行为导向期望结果。

核心概念：
- **机制（Mechanism）**：参与者 / 策略空间 / 规则（结果函数）/ 设计目标 四要素
- **博弈（Game）**：机制中的实际互动过程
- **经济建模**：从真实博弈（如招聘博弈）提炼可复用的机制结构

## 数据工程流程

经济云的数据处理遵循量潮数据工程标准：**需求澄清 → 规格设计 → 实现 → 交付**。

| 阶段 | 输入 | 输出 |
| --- | --- | --- |
| **clarify（澄清）** | 模糊的问题描述（Markdown） | 结构化需求（问题/参与者/目标/约束） |
| **design（设计）** | 结构化需求 | 机制设计规格（players/strategies/rules/objectives） |
| 实现 | 机制规格 | 可运行的机制模型/数据 |
| 交付 | 机制模型 | 展示/消费（Studio/Provider/CLI） |

## 种子数据

各端独立维护机制种子数据（`mechanisms.json`）：

| 端 | 路径 |
| --- | --- |
| CLI | `src/cli/data/mechanisms.json` |
| Provider | `src/provider/data/mechanisms.json` |
| Studio | `src/studio/assets/data/mechanisms.json` |

## 参考案例：招聘博弈机制

从 2026-08-09 日志提炼的第一个机制：候选人池 / 自找题市场化微型创业 / AI 三层筛选 / 白嫖者转化实训基地——验证"招聘从成本项变收益项"。

## 文档导航

| 文档 | 内容 |
| --- | --- |
| `default/deliverables.md` | 经济建模交付物边界（实体/分析/生态/知识四层） |
| `default/clarify-models.md` | 需求澄清思维模式 |
| `default/design-models.md` | 机制设计思维模式 |
| `mechanism/recuirtment-mechanism.md` | 招聘博弈机制深度分析 |
| `decision/platform-investment.md` | 平台投资决策 |
