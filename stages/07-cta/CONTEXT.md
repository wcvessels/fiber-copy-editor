# 07-cta

Diagnostic pass: judge the call-to-action against reader temperature and role.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Full | Running sheet: cumulative findings + HOC count + scope |
| Brief | `../../pieces/[piece-slug]/brief.md` | Full | Audience profile + calibration |
| Writer | draft file (per the brief's draft location) | Full | The copy under review |
| Stage | `references/checklist.md` | Full file | Pass questions -- temperature/role match, risk-reducing CTA standards |
| Shared | `../../shared/audience-model.md` | Full file | Temperature and decision-role dimensions |
| Shared | `../../shared/concern-definitions.md` | Full file | HOC/LOC definitions, promotion rule, cap |

## Process

1. If this pass is SKIPPED by scope, write a one-line "skipped by format" note to the sheet's Ledger and hand off.
2. Run the CTA checklist against the draft at the brief's calibration, matching CTA weight to reader temperature and decision role.
3. Tag findings HOC/LOC with line anchors; promote credibility-damaging LOCs; append to the sheet's Ledger.
4. Update the HOC count. If it passes the cap, set the sheet Verdict to `developmental`; continue.
5. Hand the sheet to 08-feedback, announcing the hand-off to the writer per Stage Handoffs in the root CLAUDE.md.

## Audit

| Check | Pass Condition |
|-------|---------------|
| Findings tagged | Every finding tagged HOC/LOC with a line anchor |
| Sheet updated | HOC count current; Verdict set to `developmental` if cap passed; skipped note written if scope-skipped |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Updated sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Findings appended, HOC count, Verdict |
