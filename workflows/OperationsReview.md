# Operations Review Workflow (Strategist + Critic)

## Trigger

User says: "operations review", "process review", "SOP check", or "how are our processes working?"

## Desired Outcome

An honest assessment of whether current operational processes — tools, workflows, knowledge capture, session patterns — are serving their purpose. The Strategist evaluates effectiveness. The Critic checks for unnecessary complexity.

The output is specific, testable process recommendations — not a framework or meta-process.

BLE note: This workflow exists to REDUCE overhead, not add it. If the review itself takes longer than the processes it evaluates, something is wrong.

## Participants

**Strategist** (primary) — evaluates operational effectiveness
**Critic** — checks proposals for unnecessary complexity and BLE violations

## Process

### 1. Load Archetypes

Read:
- `archetypes/Strategist.md`
- `archetypes/Critic.md`

### 2. Strategist Assessment

For each process under review, evaluate:
- **Agency test**: Does this process increase what the human can accomplish?
- **BLE test**: Does it specify outcomes or prescribe procedures?
- **Overhead test**: How much time does the process consume vs. the value it creates?
- **Testability**: Can we run a change for 2 weeks and measure whether it helped?
- **Elimination test**: What would we lose by removing this process entirely?

### 3. Critic Check

Review the Strategist's proposals for:
- Duplication with existing processes
- Unnecessary complexity
- Solutions looking for problems
- BLE violations in the proposals themselves

### 4. Output

```markdown
# Operations Review

**Date:** YYYY-MM-DD
**Scope:** [what was reviewed]

## Strategist — Operational Assessment

### What's Working
[Processes earning their keep — specific, with evidence]

### What's Not Working
[Processes consuming more than they produce — specific, with evidence]

### Recommendations
[Specific, testable changes — each with a 2-week test plan]

## Critic — Complexity Check

### Duplication Found
[Any recommended changes that overlap with existing processes]

### BLE Violations
[Any proposals that prescribe procedures instead of specifying outcomes]

### Simplification Opportunities
[Things that should be eliminated, not improved]

## Action Items

1. [Specific change with test period]
2. [Specific change with test period]
3. [Specific change with test period]

## Review Gate

Review these changes at: [date, 2 weeks out]
Success criteria: [how to measure whether the changes helped]

## Session Value (fill within 48 hours)

- Action taken: [ ]
- Insight I wouldn't have reached alone: [ ]
- Right team for this question: [ ] (who was missing / who wasn't needed?)
```

## Notes

- Recommend a maximum of 3 changes per review. More than that and nothing gets tested.
- If the review finds everything is working, say so. The best outcome is "no changes needed."
- Invoke when friction is noticed, not on a rigid schedule.
