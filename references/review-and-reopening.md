# Review and reopening

## Review the decision independently

For research and plan reviews, give the reviewer the original user brief, constraints, decision, relevant raw evidence or access to sources, and the evidence standard. Independence means separation from the author's judgment. A separate reviewer can form an initial view from the brief and evidence before receiving the author's ranking. Give them the author's analysis after that first pass so they can test the actual reasoning. Use an available separate reviewer such as another qualified contributor or an authorized agent. If independent review is unavailable, document its status and what confidence is missing. A self-check can improve the draft while review is pending.

For **research review**, reconstruct the question and challenge how it was framed. Inspect the vocabulary, assumptions, source and abstraction coverage, shortlist and feasibility judgments. Trace critical claims to authoritative sources or observations. Seek disconfirming evidence and perform targeted independent discovery where a miss or misinterpretation could reverse the choice. Check whether stock limitations were mistaken for adaptation limits, whether adaptation estimates reflect source boundaries, and whether the strongest alternatives got a fair comparison.

For **plan review**, walk representative user workflows through each serious path. Challenge interface semantics, dependency and platform assumptions, lifecycle costs, performance estimates, and how risks are sequenced. Verify that the plan reflects the user's requirements, that material changes are explicit, and that proposed acceptance could distinguish real success from a plausible failure. Revisit the research when the plan relies on conclusions its evidence cannot support.

Get issues in terms of the claim, conflicting evidence or missing evidence, and the decision or behavior affected. Revise the work and return material changes for targeted verification. Resolve issues through supported correction, withdrawal, bounds on the claim, or an explicit owner decision about a remaining tradeoff. Record material dissent and the evidence that could resolve it. Close when material issues are resolved or explicitly accepted by the owner. Further review depends on what remains decision-relevant and what changed during revision.

Acceptance of remaining uncertainty authorizes a decision within the agreed scope; it does not turn an unverified claim into a verified one. Record what was reviewed and its revision or scope. Reopen affected conclusions when their supporting evidence or assumptions change.

## Verify the delivered product

Have an independent reviewer exercise the actual candidate through normal entry points. Identify the revision or build, inputs, environment and observed outputs so the result is reproducible. Match coverage to meaningful failure modes. A product promise about cross-platform installation needs evidence from relevant installations. A performance promise needs representative workload and configuration. A workflow that mutates important user data needs verification of the failure and recovery behavior the product promises. Implementation checks, mocks and isolated component tests can help diagnose defects. Acceptance requires evidence that establishes the promised behavior.

When coverage is incomplete, say which claim remains open and what evidence would close it. A failed check calls for diagnosis, correction and targeted re-verification. If it reveals a false assumption underlying the design, return to the affected planning or research decision first.

## Reopen the part that changed

Examples of triggers include an overlooked adoption or extraction route, a new user workflow, an invalid capacity estimate, a target platform that fails a key assumption, or real usage that exposes unexpected support work. Assess what the new information changes among requirements, evidence, architecture, estimates and acceptance. Retain findings that still apply. Reassess alternatives and forward costs using the new evidence, including the cost of undoing, migrating, or sustaining existing work.

Bring changes that cross an authorization boundary to the owner and wait for direction on that work. Use prior authorization when it covers the changed decision. Capture the actual result and remaining uncertainty in existing project records. Preserve repeatable operational steps where collaborators already look for the procedure, with rationale and applicability limits where they help future decisions.
