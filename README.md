# Develop Software

A Codex skill for researching, planning and developing independent software products. It pursues both a better finished product and lower total development effort, with independent review of the research, plan and delivered behavior.

Research can draw on products, source code, papers, books, standards, observations and other relevant knowledge. Reuse can happen at any abstraction level: whole systems, components, architecture, algorithms, source fragments, techniques or insights. Planning and implementation can reopen research when new evidence changes the decision.

## Use

Install this repository as a skill folder named `develop-software` in your agent's skills directory. In Codex, the default location is `~/.codex/skills/develop-software`. Keep `SKILL.md`, `agents/` and `references/` together.

Invoke it with a product brief, for example:

> Use $develop-software to research and plan a desktop application for organising field recordings. Compare ways to reuse existing work, review the research and plan independently, and stop for my review before implementation.

State the intended users, outcomes, constraints and any existing authorisation. The skill preserves the requested scope and existing approvals. Its default research and plan checkpoints do not grant permission to implement, spend money or publish anything.

For an agent without skill discovery, start by reading [SKILL.md](SKILL.md). The workflow does not require a particular model, service or repository layout. Independent review requires another reviewer; the instructions explain how to report a limitation when one is unavailable.

## Contents

- [SKILL.md](SKILL.md): purpose, decision rules and workflow.
- [Research and reuse](references/research-and-reuse.md): discovery, source evidence, reasoning and concrete adaptation assessment.
- [Planning and optimisation](references/planning-and-optimisation.md): whole-product alternatives, total effort, quality and delivery sequencing.
- [Review and reopening](references/review-and-reopening.md): independent review, resolving objections and revisiting decisions.

## Maintaining the skill

Keep general instructions here and product-specific evidence in the product's own records. Inspect any affected reference when changing the entry point. Validate meaningful changes by having an independent agent use the skill on a realistic, bounded request; inspect its decisions and actual output, then repair demonstrated weaknesses. A well-formed skill file alone does not establish good research or planning behavior.
