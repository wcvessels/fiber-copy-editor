# 03-claims

Diagnostic pass: judge claim strategy against the V-B-F method.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Full | Running sheet: cumulative findings + HOC count + scope |
| Brief | `../../pieces/[piece-slug]/brief.md` | Full | Audience profile + calibration |
| Writer | draft file (per the brief's draft location) | Full | The copy under review |
| Stage | `references/checklist.md` | Full file | Pass questions |
| Stage | `references/vbf-method.md` | Full file | V-B-F diagnostic method, competitor paste test |
| Brand vault | `../../brand-vault/identity.md` | Differentiators | What the company can actually claim |
| Shared | `../../shared/fact-registry.md` | Competitive set row | Names for the competitor-paste test |
| Shared | `../../shared/failure-modes.md` | Full file | Worked failure examples |
| Shared | `../../shared/concern-definitions.md` | Full file | HOC/LOC definitions, promotion rule, cap |

## Process

1. If this pass is SKIPPED by scope (per the brief's scope block), write a one-line "skipped by format" note to the sheet's Ledger and hand off.
2. Run the claims checklist against the draft at the brief's calibration, applying the V-B-F method and competitor paste test.
3. Tag findings HOC/LOC with line anchors; promote credibility-damaging LOCs; append to the sheet's Ledger.
4. Update the HOC count. If it passes the cap, set the sheet Verdict to `developmental`; continue.
5. Hand the sheet to 04-proof, announcing the hand-off to the writer per Stage Handoffs in the root CLAUDE.md.

## Audit

| Check | Pass Condition |
|-------|---------------|
| Findings tagged | Every finding tagged HOC/LOC with a line anchor |
| Sheet updated | HOC count current; Verdict set to `developmental` if cap passed; skipped note written if scope-skipped |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Updated sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Findings appended, HOC count, Verdict |
