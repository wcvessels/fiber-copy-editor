# Judgment Calibration

Self-checks the editor runs against their own findings before the letter goes to the writer. Rules are the floor; beyond basic conventions, right/wrong decisions rarely exist -- the deliverable skill is choosing among defensible options and being able to defend the choice. Every finding is an argument, not a rule invocation.

## Judgment reasoning patterns

**Establish context before diagnosing anything.**
- Identify the audience (from the 01-intake profile: temperature, technical depth, decision role), the purpose, the format, and the register the piece has established. The same sentence warrants different treatment in different contexts.
- Identify the governing authority: the brand vault (`brand-vault/brand-voice.md`, `brand-vault/identity.md`) first, then `shared/fact-registry.md`, then field convention, then reader-intelligibility judgment recorded as a decision. Confirm what governs before ruling on anything.
- Identify the assigned pass depth (light / medium / heavy, set at intake). The brief sets what counts as a finding, not editor taste.

**Classify before you flag.** For every observation, decide which class it is:
1. **Error** -- violates a sourced rule (brand-vault, fact registry) or an internal inconsistency. Nondiscretionary.
2. **Style choice** -- a legitimate variant, governed by consistency, not correctness. A finding only when inconsistent or unrecorded.
3. **Preference** -- something the editor would have written differently. Not a finding. Silence.

**Simulate the reader, not the rulebook.**
- A grammatically fine sentence that forces the reader to reparse is still defective. Miscue trumps compliance.
- Calibrate to the least-informed plausible reader in the audience profile: domain gaps, unfamiliar jargon, abbreviations that never pay off. Whether a term needs a gloss is a per-term call, not a blanket rule.
- Judge structural devices (signposting, direct address, short paragraphs) by marketing-copy convention, not literary-prose aesthetics. What's inelegant in an essay is standard in a landing page.

**Match the register, don't correct it.** Infer intended register from the piece's consistent choices (contractions, direct address, informality) and treat them as evidence of intent, not error. Breezy is a strategy in B2B marketing copy, not a defect.

**Read for sense, always.** The highest-value catches are meaning-level: a wrong word that passes spellcheck, a tangled negative that says the opposite of what's meant, a verb whose logic contradicts the data next to it, a claim so generic it says nothing. Polish can mask wrong substance -- don't let clean styling wave through wrong numbers or contradicted claims.

**Weigh function before flagging a device.** Ask whether the marked element (emphasis, repetition, a seemingly redundant label) does communicative work the surrounding words don't already do. Cut only doubled devices doing one job.

**Respect cost.** Attention is a budget. Know the common issues cold; research only the genuinely hard calls; log what's learned into `shared/failure-modes.md` so it doesn't get re-derived next piece.

## Editor self-checks (named failure modes)

Run these against the draft findings list before it becomes the letter.

- **Over-flagging.** Flagging correct copy because it isn't how the editor would have written it. Self-check: was it wrong, or just not mine? A findings list thick with discretionary flags at a light pass is itself a defect. "No issues, verified" is a valid, complete deliverable for a clean passage.
- **Taste imposition (register trampling).** Pulling copy toward the editor's own formality, or proposing a fix that breaks the piece's established voice. Check every proposed direction against the register-match rule above.
- **False fixes (hypercorrection).** Proposing a change that would introduce an error: a comma "fix" that changes meaning, a "redundancy" the brand-vault explicitly permits for emphasis. Parse the construction fully before flagging it. Also verify the implausible before flagging it wrong -- some odd-looking names or figures are correct, and the confident correction is the actual error.
- **Missed context (attention tunneling).** Focusing on one error class hides adjacent ones; clean mechanics can mask wrong substance, and the errors easiest to miss are the ones nearest the editor's own comfort zone. Build a second pass at a different layer into every review.
- **Rule-worship (zombie-rule enforcement).** Imposing a superstition or retired rule as a correction -- banning sentence-initial conjunctions, terminal prepositions, deliberate fragments. If the only authority behind a finding is a peeve, there is no finding. Source every rule before enforcing it.
- **Content trespass.** Substituting the editor's interpretation for the writer's, or inferring a fact (a figure, an attribution) however probable. Diagnosis names the gap; the writer supplies the substance. If a proposed direction embeds a different message than the writer's, that's content, not expression -- refer it, don't flag it.
- **Scope creep.** Fixing everything the moment it's spotted, mixing HOC and LOC boundaries, chasing a trivial detail down a research hole. Noticing isn't license -- log it for the pass or round that owns it.
- **Cosmetic distancing.** Quotation marks or hedged phrasing don't neutralize a loaded word. If the word can't stand on its own, the finding is the word, not the punctuation around it.
- **Stale-template failure.** Reused phrasing or a finding template carrying a previous piece's product name or figure. Every reuse gets re-verified against this piece.
- **Calibrated humility.** Errors survive multiple competent passes, including this one. The stance toward every miss is diagnostic, never punitive -- toward the writer and toward the editor's own prior round. A missed catch is calibration data, not a verdict.

## When to leave things alone

- **Stet is an active decision**, not an absence of one. It requires the same reasoning as a flag.
- Before flagging anything that looks off, construct the reading under which it's intentional -- a deliberate register choice, a brand-voice quirk, an established fact-registry term. If that reading holds, record the reasoned leave-alone.
- **Deliberate effect is exempt.** Fragments, rhythm-driven punctuation, and rule-bending for emphasis are standard marketing technique. Determine intent before flagging; flag the accidental, respect the deliberate.
- **Zombie rules are never enforced,** regardless of how confidently they're remembered. Source the rule or drop the finding.
- **Consistency outranks conformity.** A consistently applied acceptable variant beats a "correct" form that creates visible inconsistency elsewhere in the piece.
- **When two authorities conflict** and neither is the brand-vault, the tie goes to the writer's existing choice -- record it and move on rather than litigating in the margins.
