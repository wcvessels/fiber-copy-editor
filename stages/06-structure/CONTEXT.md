# 06-structure

Diagnostic pass: judge ordering -- stakes, proof, offer, CTA, and V-B-F sequencing.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Full | Running sheet: cumulative findings + HOC count + scope |
| Brief | `../../pieces/[piece-slug]/brief.md` | Full | Audience profile + calibration |
| Writer | draft file (per the brief's draft location) | Full | The copy under review |
| Stage | `references/checklist.md` | Full file | Pass questions |
| Stage | `references/structure-guide.md` | Full file | Stakes->proof->offer->CTA ordering, story-structure diagnostics |
| Stage (cross-ref) | `../03-claims/references/vbf-method.md` | Full file | V-B-F ordering standard (one-way reference) |
| Shared | `../../shared/concern-definitions.md` | Full file | HOC/LOC definitions, promotion rule, cap |

## Process

1. If this pass is SKIPPED by scope, write a one-line "skipped by format" note to the sheet's Ledger and hand off.
2. Run the structure checklist against the draft at the brief's calibration, checking ordering against the structure guide and V-B-F sequencing.
3. Tag findings HOC/LOC with line anchors; promote credibility-damaging LOCs; append to the sheet's Ledger.
4. Update the HOC count. If it passes the cap, set the sheet Verdict to `developmental`; continue.
5. Hand the sheet to 07-cta, announcing the hand-off to the writer per Stage Handoffs in the root CLAUDE.md.

## Audit

| Check | Pass Condition |
|-------|---------------|
| Findings tagged | Every finding tagged HOC/LOC with a line anchor |
| Sheet updated | HOC count current; Verdict set to `developmental` if cap passed; skipped note written if scope-skipped |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Updated sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Findings appended, HOC count, Verdict |
