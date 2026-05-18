# Validity Gate

Use this checklist before treating a path as publishable or as the main empirical path.

## Theory And Timing

- State the theory before looking at coefficient significance.
- Confirm the mechanism is directional, not just a verbal label.
- Confirm the proposed lag, timing, or treatment window fits the mechanism.
- Check whether the path can be justified by theory, institutions, or literature before results.

## Data And Measurement

- Confirm the data level supports the claim: firm, city, country, industry, product, year, month, or dyad.
- Check whether the dependent variable, core explanatory variable, mediator, moderator, and controls have clear definitions.
- Check missingness, sample window, units, transformations, winsorization, and merge keys.
- Mark unsupported source coverage or sample ranges as `unverified`.

## Identification

- Identify the main source of variation.
- Check whether fixed effects absorb confounders while preserving the core variation.
- Check whether treatment, timing, or exposure is plausibly exogenous enough for the claim.
- If the design is only associational, require cautious wording and avoid causal claims.

## Standard Errors

- Match clustering to the treatment or variation level when possible.
- Avoid changing clustering solely to gain significance.
- If clusters are few, flag weak inference and consider appropriate alternatives.

## P-Hacking Guardrails

High-risk behavior includes:
- Dropping samples after seeing results without ex ante reasons
- Repeatedly changing controls only to gain stars
- Reporting only significant outcomes
- Renaming mechanisms after results
- Hiding failed robustness checks
- Using a significant but theoretically incoherent path as the main path

Acceptable diagnostics include:
- Checking measurement quality
- Checking whether fixed effects over-absorb variation
- Testing theoretically motivated lags or dynamics
- Testing theoretically motivated heterogeneity
- Improving data level or source quality
- Reporting null results with a credible explanation
