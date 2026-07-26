# Sample Review Sheet

Real output, not an illustration. This is the unedited sheet the editor produced for `fixtures/product-page.md`, using the brief in `fixtures/lightower-brief.md` and the prompt in `fixtures/README.md`. Run it yourself and you should get something close.

Two things to notice. Nothing in it is a rewritten line -- every finding is a diagnosis and a question handed back. And the Status field reads `open` rather than `finalized`, because no writer was present to clear the curate gate at 08; the editor declined to record an acceptance that did not happen.

The verdict is `developmental`, which is correct for this draft: the page has problems a copy pass cannot reach. That is the escalation path working, not the editor being harsh.

---

# Review Sheet -- optical-encryption-services -- Round 1
Date: 2026-07-26  |  HOC count: 12  |  Status: open

## Verdict
developmental

Set at 04-proof, when the round's HOC count passed the cap of 3. The gauntlet ran in full regardless. Two of the escalation triggers in `edit-letter-format.md` are also live: the differentiation pass found no ownable position anywhere on the page, and the defects in the proof layer are the reputational kind, not the polish kind.

## Edit Letter

**What this is.** A diagnose-only round: findings, not rewrites. Nothing below contains a replacement line, and nothing will. Items are marked Required or Open at the end. The verdict is provisional in exactly one sense -- it is a verdict on this draft, not on the piece, and the piece is recoverable.

**Where the draft stands: developmental.** That means the next move is a strategy pass, not a copy pass. It is not a statement about the writing, which is competent and in places better than that. It is a statement about what the page is currently built to do versus what the brief says it exists to do, and those two things have come apart.

**What's working -- and it is load-bearing, not softening.**

- Line 5, second sentence: "a single exposed fiber path can put customer records, trade data, and regulated information at risk the moment it leaves the building." That names the failure event, the asset at risk, and the moment it happens. Most pages in this category open on the product; this one opens on the reader's exposure, which is the correct order for a product page and the harder thing to write.
- Lines 7 and 9 position against the reader's real alternatives -- encrypting up at Ethernet or IP, and buying and running encryptor hardware -- rather than against a rival the buyer has never evaluated. The competitive-alternative test is the one most pages in this category flunk outright. This page passes it.
- The mechanism paragraph keeps its technical density (Layer 1, data agnostic, protocol overhead) instead of vaguing down. For an operator-to-specialist reader that is a credibility signal, and the restraint not to simplify it was the right call.

**Boundary line: the standing above is settled. Everything from here is coaching.**

**Problem summary.** Three things drive most of the twenty findings in the Ledger. The page has no lead ask -- its only request is a social follow, on a page whose stated job is generating qualified enterprise leads. The proof layer does not survive the reader who is paid to check it: the central certification claim is misstated and unsourced, the certs are never tied to the regimes this reader is audited against, and the one customer quote is about bandwidth. And nothing asserted on the page is actually Lightower's -- the differentiation is category language, and the assets the brand vault says are hardest to copy are either buried or absent.

**Feasibility.** Two of the three are reachable inside the existing material: the vault and the registry already hold what the proof and differentiation sections need, once the facts are verified. The first is not -- there is no offer or destination on this page to point a real CTA at, which makes it a brief question rather than a copy question.

---

### HOC 1 -- The page cannot produce the lead it exists to produce. [07 cta] [COACHING]

**Location.** Line 30, under the heading "Get Started": "Ready to make encryption a cornerstone of your network strategy? Follow Lightower on LinkedIn and X for the latest updates."

**Evidence.** The heading promises a path. The rhetorical question sets up a purchase-readiness ask. What arrives is a social follow. There is no form, no assessment, no briefing, no spec request, no contact route anywhere on the page.

**Mechanism.** The brief's goal is qualified enterprise leads. A social follow captures nothing and qualifies nobody, so the page has no mechanism for producing its stated output. Separately, the CTA is far too small for what precedes it: an evaluating security director who has just read a compliance-risk argument and a certification list is being offered a feed. The gap between the weight of the case and the weight of the ask reads as the page losing its nerve at the end.

