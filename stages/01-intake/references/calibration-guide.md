# Calibration Guide

The editor diagnoses. It never rewrites. Every finding in every downstream stage is a flag (actionable without discussion) or a query (a question only the writer can answer) -- never a replacement sentence. This guide sets the dial before any diagnostic pass begins.

## Levels of Edit as Calibration Settings

Edit depth is a setting chosen up front, not an emergent property of how much the editor notices. Three settings, each nesting the one before it:

- **Light** -- Does this page contain spelling errors, grammar failures that mislead (agreement breaks, danglers), undefined acronyms, internal factual contradictions, or claim-to-evidence mismatches (headline vs. body, CTA vs. destination)? Does anything here require legal or permissions review? Ignore diction, rhythm, and mechanical variation that does not block comprehension.
- **Medium** -- Everything in light, plus: is any sentence ambiguous, garden-path, or misattached? Is there a wordiness or redundancy cluster? Does a passive construction serve no purpose? Is terminology drifting across the page? Does tone wobble against the intended register?
- **Heavy** -- Everything in medium, plus: is the organization and ordering right? Is emphasis proportional to importance? Does the page fit its audience? Does the argument hold together logically? Heavy still means findings with proposed remedies, never rewritten prose.

Set the level deliberately per engagement. Inputs to the decision: draft maturity, audience and visibility of the page, brand stakes, schedule, and how much the writer can absorb. Default to the lightest setting that meets the brief; escalate only with explicit authorization.

## Draft-Maturity Rule

**Named failure: scrutiny mismatch.** Applying finished-copy standards to a first-pass draft is a calibration failure, not a thoroughness win.

- Is this draft a first pass? If so, does the review confine itself to strategy-level findings only -- wrong reader, wrong claim architecture, missing differentiator, missing stakes? Sentence-level diagnosis on a first pass is premature; conciseness and punch are produced by revision, not caught early.
- Is this draft near-final? If so, does the review add the full line-level pass -- jargon, throat-clearing, bloat, flat pacing?
- Is this a release candidate? If so, does the review narrow to a proof-level sweep for errors introduced in the last round, rather than reopening structural questions already settled?

Ask which maturity stage the draft is in before opening the checklist stages. A structural finding on a release candidate, or a comma finding on a first draft, is itself a miscalibration -- flag the mismatch, not just the prose.

## Editorial Triage

When time or attention is constrained, triage is a deliberate scoping act, not silent corner-cutting.

- Has the writer set priorities, or is the editor guessing at what matters most?
- Under pressure, does coverage win over depth -- spelling, serious grammar, factual inconsistency, undefined jargon, and anything needing legal review, checked everywhere, before anything else gets a second look?
- Are the highest-visibility surfaces (headline, subhead, CTA, first screen, navigation labels, prices, dates) read with maximum care regardless of remaining time?
- For B2B marketing copy specifically: does substance outrank mechanics? Audience mismatch, unproven claims, and generic differentiation should sit above comma splices and capitalization drift on any priority list.
- Is any one finding being asked to carry more weight than fifteen line-level nitpicks combined? The audience-fit, proof-weakness, and differentiation findings usually matter more than the accumulated small stuff -- rank accordingly.

## Building the Scope Block

Before running the downstream stage checklists, derive a scope block from two inputs: the format preset and the audience profile. Answer these to build it:

**Format preset.** Match the piece to a row in `shared/format-presets.md` -- that table is the single home for the format list and for which passes run at what calibration. Record the chosen row before reviewing. (Note: the preset table's per-pass calibration labels are a separate dial from the light / medium / heavy edit level above.)

**Audience profile.** Profile the reader on the four dimensions in `shared/audience-model.md`, starting from one of its presets when one fits -- that file is the single home for the dimensions, presets, and jargon/altitude rules. A reader targeted with the wrong register entirely (consumer register on B2B copy, or vice versa) is itself a finding -- flag the mismatch at intake rather than calibrating around it.

**Derived settings.** From format preset plus audience profile, fix before drafting review begins:
- Edit level (light / medium / heavy) per the draft-maturity rule above.
- Jargon tolerance: is domain vocabulary a trust signal for this reader (carrier/wholesale, technical evaluator) or an exclusion risk (budget holder, mixed committee, consumer-adjacent)?
- Tone register: does the stakes level of this page (regulated vertical, public-sector, high-consideration infrastructure purchase) rule out playful or joking language, or is levity tolerable here?
- Which downstream checklist stages apply at full weight, and which are lighter-touch for this particular asset (e.g., a pure technical spec sheet for a carrier buyer may not need a differentiation pass at all if it carries no positioning claims).

Record the scope block once per intake and hand it forward -- every downstream stage checklist should be run against this scope, not re-derived from scratch.
