# 04 · 英文系 vs 中文系：怎么选？

> 你有两套论文技能，一套英文系（多 Agent 重型管线），一套中文系（专家角色轻量流程）。9 个维度对比，帮你快速选对工具。

---

## 总览对比表

| 维度 | 英文系（Academic Research Suite） | 中文系（豆包学术系列） |
|------|-----------------------------------|------------------------|
| **目标论文语言** | 英文为主（也支持中文） | 中文为主（也支持英文 write-en） |
| **输出格式** | LaTeX / DOCX / PDF / Markdown，5 种引用格式 | Markdown + 飞书文档，引用格式按学科 |
| **Agent 数量** | 12-13 个专业 Agent 分工协作 | 1 个资深专家角色 + 子技能 |
| **适合场景** | 投国际期刊/SCI/顶会、需要严格学术格式 | 中文期刊/学位论文/课程论文、需要飞书协作 |
| **文献调研** | deep-research（APA 7.0 报告，系统性综述/元分析） | doubao-academic-researcher（结构化调研 + 飞书文档） |
| **论文写作** | academic-paper（11 种模式，6 种论文模板） | doubao-academic-polish（3 条工作线，Makefile 驱动） |
| **论文评审** | academic-paper-reviewer（5 人面板 + 编辑决策） | doubao-academic-evaluator（只看不改的教授诊断） |
| **论文精读** | deep-research（review 模式，单篇评估） | doubao-paper-close-reading（重建研究故事） |
| **全流程编排** | ✅ academic-pipeline（10 阶段自动调度） | ❌ 无（手动按顺序调用） |

---

## 逐维度详解

### 1. 目标论文语言

**英文系**：
- 设计初衷就是英文论文写作
- 双语摘要（中文繁体 + 英文）是标准配置
- 学术术语保持英文
- 也能写中文论文，但不是最优

**中文系**：
- write-zh 线专门优化中文论文写作
- 中文文献、法条案例、史料政策、实验数据等来源门控在 prepare 阶段
- write-en 线也能写英文论文
- 用户输入语言不单独决定目标论文语言（用户用中文提问不必然要中文稿）

**选择建议**：
- 明确投英文期刊 / SCI / EI / 顶会 → 英文系
- 明确写中文期刊 / 学位论文 / 课程论文 → 中文系
- 不确定 → 看目标期刊的语言要求

---

### 2. 输出格式

**英文系**：
- LaTeX（.tex + .bib）— 投计算机/物理/数学等领域期刊的标准格式
- DOCX（通过 Pandoc 转换）
- PDF（通过 LaTeX 或 Pandoc）
- Markdown
- 5 种引用格式：APA 7.0、Chicago（Author-Date / Notes-Bibliography）、MLA 9、IEEE、Vancouver
- 支持后期引用格式转换（任何两种格式之间）

**中文系**：
- Markdown 源稿
- 飞书云文档（默认最终交付）
- 引用格式按学科惯例
- 不直接生成 LaTeX

**选择建议**：
- 需要 LaTeX 源文件 / 需要特定引用格式 / 需要 PDF → 英文系
- 需要飞书文档协作 / 只要 Markdown → 中文系

---

### 3. Agent 数量与工作方式

**英文系**：
- deep-research：13 个 Agent
- academic-paper：12 个 Agent
- academic-paper-reviewer：7 个 Agent
- 每个 Agent 有明确的角色定义和职责边界
- 多 Agent 并行/串行协作，有检查点和 IRON RULE
- 有生成器-评估者合同（v3.6.6），论文盲/论文可见分离
- 有冲刺合同（v3.6.2），评审人两阶段分离

**中文系**：
- 1 个资深专家角色（导师/教授/研究者）
- 子技能分工（literature-scout / research-synthesis / review-writing / document-delivery）
- Makefile 三阶段驱动（prepare → write → deliver）
- 更像和一个经验丰富的导师聊天
- 有 OrganizeAgent 做内部调度

