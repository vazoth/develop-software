# Develop Software

A Codex skill for researching, planning and developing independent software products. It pursues both a better finished product and lower total development effort, with independent review of the research, plan and delivered behavior.

Research can draw on products, source code, papers, books, standards, observations and other relevant knowledge. Reuse can happen at any abstraction level: whole systems, components, architecture, algorithms, source fragments, techniques or insights. Planning and implementation can reopen research when new evidence changes the decision.

## Install

Use a separate installed copy for normal use. In Codex, ask `$skill-installer` to install the root of `vazoth/develop-software` as `develop-software`, selecting a release tag or full commit SHA. The installer's corresponding options are `--repo vazoth/develop-software --path . --name develop-software --ref <tag-or-commit>`.

The default destination is `~/.codex/skills/develop-software`, or `$CODEX_HOME/skills/develop-software` when configured. Keep `SKILL.md`, `agents/` and `references/` together. Choose and verify a new revision before replacing an existing installation. An installed copy stays stable while the source repository changes.

After installation, the skill is available on the next turn.

## Use

Invoke it with a product brief, for example:

> Use $develop-software to research and plan a desktop application for organising field recordings. Compare ways to reuse existing work, review the research and plan independently, and stop for my review before implementation.

State the intended users, outcomes, constraints and any existing authorisation. The skill preserves the requested scope and existing approvals. Its default research and plan checkpoints do not grant permission to implement, spend money or publish anything.

For an agent without skill discovery, start by reading [SKILL.md](SKILL.md). The workflow does not require a particular model, service or repository layout. Independent review requires another reviewer; the instructions explain how to report a limitation when one is unavailable.

## Contents

- [SKILL.md](SKILL.md): purpose, decision rules and workflow.
- [Research and reuse](references/research-and-reuse.md): discovery, source evidence, reasoning and concrete adaptation assessment.
- [Planning and optimisation](references/planning-and-optimisation.md): whole-product alternatives, total effort, quality and delivery sequencing.
- [Review and reopening](references/review-and-reopening.md): independent review, resolving objections and revisiting decisions.
