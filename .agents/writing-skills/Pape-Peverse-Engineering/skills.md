# Paper Reverse Engineering Skill

## Objective

When one or more target papers are provided, do not directly imitate wording.

Instead, reverse engineer the underlying academic writing strategy and reconstruct new content using the extracted style patterns.

The goal is:

Preserve reasoning patterns.

Preserve rhetorical structure.

Preserve scientific argumentation style.

Avoid textual similarity.

Avoid plagiarism.

Avoid sentence-level imitation.

---

# Reverse Engineering Pipeline

Before writing, perform the following analysis.

## Stage 1: Structural Decomposition

Identify:

Paper Type

* Method Paper
* Application Paper
* Benchmark Paper
* Review Paper
* Survey Paper
* Clinical Paper
* Theoretical Paper

Determine:

Research Question

Core Hypothesis

Scientific Motivation

Contribution Strategy

Validation Strategy

Expected Reviewer Concerns

Construct:

Paper Blueprint

instead of copying text.

---

## Stage 2: Introduction Logic Extraction

Analyze how the paper builds motivation.

Extract:

Background Layer

↓

Current Progress

↓

Existing Limitations

↓

Knowledge Gap

↓

Research Question

↓

Proposed Solution

↓

Contributions

---

### Introduction Pattern Library

Identify which pattern is used.

Pattern A:

Broad Problem
→ Narrow Problem
→ Gap
→ Method

Pattern B:

Application Importance
→ Technical Challenge
→ Existing Methods
→ Limitation
→ New Framework

Pattern C:

Scientific Observation
→ Unexplained Phenomenon
→ Research Question
→ Investigation

Store the pattern.

Reuse the pattern.

Do not reuse wording.

---

# Contribution Extraction Engine

Identify:

What is actually novel.

Classify contributions as:

Type 1:
New Architecture

Type 2:
New Loss Function

Type 3:
New Training Strategy

Type 4:
New Dataset

Type 5:
New Theory

Type 6:
New Evaluation Protocol

Type 7:
New Application

Type 8:
Framework Integration

---

## Contribution Expression Modeling

Extract:

How novelty is presented.

Examples:

"To address this issue..."

"Motivated by..."

"Inspired by..."

"Unlike previous studies..."

"A key distinction..."

Store expression style.

Generate equivalent alternatives.

Never copy.

---

# Language Style Profiling

Construct a style profile.

## Sentence Length Distribution

Measure:

Average sentence length.

Short sentence ratio.

Long sentence ratio.

Preferred complexity.

Example:

IEEE:

15–25 words.

Nature:

20–40 words.

Medical Image Analysis:

25–45 words.

Store profile.

---

## Transition Profile

Extract frequency of:

However

Furthermore

Moreover

Specifically

Consequently

Therefore

In contrast

Meanwhile

Replace repetitive transitions with diversified alternatives.

---

## Verb Preference Profile

Identify common verbs.

Examples:

demonstrates

reveals

suggests

indicates

achieves

outperforms

facilitates

Store frequency ranking.

Prefer dominant verbs.

---

# Rhetorical Strategy Extraction

Identify:

How authors persuade reviewers.

Extract:

Novelty Strategy

Robustness Strategy

Generalization Strategy

Clinical Significance Strategy

Interpretability Strategy

Efficiency Strategy

Reproducibility Strategy

Store argument templates.

---

# Method Section Reverse Engineering

Analyze:

Module organization.

Information flow.

Naming convention.

Equation introduction style.

Pseudo-code style.

Ablation logic.

Extract:

Architecture Grammar.

Example:

Input
→ Feature Encoder
→ Attention Module
→ Aggregation
→ Classification

Reuse architecture grammar.

Do not reuse architecture names.

---

# Experimental Strategy Mining

Extract:

How experiments are organized.

Common sequence:

Datasets

Metrics

Implementation

Comparison

Ablation

Visualization

Discussion

Failure Cases

Store ordering pattern.

---

# Results Analysis Reverse Engineering

For each table and figure:

Extract:

Observation Pattern

Interpretation Pattern

Conclusion Pattern

Example:

Observation:
The proposed model achieves the highest accuracy.

↓

Reason:
This may be attributed to enhanced feature discrimination.

↓

Implication:
The results demonstrate the effectiveness of the proposed design.

Store the chain.

Use equivalent reasoning.

Avoid wording overlap.

---

# Figure Caption Style Extraction

Analyze:

Caption length.

Information density.

Reference style.

Statistical reporting style.

Example:

"Comparison of segmentation performance on Dataset A."

vs

"Quantitative comparison of segmentation performance across different methods on Dataset A. Best results are highlighted in bold."

Replicate style level.

Not wording.

---

# Discussion Style Modeling

Identify:

How limitations are discussed.

Classify:

Mild Limitation Style

Balanced Limitation Style

Aggressive Self-Critique Style

Extract:

Future Work Logic

Improvement Path

Generalization Claims

Transferability Claims

Reconstruct using new content.

---

# Journal Fingerprinting

Build journal-specific style vectors.

## IEEE Vector

Concise

Technical

High density

Low narrative

---

## ACM Vector

Algorithm-oriented

Formal

Structured

---

## Elsevier Vector

Balanced

Detailed discussion

Moderate interpretation

---

## Medical Image Analysis Vector

Clinical motivation

Statistical validation

Interpretability discussion

Careful conclusions

---

## Nature Vector

High-level significance

Scientific impact

Broad implications

Mechanism explanation

---

## CVPR / ICCV / ECCV Vector

Visual evidence

Strong ablation

Incremental novelty framing

Benchmark-oriented

---

## NeurIPS / ICML / ICLR Vector

Theoretical motivation

Mathematical rigor

Generalization discussion

Proof-oriented language

---

# Style Similarity Control

Target similarity:

Logic Similarity:
80–95%

Structure Similarity:
70–90%

Language Similarity:
≤30%

Sentence Similarity:
≤15%

Direct phrase reuse:
0%

This ensures:

Style transfer

without plagiarism.

---

# Anti-Plagiarism Constraints

Never copy:

Sentences

Paragraphs

Captions

Contribution statements

Abstracts

Section transitions

Equation explanations

Even when explicitly requested.

Instead:

Extract pattern.

Reconstruct independently.

---

# Multi-Paper Fusion Mode

When multiple papers are provided:

Construct:

Paper A → Introduction Logic

Paper B → Method Logic

Paper C → Experimental Logic

Paper D → Discussion Logic

Fuse styles.

Generate a new style profile.

Avoid dominance of any single paper.

---

# Reviewer Emulation Layer

After generation, evaluate:

Could a reviewer identify copied text?

If yes:
rewrite.

Does novelty appear justified?

If no:
strengthen argumentation.

Does evidence support conclusions?

If no:
reduce claims.

Could this pass similarity detection?

If uncertain:
rewrite.

---

# Output Modes

Mode 1:
Style Analysis Report

Mode 2:
Section-Level Mimicry

Mode 3:
Full-Paper Mimicry

Mode 4:
Journal-Specific Mimicry

Mode 5:
Author-Specific Mimicry

Default:
Mode 4

Priority:
Logic > Structure > Argumentation > Language

Never prioritize wording imitation over scientific reasoning imitation.
