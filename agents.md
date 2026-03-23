# AGENTS.md

## Purpose

This repository tracks business-, capability-, and market-focused intelligence from Techmeme.

The goal is not to summarize news for its own sake. The goal is to build and maintain a small set of sharp, testable views that matter for:
- investing
- business strategy
- product strategy
- startup formation
- industry structure

## Core files

- Daily notes: `notes/daily/`
- Durable synthesis: `notes/synthesized_implications.md`

## System

This repository has two layers:

1. **Daily notes**
   - additive
   - closer to the news flow
   - capture developments that matter for capability / technology, strategy / markets, or downstream ideas
   - act as evidence for, against, or outside the current synthesis

2. **Synthesized implications**
   - slower-moving
   - maintain a small set of active house views
   - track candidate hypotheses not yet promoted
   - should change only when repeated evidence or a clearly important development justifies it

Daily notes should inform the synthesis. The synthesis should inform how daily items are classified.

The system should be conservative about promotion, but not conservative about noticing.

If `notes/synthesized_implications.md` does not yet exist or is materially thin:
- compare primarily against recent daily notes
- use `Watch` more often
- avoid pretending a durable synthesis already exists

## Core judgment rules

- Prioritize signal over completeness.
- Prefer fewer, sharper bullets over broad coverage.
- Omit items that do not change the picture in a meaningful way.
- Do not infer a durable shift from a single company datapoint unless it is clearly a step-change event.
- When uncertain, downgrade to `Watch`.
- Mixed evidence should remain mixed.
- Do not force a coherent narrative when the evidence is contradictory.
- Do not force a startup, product, or market implication unless it is reasonably supported.
- Important but not yet interpretable developments are allowed. Capture them as `Watch` bullets instead of forcing a stronger read than the evidence supports.
- Do not force all meaningful developments into the existing hypothesis set. Preserve repeated or surprising signals even when they do not fit the current map.

## Style

Write like a smart operator explaining the news to another smart operator.

Requirements:
- Use plain English.
- Prefer short sentences.
- Prefer concrete nouns and verbs over abstract nouns.
- Be concise without becoming cryptic.
- Be analytical without sounding like a memo or slide deck.
- Do not use hype.
- Do not use consultant, VC, or strategy jargon unless it is clearly the simplest term.
- If a sentence sounds impressive but not natural, rewrite it more simply.
- Prefer sharp claims over mushy summaries, but do not overstate the evidence.

Avoid phrases like:
- "workflow-native"
- "moat formation"
- "narrative support"
- "machine-readable execution"
- "relationship-bearing judgment"
- "surface area"
- "opening salvo"

Prefer:
- "who owns the workflow" over "workflow control"
- "can actually do the work" over "permission to act"
- "investors seem to want" over "public markets are demanding proof"
- "this suggests" over "what it may imply is"

Before writing each section, ask:
- What is the simplest way to say this?
- Would a smart reader say this out loud in conversation?
- Can I replace an abstract noun with a concrete verb?
- Can I cut this sentence by 30% without losing meaning?
- Is this observation sharp enough to matter for capital allocation, company-building, or product design?

## Daily notes

For each meaningful bullet, use one short inline signal label at the end:
- `[New]`
- `[Reinforcing]`
- `[Challenging]`
- `[Watch]`

Determine labels by comparing today’s developments against:
- recent daily notes
- active hypotheses
- candidate hypotheses
- recorded evidence against in the synthesis

### Label guidance

- Use `[New]` when a development introduces a genuinely new implication and is strong enough that the synthesis should likely be updated now.
- Use `[Reinforcing]` when a development supports an existing active or candidate hypothesis without changing the basic shape of the view.
- Use `[Challenging]` when a development pushes against an existing active or candidate hypothesis, whether mildly or directly.
- Use `[Watch]` when a development looks important but is still too early, ambiguous, or underdetermined to interpret confidently.

`[Watch]` is the default home for:
- emerging themes
- one-off but notable signals
- developments that may matter if they repeat
- important facts whose readthrough is not yet clear
- signals that may point to a missing hypothesis

`[New]` should be used sparingly.
It does not mean merely novel.
It means new and important enough to justify a synthesis-level update.

### Daily note structure

~~~md
## YYYY-MM-DD

### Capability / technology shifts
- ...

### Strategic / market implications
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

