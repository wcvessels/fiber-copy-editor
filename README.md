# Fiber Copy Editor

A diagnose-only editor for B2B fiber and telco marketing copy. Configured for {{BRAND_NAME}}.

> **Human-facing overview -- not an execution document.** No stage loads this file; the workspace runs from `CLAUDE.md` and the stage `CONTEXT.md` files. Skip it when walking the workspace as an agent.

Most fiber copy survives a paste test it should fail. Drop the headline onto a competitor's page and nothing breaks -- same carrier-grade reliability, same redundant routes, same four nines. This editor catches that before a buyer does.

It diagnoses. It never rewrites. It names the line, names the reader it fails, explains what that does to them, and hands the draft back with a question. You still do the writing.

## Try it

Runs in Claude Code, or any agent that can read and write to this folder.

Clone it, open it, and paste this:

```
setup -- I have a prepared fact sheet and voice document: fixtures/lightower-brief.md.
Use it to answer every setup question it covers. Only ask me for anything it does not answer.
```

That configures the editor for a demo brand assembled from public record. Then hand it a draft:

```
New piece for review: fixtures/product-page.md. Goal: generate qualified enterprise leads
for the optical encryption service. Audience: enterprise IT and security directors in
regulated verticals. Format: web product page. Tone dial: dry.
```

The review lands in `pieces/[slug]/r1-review.md`. `fixtures/` holds three drafts with defects planted in them, one prompt each, in `fixtures/README.md`.

## What comes back

This is a real note, from an actual run on `fixtures/product-page.md`. Run it yourself for the other nineteen.

> **Not a note:** "The intro could be stronger. Consider adding more specifics."

> **A note:** `L9 -- "End users maintain total control over the most important parts, their own security parameters and security keys."` [COACHING] -- curse-of-knowledge, internal lingo with two live readings. "End users" is telco shorthand for the customer organization. Outside the building it more often means the customer's employees. Both readings are available here, and they describe opposite security postures: the buying organization holding key material is the reassurance intended; staff holding key material is a finding in an audit. Key custody is the first question this reader asks about any encryption service, so the sentence answering it cannot support two answers. Which party holds the keys, and does the sentence name that party in a way a compliance reviewer could not misread?

Line anchor, named failure mode, coaching-or-evaluation tag, the reader and purpose it fails, and a question that hands the problem back. Every marginal note carries all five. The final pass audits for it: a sheet containing a replacement line fails, and so does a note that would read the same on somebody else's draft.

## How it runs

Eight stages. Intake builds the brief -- format, goal, audience profile, draft maturity, tone dial. Six diagnostic passes take the draft apart. Feedback triages what they found, and you curate it.

```
01-intake -> 02-audience-fit -> 03-claims -> 04-proof -> 05-differentiation
          -> 06-structure -> 07-cta -> 08-feedback
```

| Stage | Role |
| --- | --- |
| 01-intake | Build the brief: format, goal, audience profile, scope block, registry snapshot |
| 02-audience-fit | THE GATE -- right reader, right register, right funnel stage |
| 03-claims | Claim specificity: competitor paste test, unanchored adjectives |
| 04-proof | Evidence adjacent to claims; draft against the fact registry |
| 05-differentiation | Ownable vs. generic differentiators; cliche positioning |
| 06-structure | Stakes -> proof -> offer -> CTA ordering |
| 07-cta | CTA matched to audience temperature and decision role |
| 08-feedback | Triage into edit letter, marginal notes, and LOC batch; you curate |

Findings get tagged **HOC** -- strategic, the piece fails even with every sentence polished -- or **LOC**, sentence mechanics. Both are defined in `shared/concern-definitions.md`. They accumulate on the round's review sheet, which finishes as three things: an **edit letter** for pattern failures, capped so you get the few that matter instead of fifteen nitpicks; **marginal notes** for local ones; and a single **LOC batch**, kept separate so sentence noise never buries a structural problem. Nothing cut is hidden -- the full ledger stays on the sheet.

You touch it twice: confirming the brief at intake, and curating the sheet at the end. The passes in between run without stopping, each announcing its hand-off in a line or two.

