# 08-feedback

Triage the sheet, write the writer-facing sections, then present it to the writer for curate.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Full | The complete Ledger for this round |
| Brief | `../../pieces/[piece-slug]/brief.md` | Full | Audience grounding for every note |
| Shared | `../../shared/sheet-format.md` | Full file | Section contracts for the sheet it finalizes |
| Shared | `../../shared/concern-definitions.md` | Full file | HOC/LOC definitions, promotion rule, cap |
| Shared | `../../shared/fact-registry.md` | Full file | Verify doubted facts before querying the writer |
| Brand vault | `../../brand-vault/brand-voice.md` | Full file | Voice authority for evaluation notes and queries |
| Brand vault | `../../brand-vault/identity.md` | Full file | Declared positioning; authority grounding for evaluation |
| Writer | (conversation; named in `../../brand-vault/identity.md`, Roles) | Accept / edit / redirect | The human curate gate |
| Shared | `../../shared/feedback-voice.md` | Full file | Coaching persona, note anatomy, address register |
| Stage | `references/edit-letter-format.md` | Full file | Edit letter structure |
| Stage | `references/query-conventions.md` | Full file | How to phrase queries |
| Stage | `references/note-tags.md` | Full file | Coaching vs. evaluation tags |
| Stage | `references/sentence-diagnostics.md` | Full file | LOC batch vocabulary |
| Stage | `references/judgment-calibration.md` | Full file | Calibrating severity and tone |
| Shared | `../../shared/mechanics-standard.md` | Full file | Style authority hierarchy for LOC citations |

## Process

1. Triage the sheet's Ledger: rank HOCs by business impact; select at most the cap (`../../shared/concern-definitions.md`) for the Edit Letter.
2. If the Verdict is `developmental`: the Edit Letter leads with the developmental verdict; marginal notes limited to what survives a strategy change.
3. Write the Edit Letter section atop the sheet (pattern failures, audience-justified).
4. Write marginal notes for local failures: each names its failure mode (carried forward from the Ledger, or from `references/sentence-diagnostics.md` for LOCs -- not re-derived), tags coaching vs. evaluation, grounds in audience and purpose, ends with a question handing the problem back. Never a rewritten line.
5. On a rerun, write the sheet's Prior Round section: each prior finding and its status (fixed / still-open / regressed), judged from this round's Ledger against the brief's Prior Round section.
6. Write the LOC Batch section: one consolidated cleanup note using sentence-diagnostics vocabulary.
7. Finalize the Verdict: if no pass set it to `developmental`, set it to `copy-level`.
8. Run the stage audit (below); revise failures before presenting.
9. Present the finalized sheet to the writer: accept as the round's feedback, edit it directly, or send one pass back for rework. On a send-back, re-run the named pass and return here. On accept, set the header Status to `finalized`. [checkpoint] A curate loop, not a stamp.

## Checkpoints

| After Step | Agent Presents | Human Decides |
|------------|---------------|---------------|
| 9 | The finalized sheet: Verdict + Edit Letter (within cap) + marginal notes + LOC Batch + complete Ledger | Accept / edit directly / send one pass back for rework -- a curate loop, not a stamp |

## Audit

| Check | Pass Condition |
|-------|---------------|
| No rewrites | Zero corrected/replacement lines anywhere in the sheet |
| HOC cap | Edit Letter names <= cap issues |
| Audience grounding | Every note cites reader + purpose, never taste |
| Note anatomy | Every marginal note has: line anchor, failure-mode name, tag, why, hand-back question |
| Specificity | No note a writer could receive on a different draft unchanged |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Finalized review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Finalized per `../../shared/sheet-format.md` |
