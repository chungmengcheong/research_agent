---
name: synthesis-review
description: Review and conservatively update notes/synthesized_implications.md after the daily notes have been updated. Use this when the task is to maintain sharp house views, test them against recent evidence, process curated transcripts, surface missing hypotheses, and optionally write back concrete transcript datapoints into daily notes.
---

Read:
- AGENTS.md
- SOURCES.md
- notes/synthesized_implications.md
- the current monthly file in `notes/`
- recent adjacent daily notes files as needed for evidence
- every unprocessed curated transcript in `transcripts/new/`

Task:
- review notes/synthesized_implications.md conservatively
- update it only if recent evidence justifies a real change
- process curated transcripts in `transcripts/new/`
- use curated transcripts to sharpen interpretation, test hypotheses, surface candidate hypotheses, and extract material datapoints
- do not rewrite the document just to refresh wording
- only write back transcript-derived datapoints into daily notes when AGENTS.md writeback conditions are met
- after a transcript is fully processed, move it from `transcripts/new/` to `transcripts/archived/`

Follow AGENTS.md for:
- synthesis structure
- tone and style
- evidence discipline
- promotion rules
- lookback windows
- merge / split / challenge logic
- transcript source handling

Run-specific reminders:
- No change is a normal outcome.
- Most runs should result in no edit or only a small targeted edit.
- Do not mirror the daily notes.
- Maintain a small number of sharp house views, not a broad catalog.
- Also look for important hypotheses the current synthesis may be missing.
- Do not force new evidence into an existing hypothesis if it fits poorly.
- Weight sources using `SOURCES.md` and AGENTS.md source-weighting rules.
- Reported news and primary sources should do most of the work in `current evidence` and `evidence against`.
- Curated interpretive sources should do most of the work in `why we believe this`, candidate hypotheses, and sharpening implications.
- Do not promote an active hypothesis mainly because several opinion sources agree with each other.
- Distinguish inside transcripts between:
  - factual datapoints
  - first-hand operator observations
  - interpretation
  - speculation
- For each extracted item, decide not just what it is, but how much evidentiary weight it deserves based on source type and quality.
- A good review may conclude that:
  - an active hypothesis was reinforced
  - an active hypothesis was challenged
  - a new active hypothesis should be promoted
  - a candidate hypothesis should be added
  - two hypotheses should be merged
  - one hypothesis should be split into two sharper ones
- `[New]` daily-note signals may justify a synthesis update, but not automatically; check whether they are strong enough and durable enough.
- `[Reinforcing]` signals usually strengthen an existing hypothesis rather than create a new one.
- `[Challenging]` signals should update confidence, evidence against, or the hypothesis itself when warranted.
- `[Watch]` signals should usually remain in the daily layer or candidate-hypothesis layer unless repetition or a step-change event justifies promotion.
- A curated transcript can justify a candidate hypothesis faster than it can justify a promoted active hypothesis.
- Only write back transcript-derived datapoints into daily notes if they are factual, material, missing from the daily notes, and clearly marked with provenance.

Transcript-processing review:
- For each transcript in `transcripts/new/`:
  - identify the source and date
  - extract the strongest non-obvious implications or hypothesis seeds
  - extract any material factual datapoints
  - classify each extracted item as datapoint, operator observation, interpretation, or speculation
  - decide whether it:
    - reinforces an active hypothesis
    - challenges an active hypothesis
    - supports a candidate hypothesis
    - suggests a missing hypothesis
    - merits a daily-notes writeback datapoint
  - if fully processed, move it to transcripts/archived/

Missing-hypothesis review:
- After reviewing the evidence, explicitly ask:
  - Is there a repeated pattern that is not well explained by the current active hypotheses?
  - Is there a new implication that matters for investing, business building, or product strategy that is underrepresented?
  - Is there a second-order effect that may matter more than the current first-order framing?
- If yes, surface it as a candidate hypothesis even if it is not yet ready for promotion.

At the end, provide a short changelog:
- whether the synthesis changed
- what was added, strengthened, challenged, promoted, merged, split, or left unchanged
- which candidate hypotheses were reviewed, added, or promoted
- why a candidate hypothesis was not promoted yet, if applicable
- which transcripts were processed
- whether any transcript-derived datapoints were written back into daily notes
- any notable uncertainty