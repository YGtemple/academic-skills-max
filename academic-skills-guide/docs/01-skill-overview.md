# 01 · 技能详细能力边界

> 搞清楚每个技能「做什么、不做什么」，是正确使用的前提。

---

## 1. deep-research（深度研究）

### 做什么

- 把模糊的研究兴趣变成精确的研究问题（FINER 标准）
- 系统性文献检索 + 来源分级验证（掠夺性期刊检测、利益冲突标记）
- 跨来源综合、矛盾解决、主题聚类、研究空白识别
- 生成完整 APA 7.0 研究报告（含摘要、方法、发现、讨论）
- 系统性综述 + 元分析（PRISMA 标准、偏倚风险评估、GRADE 证据分级）
- 事实核查、三篇论文快速比较扫描
- 苏格拉底式研究引导（帮你想清楚研究方向）

### 不做什么

- ❌ 不写「摘要+引言+方法+结果+讨论+结论」格式的可投稿论文（那是 academic-paper 的活）
- ❌ 不做结构化同行评审（那是 reviewer 的活）
- ❌ 不做语言润色

### 8 种模式

| 模式 | 适用场景 |
|------|----------|
| `full` | 有明确 RQ，需要完整研究报告 |
| `socratic` | 有模糊想法，需要引导式思考 |
| `quick` | 需要快速摘要（30 分钟版） |
| `review` | 有一篇论文需要评估后再决定是否引用 |
| `lit-review` | 需要某个主题的文献回顾 |
| `three-way-scan` | 需要快速比较多篇论文 |
| `fact-check` | 需要验证特定事实/声明 |
| `systematic-review` | 需要 PRISMA 标准系统性综述或元分析 |

### 13 个 Agent

| # | Agent | 角色 |
|---|-------|------|
| 1 | research_question_agent | 研究问题精炼（FINER 标准） |
| 2 | research_architect_agent | 方法论蓝图设计 |
| 3 | bibliography_agent | 系统性文献检索 + 标注书目 |
| 4 | source_verification_agent | 来源验证 + 证据分级 |
| 5 | synthesis_agent | 跨来源综合 + 矛盾解决 |
| 6 | report_compiler_agent | APA 7.0 报告编译 |
| 7 | editor_in_chief_agent | Q1 期刊编辑级审查 |
| 8 | devils_advocate_agent | 魔鬼代言人（挑战假设） |
| 9 | ethics_review_agent | 伦理审查 |
| 10 | socratic_mentor_agent | 苏格拉底式导师（引导模式） |
| 11 | risk_of_bias_agent | 偏倚风险评估（RoB 2 / ROBINS-I） |
| 12 | meta_analysis_agent | 元分析设计与执行 |
| 13 | monitoring_agent | 研究后文献监测 |

---

## 2. academic-paper（论文写作）

### 做什么

- 从研究问题到可投稿论文的完整写作
- 6 种论文类型模板（IMRaD、文献综述、案例研究、理论论文、政策简报、会议论文）
- 5 种引用格式（APA 7、Chicago、MLA 9、IEEE、Vancouver）
- 双语摘要（中文繁体 + 英文，独立撰写非机翻）
- 图表生成（Python matplotlib / R ggplot2，APA 格式，色盲友好配色）
- 写作风格校准（提供 3 篇以上旧文，学习你的写作语气）
- 写作质量诊断（模糊用词、打断论证的标点、清嗓子式开头）

### 不做什么

- ❌ 不做深度文献调研（但会做基础文献检索；需要深度调研先用 deep-research）
- ❌ 不做正式多视角同行评审（内部有一轮 5 维自评，但正式评审用 reviewer）
- ❌ 不评估研究想法值不值得做（那是 evaluator 的活）

### 11 种模式

| 模式 | 适用场景 |
|------|----------|
| `full` | 从 0 到 1 写完整论文 |
| `plan` | 引导式规划（一步步指导） |
| `outline-only` | 只要大纲/结构方案 |
| `revision` | 已有草稿，实际修订 |
| `revision-coach` | 收到评审意见，解读并生成修订路线图 |
| `abstract-only` | 只要双语摘要 |
| `lit-review` | 写文献综述类论文 |
| `format-convert` | 格式转换（LaTeX/DOCX/引用格式） |
| `citation-check` | 引用格式检查 |
| `disclosure` | 生成 AI 使用声明（投稿要求） |
| `rebuttal-audit` | 检查回复信是否遗漏评审意见 |

