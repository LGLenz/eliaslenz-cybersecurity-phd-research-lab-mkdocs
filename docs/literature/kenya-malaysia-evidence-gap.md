# Kenya & Malaysia evidence gap and targeted search strategy

## Why this page exists
Your current literature mapping is rich for **Germany/UK governance and Policy‑as‑Code (PaC) practice**, but Kenya/Malaysia evidence is thinner. This is normal and defensible, as long as the gap is **explicitly declared**, and your strategy for closing it is **transparent, repeatable, and auditable**.

This page turns the gap into a method: a documented search and screening protocol you can cite in your thesis as part of your **systematic/comparative approach**.

## Gap statement (what is currently missing)
### Kenya
- Public-sector cloud migration governance details (decision rights, procurement constraints, sovereignty posture)
- Operational cloud security control baselines (IAM, logging, key management, network segmentation) documented in public standards/guidance
- Evidence of PaC/guardrails adoption (e.g., OPA/Gatekeeper, Terraform policy testing, cloud landing zones) in government or heavily regulated sectors

### Malaysia
- National/public-sector cloud governance models, especially around data residency, classification, and assurance
- How regulators and ministries operationalise continuous compliance and audit evidence in cloud
- Concrete tooling evidence for PaC guardrails and platform governance

## Targeted search protocol (repeatable)
### Databases (primary)
- Google Scholar
- IEEE Xplore
- ACM Digital Library
- Scopus / Web of Science (if access available)

### Government / regulator sources (secondary, labelled “grey”)
Kenya (examples of likely starting points):
- ICT Authority / eGovernment directorates
- Data Protection Commissioner / data protection guidance
- National cybersecurity strategy / CERT guidance

Malaysia (examples of likely starting points):
- MAMPU (public sector modernisation)
- National Cyber Security Agency (NACSA)
- Personal Data Protection Act guidance (PDPA), sector regulators

> Grey sources are acceptable when (a) they are authoritative, (b) peer‑reviewed work is scarce, and (c) they are clearly labelled and triangulated.

## Search strings (template)
Use combinations of:

- (“policy as code” OR guardrails OR “continuous compliance” OR “infrastructure as code” OR OPA OR gatekeeper OR terraform) AND (Kenya OR Malaysia) AND (government OR “public sector” OR regulator)
- (“cloud migration” OR “cloud adoption”) AND (governance OR “landing zone” OR “shared responsibility”) AND (Kenya OR Malaysia)
- (“cloud security” AND audit AND (Kenya OR Malaysia))  
- (“data residency” OR sovereignty OR “data localisation”) AND cloud AND (Kenya OR Malaysia)

## Screening & selection criteria (defensible)
### Include
- Published ≤ 6 years where possible (older only if canonical)
- Direct relevance to: cloud migration governance, controls, assurance, PaC/guardrails, training/skills
- Clear sector context (public sector preferred; regulated sectors acceptable)

### Exclude
- Purely vendor marketing with no operational detail
- Generic “cloud is good” papers without governance/control implications
- Sources without verifiable provenance (no author/organisation/date)

## Verification steps (security-by-design)
- **Default‑deny mindset:** treat governance claims as hypotheses until verified by at least two sources.
- **Provenance check:** confirm author/org legitimacy, publication date, and document integrity.
- **Cross‑jurisdiction mapping:** map each claimed control/guideline to your baseline (e.g., ISO 27001/27002, NIST 800‑53, or BSI where applicable) and note deltas.

## Output format (so you can analyse later)
Every candidate source becomes a row in the capture template CSV with:
- bibliographic data, sector, jurisdiction
- relevance to RQ1.1–RQ1.4
- evidence type and strength rating
- extracted governance/control statements (with quotes limited)

Next page: **Kenya/Malaysia capture template**.
