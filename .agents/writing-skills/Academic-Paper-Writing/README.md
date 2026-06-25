# Academic Paper Writing（学术论文写作基础规范）

## 核心定位

全流程学术写作基础技能。以研究者的身份进行写作，而非通用 AI 助手。复现同行评审学术出版物中的逻辑结构、修辞模式、证据呈现风格和语言惯例。

---

## 三大核心原则

### 1. 逻辑优先，语言其次

学术写作本质上是逻辑论证过程，遵循以下链条：

```
研究动机 → 问题定义 → 知识空白 → 提出方案 → 实验验证 → 解释 → 结论
```

每个段落必须有明确的论证目的。

### 2. 证据驱动写作

每个重要陈述必须由数据、文献、实验观察或逻辑推导支撑。

- ❌ 避免：`Obviously`、`Clearly`、`It is certain that` 等无证据的绝对化表述

### 3. 客观科学语调

保持中立、精确、可复现、可验证。

- ✅ 推荐：`The proposed method demonstrates...`
- ❌ 禁止：`This groundbreaking method...`
- 禁止个人观点、情感化语言、营销话术、宣传性措辞

---

## 段落构建框架

| 模式 | 结构 | 适用场景 |
|------|------|----------|
| 模式 A | 主张 → 证据 → 解释（Claim → Evidence → Interpretation） | 提出论点 |
| 模式 B | 问题 → 空白 → 方案（Problem → Gap → Solution） | 引出方法 |
| 模式 C | 观察 → 解释 → 含义（Observation → Explanation → Implication） | 分析结果 |

---

## 章节级写作指导

涵盖以下章节的结构化写作模板：

- **Abstract**：背景 → 问题 → 方法 → 结果 → 结论（150–300 词）
- **Introduction**：研究背景 → 重要性 → 文献综述 → 知识空白 → 研究目标 → 贡献
- **Related Work**：按主题组织，避免逐篇罗列
- **Methods**：完整可复现性描述（输入、处理、模型架构、优化、损失函数、推理过程）
- **Experimental Section**：实验设置 → 数据集 → 实现细节 → 基线 → 评估指标 → 结果 → 消融 → 讨论
- **Results Analysis**：结果 → 原因 → 科学解释
- **Discussion**：解释原因、优势、局限、应用、未来工作
- **Conclusion**：总结问题、方法、主要发现、含义、未来方向

---

## 期刊风格适配

| 期刊风格 | 特征 |
|----------|------|
| IEEE | 简洁、技术性、直接 |
| Nature | 高层意义、广泛影响、科学含义 |
| Elsevier | 技术深度平衡、强讨论章节、中等句子长度 |
| Medical Image Analysis | 方法学严谨、临床相关性、统计显著性 |

---

## 输出质量等级

| 等级 | 标准 |
|------|------|
| Level 1 | 基础学术风格 |
| Level 2 | SCI 期刊风格 |
| Level 3 | 顶级期刊风格 |
| Level 4 | 审稿就绪级别（默认） |

---

## 表达润色（Polishing Skills）

针对不同语言和格式场景的深度润色能力。

### 英文学术润色（LaTeX）

以 NeurIPS/ICLR/ICML 等顶会标准对英文 LaTeX 片段进行深度润色：

- **严谨性提升**：调整句式结构以适配顶会规范，增强正式性与逻辑连贯性
- **句法打磨**：优化长难句表达，消除非母语写作的生硬感
- **零错误原则**：彻底修正拼写、语法、标点及冠词错误
- **词汇控制**：禁止缩写形式（it's → it is），避免华丽辞藻，优先使用简洁清晰的通用学术词汇
- **所有格规避**：避免名词所有格（METHOD's → the performance of METHOD）
- **格式保持**：保留原文 LaTeX 命令与已有格式，不新增强调标记
- **输出**：Part 1 [LaTeX] + Part 2 [Translation] + Part 3 [Modification Log]

### 中文学术润色（Word）

面向《计算机学报》《软件学报》等核心期刊的中文润色，秉持"尊重原著，克制修改"原则：

- **修正阈值**：仅在口语化、语法错误、逻辑断裂或严重欧化长句时才修改；原文通顺则原样保留
- **语体规范**：坚持当代学术书面语，拒绝陈旧公文腔（如"拟""系"），去除"我们发现"等口语
- **逻辑衔接**：仅在逻辑断裂时显化连接词，优先依靠语序自然衔接
- **Word 适配**：纯文本输出，严禁 Markdown 格式，严格中文全角标点

---

## 去 AI 味检查清单（De-AI-ification Patterns）

系统化识别并消除 AI 生成文本的机械化特征，使论文读起来像人类研究者所写。

### 1. 标点陷阱

| 问题 | 对策 |
|------|------|
| 破折号（—）滥用 | 单段 ≥2 个即标记，优先用分号/逗号/括号/冒号替代 |
| 引号滥用 | 仅用于直接引用或首次提出新术语，禁止用于强调 |

### 2. 机械化连接词与序数词

- ❌ 禁止：Firstly... Secondly... Thirdly... Finally... / First and foremost / It is worth noting that
- ❌ 中文禁止：首先...其次...再次...最后
- ✅ 替代：通过句意本身的因果、递进关系自然过渡
- 过渡词密度控制：单段 ≥3 个 Moreover/Furthermore/However/Therefore 即需修剪

### 3. 高频 AI 词汇（3 级替换表）

| 等级 | 说明 | 示例 |
|------|------|------|
| Tier 1 — 强AI标记 | 尽量避免 | leverage → use; delve into → investigate; showcase → show; underscore → highlight; tapestry → context; pivotal → key; profound → deep; unveil → introduce |
| Tier 2 — 中度标记 | 谨慎使用 | elucidate → explain; ameliorate → improve; disseminate → share; scrutinize → examine |
| Tier 3 — 语境依赖 | 技术准确即可 | integrate, manifest, mediate（在特定技术语境下可保留） |

### 4. 句式结构机械化模式

- **"Not only ... but also ..."**：限制每节 ≤1 次
- **句式模板循环**：禁止 3+ 连续句子以相同方式开头（By... / Through... / Using...）
- **空泛强调词**：删除 "It is crucial/essential/important to..." 的前导句
- **Hedge 堆叠**：单句最多保留 1 个 hedge 词
- **三点式断言**：避免机械的 "faster, more accurate, and more robust" 三连

### 5. 分语言专项

**英文**：避免 -ing 分词连续开头、假学术正式语、名词化堆叠、滥用 "robust"

**中文**：去除"毋庸置疑""众所周知"等空泛辞藻、"首先其次再次"机械列举、长定语堆砌（"一个...的...的...的"）、"被"字句过度使用

### 自查协议（8 条）

1. 破折号计数 → 2. 序数词扫描 → 3. 词汇审计 → 4. 过渡词密度 → 5. 句首多样性 → 6. 空泛强调词 → 7. 引号卫生 → 8. Hedge 堆叠

---

## 相关文件

- 战术指令（AI 智能体调用）：[`skills.md`](./skills.md)
- 返回总览：[`../README.md`](../README.md)
