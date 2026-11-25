# Review and reopening

## Challenge the decision

A review that confirms a document is accurate and consistent has checked the writing. A decision is tested by an attempt to beat it.

Give the challenger the original user brief, the constraints, the decision to be made, and access to sources. Choose someone who took no part in producing the recommendation. A contributor who supplied the leading option cannot certify it. The challenger works from the brief first, without the author's ranking, and tries to:

- find a better option for each need, at any size from a whole product down to a technique;
- disqualify the leading option against each requirement and each target environment, from primary sources;
- name what the author held fixed across candidates, took larger than the product needs, or kept because it already existed;
- find a reading of the requirements under which the result fails, and say whether the owner needs to settle that reading.

The challenger then reads the author's analysis and checks it. Trace critical claims to authoritative sources or observations. Check whether stock limitations were mistaken for adaptation limits, whether adaptation estimates reflect source boundaries, and whether any question handed to the owner could have been answered by research or a probe. For a plan, walk representative user workflows through the design. Challenge interface semantics, dependency and platform assumptions, lifecycle costs, performance estimates, and how risks are sequenced. Verify that the proposed acceptance could distinguish real success from a plausible failure.

The challenger reports the best alternative found, the strongest case against the leading option, and the evidence for each. A report that found neither says what was searched, so that an empty result can be told apart from a shallow one.

If no separate challenger is available, say so and state what confidence is missing. A self-check can improve a draft. It cannot close a decision.

## Close when a challenge comes back empty

A decision is closed when a challenge of this strength returns nothing that changes it. Resolved objections do not amount to closure, because a reviewer cannot object to an option nobody found. When a finding changes the decision, revise the work and challenge the revision, using a fresh challenger once the earlier one has become a contributor. Continue for as many rounds as closure takes.

When successive rounds keep overturning the choice, examine the pattern before continuing. Either each search has been too narrow, and the next one must cover the whole decision, or the leading options are close enough that the difference between them matters little. In the second case say so and choose the option that is cheaper to reverse.

A better option that turns up after closure, because the owner asked for more research or another review, means the closure was false. Repairing that one finding is insufficient. Identify the kind of search that would have found it, such as a size of unit never examined, a part held fixed, or a constraint never checked against the target environment, and run that search across every decision before closing again.

Resolve issues through supported correction, withdrawal, or bounds on the claim. An owner decision resolves a tradeoff that research and probes cannot separate. It does not stand in for research. Record material dissent and the evidence that could resolve it, along with what was challenged and at which revision. Acceptance of remaining uncertainty authorizes a decision within the agreed scope; it does not turn an unverified claim into a verified one. Reopen affected conclusions when their supporting evidence or assumptions change.

## Verify the delivered product

Have an independent reviewer exercise the actual candidate through normal entry points. Identify the revision or build, inputs, environment and observed outputs so the result is reproducible. Match coverage to meaningful failure modes. A product promise about cross-platform installation needs evidence from relevant installations. A performance promise needs representative workload and configuration. A workflow that mutates important user data needs verification of the failure and recovery behavior the product promises. Implementation checks, mocks and isolated component tests can help diagnose defects. Acceptance requires evidence that establishes the promised behavior.

When coverage is incomplete, say which claim remains open and what evidence would close it. A failed check calls for diagnosis, correction and targeted re-verification. If it reveals a false assumption underlying the design, return to the affected planning or research decision first.

## Reopen the part that changed

Examples of triggers include a better option found after closure, a foundation that was inherited without comparison, an overlooked adoption or extraction route, a new user workflow, an invalid capacity estimate, a target platform that fails a key assumption, or real usage that exposes unexpected support work. Assess what the new information changes among requirements, evidence, architecture, estimates and acceptance. Retain findings that still apply. Reassess alternatives and forward costs using the new evidence, including the cost of undoing or migrating existing work and the continuing cost of keeping it.

Bring changes that cross an authorization boundary to the owner and wait for direction on that work. Use prior authorization when it covers the changed decision. Capture the actual result and remaining uncertainty in existing project records. Preserve repeatable operational steps where collaborators already look for the procedure, with rationale and applicability limits where they help future decisions.
