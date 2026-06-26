# 写作经验日志（Writing Experience Log）

> 本文件记录学术写作智能体在使用过程中积累的纠错经验、发现的规律、Skill 边界决策和用户反馈。
> 每条经验按日期倒序排列。被验证 ≥3 次的重要经验将回写到 `AGENT.md`。

---

## 经验索引

| 日期 | 类型 | 标题 | 关联 Skill |
|------|------|------|-----------|
| 2026-06-26 | 边界决策 | 去 AI 味唯一归属明确 | Academic-Paper-Writing |
| 2026-06-26 | 错误 | Author-Style-Fingerprint skills.md 被意外覆盖 | Author-Style-Fingerprint |
| 2026-06-26 | 规律 | skills.md 与 README.md 同步规则 | 全部 |
| 2026-06-26 | 边界决策 | Top-Journal AI Writing Suppression 误放入 | Top-Journal-Writing |
| 2026-06-26 | 规律 | 3 个 Skill 的期刊画像互补不重复 | 全部 |
| 2026-06-26 | 错误 | 输出完整性：修改前必须记录完整原始文本 | Academic-Paper-Writing |

---

## 详细记录

### [2026-06-26] 去 AI 味唯一归属明确

**类型**：边界决策

**触发场景**：从 `awesome-ai-research-writing` 分发去 AI 味相关提示词时，同时放入了 3 个 Skill。

**问题描述**：
- `Academic-Paper-Writing` 有完整的 De-AI-ification Patterns
- `Author-Style-Fingerprint-Engine` 有 De-AI-ification: English/Chinese + Vocabulary Watchlist
- `Top-Journal-Writing-Engine` 有 AI Writing Suppression Layer
- 三处内容高度重叠，维护成本高，调用时容易混淆

**根因分析**：分发时未先定义职责边界。去 AI 味是横切关注点，应该集中管理。

**解决方法**：
1. 确定 `Academic-Paper-Writing` 为去 AI 味唯一负责方
2. 从 `Author-Style-Fingerprint-Engine` 删除所有去 AI 味内容（skills.md + README.md）
3. 从 `Top-Journal-Writing-Engine` 删除 AI Writing Suppression Layer，替换为交叉引用

**预防措施**：
- 任何涉及「去 AI 味」「表达润色」「文本改写」的需求，一律归入 `Academic-Paper-Writing`
- 其他 Skill 如需使用去 AI 味能力，通过交叉引用而非内嵌实现

---

### [2026-06-26] Author-Style-Fingerprint skills.md 被意外覆盖

**类型**：错误

**触发场景**：使用 `create_file` 工具写入 Author-Style-Fingerprint-Engine/skills.md 后，文件内容被后续操作意外替换为 Academic-Paper-Writing 的内容。

**问题描述**：
- `Author-Style-Fingerprint-Engine/skills.md` 原本已写入正确的去 AI 味内容
- 后续某次操作后，文件内容变成了 `Academic Paper Writing Skill` 的完整内容
- 直到审计 README 时才被发现

**根因分析**：文件操作工具链中可能存在覆盖行为。可能原因：`create_file` 被重复调用、或 `replace_string_in_file` 的 oldString 匹配到了意外的范围。

**解决方法**：使用终端 `cat > file << 'ENDOFFILE'` 重写整个文件。

**预防措施**：
- 重要文件修改后立即用 `grep_search` 检查一级标题确认内容正确
- 使用 `create_file` 工具前确认文件不存在；如存在则用 `replace_string_in_file`
- 对于需要全量替换的文件，优先使用终端 heredoc 方式

---

### [2026-06-26] skills.md 与 README.md 同步规则

**类型**：规律

**触发场景**：多次更新 skills.md 后，用户提醒同步 README.md。

**问题描述**：
- 修改了 4 个 Skill 的 skills.md，但只更新了 `Academic-Paper-Writing` 的 README.md
- 最终需要补更新其余 3 个 README.md
- 同理，根目录 `writing-skills/README.md` 也需要同步

