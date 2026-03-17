# Pre-Brief Workflow (Oracle)

## Trigger

User says: "pre-brief:", "brief me on:", or "situation report:" followed by a project or topic.
Also runs as optional first step before any session mode.

## Desired Outcome

A concise situational briefing that gives the session current ground truth — recent activity, open decisions, relevant prior principles — plus a **team recommendation** for the upcoming session.

BLE note: This workflow specifies what information is needed, not how to gather or present it. The Oracle should produce whatever briefing format best serves the upcoming session.

## Information Sources

The Oracle should consult whichever of these are relevant:
- **Git history**: Recent commits, current branch, uncommitted changes (for code projects)
- **Test status**: Last known test results, failing suites (for code projects)
- **Recent sessions**: Last 2-3 council/war council sessions on this topic
- **Principles/lessons learned**: Any relevant documented principles
- **Current focus**: Weekly plans, active commitments
- **Memory/notes**: Relevant prior decisions and context

## Team Recommendation

The Oracle assesses the problem shape and recommends a team composition:

1. **Classify the problem type**: building, deciding, checking, exploring, sequencing, unblocking
2. **Assess stakes**: reversible vs. irreversible, blast radius, time pressure
3. **Recommend a mode**:
   - **Pipe** (1 voice) — clear problem, one dimension, low stakes
   - **Flex Team** (2-3 voices) — multi-dimensional but focused, moderate stakes
   - **Council** (4 voices) — broad exploration, idea development
   - **War Council** (5-6 voices) — high stakes, irreversible, needs full rigor
4. **Name the specific archetypes** and explain what each brings to this particular topic
5. **Note who's explicitly NOT needed** and why — this prevents scope creep

The human always has final say on team composition. The Oracle recommends; you decide.

Over time, Session Value retro data should inform these recommendations.

## Output Format

```markdown
# Pre-Brief — [Project/Topic]

**Date:** YYYY-MM-DD
**Prepared for:** [Council / War Council / Flex Team / General]

## Current State
[Factual ground truth]

## Recent Activity
[What happened since last session]

## Open Questions
[Unresolved from prior sessions]

## Relevant Principles
[From past sessions or documented lessons, if applicable]

## Risk Flags
[What warrants attention]

## Recommended Team

**Mode:** [Pipe / Flex Team / Council / War Council]
**Voices:** [Named archetypes]
**Rationale:** [Why this team for this problem — problem shape, stakes, dimensions]
**Not needed:** [Which archetypes and why — prevents scope creep]
```

## Auto-Save

Pre-briefs are NOT separately saved — they are consumed by the session that follows. If the user wants to keep one, they can ask.

## Notes

- This is reconnaissance, not analysis. The Oracle reports the terrain; the session decides the strategy.
- Keep it to 1 page. If it's longer, the Oracle is doing the session's job.
- For non-code topics (career, personal, process), skip git/test sources and focus on recent sessions + context.
