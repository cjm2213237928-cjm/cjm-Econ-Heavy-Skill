# cjm-Econ-Heavy-Skill

A Codex skill for heavy empirical review in economics and management research.

This skill helps an AI coding/research agent audit data, construct variables, compare empirical paths, diagnose weak or unstable regression results, design robustness and heterogeneity tests, write Stata or Python regression code, and revise empirical paper wording with defensible claims.

## What It Does

- Audits data, variables, sample windows, and evidence status.
- Separates file-supported facts, user assumptions, model inferences, and unverified hypotheses.
- Generates and screens candidate empirical paths before ranking them.
- Guards against p-hacking, hidden failed attempts, and significance-only model selection.
- Scores publishable paths by theory, identification, signal stability, robustness, feasibility, and writing value.
- Produces cautious empirical interpretation, code directions, and paper-ready wording when appropriate.

## Install

Clone this repository into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/cjm2213237928-cjm/cjm-Econ-Heavy-Skill.git ~/.codex/skills/cjm-Econ-Heavy-Skill
```

Restart Codex after installation. Then trigger the skill with:

```text
$cjm-Econ-Heavy-Skill
```

## Repository Structure

```text
cjm-Econ-Heavy-Skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── path-scoring.md
    ├── review-cards.md
    └── validity-gate.md
```

## Recommended Use Cases

- Economics or management empirical paper review.
- Thesis empirical strategy design.
- Regression path selection when significance is unstable.
- Robustness, heterogeneity, mechanism, or endogeneity test planning.
- Stata or Python regression workflow design.
- Conservative rewriting of empirical claims.

## License

MIT License. See [LICENSE](LICENSE).
