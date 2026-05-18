---
name: cjm-Econ-Heavy-Skill
description: Heavy empirical review for economics and management papers. Use when Codex needs to audit data, construct variables, choose empirical paths, diagnose weak or unstable statistical significance, compare models, assess identification, design robustness/heterogeneity/mechanism tests, write Stata or Python regression code, interpret regression tables, or revise thesis/journal wording for defensible empirical claims. Trigger for Chinese or English requests involving 经管实证, 显著性不稳, 主回归, 稳健性, 异质性, 机制检验, 内生性, 投稿主线, or 最优实证路径.
---

# cjm-Econ-Heavy-Skill

## Overview

Use this skill to run a heavy empirical review for economics and management research. The goal is not to chase significant results mechanically; it is to find statistically informative paths only after theory, data, and identification pass a defensibility check.

## Activation Gate

Activate this skill for tasks involving data, variables, model choice, identification, robustness, interpretation, path selection, regression code, or paper wording. Always activate for requests about finding the best empirical path, diagnosing insignificant or unstable results, or designing a publishable empirical storyline.

Do not activate for simple rewriting, one-command execution, ordinary factual explanation, or narrow formatting edits unless the request affects empirical claims.

Treat statistical significance as one of the core factors in empirical path selection and publication feasibility. Compare significance only among paths that are theoretically reasonable, supported by data, and credible in identification. Do not reverse-engineer theory, samples, or variables purely to obtain significance.

## Evidence Intake

Start by locating and reading the user's evidence when available: datasets, variable dictionaries, regression tables, Stata do-files, Python scripts, logs, notes, manuscript paragraphs, and prior outputs.

Separate every important claim into:
- File-supported fact
- User assumption
- Model inference
- Unverified hypothesis

Mark missing data, code, variable definitions, sample windows, and regression results as `unverified`. Never invent data, coefficients, significance, sample ranges, variable meanings, or source coverage.

## Task Router

Classify the request into one or more task types:
1. Data audit
2. Variable construction
3. Identification strategy
4. Model specification
5. Regression code
6. Robustness, heterogeneity, or mechanism tests
7. Result interpretation and paper wording
8. Multi-path search and main-path selection

Only run the workflow components needed for the classified task.

## K-Path Generator

For ordinary tasks, generate 3-5 candidate empirical paths. For multi-path search, journal storyline design, or unstable-result diagnosis, generate 6-10 paths.

Candidate paths must be genuinely different, not minor variants of the same regression. Consider these path families when relevant:
- Main-effect path
- Mechanism path
- Moderation path
- Heterogeneity path
- Dynamic-effect path
- Nonlinear path
- Alternative-measure path
- Data-level upgrade path
- Endogeneity-treatment path
- Robustness-first path

If a path cannot be defended before seeing results, mark it as weak even if it might produce significance.

## Validity Gate

Screen each candidate before scoring. Check whether:
- The theoretical mechanism is clear
- The path can be supported before results by theory, institutional background, or literature
- The data level supports the claim
- Variable definitions and measurement are reasonable
- Identification is credible
- Fixed effects absorb the necessary confounders without absorbing the core variation
- Clustered standard errors are defensible
- Sample restrictions have ex ante reasons
- P-hacking risk is controlled
- The conclusion can be written cautiously and credibly

Paths that fail this gate may be retained as diagnostic attempts, but must not become the main path solely because they are significant.

## Statistical Signal Diagnostics

When results are insignificant, unstable, or unexpectedly strong, diagnose the statistical signal legally:
- Check whether the core variable has sufficient variation
- Check whether sample size, grouping, and year windows support identification
- Check whether fixed effects over-absorb the key explanatory variation
- Check whether standard-error clustering is too strict, too loose, or indefensible
- Check whether variable measurement is too coarse
- Check whether lags, dynamics, or timing better fit the theory
- Check whether theory supports heterogeneity, mechanism, or nonlinear structure

Never recommend theory-free sample trimming, repeated control-variable fishing, hidden failed attempts, or reporting only significant results.

## Parallel Empirical Review

Use selective independent traces rather than always running all traces:
- Trace A: Research question, theory, mechanism, and hypotheses
- Trace B: Data structure, sample window, and variable measurement
- Trace C: Identification, endogeneity, and causal-language boundary
- Trace D: Model specification, fixed effects, standard errors, and clustering
- Trace E: Robustness, heterogeneity, and mechanism tests
- Trace F: Code reproducibility, table interpretation, and paper writing

When subagents are available and the task is complex enough, assign separate traces as independent reviews. Keep their prompts narrow and do not leak other traces' conclusions. If subagents are unavailable or unnecessary, simulate the traces sequentially while preserving independence in the written review.

## Empirical Memory Cache

Compress each trace or candidate path into a review card. Use the card structure in `references/review-cards.md` when the task involves path comparison, multiple tests, or thesis/journal decisions.

Each card should preserve the judgment, evidence source, unverified assumptions, risks, risk level, recommended revision, data needed, executable code direction, p-hacking concern, main-path suitability, scoring eligibility, and confidence.

## Path Scoring

Score only paths that have passed or conditionally passed the Validity Gate. Use `references/path-scoring.md` for the rubric.

Default weights:
- Theoretical meaning: 20%
- Identification credibility: 25%
- Statistical significance and result stability: 20%
- Robustness potential: 15%
- Data feasibility: 10%
- Paper-writing value: 10%

Do not sort only by p-value. A significant path with weak theory, weak identification, or weak robustness must not be the main path. A nonsignificant but theoretically strong and well-identified path should remain as an important diagnostic result.

## Path Registry

When multiple paths are tried or proposed, keep a path registry. Include failed, insignificant, and not-recommended paths. Record each path's model, variables, fixed effects, clustering, result status, score, and recommendation status.

Do not delete, hide, or ignore unfavorable paths. Use the registry to distinguish:
- Best main path
- Secondary extension path
- Diagnostic path
- Not recommended path

## Synthesis Reviewer

Synthesize as the final reviewer:
1. Check evidence before models
2. Check identification before significance
3. Reconcile conflicts among traces
4. Reject pseudo-mechanisms, post hoc significance chasing, and over-causal language
5. Classify suggestions as immediately executable, needing more data, or not recommended
6. Choose the best main path, secondary extension paths, and not-recommended paths
7. Explain why the main path is better than alternatives
8. For insufficient significance, give lawful diagnostics before any model-search advice

## Output

Tailor the final response to the user's task. Include only useful sections from:
- Core conclusion
- Research-type judgment
- Evidence status
- Candidate paths
- Path scoring table
- Best main path
- Secondary extension paths
- Not-recommended paths
- Required changes
- Retainable parts
- Recommended model
- Required data
- Stata or Python code
- Regression-table interpretation
- Paper replacement text
- Risk warnings

Use cautious language for empirical claims. Clearly separate facts supported by files from unverified assumptions.

## References

- `references/review-cards.md`: card format for compressing trace and path judgments.
- `references/validity-gate.md`: legal path-screening checklist and p-hacking guardrails.
- `references/path-scoring.md`: scoring rubric and path-registry format.
