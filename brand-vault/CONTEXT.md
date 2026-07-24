# Brand Vault

Routing for the brand-vault folder. This file contains no content of its own -- only the file inventory and the rules for using it.

## Files in This Folder

| File | Contents |
|---|---|
| `brand-voice.md` | Core voice, messaging pillars, VBF ordering, words to use/avoid, go-to patterns, final check, brand-vs-research contradictions |
| `identity.md` | Brand name, legal entity, domain, footprint, network model, verticals + compliance, differentiators, competitive set, tagline, roles (writer) |

## Consumers

Which stage loads which file and section is declared in that stage's `CONTEXT.md` Inputs table -- that table is the single home for load specs. This folder keeps no consumer list of its own.

## Rules

- One-way references only: this folder is read by stages, and reads nothing itself.
- Placeholders in these files are replaced once, during `setup`. No stage should see an unresolved double-brace placeholder at runtime -- if one appears, treat it as a setup failure and route back to onboarding.
- Contradictions in `brand-voice.md` are not resolved here. They are carried forward as documented tension for 02 and 05 to apply, per the precedence stated in that file.
- `brand-voice.md` sections are a fixed schema: stages load sections by name. Setup replaces content within the setup-owned sections (see the strata note at the top of that file); section names never change.
