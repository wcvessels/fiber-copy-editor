# Format Presets

One pipeline; presets toggle which of passes 02-07 run and at what calibration. A new copy type is a new row in the table below, never a new stage folder.

## Preset Table

| Format | 02 audience-fit | 03 claims | 04 proof | 05 differentiation | 06 structure | 07 cta |
|---|---|---|---|---|---|---|
| Product / vertical page | full | full | full | full | full | full |
| Cold display / social ad | full | full | light | full | skip | full |
| Email | full + subject line | full | full | full | full | full + subject line |
| Blog / thought leadership | full | full | full | light | full | soft-cta |
| Press release | full | full | strictest | light | full | skip |
| Analyst briefing | full | full | strictest | full | full | skip |

**Calibration labels:**

- **full** -- run the pass's complete checklist at standard depth.
- **light** -- run the pass but hold findings to a higher bar; only flag issues that would meaningfully hurt the piece's specific job.
- **skip** -- pass writes a one-line "skipped by format" note to the sheet's Ledger; no findings are generated.
- **strictest** -- run the pass at maximum scrutiny; even minor issues get flagged. Reserved for formats where a single error is disproportionately costly.
- **full + subject line** -- the standard checklist, plus the subject line is treated as its own audience-fit and cta surface.
- **soft-cta** -- 07 runs, but findings are judged against a lower-pressure conversion ask (e.g., "read more," "subscribe") rather than a hard sales cta.

## Per-Format Notes

**Product / vertical page.** The default, highest-scrutiny format -- it is usually the piece a champion forwards to a signer. Every pass runs full. The audience profile should almost always include both champion and signer.

**Cold display / social ad.** No signer exists yet at this temperature; audience-fit judges register and stakes-before-proof, not decision-role fit. 04-proof runs light because ad copy rarely carries enough claims to need deep fact-checking; 05-differentiation stays full because a generic ad is wasted spend. 06-structure is skipped -- there is no room for stakes-proof-offer sequencing in ad-length copy.

**Email.** Full scrutiny across the board, plus the subject line gets its own audience-fit and cta check -- a subject line that misreads the audience kills the piece before the body copy matters.

**Blog / thought leadership.** 05-differentiation runs light: thought leadership earns trust through insight, not through hammering competitive differentiation. 07-cta is soft -- the ask is attention and credibility, not a signed deal.

**Press release.** 04-proof runs at strictest calibration -- press releases are quoted, archived, and cited by trade press, so a factual error propagates furthest and is hardest to walk back. 07-cta is skipped; a press release does not carry a conversion ask.

**Analyst briefing.** Reader is the Industry analyst preset (`audience-model.md`, this folder). 04-proof runs strictest -- analyst reports cite and archive claims, so every figure needs a checkable source. Mechanism-first ordering is expected here as with spec pages, so 06 judges coherence rather than the stakes-first arc. 07 is skipped -- no conversion ask.