### 12 个 Agent

| # | Agent | 角色 |
|---|-------|------|
| 1 | intake_agent | 配置访谈（论文类型、学科、期刊、引用格式等） |
| 2 | literature_strategist_agent | 文献检索策略 + 来源筛选 |
| 3 | structure_architect_agent | 论文结构设计 + 详细大纲 |
| 4 | argument_builder_agent | 论证构建 + 论点-证据链 |
| 5 | draft_writer_agent | 逐节全文起草 |
| 6 | citation_compliance_agent | 引用格式合规检查 |
| 7 | abstract_bilingual_agent | 双语摘要生成 |
| 8 | peer_reviewer_agent | 内部 5 维自评 + 修订建议 |
| 9 | formatter_agent | 格式转换 + 期刊排版 |
| 10 | socratic_mentor_agent | 计划模式苏格拉底导师 |
| 11 | visualization_agent | 图表生成（Python/R） |
| 12 | revision_coach_agent | 修订教练（评审意见解读） |

---

## 3. academic-paper-reviewer（论文评审）

### 做什么

- 模拟完整国际期刊同行评审流程
- 自动识别论文领域，动态配置 4 位评审人身份 + 1 位固定魔鬼代言人
- 5 个角色分离的评审视角：
  - **期刊适配评审人**：期刊匹配度、原创性、整体质量
  - **方法学评审人**：研究设计、统计有效性、可复现性
  - **领域评审人**：文献覆盖、理论框架、领域贡献
  - **跨学科评审人**：跨学科联系、实践影响、基础假设挑战
  - **魔鬼代言人**：核心论证挑战、逻辑谬误检测、最强反论点
- 编辑综合决策（Accept / Minor Revision / Major Revision / Reject）
- 不可变修订路线图 + 作者裁决记录
- 修订后验证审查（检查修订是否真正回应了评审意见）

### 不做什么

- ❌ 不修改论文（只读约束，所有输出都是独立文档）
- ❌ 不写论文（那是 writer 的活）
- ❌ 不做深度研究

### 6 种模式

| 模式 | 适用场景 |
|------|----------|
| `full` | 完整评审（首次投稿前） |
| `re-review` | 修订后验证审查 |
| `quick` | 快速评估（15 分钟版） |
| `methodology-focus` | 只审查方法/统计 |
| `guided` | 引导式学习评审 |
| `calibration` | 评审人校准（测量评审准确度） |

### 7 个 Agent

| # | Agent | 角色 |
|---|-------|------|
| 1 | field_analyst_agent | 领域分析 + 评审人身份配置 |
| 2 | eic_agent | 期刊适配评审人 |
| 3 | methodology_reviewer_agent | 方法学评审人 |
| 4 | domain_reviewer_agent | 领域评审人 |
| 5 | perspective_reviewer_agent | 跨学科评审人 |
| 6 | devils_advocate_reviewer_agent | 魔鬼代言人 |
| 7 | editorial_synthesizer_agent | 编辑综合决策 |

---

## 4. academic-pipeline（全流程编排器）

### 做什么

- 不做实质性工作，只做**编排**：检测阶段、推荐模式、调度技能、管理转换、跟踪状态
- 10 阶段端到端流水线：
  1. 研究（deep-research）
  2. 写作（academic-paper）
  3. 完整性检查
  4. 评审（academic-paper-reviewer）
  5. 修订（academic-paper）
  6. 复审（academic-paper-reviewer re-review）
  7. 再修订
  8. 最终完整性检查
  9. 定稿
  10. 交付
- 协调 deep-research、academic-paper、academic-paper-reviewer 三者
- 强制性完整性检查（引用验证、数据可追溯性、作者贡献声明等）
- 两阶段同行评审（首轮 + 修订验证）
- 可审计的质量保证产物

### 不做什么

- ❌ 不直接写论文、不做研究、不做评审（都是调度其他技能）
- 只编排英文系技能（deep-research + academic-paper + reviewer）
- 中文系技能需要手动按路径调用

---

## 5. doubao-academic-researcher（中文学术文献调研）

### 做什么

