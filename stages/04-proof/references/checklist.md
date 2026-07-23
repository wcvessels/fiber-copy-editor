# Proof Checklist

The editor diagnoses missing or misplaced proof. It never inserts evidence on the writer's behalf -- it flags the gap or queries the source.

## Evidence Adjacency

- What evidence appears nearest to the strongest claim on this page? If the strongest claim has no evidence within the same section, flag as **unsupported claim**.
- Does each feature mentioned answer "so the buyer can ___"? If a feature is listed with no attached consequence, flag as **feature without stakes**.
- Is a testimonial or customer quote being used as proof of the specific thing the page claims, or as generic praise that could apply to anything? Flag generic-praise testimonials as **proof mismatch**.
- Are quantitative claims (uptime figures, peer counts, latency numbers, satisfaction scores) placed next to the claim they support, or buried in an unrelated section where the reader cannot connect them?

## Registry Consistency

- Are the network, scale, or company figures on this page (route miles, location counts, customer counts, data center counts) consistent with the same figures elsewhere on the site or in other recently reviewed pages?
- If two figures conflict, is this flagged as a **registry inconsistency** rather than silently resolved by picking one? See the verification-duties reference in this stage for how to handle this.
- Is any figure stated with a different level of precision in different places (e.g., a round number in one spot, an exact figure in another) that suggests one of them is stale?

## Cert-to-Named-Risk

- If the page lists a compliance certification (HIPAA, PCI DSS, SOC 2, CJIS, ITAR), does the copy connect it to the specific risk it mitigates for this buyer -- audit exposure, breach penalty, procurement eligibility, criminal-justice data handling -- or is it presented as an unexplained acronym in a list? Flag as **orphaned certification**.
- If multiple certifications are listed together, does each one map to a different buyer fear, or are they flattened into one undifferentiated badge row? Flag as **badge wallpaper** if the copy cannot say which cert answers which fear.
- For a regulated-vertical page, does the certification list appear where the buyer is deciding, or is it demoted to a footer where it does no persuasive work?

## Testimonial Use

- Does the testimonial prove the specific claim the surrounding copy makes, or is it doing work the body copy should be doing itself (e.g., a testimonial about local support standing in for a claim the page never states directly)?
- Is the testimonial specific and attributable, or vague and unattached to a checkable circumstance? Flag vague or unattributed testimonials.
- Is the testimonial placed where the relevant decision actually happens on the page, or dropped in a generic praise block disconnected from the claim it should support?

## Fact-Discipline Pass

- Extract every statement this page presents as fact -- numbers, dates, names, capabilities, comparisons. Has each one been verified, or is it sitting on the page unverified?
- Does any claim use exaggeration as a substitute for evidence -- inflated counts, minimized effort ("quick," "simple," "seamless" for something not shown to be so), or an unsubstantiated superlative ("best," "fastest," "most powerful," "award-winning")? Flag each as an exaggeration finding.
- Is any cited study, statistic, or external claim missing a source or link? Flag as missing attribution.
- Are empty intensifiers ("truly," "incredibly," "the ultimate") standing in for a concrete, checkable capability? Flag for the writer to replace with something specific.
- Is there a claim that sounds appealing but, on inspection, is not exactly true? Flag it regardless of how minor -- this is where trust erodes fastest in high-consideration B2B copy.

## Unverifiable-Number Queries

- Does this page state a comparative or percentage figure (NPS comparisons and similar percent-better claims) without an absolute number, baseline, source, or date? Query the writer for the missing anchor rather than assuming the number is false.
- Is a network or scale statistic present without a stated as-of date? Flag as stale-risk and query freshness.
- Does a claim depend on a source the editor cannot access (internal research, a named but unlinked study)? Flag as unverifiable and route per the verification-duties reference -- do not silently pass it and do not silently reject it.
