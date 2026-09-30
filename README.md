# academic-skills-max · 论文撰写技能体系整合使用指南

> 一句话简介：整合 8 个 AI 学术技能的"选型与串联"决策指南——从想法萌芽到投稿交付全链路，给决策树、典型工作流与速查表。

## 一、项目概述与定位

这不是某个单独的学术技能，而是一套**"技能体系的使用说明书"**：把 8 个论文相关 AI 技能整合起来，回答"面对一堆论文技能，到底先用哪个、再用哪个、最后用哪个"的问题。核心逻辑是一句话：

```
想清楚方向 → 摸清领域 → 评估想法 → 写论文 → 自检/评审 → 修订 → 验证 → 投稿准备
```

它面向两类工具生态：
- **英文系（Academic Research Suite，重型多 Agent 管线）**：`deep-research`（13 Agent，深度研究/文献调研）、`academic-paper`（12 Agent，论文全文写作，输出 LaTeX/DOCX/PDF）、`academic-paper-reviewer`（7 Agent，多视角同行评审模拟）、`academic-pipeline`（编排层，10 阶段端到端流水线）。
- **中文系（豆包学术系列，轻量专家角色）**：`doubao-academic-researcher`（中文文献调研，出飞书文档）、`doubao-academic-polish`（论文写作/结构/润色总入口）、`doubao-academic-evaluator`（学术评判，只看不改）、`doubao-paper-close-reading`（单篇论文深度精读）。

并说明三对**同物异名**：`academic-paper = paper-writer`、`academic-paper-reviewer = paper-reviewer`、`academic-pipeline = research-pipeline`，内容一致任选其一。

## 二、核心内容（决策树与工作流）

### 30 秒决策速查
| 当前状态 | 直接用这个 |
|---|---|
| 只有模糊想法 | `deep-research`（socratic 模式） |
| 有明确问题要做文献调研 | `deep-research`（full）或 `doubao-academic-researcher` |
| 写英文论文/投国际期刊 | `academic-paper`（full） |
| 写中文论文/学位论文 | `doubao-academic-polish`（write-zh） |
| 投稿前挑硬伤 | `doubao-academic-evaluator` |
| 模拟正式同行评审 | `academic-paper-reviewer`（full） |
| 收到评审意见要修改 | `academic-paper`（revision） |
| 从头到尾走一遍 | `academic-pipeline`（自动调度） |

### 典型工作流（路径 A：从 0 到 1 发英文论文）
deep-research(socratic) 厘清方向 → deep-research(full) 系统调研 → evaluator 评估想法 → academic-paper(full) 写全文 → reviewer(full) 模拟评审 → academic-paper(revision) 修订 → reviewer(re-review) 验证 → academic-paper(format-convert + disclosure) 投稿准备。

### 英文系 vs 中文系选择
投英文期刊/要 LaTeX/要模拟正式同行评审 → 英文系；写中文论文/要飞书文档/要导师聊天式体验 → 中文系；两套可混用（如中文 researcher 调研 + 英文 academic-paper 写作）。

## 三、目录结构

```
academic-skills-max/
├── README.md                          # 根目录概览（与下方 README 同源，约 9.3KB）
└── academic-skills-guide/
    ├── LICENSE                        # MIT
    ├── README.md                     # 整合指南主文档（概览/快速开始/技能总览/协作关系/边界）
    └── docs/
        ├── 01-skill-overview.md       # 8 个技能详细能力边界（做什么/不做什么/模式列表，11.6KB）
        ├── 02-decision-tree.md        # 核心使用决策树（20+ 场景完整判断路径，10.5KB）
        ├── 03-workflows.md            # 4 条典型工作流（从 0 到 1 完整步骤，10KB）
        ├── 04-comparison.md           # 英文系 vs 中文系 9 维度对比（10.4KB）
        ├── 05-cheatsheet.md           # 28 种常见需求速查表（需求→技能→模式→下一步，9.5KB）
        └── 06-notes.md                 # 重要注意事项（IRON RULE/技能边界/混用技巧，13.4KB）
```

## 四、关键内容解读

- **`02-decision-tree.md`**：20+ 种场景的完整判断路径，是"不知道用哪个"时的第一入口。
- **`05-cheatsheet.md`**：28 种常见需求的速查表（需求→技能→模式→下一步），最实用的一页纸。
- **`06-notes.md`**：强调**技能边界不可越界**——researcher 不写论文成品、evaluator 只看不改、reviewer 不修改论文、close-reading 必须有具体论文；以及每个技能自己的 **IRON RULE**（如 researcher 不编造引用、academic-paper 不虚构引用须 DOI 验证且最多 2 轮修订、reviewer 的 CRITICAL 问题不可忽略），优先级高于临时指令。
- **技能协作关系图**：从"想法萌芽"出发，经调研/评估/精读分流，到写作、自检/评审、意见解读/修订/回复信、re-review 验证、定稿投稿的完整链路。

## 五、运行与使用

纯 Markdown 文档库，无需运行。阅读路径：先看根 README 的 30 秒决策表 → 不确定时查 `docs/02-decision-tree.md` → 按 `docs/03-workflows.md` 串联 → 速查用 `docs/05-cheatsheet.md` → 避坑看 `docs/06-notes.md`。

## 六、数据/资源构成

全部为**文本文件**（Markdown + License），无图片、音视频、字体、压缩包等二进制文件。共约 10 个文本文件。

## 七、项目特点

1. **"元技能"定位**：本身不产出论文，而是教人如何正确编排其他学术技能，降低工具选择与串联成本。
2. **双语生态对照**：把重型多 Agent 英文管线与轻量中文专家角色放在同一张地图上对比，并允许混用。
3. **强调纪律**：反复强调各技能的能力边界与 IRON RULE，防止越界使用（如让只做调研的技能去写成品）。
4. **决策导向**：以决策树/速查表/工作流为组织方式，而非按技能平铺罗列。
