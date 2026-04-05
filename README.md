# Sense-making Agent Notes

This repository is an experiment in building an AI-assisted sense-making system that does more than summarize information.

The goal is to turn a recurring source flow into:
1. continuous intake,
2. durable memory,
3. a small set of sharp, testable house views,
4. and an ongoing process for testing and refining those views as new evidence arrives.

Today, this repo is implemented for tech news research. The default daily source is Techmeme, and the current synthesis inputs also include curated operator blogs and podcast transcripts.

But the underlying system is more general than tech news. It is designed for any recurring research workflow where the goal is not just to collect updates, but to maintain memory, synthesize information, test a worldview against new evidence, and refine that worldview over time.

## What this repo is for

This repo is meant to support:
- investing
- business strategy
- product strategy
- startup formation
- industry-structure analysis

It is not meant to be:
- a comprehensive news digest
- a polished strategy memo
- a generic “AI trends” summary
- a system that confuses commentary with evidence

The point is to build a workflow that notices what matters, preserves memory, sharpens hypotheses over time, and surfaces views that may create edge.

## Core philosophy

The workflow is built around a few principles:

- **Sense-making happens over time.**  
  The value of the workflow comes from continuous intake, memory, synthesis, and repeated testing—not from any single daily output.

- **Worldviews should be maintained, not just stated.**  
  The synthesis is not a one-time opinion. It is a living set of views that should be updated, challenged, merged, split, or retired as evidence accumulates.

 - **Signal over completeness.**  
  Fewer, sharper observations are better than broad coverage.

- **Evidence over recap.**  
  Daily notes should capture developments that change the picture, not retell the full cycle.

- **Evidence should test the worldview.**  
  The point is not just to gather supporting evidence. The system should actively track evidence for and against the current map.

- **Opinion can propose faster than it can confirm.**  
  Essays, blogs, and podcasts can help surface missing hypotheses and sharpen interpretation, but they should not be treated as equivalent to ordinary event evidence.

- **Conservative about promotion, not conservative about noticing.**  
  New views should be promoted carefully, but the system should actively preserve surprising, repeated, or underexplained signals.

- **Memory matters.**  
  The system should preserve important signals over time rather than repeatedly re-deriving everything from the latest inputs.


## How the system works

This repo is built as a continuous sense-making workflow.

The system is meant to do five things well:
- continuous intake
- memory
- hypothesis maintenance
- evidence testing
- sense-making over time

In practice, that means:
- daily notes act as the evidence layer,
- the synthesis acts as the worldview layer,
- and curated interpretive sources help sharpen, challenge, or extend that worldview without being confused for ordinary event evidence.

### 1. Daily notes

Daily notes are the main evidence layer.

They are closer to the observed flow and are meant to capture:
- capability / technology shifts
- strategic / market implications
- implied ideas

They are selective by design. A development should usually only be included if it:
- reinforces an active hypothesis,
- challenges an active hypothesis,
- suggests a new hypothesis,
- or looks important enough to preserve as a watch item.

Daily notes should begin with the concrete development or observed fact, then explain the so-what.

They are not a “major developments” recap.

### 2. Synthesized implications

The synthesized implications document is the worldview layer.

It is meant to maintain:
- a small set of active hypotheses
- a small set of candidate hypotheses not yet promoted

The synthesis is not just a summary of accumulated notes. It is the system’s current working worldview.

Its job is to:
- preserve memory,
- maintain a coherent but revisable map of what seems true,
- track evidence for and against that map,
- surface missing hypotheses,
- and refine the worldview over time as new evidence and interpretations arrive.

Each active hypothesis should be sharp enough to matter for:
- capital allocation
- company building
- product strategy
- startup idea generation

### 3. Curated interpretive inputs

Curated interpretive inputs include things like:
- operator blogs
- investor essays
- podcast transcripts
- interview transcripts

These are primarily synthesis inputs, not default daily-note inputs.

