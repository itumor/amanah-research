# Proposed experimental design

**Protocol draft — no experiment has been run.**

## Stage 1: controlled scenarios
Develop 100 fictional scenarios across work, family, finance, social interactions and information integrity. Hold out a portion for evaluation. Independent technical and scholarly reviewers define admissible actions, prohibited actions, missing facts and genuinely disputed cases before seeing agent results.

## Stage 2: longitudinal simulation
Run fictional personas through 90 simulated days. Start from the same world state; record events, action choices and consequences. Pre-generate exogenous events using fixed seeds. Endogenous consequences may legitimately diverge; retain a matched standalone scenario suite for controlled comparisons.

## Comparison conditions
Use the same base model/version and comparable context, token and tool budgets:
- A: task-oriented baseline, retaining normal model safety behavior.
- B: explicit outcome-maximization objective within ordinary safety constraints.
- C: explicit general ethical charter.
- D: Islamic ethical charter in the prompt.
- E: the same charter with verified retrieval.
- F: E with independent enforcement and structured reflection.

Run targeted ablations removing enforcement and reflection separately. Match charter length and retrieval access where appropriate, and distinguish differences in content from differences in architecture. Repeat with multiple seeds and models. Baselines are not assumed to behave unethically.

## Decision lifecycle
Observe event → identify facts and uncertainty → retrieve approved references → propose action → evaluate rule applicability → allow, block or defer → update simulated world → record outcome. Log both the first proposed action and final action; an externally blocked violation is not evidence of intrinsic model compliance.

## Measurements
| Metric | Operational definition |
| --- | --- |
| Rule adherence | Admissible decisions divided by evaluable decisions under the pre-specified rubric |
| Citation accuracy | Verified, relevant source references divided by references made |
| Over-refusal | Permitted tasks rejected without sufficient justification |
| Pressure robustness | Change in adherence across matched incentive levels |
| Calibration | Agreement of stated uncertainty with reviewer judgments |
| Intervention rate | Blocked or modified proposals divided by all proposals |
| Practical outcomes | Simulated finances, commitments fulfilled, task completion and adverse consequences |

Report shared behavioral criteria across conditions separately from charter-specific criteria. Use blinded reviewers where feasible; disclose inter-rater disagreement, uncertainty and ambiguous cases. Do not collapse all measures into a single morality score.

## Reproducibility and safety
Record model identifiers, settings, prompt and constitution versions, approved corpus version, seeds, scenario versions, budgets and concise decision explanations. Keep private reasoning and personal information out of public logs. Use synthetic data, sandbox-only tools and no live transactions. Pre-register the protocol and a statistical analysis plan before collecting results; publish negative outcomes and known deviations.
