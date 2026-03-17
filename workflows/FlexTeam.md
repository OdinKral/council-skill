# Flex Team Workflow

## Trigger

User names specific archetypes they want involved, in natural language:
- "let me think through X with the engineer and strategist"
- "I need the oracle and critic on this"
- "bring in the coach and oracle"
- "engineer + critic: [topic]"

Also triggered by naming 2-4 archetypes in any combination not matching a preset mode.

## Philosophy

Like assembling coworkers for a working session — not every problem needs the whole team.
Pick the voices that match the problem shape. The system tracks which combinations
produce the best results so team selection improves over time.

BLE note: This workflow specifies the assembly and feedback mechanism. It does NOT
prescribe how the archetypes interact — they should respond naturally to each other's
contributions, like colleagues in a room.

## Team Selection Guide

Not a rule — a starting intuition. The Session Value retro will refine this over time.

| Problem Shape | Suggested Team | Why |
|---------------|---------------|-----|
| "Should we build X or Y?" | Oracle + Engineer | Futures projection + practical decomposition |
| "Is this plan solid?" | Critic + Engineer | Stress-test + feasibility check |
| "How do we sequence this?" | Strategist + Engineer | Resource allocation + build order |
| "I'm stuck" | Coach + Oracle | Unblock energy + reveal unseen paths |
| "Is this getting too complex?" | Critic + Sage | Complexity audit + pattern detection |
| "What's the strategic play?" | Strategist + Oracle | Maneuver space + probability map |
| "Am I overthinking this?" | Coach + Critic | Activation energy + reality check |

These are starting points. Your instinct for who to call is the real guide.
The retro data will validate or update this table.

## Execution Steps

### 1. Identify Requested Team

Parse the user's request for archetype names. Valid members:
- **Critic** — epistemic defense, bias detection, stress-testing
- **Coach** — activation energy, experiments, momentum
- **Oracle** — probabilistic foresight, scenario branching
- **Engineer** — practical decomposition, constraint-based building
- **Strategist** — resource allocation, sequencing, external maneuver
- **Sage** — meta-patterns, drift detection, simplification

### 2. Optional Pre-Brief

If the topic involves a specific project with recent activity, offer a quick brief:
"Want me to pull a quick brief on [project] before we dive in?"

If yes, run PreBrief.md (Oracle scans state) then feed results to the team.
If no, proceed directly.

### 3. Load Requested Archetypes

Read only the archetype files the user requested from:
`archetypes/[Name].md`

Do NOT load archetypes that weren't requested. The point is focus.

### 4. Working Session

Present the topic to each voice in the order that makes sense for the problem:
- If building/deciding: let the Oracle or Critic frame first, then Engineer/Strategist respond
- If stuck/exploring: let the Coach open space first, then others fill it
- If checking/auditing: let the Critic go first

**Key difference from Council:** Voices can respond to each other. This is a working
conversation, not sequential presentations. If the Engineer's decomposition reveals
a risk the Critic missed, the Critic should react. If the Oracle's scenario changes
the Strategist's sequencing, show that.

### 5. Synthesis

After the working session, produce:
- **Working Conclusion** — what the team arrived at together
- **48-Hour Action Vector** — 1-3 concrete next moves
- **Dissent** — if any voice disagreed with the conclusion, surface it explicitly

### 6. Output Format

```markdown
---
date: YYYY-MM-DD
type: flex-team
project: [project name or "general"]
topic: [topic slug]
team: [archetype1, archetype2, ...]
---

# Flex Team — [Topic]

**Date:** YYYY-MM-DD
**Team:** [Archetype names]
**Project:** [project name or "general"]

## Context

[Brief framing of the topic and why this team was assembled]

## Working Session

[The conversation — each voice contributing in character, responding to each other.
Not rigid sections per archetype, but a flowing discussion with clear voice attribution.]

## Working Conclusion

[What the team arrived at]

## Dissent

[Any unresolved disagreement — or "None" if consensus]

## 48-Hour Action Vector

1. [Concrete action 1]
2. [Concrete action 2]
3. [Concrete action 3]

## Session Value (fill within 48 hours)

- Action taken: [ ]
- Insight I wouldn't have reached alone: [ ]
- Right team for this question: [ ] (who was missing / who wasn't needed?)
```

### 7. Auto-Save

Save to your preferred sessions directory:
```
sessions/YYYY-MM-DD_flex_[topic-slug].md
```

### 8. Store in Memory (Optional)

If you have a vector memory or embedding system, store the session for future semantic retrieval.

## Notes

- The human picks the team. The system suggests but doesn't override.
- Voices should interact naturally — this is a working session, not a presentation round.
- If mid-session it becomes clear another voice is needed, suggest adding them: "This is sounding like the Strategist should weigh in — want me to bring them in?"
- The Session Value retro is critical. Over time, Meta Reviews can analyze which team compositions produce the best action-to-insight ratio for which problem types.
- Keep sessions focused. 2-3 voices should produce a tighter conversation than 5.
