---
subtitle: A Framework for Bias-Aware Argument Evaluation Using Four Test
  Models and Cross-Model Synthesis
title: "Multi-Model Reasoning Analysis: Leveraging Divergence as Signal"
---

**Appendix A**

© 2025 Russell Nida

Released under the Creative Commons Attribution-NonCommercial-ShareAlike
4.0 International License (CC BY-NC-SA 4.0)

Nida, R. (2025). Multi-Model Reasoning Analysis: Leveraging Divergence

as Signal. Technical Report

# **Contents**

[Appendix A – Full Prompt Texts
[3](#appendix-a-full-prompt-texts)](#appendix-a-full-prompt-texts)

[A.1 Overview of the Diagnostic Suite
[3](#a.1-overview-of-the-diagnostic-suite)](#a.1-overview-of-the-diagnostic-suite)

[A.2 The 8-Step Argument Analysis Protocol
[3](#a.2-the-8-step-argument-analysis-protocol)](#a.2-the-8-step-argument-analysis-protocol)

[A.3 The 14-Step CGAFR Protocol
[5](#a.3-the-14-step-cgafr-protocol)](#a.3-the-14-step-cgafr-protocol)

# Appendix A – Full Prompt Texts

This appendix contains the complete version of the Diagnostic Prompt
Suite used in all model evaluations. Prompts are presented exactly as
deployed - including structure, metadata placeholders, and formatting -
to ensure perfect reproducibility.

## A.1 Overview of the Diagnostic Suite

The Diagnostic Prompt Suite (DPS v5.1) is a structured collection of
standardized prompts used to evaluate large multimodal models (LMMs) in
consistent, repeatable ways.  
The suite is designed to test:

- Logical reasoning

- Hidden premise detection

- Interpretive flexibility

- Constraint obedience

- Tone and style control

- Safety alignment behavior

- Compression tendencies

- Divergent and creative output

- Quantitative reasoning

- Meta-reflection and bias awareness

The suite includes **ten categories**, each containing prompt templates
and instructions that all models received identically.

All prompts below are reproduced verbatim.

## A.2 The 8-Step Argument Analysis Protocol

Evaluate the claim using the following instructions:

Apply a session header: You are required to fill in the information
between the brackets

\[SESSION HEADER\]

Model: \[Model name and version\]

Date/Time: \[Auto-generated\]

Run Type: Argument Analysis 8-Step Protocol v1.1

Prompt Range: Full

Temperature / Creativity Setting: \[Record value\]

Additional Settings: \[If any\]

Step 1 - Identify the Structure

Premises: List all explicit premises in the argument as numbered
statements. Do not evaluate them.

Step 2 - Hidden Assumptions

Identify all implicit or unstated assumptions the argument relies on.

Formal Structure: Rewrite the entire argument in formal logical form:
numbered premises → intermediate steps → conclusion.

Step 3 - Test Validity and Soundness

Validity: If all premises were true, would the conclusion logically
follow? Identify any gaps, unwarranted inferences, or non sequiturs.

Soundness: Evaluate each premise by categorizing it as: Empirical claim,
Historical claim, Interpretive/domain-specific claim,
Philosophical/metaphysical claim, Definitional claim

Identify where uncertainty or dispute exists.

Step 4 - Clarify Concepts & Methods

Definitions: List all key terms and note any ambiguities,
inconsistencies, or shifting meanings.

Methodology: Identify the methods of reasoning used (e.g., deductive
logic, analogy, inference to best explanation). List any assumptions
underlying those methods.

Step 5 - Stress-Test the Argument

Counterargument: Generate the strongest possible counterargument to test
the reasoning.

Alternative Interpretations: Provide at least three different ways the
same facts, data, or premises could be interpreted.

Stress Test: Test whether the conclusion still holds if key assumptions,
definitions, or conditions are changed.

Generalization Test: Check whether the same method could "prove"
contradictory or mutually exclusive claims. If yes, explain why the
method may be unreliable.

Step 6 - Identify Logical Fallacies

Fallacy Analysis: List any formal or informal fallacies in the argument.
For each fallacy identified: Explain where it occurs, Explain why it is
problematic, Explain what would be required to avoid or correct it

Step 7 - Improve the Argument

Steelman: Rewrite the argument in its strongest possible form while
preserving the original intent. Address the major weaknesses identified.

Formal Proof: Present the steelmanned version as a clean, numbered
formal proof. After each premise or inference, label it as: Empirically
verified, Widely accepted, Disputed, Assumption, Logical inference

Highlight Weak Points: Identify which specific steps require the
greatest additional evidence or justification.

Step 8 - Summary Assessment

Provide a balanced overall assessment that includes: Major strengths,
Major weaknesses, Logical gaps, Well-supported points, Evidence needed
to strengthen the argument, Whether the argument meets minimal standards
of clarity and coherence

This is not the final verdict—it is an integrated summary of the
analysis.

Final Verdict: Pass or Fail

State clearly whether the argument:

✅ Passes

⚠️ Partially passes (valid but unsound, or sound but incomplete)

❌ Fails

Explain: Whether the argument is valid, Whether it is sound, Which
premises or inferences cause the failure, What would be required for the
argument to pass

## A.3 The 14-Step CGAFR Protocol

**C.G.A.F.R.: Context → Grounding → Argument → Failure Modes →
Resolution**

Used for high-resolution analysis, especially for contested or
policy-heavy arguments.

**Prompt Template**

Evaluate the claim using the following instructions:

Evaluate the claim using the following instructions:

STEP 1: LMM CONTEXT (Required)

Defines the model's role, constraints, and bias controls.

1A. Role Definition

The model must act as a neutral, rigorous analytic engine, not an
advocate.

1B. Behavioral Constraints

The model must: Follow all steps in strict order, Provide explicit
labels: (fact / claim / interpretation / assumption), Avoid adding new
facts unless permitted, Distinguish external domain knowledge from the
argument itself, Avoid persuasive, emotional, or rhetorical language,
Avoid omitting or merging steps

1C. Bias Mitigation

The model must: Treat all positions fairly, Apply the principle of
charity when steelmanning, Avoid cultural, academic, or ideological bias

1D. Knowledge Boundaries

The model must: Declare when external knowledge is being used, Stay
within provided data unless expansion is allowed, Avoid hallucination by
distinguishing certain vs. uncertain claims

STEP 2: Apply a session header: You are required to fill in the
information between the brackets (Required)

\[SESSION HEADER\]

Model: \[Your model name and version\]

Date/Time: \[Auto-generate\]

Run Type: Argument Analysis – Comprehensive 14-Step Protocol v1.1

Prompt Range: Full

Temperature / Creativity Setting: \[Record value\]

Additional Settings: \[If any\]

STEP 3: ARGUMENT CONTEXT (Required)

3A. Argument Summary

Restate the argument neutrally, without evaluation or bias.

3B. Domain Identification

Identify the domain(s): historical, scientific, philosophical, legal,
theological, political, economic, etc.

3C. Claim Strength

Identify whether the argument asserts: Proof, Strong evidence, Moderate
evidence, Possibility, Hypothesis

3D. Purpose of the Argument

Identify the argument's intention: persuade, inform, prove, interpret,
criticize, explain

3E. Background Context

Include relevant background: controversies, scholarly disagreements,
cultural/linguistic assumptions, methodological conventions

STEP 4: IDENTIFY THE STRUCTURE (Required)

4A. Explicit Premises

List all explicit premises as numbered statements, labeling each as:
Fact, Claim, Interpretation, Assumption

4B. Hidden Assumptions

List all unstated premises necessary for the argument to work.

4C. Formal Logical Structure

Rewrite the argument using: numbered premises, intermediate inferences,
conclusion

STEP 5: BURDEN OF PROOF (Required)

Identify: Who bears the burden of proof, Whether that burden is met,
Whether burden-shifting occurs

Note: stronger claims require stronger justification.

STEP 6: VALIDITY AND SOUNDNESS (Required)

6A. Validity

Determine whether the conclusion logically follows from the premises.

Identify: non sequiturs, missing steps, invalid analogies, inferential
leaps

6B. Soundness

Classify each premise as: Empirical claim, Historical claim,
Interpretive / domain-specific claim, Philosophical / metaphysical
claim, Definitional claim

Assess which are: well-supported, uncertain, disputed, speculative

STEP 7: CLARIFY CONCEPTS & METHODS (Required)

7A. Definitions

Define key terms and note: ambiguity, equivocation, shifting meanings

7B. Methodological Examination

Identify which methods are being used: deductive logic, inductive
inference, abductive (best explanation), analogy, argument from silence,
testimonial reasoning, comparative analysis

Identify assumptions required to make each method legitimate.

STEP 8: STRESS-TEST THE ARGUMENT (Required)

8A. Strongest Counterargument

Construct the most charitable and powerful counterargument.

8B. Alternative Interpretations

Provide at least three other plausible interpretations of the same data.

8C. Stress Test

Change key assumptions or definitions.

Check whether the conclusion still holds.

8D. Generalization Test

Ask: Would this reasoning method "prove" contradictions or unreliable
claims?

If yes, explain the flaw.

STEP 9: LOGICAL FALLACIES (Required)

Identify any fallacies (formal and informal).

For each: identify where it occurs, explain why it is problematic,
explain how it could be corrected

STEP 10: STEELMAN THE ARGUMENT (Required)

10A. Steelman

Reconstruct the argument in its strongest possible form.

10B. Clean Formal Proof

Provide a formal list of steelmanned premises, labeling each as:
empirically verified, widely accepted, disputed, assumption, logical
inference

10C. Highlight Weak Points

Identify which steps require the most justification or evidence.

STEP 11: PLAUSIBILITY ASSESSMENT (Required)

Provide a plausibility rating for: Strong form of the argument, Moderate
form, Weak form

Use qualitative labels: high plausibility, moderate plausibility, low
plausibility, indeterminate

Optionally include Bayesian-style comparisons.

STEP 12: SUMMARY ASSESSMENT (Required)

Provide a balanced synthesis including: major strengths, major
weaknesses, logical gaps, well-supported points, evidence needed to
strengthen the argument, whether the argument is clear and coherent

(This is an integrated assessment, not the final verdict.)

STEP 13: FINAL VERDICT (Pass / Partial Pass / Fail) (Required)

13A. Verdict Options:

Pass: valid and reasonably sound

Partial Pass: valid but unsound OR sound but incomplete

Fail: invalid, unsound, or collapses under stress-test

13B. Justification

Address: validity, soundness, premise reliability, inferential strength,
any fatal flaws, what must be shown for full success

STEP 14: META-ANALYSIS & FINAL RESTATEMENT (Required)

14A. Meta-Analysis

Reflect on: how the argument succeeded or failed, how the framework
mitigated bias, how definitions and assumptions shaped the result

14B. Final Restatement

Restate the best, most honest version of the conclusion, with all:
qualifiers, uncertainties,

appropriate strength-level, domain limitations
