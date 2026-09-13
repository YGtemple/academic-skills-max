# 02 · 核心使用流程决策树

> 这是本指南最重要的部分。从「你想做什么？」出发，覆盖 20+ 种场景，每种都明确给出「先用哪个、再用哪个」。

---

## 主决策树

```
你想做什么？
│
├─ 我只有一个模糊的想法，还不知道研究什么
│   └─ 先用：deep-research（socratic 模式）
│      或 doubao-academic-researcher
│      （帮你厘清方向、形成研究问题）
│
├─ 我有明确的研究问题，但还没做文献调研
│   └─ 先用：deep-research（full 或 systematic-review 模式）
│      或 doubao-academic-researcher（中文方向）
│      → 产出：研究报告 / 调研结果 + 文献基础
│      → 然后用：academic-paper 或 doubao-academic-polish 写论文
│
├─ 我想评估这个研究想法值不值得做
│   └─ 用：doubao-academic-evaluator（想法评估模式）
│      → 产出：可行性判断、新颖性检查、打分
│      → 如果值得做 → 进入文献调研 → 写作
│
├─ 我有文献基础，要开始写论文了
│   ├─ 要英文论文 / 投国际期刊 / 需要 LaTeX 输出
│   │   └─ 用：academic-paper（full 模式）
│   │      （12 Agent 管线，8 阶段，输出 LaTeX/DOCX/PDF）
│   │
│   ├─ 要中文论文 / 学位论文 / 中文期刊
│   │   └─ 用：doubao-academic-polish（write-zh 线）
│   │
│   ├─ 只要大纲 / 结构方案
│   │   └─ 用：academic-paper（outline-only 模式）
│   │      或 doubao-academic-polish（shape 结构模式）
│   │
│   └─ 要从头到尾完整走一遍（研究→写作→评审→修订）
│       └─ 用：academic-pipeline（编排器，自动调度全部技能）
│
├─ 我已经有论文草稿了
│   ├─ 想投稿前先自己审一遍，挑硬伤
│   │   └─ 用：doubao-academic-evaluator（投稿前审查模式）
│   │      （只看不改，给判断和方向）
│   │
│   ├─ 想模拟正式同行评审，知道审稿人会怎么说
│   │   └─ 用：academic-paper-reviewer（full 模式）
│   │      （5 人评审面板 + 编辑决策 + 修订路线图）
│   │
│   ├─ 只想快速看看有没有明显问题
│   │   └─ 用：academic-paper-reviewer（quick 模式，15 分钟版）
│   │
│   └─ 只想检查方法/统计有没有问题
│       └─ 用：academic-paper-reviewer（methodology-focus 模式）
│
├─ 我收到了评审意见，要修改论文
│   ├─ 想先搞懂评审意见在说什么、怎么改
│   │   └─ 用：academic-paper（revision-coach 模式）
│   │      （把非结构化评审意见变成修订路线图）
│   │
│   ├─ 要实际动手修改论文
│   │   └─ 用：academic-paper（revision 模式）
│   │      或 doubao-academic-polish（实质性修订走 write 线）
│   │
│   └─ 改完了，想验证修订是否真正回应了评审意见
│       └─ 用：academic-paper-reviewer（re-review 模式）
│
├─ 我要写回复信（Response to Reviewers）
│   ├─ 还没写，想生成回复框架
│   │   └─ 用：academic-paper（revision-coach 模式）
│   │
│   └─ 已经写了回复信，想检查有没有遗漏评审意见
│       └─ 用：academic-paper（rebuttal-audit 模式）
│       （逐条覆盖检查 + 缺口 + 风险标记，不生成新回复）
│
├─ 我想深入理解某一篇具体论文
│   └─ 用：doubao-paper-close-reading
│      （重建研究故事、方法拆解、可信边界、复现风险）
│
├─ 我想快速比较几篇论文
│   └─ 用：deep-research（three-way-scan 模式，三篇快速比较）
│
├─ 我要检查引用格式对不对
│   └─ 用：academic-paper（citation-check 模式）
│
├─ 我要转换论文格式（LaTeX/DOCX/引用格式）
│   └─ 用：academic-paper（format-convert 模式）
│
├─ 我要写 AI 使用声明（投稿要求）
│   └─ 用：academic-paper（disclosure 模式）
│
└─ 我只要摘要
    └─ 用：academic-paper（abstract-only 模式，双语摘要）
```

---

## 按论文工作阶段细分

### 阶段 1：选题与方向探索

| 你的状态 | 首选技能 | 模式 | 产出 | 接着用 |
|----------|----------|------|------|--------|
| 完全不知道研究什么 | deep-research | socratic | 研究问题 + 方向建议 | researcher 做调研 |
| 有大致方向但不精确 | deep-research | socratic | 精炼后的研究问题 | full 模式深入 |
| 想知道某个方向有没有人做 | doubao-academic-evaluator | 想法评估 | 新颖性检查 + 可行性打分 | researcher 做调研 |
| 想摸清某个领域全貌 | doubao-academic-researcher | — | 结构化调研结果 + 文献地图 | polish 写论文 |

### 阶段 2：文献调研

