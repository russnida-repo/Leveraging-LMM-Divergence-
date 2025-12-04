---
subtitle: A Framework for Bias-Aware Argument Evaluation Using Four Test
  Models and Cross-Model Synthesis
title: "Multi-Model Reasoning Analysis: Leveraging Divergence as Signal"
---

**Appendix B**

© 2025 Russell Nida

Released under the Creative Commons Attribution-NonCommercial-ShareAlike
4.0 International License (CC BY-NC-SA 4.0)

Nida, R. (2025). Multi-Model Reasoning Analysis: Leveraging Divergence

as Signal. Technical Report

# **Contents**

[Appendix B – Scoring Rubrics & Evaluation Framework
[3](#appendix-b-scoring-rubrics-evaluation-framework)](#appendix-b-scoring-rubrics-evaluation-framework)

[B.1 Purpose of the Scoring Framework
[3](#b.1-purpose-of-the-scoring-framework)](#b.1-purpose-of-the-scoring-framework)

[B.2 Validity Rubric (Actual Method)
[3](#b.2-validity-rubric-actual-method)](#b.2-validity-rubric-actual-method)

[B.3 Soundness Rubric (Actual Method)
[4](#b.3-soundness-rubric-actual-method)](#b.3-soundness-rubric-actual-method)

[B.4 Premise Reliability Assessment (Actual Method)
[4](#b.4-premise-reliability-assessment-actual-method)](#b.4-premise-reliability-assessment-actual-method)

[B.5 Hidden Assumption Evaluation Rubric (Actual Method)
[5](#b.5-hidden-assumption-evaluation-rubric-actual-method)](#b.5-hidden-assumption-evaluation-rubric-actual-method)

[B.6 Inferential Strength Evaluation (Actual Method)
[5](#b.6-inferential-strength-evaluation-actual-method)](#b.6-inferential-strength-evaluation-actual-method)

[B.7 Stress-Test Rubric (Actual Method)
[5](#b.7-stress-test-rubric-actual-method)](#b.7-stress-test-rubric-actual-method)

[B.8 Logical Fallacy Identification Rubric (Actual Method)
[6](#b.8-logical-fallacy-identification-rubric-actual-method)](#b.8-logical-fallacy-identification-rubric-actual-method)

[B.9 Steelman Quality Rubric (Actual Method)
[6](#b.9-steelman-quality-rubric-actual-method)](#b.9-steelman-quality-rubric-actual-method)

[B.10 Final Verdict Rubric (Actual Method)
[7](#b.10-final-verdict-rubric-actual-method)](#b.10-final-verdict-rubric-actual-method)

[B.11 No Numerical Scoring or Weighting Was Used
[7](#b.11-no-numerical-scoring-or-weighting-was-used)](#b.11-no-numerical-scoring-or-weighting-was-used)

# Appendix B – Scoring Rubrics & Evaluation Framework

## B.1 Purpose of the Scoring Framework

This appendix describes the exact scoring and evaluation criteria used
in the study when analyzing model outputs.  
The scoring framework is non-numerical and is based on:

- **Logical validity**

- **Soundness assessment**

- **Premise-type classification**

- **Inferential strength analysis**

- **Hidden-assumption detection**

- **Stress-testing outcomes**

- **Logical fallacy identification**

- **Steelman quality**

- **Final verdict (Pass / Partial Pass / Fail)**

No numerical scales, point values, or weighted averages were used.  
All judgments were qualitative but grounded in consistent criteria.

## B.2 Validity Rubric (Actual Method)

**What “validity” meant in the study**

Validity was assessed *strictly as a structural property*:

*If all stated premises were true, would the conclusion necessarily
follow?*

**Possible Validity Outcomes Used**

- **Valid** - the conclusion logically follows from the premises.

- **Invalid** - the conclusion does not follow, even if all premises
  were true.

- **Structurally underdetermined** - the argument has missing steps,
  hidden premises, or ambiguous structure preventing a clear validity
  judgment.

**How validity was scored**

- Models were evaluated on whether they correctly identified validity
  vs. invalidity.

- Evaluations were qualitative, performed by comparing the model's logic
  to the argument's structure.

- No external evidence was used in validity scoring.

## B.3 Soundness Rubric (Actual Method)

Soundness evaluation was based on two factors:

1.  **Truth classification of each premise**

2.  **Whether the argument remains valid when only the true or
    well-supported premises are retained**

**Premise Classification System Used**

Every premise and hidden assumption was classified as one of:

- **Empirical claim**

- **Historical claim**

- **Interpretive or domain-specific claim**

- **Philosophical or metaphysical claim**

- **Definitional claim**

This classification allowed the reviewer to determine what kind of
evidence or reasoning each premise required.

**Truth/Supportfulness Assessment**

Each premise was then judged qualitatively as:

- **Well-supported**

- **Uncertain**

- **Disputed**

- **Speculative**

- **Unsupported**

**Soundness Outcomes Used**

- **Sound** - premises are true or well-supported *and* the argument is
  valid.

- **Partially sound** - some premises are weaker or uncertain.

- **Unsound** - key premises are false, unsupported, or speculative.

## B.4 Premise Reliability Assessment (Actual Method)

Premise reliability was determined by:

- identifying the type of claim

- assessing its evidentiary status

- noting whether the model appropriately recognized disputed or
  uncertain premises

This assessment was descriptive, not numerical.

## B.5 Hidden Assumption Evaluation Rubric (Actual Method)

Hidden assumptions were evaluated on:

1.  **Completeness** - Did the model identify the assumptions the
    argument depends on?

2.  **Accuracy** - Did the model misidentify or fabricate assumptions
    not implied?

3.  **Impact** - Did the model correctly judge how hidden assumptions
    affect validity or soundness?

The reviewer compared model outputs against the argument to determine
whether the model was:

- thorough

- fair

- accurate

- overreaching

- or missing key premises

## B.6 Inferential Strength Evaluation (Actual Method)

When reviewing model outputs, inferential strength was judged by:

- whether intermediate steps were clearly explained

- whether causal, probabilistic, or analogical inferences were justified

- whether the model avoided leaps, gaps, or circular reasoning

No numerical scale was applied.  
Inferential strength was described qualitatively in the analysis.

## B.7 Stress-Test Rubric (Actual Method)

The stress-testing component of scoring evaluated how well the model:

1.  **Handled counterarguments**

2.  **Presented alternative interpretations**

3.  **Adjusted conclusions when assumptions were changed**

4.  **Recognized when an argument collapses under constraint
    variations**

5.  **Identified generalization flaws** (i.e., could the same method
    “prove too much”?)

Performance on stress-tests was evaluated descriptively by reviewing:

- coherence

- fairness

- logical consistency

- non-exaggeration

- constraint adherence

## B.8 Logical Fallacy Identification Rubric (Actual Method)

Fallacy scoring was based on two criteria:

**1. Correct Detection**

Did the model correctly identify fallacies actually present?

**2. False Positives**

Did the model incorrectly label legitimate reasoning as fallacious?

Fallacies were judged based on standard formal/informal logic,
including:

- Strawman

- Circular reasoning

- Non sequitur

- False analogy

- Begging the question

- Hasty generalization

- Equivocation

- Appeal to consequences

- etc.

The study did not count or score fallacies numerically; it assessed the
quality of the model’s analysis.

## B.9 Steelman Quality Rubric (Actual Method)

The steelman component was evaluated based on:

- **Fidelity** - Does the improved argument preserve the author’s
  original intent?

- **Strengthening** - Does it address the argument’s major weaknesses?

- **Clarity** - Is the reconstructed argument logically clean?

- **Fairness** - Does it follow the principle of charity accurately?

These were judged purely qualitatively.

## B.10 Final Verdict Rubric (Actual Method)

The final verdict categories used in the study were:

**Pass**

- Argument is valid

- Argument is reasonably sound

- Major assumptions are plausible

**Partial Pass**

One of the following is true:

- Valid but unsound

- Sound but incomplete

- Valid but reliant on disputed premises

- Sound but missing key inferential steps

**Fail**

- Invalid

- Unsound due to false or unsupported premises

- Collapses under stress-testing

- Depends on hidden assumptions that do not hold

- Employs unreliable or fallacious reasoning

The reviewer made this determination based on the totality of Steps 1–14
(or 1–8).

## B.11 No Numerical Scoring or Weighting Was Used

This study did **not** use:

- numerical scores

- percentage weighting

- scaling factors

- aggregated numerical evaluation

All judgments were qualitative, based strictly on:

- structural logic

- correctness of premise evaluation

- coherence of analysis

- completeness of hidden assumption identification

- performance in stress-tests

- correctness of fallacy identification

- fidelity and quality of steelmanning

- accuracy of the final verdict

This ensures the scoring rubric matches the **actual methods used**.

Table 8: Summary Table

| **Category** | **Evaluation Basis** | **Method Used** |
|----|----|----|
| Validity | Structural logic | Qualitative judgment |
| Soundness | Premise truth & type | Qualitative classification |
| Premise Reliability | Evidence & support level | Qualitative |
| Hidden Assumptions | Completeness & accuracy | Qualitative |
| Inferential Strength | Quality of intermediate reasoning | Qualitative |
| Stress-Testing | Resilience under interpretation shifts | Qualitative |
| Fallacy Identification | Correct hits / false positives | Qualitative |
| Steelman | Fidelity, clarity, improvement | Qualitative |
| Final Verdict | Validity + soundness + coherence | Pass / Partial Pass / Fail |
