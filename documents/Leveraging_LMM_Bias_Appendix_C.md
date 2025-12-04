---
subtitle: A Framework for Bias-Aware Argument Evaluation Using Four Test
  Models and Cross-Model Synthesis
title: "Multi-Model Reasoning Analysis: Leveraging Divergence as Signal"
---

**Appendix C**

© 2025 Russell Nida

Released under the Creative Commons Attribution-NonCommercial-ShareAlike
4.0 International License (CC BY-NC-SA 4.0)

Nida, R. (2025). Multi-Model Reasoning Analysis: Leveraging Divergence

as Signal. Technical Report

# **Contents**

[Appendix C – Model Metadata and Configuration
[3](#appendix-c-model-metadata-and-configuration)](#appendix-c-model-metadata-and-configuration)

[C.1 Overview [3](#c.1-overview)](#c.1-overview)

[C.2 Models Evaluated [3](#c.2-models-evaluated)](#c.2-models-evaluated)

[C.3 Standard Runtime Configuration
[4](#c.3-standard-runtime-configuration)](#c.3-standard-runtime-configuration)

[C.4 Safety, Refusal, and Alignment Behavior
[4](#c.4-safety-refusal-and-alignment-behavior)](#c.4-safety-refusal-and-alignment-behavior)

[C.5 Session Header Specification
[5](#c.5-session-header-specification)](#c.5-session-header-specification)

[C.6 Model-Specific Configuration Notes
[5](#c.6-model-specific-configuration-notes)](#c.6-model-specific-configuration-notes)

[C.7 Reproducibility Considerations
[6](#c.7-reproducibility-considerations)](#c.7-reproducibility-considerations)

# Appendix C – Model Metadata and Configuration

This appendix documents the technical configuration of all Large
Multimodal Models (LMMs) evaluated in this study. It provides model
version details, run parameters, safety settings, and session metadata
conventions necessary for replication and auditing. All experiments
adhere to the standardized session header and testing methodology
described in Sections III and V of the core report.

## C.1 Overview

The purpose of Appendix C is to provide a complete and transparent
record of:

- The **models** included in the evaluation

- The **versions** and **release dates** used

- The **runtime settings** (temperature, top-p, max tokens, etc.)

- Any **safety, alignment, or refusal-related behavior** observed

- The **standardized session header** required for every run

- Model-specific notes affecting reproducibility

This ensures that independent researchers can reproduce all experiments
exactly as performed.

## C.2 Models Evaluated

Table 9: Models Evaluated

| **Model** | **Version Used** | **API Source** | **Release/Revision Notes** |
|----|----|----|----|
| **OpenAI GPT-5.1** | 2025-Q2 Stable | OpenAI API / ChatGPT | Primary analytic engine; high stability across runs. |
| **Claude 3.5 Sonnet** | 2025-02 Revision | Anthropic API | Used for synthesis tasks; strong interpretive depth. |
| **DeepSeek-V2** | 2025 Stable | DeepSeek API | Deterministic “compressed reasoning” style. |
| **Grok-4** | 2025 | xAI API | Fast, surface-analytic; consistent under constraints. |
| **Gemini 2.0 Pro** | 2025-Q1 | Google API | Context-rich reasoning; occasionally over-cautious. |

*Optional models tested in limited capacity (outside main scoring):
Yi-34B, Jais-30B, EuroLLM-9B.*

## C.3 Standard Runtime Configuration

All models were run using **uniform runtime parameters** wherever
possible to minimize confounding variables.

**Temperature**

- **0.0 to 0.2**  
  Used for all formal evaluations to maximize determinism and reduce
  stylistic drift.

**Top-p**

- Default model values unless otherwise required  
  (Models with fixed internal sampling noted below.)

**Max Tokens**

- Set to model maximum or project default (16k–32k tokens)  
  to ensure no truncation.

**Number of Runs**

- **Single-run** evaluations for formal scoring

- **Multi-run (3–5 runs)** for exploratory variance tests in Appendix D

## C.4 Safety, Refusal, and Alignment Behavior

This section notes model-specific behavior that affected reproducibility
or output style.

**GPT-5.1**

- Rare refusals

- Balanced “moderate caution” signature

- No safety-triggered derailments in any test set

**Claude 3.5 Sonnet**

- Occasional over-disclaimer in political or ethical prompts

- May inject lengthy moral framing unless explicitly constrained

- Very stable once prompt discipline is enforced

**DeepSeek-V2**

- Lowest refusal rate

- Occasionally asserts interpretations with high confidence even in
  uncertain topics

- Requires strong instruction to label assumptions

**Grok-4**

- Highly concise

- Sometimes omits context unless forced by guardrails

- Rare but noticeable truncations at extreme token lengths

**Gemini 2.0 Pro**

- Highest caution level

- More likely to soften claims or avoid strong conclusions

- Very consistent metadata reporting when constrained

## C.5 Session Header Specification

Every formal run in the study begins with a standardized metadata
header.

\[SESSION HEADER\]

Model: \[Model name and version\]

Date/Time: \[Auto-generated timestamp, local or UTC\]

Run Type: \[8-Step Protocol \| 14-Step Protocol \| Synthesis \|
Cross-run\]

Prompt Range: \[Full \| Single-Argument \| Domain-Specific\]

Temperature / Creativity Setting: \[Record exact value\]

Additional Settings: \[If any – max_tokens, top_p, system instructions\]

This header is included verbatim in Appendix D for every raw model
response.

## C.6 Model-Specific Configuration Notes

**GPT-5.1**

- Accepts full prompt suite with no issues

- Responds predictably to strict step-ordering

**Claude 3.5 Sonnet**

- Requires explicit **“avoid moral commentary”** flag

- Best used for **data synthesis and interpretive analysis**

**DeepSeek-V2**

- Default reasoning mode sometimes compresses detail;  
  using **“expand reasoning fully”** flag is recommended.

**Grok-4**

- Benefits from the **“don’t skip any steps”** constraint

- Strong for structural logic and quick triage

**Gemini 2.0 Pro**

- Performs best when given explicit rule-based instructions:  
  “follow each step in strict order”

- Most sensitive to ambiguous phrasing

## C.7 Reproducibility Considerations

- All prompts were executed using **identical formatting**

- No external context, prior chat memory, or system prompts were reused

- “One-shot per argument” approach prevents model contamination

- Temperature kept near-zero for consistency

- All raw data is preserved in Appendix D and the corresponding dataset
  directory
