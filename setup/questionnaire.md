# Onboarding Questionnaire

<!-- Agent instructions: Read this file when the user types "setup". Ask ALL questions
     in a single conversational pass. The user should be able to answer everything in one
     message. Collect the answers, then follow the After Onboarding procedure at the end
     of this file.

     Reserved syntax: double curly braces mark a placeholder, nothing else. Elsewhere, name
     placeholders in words -- never a brace-token -- so any double-brace token left outside
     `setup/` is always a live one for the run-gate to catch.

     REQUIRED questions (marked "Required: yes" below) have no default and no skip
     path -- setup is not complete while any of them lacks an explicit answer ("none"
     counts only where the question documents a none path). Never invent, genericize,
     or default a required specific.

     Fact-sheet shortcut: Q13 lets the user point to a prepared fact sheet instead of
     answering Q14-Q22 one at a time. If they do, extract each fact's value, source, and
     as-of date from that document. Any fact the sheet doesn't cover, ask for individually
     using the corresponding question below. Every registry row keeps its "stale" status
     regardless of source -- onboarding fills the registry, it does not verify it.

     Voice-document shortcut: Q27 works the same way for brand voice -- a supplied voice
     document replaces Q28-Q30 for whatever it covers, mapped into brand-voice.md's
     setup-owned sections per the strata note at the top of that file. Anything not
     covered keeps the shipped category default. -->

