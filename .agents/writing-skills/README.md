# 学术写作智能体技能集（Writing Skills）

本目录包含 5 个学术写作辅助技能（Skill），每个技能针对学术论文写作的不同阶段和维度提供专业化指导。所有技能均以英文编写战术指令（skills.md），中文编写人类可读说明（README.md）。

---

## 技能总览

| # | 技能名称 | 章节数 | 核心定位 | 适用阶段 |
|---|---------|--------|---------|---------|
| 1 | Academic Paper Writing | 8 章 | 基础规范 + 去 AI 味 + 引用透明 + 润色 | 全流程 |
| 2 | Author Style Fingerprint Engine | 7 章 | 作者/期刊风格指纹建模与迁移 | 写作前 |
| 3 | Paper Reverse Engineering | 4 章 | 单篇论文写作策略逆向工程 | 阅读/分析 |
| 4 | Reviewer Simulation & Rejection Prediction | 6 章 | 审稿模拟 + 拒稿预测 | 投稿前 |
| 5 | Top-Journal Writing Engine | 7 章 | 可发表性最大化 + 期刊画像 | 写作/修改 |

---

## 技能简介

### 1. Academic Paper Writing（学术论文写作基础规范）

全流程学术写作基础技能，以研究者身份写作。**8 章递进结构**：角色定义 → 基础原则（逻辑优先/证据驱动/科学语调/学术诚信）→ 写作框架（段落 + 章节模板）→ 引用管理（6 条子规则）→ 去 AI 味系统（7 个子节/70+ 词汇替换/8 条自查）→ 润色工作流（英文 LaTeX + 中文 Word + 润色约束）→ 质量保证（5 项检查）→ 交叉引用。

**唯一负责**：去 AI 味、引用透明、输出完整性、学术润色。

→ [`Academic-Paper-Writing/README.md`](./Academic-Paper-Writing/README.md) | 战术指令：[`skills.md`](./Academic-Paper-Writing/skills.md)

### 2. Author Style Fingerprint Engine（作者风格指纹引擎）

建模作者的科学思维过程与论证策略（非措辞模仿）。**7 章递进结构**：角色定义 → 优先级排序 → 5 层指纹提取（思维画像/引言/贡献/修辞/语言量化）→ 风格迁移（约束矩阵 + 反抄袭 + 多作者融合）→ 期刊指纹引用 → 5 种输出模式 → 交叉引用。

→ [`Author-Style-Fingerprint-Engine/README.md`](./Author-Style-Fingerprint-Engine/README.md) | 战术指令：[`skills.md`](./Author-Style-Fingerprint-Engine/skills.md)

### 3. Paper Reverse Engineering（论文逆向工程）

对单篇目标论文进行写作策略逆向工程。**4 章递进结构**：目标与区别 → 8 阶段逆向流水线（结构→引言→贡献→方法→实验→结果→图表→讨论）→ 质量保证（审稿人仿真 + 优先级）→ 交叉引用矩阵。

→ [`Paper-Reverse-Engineering/README.md`](./Paper-Reverse-Engineering/README.md) | 战术指令：[`skills.md`](./Paper-Reverse-Engineering/skills.md)

### 4. Reviewer Simulation & Rejection Prediction Engine（审稿人模拟与拒稿预测引擎）

模拟顶级期刊审稿人委员会（4 审稿人 + AE + EIC）进行预审。**6 章递进结构**：角色定义 → 使用时机（前移指导）→ 委员会架构 → 评估框架（四维 + 拒稿矩阵）→ 审稿协议（全文/投稿前/5 问自检）→ 交叉引用。

→ [`Reviewer-Simulation&Rejection-Prediction-Engine/README.md`](./Reviewer-Simulation%26Rejection-Prediction-Engine/README.md) | 战术指令：[`skills.md`](./Reviewer-Simulation&Rejection-Prediction-Engine/skills.md)

### 5. Top-Journal Writing Engine（顶级期刊写作引擎）

以最大化可发表性为目标。**7 章递进结构**：使命与哲学 → 科学叙事框架（故事链/新颖性/影响力）→ 章节级写作（引言/贡献/摘要/方法/机制）→ 实验卓越（设计/基准/统计/讨论/局限）→ 期刊特定画像（7 大领域：综合科学/生物与生态/生信/CS/工程/医学影像/遥感）→ 质量保证（4 项）→ 交叉引用。

**唯一负责**：期刊特定画像、科学叙事引擎、新颖性放大框架、可发表性优化。

→ [`Top-Journal-Writing-Engine/README.md`](./Top-Journal-Writing-Engine/README.md) | 战术指令：[`skills.md`](./Top-Journal-Writing-Engine/skills.md)

---

## 使用建议

1. **写作前**：使用 `Author Style Fingerprint Engine` 分析目标期刊/作者风格
2. **阅读阶段**：使用 `Paper Reverse Engineering` 深入理解参考论文的写作策略
3. **写作阶段**：以 `Academic Paper Writing` 为基础规范，结合 `Top-Journal Writing Engine` 提升稿件质量
4. **投稿前**：使用 `Reviewer Simulation & Rejection Prediction Engine` 进行模拟审稿，预判潜在问题

---

## 职责边界

```
Academic-Paper-Writing（唯一负责）
├── 去 AI 味（De-AI-ification）
├── 引用透明（Citation Transparency）
├── 输出完整性（Output Completeness）
├── 学术润色（English LaTeX + Chinese Word）
└── 稿件一致性检查

Top-Journal-Writing-Engine（唯一负责）
├── 期刊特定画像（7 大领域）
├── 科学叙事引擎
├── 新颖性放大框架
└── 可发表性优化

Reviewer-Simulation（唯一负责）
└── 审稿人视角评估（不含文本生成）

Author-Style-Fingerprint + Paper-Reverse-Engineering
└── 共用模块由 Fingerprint 维护，Reverse-Engineering 引用
```

---

## 文件结构

```
writing-skills/
├── README.md                                                    # 本文件（总览）
├── Academic-Paper-Writing/
│   ├── README.md                                                # 技能说明（8 章）
│   └── skills.md                                                # AI 战术指令
├── Author-Style-Fingerprint-Engine/
│   ├── README.md                                                # 技能说明（7 章）
│   └── skills.md                                                # AI 战术指令
├── Paper-Reverse-Engineering/
│   ├── README.md                                                # 技能说明（4 章）
│   └── skills.md                                                # AI 战术指令
├── Reviewer-Simulation&Rejection-Prediction-Engine/
│   ├── README.md                                                # 技能说明（6 章）
│   └── skills.md                                                # AI 战术指令
└── Top-Journal-Writing-Engine/
    ├── README.md                                                # 技能说明（7 章）
    └── skills.md                                                # AI 战术指令
```