Two things bend the line:

- **Skips.** The format preset (`shared/format-presets.md`) decides which passes run. A press release gets the strictest proof pass and no CTA pass. Skips are logged, never silent.
- **Developmental verdict.** When a piece needs a strategy pass instead of a copy pass, the sheet says so first and the edit letter leads with it. Triggers are in `stages/08-feedback/references/edit-letter-format.md`.

Every submission runs the full gauntlet. A revision is a new round, and intake carries the last round's findings forward so the passes judge what changed rather than re-litigating.

## Point it at your own brand

Type `setup`. One pass of questions -- footprint, verticals, compliance regimes, competitors, voice, and the facts the editor may treat as verified. It shows you the assembled identity, competitor set, and fact registry before writing anything to disk.

Answer it properly. Unconfigured slots ship as double-brace placeholder tokens, and intake checks for them before every run and stops if it finds one. An editor that guesses at your SLA is worse than no editor.

| Trigger | What it does |
| --- | --- |
| `setup` | Onboarding. Once per deployment. |
| `status` | Every piece in flight: current round, sheet open or finalized. |
| `facts` | Surfaces stale and disputed entries in the fact registry. Coverage maps and SLA terms rot, and a stale number in live copy is a credibility failure, not a typo. |

## How the folder is built

Folders are the architecture. Each does one job, and the split between them is load-bearing.

```
CLAUDE.md      entry point -- what the editor is, folder map, triggers
CONTEXT.md     task routing -- which stage handles what
setup/         onboarding questionnaire
brand-vault/   who the brand is: identity, voice, positioning, roles
shared/        the editorial method: audience model, concern definitions,
               sheet format, fact registry, format presets, feedback voice
stages/        the eight passes, one folder each: contract in CONTEXT.md,
               method in references/
pieces/        one folder per piece: the brief, plus a review sheet per round
fixtures/      demo brand and defect-seeded drafts
```

`shared/` is the method and survives every deployment. `brand-vault/` is instance data, replaced wholesale at setup. `pieces/` is the product. Swap the vault and the same editor works for a different provider.

Each stage's `CONTEXT.md` declares its own inputs, process, checkpoints, audit, and outputs, and a stage loads what that table names and nothing else. That is what keeps a pass reading like a pass instead of like the whole workspace at once.

## Bibliography

None of this was invented here. Every pass traces back to a book -- the first group is what the editor looks for, the second is how to say so without making an enemy of the writer.

**What good copy has to do**

- **Stratton, *Make It Punchy*.** V-B-F and the So What trace. The reason 03 will not let a claim stand until it names what the reader actually gets, and the audience-calibration standard behind 03 and 06.
- **Dunford, *Obviously Awesome*.** Positioning components, and the source of 05's total lack of patience with "the leading provider of." The book stops at positioning strategy; the procedure for tracing positioning down into a line of copy was built here.
- **Fenton & Kiefer Lee, *Nicely Said*.** Web-reading behavior and fact discipline. Behind 04, 06, and the format presets, including the rule that a page should point onward rather than explain everything at once.

**How to tell someone theirs doesn't**

- **Williams & Bizup, *Style: Lessons in Clarity and Grace*, 13th ed.**, with **Williams, Bizup & Colomb, *Style: The Basics of Clarity and Grace***. The vocabulary for naming what is wrong with a sentence without rewriting it, which is the whole trick the LOC batch runs on.
- **Norton, *Developmental Editing*, 2nd ed.** The edit letter, and the call between "this needs a copy pass" and "this needs a rethink." The developmental verdict comes straight from here.
- **Einsohn & Schwartz, *The Copyeditor's Handbook*, 4th ed.**, with **Buky, Schwartz & Einsohn, *The Copyeditor's Workbook***. Levels of edit and the craft of the query. Informs 01, 04, and 08.
- **Saller, *The Subversive Copy Editor*.** Editorial posture and query etiquette -- how to raise a problem without starting a fight. Shapes 08's voice.
- **Stone & Heen, *Thanks for the Feedback*, 2015 ed.** Why feedback bounces off, and the coaching-versus-evaluation split that every note in here is tagged with.
