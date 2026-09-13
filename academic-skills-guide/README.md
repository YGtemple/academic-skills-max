# 📚 论文撰写技能体系 · 整合使用指南

> 一套覆盖「从想法萌芽到投稿交付」全链路的 AI 论文工作流指南。帮你在任何一个论文工作阶段，都能准确判断 **先用哪个技能、再用哪个、最后用哪个**。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Docs](https://img.shields.io/badge/docs-complete-brightgreen.svg)](#-文档目录)
[![Skills](https://img.shields.io/badge/skills-8-blue.svg)](#-技能体系总览)

---

## 🎯 这是什么

你是否面对一堆论文相关的 AI 技能，却不知道该从哪个下手？

- 想写论文，是用 `academic-paper` 还是 `doubao-academic-polish`？
- 想做文献调研，是用 `deep-research` 还是 `doubao-academic-researcher`？
- 想审稿，是用 `academic-paper-reviewer` 还是 `doubao-academic-evaluator`？
- 想从头到尾走一遍完整流程，该怎么串联这些技能？

本指南整合了 **8 个论文相关技能**，提供清晰的**决策树**、**典型工作流**和**速查表**，让你不再纠结。

---

## 🚀 快速开始

### 一句话核心逻辑

```
想清楚方向 → 摸清领域 → 评估想法 → 写论文 → 自检/评审 → 修订 → 验证 → 投稿准备
```

### 30 秒决策

| 你现在的状态 | 直接用这个 |
|-------------|-----------|
| 只有模糊想法，不知道研究什么 | `deep-research`（socratic 模式） |
| 有明确问题，要做文献调研 | `deep-research`（full 模式）或 `doubao-academic-researcher` |
| 要写英文论文 / 投国际期刊 | `academic-paper`（full 模式） |
| 要写中文论文 / 学位论文 | `doubao-academic-polish`（write-zh 线） |
| 已有草稿，投稿前挑硬伤 | `doubao-academic-evaluator`（投稿前审查） |
| 模拟正式同行评审 | `academic-paper-reviewer`（full 模式） |
| 收到评审意见，要修改 | `academic-paper`（revision 模式） |
| 从头到尾完整走一遍 | `academic-pipeline`（自动调度全部） |

> 💡 **更详细的决策树见** → [docs/02-decision-tree.md](docs/02-decision-tree.md)

---

## 📋 技能体系总览

### 英文系（Academic Research Suite，重型多 Agent 管线）

| 技能 | 定位 | Agent 数 | 核心产出 |
|------|------|----------|----------|
| **deep-research** | 深度研究与文献调研 | 13 | APA 7.0 研究报告、系统性综述、元分析 |
| **academic-paper** | 论文全文写作 | 12 | 可投稿论文草稿（LaTeX/DOCX/PDF）、双语摘要 |
| **academic-paper-reviewer** | 多视角同行评审模拟 | 7 | 5 人评审报告 + 编辑决策信 + 修订路线图 |
| **academic-pipeline** | 全流程编排器 | 编排层 | 协调上述三者，10 阶段端到端流水线 |

### 中文系（豆包学术系列，轻量专家角色）

| 技能 | 定位 | 核心产出 |
|------|------|----------|
| **doubao-academic-researcher** | 学术文献调研（中文） | 结构化调研结果 + 综述正文示例段 + 飞书文档 |
| **doubao-academic-polish** | 论文写作/结构/润色总入口 | 中文/英文论文正文、结构方案、语言润色 |
| **doubao-academic-evaluator** | 学术评判（只看不改） | 想法可行性评估、投稿前硬伤审查 |
| **doubao-paper-close-reading** | 单篇论文深度精读 | 研究故事重建、方法拆解、可信边界判断 |

> ⚠️ **关于重复技能**：`academic-paper` = `paper-writer`，`academic-paper-reviewer` = `paper-reviewer`，`academic-pipeline` = `research-pipeline`。这三对是同一技能的两个名称，内容完全一致，使用时任选其一即可。

> 📖 **每个技能的详细能力边界** → [docs/01-skill-overview.md](docs/01-skill-overview.md)

---

## 📂 文档目录

| 文档 | 内容 |
|------|------|
| [README.md](README.md) | 本页：概览、快速开始、技能总览 |
| [docs/01-skill-overview.md](docs/01-skill-overview.md) | 8 个技能的详细能力边界（做什么/不做什么/模式列表） |
| [docs/02-decision-tree.md](docs/02-decision-tree.md) | 核心使用流程决策树（20+ 种场景的完整判断路径） |
| [docs/03-workflows.md](docs/03-workflows.md) | 4 条典型工作流路径（从 0 到 1 的完整步骤） |
| [docs/04-comparison.md](docs/04-comparison.md) | 英文系 vs 中文系：9 个维度对比，帮你选对工具 |
| [docs/05-cheatsheet.md](docs/05-cheatsheet.md) | 28 种常见需求速查表（需求 → 技能 → 模式 → 下一步） |
| [docs/06-notes.md](docs/06-notes.md) | 重要注意事项（IRON RULE、技能边界、混用技巧） |

---

## 🔄 典型工作流预览

### 路径 A：从 0 到 1 发一篇英文论文

```
第1步  deep-research (socratic)     → 厘清研究方向
第2步  deep-research (full)          → 系统性文献调研
第3步  doubao-academic-evaluator     → 评估想法可行性（可选）
第4步  academic-paper (full)          → 12 Agent 管线写完整论文
第5步  academic-paper-reviewer (full) → 5 人评审面板模拟同行评审
第6步  academic-paper (revision)      → 根据评审意见修订
第7步  academic-paper-reviewer (re-review) → 验证修订质量
第8步  academic-paper (format-convert + disclosure) → 投稿准备
```

> 📖 **4 条完整工作流详解** → [docs/03-workflows.md](docs/03-workflows.md)

---

## 🛠️ 技能协作关系

```
想法萌芽
   ↓
deep-research (socratic) / doubao-academic-researcher
   ↓
研究问题形成
   ↓
┌─────────────┬─────────────┬─────────────┐
↓             ↓             ↓             ↓
想法评估      文献调研      论文精读
(evaluator)   (deep-research) (close-reading)
└─────────────┴──────┬──────┴─────────────┘
                      ↓
                 论文写作
        academic-paper / doubao-academic-polish
                      ↓
                 草稿完成
                      ↓
        ┌─────────────┼─────────────┐
        ↓             ↓             ↓
   投稿前自检     模拟正式评审    引用/格式检查
   (evaluator)   (reviewer)      (academic-paper)
        └─────────────┼─────────────┘
                      ↓
              收到评审意见
                      ↓
        ┌─────────────┼─────────────┐
        ↓             ↓             ↓
   意见解读       实际修订        写回复信
   (revision-    (revision/      (revision-coach
    coach)        polish)         → rebuttal-audit)
        └─────────────┼─────────────┘
                      ↓
              修订验证 (re-review)
                      ↓
              定稿 + 投稿准备
```

---

## ⚡ 英文系 vs 中文系 怎么选？

| 维度 | 英文系 | 中文系 |
|------|--------|--------|
| 目标论文语言 | 英文为主 | 中文为主 |
| 输出格式 | LaTeX / DOCX / PDF，5 种引用格式 | Markdown + 飞书文档 |
| Agent 数量 | 12-13 个专业 Agent 分工 | 1 个资深专家角色 |
| 适合场景 | 投国际期刊/SCI/顶会 | 中文期刊/学位论文/课程论文 |
| 全流程编排 | ✅ academic-pipeline 自动调度 | ❌ 手动按顺序调用 |

**简单判断**：
- 投英文期刊 / 需要 LaTeX / 要模拟正式同行评审 → **英文系**
- 写中文论文 / 要飞书文档 / 想要导师聊天式体验 → **中文系**
- 两套可以混用！比如用中文 researcher 做调研，用英文 academic-paper 写论文

> 📖 **完整 9 维度对比** → [docs/04-comparison.md](docs/04-comparison.md)

---

## 📌 重要提醒

### 关于技能边界（不要越界使用）
- **researcher 不写论文成品**：只做调研，即使要求"写成完整论文"也不会做
- **evaluator 不动手**：只看不改，需要改写时会建议转 polish
- **reviewer 不修改论文**：只读约束，所有评审输出都是独立文档
- **close-reading 不做开放检索**：必须有具体论文才能用

### 关于 IRON RULE（不可覆盖规则）
每个技能都有自己的 IRON RULE，优先级高于任何临时指令。比如：
- researcher：不编造引用、不生成成品论文、证据分级不可压成一轴
- academic-paper：不虚构引用（必须 DOI 验证）、最多 2 轮修订
- reviewer：不修改论文、魔鬼代言人的 CRITICAL 问题不可忽略

> 📖 **完整注意事项** → [docs/06-notes.md](docs/06-notes.md)

---

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源。

---

## 🙏 致谢

本指南整合的技能包括：
- Academic Research Suite（academic-paper / academic-paper-reviewer / academic-pipeline / deep-research）
- 豆包学术系列（doubao-academic-researcher / doubao-academic-polish / doubao-academic-evaluator / doubao-paper-close-reading）

---

<div align="center">

**觉得有用？给个 ⭐ Star 支持一下！**

</div>
