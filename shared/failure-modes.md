# Failure Mode Library

Six recurring failure patterns in B2B fiber/telco marketing copy. Each entry gives the one-question test that surfaces it, a worked example showing the weak line, the editorial note a passing review would leave, and why that note works. Notes diagnose; they never rewrite.

---

## 1. Undifferentiated Reliability Claims

**Feeds:** 03-claims

**Diagnostic test:** Could a competitor paste this exact sentence onto their own site without changing a word? If yes, it differentiates nothing.

**Weak line:** "Our network employs redundant equipment, connections, and power supplies, deployed in a ring architecture, allowing for no single point of failure."

**Editorial note:** "Every provider in this category claims redundancy and no single point of failure -- it's table stakes, not a differentiator. This sentence describes the category, not {{BRAND_NAME}}. What here is true of {{BRAND_NAME}} that is not true of {{COMPETITOR_1}} or {{COMPETITOR_2}}? Until that's answered, flag as undifferentiated."

**Why it works:** Gives a concrete falsification test (the paste test), names the category-vs-brand gap precisely, and hands back a question instead of a rewrite.

---

## 2. Features Without Stakes

**Feeds:** 04-proof

**Diagnostic test:** After each feature, can you answer "so the buyer can ___"? If the consequence is missing, the feature is inert.

**Weak line:** "Dedicated bandwidth, symmetrical connection speeds, low latency, and high capacity are just some of the benefits of our network."

**Editorial note:** "This is a spec list wearing the word 'benefits.' None of the four items connects to a consequence this audience cares about -- symmetrical speed matters to a reader moving large files under deadline pressure, but the copy never makes that leap. Mark each spec as feature-no-stakes and send back with: for this piece's reader, what does each spec let them do or avoid?"

**Why it works:** Names the disguised-spec-list pattern, supplies the so-what test, and ties the fix to the piece's actual profiled reader rather than a generic buyer.

---

## 3. Orphaned Compliance Certs

**Feeds:** 04-proof

**Diagnostic test:** Does this cert connect to the specific bad thing this audience fears -- a fine, a breach headline, a failed audit -- or is it just an alphabet row?

**Weak line:** "Compliance-ready reporting mapped to SOC 2, HIPAA, and PCI-DSS, with full dashboard access."

**Editorial note:** "These certs are stacked but orphaned -- each maps to a different buyer's specific nightmare, and the line ties none of them to it. For this piece's reader, each cert should evoke the exact consequence of failing it, not a checkbox. Flag as certs-without-consequences and note which fear each cert is supposed to address."

**Why it works:** Distinguishes the certs by the distinct fear each addresses instead of treating them as interchangeable, and gives a per-cert repair target without drafting the fix.

---

## 4. Buried Regional Advantage

**Feeds:** 05-differentiation

**Diagnostic test:** Is the hardest-to-copy advantage -- owned regional density, local support -- surfaced where the reader decides, or buried below generic claims?

**Weak line (appears well down the page, under generic peering copy):** "When your business is in crisis, can you really afford to rely on an overseas call center... At {{BRAND_NAME}} we have local technicians in each of our markets."

**Editorial note:** "This is arguably the strongest, hardest-to-copy differentiator {{BRAND_NAME}} has -- local support and an owned regional network -- and it's parked mid-page under generic copy. Customer testimonials confirm this is what actually drives the decision. Why is it not surfaced where the reader decides? Flag as buried differentiator."

**Why it works:** Identifies the specific asset, points to evidence (testimonials) that it drives decisions, and diagnoses a placement problem rather than rewriting the line.

---

## 5. Vendor-Consolidation Cliche

**Feeds:** 05-differentiation

**Diagnostic test:** Is the one-provider promise presented as if it's ours, when it's an industry-wide trope? Does anything make this version specific and provable?

**Weak line:** "One provider. No gaps, no finger-pointing, no vendor chaos."

**Editorial note:** "This phrasing is one of the most worn tropes in B2B tech and telecom -- a category claim any competitor could make as written. What makes the single-provider promise from {{BRAND_NAME}} provable and specific -- the owned network, the one-bill model, a real proof point? Right now the differentiator is asserted, not evidenced. Flag as undifferentiated positioning."

**Why it works:** Proves the phrase is generic, distinguishes assertion from evidence, and points the writer toward the brand's own provable assets without supplying replacement copy. Note: if the exact phrase is brand-mandated (see `brand-voice.md` contradictions), the note flags it for adjacent proof and never recommends striking it.

---

## 6. Factual Self-Contradiction

**Feeds:** 04-proof

**Diagnostic test:** Do the numbers on this page match each other, the footer, other pages, and the fact registry?

**Weak line:** A stat block reads one route-mile figure while the same page's footer reads a different one for the same fact.

**Editorial note:** "This page contradicts itself: the stat block and the footer give two different route-mile figures. This isn't a style issue -- it's a credibility issue with readers who verify claims before they buy. Mark every figure that doesn't match the fact registry and route it back to a single source of truth before publication."

**Why it works:** It's objective and undeniable (the page disagrees with itself), names the audience most sensitive to it, and prescribes a process fix (single source of truth) without inventing a corrected number. This is the promotion-rule case: an LOC-sized error that damages credibility becomes an HOC regardless of size (see `concern-definitions.md`).
