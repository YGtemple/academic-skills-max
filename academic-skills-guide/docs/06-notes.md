# 06 · 重要注意事项

> 使用这些技能前必读。包含 IRON RULE、技能边界、混用技巧、常见陷阱。

---

## 一、关于重复技能

你可能注意到技能列表中有三对名称不同但内容完全一致的技能：

| 名称 A | 名称 B | 说明 |
|--------|--------|------|
| `academic-paper` | `paper-writer` | 同一技能的两个名称，内容完全一致 |
| `academic-paper-reviewer` | `paper-reviewer` | 同一技能的两个名称，内容完全一致 |
| `academic-pipeline` | `research-pipeline` | 同一技能的两个名称，内容完全一致 |

**使用建议**：
- 任选其一即可，不需要同时调用
- 本指南统一使用 `academic-paper`、`academic-paper-reviewer`、`academic-pipeline` 这组名称
- 如果你的环境中只有另一组名称，直接对应替换即可

---

## 二、技能边界（不要越界使用）

### 1. doubao-academic-researcher 的硬边界（IRON RULE 6）

researcher **只做文献调研与证据支撑**，以下事情即使你明确要求也不会做：

- ❌ 不产出「摘要+引言+方法+结果+讨论+结论」的可投稿成品论文
- ❌ 不代写论文的任何具体段落
- ❌ 不代写你论文里的「文献综述」那一章成品

**判断标准**：如果你已经在写论文、要的是论文成品部分（含文献综述章节），说明你已进入论文写作阶段，应该用 `doubao-academic-polish`，而不是 researcher。

**researcher 会产出什么**：
- ✅ 结构化调研结果（核心结论/维度分析/争议/方向/参考文献）
- ✅ 一段连续综述正文示例段（面向大方向的格式示例，不是针对你具体题目的成品）
- ✅ 飞书云文档（含文献地图表格、核心逻辑图）

---

### 2. doubao-academic-evaluator 的边界

evaluator **只看不改**：

- ❌ 不替你写正文
- ❌ 不替你画图
- ❌ 不做语言润色

当 evaluator 发现某处需要动手改写时，会自然建议「这块建议重写，可以用 doubao-academic-polish 帮你润色」。

**evaluator 的两类任务**：
1. **想法评估**：还没开始做，判断值不值得投入
2. **投稿前审查**：论文写得差不多了，挑硬伤、判断能不能投

---

### 3. academic-paper-reviewer 的边界

reviewer **只读不写**：

- ❌ 不修改论文（IRON RULE：READ-ONLY CONSTRAINT）
- ❌ 所有评审输出（报告/决策/路线图）都是独立文档
- ❌ 如果 reviewer 试图编辑手稿文件，会被停止并重定向到报告生成

**reviewer 做什么**：
- ✅ 5 人评审面板的评审报告
- ✅ 编辑决策信
- ✅ 修订路线图（告诉你该改什么，但不帮你改）

实际修订要用 `academic-paper`（revision 模式）或 `doubao-academic-polish`。

---

### 4. doubao-paper-close-reading 的边界

close-reading **必须有具体论文**：

- ❌ 不做没有种子论文的开放主题检索（转 researcher）
- ❌ 不做论文代写或语言润色（转 polish）
- ❌ 不做正式同行评审或编辑决策（转 evaluator / reviewer）

---

### 5. academic-pipeline 的边界

pipeline **只编排不做事**：

- ❌ 不直接写论文
- ❌ 不做研究
- ❌ 不做评审

它只检测阶段、推荐模式、调度其他技能、管理转换、跟踪状态。

pipeline 只编排**英文系**技能（deep-research + academic-paper + reviewer）。中文系技能需要手动按路径调用。

---

## 三、IRON RULE（不可覆盖规则）

每个技能都有自己的 IRON RULE，优先级高于你的任何临时指令。以下是最重要的几条：

### deep-research / academic-paper 系列

1. **不虚构引用**：每篇引用必须通过 DOI 或 WebSearch 验证
2. **最多 2 轮修订**：未解决的问题归入「Acknowledged Limitations」
3. **评审人只读**：reviewer 不修改手稿
4. **魔鬼代言人 CRITICAL 不可忽略**：每个 DA CRITICAL 问题必须在编辑决策中可见地裁决
5. **合成器不编造**：编辑综合的每个观点必须追溯到具体的 Phase 1 评审报告
6. **角色分离不等于独立**：5 个评审席位的角色分离不声称是独立错误过程

### doubao-academic-researcher

