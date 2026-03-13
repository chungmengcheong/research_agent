# AGENTS.md

## Purpose
This repository tracks business- and capability-focused intelligence from Techmeme.

The goal is not to summarize news for its own sake.
The goal is to identify implications that matter for:
- markets and macro-sensitive sectors
- industry structure and competition
- investment watchlists
- startup opportunities
- product strategy

## Core files
- Daily notes: `notes/daily/`
- Durable synthesis: `notes/synthesized-implications.md`

## System
This repository has two layers:

1. **Daily notes**
   - additive
   - closer to the news flow
   - capture what changed, why it matters, and what it may imply

2. **Synthesized implications**
   - slower-moving
   - capture only durable, higher-signal implications
   - should change only when repeated evidence or a clearly material development justifies it

Daily notes should inform the synthesis.
The synthesis should inform how daily items are classified.

If `notes/synthesized-implications.md` does not yet exist or is materially thin:
- compare primarily against recent daily notes
- use `Tentative / watchlist` more often
- avoid pretending a durable synthesis already exists

## Core judgment rules
- Prioritize signal over completeness.
- Prefer fewer, sharper bullets over broad coverage.
- Omit items that do not change the strategic picture.
- Do not infer a durable industry shift from a single company datapoint unless it is clearly a step-change event.
- When uncertain, downgrade to `Tentative / watchlist`.
- Mixed evidence should remain mixed.
- Do not force a coherent narrative when the evidence is contradictory.

## Daily notes
For each meaningful bullet, use one inline signal label:
- New signal
- Reinforcing signal
- Material update to existing implication
- Weakening signal
- Contradictory evidence
- Tentative / watchlist

Determine labels by comparing today’s developments against:
- recent daily notes
- active implications
- watchlist implications
- recorded disconfirming evidence in the synthesis

### Daily note structure
~~~md
## YYYY-MM-DD

### Major developments
- ...

### Capability shifts
- ...

### Business / strategic implications
- ...

### Market / industry implications
- ...

### Implied ideas

#### Higher-conviction ideas
##### Investment watchlist ideas
- ...
##### Startup ideas
- ...
##### Product ideas
- ...

#### Speculative ideas worth tracking
##### Investment watchlist ideas
- ...
##### Startup ideas
- ...
##### Product ideas
- ...
~~~

### Daily note guidance
- **Major developments:** what happened
- **Capability shifts:** what appears to be changing in product, model, platform, infrastructure, or workflow capability
- **Business / strategic implications:** company strategy, competition, pricing, monetization, positioning
- **Market / industry implications:** broader sector or industry readthroughs
- **Implied ideas:** downstream interpretations, not restatements of the news

## Synthesis
Do not mirror the daily notes.
Update the synthesis only when there is durable evidence, repeated support, or a clearly material development.

For each active implication, maintain:
- title
- status
- confidence
- time horizon
- what is happening
- why it matters
- evidence base
- contradictory / disconfirming evidence
- potential implications
- contrarian view
- what would change the view

### Evidence discipline
- `Contradictory / disconfirming evidence` must contain actual observed facts or outcomes that cut against the thesis.
- Do not place hypothetical objections there.
- If no disconfirming evidence exists yet, say so explicitly.
- `Contrarian view` should contain the strongest reasonable opposing interpretation.

### Tangible examples
In `Potential implications`, include illustrative company, product, or category examples when they make the point more concrete.
Use examples to clarify the implication, not to overstate certainty.

## Ideas
Separate ideas into:
- **Higher-conviction ideas**
- **Speculative ideas worth tracking**

Rules:
- Higher-conviction ideas should be closely tied to observed developments.
- Speculative ideas are optional.
- Speculative ideas must be explicitly labeled and tied to an observed development.
- A speculative idea should usually be only one or two inferential steps beyond the evidence.
- If a speculative idea is weak or generic, omit it.

## Hard caps
These are ceilings, not targets. Empty sections are allowed.

Per daily entry:
- Major developments: max 3
- Capability shifts: max 3
- Business / strategic implications: max 3
- Market / industry implications: max 3

Ideas:
- Higher-conviction investment ideas: max 2
- Higher-conviction startup ideas: max 2
- Higher-conviction product ideas: max 2
- Speculative investment ideas: max 1
- Speculative startup ideas: max 1
- Speculative product ideas: max 1

## Style
- Plain English
- Crisp, analytical, businesslike
- No hype
- Prefer synthesis over recap
- Be explicit when evidence is ambiguous or contradictory

## Change management
At the end of each run, provide a short changelog stating:
- what was added
- whether the synthesis changed
- what was strengthened, weakened, challenged, or left unchanged
- any notable uncertainty