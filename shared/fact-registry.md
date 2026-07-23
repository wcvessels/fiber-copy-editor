# Fact Registry

## What This Is

The registry is the workspace's source of consistency, not a source of truth. It exists so that every piece of copy citing a company fact cites the same value the last piece cited -- not so that the value itself is guaranteed correct. Verifying a fact against reality is the writer's job, done outside this pipeline. The registry's job is to make sure copy never contradicts itself, contradicts the footer of the same page, or contradicts last quarter's press release.

04-proof checks every draft claim against this registry. A match is silent. A mismatch is a finding. A registry entry that is itself unverified does not get treated as ground truth to correct the draft against -- see staleness discipline below.

## Staleness Discipline

Every entry has a status: **verified**, **stale**, or **disputed**.

- **verified** -- the writer has confirmed this value against a current source since the as-of date.
- **stale** -- seeded but not yet confirmed, or confirmed too long ago to trust without a recheck.
- **disputed** -- two sources disagree and neither has been resolved.

**The rule that matters:** when 04-proof encounters a draft claim that matches a stale or disputed registry entry, the finding is not "this is correct" or "this is wrong" -- it is a query. The pass flags the claim and asks the writer to verify the registry entry, rather than asserting the draft is either right or wrong. Stale entries become queries, not assertions. Only a verified entry can be used to fail a draft claim outright.

**Promotion to HOC:** a draft claim that contradicts the registry outright (a different number for the same fact, with no stale/disputed excuse) is a factual self-contradiction and promotes automatically -- see `failure-modes.md`.

**Maintenance:** the `facts` trigger opens this file for review. The writer (named in `brand-vault/identity.md`, Roles) owns every status change. Entries do not silently age from stale to verified; a human confirms it.

## Registry

| Fact | Value | Source | As-of | Status |
|---|---|---|---|---|
| Route miles | {{ROUTE_MILES}} | {{ROUTE_MILES_SOURCE}} | {{ROUTE_MILES_AS_OF}} | stale |
| Lit / on-net locations | {{LIT_ON_NET_LOCATIONS}} | {{LIT_ON_NET_SOURCE}} | {{LIT_ON_NET_AS_OF}} | stale |
| Serviceable locations | {{SERVICEABLE_LOCATIONS}} | {{SERVICEABLE_LOCATIONS_SOURCE}} | {{SERVICEABLE_LOCATIONS_AS_OF}} | stale |
| Data centers + certifications | {{DATA_CENTERS_AND_CERTS}} | {{DATA_CENTERS_SOURCE}} | {{DATA_CENTERS_AS_OF}} | stale |
| Direct peers | {{DIRECT_PEERS}} | {{DIRECT_PEERS_SOURCE}} | {{DIRECT_PEERS_AS_OF}} | stale |
| Footprint states | {{FOOTPRINT_STATES}} | {{FOOTPRINT_STATES_SOURCE}} | {{FOOTPRINT_STATES_AS_OF}} | stale |
| NPS claim + methodology | {{NPS_CLAIM}} ({{NPS_METHODOLOGY}}) | {{NPS_SOURCE}} | {{NPS_AS_OF}} | stale |
| Key testimonials | {{KEY_TESTIMONIALS}} | {{TESTIMONIALS_SOURCE}} | {{TESTIMONIALS_AS_OF}} | stale |
| Procurement vehicles | {{PROCUREMENT_VEHICLES}} | {{PROCUREMENT_VEHICLES_SOURCE}} | {{PROCUREMENT_VEHICLES_AS_OF}} | stale |
| Competitive set (paste-test names) | {{COMPETITOR_1}}, {{COMPETITOR_2}}, {{COMPETITOR_3}} | setup questionnaire (Q11) | {{SETUP_DATE}} | stale |

Add rows as new fact types recur across pieces. One row per discrete fact -- do not bundle unrelated numbers into a single cell beyond what is shown above.
