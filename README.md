# Fiber Copy Editor

A marketing copy editor for B2B fiber/telco providers ({{BRAND_NAME}}).

> **Human-facing overview -- not an execution document.** No stage loads this file; the workspace runs from `CLAUDE.md` and the stage `CONTEXT.md` files. Skip it when walking the workspace as an agent.

## What This Workspace Does

The editor diagnoses. It never rewrites. It points at the specific lines that fail, names the audience and purpose they fail for, explains why, and hands the draft back. A corrected line never appears in feedback -- generic notes ("tighten this intro") are a fail.

A submitted draft moves through eight stages: an intake brief captures format, goal, and audience profile; six diagnostic passes (audience-fit, claims, proof, differentiation, structure, CTA) tag findings as HOC (higher-order concern -- strategic failures) or LOC (lower-order concern -- sentence mechanics; definitions in `shared/concern-definitions.md`) on the round's review sheet; a feedback stage triages the sheet into edit letter, marginal notes, and LOC batch, and the writer curates it (the writer is named in `brand-vault/identity.md`, Roles).

The feedback package that reaches the writer has three parts:

- **Edit letter** -- pattern-level failures, capped at the HOC cap set in `shared/concern-definitions.md` so the writer isn't drowned in fifteen nitpicks.
- **Marginal notes** -- line-anchored diagnoses for local failures, each naming its failure mode, tagging coaching vs. evaluation, grounding in audience and purpose, and ending with a question that hands the problem back.
- **LOC batch** -- one consolidated cleanup note for sentence-level mechanics, using shared diagnostic vocabulary rather than corrected lines.

Two things bend the straight line through the stages:

- **Skips:** the format preset applied at intake (format list: `shared/format-presets.md`) sets which of the audience-fit-through-CTA passes run, and at what calibration, for that piece. A skipped pass writes a one-line "skipped by format" note to the sheet's Ledger, so the record stays complete.
- **Developmental verdict:** if a pass's findings push the HOC count past the cap, or the audience-fit pass hard-fails, the pass sets the sheet Verdict to `developmental` ("this needs a strategy pass, not a copy pass"). The gauntlet still runs in full; the verdict leads the edit letter so the writer sees "stop, rethink" first. The writer curates the result at 08.

Every submission runs the full gauntlet. A revision is a new round: intake opens the next review sheet, carrying the prior round's findings and their status forward into the brief so the passes judge progress rather than re-litigate.

## How a Writer Uses It

1. Submit a draft (any format) with its goal and intended audience, or hand over a complete brief if one already exists.
2. The workspace assembles a brief, profiles the audience, and confirms it back before the diagnostic passes run.
3. The draft runs the full gauntlet of in-scope diagnostic passes uninterrupted -- human judgment enters at intake and at curate, not at every finding.
4. At 08 the finalized review sheet is presented for curate: accept it, edit it directly, or send one pass back for rework.
5. Read the edit letter, marginal notes, and LOC batch, revise, and resubmit. The revision runs as a new round; intake carries the prior round's findings forward so the passes judge what changed.

## Pipeline at a Glance

```
01-intake -> 02-audience-fit -> 03-claims -> 04-proof -> 05-differentiation
          -> 06-structure -> 07-cta -> 08-feedback
```

| Stage              | Role                                                                                     |
| ------------------ | ---------------------------------------------------------------------------------------- |
| 01-intake          | Assemble the piece brief: format, goal, audience profile, scope block, registry snapshot |
| 02-audience-fit    | THE GATE -- right reader, right register, right funnel stage                             |
| 03-claims          | Claim specificity: competitor paste test, unanchored adjectives                          |
| 04-proof           | Evidence adjacent to claims; draft-vs-registry consistency                               |
| 05-differentiation | Ownable vs. generic differentiators; cliche positioning                                  |
| 06-structure       | Stakes -> proof -> offer -> CTA ordering                                                 |
| 07-cta             | CTA matched to audience temperature and decision role                                    |
| 08-feedback        | Triage the sheet into the edit letter, marginal notes, and LOC batch; the writer curates   |

## Bibliography

This workspace was built using learnings from the following source books. Reference docs elsewhere carry the operational method these books informed. This wouldn't be complete or effective without them. All are worth reading to better understand the frameworks governing this workspace.

- **Stratton, *Make It Punchy*.** V-B-F diagnostic method and the So What trace; informs the shared audience model and the claims (03) and structure (06) passes' audience-calibration standard.
- **Dunford, *Obviously Awesome*.** Positioning components; informs the differentiation (05) pass. The positioning-to-copy traceability procedure used in this workspace is an adaptation built for this pipeline -- the book itself stops at positioning strategy, not copy diagnosis.
- **Williams & Bizup, *Style: Lessons in Clarity and Grace*, 13th ed.**, and **Williams, Bizup & Colomb, *Style: The Basics of Clarity and Grace***. Sentence-diagnosis vocabulary; informs the line-level (LOC) reference material.
- **Norton, *Developmental Editing*, 2nd ed.** Edit letter method and the developmental-vs-copy triage judgment; informs the feedback (08) pass and the developmental-verdict language.
- **Einsohn & Schwartz, *The Copyeditor's Handbook*, 4th ed.**, and **Buky, Schwartz & Einsohn, *The Copyeditor's Workbook***. Levels of edit, query craft, and judgment patterns; inform intake (01), proof (04), and feedback (08).
- **Saller, *The Subversive Copy Editor*.** Editorial posture and query etiquette; informs the feedback (08) voice.
- **Stone & Heen, *Thanks for the Feedback*, 2015 ed.** Coaching vs. evaluation note-typing and trigger-aware phrasing; informs the feedback (08) pass.
- **Fenton & Kiefer Lee, *Nicely Said*.** Web copy diagnostics and fact discipline; inform the proof (04) and structure (06) passes and the format presets.