**Path forward -- escalation, not a line edit.** This is a scope decision before it is a copy decision. What is the actual next step this page is allowed to offer, and does it exist yet. Until that is answered, no CTA wording can be evaluated.

**Target effect.** A reader who has just decided this is worth a conversation should find, at the bottom of the page, the specific low-commitment step that starts one -- and should be able to tell what happens after the click before clicking.

### HOC 2 -- The proof layer does not survive an audit-minded reader. [04 proof] [COACHING]

Three locations, one pattern. This reader's entire job is verifying claims like these before signing.

**2a. Line 13: "NIST-compliant AES-256 encryption, FIPS 104-2 and FIPS 197 certified."** The designation "FIPS 104-2" does not resolve to anything the workspace can match -- and the fact registry's certifications row currently reads "facility certifications: none claimed," so there is no entry backing any FIPS certification at all. This is the page's central proposition, sitting on nothing checkable. "NIST-compliant" has the same problem in a smaller way: NIST is an agency, so the phrase does not name a standard anyone can look up. Query, not a correction -- the editor does not supply the number. Which publication is the certification actually against, who holds it, and can it get a verified registry row before this page ships.

**2b. Lines 23-26.** The introducing line claims "Customers across regulated industries rely on Lightower's optical encryption service." The quote that follows is from a university -- not one of the three verticals the page named at line 5 -- and it is about scaling bandwidth and network performance. It does not mention encryption, security, compliance, or this service. The registry confirms it is logged as a general product-page testimonial, status stale. As proof it is doing no work; as generic praise under a specific claim it actively undercuts the claim above it. Does a customer quote exist that speaks to the encryption service, or does the header need to narrow to what the available proof can carry.

**2c. Line 13 against line 5.** The page names finance, healthcare, and government at line 5. Per the brand vault those carry SEC/FINRA, HIPAA, and CJIS. None of those three appears anywhere on the page. What appears instead is a row of federal cryptographic standards, which are not the regimes this reader is examined against, presented with no consequence attached to any of them. Orphaned certification, and badge wallpaper where the certs are flattened into one undifferentiated row. Which fear is each cert answering for which of the three named verticals -- and if the page cannot say, is it carrying three verticals it cannot serve.

**Path forward.** Required, and it starts outside the copy: run the `facts` trigger, get the certification and the network figures to verified status, then revise. A targeted rewrite prompt the writer executes -- not a restructure.

**Target effect.** Every claim on this page that a compliance officer would check should have something adjacent that survives the check, and every cert should carry the specific consequence of failing it for a named vertical.

### HOC 3 -- Nothing asserted here is Lightower's. [05 differentiation] [COACHING]

**Location.** Line 21, "The combination of Layer 1 encryption and dedicated wavelengths deliver security without compromise." Also the header at line 11 and the bullets beneath it. Also the treatment of the network at lines 17 and 21.

**Evidence.** Substitute either name from the registry's competitive set into line 21 and nothing about the sentence becomes untrue. "Security without compromise" is category language with better rhythm. Under a header that promises reasons to choose *Lightower* specifically, four of the five bullets -- speeds, zero latency impact, no hardware, AES-256 -- are things any Layer-1 encryption provider publishes unchanged. The owned network appears twice, both times below the fold and both times framed as background rather than as part of the security argument. The regional density figures at line 21 are stated as raw scale with no consequence attached for someone buying encryption. And the differentiator the vault calls out first -- 80% of staff in care and engineering, the recurring support award, the local NOC -- does not appear on the page at all.

**Mechanism.** This reader is comparing three or four providers who all have FIPS-certified optical encryption. A page made entirely of things all of them can say gives the champion nothing to bring to the comparison, and gives the signer no reason to prefer this one.

**Path forward.** Strategy pass, not a line edit. The material exists in `brand-vault/identity.md`; the page does not use it.

**Target effect.** At least one claim on the first screen that a competitor could not paste onto their own page without it becoming false.

---

**LOC batch.** Seven sentence-level findings are consolidated into a single note below, kept out of this list deliberately -- mixing scales buries the three problems above under punctuation. An eighth LOC-tagged finding (Ledger 2) is carried as a marginal note instead, because the problem there is meaning rather than mechanics. One further item was promoted out of the batch and into the Ledger as an HOC: the misspelling at line 21 sits inside the sentence carrying the page's network proof, on a page selling certified security. That is the promotion rule doing its job, not a comment on proofreading.

