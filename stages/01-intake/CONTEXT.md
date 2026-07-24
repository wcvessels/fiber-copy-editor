# 01-intake

Assemble the piece brief and open the round's review sheet before the diagnostic gauntlet runs.

## Inputs

| Source | File/Location | Section/Scope | Why |
|--------|--------------|---------------|-----|
| Writer | draft file (any format) | Full | The copy under review |
| Writer | (conversation) | Goal, audience, format if not supplied in a brief | Brief ingredients |
| Prior round (reruns only) | `../../pieces/[piece-slug]/r[N-1]-review.md` | Full | Distil last round's findings + status into the brief |
| Shared | `../../shared/audience-model.md` | Dimensions + presets | Profile the audience |
| Shared | `../../shared/format-presets.md` | Full file | Set pass scope + calibration |
| Shared | `../../shared/sheet-format.md` | Full file | Sheet skeleton spec |
| Shared | `../../shared/fact-registry.md` | Full file | Attach registry snapshot reference to brief |
| Brand vault | `../../brand-vault/identity.md` | Footprint, verticals + compliance | Build the audience profile; confirm which compliance regime applies |
| Shared | `../../shared/feedback-voice.md` | Tone Dial section | Record the piece's dial in the brief |
| Stage | `references/calibration-guide.md` | Full file | Draft-maturity calibration |

## Process

1. Pre-flight -- setup gate: scan the workspace (every folder except `setup/`, which documents the placeholders) for any unresolved double-brace placeholder. Any hit means setup is incomplete: stop -- no intake, no brief -- and route to `setup/questionnaire.md`, per the placeholder rule in `../../brand-vault/CONTEXT.md` (Rules). The editor never invents or defaults a missing specific.
2. Identify the piece: format, goal, funnel position, and draft maturity (first pass / near-final / release candidate -- see `references/calibration-guide.md`). First-pass drafts get strategy-level scrutiny only; sentence-level diagnostics are held for later rounds.
3. Profile the audience on the model's dimensions (temperature, technical depth, decision role, risk lens); start from a preset when one fits. When none fits, append the writer-defined profile as a candidate line in `../../shared/audience-model.md` (Candidate Profiles); if it matches an existing candidate line, append the slug there and flag the recurrence at the step-6 checkpoint. For committee purchases, identify both the champion (register target) and the signer (whose risk lens sets required proof).
4. Apply the format preset; record the scope block: which of 02-07 run, at what calibration, with intake-judgment overrides noted. Record the Tone dial: the deployment default from the Tone Dial section of `../../shared/feedback-voice.md` unless the writer overrides it for this piece; write the setting plus its one-line gloss into the brief.
5. On a rerun (a prior-round sheet exists in the piece folder), read it and write a Prior Round section for the brief: each prior finding and its status (fixed / still-open / regressed). The gauntlet re-runs in full regardless -- this is context, not a routing decision.
6. Confirm the brief with the writer in one pass (skip if a complete brief was supplied). [checkpoint]
7. Write the brief and open the round's review sheet per `../../shared/sheet-format.md` -- round number N = (existing `r*-review.md` in the piece folder) + 1. New piece: derive `[piece-slug]` kebab-case from the confirmed brief title (it rides in the step-6 confirm) and create `../../pieces/[piece-slug]/`; reruns reuse the existing folder.
8. Hand the brief and sheet to 02-audience-fit, announcing the hand-off to the writer per Stage Handoffs in the root CLAUDE.md.

## Checkpoints

| After Step | Agent Presents | Human Decides |
|------------|---------------|---------------|
| 6 | The assembled brief (incl. the Prior Round section on reruns) | Confirm or correct before the gauntlet runs |

## Audit

| Check | Pass Condition |
|-------|---------------|
| Setup gate | No unresolved double-brace placeholder anywhere outside `setup/` at intake time |
| Brief complete | Format, goal, audience profile (incl. champion + signer for committee buys), draft maturity, scope block, Tone dial, and registry reference all present |
| Rerun context | On a rerun, the brief's Prior Round section names each prior finding and its status |

## Outputs

| Artifact | Location | Format |
|----------|----------|--------|
| Piece brief | `../../pieces/[piece-slug]/brief.md` | Format, goal, audience profile, scope block, Tone dial (setting + gloss), registry reference, draft location, Prior Round (reruns) |
| Review sheet (round N, open) | `../../pieces/[piece-slug]/r[N]-review.md` | Skeleton per `../../shared/sheet-format.md` |
| Candidate profile (when no preset fits) | `../../shared/audience-model.md`, Candidate Profiles | One line: name \| four dials \| piece slug |
