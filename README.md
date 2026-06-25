# Amazing Writing Skills — AI 学术写作智能体技能集

[English](#english) | [中文](#chinese)

---

<h2 id="english">📝 Amazing Writing Skills — AI Academic Writing Agent Skills Suite</h2>

**Amazing Writing Skills** is a curated collection of AI agent skills and prompts designed to assist researchers through every stage of academic paper writing — from ideation and drafting to revision and pre-submission review.

### 🎯 What's Inside

This repository bundles three major components:

#### 1. Writing Skills（5 Agent Skills）

A suite of five specialized agent skills covering the full academic writing lifecycle:

| Skill | Focus | Best Used |
|-------|-------|-----------|
| **Academic Paper Writing** | Fundamental writing norms for SCI/EI/IEEE/ACM papers | Entire workflow |
| **Author Style Fingerprint Engine** | Learn & reproduce a target author's scientific reasoning patterns | Pre-writing |
| **Paper Reverse Engineering** | Reverse-engineer the writing strategies of published papers | Reading & analysis |
| **Reviewer Simulation & Rejection Prediction Engine** | Simulate top-journal peer review to catch weaknesses early | Pre-submission |
| **Top-Journal Writing Engine** | Maximize publishability with advanced narrative frameworks | Writing & revision |

> All skills emphasize **logic-first, evidence-driven** writing that replicates the rhetorical patterns found in top peer-reviewed publications — not surface-level language mimicry.

#### 2. PaperSpine

A **motivation-driven** paper and report writing skill suite for Codex, Claude Code, and OpenClaw. It guides the agent through learning the target format and strong exemplars before writing, then records the rationale behind every manuscript decision.

#### 3. Awesome AI Research Writing

A community-sourced collection of battle-tested prompts and skill configurations from researchers at **MSRA**, **ByteDance Seed**, **SH AI Lab**, and top Chinese universities (PKU, USTC, SJTU). Covers translation, polishing, de-AI-ification, logic checking, figure/table captioning, and reviewer-perspective review.

### 🚀 Quick Start

1. **Pre-writing**: Use the `Author Style Fingerprint Engine` to analyze your target journal or a admired author's style.
2. **Reading phase**: Apply `Paper Reverse Engineering` to deeply understand the writing strategies of reference papers.
3. **Writing phase**: Build your draft with `Academic Paper Writing` fundamentals, then elevate it with the `Top-Journal Writing Engine`.
4. **Pre-submission**: Run the `Reviewer Simulation & Rejection Prediction Engine` to identify and fix weaknesses before real reviewers see them.

### ✨ Philosophy

```
Scientific Significance > Novelty of Method > Experimental Performance
```

Stop wasting time debugging prompts. Focus on what matters — your research.

---

<h2 id="chinese">📝 Amazing Writing Skills — AI 学术写作智能体技能集</h2>

**Amazing Writing Skills** 是一套精选的 AI 智能体（Agent）技能与 Prompt 合集，旨在助力研究者完成学术论文写作的每一个环节——从构思、起草到润色与投稿前审阅。

### 🎯 内容概览

本仓库整合了三大核心组件：

#### 1. Writing Skills（5 大智能体技能）

一套覆盖学术写作全流程的五大专项技能：

| 技能 | 核心定位 | 适用阶段 |
|------|----------|----------|
| **Academic Paper Writing** | SCI/EI/IEEE/ACM 论文写作基础规范 | 全流程 |
| **Author Style Fingerprint Engine** | 学习并复现目标作者的科学推理模式 | 写作前 |
| **Paper Reverse Engineering** | 逆向工程已发表论文的写作策略 | 阅读/分析 |
| **Reviewer Simulation & Rejection Prediction Engine** | 模拟顶级期刊审稿，提前发现拒稿风险 | 投稿前 |
| **Top-Journal Writing Engine** | 以最大化可发表性为目标的叙事框架 | 写作/修改 |

> 所有技能强调**逻辑优先、证据驱动**的写作原则，复现顶级同行评审出版物中的论证模式，而非表面的语言模仿。

#### 2. PaperSpine

一套以 **motivation（研究动机）** 为主线的论文与报告写作 skill suite，支持 Codex、Claude Code 和 OpenClaw。它引导智能体在写作前先学习目标格式和优秀范例，再记录每一个写作决策背后的逻辑。

#### 3. Awesome AI Research Writing

来自 **MSRA**、**字节跳动 Seed**、**上海 AI Lab** 以及北大、中科大、上交等顶尖高校硕博同学实战打磨的 Prompt 与 Skills 配置合集。涵盖翻译、润色、去 AI 味、逻辑检查、图表标题生成、审稿人视角审视等场景。

### 🚀 快速上手

1. **写作前**：使用 `Author Style Fingerprint Engine` 分析目标期刊或心仪作者的写作风格
2. **阅读阶段**：用 `Paper Reverse Engineering` 深入理解参考论文的写作策略
3. **写作阶段**：以 `Academic Paper Writing` 为基础规范，结合 `Top-Journal Writing Engine` 提升稿件质量
4. **投稿前**：运行 `Reviewer Simulation & Rejection Prediction Engine` 进行模拟审稿，在真实审稿人看到之前修复弱点

### ✨ 核心理念

```
科学意义 > 方法新颖性 > 实验性能
```

不要在 prompt 调试上浪费时间，把精力留给真正的科研。

---

<h2 id="structure">📂 Repository Structure</h2>

```
.
├── .agents/
│   ├── writing-skills/              # 5 大核心学术写作技能
│   │   ├── Academic-Paper-Writing/
│   │   ├── Author-Style-Fingerprint-Engine/
│   │   ├── Pape-Peverse-Engineering/
│   │   ├── Reviewer-Simulation&Rejection-Prediction-Engine/
│   │   └── Top-Journal-Writing-Engine/
│   └── skills/
│       ├── PaperSpine-main/         # PaperSpine 论文写作 skill suite
│       └── awesome-ai-research-writing/  # AI 学术写作 Prompt & Skills 合集
└── README.md
```