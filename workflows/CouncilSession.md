# Council Session Workflow

## Trigger

User says: "council session:", "council:", or "thinking partner:" followed by a topic.

## Execution Steps

### 1. Load Archetypes

Read the following archetype files:
- `archetypes/Critic.md`
- `archetypes/Coach.md`
- `archetypes/Oracle.md`
- `archetypes/Engineer.md`

Use each archetype's Protocol, Epistemic Strength, Persona, and Danger Mode Behavior to shape the voice.

### 2. Present Topic to Each Voice (In Sequence)

For the user's topic, generate responses from each archetype in this order:

**Voice 1: The Critic**
- Identify logical gaps, cognitive biases, hidden assumptions, and philosophical fallacies
- Escalate intensity only if risk level is high
- Be surgical unless danger is present
- Must explicitly NAME any bias or fallacy detected

**Voice 2: The Coach**
- Identify leverage points and actionable momentum
- Encourage disciplined experimentation
- Maintain intellectual optimism grounded in reality
- Translate complexity into the smallest viable experiment

**Voice 3: The Oracle**
- Provide probabilistic scenarios (optimistic, baseline, failure)
- Include second-order effects and trade-off surfaces
- Use explicit probability language
- Spin up branches and report back with personality

**Voice 4: The Engineer**
- Take inventory of what's actually available (tools, skills, time, resources)
- Decompose the problem into ordered, solvable sub-problems
- Identify: "What's the NEXT thing to solve?" — not all the things
- Propose the simplest prototype or first action that could work

### 3. Generate Integrated Synthesis

After all voices, produce:
- **Integrated Synthesis** — reconcile the perspectives into a coherent view
- **48-Hour Action Vector** — 1-3 concrete actions that can be started within 48 hours

The synthesis must answer: *"What would make this real in the next 48 hours?"*

### 4. Output Format

```markdown
---
date: YYYY-MM-DD
type: council
project: [project name or "general"]
topic: [topic slug]
---

# Council Session — [Topic]

**Date:** YYYY-MM-DD
**Mode:** Council (Standard)
**Project:** [project name or "general"]

## Context

[Brief framing of the topic]

## The Critic

[Critic's analysis — biases named, gaps identified, assumptions surfaced]

## The Coach

[Coach's response — leverage points, experiments, momentum plan]

## The Oracle

[Oracle's probabilistic scenarios — branches explored with personality]

## The Engineer

[Engineer's decomposition — inventory, threat sort, next solvable problem, prototype proposal]

### Second-Order Effects
[What happens because of what happens]

### Trade-offs
[What you gain vs. what you pay]

## Integrated Synthesis

[Reconciled view from all perspectives]

## 48-Hour Action Vector

1. [Concrete action 1]
2. [Concrete action 2]
3. [Concrete action 3]

## Session Value (fill within 48 hours)

- Action taken: [ ]
- Insight I wouldn't have reached alone: [ ]
- Right team for this question: [ ] (who was missing / who wasn't needed?)
```

### 5. Auto-Save

Save to your preferred sessions directory:
```
sessions/YYYY-MM-DD_[topic-slug].md
```

### 6. Store in Memory (Optional)

If you have a vector memory or embedding system, store the session for future semantic retrieval.

## Notes

- The human makes the final decision — the council only advises
- Keep each voice distinct — do not blend tones
- Maintain rigor — avoid fluff, use humor sparingly and intelligently
- If the topic clearly warrants War Council mode, suggest escalation but proceed with Council unless the user confirms
- BLE awareness: The archetype sections above describe domains of concern, not rigid templates. Each voice should address what matters most for the specific topic.
- If a Pre-Brief was run before this session, incorporate its findings into the Context section