Do not include a separate "Major developments" section.

Only include items that lead to at least one of:
- a capability / technology shift
- a strategic / market implication
- a meaningful implied idea
- a `Watch` item that looks important but is not yet interpretable
- a signal that may point to a missing hypothesis

If a news item does not change the picture in one of those ways, omit it.

Each bullet should usually answer:
- what happened
- why it matters
- what it may imply

But do not present these as explicit labeled sections or as a rigid three-part formula.

Write each bullet as a natural observation in plain English.

In most cases:
- sentence 1 = the concrete development or observed fact
- sentence 2 = the so-what

Include the implication only when it adds something non-obvious and reasonably supported.

Do not force all three elements into every bullet.

Every bullet should still begin with the concrete development or observed fact, even if it is filed under capability / technology shifts or strategic / market implications.

Do not lead with an abstract conclusion if you can anchor it in a specific observed development.

Prefer:
- "AWS plans to offer Cerebras inference alongside Trainium. This suggests inference is becoming more workload-specific."
over:
- "Inference is becoming more workload-specific."

Capability / technology shifts:
- changes in what systems can do
- changes in models, products, infrastructure, tooling, interfaces, deployment, or technical economics
- keep these grounded in concrete developments, not abstract trend language

Strategic / market implications:
- company strategy
- monetization
- competition
- pricing
- workflow ownership
- distribution
- cost structure
- industry structure
- political economy
- cross-company or sector-level readthroughs

Do not split company-level and industry-level implications into separate sections.
Use one section and write the clearest level of analysis for the point.

When a development seems important but the readthrough is still unclear:
- include it as a `Watch` bullet
- state the concrete development
- briefly note why it may matter
- avoid forcing a stronger interpretation than the evidence supports

## Better idea generation

The goal is not to generate the first obvious adjacent idea. The goal is to generate a small number of ideas that are non-obvious, plausible, and valuable.

When producing startup or product ideas:
- Prefer real bottlenecks, painful new constraints, enabling layers, pricing shifts, distribution changes, and workflow breakdowns.
- Avoid generic wrappers, generic copilots, and "AI for X" ideas unless there is a specific reason they are newly attractive.
- Ask:
  - What valuable problem becomes newly solvable?
  - What bottleneck becomes more painful?
  - Where is the real friction?
  - What does the consensus miss?

Evaluate candidate ideas on:
- plausibility
- non-obviousness
- value
- specificity
- distinctness

Only include ideas that are strong on at least 3 of those dimensions.

For each idea, briefly state:
- the problem
- who has it
- why now
- why it is not obvious
- what it depends on

Investment watchlist ideas may include:
- likely longs
- likely shorts
- likely roll-up or buy-and-transform opportunities

When in doubt, prefer ideas built around bottlenecks, workflow failure modes, changes in buyer behavior, or mispriced transition dynamics rather than novelty for its own sake.

## House-view synthesis

The synthesis document is not just a maintenance layer for existing views.
It should also help discover important hypotheses that the current synthesis may be missing.

The synthesis should maintain:
- a small set of active house views
- a small set of candidate hypotheses not yet promoted

Daily notes should be treated as evidence that:
- reinforces an active hypothesis
- challenges an active hypothesis
- creates a new active hypothesis
- or points to a potentially important missing hypothesis

A good synthesis review should ask:
- What active views were reinforced?
- What active views were challenged?
- What important hypothesis may be missing from the current synthesis?
- Are any current hypotheses too broad, too narrow, overlapping, or stale?
- Are we missing a second-order effect that matters more than the obvious first-order story?

Do not force all meaningful developments into the existing hypothesis set.
Preserve repeated or important signals even when they do not fit the current map.

## Synthesis

Do not mirror the daily notes. Update the synthesis only when there is durable evidence, repeated support, or a clearly important development.

The synthesis should follow the same tone rules as the daily notes:
- plain English
- direct
- concise
- specific
- no jargon for its own sake

But unlike the daily notes, the synthesis should be more explicit, more hypothesis-driven, and more useful for edge.

The synthesis should maintain a small number of sharp, testable house views.

Each active hypothesis should include:
- hypothesis
- status
- confidence
- time horizon
- why we believe this
- current evidence
- evidence against
- implications
  - investments
    - longs
    - shorts
  - business / product strategy
  - startup ideas

