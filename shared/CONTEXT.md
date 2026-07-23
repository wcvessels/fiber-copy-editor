# Shared

Routing for the shared folder: the cross-stage reference layer. This file contains no content of its own -- only the file inventory and the rules for using it. Which stage loads which file is declared in that stage's `CONTEXT.md` Inputs table, nowhere else.

## Files in This Folder

| File | Contents |
|---|---|
| `audience-model.md` | Four profiling dimensions, preset profiles (open list), jargon/altitude calibration, champion test |
| `fact-registry.md` | Company facts with value, source, as-of date, and verified/stale/disputed status -- the single home for every fact it tracks |
| `failure-modes.md` | Six recurring failure patterns with worked diagnostic notes |
| `format-presets.md` | Per-format pass scope and calibration, applied at intake |
| `concern-definitions.md` | HOC/LOC definitions, promotion rule, HOC cap -- canonical home |
| `feedback-voice.md` | Coaching persona, address register, tone dial, note types, note anatomy, trigger-aware phrasing |
| `sheet-format.md` | The review-sheet shape: skeleton, header fields, section contracts -- single home |
| `mechanics-standard.md` | Style authority hierarchy for LOC citations, legal escalation contact |

## Rules

- One-way references: stages read this folder; nothing here reads stage outputs.
- Two surfaces here change routinely: `fact-registry.md` rows (via the `facts` trigger, the writer owning every status change) and the Candidate Profiles block in `audience-model.md` (appended by 01-intake, promoted or deleted by the writer). If a fact has a registry row, no other file carries its value; reference the row instead of copying it.
- Everything else changes only at setup or by deliberate edit.
- Placeholders here are replaced once, during `setup`. No stage should see an unresolved `{{NAME}}` placeholder at runtime -- if one appears, treat it as a setup failure and route back to onboarding.
