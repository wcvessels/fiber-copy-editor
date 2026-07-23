# 02-audience-fit

The gate: diagnose whether the draft fits its reader before any other pass runs.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Brief | `../../pieces/[piece-slug]/brief.md` | Full | Scope, audience profile, draft location |
| Writer | draft file (per the brief's draft location) | Full | The copy under review |
| Review sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Full | The running sheet for this round |
| Shared | `../../shared/audience-model.md` | Full file | The judgment standard: jargon, altitude, champion/signer, single-reader |
| Brand vault | `../../brand-vault/brand-voice.md` | Core Voice + Brand-vs-Research Contradictions sections | Brand default vs. audience override |
| Stage | `references/checklist.md` | Full file | Pass questions |
| Shared | `../../shared/concern-definitions.md` | Full file | HOC/LOC definitions, promotion rule, cap |

## Process

1. Read the draft against the brief's audience profile.
2. Run the audience-fit checklist: right reader, right register, right funnel stage, jargon matched to depth, stakes before proof for cold/nontechnical readers.
3. Tag findings HOC/LOC with line anchors; append to the sheet's Ledger; update the HOC count.
4. If the gate hard-fails (wrong reader or wrong register throughout) or the HOC count passes the cap, set the sheet Verdict to `developmental`. Continue either way -- the gauntlet always runs; the writer curates at 08.
5. Hand the sheet to 03-claims, announcing the hand-off to the writer per Stage Handoffs in the root CLAUDE.md.

## Audit

| Check | Pass Condition |
|-------|---------------|
| Findings tagged | Every finding tagged HOC/LOC with a line anchor |
| Sheet updated | HOC count current; Verdict set to `developmental` if the gate hard-failed or the cap was passed |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Updated sheet | `../../pieces/[piece-slug]/r[N]-review.md` | Findings appended, HOC count, Verdict |