**选择建议**：
- 需要多视角、多角色、严格流程的专业产出 → 英文系
- 想要更个性化、更像导师指导的体验 → 中文系

---

### 4. 适合场景

**英文系最佳场景**：
- 投国际顶级期刊（Nature/Science/Cell 子刊等）
- 投 SCI/EI 检索期刊
- 投计算机顶会（NeurIPS/ICML/CVPR/ACL 等）
- 需要严格遵循期刊格式要求
- 需要 LaTeX 源文件
- 需要模拟正式同行评审流程
- 需要系统性综述/元分析（PRISMA 标准）

**中文系最佳场景**：
- 投中文核心期刊（CSSCI/北大核心等）
- 写本科/硕士/博士学位论文
- 写课程论文/学期报告
- 需要飞书文档协作和分享
- 想要中文界面和中文交互体验
- 需要中文文献调研（含中文期刊、政策文件等）

---

### 5. 文献调研对比

| 维度 | deep-research（英文系） | doubao-academic-researcher（中文系） |
|------|------------------------|--------------------------------------|
| 输出格式 | APA 7.0 完整研究报告 | 结构化调研结果 + 飞书文档 |
| 系统性综述 | ✅ PRISMA 标准 + 元分析 | ❌ 不做正式系统性综述 |
| 偏倚风险评估 | ✅ RoB 2 / ROBINS-I | ❌ |
| GRADE 证据分级 | ✅ | ❌ |
| 中文文献支持 | 一般 | ✅ 优化 |
| 文献地图表格 | ❌ | ✅ |
| 核心逻辑图 | ❌ | ✅ |
| 飞书文档交付 | ❌ | ✅ |
| 研究后监测 | ✅ monitoring_agent | ❌ |
| 三篇快速比较 | ✅ three-way-scan | ❌ |
| 事实核查 | ✅ fact-check | ❌ |

**选择建议**：
- 需要正式系统性综述/元分析/PRISMA → deep-research
- 需要中文文献调研 + 飞书文档 + 可视化图表 → researcher
- 可以混用：先用 researcher 摸清中文方向，再用 deep-research 补充英文文献

---

### 6. 论文写作对比

| 维度 | academic-paper（英文系） | doubao-academic-polish（中文系） |
|------|--------------------------|----------------------------------|
| 论文类型模板 | 6 种（IMRaD/综述/案例/理论/政策/会议） | 按学科范式自适应 |
| 引用格式 | 5 种（APA/Chicago/MLA/IEEE/Vancouver） | 按学科惯例 |
| 双语摘要 | ✅ 标准配置 | 可选 |
| 图表生成 | ✅ Python/R 代码 | ❌ |
| 写作风格校准 | ✅ 学习你的写作语气 | ❌ |
| 写作质量诊断 | ✅ | ✅ |
| 内部评审 | ✅ 5 维自评 + 最多 2 轮 | ✅ 正文检查 |
| 飞书文档 | ❌ | ✅ 默认交付 |
| LaTeX 输出 | ✅ | ❌ |
| 11 种模式 | ✅ | 3 条工作线 |
| 修订协议 | ✅ #390 Patch Protocol | ✅ Makefile |

---

### 7. 论文评审对比

| 维度 | academic-paper-reviewer（英文系） | doubao-academic-evaluator（中文系） |
|------|-----------------------------------|------------------------------------|
| 评审人数 | 5 人面板 + 编辑综合 | 1 位资深教授 |
| 角色分离 | ✅ 5 个不同视角 | ❌ 单一视角 |
| 魔鬼代言人 | ✅ 固定席位 | ❌ |
| 编辑决策 | ✅ Accept/Minor/Major/Reject | ✅ 能不能投的判断 |
| 修订路线图 | ✅ 不可变核心 + 作者裁决 | ❌ 只给修改方向 |
| 修订验证 | ✅ re-review 模式 | ❌ |
| 方法学专项 | ✅ methodology-focus | ✅ 分章审阅要点 |
| 快速评估 | ✅ quick（15 分钟） | ✅ |
| 想法评估 | ❌ | ✅ 另一类任务 |
| 只读约束 | ✅ IRON RULE | ✅ 只看不改 |

