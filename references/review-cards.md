# Review Cards

Use review cards to compress independent traces or candidate empirical paths before synthesis.

## Trace Review Card

```text
Trace:
Scope:
Core judgment:
Evidence source:
File-supported facts:
User assumptions:
Model inferences:
Unverified hypotheses:
Main risks:
Risk level: low / medium / high
Recommended revision:
Required data or files:
Executable code direction:
P-hacking concern: none / possible / high
Confidence: low / medium / high
```

## Path Review Card

```text
Path ID:
Path name:
Path family:
Research role: main / mechanism / moderation / heterogeneity / robustness / diagnostic
Model idea:
Dependent variable:
Core explanatory variable:
Mechanism or moderator:
Fixed effects:
Standard errors or clustering:
Sample:
Evidence source:
Current result status: not run / significant / insignificant / mixed / unstable
Unverified assumptions:
Main risks:
Risk level: low / medium / high
Recommended modification:
Required data:
Executable code direction:
P-hacking concern: none / possible / high
Suitable as main path: yes / conditional / no
Enter path scoring: yes / conditional / no
Confidence: low / medium / high
```

## Compression Rules

- Preserve evidence, risk, and action; discard repetitive reasoning.
- Mark missing inputs as `unverified` rather than filling gaps.
- Record insignificant or failed paths as evidence, not as waste.
- Do not let majority agreement override a better-supported minority trace.