### Q1: What's the brand name?
- Placeholder: `{{BRAND_NAME}}`
- Files: `brand-vault/identity.md`, `brand-vault/brand-voice.md`, `shared/failure-modes.md`, `README.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q2: What's the legal entity name (the one that goes on contracts, not the marketing name)?
- Placeholder: `{{LEGAL_ENTITY}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Default: [same as brand name if no separate legal entity]

### Q3: What's the company's domain?
- Placeholder: `{{DOMAIN}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q4: What's the company's tagline?
- Placeholder: `{{TAGLINE}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Default: [leave blank if none -- write "no standing tagline"]

### Q5: What states or regions does the network serve?
- Placeholder: `{{FOOTPRINT_STATES}}`
- Files: `shared/fact-registry.md` (single home; `brand-vault/identity.md` points to the registry row)
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q6: Is the network owned, leased, or a mix? Describe the ownership model in one or two sentences -- this determines which reliability and control claims the editor lets through.
- Placeholder: `{{NETWORK_OWNERSHIP_MODEL}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q7: What verticals do you sell into, and what compliance regime applies to each? List up to four (vertical: regime).
- Placeholder: `{{VERTICAL_1}}`, `{{VERTICAL_1_COMPLIANCE}}`, `{{VERTICAL_2}}`, `{{VERTICAL_2_COMPLIANCE}}`, `{{VERTICAL_3}}`, `{{VERTICAL_3_COMPLIANCE}}`, `{{VERTICAL_4}}`, `{{VERTICAL_4_COMPLIANCE}}`
- Files: `brand-vault/identity.md`
- Type: free text (list)
- Required: yes -- at least one vertical: regime pair
- Default: none -- REQUIRED, must come from setup

### Q8: What makes your local support or NOC model different from a call center? (in-region technicians, response-time commitment, escalation path)
- Placeholder: `{{LOCAL_SUPPORT_MODEL}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q9: What's the specific, provable claim about your regional network density? (not "extensive network" -- an actual number or comparison)
- Placeholder: `{{REGIONAL_DENSITY_DESCRIPTION}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q10: When a customer consolidates onto your network, what vendors, contracts, or failure points actually disappear for them?
- Placeholder: `{{CONSOLIDATION_REMOVES}}`
- Files: `brand-vault/identity.md`
- Type: free text
- Required: yes -- setup cannot complete without an explicit answer
- Default: none -- REQUIRED, must come from setup

### Q11: Who are your top 1-3 direct competitors (the names copy gets checked against for the competitor paste test)?
- Placeholder: `{{COMPETITOR_1}}`, `{{COMPETITOR_2}}`, `{{COMPETITOR_3}}`
- Files: `shared/fact-registry.md` (single home -- the Competitive set row; `brand-vault/identity.md` points to it), `shared/failure-modes.md` (worked-example prose only)
- Type: free text (list)
- Required: yes -- at least one name (the editor works with as few as one; zero is a setup failure)
- Default: none -- REQUIRED, must come from setup
- Derived: `{{SETUP_DATE}}` -- the date setup runs, stamped by the agent as the Competitive set row's as-of date. Not asked.

### Q12: Do you have a standing "one-provider" or consolidation tagline you want the editor to recognize as brand-mandated? Give the exact wording.
- Placeholder: `{{CONSOLIDATION_TAGLINE}}`
- Files: `brand-vault/brand-voice.md`
- Type: free text
- Required: yes -- exact wording, or an explicit "none" (the After Onboarding no-tagline conditional applies)
- Default: none -- REQUIRED, must come from setup

### Q13: Do you have a prepared fact sheet (a document listing network stats with their sources and as-of dates)? If yes, share it or paste its contents and skip Q14-Q22 for anything it covers -- the agent will pull value, source, and as-of date for each fact from it. If no, answer Q14-Q22 individually.
- Type: free text or file reference
- Default: no fact sheet -- answer Q14-Q22 individually

### Q14: Route miles -- what's the figure, where does it come from, and as of when?
- Placeholder: `{{ROUTE_MILES}}`, `{{ROUTE_MILES_SOURCE}}`, `{{ROUTE_MILES_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q15: Lit / on-net locations -- what's the figure, where does it come from, and as of when?
- Placeholder: `{{LIT_ON_NET_LOCATIONS}}`, `{{LIT_ON_NET_SOURCE}}`, `{{LIT_ON_NET_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q16: Serviceable locations -- what's the figure, where does it come from, and as of when?
- Placeholder: `{{SERVICEABLE_LOCATIONS}}`, `{{SERVICEABLE_LOCATIONS_SOURCE}}`, `{{SERVICEABLE_LOCATIONS_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q17: Data centers and their certifications -- what's the list, where does it come from, and as of when?
- Placeholder: `{{DATA_CENTERS_AND_CERTS}}`, `{{DATA_CENTERS_SOURCE}}`, `{{DATA_CENTERS_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q18: Direct peers (network peering relationships) -- what's the list, where does it come from, and as of when?
- Placeholder: `{{DIRECT_PEERS}}`, `{{DIRECT_PEERS_SOURCE}}`, `{{DIRECT_PEERS_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q19: For the footprint-states fact already given in Q5 -- what's the source and as-of date (for the registry entry specifically)?
- Placeholder: `{{FOOTPRINT_STATES_SOURCE}}`, `{{FOOTPRINT_STATES_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (source / date)
- Required: yes -- source/date, or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q20: NPS claim -- what's the figure, what methodology backs it, where does it come from, and as of when? (this feeds a claim with a history of conflicting public sources -- see brand-voice.md contradiction 3 and the registry's staleness discipline)
- Placeholder: `{{NPS_CLAIM}}`, `{{NPS_METHODOLOGY}}`, `{{NPS_SOURCE}}`, `{{NPS_AS_OF}}`
- Files: `shared/fact-registry.md` (single home; brand-voice and the 03/04 checklists reference the registry row, never the value)
- Type: free text (value / methodology / source / date)
- Required: yes -- value/methodology/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q21: Key testimonials you want the editor to know about -- who said what, where does it come from, and as of when?
- Placeholder: `{{KEY_TESTIMONIALS}}`, `{{TESTIMONIALS_SOURCE}}`, `{{TESTIMONIALS_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q22: Procurement vehicles (state contracts, GSA schedules, cooperative purchasing agreements) -- what's the list, where does it come from, and as of when?
- Placeholder: `{{PROCUREMENT_VEHICLES}}`, `{{PROCUREMENT_VEHICLES_SOURCE}}`, `{{PROCUREMENT_VEHICLES_AS_OF}}`
- Files: `shared/fact-registry.md`
- Type: free text (value / source / date)
- Required: yes -- value/source/date, an explicit "none claimed", or coverage via Q13's fact sheet
- Default: none -- REQUIRED, must come from setup

### Q23: How many HOCs (higher-order concerns) should the edit letter cap at per round?
- Placeholder: `{{HOC_CAP}}`
- Files: `shared/concern-definitions.md` (single home; the 08 references point to it)
- Type: free text (number)
- Default: 3

### Q24: Who's the legal escalation contact -- the person or team the editor should name when it flags a suspected legal or regulatory issue for review? (name, title, or an email/alias is fine)
- Placeholder: `{{LEGAL_CONTACT}}`
- Files: `shared/mechanics-standard.md`
- Type: free text
- Default: Legal/Compliance team

### Q25: What should the editor call you -- the name it uses when it addresses you in feedback?
- Placeholder: `{{WRITER}}`
- Files: `brand-vault/identity.md` (single home; every other file says "the writer")
- Type: free text
- Default: not named

### Q26: The mechanics authority hierarchy defaults to AP Stylebook for public-facing copy, with Microsoft's guide as a supplementary authority for product/technical content and Chicago for designated long-form editorial pieces. Keep this default?
- Type: yes/no
- If YES: no changes needed -- `shared/mechanics-standard.md` already reflects this.
- If NO: note the requested authority and flag `shared/mechanics-standard.md` for manual edit. The authority ranking is hardcoded reference content (only the legal-contact name in it is a placeholder) -- the agent cannot template a style-authority hierarchy change from a single answer, so it surfaces the request instead of silently rewriting the ranking.

### Q27: Do you have a brand voice document (voice guide, messaging framework, tone guidelines)? If yes, share it or paste its contents and skip Q28-Q30 for anything it covers -- the agent maps its content into the setup-owned sections of `brand-vault/brand-voice.md` (see the strata note at the top of that file). Any section the document doesn't cover keeps its shipped B2B-fiber category default.
- Type: free text or file reference
- Default: no voice document -- answer Q28-Q30

### Q28: Core voice -- give 2-4 adjectives and one example sentence that sounds unmistakably like the brand.
- Section: `brand-vault/brand-voice.md`, Core Voice (content replacement within the section, not a placeholder)
- Type: free text (adjectives + example sentence)
- Default: keep the shipped default (Plainspoken. Confident. Real. -- partner-not-vendor, outcomes over features)

### Q29: Messaging pillars -- up to four themes every piece should anchor in at least one of.
- Section: `brand-vault/brand-voice.md`, Messaging Pillars (content replacement within the section)
- Type: free text (list)
- Default: keep the shipped default (Reliability, Simplicity, Ownership, Support)

### Q30: Words and phrases to use, and words to avoid. Concrete examples beat descriptions -- give the actual phrases.
- Section: `brand-vault/brand-voice.md`, Words to Use / Words to Avoid (content replacement within the sections)
- Type: free text (two lists)
- Default: keep the shipped defaults

### Q31: How much edge should the editor's feedback voice carry by default -- straight (no wit), dry (restrained wit), or sharp (open snark, always at the copy's expense, never yours)?
- Placeholder: `{{TONE_DIAL_DEFAULT}}`
- Files: `shared/feedback-voice.md` (Tone Dial section -- single home for the definition and the deployment default; the per-piece value lives in each brief)
- Type: one of: straight / dry / sharp
- Default: dry

---

## After Onboarding

1. Assemble the answers into `brand-vault/identity.md`, `brand-vault/brand-voice.md`, and `shared/fact-registry.md`.
2. Voice mapping (Q27-Q30): replace content within the setup-owned sections of `brand-vault/brand-voice.md` only, per the strata note at the top of that file. Any section the answers don't cover keeps its shipped category default. Preserve the register-default line in Core Voice (it defers to the audience model). Never rename, remove, or reorder sections -- stages load them by name.
3. Conditionals in the method-invariant sections:
   - Q12 answered "no standing tagline": collapse Brand-vs-Research contradiction 1 to a one-line N/A ("No brand-mandated consolidation tagline; no tension to carry") and drop the tagline reference from the Go-To Messaging Patterns Ownership bullet.
   - Q20 answered with no NPS claim: collapse contradiction 3 to a one-line N/A and set the registry's NPS row value to "none claimed."
   - Any other Q14-Q22 fact answered "none" / "not used": set that registry row's value to "none claimed" and its source and as-of cells to "--". The row stays; the fact is explicitly unclaimed, not silently absent.
4. Show the user the assembled identity block, the full `brand-voice.md`, and the fact registry table (values, sources, as-of dates -- all still status "stale" pending the writer's verification). This catches misheard names, wrong compliance pairings, and misfiled source citations before they are baked in. Let them correct anything before it's written; only proceed to replacement after they confirm or correct.
5. On confirmation, replace every placeholder across all files listed above.
6. Collapse unused multi-slot placeholders to the count actually supplied: fewer than four verticals -> delete the unused rows from identity.md's verticals table; fewer than three competitors -> the registry's Competitive set row and the failure-modes worked-example prose carry only the names given (single-name deployments collapse the example's two-name comparison to one). No slot may survive setup unresolved.
7. Scan the entire workspace for any remaining unresolved double-brace placeholder, excluding this questionnaire (which documents them). If any remain, ask for the missing info.
8. Tell the user: setup is complete, every piece now runs through `stages/01-intake/CONTEXT.md`, and the `facts` trigger opens the registry any time they want to verify a stale or disputed entry.