- 面向**尚未锁定具体论文题目**、想先摸清某个大方向的用户
- 系统检索 + 引用真实性核验 + 证据分级（研究设计层级 × 学科适配度双轴）
- 主题聚类 + 交叉综合 + 争议与空白识别
- 产出：核心结论 + 维度分析 + 争议 + 研究方向 + 经核验参考文献 + 一段连续综述正文示例
- 生成飞书云文档（含文献地图表格、核心逻辑图）

### 不做什么（IRON RULE 6，边界很硬）

- ❌ 不产出「摘要+引言+方法+结果+讨论+结论」的可投稿成品论文
- ❌ 不代写论文的任何具体段落
- ❌ 不代写你论文里的「文献综述」那一章成品
- 如果你已经在写论文、要的是论文成品部分 → 转 doubao-academic-polish

### 4 个阶段

1. **literature-scout**：系统检索 + 引用核验
2. **research-synthesis**：主题聚类 + 交叉综合 + 6 维质量门禁
3. **review-writing**：综述正文示例段生成
4. **document-delivery**：飞书文档交付

---

## 6. doubao-academic-polish（论文写作/润色总入口）

### 做什么

三条工作线，先判产物再判语言：

| 工作线 | 处理需求 |
|--------|----------|
| **骨架与润色（shape）** | 搭结构、理主线、给重排方案但不实际移动正文；润色中英文已有文本或中译英 |
| **中文撰写（write-zh）** | 从想法起草中文论文（中文期刊/学位论文等） |
| **英文撰写（write-en）** | 从想法或材料写出可投稿英文正文（SCI/EI/顶会） |

- Makefile 三阶段驱动：`prepare`（读材料、核验来源）→ `write`（按学科结构写）→ `deliver`（生成终稿、创建飞书、读回校验）
- 规划正文时读取结构方法，语言收尾时读取润色方法

### 不做什么

- ❌ 不评估研究想法值不值得做（转 evaluator）
- ❌ 不做独立系统性文献调研（转 researcher）
- ❌ 不做正式同行评审（转 reviewer）

---

## 7. doubao-academic-evaluator（学术评判，只看不改）

### 做什么

两类任务，都是**只诊断不动手**：

1. **评判研究想法**：还没开始做，想知道值不值得投入（打分、查新颖性、判可行性）
2. **投稿前审查**：论文写得差不多了，以审稿人视角挑硬伤，判断能不能投

- 用资深教授的眼光，诚实判断、指出问题、给修改方向

### 不做什么

- ❌ 不替你写正文、不替你画图、不做语言润色（转 polish）
- 发现需要动手改写时，会自然建议「这块建议重写，可以用 polish 帮你润色」

---

## 8. doubao-paper-close-reading（单篇论文精读）

### 做什么

- 不按章节机械复述，而是**重建论文的研究故事**
- 讲清：研究问题 → 现有缺口 → 核心洞察 → 方法/理论 → 关键证据 → 结论 → 可信边界
- 深读决定性实验、图表、关键数字、消融和误差分析
- 主动发现反直觉结果、失效条件、未胜过基线
- 区分四类信息：论文直接报告的事实 / 作者的解释 / 分析推断 / 无法确认
- 判断证据强度、可信边界、复现风险、适用条件
- 生成高级 Markdown 精读报告 + 飞书文档

### 不做什么

- ❌ 不做没有种子论文的开放主题检索（转 researcher）
- ❌ 不做论文代写或语言润色（转 polish）
- ❌ 不做正式同行评审或编辑决策（转 evaluator / reviewer）

---

## 快速对照

| 技能 | 写论文 | 做调研 | 审论文 | 精读论文 | 评估想法 | 全流程编排 |
|------|--------|--------|--------|----------|----------|-----------|
| deep-research | ❌ | ✅ | ❌ | 部分 | ❌ | ❌ |
| academic-paper | ✅ | 基础 | 内部自评 | ❌ | ❌ | ❌ |
| academic-paper-reviewer | ❌ | ❌ | ✅ | ❌ | ❌ | ❌ |
| academic-pipeline | 调度 | 调度 | 调度 | ❌ | ❌ | ✅ |
| doubao-academic-researcher | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| doubao-academic-polish | ✅ | 定向核实 | ❌ | ❌ | ❌ | ❌ |
| doubao-academic-evaluator | ❌ | ❌ | ✅ | ❌ | ✅ | ❌ |
| doubao-paper-close-reading | ❌ | ❌ | ❌ | ✅ | ❌ | ❌ |