**选择建议**：
- 想模拟正式期刊同行评审流程，知道不同审稿人会怎么说 → reviewer
- 想让一个资深教授快速帮你挑硬伤、判断能不能投 → evaluator
- 可以串联：先用 evaluator 快速筛一遍，再用 reviewer 做深度评审

---

### 8. 论文精读对比

| 维度 | deep-research review 模式（英文系） | doubao-paper-close-reading（中文系） |
|------|-------------------------------------|--------------------------------------|
| 定位 | 单篇论文评估（决定要不要引用） | 深度精读（重建研究故事） |
| 输出 | 评估报告 | 高级 Markdown + 飞书文档 |
| 研究故事重建 | ❌ | ✅ |
| 方法机制拆解 | 部分 | ✅ |
| 可信边界判断 | ❌ | ✅ |
| 复现风险评估 | ❌ | ✅ |
| 四类信息区分 | ❌ | ✅（事实/解释/推断/无法确认） |
| 飞书文档 | ❌ | ✅ |

**选择建议**：
- 只想快速判断一篇论文值不值得引用 → deep-research review
- 想深入理解一篇论文的方法、证据和局限 → close-reading

---

### 9. 全流程编排

**英文系**：
- ✅ `academic-pipeline` 编排器
- 10 阶段端到端流水线
- 自动调度 deep-research + academic-paper + reviewer
- 强制性完整性检查
- 两阶段同行评审
- 可审计的质量保证产物
- 支持跨会话恢复（Material Passport）

**中文系**：
- ❌ 没有统一编排器
- 需要手动按顺序调用各个技能
- 但 doubao-academic-researcher 内部有 OrganizeAgent 调度 4 个子阶段
- doubao-academic-polish 内部有 Makefile 三阶段

**选择建议**：
- 想一键走完全流程，不想手动调度 → 英文系 + academic-pipeline
- 想自己控制每一步，灵活调整 → 中文系手动串联

---

## 混合使用技巧

### 技巧 1：中文调研 + 英文写作

```
doubao-academic-researcher（摸清中文方向）
    → deep-research full（补充英文文献）
    → academic-paper full（写英文论文）
```

### 技巧 2：英文写作 + 中文评审

```
academic-paper full（写英文论文）
    → doubao-academic-evaluator（中文教授挑硬伤）
    → academic-paper-reviewer full（英文正式评审）
```

### 技巧 3：中文论文 + 英文文献基础

```
deep-research full（英文文献调研）
    → doubao-academic-polish write-zh（写中文论文）
```

### 技巧 4：精读 + 调研 + 写作全链路

```
doubao-paper-close-reading（精读关键论文）
    → deep-research three-way-scan（比较核心论文）
    → doubao-academic-researcher（摸清方向全貌）
    → academic-paper full（写论文）
```

---

## 最终选择决策

```
你要写什么语言的论文？
│
├─ 英文
│   ├─ 需要 LaTeX / 严格期刊格式？
│   │   └─ 是 → 英文系（academic-paper）
│   │   └─ 否 → 都可以，英文系更专业
│   └─ 需要模拟正式同行评审？
│       └─ 是 → 英文系（reviewer）
│
├─ 中文
│   ├─ 需要飞书文档协作？
│   │   └─ 是 → 中文系（polish write-zh）
│   │   └─ 否 → 都可以
│   └─ 主要参考中文文献？
│       └─ 是 → 中文系（researcher + polish）
│
└─ 不确定
    └─ 先用中文系轻量探索，需要时再切入英文系重型管线
```
