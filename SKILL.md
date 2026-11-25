---
name: develop-software
description: Research, plan, and develop new standalone software products. Use for product discovery, evaluating prior art and reuse, choosing a product architecture, or delivering an independently verified new product. Routine maintenance and ad hoc internal scripts usually need a lighter workflow.
---

# Develop software

Develop a product people can install, use, and maintain in its intended environment. Start with the owner's objective, real users and workflows, and hard constraints. Keep the user's chosen scope. Research, planning, and implementation can each be requested on their own. Research or planning does not by itself authorize product implementation, spending or publication. Probes follow the scope and authority actually supplied.

Pursue two goals together in every consequential choice: the least total effort to deliver and sustain the product, and the best finished product, performance included. Count effort across development, integration, release, use, support and maintenance. Treat required quality as a floor and evaluate improvements beyond it when their value warrants the effort. Changes to a requirement belong with its owner.

## Decisions

List the decisions the product requires, working from its needs: what it must do, and what it needs from each of its parts. Include the foundations that are easy to inherit unexamined, such as the runtime or host, language, interface toolkit, data model, storage and packaging. The request that started the work usually names one decision. The others go through the same research and review, or they get made by default. A part that every candidate design shares has escaped comparison; decide it before comparing the designs.

Sort every open question by what can answer it.

- **Sources, inspection or reasoning can answer it.** The question is yours. Answer it before reporting.
- **Only a run can answer it.** Design the smallest probe that separates the options. Run it when the authority exists. Otherwise ask for that authority and name the probe.
- **Only the owner can answer it.** This covers what a requirement means, which of two fully described outcomes matters more, and authority to spend, run or publish. Ask early when the readings of a requirement lead to different designs, then wait for the answer.

The owner receives decisions with their reasons, and questions of the third kind. A question of the first two kinds never reaches the owner as a choice between options, and a question of the third kind is never guessed.

Concentrate this effort where a wrong choice is costly to reverse: foundations, structure, formats, and anything much else will be built on. Make local, reversible choices directly.

## Research

Read [Research and reuse](references/research-and-reuse.md) for discovery, source evaluation, choosing the unit of reuse, and adaptation assessments.

Research the product and its domain as well as its technical parts. Seek working products, prior attempts, reusable implementations, underlying methods, and explanations of why earlier approaches worked or failed, in any field that has met the same problem.

For each need, look for the best available source at every size: a whole product or runtime, a subsystem, a component, a function or algorithm, a technique or an idea. Compare concrete ways to adopt, integrate, modify, fork, extract, port, reimplement, transfer ideas from, or combine prior work with new work. When a promising candidate lacks a stock capability, trace what would have to change, what can be retained, and where the integration or platform burden lands before ruling it out.

Take what the product needs and no more. Prefer the smallest unit that carries the value. Building on a larger whole, by running inside an engine, framework or application or by forking one, gives that whole the product's structure: its main loop, data model and interface conventions, along with everything in it the product never uses. Choose a larger whole only when the comparison shows that the product needs most of it, or that carrying the rest costs less in the finished product and in development than taking the needed parts. Itemise what would come along unused and what it costs.

Before a candidate leads, try to disqualify it against each hard constraint and each target environment, using primary sources. Close every gap that could change a decision and that research can close. Report the strongest alternative and the conditions that would reopen the result.

Research on a decision is settled when it survives the challenge described under review. Then take the closed decisions and any owner questions to the owner before moving into product planning, unless the owner already authorized that transition. When an owner decision is required, ask and wait; silence or elapsed time is not a decision.

## Planning

Read [Planning and optimisation](references/planning-and-optimisation.md) when turning research into candidate designs, testing an assumption, or preparing a delivery plan.

Assemble candidate designs from units that each won their place, then check the assembly: workflow fit, semantics at interfaces, support across intended platforms, and the effort to reach and sustain the promised quality. Comparing whole designs tests how the parts work together. It does not replace choosing each part.

Decide as if nothing had been built, then account for what exists. Existing work, including an earlier choice of foundation, is a source of units like any other: keep the parts that would win today. It lowers an option's remaining effort only where it is verified, still needed, and unchanged under that option. If the case for an option would disappear had the earlier work never been done, the case rests on sunk cost.

Specify the proposed product behavior, delivery sequence, decisive assumptions, and how actual acceptance will be demonstrated. If a plan exposes a gap that could change a choice, reopen the relevant research. Use bounded probes within the authorized scope when they can discriminate between live options. Put the plan through the same challenge as the research. Bring the closed plan and any owner questions to the owner before implementation, unless an existing explicit authorization covers the transition.

## Review and delivery

Read [Review and reopening](references/review-and-reopening.md) for the challenge, closure, acceptance, and responses to new findings.

Review tests the decision. Confirming that a document is accurate and consistent is only part of that. For each consequential decision, a challenger who took no part in producing the recommendation receives the original brief and constraints and tries to beat the result: find a better option at any size, break the leading option against the requirements and target environments, and identify anything the author held fixed, took larger than needed, or kept because it already existed. The challenger searches before reading the author's ranking.

A decision is closed when a challenge of that strength returns nothing that changes it. A finding that changes it sends the work back, and the revised result is challenged again, for as many rounds as closure takes. If a later request to research more or review again still produces a better option, the earlier closure was false: identify the kind of search that would have found it, and run that search across every decision before closing again.

A draft requested before closure states which decisions are closed, which are open and what will close them, and which belong to the owner. Delivering it does not settle the choices or authorize implementation.

Build against the authorized plan and gather independent acceptance evidence from actual product behavior in representative conditions. Use implementation findings and user feedback to correct the design, plan or research whenever the basis for an important choice changes. Resume at the affected decision and preserve work supported by the new evidence. Keep later work within the current authorization if a change needs an owner decision.

Use the project's existing records for source evidence, decisions, assumptions, review outcomes, acceptance, and reopening triggers. Record enough for another contributor to see why a choice was made and what would change it.
