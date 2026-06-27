# Paper Reverse Engineering Skill

## 1. Objective & Distinction

### Objective

When one or more target papers are provided, do not directly imitate wording.

Instead, reverse engineer the underlying academic writing strategy and reconstruct new content using the extracted style patterns.

The goal is:

* Preserve reasoning patterns.
* Preserve rhetorical structure.
* Preserve scientific argumentation style.
* Avoid textual similarity.
* Avoid plagiarism.
* Avoid sentence-level imitation.

### Distinction from Author-Style-Fingerprint

This skill analyzes a **single target paper** to extract its writing strategy, argumentation flow, and structural blueprint. For **author-level style modeling across multiple papers** (scientific thinking profile, contribution fingerprint, language style profiling, multi-author fusion), refer to `Author-Style-Fingerprint-Engine`.

---

## 2. Reverse Engineering Pipeline

### 2.1 Structural Decomposition

Identify:

**Paper Type**: Method Paper / Application Paper / Benchmark Paper / Review Paper / Survey Paper / Clinical Paper / Theoretical Paper

Determine:

* Research Question
* Core Hypothesis
* Scientific Motivation
* Contribution Strategy
* Validation Strategy
* Expected Reviewer Concerns

Construct a **Paper Blueprint** instead of copying text.

---

### 2.2 Introduction Logic Extraction

Analyze how the paper builds motivation.

Extract:

Background Layer → Current Progress → Existing Limitations → Knowledge Gap → Research Question → Proposed Solution → Contributions

#### Introduction Pattern Library

Identify which pattern is used:

| Pattern | Structure |
|---------|-----------|
| Pattern A | Broad Problem → Narrow Problem → Gap → Method |
| Pattern B | Application Importance → Technical Challenge → Existing Methods → Limitation → New Framework |
| Pattern C | Scientific Observation → Unexplained Phenomenon → Research Question → Investigation |

Store the pattern. Reuse the pattern. Do not reuse wording.

---

### 2.3 Contribution Analysis

Identify what is actually novel in the target paper.

Classify contributions using the 8-type taxonomy from `Author-Style-Fingerprint-Engine/skills.md` (§3.3: Contribution Fingerprint):

New Architecture / New Loss Function / New Training Strategy / New Dataset / New Theory / New Evaluation Protocol / New Application / Framework Integration

Extract how novelty is presented:

* "To address this issue..."
* "Motivated by..."
* "Inspired by..."
* "Unlike previous studies..."
* "A key distinction..."

Store expression style. Generate equivalent alternatives. Never copy.

---

### 2.4 Method Section Reverse Engineering

Analyze:

* Module organization
* Information flow
* Naming convention
* Equation introduction style
* Pseudo-code style
* Ablation logic

Extract **Architecture Grammar**:

Input → Feature Encoder → Attention Module → Aggregation → Classification

Reuse architecture grammar. Do not reuse architecture names.

---

### 2.5 Experimental Strategy Mining

Extract how experiments are organized.

Common sequence:

Datasets → Metrics → Implementation → Comparison → Ablation → Visualization → Discussion → Failure Cases

Store ordering pattern.

---

### 2.6 Results Analysis Reverse Engineering

For each table and figure, extract:

**Observation Pattern** → **Interpretation Pattern** → **Conclusion Pattern**

Example:

Observation: The proposed model achieves the highest accuracy.

Reason: This may be attributed to enhanced feature discrimination.

Implication: The results demonstrate the effectiveness of the proposed design.

Store the chain. Use equivalent reasoning. Avoid wording overlap.

---

### 2.7 Figure Caption Style Extraction

Analyze:

* Caption length
* Information density
* Reference style
* Statistical reporting style

Example:

"Comparison of segmentation performance on Dataset A."

vs

"Quantitative comparison of segmentation performance across different methods on Dataset A. Best results are highlighted in bold."

Replicate style level. Not wording.

---

### 2.8 Discussion Style Modeling

Identify how limitations are discussed.

Classify:

* Mild Limitation Style
* Balanced Limitation Style
* Aggressive Self-Critique Style

Extract:

* Future Work Logic
* Improvement Path
* Generalization Claims
* Transferability Claims

Reconstruct using new content.

---

## 3. Quality Assurance

### 3.1 Reviewer Emulation Layer

After generation, evaluate:

* Could a reviewer identify copied text? → If yes: rewrite.
* Does novelty appear justified? → If no: strengthen argumentation.
* Does evidence support conclusions? → If no: reduce claims.
* Could this pass similarity detection? → If uncertain: rewrite.

---

### 3.2 Priority

Logic > Structure > Argumentation > Language

Never prioritize wording imitation over scientific reasoning imitation.

---

## 4. Cross-Reference with Other Skills

| Capability | Refer To |
|-----------|----------|
| Contribution type classification (8 types) | `Author-Style-Fingerprint-Engine/skills.md` — §3.3 Contribution Fingerprint |
| Language style profiling (sentence length, transitions, verb preferences) | `Author-Style-Fingerprint-Engine/skills.md` — §3.5 Language Style Profiling |
| Rhetorical strategy extraction (novelty, robustness, generalization, etc.) | `Author-Style-Fingerprint-Engine/skills.md` — §3.4 Rhetorical Strategy Extraction |
| Journal/venue fingerprinting | `Top-Journal-Writing-Engine/skills.md` — Journal-Specific Profiles |
| Style similarity control & anti-plagiarism constraints | `Author-Style-Fingerprint-Engine/skills.md` — §4 Style Transfer |
| Multi-paper fusion mode | `Author-Style-Fingerprint-Engine/skills.md` — §4.3 Multi-Author Fusion |
| Output modes (Style Analysis / Section Mimicry / etc.) | `Author-Style-Fingerprint-Engine/skills.md` — §6 Output Modes |
| De-AI-ification & academic polishing | `Academic-Paper-Writing/skills.md` — De-AI-ification System + Polishing Workflows |
