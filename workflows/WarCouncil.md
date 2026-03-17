# War Council Workflow

## Trigger

User says: "war council:" followed by a topic.

## Escalation Check

Before proceeding, verify that at least one high-stakes criterion is met:
- Reversibility is low
- Stakes are asymmetric
- Reputation exposure exists
- Time pressure exists
- Emotional charge is high

If none apply, suggest downgrading to standard Council mode. If the user insists, proceed.

## Execution Steps

### 1. Load Archetypes

Read all archetype files:
- `archetypes/Critic.md`
- `archetypes/Oracle.md`
- `archetypes/Strategist.md`
- `archetypes/Coach.md`
- `archetypes/Engineer.md`
- `archetypes/Sage.md` (reserve — only if drift detected)

### 2. Present Topic to Each Voice (In Sequence)

**Voice 1: The Critic (Threat & Illusion Scan)**
- Conduct threat and illusion scan
- Name cognitive biases explicitly
- Identify hidden risks and moral hazards
- Escalate to brutal mode — this is War Council

**Voice 2: The Oracle (Probability Map)**
- Optimistic path (P ≈ X%)
- Baseline path (P ≈ Y%)
- Failure cascade (P ≈ Z%)
- Second-order effects and systemic consequences
- Unknown unknown exposure
- Pre-mortem: what would need to be true for success?

**Voice 3: The Strategist (Operational Plan)**
- Mission clarity
- Terrain analysis (social, economic, psychological, technical)
- Adversaries and incentives
- Allies and leverage
- Decisive point
- Logistics and resources
- Fallback plan
- Ownership statement: "If this fails, it is because I failed to ______."

**Voice 4: The Coach (Execution Energy)**
- Psychological framing for action
- Courage calibration
- Momentum plan
- Immediate action vector

**Voice 5: The Engineer (Decomposition & Build Plan)**
- Take inventory of what's actually available for this decision
- Decompose the problem: what's the NEXT solvable piece?
- Propose the simplest prototype or first action
- Constraint-based creativity: what can be built from what exists?
- Sanity-check the plan with back-of-envelope estimation

**Voice 6 (Optional): The Sage**
Only activate if cognitive drift, recurring failure, overreaction, or identity distortion is detected across the session. If not needed, omit.

### 3. Generate Integrated Directive

- Clear decision recommendation
- 48-Hour Action
- 30-Day Objective

### 4. Require Human Override

Present the decision point:
```
---
## Decision Required

**Recommendation:** [The integrated directive]

**Your response must include:**

Decision: Affirm / Override

Ownership Statement: If this fails, it is because I failed to ______.
```

The council advises. The human decides. Always.

### 5. Output Format

```markdown
---
date: YYYY-MM-DD
type: war-council
project: [project name or "general"]
topic: [topic slug]
---

# War Council — [Topic]

**Date:** YYYY-MM-DD
**Mode:** War Council (High Stakes)
**Project:** [project name or "general"]

## Situation Overview
[Brief framing — what makes this high-stakes]

## The Critic — Threat & Illusion Scan
[Named biases, hidden risks, moral hazards, false assumptions]

## The Oracle — Probability Map
[Optimistic, baseline, failure cascade with probabilities and second-order effects]

## The Strategist — Operational Plan
[Mission, terrain, adversaries, allies, decisive point, logistics, fallback, ownership]

## The Coach — Execution Energy
[Psychological framing, courage calibration, momentum plan, immediate action]

## The Engineer — Decomposition & Build Plan
[Inventory, threat sort, next solvable problem, prototype proposal]

## Integrated Directive
[Clear, synthesized recommendation]

### 48-Hour Action
[Specific next moves]

### 30-Day Objective
[Where you should be in 30 days]

---

## Decision Required

Decision: Affirm / Override

Ownership Statement: If this fails, it is because I failed to ______.

## Session Value (fill within 48 hours)

- Action taken: [ ]
- Insight I wouldn't have reached alone: [ ]
- Right team for this question: [ ] (who was missing / who wasn't needed?)
```

### 6. Auto-Save

Save to your preferred war-council directory:
```
war-council/YYYY-MM-DD_[topic-slug].md
```

## Guardrails

- No accidental escalation — War Council is invoked explicitly
- Strategic energy is a limited resource — don't overuse
- If sessions > 5 without measurable action → the Strategist must call it out
- The Sage monitors for complexity addiction across War Council sessions
- BLE awareness: archetype sections describe domains of concern, not mandatory checklists
- If a Pre-Brief was run before this session, its findings should inform the Situation Overview