**Everything else.** Twenty findings were logged this round; three are named above. The rest are in the Ledger below, in run order, none dropped. The triage was by business impact, and the cut is visible rather than silent.

**Required before the next round.**

- The certification designation and its source, resolved and registered (Ledger 5).
- The data-center figure reconciled against a single source of truth, and the registry rows behind the network stats moved off stale or the figures pulled (Ledger 8).
- A decision on what this page's actual conversion step is (Ledger 12).
- The misspelling at line 21 (Ledger 13).

**Open -- writer's call.**

- Whether the four fragments at line 5 come out or get reworked (Ledger 1).
- Whether the testimonial is replaced or the claim above it narrowed to fit (Ledger 6).
- Where the proof block sits (Ledger 11).
- The entire LOC batch.

**Routing.** This needs a scope decision on the conversion path before another diagnostic round runs. The other two problems are workable inside the existing material.

**Close.** The opening of this page is better than the page. The stakes sentence, the framing against higher-layer encryption, and the decision to keep the technical density are all correct calls, and they are the parts that are hardest to produce. What is missing is the evidence layer and the ask -- both of which are supply problems more than writing problems. Worth a read back on whether the conversion-path question is answerable before the next round, since everything at HOC 1 waits on it.

**Curate gate.** The 08 checkpoint was not cleared -- no writer was available to accept, edit, or send a pass back. Status stays `open` for that reason and that reason only.

## Marginal Notes

Held to findings that survive a strategy change, per the developmental verdict. Notes tied to material a strategy pass may delete were logged in the Ledger and left there.

**M1 -- Line 5: "Easy. Affordable. Secure. Full Control."** Named failure: consumer-register-on-B2B. [COACHING] The four fragments close a paragraph that has just put customer records, trade data, and regulated information at risk. Read as data: three of the four are unanchored adjectives and the fourth prices the decision. Read as effect on this reader: "Affordable" argues on the axis a security director in a regulated vertical is least able to defend upward -- a compliance officer does not approve encryption because it was reasonably priced -- and the staccato ad rhythm sits against the seriousness of the two sentences before it. This is the one line on the page the champion would have to skip past on the way to the signer. What does the first screen need to say about the decision this reader is actually making, and does anything in these four words say it?

**M2 -- Line 9: "End users maintain total control over the most important parts, their own security parameters and security keys."** Named failure: curse-of-knowledge, internal lingo with two live readings. [COACHING] "End users" is telco-internal shorthand for the customer organization. Outside the building it more commonly means the customer's employees. Both readings are available here, and they describe opposite security postures: the buying organization holding key material is the reassurance intended; staff holding key material is a finding in an audit. Key custody is the first question this reader asks about any encryption service, so the sentence that answers it cannot support two answers. Which party holds the keys, and does the sentence name that party in a way a compliance reviewer could not misread?

**M3 -- Line 16: "Zero impact on latency or throughput," against line 7: "our Layer 1 approach adds zero protocol overhead."** Named failure: claim exceeds its own evidence. [COACHING] The body claims zero protocol overhead. The bullet promotes that to zero impact on latency. Those are not the same claim -- overhead is a framing cost, latency is what the encryption engine adds -- and this page's reader is technical enough to know the difference. On first read the bullet lands as the stronger version of a claim the body only supports in its weaker form, which is the pattern that makes a specialist start discounting everything else in the list. What measurement backs the latency half specifically, and if there isn't one, does the claim need to narrow to what line 7 already earns?

**M4 -- Line 21: "32,000+ route miles connecting more than 350 data centers."** Named failure: registry inconsistency, raised as a query. [COACHING] The registry's data-center row reads "275+ connected data centers." This page reads "more than 350." The editor is not picking between them -- the registry row carries status stale, dated 2017-04, and a stale row cannot fail a draft claim. Both figures are cited here so they can be reconciled against one source rather than resolved by whichever page was written most recently. The route-mile figure matches the registry exactly but that row is stale too, and the Fortune 500 percentage in the same sentence has no registry row at all. For a reader who checks claims before signing, a number that disagrees with the company's own record is a bigger problem than a number that is merely old. Which figure is current, and can all three carry a verified row before this page ships?