1. **证据分级不可压成一轴**：始终用「研究设计层级 × 学科内适配度」双轴定级，不接受「把所有非 RCT 一律标为低质量」
2. **编造/不可核验的引用一条都不能进**：灰区 = 不使用；DOI 能解析但标题对不上 = 幻觉信号，必须拦
3. **具体数字/方法细节必须可追溯**：只有全文精读或可靠解析后才能写精确指标
4. **错误前提不作为事实写入**：用户给的前提若与文献/时间线冲突，不顺着写
5. **成稿层不新增判断或引用**：发现证据不足回退 research-synthesis，绝不在成稿层自行补内容
6. **不生成论文式整篇文章/不代写论文段落/不代写文献综述章节**（IRON RULE 6）
7. **质量门禁失败必须回退**：6 维门禁任一不过，按失败路由回退处理

### doubao-academic-evaluator

1. **没有的数字不要编**：对方还没做实验、没给数据，绝不能凭空说出具体数字
2. **判断要配得上证据**：说一个想法很强，得指出强在哪；说一篇稿子有问题，得指出问题在哪一处
3. **乐观要有分寸**：还没验证的想法，语气最多到「值得一试，但要靠实验确认」
4. **结论要和挑出的问题一致**：指出了足以让论文被拒的硬伤，就不能同时说「整体不错可以投」

---

## 四、中英文混用技巧

### 技巧 1：中文调研 + 英文写作

这是最常见的混合模式：
1. 用 `doubao-academic-researcher` 摸清中文方向（含中文文献、政策文件等）
2. 用 `deep-research`（full 模式）补充英文文献
3. 用 `academic-paper`（full 模式）写英文论文

**适用场景**：研究主题涉及中国情境，但要投英文期刊。

---

### 技巧 2：英文写作 + 中文评审

1. 用 `academic-paper` 写英文论文
2. 用 `doubao-academic-evaluator`（中文教授）快速挑硬伤
3. 用 `academic-paper-reviewer`（英文正式评审）做深度评审

**适用场景**：想要中文交互的快速反馈 + 英文正式评审的专业深度。

---

### 技巧 3：中文论文 + 英文文献基础

1. 用 `deep-research`（full 模式）做英文文献调研
2. 用 `doubao-academic-polish`（write-zh 线）写中文论文

**适用场景**：研究领域以英文文献为主，但要写中文学位论文或期刊论文。

---

### 技巧 4：精读 + 调研 + 写作全链路

1. 用 `doubao-paper-close-reading` 精读领域内关键论文
2. 用 `deep-research`（three-way-scan）比较 3 篇核心论文
3. 用 `doubao-academic-researcher` 摸清方向全貌
4. 用 `deep-research`（socratic）引导式找研究问题
5. 用 `doubao-academic-evaluator` 评估想法
6. 用 `academic-paper` 或 `polish` 写论文

**适用场景**：研究生入门、开题前的方向探索。

---

## 五、常见陷阱与避坑指南

### 陷阱 1：用 researcher 写论文

**错误做法**：对 researcher 说「帮我把这些调研结果写成一篇完整论文」

**为什么错**：researcher 的 IRON RULE 6 明确禁止生成成品论文，它会拒绝并引导你转 polish。

**正确做法**：
- 要英文论文 → `academic-paper`（full 模式）
- 要中文论文 → `doubao-academic-polish`（write-zh 线）

---

### 陷阱 2：用 evaluator 改论文

**错误做法**：对 evaluator 说「你觉得这里有问题，那你帮我改一下」

**为什么错**：evaluator 只看不改，它的定位是「诊断」不是「治疗」。

**正确做法**：
- evaluator 指出问题后，用 `academic-paper`（revision 模式）或 `doubao-academic-polish` 实际修改

---

### 陷阱 3：用 reviewer 改论文

**错误做法**：对 reviewer 说「你觉得这段写得不好，那你直接帮我改了吧」

**为什么错**：reviewer 有只读约束（IRON RULE），不修改手稿。

**正确做法**：
- reviewer 给出修订路线图后，用 `academic-paper`（revision 模式）实际修订
- 修订完后用 `reviewer`（re-review 模式）验证

---

### 陷阱 4：跳过调研直接写论文

**错误做法**：只有一个模糊想法，直接说「帮我写一篇关于 X 的论文」

**为什么可能出问题**：没有文献基础，论文的研究空白识别、文献综述部分可能不够扎实，甚至可能重复已有工作。

**正确做法**：
1. 先用 `deep-research`（socratic）厘清研究问题
2. 再用 `deep-research`（full）或 `researcher` 做文献调研
3. 最后用 `academic-paper` 或 `polish` 写论文

**捷径**：如果嫌麻烦，直接用 `academic-pipeline`，它会自动调度调研→写作→评审全流程。

