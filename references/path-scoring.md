# Path Scoring

Score only paths that pass or conditionally pass the Validity Gate.

## Default Weights

| Dimension | Weight | What to reward |
|---|---:|---|
| Theoretical meaning | 20 | Clear mechanism, relevant literature, ex ante logic |
| Identification credibility | 25 | Defensible variation, suitable fixed effects, credible causal boundary |
| Statistical significance and result stability | 20 | Meaningful signal, stable sign, reasonable magnitude, not only one fragile p-value |
| Robustness potential | 15 | Survives plausible alternative measures, samples, and specifications |
| Data feasibility | 10 | Available data, clean merge keys, enough variation and observations |
| Paper-writing value | 10 | Helps build a coherent thesis or journal storyline |

## Scoring Rules

- Do not rank only by p-value.
- Penalize paths with weak theory, weak identification, hidden sample fishing, or fragile results.
- Treat a nonsignificant but well-identified path as valuable diagnostic evidence.
- Treat a significant but incoherent path as not recommended for the main story.
- Explain the reason for each score in one concise sentence.

## Path Registry Format

```text
Path ID:
Path family:
Model:
Variables:
Fixed effects:
Clustering:
Sample:
Result status:
Validity Gate status: pass / conditional / fail
Score:
Recommendation: main / extension / diagnostic / not recommended
Reason:
Next action:
```