| 你的需求 | 首选技能 | 模式 | 产出 |
|----------|----------|------|------|
| 系统性文献调研（英文） | deep-research | full | APA 7.0 研究报告 |
| 系统性文献调研（中文） | doubao-academic-researcher | — | 调研结果 + 飞书文档 |
| PRISMA 标准系统性综述 | deep-research | systematic-review | 综述 + 元分析（可选） |
| 只要文献回顾部分 | deep-research | lit-review | 标注书目 + 综合 |
| 快速比较 3 篇论文 | deep-research | three-way-scan | 比较矩阵 |
| 验证某个事实/声明 | deep-research | fact-check | 事实核查报告 |
| 评估某篇论文值不值得引用 | deep-research | review | 单篇评估报告 |

### 阶段 3：论文写作

| 你的需求 | 首选技能 | 模式/线 | 产出 |
|----------|----------|---------|------|
| 英文论文从 0 到 1 | academic-paper | full | 完整论文 + 双语摘要 |
| 中文论文从 0 到 1 | doubao-academic-polish | write-zh | 中文论文 + 飞书文档 |
| 英文论文从材料到成稿 | doubao-academic-polish | write-en | 英文论文 + 飞书文档 |
| 引导式一步步写 | academic-paper | plan | 章节计划 + 指导 |
| 只要大纲 | academic-paper | outline-only | 详细大纲 + 证据地图 |
| 只要结构方案 | doubao-academic-polish | shape 结构 | 重排方案（不改正文） |
| 只要双语摘要 | academic-paper | abstract-only | 中英文摘要 + 关键词 |
| 写文献综述类论文 | academic-paper | lit-review | 综述论文 |
| 自动走完全流程 | academic-pipeline | — | 端到端流水线 |

### 阶段 4：自检与评审

| 你的需求 | 首选技能 | 模式 | 产出 |
|----------|----------|------|------|
| 投稿前快速挑硬伤 | doubao-academic-evaluator | 投稿前审查 | 问题清单 + 能不能投的判断 |
| 模拟正式同行评审 | academic-paper-reviewer | full | 5 人评审 + 编辑决策 + 修订路线图 |
| 快速评估（15 分钟） | academic-paper-reviewer | quick | 期刊适配评审人快速意见 |
| 只审方法/统计 | academic-paper-reviewer | methodology-focus | 方法学深度审查 |
| 引导式学习评审 | academic-paper-reviewer | guided | 苏格拉底式问题引导 |
| 深度精读一篇论文 | doubao-paper-close-reading | — | 研究故事 + 可信边界 |

### 阶段 5：修订与回复

| 你的需求 | 首选技能 | 模式 | 产出 |
|----------|----------|------|------|
| 解读评审意见 | academic-paper | revision-coach | 修订路线图 |
| 实际修订论文 | academic-paper | revision | 修订后的论文 |
| 中文论文修订 | doubao-academic-polish | write 线 | 修订后的中文论文 |
| 只做语言润色 | doubao-academic-polish | shape 润色 | 润色后的文本 |
| 验证修订质量 | academic-paper-reviewer | re-review | 验证报告 + 新决策 |
| 生成回复信框架 | academic-paper | revision-coach | 回复信骨架 |
| 检查回复信完整性 | academic-paper | rebuttal-audit | 覆盖检查 + 缺口 |

### 阶段 6：投稿准备

| 你的需求 | 首选技能 | 模式 | 产出 |
|----------|----------|------|------|
| 检查引用格式 | academic-paper | citation-check | 引用错误报告 |
| 转换为 LaTeX | academic-paper | format-convert | .tex + .bib 文件 |
| 转换为 DOCX | academic-paper | format-convert | Word 文档 |
| 转换引用格式 | academic-paper | format-convert | 新格式引用 |
| 生成 AI 使用声明 | academic-paper | disclosure | 期刊适配的声明 |

---

## 常见组合路径

### 组合 1：英文系全链路（推荐投国际期刊）

```
deep-research (socratic)
    → deep-research (full)
    → academic-paper (full)
    → academic-paper-reviewer (full)
    → academic-paper (revision)
    → academic-paper-reviewer (re-review)
    → academic-paper (format-convert + disclosure)
```

### 组合 2：中文系全链路（推荐中文期刊/学位论文）

```
doubao-academic-researcher
    → doubao-academic-evaluator（想法评估，可选）
    → doubao-academic-polish (write-zh)
    → doubao-academic-evaluator（投稿前审查）
    → doubao-academic-polish (shape 润色)
```

### 组合 3：混合链路（中文调研 + 英文写作）

```
doubao-academic-researcher（中文调研，摸清方向）
    → deep-research (full)（英文文献补充）
    → academic-paper (full)（英文论文写作）
    → academic-paper-reviewer (full)（评审）
    → academic-paper (revision)（修订）
```

### 组合 4：学生读论文 + 找方向

```
doubao-paper-close-reading（精读关键论文）
    → deep-research (three-way-scan)（比较 3 篇核心论文）
    → doubao-academic-researcher（摸清方向全貌）
    → deep-research (socratic)（引导式找研究问题）
    → doubao-academic-evaluator（评估想法）
```

---

## 决策原则

1. **先判断阶段，再选择技能** — 你在选题、调研、写作、评审、修订还是投稿准备？
2. **先判断语言，再选择系列** — 英文论文优先英文系，中文论文优先中文系
3. **不确定时从轻量开始** — 先用 quick/socratic 模式探索，再进入 full 模式
4. **评估和写作分开** — evaluator 只看不改，polish/writer 只写不评，不要混着用
5. **调研和写作分开** — researcher 只做调研不写成品，writer 写论文但不做深度调研
6. **嫌麻烦就用 pipeline** — academic-pipeline 自动调度英文系全流程