---

### 陷阱 5：写完直接投稿，不做自检

**错误做法**：论文写完直接投稿，不做任何自检和评审

**为什么可能出问题**：可能存在方法漏洞、引用错误、格式问题、论证不充分等硬伤，浪费审稿周期。

**正确做法**（至少做一项）：
- 快速自检：`doubao-academic-evaluator`（投稿前审查）
- 深度评审：`academic-paper-reviewer`（full 模式）
- 引用检查：`academic-paper`（citation-check 模式）

---

### 陷阱 6：收到评审意见后盲目修改

**错误做法**：收到评审意见后，直接说「帮我按照这些意见改论文」，不先理解意见

**为什么可能出问题**：可能误解评审意图，或者修改了不该改的，遗漏了该改的。

**正确做法**：
1. 先用 `academic-paper`（revision-coach 模式）解读评审意见，生成修订路线图
2. 明确哪些要改（will_address）、哪些不改（wont_address）、哪些不相关（not_on_point）
3. 再用 `academic-paper`（revision 模式）实际修订
4. 最后用 `reviewer`（re-review 模式）验证

---

### 陷阱 7：混淆 close-reading 和 reviewer

**区别**：
- `doubao-paper-close-reading`：帮你**理解**一篇论文（研究故事、方法、可信边界），是学习工具
- `academic-paper-reviewer`：帮你**评审**一篇论文（挑错、给决策、给修订路线图），是投稿前检查工具

**选择**：
- 想学习一篇论文的方法和思想 → close-reading
- 想检查自己的论文能不能投 → reviewer / evaluator

---

## 六、性能与成本考虑

### 什么时候用 full 模式，什么时候用 quick？

- **full 模式**：重要论文、投稿前、需要全面评审 → 成本高但质量好
- **quick 模式**：早期草稿、快速了解问题、时间紧张 → 成本低但只覆盖关键问题

**建议流程**：先用 quick 筛一遍大问题，修改后再用 full 做深度评审。

---

### 什么时候用 academic-pipeline？

- ✅ 从 0 到 1 完整发一篇论文，不想手动调度
- ✅ 需要严格的质量保证流程
- ✅ 需要可审计的质量保证产物
- ❌ 只需要某一个环节（如只写摘要、只检查引用）
- ❌ 需要灵活调整流程（pipeline 是固定的 10 阶段）

---

### 中英文系的成本对比

- **英文系**：多 Agent 管线，调用次数多，成本相对高，但产出更专业
- **中文系**：单专家角色 + 子技能，调用次数少，成本相对低，体验更灵活

**建议**：重要的英文期刊论文用英文系，中文论文或早期探索用中文系。

---

## 七、故障排除

### 问题 1：技能说「BLOCKED」或「需要更多信息」

**可能原因**：
- researcher 需要先完成需求清单（requirement_checklist）
- polish 需要确认目标语言
- reviewer 需要确认论文领域

**解决方法**：按照技能的提示补充信息，不要强行跳过。

---

### 问题 2：生成的引用看起来不对

**可能原因**：
- 引用是幻觉（DOI 无法验证）
- 引用格式不符合目标期刊要求

**解决方法**：
- 用 `academic-paper`（citation-check 模式）检查引用
- 对关键引用手动验证 DOI
- 确认目标期刊的引用格式要求

---

### 问题 3：评审意见和我预期的不一样

**可能原因**：
- 评审人配置不符合目标期刊
- 论文领域识别有误

**解决方法**：
- 在 reviewer 的 Phase 0（领域分析与配置）后，检查评审人配置是否符合预期
- 可以手动调整评审人身份和关注点
- 明确说明目标期刊和领域

---

### 问题 4：修订后问题还在

**可能原因**：
- 修订没有真正回应评审意见
- 修订引入了新问题

**解决方法**：
- 用 `reviewer`（re-review 模式）做验证审查
- 检查可追溯性矩阵，确认每条意见都有回应
- 如果 re-review 发现残留问题，继续修订

---

## 八、最佳实践总结

1. **先调研后写作**：不要跳过文献调研直接写论文
2. **先评估后投入**：重要研究方向先做想法评估
3. **先自检后投稿**：投稿前至少做一次自检或评审
4. **先解读后修订**：收到评审意见先解读，再实际修改
5. **改完要验证**：修订后用 re-review 验证
6. **分工要明确**：调研用 researcher，写作用 writer/polish，评审用 reviewer/evaluator，不要越界
7. **不确定用 pipeline**：嫌麻烦就用 academic-pipeline 一键走完全程
8. **中英文可混用**：根据需要灵活组合中英文系技能
