# Review Sheet Format

Single home for the shape of `pieces/[piece-slug]/r[N]-review.md`. 01-intake opens the skeleton; 02-07 append Ledger rows; 08-feedback writes the writer-facing sections. Contracts point here -- do not restate the shape elsewhere.

## Skeleton (opened by 01-intake)

```
# Review Sheet -- [piece-slug] -- Round N
Date: [date]  |  HOC count: 0  |  Status: open

## Verdict
unset

## Edit Letter

## Prior Round

## Marginal Notes

## LOC Batch

## Ledger
| # | pass | anchor | HOC/LOC | failure mode | diagnosis + hand-back question |
|---|------|--------|---------|--------------|--------------------------------|
```

Prior Round appears on reruns only -- omit the section on round 1.

## Header fields

- **HOC count** -- running total; each appending pass updates it. Crossing the cap (`concern-definitions.md`) sets the Verdict to `developmental`; the gauntlet still runs in full.
- **Status** -- `open` while the round is in flight; 08 sets `finalized` when the writer accepts the sheet at the curate checkpoint.

## Section contracts

- **Verdict** -- `copy-level` (fundamentals hold) or `developmental` (needs a strategy pass, not a copy pass). Set by any pass that crosses the cap, or by a 02 hard-fail; finalized by 08. One home: this section, not the header.
- **Edit Letter** -- pattern-level HOCs, at most the cap, ranked by business impact, each audience-grounded. Structure: `stages/08-feedback/references/edit-letter-format.md`. Written by 08.
- **Prior Round** (reruns only) -- each prior-round finding and its status: fixed / still-open / regressed. Written by 08 from this round's Ledger judged against the brief's Prior Round section.
- **Marginal Notes** -- line-anchored notes for local failures, per the note anatomy in `feedback-voice.md`. Written by 08.
- **LOC Batch** -- one consolidated sentence-mechanics cleanup note, in sentence-diagnostics vocabulary. Written by 08.
- **Ledger** -- complete, append-only log of every finding from every pass, in run order. A format-skipped pass appends a one-line "skipped by format" note. 02-07 append; 08 appends its own sentence-level findings and triages all rows, but never edits or removes an upstream row. Nothing discarded.