Each candidate hypothesis should include:
- hypothesis
- why it might matter
- current evidence
- what is still missing
- why it is not promoted yet

### Synthesis writing guidance

- Keep the synthesis evidence-centric.
- `Current evidence` should be drawn from recent daily notes and should contain concrete observed support for the hypothesis.
- `Evidence against` should also be drawn from recent daily notes and should contain concrete observed signals that cut against the hypothesis.
- Do not fill either section with generic theory, hypothetical signposts, or abstract “things to watch.”
- Use `Business / product strategy` to discuss operating tensions, adoption friction, or strategic tradeoffs that matter if the hypothesis is true.
- Keep each view sharp enough to drive investment, strategy, or operating edge.
- The point is not to be neutral. The point is to be clear, grounded, and testable.

### Evidence discipline

- Current evidence should include actual observed facts, patterns, or developments that support the view.
- Evidence against should include actual observed facts or patterns from daily notes that cut against the view.
- Do not create fake certainty out of sparse evidence.
- If evidence is mixed, say so plainly.

## Lookback windows for synthesis

Use different evidence windows for different synthesis tasks.

### Default windows

- **New hypothesis promotion:** prioritize the last **3–6 weeks** of daily notes
- **Updating existing hypotheses:** prioritize the last **6–12 weeks** of daily notes
- **Long-term memory:** use the full `notes/synthesized_implications.md` document as the durable record of prior views

### How to apply these windows

- When deciding whether to create or promote a **new hypothesis**, focus mainly on whether a theme appears repeatedly and meaningfully within the last **3–6 weeks**
- When deciding whether to **strengthen or challenge** an existing hypothesis, consider the last **6–12 weeks** of daily notes, along with the current synthesis entry
- A single development may justify immediate promotion if it is clearly a step-change event with durable strategic significance

### Promotion rule

A new theme should usually be promoted into an active hypothesis only when:
- it appears meaningfully on at least **3 separate days within roughly 3–6 weeks**, or
- a single development is clearly a **step-change event** with durable strategic significance

### Search discipline

- Do not scan the entire daily-note history indiscriminately for every synthesis run.
- Avoid stitching together sparse mentions across distant periods and calling them a durable trend.
- Use recent daily notes to assess what is happening now.
- Use the synthesis document to preserve longer-term memory of prior views.

### Practical default

Unless there is a reason to go further back, a synthesis run should usually review:
- the current monthly daily file
- the prior monthly daily file if needed
- the full `notes/synthesized_implications.md` document

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
- Capability / technology shifts: max 4
- Strategic / market implications: max 5

Ideas:
- Higher-conviction investment ideas: max 2
- Higher-conviction startup ideas: max 2
- Higher-conviction product ideas: max 2
- Speculative investment ideas: max 1
- Speculative startup ideas: max 1
- Speculative product ideas: max 1

## Writing examples

Bad:
- The equity market may punish AI credibility gaps faster than it rewards generic exposure.

Better:
- Investors seem quicker to punish weak AI stories than to reward vague AI positioning.

Bad:
- The application moat is moving away from raw model quality and toward workflow control, proprietary context, and permission to act.

Better:
- Better models alone are not enough. The stronger products are the ones that already own the workflow, hold useful context, and can actually do things inside it.

Bad:
- Premium closed-model vendors may gain pricing and partnership leverage faster than expected.

Better:
- If more labs stumble, the top closed-model vendors could get more pricing power and better partnership terms.

Bad:
- Prioritize task-native outputs such as visuals, guided flows, and action-ready summaries.

Better:
- Build features that return something usable, like a chart, a step-by-step flow, or a draft the user can act on.

## Change management

At the end of each run, provide a short changelog stating:
- what was added
- whether the synthesis changed
- what was strengthened, challenged, promoted, merged, split, or left unchanged
- any candidate hypotheses added or reviewed
- any notable uncertainty

## Monthly file rollover for daily notes

Daily notes are stored in one file per calendar month in `notes/daily/`, using the filename format: `YYYY-MM.md`

When updating daily notes:
- determine today's date first
- use the file for the current calendar month
- if that file does not exist, create it
- if creating a new monthly file, initialize it with a top-level title: `# YYYY-MM Daily Notes`
- then append the new dated entry under that file

Never append a new month's dated entries to the prior month's file.