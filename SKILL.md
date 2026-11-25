---
name: develop-software
description: Research, plan, and develop new standalone software products. Use for product discovery, evaluating prior art and reuse, choosing a product architecture, or delivering an independently verified new product. Routine maintenance and ad hoc internal scripts usually need a lighter workflow.
---

# Develop software

Develop a product people can install, use, and maintain in its intended environment. Start with the owner's objective, real users and workflows, hard constraints, and the decisions the current assignment is meant to resolve. Keep the user's chosen scope. Research, planning, and implementation can each be requested on their own. Research or planning does not by itself authorize product implementation, spending or publication. Probes follow the scope and authority actually supplied.

For consequential choices, compare the effort needed across development, integration, release, use, support and maintenance, together with the finished quality each option can achieve. Include performance wherever it affects users or operating cost. Treat required quality as a floor and evaluate improvements beyond it when their value warrants the effort. Changes to a requirement belong with its owner. Explain tradeoffs and uncertainties in terms the owner can act on.

Produce requested review drafts even when independent review is still pending. A request for a combined research-and-plan draft also permits provisional design work that helps expose research questions. Label unsettled findings and review status clearly. Delivering such a draft does not settle the choices, complete a review, or authorize implementation. The checkpoints below govern commitments and transitions, not the preparation of material for review.

## Research

Read [Research and reuse](references/research-and-reuse.md) for discovery, source evaluation, and adaptation assessments.

Research the product and its domain as well as its technical parts. Seek working products, prior attempts, reusable implementations, underlying methods, and explanations of why earlier approaches worked or failed. Search across abstraction levels and disciplines when they can change a choice. A finished product, a supported library, a transplantable method, and a small optimization can each redirect the design.

Compare concrete ways to adopt, integrate, modify, fork, extract, port, reimplement, transfer ideas from, or combine prior work with new work. When a promising candidate lacks a stock capability, trace what would have to change, what can be retained, and where the integration or platform burden lands before ruling it out. Surface decision-changing evidence gaps, the strongest alternative, and the conditions that would reopen the result.

Independently review the research and revise it before treating it as settled; use [Review and reopening](references/review-and-reopening.md) at this stage as well as for later reviews. By default, take the revised findings, live alternatives, and open decisions to the owner before moving into product planning. Use authority the owner already supplied for that transition. When an owner decision is required, ask and wait; silence or elapsed time is not a decision.

## Planning

Read [Planning and optimisation](references/planning-and-optimisation.md) when turning research into candidate designs, testing an assumption, or preparing a delivery plan.

Compare coherent products and the paths needed to deliver them. Check workflow fit, semantics at interfaces, support across intended platforms, and the effort to reach and sustain the promised quality. Put existing implementation on the same footing as other candidates. Its working behavior and avoidable future work matter. Effort already spent has no value on its own.

Specify the proposed product behavior, delivery sequence, decisive assumptions, and how actual acceptance will be demonstrated. If a plan exposes a gap that could change the choice, reopen the relevant research. Use bounded probes within the authorized scope when they can discriminate between live options. Independently review and revise the plan. By default, bring the revised plan and remaining decisions to the owner before implementation. An existing explicit authorization that covers the transition is sufficient.

## Review and delivery

Read [Review and reopening](references/review-and-reopening.md) for independent review, evidence to retain, and responses to new findings.

Give reviewers the original brief, source access, constraints and decision under review. Let them investigate before seeing the author's ranking. Use independent discovery or verification where it can change the conclusion. Resolve material issues with evidence or take unresolved decisions to their owner. Preserve material dissent.

Build against the authorized plan and gather independent acceptance evidence from actual product behavior in representative conditions. Use implementation findings and user feedback to correct the design, plan or research whenever the basis for an important choice changes. Resume at the affected decision and preserve work supported by the new evidence. Keep later work within the current authorization if a change needs an owner decision.

Use the project's existing records for source evidence, decisions, assumptions, review outcomes, acceptance, and reopening triggers. Record enough for another contributor to see why a choice was made and what would change it. Match the depth of research, review and documentation to the consequences of being wrong.
