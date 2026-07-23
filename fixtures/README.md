# Fixtures — Demo Quick Start

**Human-facing. Agents: see CONTEXT.md — do not load this file in a run.**

This folder holds everything needed to demo or test the editor without real client data. The brand is **Lightower Fiber Networks** — a real fiber provider that was acquired by Crown Castle in 2017 and dissolved, chosen so the demo implicates no live business. All brand facts are public record.

Contents:
- `lightower-brief.md` — setup input (fact sheet + voice document + all direct answers)
- `product-page.md`, `social-post.md`, `blog-intro.md` — test drafts, each with known defects

## How to run a demo

**1. One-time setup.** In a fresh session at the workspace root, paste:

```
setup — I have a prepared fact sheet and voice document: fixtures/lightower-brief.md. Use it to answer every setup question it covers (direct answers, Q13 fact sheet, Q27 voice document, config). It should cover everything; only ask me for anything it genuinely does not answer.
```

When the agent shows you the assembled identity block, competitor set, and fact registry for review, confirm (or correct) and let it finish. Setup runs once; after that every session goes straight to reviews.

**2. Run a draft through the pipeline.** Paste any of these:

Product page:
```
New piece for review: fixtures/product-page.md. Goal: generate qualified enterprise leads for the optical encryption service. Audience: enterprise IT and security directors in regulated verticals. Format: web product page. Tone dial: dry.
```

Social post:
```
New piece for review: fixtures/social-post.md. Goal: drive webinar registrations. Audience: enterprise IT decision-makers on LinkedIn. Format: LinkedIn company post. Tone dial: dry.
```

Blog intro:
```
New piece for review: fixtures/blog-intro.md. Goal: thought-leadership traffic and newsletter signups. Audience: network architects and IT leaders in financial services. Format: blog post introduction. Tone dial: dry.
```

**3. Read the review sheet** in `pieces/[slug]/r1-review.md`: Verdict, Edit Letter, Ledger, LOC batch.

Notes:
- Each draft contains known defects at both HOC and LOC levels — the review sheets should surface them.
- The editor diagnoses; it never rewrites. If a demo asks it to fix the copy, it should decline and point at the diagnosis.