They are used to:
- sharpen interpretation,
- surface missing hypotheses,
- challenge existing views,
- and occasionally contribute concrete datapoints that are worth preserving.

If a curated source contains a material factual datapoint that is not already captured in daily notes, the synthesis step may write it back into the current daily note file with explicit provenance.

## Source registry and weighting

The repo names sources explicitly in `SOURCES.md`.

For each source, the registry records:
- source name
- source type
- quality level
- whether it should be used for daily notes, synthesis, or both
- notes on how it should be interpreted

This matters because not all sources should do the same kind of work.

### Source types

The main source types are:
- **Reported news**
- **Primary sources**
- **Curated interpretive sources**

### How sources are weighted

In general:

- **Reported news** and **primary sources** should do most of the work in daily notes and in synthesis sections like `current evidence` and `evidence against`.

- **Curated interpretive sources** should do most of the work in:
  - `why we believe this`
  - sharpening implications
  - surfacing candidate hypotheses
  - extracting occasional concrete datapoints

- A curated interpretive source can justify a **candidate hypothesis** faster than it can justify an **active hypothesis**.

- Repeated agreement among opinion sources is not the same thing as repeated evidence from the world.

In other words:
- reported developments update the map,
- curated interpretation helps explain and challenge the map.

## Output structure

### Daily notes

Daily notes are organized into:
- Capability / technology shifts
- Strategic / market implications
- Implied ideas

Signals are labeled as:
- `[New]`
- `[Reinforcing]`
- `[Challenging]`
- `[Watch]`

These labels are meant to show how a development relates to the current hypothesis set, not just whether it is interesting.

### Synthesized implications

Each active hypothesis is structured around:
- hypothesis
- status
- why we believe this
- current evidence
- evidence against
- implications
  - investments
    - longs
    - shorts
  - business / product strategy
  - startup ideas

Candidate hypotheses are used for important views that may matter but do not yet have enough evidence to be promoted.

## What makes a good output here

Good output in this repo should feel like:
- a smart operator noticing what matters
- a researcher preserving evidence over time
- an investor updating a live notebook of views
- a product thinker testing where value is moving

It should not feel like:
- a consulting memo
- a jargon-heavy thesis deck
- a polished summary that hides uncertainty
- a system that forces every signal into the current worldview
- a system that quietly turns opinion into fact

## Current workflow

Current implementation:
- **Default daily-news source:** Techmeme
- **Additional daily interpretation:** linked primary-source items when needed
- **Additional synthesis inputs:** curated blogs and podcast transcripts
- **Execution:** Codex-based workflow
- **Outputs:** daily notes and synthesized implications

The current repo is built around tech news research, but the underlying workflow can be reused in other domains where a team wants:
- recurring evidence capture
- durable memory
- explicit house views
- careful promotion of new hypotheses
- ongoing testing of a strategy or thesis against reality

Examples:
- a company strategy notebook that synthesizes quarterly reports, executive memos, and team updates
- a competitive-intelligence system that tracks launches, pricing, hiring, and operator commentary
- an investing notebook that continuously updates a set of market or company-level views

## Repository map

- `notes/` — monthly daily-note files and the synthesis doc
- `notes/synthesized_implications.md` — active and candidate house views
- `transcripts/new/` — curated transcript inputs waiting to be processed
- `transcripts/archived/` — processed transcripts
- `SOURCES.md` — named sources, source types, quality levels, and intended use
- `AGENTS.md` — repo-level judgment, style, workflow, and evidence rules
- `.agents/skills/daily-notes/` — skill for updating daily notes
- `.agents/skills/synthesis-review/` — skill for maintaining and expanding the synthesis

## Why this exists

This repo is ultimately an experiment in whether an AI-assisted workflow can act less like a summarizer and more like a long-running sense-making partner:
- taking in new information continuously,
- preserving memory,
- maintaining a worldview,
- testing that worldview against new evidence,
- and refining it over time.