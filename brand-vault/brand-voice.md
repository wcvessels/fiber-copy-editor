# Brand Voice

<!-- Setup strata (see setup/questionnaire.md, Q27-Q30):
     SETUP-OWNED sections -- content is replaced from onboarding answers; shipped content is
     the B2B-fiber category default kept when the user skips: "Core Voice", "Start Here
     (Every Time)", "Messaging Pillars", "Words to Use", "Words to Avoid", "Go-To Messaging
     Patterns".
     METHOD-INVARIANT sections -- setup fills placeholders and applies the documented
     conditionals but never restructures: "VBF Ordering", "Final Check", "Brand-vs-Research
     Contradictions".
     Section names are the interface: stages load sections by name (see stage CONTEXT.md
     Inputs tables). Never rename, remove, or reorder sections. When replacing Core Voice,
     preserve the register-default line that defers to the audience model. -->

## Core Voice

Plainspoken. Confident. Real.

- We sound like a partner, not a vendor.
- We speak clearly, not technically. **Default register only** -- see Brand-vs-Research Contradictions below. The audience model overrides this for specialist and committee-signer audiences.
- We focus on outcomes, not features.

## Start Here (Every Time)

Lead with what the reader is dealing with:

- Too many vendors
- Constant issues
- Security concerns
- Pressure to do more with less

## Messaging Pillars

Anchor every piece in at least one:

- **Reliability** -- uptime, consistency
- **Simplicity** -- less to manage, fewer vendors
- **Ownership** -- one call, no runaround
- **Support** -- real people, fast response

## VBF Ordering

Value, then Benefits, then Features -- in that order, every time.

- **Value** -- what changes for the reader
- **Benefits** -- how it helps
- **Features** -- what it is

Leading with value and benefits gives the reader a reason to keep reading before they hit the mechanism. Leading with features loses skimmers before the value ever lands.

## Words to Use

Accountable, proven track record, there when you need us, one call, no runaround, responsive support.

## Words to Avoid

Optimize, transform, best-in-class, leverage, synergy, cutting-edge.

If it sounds like every other provider, don't use it.

## Go-To Messaging Patterns

- **With vs. Without** -- without {{BRAND_NAME}}, chaos; with {{BRAND_NAME}}, clarity.
- **Reduce the Burden** -- "you've got enough on your plate"; "we take that off your team"; "no heavy lifting or additional tools for your team to learn."
- **Ownership** -- "we own it"; {{CONSOLIDATION_TAGLINE}} -- see contradiction 1 below before using this line unsupported.

## Final Check

Before sending copy forward, ask:

- Would a busy reader in this audience believe this?
- Does this make their life feel easier?
- Does it sound like every other provider?
- Is it filled with corporate jargon?

If not, send it back.

## Brand-vs-Research Contradictions

The workspace carries these as a named tension rather than resolving them silently. The editor holds both truths at once.

**1. Consolidation tagline needs adjacent proof.** {{CONSOLIDATION_TAGLINE}} is a mandated go-to pattern, but it is also an industry-wide cliche that fails the competitor-paste test (see `shared/failure-modes.md`, Vendor-Consolidation Cliche) and fails this file's own Final Check ("does it sound like every other provider?"). Editor treatment: never strike the phrase, it is brand-mandated. Flag it whenever it appears without adjacent proof (an owned asset, a specific number, a named process) backing it up.

**2. "We speak clearly, not technically" is the default, not a universal rule.** This file states it as a blanket rule; the audience model shows dense technical vocabulary is mandatory for specialist and carrier/wholesale readers, and simplifying it there destroys credibility. Precedence: `shared/audience-model.md` overrides this file for specialist audiences. This file's register is the default for IT-leader and budget-holder audiences only.

**3. The NPS claim carries conflicting sources.** Copy regularly cites an NPS comparison figure. The fact registry (`shared/fact-registry.md`) is the single home for that figure and its status -- different public sources have stated different percentages. Never treat an NPS figure in draft copy as verified; check the registry row's current status before a piece ships with the claim.

**4. VBF alignment.** This file's Value-Benefits-Features ordering matches the workspace's V-B-F diagnostic method used in 03-claims and 06-structure. Brand voice and editorial method agree on this hierarchy -- no tension here, just confirmation that the two systems reinforce each other.
