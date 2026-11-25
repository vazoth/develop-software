# Research and reuse

## Search from the product down and from the field up

Describe the user situation, desired outcome, current workaround, environment, and the choice at stake. Learn the vocabulary used by users, relevant disciplines, and maintainers. A useful technique may be cataloged under another problem. Search the job users do, the workflow they follow, the domain model, system architectures, components, algorithms, code fragments, and the insights and optimizations behind them. Follow promising findings up to their assumptions and down to their actual implementations.

Choose sources for the claim you need. Inspect working and discontinued products, public repositories and version histories, issue discussions, documentation, standards, papers, books, theses, patents, technical talks, historical accounts, postmortems, direct observations, and practitioner explanations. Product demos show a possible workflow. Source and release artifacts can establish what ships and where extension seams exist. Issue histories can expose assumptions, unresolved platform issues, or earlier abandoned attempts. A patent or paper can describe a technique whose practicality remains to be demonstrated. A user's observed workflow can overturn a domain assumption the literature takes for granted.

These source families and abstraction levels are open-ended discovery prompts. Do not exclude one merely because it is unfamiliar, inconvenient or outside software engineering. Start broadly enough to discover alternatives to the initial framing, then investigate promising routes in depth. Make consequential coverage gaps and the reasons for exclusions visible to review. Source counts and completed checklists do not establish coverage or quality. Proprietary products may inform observable design; learning from a product and obtaining rights to reuse its implementation are separate questions.

Read sources closely when they carry a decision. Follow citations, implementation links, release history, and competing terminology. Look for evidence that would make a favored option fail or a dismissed option viable. Treat unsupported product summaries as leads. Record source version, conditions, and dates where they affect the comparison.

Identify what was actually accessible: a full text, relevant chapter, source revision, abstract or secondhand account. Do not represent an unread book or inaccessible paper as inspected evidence. Verify rights and obligations for the particular code, text, data or other material proposed for reuse against the owner's distribution and licensing requirements; source availability alone does not settle them.

## Find the right unit for each need

Work from the product's needs. For each need, find the best available source at each size: a whole product or runtime, a subsystem, a component, a function or algorithm, a technique or an idea. Where a size has no candidate, say whether you looked. The useful unit differs from need to need, and the strongest source for one need is often a small part of something whose other parts the product would never use.

Prefer the smallest unit that carries the value. Prior work can be depended on in two different ways. Its code, methods and ideas can be taken into a structure the product owns. Or the product can live inside someone else's structure: run on an engine or framework, extend an application, or fork one. The second kind decides the product's main loop, data model, interface conventions, packaging and upgrade path, and it brings every capability the whole contains. It is also the hardest choice to reverse.

Before building on a whole, list what the product needs from it and what else would come along. Cost the surplus on both sides. In the finished product it appears as size, startup time, memory, performance ceilings, imposed behaviour and platform limits. In development it appears as expressing the product's model through a foreign one, working around assumptions made for other uses, and following upgrades the product has no use for. Compare that with taking the needed parts, from this source or from better ones, into the product's own structure. A whole wins when the product needs most of it, or when separating the needed parts demonstrably costs more than carrying the rest. Being able to do the job establishes neither.

For example, a note-taking application needs rich text layout. Embedding a browser engine supplies layout along with a script runtime, a network stack and a process model. The shaping and line-breaking libraries that browsers themselves use can be linked directly. Which is better depends on how much of the browser the product will actually use, and that has to be shown.

Apply the same decomposition to work that already exists, including a prototype and the foundation it was built on. Each of its parts competes with the alternatives for that need.

## Assess reuse at the point of change

For a promising candidate, identify what to retain and the seams where it can be extended, isolated or translated. Inspect the relevant source or specification and trace the path from real input through the behavior you need. Identify required changes to interfaces, data, algorithms, dependencies, build, packaging and operations. Compare upstream integration, maintaining a fork, extracting or porting a subset, and reimplementing the method where each is plausible. Check licensing and redistribution, maintenance ownership, test fixtures and conformance, upstream change exposure, and target runtime, toolchain and deployment constraints. Estimate the hard parts with observable evidence or state what remains unknown.

For example, an offline editor may lack the export format that users require. Its document model and serializer could still support an export extension. Trace whether required document semantics survive serialization, whether the extension runs on each intended platform, and whether it can be maintained across upgrades. A standalone exporter using a published model and an application fork represent different ongoing commitments. An interesting serializer extracted from the editor may be coupled to runtime state or internal types, which changes the extraction estimate.

A hybrid is a candidate when its seams make sense. For instance, a service's high-throughput index and another product's offline sync algorithm can each work in isolation while assuming different ownership of record identity and deletion. Compare the cost of reconciling those assumptions with the quality of complete alternatives.

Before a candidate leads, try to disqualify it. Check each hard constraint and each target environment against the pinned source or the vendor's own documentation: the exact hardware generation, operating system version, toolchain, licence and distribution terms. Support stated for a platform does not establish that the particular path the product needs runs on the particular machine. Before planning work to answer a question, check whether a released build or an existing artifact already answers it.

## Be specific about what the evidence supports

Keep these distinctions visible when they affect a decision.

- **Source evidence** is what an identifiable source says or shows. Include relevant context and check whether claims apply to the selected version or environment.
- **Observation** is what was directly inspected or measured under stated conditions. Separate observed behavior from the explanation for it.
- **Deduction** follows from explicit premises. Identify which premises are established and which depend on the proposed design.
- **Induction** generalizes from observations. Describe the sample and the limits of transferring the pattern.
- **Abduction** proposes an explanation. Give plausible rivals and evidence that could distinguish them.
- **An estimate or hypothesis** specifies what is uncertain and, for consequential cases, what would narrow the uncertainty.
- **Synthesis** creates a proposed design from findings. State the compatibility assumptions and where they need validation.

Before closing, explain which findings discriminate among live paths, why the strongest rival ranks where it does, and when to reopen. State the coverage for each decision: the sizes and kinds of source searched, and what was found at each. A plausible shortlist is the starting point for the challenge described in [Review and reopening](review-and-reopening.md), and research on a decision is settled when it survives that challenge. Questions that sources and reasoning can answer are answered before then. If access or authority ends first, name the open question, what would answer it, and who can provide that.

Describe the best-supported choice under the examined conditions, without claiming exhaustive knowledge or a global optimum. A better result remains worth pursuing when new evidence justifies reopening the decision.
