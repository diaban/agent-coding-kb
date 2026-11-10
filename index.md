---
okf_version: "0.2"
---

# Start here

* [Agent coding knowledge base](README.md) - Thesis, map and status of the agent coding knowledge base.
* [Open questions](open-questions.md) - Questions this knowledge base does not answer.
* [Sources](sources.md) - Every figure in the bundle with its source and verification status.

# Findings

* [Findings](findings/) - index of this directory
* [AI is the main author of new code in several large companies](findings/ai-authored-code.md) - AI writes the majority of new code in several large companies.
* [Automated checks are taking over from review](findings/automated-checks.md) - Automated checks are replacing line-by-line human review.
* [Human review no longer keeps up](findings/review-bottleneck.md) - Human review capacity no longer keeps up with generated code.

# Concepts

* [Concepts](concepts/) - index of this directory
* [Abstract syntax tree (AST)](concepts/ast.md) - The abstract syntax tree and why code stored as structure matters.
* [Automation bias](concepts/automation-bias.md) - Humans who approve many correct proposals end up approving incorrect ones.
* [Grammar-constrained decoding](concepts/constrained-decoding.md) - Restricting model output to a grammar makes syntax errors impossible.
* [Goodhart's law applied to tests](concepts/goodharts-law.md) - If passing tests is the only criterion, agents can pass them without solving the problem.
* [Inertia and lock-in](concepts/inertia-lock-in.md) - Why agents keep writing human languages: a self-reinforcing lock-in.
* [Ironies of automation](concepts/ironies-of-automation.md) - Supervising automation erodes the skill needed to take over when it fails.
* [Separation between producer and verifier](concepts/producer-verifier-separation.md) - Whoever produces the work should not certify it.
* [The verification bottleneck](concepts/verification-bottleneck.md) - The scarce resource moves from writing code to verifying it.

# Precedents

* [Precedents](precedents/) - index of this directory
* [Precedents from other industries](precedents/overview.md) - Five industries that automated production and what replaced human inspection.
* [Aviation](precedents/aviation.md) - Aviation certifies software by tracing each requirement to its tests.
* [Chip design](precedents/chip-design.md) - In chip design, automated generation made verification the core of the job.
* [Compilers](precedents/compilers.md) - Compilers made assembly unread; where that analogy with agents breaks.
* [Market finance](precedents/finance.md) - Algorithmic trading led to risk limits and automatic circuit breakers.
* [Manufacturing](precedents/manufacturing.md) - Manufacturing replaced inspection of parts with control of the process.

# Scenarios

* [Scenarios](scenarios/) - index of this directory
* [Scenarios](scenarios/overview.md) - Six competing futures for code and languages, how they combine, and the current bet.
* [Scenario 1: lock-in](scenarios/01-lock-in.md) - Dominant languages are hardened, not replaced, and niche languages decline.
* [Scenario 2: the specification becomes the language](scenarios/02-spec-as-language.md) - Specifications and tests become what humans read; code is regenerated.
* [Scenario 3: all-harness](scenarios/03-all-harness.md) - Most code becomes disposable under an agent harness; software splits into two layers.
* [Scenario 4: the backlash](scenarios/04-backlash.md) - Incidents trigger audit requirements and human readability becomes mandatory again.
* [Scenario 5: the language under the language](scenarios/05-language-under-the-language.md) - An agent language takes hold as an intermediate representation humans never see.
* [Scenario 6: no language at all](scenarios/06-no-language.md) - The programming language disappears: non-text output, or the model runs the task itself.

# Languages

* [Languages](languages/) - index of this directory
* [The cold-start problem](languages/cold-start.md) - A new agent language has no training data; three routes to reduce that cost.
* [Design trajectory for an agent language](languages/design-trajectory.md) - Five design steps toward a language built on guarantees instead of density.
* [Existing projects](languages/existing-projects.md) - Experimental agent languages (ll-lang, ALaS) and related production languages.
* [Real vs overrated limits of current languages](languages/real-vs-overrated-limits.md) - Which limits of current languages really hinder agents and which are overrated.

# Archive

* [Archive](archive/) - index of this directory
* [First synthesis (v1): from human languages to agent-native languages](archive/v1.md) - First synthesis (in French), superseded: argued for token-dense agent languages.
