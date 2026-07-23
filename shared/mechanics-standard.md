# Mechanics Standard and Style Authority Hierarchy

The precedence order for every editorial judgment. Higher entries win conflicts. The LOC batch note cites the governing authority by name and rule for each finding.

## Authority Hierarchy

| Rank | Authority | Where it lives |
|------|-----------|---------------|
| 1 | Applicable law and regulatory guidance | External. The editor FLAGS suspected legal/regulatory issues for escalation to {{LEGAL_CONTACT}}; it never rules on them |
| 2 | Approved facts, claims, and product source of truth | `fact-registry.md` (this folder) |
| 3 | Campaign brief and audience definition | The piece brief from 01-intake |
| 4 | Brand positioning and messaging architecture | The positioning method (05-differentiation; cited by name, not loaded) + declared positioning in `../brand-vault/identity.md` |
| 5 | Brand voice and content standards | `../brand-vault/brand-voice.md` |
| 6 | Channel-specific rules | `format-presets.md` (this folder) |
| 7 | AP Stylebook | External. Default mechanics authority for public-facing copy |
| 8 | Microsoft Writing Style Guide | External. Supplementary authority for digital product and technology content |
| 9 | Chicago Manual of Style | External. Designated long-form editorial content only |
| 10 | Merriam-Webster's Collegiate Dictionary | External. Spelling and usage arbiter |
| 11 | WCAG and plain-language guidance (PlainLanguage.gov) | External. Accessibility and plain-language decisions |
| 12 | Documented editorial judgment | `../stages/08-feedback/references/judgment-calibration.md` |

## Policy Statement

Marketing content follows the approved brief, messaging architecture, `brand-vault/brand-voice.md`, and applicable legal and regulatory requirements. Unless a channel-specific standard provides otherwise, public-facing copy follows AP style and Merriam-Webster's Collegiate Dictionary. Designated long-form editorial publications follow Chicago. Digital product and technology content uses the Microsoft Writing Style Guide as a supplementary authority. Accessibility decisions follow applicable WCAG guidance. In all conflicts, legal requirements, factual accuracy, approved claims, and explicit brand standards take precedence over external style authorities.

## Per-Format Authority Declaration

The authority set for a piece follows from the brief's declared format via the table below -- the LOC note derives it; passes never guess.

| Format | Mechanics authority set |
|--------|------------------------|
| Product/vertical page, ad, email, press release, analyst briefing | AP + Merriam-Webster (+ Microsoft for product/technology UI or spec content) |
| Blog / thought leadership | AP + Merriam-Webster by default; Chicago when the piece is designated long-form editorial |
| All formats | WCAG + plain-language checks apply |

## Conflict Handling

1. A finding grounded in ranks 1-6 always outranks a style-authority finding (ranks 7-11).
2. When two external authorities disagree, the declared authority set for the piece wins; if both are declared, the higher rank wins.
3. A style-rule application that damages clarity for the profiled audience yields to documented editorial judgment (rank 12) -- record the judgment and its reason in the note.