**M5 -- Line 7: "Operating at Layer 1, the Physical Layer, the encryption is data agnostic, while maximizing network throughput by eliminating the encryption headers used at higher layers like Ethernet or Internet Protocol."** [APPRECIATION] The move that works: this positions the service against what the reader would otherwise actually do -- encrypt further up the stack -- rather than against a named rival, and it does so by naming the specific cost of the alternative. Most copy in this category asserts superiority against a competitor the buyer has never shortlisted. Line 9 then does the same thing again against the other real alternative, buying and running the hardware. That is two of the three genuine alternatives handled in three sentences, and it is the reason the mechanism paragraph reads as a serious argument rather than a spec dump. The move is named-alternative-before-claimed-advantage, and it is repeatable. The third alternative for this reader is doing nothing until the next audit forces the question -- where on the page could that one get the same treatment these two got?

## LOC Batch

One consolidated cleanup pass. Authority set for this format per `mechanics-standard.md`: AP Stylebook and Merriam-Webster, with Microsoft Writing Style Guide supplementary for the technical content, plus plain-language checks. Sentence-level work belongs after the structure settles -- given the developmental verdict, treat this batch as a hold-for-later list rather than this week's task.

1. **Line 5, "Encryption of in-flight data should be a cornerstone of every organization's security strategy."** ABSTRACT SUBJECT and THROAT-CLEARING. The subject slot holds a process, not a character, and the sentence's job is to warm up for the one after it -- which is the sentence that actually has the stakes in it. The reader meets the page's best line second. Direction: front-load, and check whether the opener is doing work the second sentence does not already do better.
2. **Line 7, "utilizes revolutionary technology to offer FIPS-certified encryption."** PHRASE BLOAT. Merriam-Webster carries a shorter form of the verb with no loss of meaning; the longer one is doing register work, not semantic work. (The adjective in the same phrase is logged separately as an HOC -- it is a claim problem, not a word-choice problem.)
3. **Line 7, "Encryption shouldn't slow your network down, our Layer 1 approach adds zero protocol overhead."** Comma splice -- two independent clauses joined by a comma. AP, rank 7 in the authority hierarchy. Direction: repunctuate or resegment; the fix does not change meaning either way.
4. **Line 7, "from end-point to end-point."** One term per concept. Merriam-Webster styles this closed. The page also runs "end users" open in the next paragraph, so the compound styling is drifting within four lines. Direction: pick one styling and enforce it across the page.
5. **Line 9, "Since Lightower offers Optical Encryption as a service, there is no need to purchase, deploy, and manage equipment."** SLOW START plus DELETED DOER. A ten-word introductory clause holds the main clause in memory, and the main clause then opens on "there is," which strands the reader without a party -- no need for whom. Direction: give the clause a doer and shorten the runway.
6. **Line 9, "total control over the most important parts, their own security parameters and security keys."** Punctuation: an appositive attached with a comma where the grammar wants a stronger mark, which is why the sentence reads as a splice. AP. The vagueness of "the most important parts" is handled in M2 as a meaning issue, not here.
7. **Line 21, "The combination of Layer 1 encryption and dedicated wavelengths deliver security without compromise."** Subject-verb disagreement -- the simple subject is "combination," singular. AP and Merriam-Webster. Considered for promotion under the promotion rule and held at LOC: it is a visible slip but not a claim-bearing one, and the promoted item this round is the certification designation. Noted here so the call is visible rather than assumed.
8. **Heading capitalization, lines 11, 19, 28.** Consistent title case throughout. Recorded as a reasoned leave-alone, not a gap in the pass.

Two further leave-alones worth recording so they read as decisions rather than misses. The technical vocabulary at line 7 was not flagged as jargon: for an operator-to-specialist reader it is a trust signal, and the audience model is explicit that simplifying it would be the error. The echo of "cornerstone" between line 5 and line 30 was not flagged either -- a closing callback to the opening frame is a deliberate device doing structural work, and the problem at line 30 is what follows the question, not the question.

