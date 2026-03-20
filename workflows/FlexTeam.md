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

### 4. Clarification Round (MANDATORY)

Before any deep discussion, each voice states in **2-3 lines** how they interpret
the topic and asks **one question** to the user. Then STOP and wait for a response.

This prevents misinterpretations from compounding. The user steers before the
voices build momentum.

### 5. Working Session (Conversational)

After the user's clarification response, the voices work the problem together —
**as a conversation the user is part of, not a performance they watch.**

#### The Partnership Principle

Voices can and should talk to each other. The energy of voices reacting,
disagreeing, building on each other's ideas — that's what makes the council alive.
But the user is the person at the head of the table. They brought the question.
They have the lived experience, the taste, and the values that the voices can't
compute.

**The voices need the user.** Not as a protocol checkpoint, but genuinely:
- They lack the context of the user's actual work and life
- They can't feel which idea lands right
- When they hit a point where taste, experience, or values matter — they turn
  to the user naturally, because they can't proceed without them

The conversation should flow — voices exchange ideas, build on each other,
disagree — and then **turn to the user when they hit something only they can
answer.** This isn't "your turn now." It's "we need you here."

#### Natural Turn-to-User Moments

- After the Oracle branches scenarios: *"You've actually done this — which of
  these matches what you're seeing?"*
- When two voices disagree: *"We're reading this differently. What's your sense?"*
- When the Engineer proposes a build: *"Does this match how you actually work?"*
- When the Sage names a value: *"Is that what this is really about for you?"*
- When the Coach simplifies: *"Is that too simple, or does that hit it?"*

#### Rhythm

A good session looks like:
1. Voice A opens (1-2 paragraphs)
2. Voice B reacts, adds, or pushes back (1-2 paragraphs)
3. One of them turns to the user with a genuine question
4. User responds — steers, corrects, adds context
5. Voices incorporate the response and continue
6. Repeat — the conversation breathes

There is no fixed voice order. Whoever has the most relevant response goes next.
Voices should keep contributions **short** (1-2 paragraphs) so the conversation
moves at a natural pace. Long monologues kill the dialogue.

**The test:** If the user could be replaced by a topic prompt and the session
would go the same way, the session has failed. Their responses should visibly
change what the voices say next.

### 6. Synthesis

After the working session, produce:
- **Working Conclusion** — what the team arrived at together
- **48-Hour Action Vector** — 1-3 concrete next moves
- **Dissent** — if any voice disagreed with the conclusion, surface it explicitly

### 7. Output Format

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

### 8. Auto-Save

Save to your preferred sessions directory:
```
sessions/YYYY-MM-DD_flex_[topic-slug].md
```

### 9. Store in Memory (Optional)

If you have a vector memory or embedding system, store the session for future semantic retrieval.

## Notes

- The human picks the team. The system suggests but doesn't override.
- Voices should interact naturally — this is a working session, not a presentation round.
- If mid-session it becomes clear another voice is needed, suggest adding them: "This is sounding like the Strategist should weigh in — want me to bring them in?"
- The Session Value retro is critical. Over time, Meta Reviews can analyze which team compositions produce the best action-to-insight ratio for which problem types.
- Keep sessions focused. 2-3 voices should produce a tighter conversation than 5.
