# 学术写作智能体技能集（Writing Skills）

本目录包含 5 个学术写作辅助技能（Skill），每个技能针对学术论文写作的不同阶段和维度提供专业化指导。所有技能均以英文编写，供 AI 智能体（Agent）在辅助学术写作时调用。

---

## 技能总览

| 序号 | 技能名称 | 核心定位 | 适用阶段 |
|------|----------|----------|----------|
| 1 | Academic Paper Writing | 学术论文写作基础规范 | 全流程 |
| 2 | Author Style Fingerprint Engine | 作者风格分析与复现 | 写作前 |
| 3 | Paper Reverse Engineering | 论文逆向工程 | 阅读/分析 |
| 4 | Reviewer Simulation & Rejection Prediction Engine | 审稿模拟与拒稿预测 | 投稿前 |
| 5 | Top-Journal Writing Engine | 顶级期刊写作优化 | 写作/修改 |

---

## 技能简介

### 1. Academic Paper Writing（学术论文写作基础规范）

全流程学术写作基础技能，以研究者身份写作，遵循 **逻辑优先 → 证据驱动 → 客观科学语调** 三大核心原则。涵盖段落构建框架、各章节结构化写作模板、**英/中文学术润色**（顶会级英文 LaTeX + 核心期刊中文 Word）以及 **去 AI 味检查清单**（破折号滥用、序数词机械化、高频 AI 词汇替换表、句式结构模式、8 条自查协议）。

→ 详见 [`Academic-Paper-Writing/README.md`](./Academic-Paper-Writing/README.md) | 战术指令：[`skills.md`](./Academic-Paper-Writing/skills.md)

### 2. Author Style Fingerprint Engine（作者风格指纹引擎）

学习并复现特定作者/研究组的科学思维过程与论证策略（非措辞模仿）。通过三层指纹构建（科学思维画像 → 引言指纹 → 贡献指纹）建模作者的推理模式、科学叙事和结构偏好。支持期刊指纹识别（6 种期刊/会议风格向量）、语言风格量化画像、多作者融合模式。去 AI 味功能统一由 `Academic Paper Writing` 负责。

→ 详见 [`Author-Style-Fingerprint-Engine/README.md`](./Author-Style-Fingerprint-Engine/README.md) | 战术指令：[`skills.md`](./Author-Style-Fingerprint-Engine/skills.md)

### 3. Paper Reverse Engineering（论文逆向工程）

对目标论文进行底层写作策略逆向工程，提取推理模式、修辞结构和科学论证风格后进行重构。涵盖：结构分解 → 引言逻辑提取 → 贡献分类（8 种类型）→ 语言风格画像 → 方法/实验/结果/讨论逆向 → 期刊指纹识别（7 种期刊/会议风格向量）→ 多论文融合模式 → 反抄袭约束。

→ 详见 [`Pape-Peverse-Engineering/README.md`](./Pape-Peverse-Engineering/README.md) | 战术指令：[`skills.md`](./Pape-Peverse-Engineering/skills.md)

### 4. Reviewer Simulation & Rejection Prediction Engine（审稿人模拟与拒稿预测引擎）

模拟顶级期刊/会议的审稿人委员会（4 位审稿人 + AE + EIC），从新颖性、方法论、实验、影响力四个维度进行预审。**新增**：全文审稿协议（Summary + Strengths + Weaknesses + Rating + Strategic Advice）、投稿前快速检查清单、拒稿风险评估矩阵（5 维度 × 3 等级）、分阶段使用时机指南。

→ 详见 [`Reviewer-Simulation&Rejection-Prediction-Engine/README.md`](./Reviewer-Simulation&Rejection-Prediction-Engine/README.md) | 战术指令：[`skills.md`](./Reviewer-Simulation&Rejection-Prediction-Engine/skills.md)

### 5. Top-Journal Writing Engine（顶级期刊写作引擎）

以**最大化可发表性**为目标，构建完整科学叙事链。包含：科学叙事引擎、新颖性放大框架、7 层高影响力引言生成器、贡献优化引擎（SMNV 标准）、章节级写作优化（摘要/方法/讨论/局限性）、审稿人期望模拟、期刊特定画像（5 种期刊/会议风格）、科学影响力生成器、5 级输出质量体系。去 AI 味统一由 `Academic Paper Writing` 负责。

→ 详见 [`Top-Journal-Writing-Engine/README.md`](./Top-Journal-Writing-Engine/README.md) | 战术指令：[`skills.md`](./Top-Journal-Writing-Engine/skills.md)

---

## 使用建议

1. **写作前**：使用 `Author Style Fingerprint Engine` 分析目标期刊/作者风格
2. **阅读阶段**：使用 `Paper Reverse Engineering` 深入理解参考论文的写作策略
3. **写作阶段**：以 `Academic Paper Writing` 为基础规范，结合 `Top-Journal Writing Engine` 提升稿件质量
4. **投稿前**：使用 `Reviewer Simulation & Rejection Prediction Engine` 进行模拟审稿，预判潜在问题

---

## 文件结构

```
writing-skills/
├── README.md                                                    # 本文件（总体骨架）
├── Academic-Paper-Writing/
│   ├── README.md                                                # 技能说明
│   └── skills.md                                                # AI 战术指令
├── Author-Style-Fingerprint-Engine/
│   ├── README.md                                                # 技能说明
│   └── skills.md                                                # AI 战术指令
├── Pape-Peverse-Engineering/
│   ├── README.md                                                # 技能说明
│   └── skills.md                                                # AI 战术指令
├── Reviewer-Simulation&Rejection-Prediction-Engine/
│   ├── README.md                                                # 技能说明
│   └── skills.md                                                # AI 战术指令
└── Top-Journal-Writing-Engine/
    ├── README.md                                                # 技能说明
    └── skills.md                                                # AI 战术指令
```