## Ledger
| # | pass | anchor | HOC/LOC | failure mode | diagnosis + hand-back question |
|---|------|--------|---------|--------------|--------------------------------|
| 1 | 02 audience-fit | Line 5, "Easy. Affordable. Secure. Full Control." | HOC | consumer-register-on-B2B | Four consumer-ad fragments close the paragraph that establishes regulatory exposure; "Affordable" argues on the axis this reader can least defend to a compliance signer, and the ad rhythm flattens the two sentences before it. What does the first screen need to say about the decision this reader is making, and do these four words say any of it? |
| 2 | 02 audience-fit | Line 9, "End users maintain total control ... their own security parameters and security keys." | LOC | curse-of-knowledge; internal lingo, two readings | "End users" reads as the customer organization inside telco and as the customer's staff outside it; the two readings describe opposite key-custody postures on the one question this reader asks first. Which party holds the keys, and does the sentence name that party unambiguously? |
| 3 | 03 claims | Line 3, "for the Ultimate in Security and Efficient Management"; line 7, "revolutionary technology" | HOC | unanchored adjective, two instances | Both are superlatives with no basis stated and no mechanism attached; the technology is never named, so the claim traces down to nothing. The subhead's front half is checkable and its back half is not, which means the only value claim in the headline is the unprovable part -- feature-led ordering with a vague tail. What is the basis for each, and if none can be produced, what does the headline lead with instead? |
| 4 | 03 claims | Line 16, "Zero impact on latency or throughput," against line 7, "adds zero protocol overhead" | HOC | claim exceeds its own evidence | The body supports zero protocol overhead; the bullet promotes it to zero latency impact, which is a different and larger claim, and this reader knows the difference. What measurement backs the latency half, and if there is none, can the claim narrow to what line 7 already earns? |
| 5 | 04 proof | Line 13, "NIST-compliant AES-256 encryption, FIPS 104-2 and FIPS 197 certified" | HOC | unverifiable central claim; promotion rule applies | The designation "FIPS 104-2" resolves to nothing the workspace can match, and the registry's certifications row reads "none claimed," so the page's central proposition has no backing entry. "NIST-compliant" names an agency, not a standard. Editor does not supply a corrected designation. Which publication is the certification against, who holds it, and can it carry a verified registry row before ship? |
| 6 | 04 proof | Lines 23-26, testimonial and its introducing line | HOC | proof mismatch; generic praise under a specific claim | The header claims regulated-industry customers rely on the encryption service; the quote is from a university, names none of the three verticals at line 5, and is about bandwidth scaling rather than encryption or compliance. Registry confirms it as a general product-page quote, status stale. Does a quote exist that speaks to this service, or does the claim above need to narrow to what the available proof carries? |
| 7 | 04 proof | Line 13 bullet, read against line 5's "finance, healthcare, and government" | HOC | orphaned certification; badge wallpaper | The page names three verticals carrying SEC/FINRA, HIPAA, and CJIS per the brand vault, then cites none of them; what appears instead is a flattened row of federal crypto standards with no consequence attached to any one of them. Which fear does each cert answer for which named vertical, and if the page cannot say, can it carry three verticals at once? |
| 8 | 04 proof | Line 21, "more than 350 data centers"; "32,000+ route miles"; "25% of Fortune 500 companies" | HOC | registry inconsistency plus stale-risk; raised as query | The registry reads "275+ connected data centers" against this page's "more than 350." Editor does not pick: the registry row is stale as of 2017-04 and a stale row cannot fail a draft claim. The route-mile figure matches a row that is also stale; the Fortune 500 percentage has no row at all. Which figure is current, and can all three carry verified rows before ship? |
| 9 | 05 differentiation | Line 21, "deliver security without compromise" | HOC | category language | Substitute either name from the registry's competitive set and the sentence stays equally true, which is the paste test failing outright. This sits in the position where the page makes its security argument. What is true of Lightower's encryption here that is not true of the competitive set? |
| 10 | 05 differentiation | Line 11 header and lines 13-17 bullets; line 17; line 21 | HOC | buried differentiator; category claim dressed as company claim | Under a header promising reasons to choose Lightower, four of five bullets are publishable unchanged by any Layer-1 encryption provider. The owned network appears twice, both below the fold and both as background rather than as security argument. Regional density is stated as raw scale with no consequence for an encryption buyer. The vault's first-named differentiator -- 80% of staff in care and engineering, the support award, the local NOC -- is absent entirely. Which ownable asset belongs on the first screen, and what does it let this reader do that the alternatives do not? |
| 11 | 06 structure | Lines 19-26, read against lines 13-17 | HOC | proof isolated from the claims it supports | The page's only two pieces of evidence sit in a terminal block headed as network background, after the reasons-to-believe bullets rather than beside them. The certification claim, the zero-impact claim, and the no-hardware claim each stand with nothing adjacent; the evidence that does exist is adjacent to nothing. Which claim on this page most needs proof standing next to it, and is the current block placed where that reader is deciding? |
| 12 | 07 cta | Line 30, "Ready to make encryption a cornerstone of your network strategy? Follow Lightower on LinkedIn and X for the latest updates." | HOC | CTA-to-goal mismatch; destination mismatch | The brief's goal is qualified enterprise leads; a social follow captures and qualifies nobody, so the page has no mechanism for its stated output. The heading and the rhetorical question set up a purchase-readiness ask and deliver a feed, and the ask is far too small for the compliance case just made. What next step is this page allowed to offer, and does it exist yet? |
| 13 | 08 feedback | Line 21, "Our encryption serivces ride the same all-fiber network" | HOC | misspelling; promoted per the promotion rule | A transposition inside the sentence carrying the page's network proof, on a page selling certified security to readers who verify before signing. Promoted because of where it sits, not because of its size; ranked last for the letter and is a proofing item, not a strategy item. Does the page get a proofing pass against Merriam-Webster before it ships? |
| 14 | 08 feedback | Line 5, "Encryption of in-flight data should be a cornerstone of every organization's security strategy." | LOC | ABSTRACT SUBJECT; THROAT-CLEARING | Subject slot holds a process rather than a character, and the sentence warms up for the stakes sentence that follows it, so the page's strongest line lands second. Does the opener do work the next sentence does not already do better? |
| 15 | 08 feedback | Line 7, "utilizes revolutionary technology to offer" | LOC | PHRASE BLOAT | Longer verb form doing register work rather than semantic work; Merriam-Webster carries the shorter form with no loss. Is the extra length buying anything here? |
| 16 | 08 feedback | Line 7, "Encryption shouldn't slow your network down, our Layer 1 approach adds zero protocol overhead." | LOC | comma splice; AP, rank 7 | Two independent clauses joined by a comma. Repunctuating or resegmenting changes no meaning. Which of the two does the paragraph's rhythm want? |
| 17 | 08 feedback | Line 7, "from end-point to end-point," against line 9, "End users" | LOC | one term per concept; Merriam-Webster styling | Merriam-Webster styles the first compound closed; the page also runs a related compound open four lines later, so the styling is drifting within one screen. Which styling holds across the page? |
| 18 | 08 feedback | Line 9, "Since Lightower offers Optical Encryption as a service, there is no need to purchase, deploy, and manage equipment." | LOC | SLOW START; DELETED DOER | A ten-word introductory clause holds the main clause in memory, and the main clause opens on an expletive that strands the reader without a party -- no need for whom. Who is the doer this sentence is about? |
| 19 | 08 feedback | Line 9, "total control over the most important parts, their own security parameters and security keys" | LOC | appositive punctuation; AP | The appositive is attached with a comma where the grammar wants a stronger mark, which is what makes the sentence read as a splice. Meaning issue handled separately at row 2. Which mark does the sentence need? |
| 20 | 08 feedback | Line 21, "The combination of Layer 1 encryption and dedicated wavelengths deliver security without compromise." | LOC | subject-verb disagreement; AP and Merriam-Webster | Simple subject is "combination," singular. Considered for promotion and held at LOC: visible but not claim-bearing, and the promoted item this round is the certification designation. Recorded so the call is visible rather than assumed. |