**根因分析**：缺少强制同步检查机制。修改 skills.md 和更新 README.md 是两个独立操作，容易遗漏。

**解决方法**：
1. 在 `AGENT.md` 自审清单中加入「文件同步」检查项（D 类）
2. 明确同步链路：`skills.md → Skill README.md → writing-skills/README.md`
3. 每次修改 skills.md 后，同一轮对话中必须完成 README.md 更新

**预防措施**：
- 使用 `multi_replace_string_in_file` 时，同时包含 skills.md 和 README.md 的修改
- 自审 Phase 3 中优先检查 D 类项目

---

### [2026-06-26] Top-Journal AI Writing Suppression 误放入

**类型**：边界决策

**触发场景**：全面审计 Skill 职责时发现。

**问题描述**：`Top-Journal-Writing-Engine/skills.md` 中存在 `# AI Writing Suppression Layer` 章节，内容为去 AI 模式清单（Furthermore/Moreover/Additionally 重复、三段同构、无证据声明等），与 `Academic-Paper-Writing` 的 De-AI-ification Patterns 重叠。

**根因分析**：该 Skill 的 skills.md 在被外部填充时混入了不属于其职责的内容。`Top-Journal-Writing` 的核心是「可发表性最大化」，而非「去 AI 模式」。

**解决方法**：将 AI Writing Suppression Layer 替换为交叉引用，指向 `Academic-Paper-Writing` 的 De-AI-ification Patterns。同步更新 README.md 和总览 README.md。

**预防措施**：审计清单 C 类「Skill 职责边界」中明确定义：去 AI 味仅由 `Academic-Paper-Writing` 负责。

---

### [2026-06-26] 3 个 Skill 的期刊画像互补不重复

**类型**：规律

**触发场景**：审计时发现 `Author-Style-Fingerprint`、`Paper-Reverse-Engineering`、`Top-Journal-Writing` 三个 Skill 都有期刊/会议风格相关内容。

**问题描述**：担心三处期刊画像重复。

**根因分析**：仔细对比后发现三者视角不同：
- `Author-Style-Fingerprint`：风格向量（用于 Style Transfer 时的目标参照）
- `Paper-Reverse-Engineering`：逆向目标（提取参考论文所属期刊的风格特征）
- `Top-Journal-Writing`：写作策略（针对不同期刊调整写作方式和重点）

**解决方法**：确认不重复，保留三处。在 `AGENT.md` 中记录此决策。

**预防措施**：遇到疑似重复时，先对比「使用场景」而非「内容关键词」来判断是否真正重复。

---

### [2026-06-26] 输出完整性：修改前必须记录完整原始文本

**类型**：错误

**触发场景**：生成论文优化报告时，在「修改前」区块使用 `...` 截断原文，导致作者无法对照查看完整变更。

**问题描述**：Introduction 仅贴了前 2 段、Discussion 部分段落用 `...` 省略、Audio Data Collection 用 `...` 省略细节——作者无法判断完整变更范围。

**根因分析**：为节省报告篇幅而截断原文，但违反了「透明可对照」的输出原则。

**解决方法**：每个「修改前」区块必须包含被修改段落的完整原始文本，逐段对应，禁止任何省略标记。

**预防措施**：生成报告后逐项自查，确认所有「修改前」区块无 `...` 截断。

**关联 Skill**：Academic-Paper-Writing

---

## 待验证的经验

> 以下经验尚未达到回写阈值（<3 次验证），暂存于此。

- （暂无）

---

## 回写记录

> 记录哪些经验已被回写到 AGENT.md。

| 日期 | 经验标题 | 回写至 AGENT.md 章节 |
|------|---------|---------------------|
| 2026-06-26 | Skill 职责边界：去 AI 味唯一归属 | 经验积累 |
| 2026-06-26 | skills.md 与 README.md 必须同步 | 经验积累 |
| 2026-06-26 | 输出完整性：修改前必须记录完整原始文本 | 经验积累 |
